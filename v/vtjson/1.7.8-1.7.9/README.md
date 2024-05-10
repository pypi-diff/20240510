# Comparing `tmp/vtjson-1.7.8.tar.gz` & `tmp/vtjson-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.7.8.tar", last modified: Sun Apr 28 05:42:54 2024, max compression
+gzip compressed data, was "vtjson-1.7.9.tar", last modified: Sun Apr 28 06:37:06 2024, max compression
```

## Comparing `vtjson-1.7.8.tar` & `vtjson-1.7.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:42:54.975399 vtjson-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-28 05:42:50.000000 vtjson-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 05:42:54.975399 vtjson-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19109 2024-04-28 05:42:50.000000 vtjson-1.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-28 05:42:50.000000 vtjson-1.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:42:54.975399 vtjson-1.7.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:42:54.975399 vtjson-1.7.8/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30742 2024-04-28 05:42:50.000000 vtjson-1.7.8/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:37:06.217266 vtjson-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-28 06:37:00.000000 vtjson-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 06:37:06.217266 vtjson-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19109 2024-04-28 06:37:00.000000 vtjson-1.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-28 06:37:00.000000 vtjson-1.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:37:06.217266 vtjson-1.7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:37:06.217266 vtjson-1.7.9/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 06:37:06.000000 vtjson-1.7.9/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30777 2024-04-28 06:37:00.000000 vtjson-1.7.9/vtjson.py
```

### Comparing `vtjson-1.7.8/LICENSE` & `vtjson-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.8/PKG-INFO` & `vtjson-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.8
+Version: 1.7.9
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vtjson-1.7.8/README.md` & `vtjson-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.8/pyproject.toml` & `vtjson-1.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.8/vtjson.egg-info/PKG-INFO` & `vtjson-1.7.9/vtjson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.8
+Version: 1.7.9
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vtjson-1.7.8/vtjson.py` & `vtjson-1.7.9/vtjson.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.7.8"
+__version__ = "1.7.9"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -327,17 +327,19 @@
 
     def __validate__(self, object, name, strict):
         try:
             object_mime_type = magic_.from_buffer(object, mime=True)
         except Exception as e:
             return _wrong_type_message(object, name, self.__name__, str(e))
         if object_mime_type != self.mime_type:
-            return (
-                f"The mime type of {name} is equal to {repr(object_mime_type)} "
-                f"which is different from {repr(self.mime_type)}"
+            return _wrong_type_message(
+                object,
+                name,
+                self.__name__,
+                f"{repr(object_mime_type)} is different from {repr(self.mime_type)}",
             )
         return ""
 
 
 class div:
     def __init__(self, divisor, remainder=0, name=None):
         if not isinstance(divisor, int):
```

