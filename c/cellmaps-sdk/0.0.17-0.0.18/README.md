# Comparing `tmp/cellmaps_sdk-0.0.17.tar.gz` & `tmp/cellmaps_sdk-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmaps_sdk-0.0.17.tar", last modified: Fri May 10 14:22:27 2024, max compression
+gzip compressed data, was "cellmaps_sdk-0.0.18.tar", last modified: Fri May 10 14:34:11 2024, max compression
```

## Comparing `cellmaps_sdk-0.0.17.tar` & `cellmaps_sdk-0.0.18.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:22:27.346989 cellmaps_sdk-0.0.17/
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.17/LICENSE.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1570 2024-05-10 14:22:27.346721 cellmaps_sdk-0.0.17/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.17/README.rst
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1562 2024-05-10 14:22:20.000000 cellmaps_sdk-0.0.17/pyproject.toml
--rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-05-10 14:22:27.347045 cellmaps_sdk-0.0.17/setup.cfg
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:22:27.339590 cellmaps_sdk-0.0.17/src/
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:22:27.345075 cellmaps_sdk-0.0.17/src/cellmaps_sdk/
--rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/__init__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/__main__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    36830 2024-02-23 16:16:31.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/_cli_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1714 2024-05-10 13:01:29.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/_config.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     9733 2024-05-09 13:35:31.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/_raw_data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/_test_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1820 2024-04-24 15:54:59.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    35543 2024-05-10 14:19:40.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/data_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    29788 2024-03-06 12:03:46.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/process.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk/py.typed
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:22:27.346155 cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1570 2024-05-10 14:22:27.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      595 2024-05-10 14:22:27.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-05-10 14:22:27.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-05-10 14:22:27.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/entry_points.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)      171 2024-05-10 14:22:27.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/requires.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-05-10 14:22:27.000000 cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:34:11.654628 cellmaps_sdk-0.0.18/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.18/LICENSE.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1570 2024-05-10 14:34:11.654296 cellmaps_sdk-0.0.18/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.18/README.rst
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1562 2024-05-10 14:33:25.000000 cellmaps_sdk-0.0.18/pyproject.toml
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-05-10 14:34:11.654698 cellmaps_sdk-0.0.18/setup.cfg
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:34:11.646499 cellmaps_sdk-0.0.18/src/
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:34:11.651842 cellmaps_sdk-0.0.18/src/cellmaps_sdk/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/__init__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/__main__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    36830 2024-02-23 16:16:31.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/_cli_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1765 2024-05-10 14:32:03.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/_config.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     9733 2024-05-09 13:35:31.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/_raw_data.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/_test_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1820 2024-04-24 15:54:59.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    35548 2024-05-10 14:32:30.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/data.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/data_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    29788 2024-03-06 12:03:46.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/process.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk/py.typed
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-10 14:34:11.652899 cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1570 2024-05-10 14:34:11.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      595 2024-05-10 14:34:11.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-05-10 14:34:11.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-05-10 14:34:11.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      171 2024-05-10 14:34:11.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/requires.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-05-10 14:34:11.000000 cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/top_level.txt
```

### Comparing `cellmaps_sdk-0.0.17/PKG-INFO` & `cellmaps_sdk-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.17
+Version: 0.0.18
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
```

### Comparing `cellmaps_sdk-0.0.17/pyproject.toml` & `cellmaps_sdk-0.0.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "cellmaps-sdk"
 authors = [{name = "Colm Brandon", email = "colm.brandon@ul.ie"}]
-version = "0.0.17"
+version = "0.0.18"
 description = "The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME"
 readme = "README.rst"
 license = {file = "LICENSE.txt"}
 keywords = ["Highly-plexed Tissue Imaging", "AI",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
```

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/__main__.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/_cli_utils.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/_cli_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/_config.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     _JMS_ADDRESS = f"{os.getenv('JOBS_API_SERVICE_HOST')}:{os.getenv('JOBS_API_SERVICE_PORT')}"
 
     # Minio Config
     _MINIO_ACCESS_KEY = os.getenv('MINIO_ACCESS_KEY')
     _MINIO_SECRET_KEY = os.getenv('MINIO_SECRET_KEY')
     _MINIO_WORKFLOW_BUCKET = os.getenv('MINIO_WORKFLOW_BUCKET')
     _MINIO_EXPERIMENT_BUCKET = os.getenv('MINIO_EXPERIMENT_BUCKET')
-    _MINIO_PRESIGNED_INGRESS_PATH = os.getenv('MINIO_PRESIGNED_INGRESS_PATH')
+    # This is only added for interactive services
+    _MINIO_PRESIGNED_INGRESS_PATH = os.getenv('MINIO_PRESIGNED_INGRESS_PATH') 
     try:
         # This will throw an error if the env var is not set (i.e. in Debug mode)
         _MINIO_NUM_PARALLEL_UPLOADS = int(os.getenv('MINIO_NUM_PARALLEL_UPLOADS'))
     except:
         # Default to 1 for Debug (variable isn't used anyway in Debug mode)
         _MINIO_NUM_PARALLEL_UPLOADS = 1
```

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/_raw_data.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/_raw_data.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/_test_utils.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/_test_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/_utils.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/data.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
         parser_external_url = _urlparse(_os.environ.get('CINCODEBIO_BASE_URL'))
 
          # path to be prepened to the url (path)
         parsed_url = _urlparse(self.url)
         # this is an external url that points to the reverse proxy that ensures Signature is correct
         return parsed_url._replace(
             netloc=parser_external_url.netloc,
-            path=_Config._MINIO_PRESIGNED_INGRESS_PATH + parsed_url.path # prepend the path with the minio presigned path
+            path=str(_Config._MINIO_PRESIGNED_INGRESS_PATH) + parsed_url.path # prepend the path with the minio presigned path
             ).geturl()
 
 
 # Semantic Data Types
 
 class _SemanticData(_ABC):
     def __init__(self) -> None:
```

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/data_utils.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/data_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk/process.py` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk/process.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/PKG-INFO` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.17
+Version: 0.0.18
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
```

### Comparing `cellmaps_sdk-0.0.17/src/cellmaps_sdk.egg-info/SOURCES.txt` & `cellmaps_sdk-0.0.18/src/cellmaps_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

