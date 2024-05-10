# Comparing `tmp/ieugwaspy-1.0.2.tar.gz` & `tmp/ieugwaspy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieugwaspy-1.0.2.tar", last modified: Sun May  5 09:28:19 2024, max compression
+gzip compressed data, was "ieugwaspy-1.0.3.tar", last modified: Fri May 10 19:34:11 2024, max compression
```

## Comparing `ieugwaspy-1.0.2.tar` & `ieugwaspy-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1455 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.516997 ieugwaspy-1.0.2/ieugwaspy/
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      838 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/backwards.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6860 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/query.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/ieugwaspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      695 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:34:11.527626 ieugwaspy-1.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-10 19:34:11.527626 ieugwaspy-1.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1455 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:34:11.523626 ieugwaspy-1.0.3/ieugwaspy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/ieugwaspy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      838 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/ieugwaspy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/ieugwaspy/backwards.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1321 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/ieugwaspy/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6923 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/ieugwaspy/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/ieugwaspy/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:34:11.527626 ieugwaspy-1.0.3/ieugwaspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-10 19:34:11.000000 ieugwaspy-1.0.3/ieugwaspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-10 19:34:11.000000 ieugwaspy-1.0.3/ieugwaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:34:11.000000 ieugwaspy-1.0.3/ieugwaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 19:34:11.000000 ieugwaspy-1.0.3/ieugwaspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 19:34:11.000000 ieugwaspy-1.0.3/ieugwaspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:34:11.527626 ieugwaspy-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      741 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:34:11.527626 ieugwaspy-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 19:34:02.000000 ieugwaspy-1.0.3/tests/test_api.py
```

### Comparing `ieugwaspy-1.0.2/LICENSE` & `ieugwaspy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.2/PKG-INFO` & `ieugwaspy-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieugwaspy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python interface to IEU GWAS database API
 Home-page: https://mrcieu.github.io/ieugwaspy/
 Author: Tom Gaunt
 Author-email: tom@biocompute.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ieugwaspy-1.0.2/README.md` & `ieugwaspy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.2/ieugwaspy/api.py` & `ieugwaspy-1.0.3/ieugwaspy/api.py`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.2/ieugwaspy/backwards.py` & `ieugwaspy-1.0.3/ieugwaspy/backwards.py`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.2/ieugwaspy/config.py` & `ieugwaspy-1.0.3/ieugwaspy/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Args:
     env: all the active configurations
     urls: API base urls available
     url_obtain_jwt: URL for the webpage to obtain a JWT
 """
 import json
 
+__version__ = "1.0.3"
 
 env = {
     "base_url": "https://api.opengwas.io/api/",
     "jwt": "",
     "test_mode_key": ""
 }
 urls = {
```

### Comparing `ieugwaspy-1.0.2/ieugwaspy/query.py` & `ieugwaspy-1.0.3/ieugwaspy/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 
     Returns:
         data: JSON object as returned by API
 
     """
     url = urljoin(config.env["base_url"], path)
 
-    headers = {}
+    headers = {
+        "X-API-SOURCE": "ieugwaspy/" + config.__version__
+    }
     if config.env["jwt"]:
         headers["Authorization"] = "Bearer " + config.env["jwt"]
     if config.env["test_mode_key"]:
         headers["X-TEST-MODE-KEY"] = config.env["test_mode_key"]
 
     if method == "GET":
         response = requests.get(url, headers=headers)
```

### Comparing `ieugwaspy-1.0.2/ieugwaspy/variants.py` & `ieugwaspy-1.0.3/ieugwaspy/variants.py`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.2/ieugwaspy.egg-info/PKG-INFO` & `ieugwaspy-1.0.3/ieugwaspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieugwaspy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python interface to IEU GWAS database API
 Home-page: https://mrcieu.github.io/ieugwaspy/
 Author: Tom Gaunt
 Author-email: tom@biocompute.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ieugwaspy-1.0.2/setup.py` & `ieugwaspy-1.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import setuptools
 
+from ieugwaspy.config import __version__
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="ieugwaspy",
-    version="1.0.2",
+    version=__version__,
     author="Tom Gaunt",
     author_email="tom@biocompute.org.uk",
     description="Python interface to IEU GWAS database API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mrcieu.github.io/ieugwaspy/",
     packages=setuptools.find_packages(),
```

### Comparing `ieugwaspy-1.0.2/tests/test_api.py` & `ieugwaspy-1.0.3/tests/test_api.py`

 * *Files identical despite different names*

