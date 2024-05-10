# Comparing `tmp/omuplugin_emoji-0.2.5.tar.gz` & `tmp/omuplugin_emoji-0.3.0.tar.gz`

## Comparing `omuplugin_emoji-0.2.5.tar` & `omuplugin_emoji-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.5/src/omuplugin_emoji/__init__.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.5/src/omuplugin_emoji/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.5/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.5/README.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.0/src/omuplugin_emoji/__init__.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.0/src/omuplugin_emoji/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.0/src/omuplugin_emoji/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.0/README.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 omuplugin_emoji-0.3.0/PKG-INFO
```

### Comparing `omuplugin_emoji-0.2.5/src/omuplugin_emoji/plugin.py` & `omuplugin_emoji-0.3.0/src/omuplugin_emoji/plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import re
+from collections.abc import Mapping
 from dataclasses import dataclass
-from typing import List, Literal, Mapping, Tuple, TypedDict
+from typing import Literal, TypedDict
 
+from loguru import logger
 from omu.extension.table.table import TableType
 from omu.identifier import Identifier
 from omu.interface.keyable import Keyable
 from omu.model import Model
 from omuchat import App, Client
 from omuchat.event.event_types import events
 from omuchat.model import content
@@ -15,14 +17,30 @@
 APP = App(
     IDENTIFIER,
     version="0.1.0",
 )
 client = Client(APP)
 
 
+class EmojiConfig(TypedDict):
+    active: bool
+
+
+config = EmojiConfig(
+    active=False,
+)
+
+
+@client.registry.create("config", config).listen
+async def on_config_change(new_config: EmojiConfig):
+    global config
+    config = new_config
+    logger.info(f"emoji config updated: {config}")
+
+
 class TextPattern(TypedDict):
     type: Literal["text"]
     text: str
 
 
 class ImagePattern(TypedDict):
     type: Literal["image"]
@@ -36,23 +54,23 @@
 
 type Pattern = TextPattern | ImagePattern | RegexPattern
 
 
 class EmojiData(TypedDict):
     id: str
     asset: str
-    patterns: List[Pattern]
+    patterns: list[Pattern]
 
 
 class Emoji(Model[EmojiData], Keyable):
     def __init__(
         self,
         id: str,
         asset: Identifier,
-        patterns: List[Pattern],
+        patterns: list[Pattern],
     ) -> None:
         self.id = id
         self.asset = asset
         self.patterns = patterns
 
     def key(self) -> str:
         return self.id
@@ -79,17 +97,17 @@
     model_type=Emoji,
 )
 emoji_table = client.tables.get(EMOJI_TABLE_TYPE)
 emoji_table.set_cache_size(1000)
 
 
 class Patterns:
-    text: List[Tuple[TextPattern, Emoji]] = []
-    image: List[Tuple[ImagePattern, Emoji]] = []
-    regex: List[Tuple[RegexPattern, Emoji]] = []
+    text: list[tuple[TextPattern, Emoji]] = []
+    image: list[tuple[ImagePattern, Emoji]] = []
+    regex: list[tuple[RegexPattern, Emoji]] = []
 
 
 @emoji_table.listen
 async def update_emoji_table(items: Mapping[str, Emoji]):
     Patterns.text.clear()
     Patterns.image.clear()
     Patterns.regex.clear()
@@ -183,14 +201,16 @@
         if match.start == 0:
             break
     return match
 
 
 @client.chat.messages.proxy
 async def on_message(message: Message):
+    if not config["active"]:
+        return message
     if not message.content:
         return message
     message.content = transform(message.content)
     return message
 
 
 @client.on(events.ready)
```

### Comparing `omuplugin_emoji-0.2.5/pyproject.toml` & `omuplugin_emoji-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_emoji"
-version = "0.2.5"
+version = "0.3.0"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
-dependencies = ["omuchat>=0.1.9"]
+dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuplugin_emoji:plugin"
 
 [build-system]
```

