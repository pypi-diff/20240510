# Comparing `tmp/omuplugin_translator-0.2.5.tar.gz` & `tmp/omuplugin_translator-0.3.0.tar.gz`

## Comparing `omuplugin_translator-0.2.5.tar` & `omuplugin_translator-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/src/omuplugin_translator/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/src/omuplugin_translator/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.0/src/omuplugin_translator/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.0/src/omuplugin_translator/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.0/src/omuplugin_translator/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.0/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 omuplugin_translator-0.3.0/PKG-INFO
```

### Comparing `omuplugin_translator-0.2.5/src/omuplugin_translator/plugin.py` & `omuplugin_translator-0.3.0/src/omuplugin_translator/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,100 @@
 from __future__ import annotations
 
 from typing import TypedDict
 
 from edgetrans import EdgeTranslator, Language, Translator
 from loguru import logger
 from omu.identifier import Identifier
-from omuchat import App, Client, content, model
+from omuchat import App, Client, model
 from omuchat.event.event_types import events
+from omuchat.model.content import Component, Root, System, Text
 
-IDENTIFIER = Identifier("cc.omuchat", "plugin-translator")
+IDENTIFIER = Identifier("cc.omuchat", "translator", "plugin")
 APP = App(
     IDENTIFIER,
     version="0.1.0",
 )
 client = Client(APP)
 
 translator: Translator | None = None
 
 
 class TrasnlatorConfig(TypedDict):
     active: bool
-    language: Language
+    languages: list[Language]
 
 
-config = TrasnlatorConfig(active=False, language="ja")
+config = TrasnlatorConfig(
+    active=False,
+    languages=["ja", "en"],
+)
 CONFIG_REGISTRY_TYPE = client.registry.create("config", config)
 
 
 @CONFIG_REGISTRY_TYPE.listen
 async def on_config_change(new_config: TrasnlatorConfig):
     global config
     config = new_config
     logger.info(f"translator config updated: {config}")
 
 
-async def translate(component: content.Component) -> content.Component:
+async def translate(component: Component, lang: Language) -> Component:
+    component = component.copy()
     if not translator:
         return component
-    texts = [
-        sibling for sibling in component.iter() if isinstance(sibling, content.Text)
-    ]
+    texts = [sibling for sibling in component.iter() if isinstance(sibling, Text)]
     translated = await translator.translate(
-        [text.text for text in texts if text.text], config["language"]
+        [text.text for text in texts if text.text],
+        lang,
     )
-    for text, (translation, _) in zip(texts, translated):
+    for text, (translation, _) in zip(texts, translated, strict=False):
         text.text = translation
     return component
 
 
+def is_same_content(a: Component, b: Component) -> bool:
+    texts_a = [
+        sibling.text.lower() for sibling in a.iter() if isinstance(sibling, Text)
+    ]
+    texts_b = [
+        sibling.text.lower() for sibling in b.iter() if isinstance(sibling, Text)
+    ]
+    return all(a == b for a, b in zip(texts_a, texts_b, strict=False))
+
+
 @client.chat.messages.proxy
 async def on_message_add(message: model.Message) -> model.Message:
     if not config["active"]:
         return message
     if not message.content:
         return message
-    message.content = await translate(message.content)
+    translations: dict[str, Component] = {}
+    if len(config["languages"]) == 1:
+        lang = config["languages"][0]
+        translated = await translate(message.content, lang)
+        message.content = translated
+        return message
+    for lang in config["languages"]:
+        translated = await translate(message.content, lang)
+        translations[lang] = translated
+    if all(
+        is_same_content(translations[lang], translations[config["languages"][0]])
+        for lang in config["languages"][1:]
+    ):
+        message.content = translations[config["languages"][0]]
+        return message
+    content = Root()
+    for i, (lang, translated) in enumerate(translations.items()):
+        lines = [
+            Text(f"{lang}:") if i == 0 else Text(f" {lang}:"),
+            translated,
+        ]
+        content.add(System(lines))
+    message.content = content
     return message
 
 
 @client.on(events.ready)
 async def on_ready():
     global translator, config
     config = await CONFIG_REGISTRY_TYPE.get()
```

