# Comparing `tmp/anything_world-0.1.5.tar.gz` & `tmp/anything_world-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anything_world-0.1.5.tar", last modified: Mon Mar 18 10:55:08 2024, max compression
+gzip compressed data, was "anything_world-0.1.6.tar", last modified: Fri May 10 08:29:13 2024, max compression
```

## Comparing `anything_world-0.1.5.tar` & `anything_world-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.997630 anything_world-0.1.5/
--rw-r--r--   0 vilson     (501) staff       (20)     1071 2023-12-15 20:15:20.000000 anything_world-0.1.5/LICENSE
--rw-r--r--   0 vilson     (501) staff       (20)      241 2024-01-15 19:55:45.000000 anything_world-0.1.5/MANIFEST.in
--rw-r--r--   0 vilson     (501) staff       (20)     4500 2024-03-18 10:55:08.997323 anything_world-0.1.5/PKG-INFO
--rw-r--r--   0 vilson     (501) staff       (20)     3868 2024-03-18 10:45:06.000000 anything_world-0.1.5/README.md
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.991317 anything_world-0.1.5/anything_world/
--rw-r--r--   0 vilson     (501) staff       (20)        0 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/__init__.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.993810 anything_world-0.1.5/anything_world/async_api/
--rw-r--r--   0 vilson     (501) staff       (20)       32 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/async_api/__init__.py
--rw-r--r--   0 vilson     (501) staff       (20)    12407 2024-03-18 10:41:48.000000 anything_world-0.1.5/anything_world/async_api/api_client.py
--rw-r--r--   0 vilson     (501) staff       (20)     3163 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/async_api/utils.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.995184 anything_world-0.1.5/anything_world/sync_api/
--rw-r--r--   0 vilson     (501) staff       (20)       32 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/sync_api/__init__.py
--rw-r--r--   0 vilson     (501) staff       (20)    12250 2024-03-18 10:38:29.000000 anything_world-0.1.5/anything_world/sync_api/api_client.py
--rw-r--r--   0 vilson     (501) staff       (20)     2755 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/sync_api/utils.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.995511 anything_world-0.1.5/anything_world/utils/
--rw-r--r--   0 vilson     (501) staff       (20)     2872 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/utils/__init__.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.996955 anything_world-0.1.5/anything_world.egg-info/
--rw-r--r--   0 vilson     (501) staff       (20)     4500 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/PKG-INFO
--rw-r--r--   0 vilson     (501) staff       (20)      634 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/SOURCES.txt
--rw-r--r--   0 vilson     (501) staff       (20)        1 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/dependency_links.txt
--rw-r--r--   0 vilson     (501) staff       (20)       46 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/entry_points.txt
--rw-r--r--   0 vilson     (501) staff       (20)      119 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/requires.txt
--rw-r--r--   0 vilson     (501) staff       (20)       23 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/top_level.txt
--rw-r--r--   0 vilson     (501) staff       (20)      132 2024-01-12 14:53:25.000000 anything_world-0.1.5/env.example
--rw-r--r--   0 vilson     (501) staff       (20)      829 2024-03-18 10:50:07.000000 anything_world-0.1.5/pyproject.toml
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.995712 anything_world-0.1.5/scripts/
--rw-r--r--   0 vilson     (501) staff       (20)       95 2024-01-26 12:20:47.000000 anything_world-0.1.5/scripts/cli.py
--rw-r--r--   0 vilson     (501) staff       (20)       38 2024-03-18 10:55:08.997680 anything_world-0.1.5/setup.cfg
--rw-r--r--   0 vilson     (501) staff       (20)       91 2024-01-12 14:53:25.000000 anything_world-0.1.5/setup.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.996568 anything_world-0.1.5/tests/
--rw-r--r--   0 vilson     (501) staff       (20)     2110 2024-01-22 18:22:58.000000 anything_world-0.1.5/tests/test_async_api.py
--rw-r--r--   0 vilson     (501) staff       (20)     2006 2024-01-22 18:22:58.000000 anything_world-0.1.5/tests/test_sync_api.py
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.720955 anything_world-0.1.6/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     1071 2024-05-10 08:20:41.000000 anything_world-0.1.6/LICENSE
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      241 2024-05-10 08:20:41.000000 anything_world-0.1.6/MANIFEST.in
+-rw-r--r--   0 vilson    (1000) vilson    (1001)     4545 2024-05-10 08:29:13.720955 anything_world-0.1.6/PKG-INFO
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     3913 2024-05-10 08:21:23.000000 anything_world-0.1.6/README.md
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/__init__.py
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/async_api/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       32 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/async_api/__init__.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)    12407 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/async_api/api_client.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     3163 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/async_api/utils.py
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/sync_api/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       32 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/sync_api/__init__.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)    12250 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/sync_api/api_client.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2755 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/sync_api/utils.py
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world/utils/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2872 2024-05-10 08:20:41.000000 anything_world-0.1.6/anything_world/utils/__init__.py
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/anything_world.egg-info/
+-rw-r--r--   0 vilson    (1000) vilson    (1001)     4545 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/PKG-INFO
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      634 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/SOURCES.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)        1 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/dependency_links.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       46 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/entry_points.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      119 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/requires.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       23 2024-05-10 08:29:13.000000 anything_world-0.1.6/anything_world.egg-info/top_level.txt
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      132 2024-05-10 08:20:41.000000 anything_world-0.1.6/env.example
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)      829 2024-05-10 08:26:56.000000 anything_world-0.1.6/pyproject.toml
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/scripts/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       95 2024-05-10 08:20:41.000000 anything_world-0.1.6/scripts/cli.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       38 2024-05-10 08:29:13.720955 anything_world-0.1.6/setup.cfg
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)       91 2024-05-10 08:20:41.000000 anything_world-0.1.6/setup.py
+drwxrwxr-x   0 vilson    (1000) vilson    (1001)        0 2024-05-10 08:29:13.710955 anything_world-0.1.6/tests/
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2110 2024-05-10 08:20:41.000000 anything_world-0.1.6/tests/test_async_api.py
+-rw-rw-r--   0 vilson    (1000) vilson    (1001)     2006 2024-05-10 08:20:41.000000 anything_world-0.1.6/tests/test_sync_api.py
```

### Comparing `anything_world-0.1.5/LICENSE` & `anything_world-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/PKG-INFO` & `anything_world-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anything_world
-Version: 0.1.5
+Version: 0.1.6
 Summary: Anything World API wrapper library and CLI
 Author-email: Anything World <support@anything.world>
 License: MIT
 Project-URL: Homepage, https://anything.world
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -62,14 +62,16 @@
 if you use-case requires async calls, please follow the next section for its
 implementation.
 
 ## Sync
 
 ```python
 from anything_world.sync_api import AWClient
+from dotenv import load_dotenv
+load_dotenv()
 
 # Create a client to be able to query Anything World's API
 client = AWClient()
 
 # Search for 3D models of `cats`:
 response = client.find('cats')
```

