# Comparing `tmp/luxos-0.0.7b23.tar.gz` & `tmp/luxos-0.0.7b24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.7b23.tar", last modified: Thu May  9 14:13:23 2024, max compression
+gzip compressed data, was "luxos-0.0.7b24.tar", last modified: Fri May 10 07:33:08 2024, max compression
```

## Comparing `luxos-0.0.7b23.tar` & `luxos-0.0.7b24.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-09 14:13:23.571790 luxos-0.0.7b23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-09 14:12:51.000000 luxos-0.0.7b23/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-09 14:13:21.000000 luxos-0.0.7b23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:13:23.571790 luxos-0.0.7b23/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.563790 luxos-0.0.7b23/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.567790 luxos-0.0.7b23/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-09 14:13:21.000000 luxos-0.0.7b23/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.567790 luxos-0.0.7b23/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_luxos_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:33:08.349321 luxos-0.0.7b24/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-10 07:33:08.349321 luxos-0.0.7b24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-10 07:32:38.000000 luxos-0.0.7b24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-10 07:33:06.000000 luxos-0.0.7b24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:33:08.349321 luxos-0.0.7b24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:33:08.345321 luxos-0.0.7b24/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:33:08.345321 luxos-0.0.7b24/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 07:33:06.000000 luxos-0.0.7b24/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:33:08.349321 luxos-0.0.7b24/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:33:08.349321 luxos-0.0.7b24/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-10 07:32:38.000000 luxos-0.0.7b24/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:33:08.349321 luxos-0.0.7b24/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-10 07:33:08.000000 luxos-0.0.7b24/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-10 07:33:08.000000 luxos-0.0.7b24/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:33:08.000000 luxos-0.0.7b24/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 07:33:08.000000 luxos-0.0.7b24/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 07:33:08.000000 luxos-0.0.7b24/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 07:33:08.000000 luxos-0.0.7b24/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:33:08.349321 luxos-0.0.7b24/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-10 07:32:38.000000 luxos-0.0.7b24/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-10 07:32:38.000000 luxos-0.0.7b24/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-10 07:32:38.000000 luxos-0.0.7b24/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 07:32:38.000000 luxos-0.0.7b24/tests/test_luxos_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-10 07:32:38.000000 luxos-0.0.7b24/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-10 07:32:38.000000 luxos-0.0.7b24/tests/test_utils.py
```

### Comparing `luxos-0.0.7b23/PKG-INFO` & `luxos-0.0.7b24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.7b23
+Version: 0.0.7b24
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.7b23/README.md` & `luxos-0.0.7b24/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/pyproject.toml` & `luxos-0.0.7b24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.7b23"
+version = "0.0.7b24"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.7b23/src/luxos/api.json` & `luxos-0.0.7b24/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/api.py` & `luxos-0.0.7b24/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/asyncops.py` & `luxos-0.0.7b24/src/luxos/asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/cli/v1.py` & `luxos-0.0.7b24/src/luxos/cli/v1.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/exceptions.py` & `luxos-0.0.7b24/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/misc.py` & `luxos-0.0.7b24/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/scripts/async_luxos.py` & `luxos-0.0.7b24/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/scripts/health_checker.py` & `luxos-0.0.7b24/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/scripts/luxos.py` & `luxos-0.0.7b24/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/text.py` & `luxos-0.0.7b24/src/luxos/text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos/utils.py` & `luxos-0.0.7b24/src/luxos/utils.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.7b24/src/luxos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.7b23
+Version: 0.0.7b24
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.7b23/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.7b24/src/luxos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/tests/test_cli.py` & `luxos-0.0.7b24/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/tests/test_luxos_asyncops.py` & `luxos-0.0.7b24/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/tests/test_luxos_misc.py` & `luxos-0.0.7b24/tests/test_luxos_misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/tests/test_text.py` & `luxos-0.0.7b24/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.7b23/tests/test_utils.py` & `luxos-0.0.7b24/tests/test_utils.py`

 * *Files identical despite different names*

