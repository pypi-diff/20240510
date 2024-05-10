# Comparing `tmp/omuplugin_nyanya-0.2.5.tar.gz` & `tmp/omuplugin_nyanya-0.3.0.tar.gz`

## Comparing `omuplugin_nyanya-0.2.5.tar` & `omuplugin_nyanya-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/src/omuplugin_nyanya/__init__.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/src/omuplugin_nyanya/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.0/src/omuplugin_nyanya/__init__.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.0/src/omuplugin_nyanya/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.0/src/omuplugin_nyanya/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.0/README.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.3.0/PKG-INFO
```

### Comparing `omuplugin_nyanya-0.2.5/src/omuplugin_nyanya/plugin.py` & `omuplugin_nyanya-0.3.0/src/omuplugin_nyanya/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 client = Client(APP)
 replaces = {
     "な": "にゃ",
     "ナ": "ニャ",
 }
 
 
-async def translate(component: content.Component) -> content.Component:
+async def translate(
+    component: content.Component,
+) -> content.Component:
     for child in component.iter():
         if not isinstance(child, content.Text):
             continue
         child.text = child.text.translate(str.maketrans(replaces))
     return component
```

### Comparing `omuplugin_nyanya-0.2.5/pyproject.toml` & `omuplugin_nyanya-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_nyanya"
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
 plugin = "omuplugin_nyanya:plugin"
 
 [build-system]
```

