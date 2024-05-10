# Comparing `tmp/py_allspice-2.5.0.tar.gz` & `tmp/py_allspice-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_allspice-2.5.0.tar", last modified: Tue Apr 16 15:33:26 2024, max compression
+gzip compressed data, was "py_allspice-3.0.0.tar", last modified: Fri May 10 14:34:57 2024, max compression
```

## Comparing `py_allspice-2.5.0.tar` & `py_allspice-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.335110 py_allspice-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-16 15:33:19.000000 py_allspice-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-16 15:33:26.335110 py_allspice-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-16 15:33:19.000000 py_allspice-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.331110 py_allspice-2.5.0/allspice/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/allspice.py
--rw-r--r--   0 runner    (1001) docker     (127)    75142 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/apiobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/baseapiobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/ratelimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.331110 py_allspice-2.5.0/allspice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/bom_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/netlist_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.335110 py_allspice-2.5.0/py_allspice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 15:33:19.000000 py_allspice-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:33:26.335110 py_allspice-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-16 15:33:19.000000 py_allspice-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.335110 py_allspice-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    32675 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_api_longtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_api_ratelimiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.861518 py_allspice-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 14:34:50.000000 py_allspice-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-10 14:34:57.857518 py_allspice-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-10 14:34:50.000000 py_allspice-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/allspice/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/allspice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75142 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/apiobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/baseapiobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/ratelimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/allspice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21370 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/bom_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/netlist_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/py_allspice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 14:34:50.000000 py_allspice-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:34:57.861518 py_allspice-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-10 14:34:50.000000 py_allspice-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    32675 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_api_longtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_api_ratelimiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_utils.py
```

### Comparing `py_allspice-2.5.0/LICENSE` & `py_allspice-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/PKG-INFO` & `py_allspice-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 2.5.0
+Version: 3.0.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/AllSpiceIO/py-allspice
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py_allspice-2.5.0/README.md` & `py_allspice-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/__init__.py` & `py_allspice-3.0.0/allspice/__init__.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/allspice.py` & `py_allspice-3.0.0/allspice/allspice.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/apiobject.py` & `py_allspice-3.0.0/allspice/apiobject.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/baseapiobject.py` & `py_allspice-3.0.0/allspice/baseapiobject.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/exceptions.py` & `py_allspice-3.0.0/allspice/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/ratelimiter.py` & `py_allspice-3.0.0/allspice/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/utils/core.py` & `py_allspice-3.0.0/allspice/utils/core.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/allspice/utils/netlist_generation.py` & `py_allspice-3.0.0/allspice/utils/netlist_generation.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/py_allspice.egg-info/PKG-INFO` & `py_allspice-3.0.0/py_allspice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 2.5.0
+Version: 3.0.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/AllSpiceIO/py-allspice
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py_allspice-2.5.0/py_allspice.egg-info/SOURCES.txt` & `py_allspice-3.0.0/py_allspice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/setup.py` & `py_allspice-3.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name="py-allspice",
-    version="2.5.0",
+    version="3.0.0",
     description="A python wrapper for the AllSpice Hub API",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     author="AllSpice, Inc.",
     author_email="maintainers@allspice.io",
```

### Comparing `py_allspice-2.5.0/tests/test_api.py` & `py_allspice-3.0.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/tests/test_api_longtests.py` & `py_allspice-3.0.0/tests/test_api_longtests.py`

 * *Files identical despite different names*

### Comparing `py_allspice-2.5.0/tests/test_api_ratelimiting.py` & `py_allspice-3.0.0/tests/test_api_ratelimiting.py`

 * *Files identical despite different names*