### Comparing `anything_world-0.1.5/README.md` & `anything_world-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 if you use-case requires async calls, please follow the next section for its
 implementation.
 
 ## Sync
 
 ```python
 from anything_world.sync_api import AWClient
+from dotenv import load_dotenv
+load_dotenv()
 
 # Create a client to be able to query Anything World's API
 client = AWClient()
 
 # Search for 3D models of `cats`:
 response = client.find('cats')
```

### Comparing `anything_world-0.1.5/anything_world/async_api/api_client.py` & `anything_world-0.1.6/anything_world/async_api/api_client.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/anything_world/async_api/utils.py` & `anything_world-0.1.6/anything_world/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/anything_world/sync_api/api_client.py` & `anything_world-0.1.6/anything_world/sync_api/api_client.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/anything_world/sync_api/utils.py` & `anything_world-0.1.6/anything_world/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/anything_world/utils/__init__.py` & `anything_world-0.1.6/anything_world/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/anything_world.egg-info/PKG-INFO` & `anything_world-0.1.6/anything_world.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anything_world
-Version: 0.1.5
+Version: 0.1.6
 Summary: Anything World API wrapper library and CLI
 Author-email: Anything World <support@anything.world>
 License: MIT
 Project-URL: Homepage, https://anything.world
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -62,14 +62,16 @@
 if you use-case requires async calls, please follow the next section for its
 implementation.
 
 ## Sync
 
 ```python
 from anything_world.sync_api import AWClient
+from dotenv import load_dotenv
+load_dotenv()
 
 # Create a client to be able to query Anything World's API
 client = AWClient()
 
 # Search for 3D models of `cats`:
 response = client.find('cats')
```

### Comparing `anything_world-0.1.5/anything_world.egg-info/SOURCES.txt` & `anything_world-0.1.6/anything_world.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/pyproject.toml` & `anything_world-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anything_world"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     {name = "Anything World", email = "support@anything.world"},
 ]
 description = "Anything World API wrapper library and CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
```

### Comparing `anything_world-0.1.5/tests/test_async_api.py` & `anything_world-0.1.6/tests/test_async_api.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.5/tests/test_sync_api.py` & `anything_world-0.1.6/tests/test_sync_api.py`

 * *Files identical despite different names*

