# Comparing `tmp/upsonic_legacy-0.23.5.tar.gz` & `tmp/upsonic_legacy-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsonic_legacy-0.23.5.tar", last modified: Thu Apr 25 18:29:49 2024, max compression
+gzip compressed data, was "upsonic_legacy-0.23.6.tar", last modified: Fri May 10 14:02:58 2024, max compression
```

## Comparing `upsonic_legacy-0.23.5.tar` & `upsonic_legacy-0.23.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:29:49.745231 upsonic_legacy-0.23.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-25 18:29:49.745231 upsonic_legacy-0.23.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:29:49.745231 upsonic_legacy-0.23.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:29:49.745231 upsonic_legacy-0.23.5/upsonic/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/upsonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:29:49.745231 upsonic_legacy-0.23.5/upsonic/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/upsonic/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/upsonic/remote/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/upsonic/remote/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/upsonic/remote/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:29:49.745231 upsonic_legacy-0.23.5/upsonic/remote/localimport/
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/upsonic/remote/localimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51844 2024-04-25 18:29:41.000000 upsonic_legacy-0.23.5/upsonic/remote/on_prem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:29:49.745231 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-25 18:29:49.000000 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-25 18:29:49.000000 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:29:49.000000 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 18:29:49.000000 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:29:49.000000 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-25 18:29:49.000000 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 18:29:49.000000 upsonic_legacy-0.23.5/upsonic_legacy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:02:58.828552 upsonic_legacy-0.23.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-10 14:02:58.828552 upsonic_legacy-0.23.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:02:58.828552 upsonic_legacy-0.23.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:02:58.824552 upsonic_legacy-0.23.6/upsonic/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/upsonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:02:58.828552 upsonic_legacy-0.23.6/upsonic/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/upsonic/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/upsonic/remote/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/upsonic/remote/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/upsonic/remote/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:02:58.828552 upsonic_legacy-0.23.6/upsonic/remote/localimport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/upsonic/remote/localimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52180 2024-05-10 14:02:49.000000 upsonic_legacy-0.23.6/upsonic/remote/on_prem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:02:58.828552 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-10 14:02:58.000000 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-10 14:02:58.000000 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:02:58.000000 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 14:02:58.000000 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:02:58.000000 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 14:02:58.000000 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 14:02:58.000000 upsonic_legacy-0.23.6/upsonic_legacy.egg-info/top_level.txt
```

### Comparing `upsonic_legacy-0.23.5/LICENSE` & `upsonic_legacy-0.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.5/PKG-INFO` & `upsonic_legacy-0.23.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic_legacy
-Version: 0.23.5
+Version: 0.23.6
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
```

### Comparing `upsonic_legacy-0.23.5/README.md` & `upsonic_legacy-0.23.6/README.md`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.5/setup.py` & `upsonic_legacy-0.23.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="upsonic_legacy",
-    version="0.23.5",
+    version="0.23.6",
     description="""Magic Cloud Layer""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/Upsonic/Upsonic",
     author="Upsonic",
     author_email="onur.atakan.ulusoy@upsonic.co",
     license="MIT",
```

### Comparing `upsonic_legacy-0.23.5/upsonic/__init__.py` & `upsonic_legacy-0.23.6/upsonic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 from .remote import decrypt
 from .remote import upsonic_serializer
 from .remote import interface
 
 
 open_databases = {}
 
-__version__ = '0.23.5'
+__version__ = '0.23.6'
```

### Comparing `upsonic_legacy-0.23.5/upsonic/remote/__init__.py` & `upsonic_legacy-0.23.6/upsonic/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.5/upsonic/remote/controller.py` & `upsonic_legacy-0.23.6/upsonic/remote/controller.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.5/upsonic/remote/helper.py` & `upsonic_legacy-0.23.6/upsonic/remote/helper.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.5/upsonic/remote/interface.py` & `upsonic_legacy-0.23.6/upsonic/remote/interface.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.5/upsonic/remote/localimport/__init__.py` & `upsonic_legacy-0.23.6/upsonic/remote/localimport/__init__.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.23.5/upsonic/remote/on_prem.py` & `upsonic_legacy-0.23.6/upsonic/remote/on_prem.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,14 +648,23 @@
         the_version = []
         the_version.append(int(total.split(".")[0]))
         the_version.append(int(total.split(".")[1]))
         the_version.append(int(total.split(".")[2]))
         return the_version
 
 
+
+    def get_lock(self, key):
+        data = {"scope": key}
+        lock = self._send_request("POST", "/get_lock_of_scope", data)
+        return lock
+
+
+
+
     def set(
             self,
             key,
             value,
     ):
 
         if key.startswith("."):
@@ -672,14 +681,20 @@
             return False
         if ".." in key:
             self._log("Error: The key can not include multiple dot one after one'..'")
             return False
 
 
 
+        try:
+            if self.get_lock(key):
+                self._log("This scope is locked now! Someone dumping.")
+                return False
+        except:
+            pass
 
 
         the_type = type(value).__name__
         if the_type == "type":
             the_type = "class"
 
         encryption_key = "u"
```

### Comparing `upsonic_legacy-0.23.5/upsonic_legacy.egg-info/PKG-INFO` & `upsonic_legacy-0.23.6/upsonic_legacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic-legacy
-Version: 0.23.5
+Version: 0.23.6
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
```

### Comparing `upsonic_legacy-0.23.5/upsonic_legacy.egg-info/SOURCES.txt` & `upsonic_legacy-0.23.6/upsonic_legacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

