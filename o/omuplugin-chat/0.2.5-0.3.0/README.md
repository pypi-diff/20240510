# Comparing `tmp/omuplugin_chat-0.2.5.tar.gz` & `tmp/omuplugin_chat-0.3.0.tar.gz`

## Comparing `omuplugin_chat-0.2.5.tar` & `omuplugin_chat-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/src/omuplugin_chat/__init__.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/src/omuplugin_chat/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.0/src/omuplugin_chat/__init__.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.0/src/omuplugin_chat/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.0/src/omuplugin_chat/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.0/README.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 omuplugin_chat-0.3.0/PKG-INFO
```

### Comparing `omuplugin_chat-0.2.5/pyproject.toml` & `omuplugin_chat-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_chat"
-version = "0.2.5"
+version = "0.3.0"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
-dependencies = ["omuchat>=0.1.9"]
+dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9", "iwashi>=3.0.1"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuplugin_chat:plugin"
 
 [build-system]
```

