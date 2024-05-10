# Comparing `tmp/cloudframework-1.0.8.tar.gz` & `tmp/cloudframework-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudframework-1.0.8.tar", last modified: Sun Mar 28 08:45:41 2021, max compression
+gzip compressed data, was "cloudframework-1.0.9.tar", last modified: Sun Mar 28 08:46:09 2021, max compression
```

## Comparing `cloudframework-1.0.8.tar` & `cloudframework-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:45:41.430396 cloudframework-1.0.8/
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      718 2021-03-28 08:45:41.430086 cloudframework-1.0.8/PKG-INFO
--rw-r--r--   0 adrianmartinez   (501) staff       (20)     1587 2021-03-28 07:40:12.000000 cloudframework-1.0.8/README.md
-drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:45:41.425813 cloudframework-1.0.8/cloudframework/
--rw-r--r--   0 adrianmartinez   (501) staff       (20)    18531 2021-03-28 08:44:17.000000 cloudframework-1.0.8/cloudframework/CoreFlask.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)     5990 2021-03-27 11:51:08.000000 cloudframework-1.0.8/cloudframework/RESTFul.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      194 2021-03-28 05:58:15.000000 cloudframework-1.0.8/cloudframework/__init__.py
-drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:45:41.428014 cloudframework-1.0.8/cloudframework/api/
--rw-r--r--   0 adrianmartinez   (501) staff       (20)        0 2021-03-27 10:08:35.000000 cloudframework-1.0.8/cloudframework/api/__init__.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      227 2021-03-27 10:24:56.000000 cloudframework-1.0.8/cloudframework/api/_notfound.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      401 2021-03-28 08:43:57.000000 cloudframework-1.0.8/cloudframework/api/_version.py
-drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:45:41.429273 cloudframework-1.0.8/cloudframework/lib/
--rw-r--r--   0 adrianmartinez   (501) staff       (20)       23 2021-03-27 06:40:06.000000 cloudframework-1.0.8/cloudframework/lib/Buckets.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      107 2021-03-27 06:40:06.000000 cloudframework-1.0.8/cloudframework/lib/DataSQL.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      665 2021-03-27 06:40:06.000000 cloudframework-1.0.8/cloudframework/lib/DataStore.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)       22 2021-03-27 06:40:06.000000 cloudframework-1.0.8/cloudframework/lib/Email.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)        0 2021-03-27 06:40:06.000000 cloudframework-1.0.8/cloudframework/lib/__init__.py
-drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:45:41.429684 cloudframework-1.0.8/cloudframework/python-dist/
--rw-r--r--   0 adrianmartinez   (501) staff       (20)        0 2021-03-27 06:40:06.000000 cloudframework-1.0.8/cloudframework/python-dist/__init__.py
--rw-r--r--   0 adrianmartinez   (501) staff       (20)     1467 2021-03-27 10:56:43.000000 cloudframework-1.0.8/cloudframework/python-dist/main.py
-drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:45:41.427269 cloudframework-1.0.8/cloudframework.egg-info/
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      718 2021-03-28 08:45:41.000000 cloudframework-1.0.8/cloudframework.egg-info/PKG-INFO
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      607 2021-03-28 08:45:41.000000 cloudframework-1.0.8/cloudframework.egg-info/SOURCES.txt
--rw-r--r--   0 adrianmartinez   (501) staff       (20)        1 2021-03-28 08:45:41.000000 cloudframework-1.0.8/cloudframework.egg-info/dependency_links.txt
--rw-r--r--   0 adrianmartinez   (501) staff       (20)       20 2021-03-28 08:45:41.000000 cloudframework-1.0.8/cloudframework.egg-info/requires.txt
--rw-r--r--   0 adrianmartinez   (501) staff       (20)       15 2021-03-28 08:45:41.000000 cloudframework-1.0.8/cloudframework.egg-info/top_level.txt
--rw-r--r--   0 adrianmartinez   (501) staff       (20)       38 2021-03-28 08:45:41.430487 cloudframework-1.0.8/setup.cfg
--rw-r--r--   0 adrianmartinez   (501) staff       (20)      950 2021-03-28 08:44:31.000000 cloudframework-1.0.8/setup.py
+drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:46:09.621464 cloudframework-1.0.9/
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      718 2021-03-28 08:46:09.621138 cloudframework-1.0.9/PKG-INFO
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)     1587 2021-03-28 07:40:12.000000 cloudframework-1.0.9/README.md
+drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:46:09.616488 cloudframework-1.0.9/cloudframework/
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)    18531 2021-03-28 08:44:17.000000 cloudframework-1.0.9/cloudframework/CoreFlask.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)     5990 2021-03-27 11:51:08.000000 cloudframework-1.0.9/cloudframework/RESTFul.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      194 2021-03-28 05:58:15.000000 cloudframework-1.0.9/cloudframework/__init__.py
+drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:46:09.618741 cloudframework-1.0.9/cloudframework/api/
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)        0 2021-03-27 10:08:35.000000 cloudframework-1.0.9/cloudframework/api/__init__.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      227 2021-03-27 10:24:56.000000 cloudframework-1.0.9/cloudframework/api/_notfound.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      401 2021-03-28 08:43:57.000000 cloudframework-1.0.9/cloudframework/api/_version.py
+drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:46:09.620274 cloudframework-1.0.9/cloudframework/lib/
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)       23 2021-03-27 06:40:06.000000 cloudframework-1.0.9/cloudframework/lib/Buckets.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      107 2021-03-27 06:40:06.000000 cloudframework-1.0.9/cloudframework/lib/DataSQL.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      665 2021-03-27 06:40:06.000000 cloudframework-1.0.9/cloudframework/lib/DataStore.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)       22 2021-03-27 06:40:06.000000 cloudframework-1.0.9/cloudframework/lib/Email.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)        0 2021-03-27 06:40:06.000000 cloudframework-1.0.9/cloudframework/lib/__init__.py
+drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:46:09.620699 cloudframework-1.0.9/cloudframework/python-dist/
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)        0 2021-03-27 06:40:06.000000 cloudframework-1.0.9/cloudframework/python-dist/__init__.py
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)     1467 2021-03-27 10:56:43.000000 cloudframework-1.0.9/cloudframework/python-dist/main.py
+drwxr-xr-x   0 adrianmartinez   (501) staff       (20)        0 2021-03-28 08:46:09.617939 cloudframework-1.0.9/cloudframework.egg-info/
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      718 2021-03-28 08:46:09.000000 cloudframework-1.0.9/cloudframework.egg-info/PKG-INFO
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      607 2021-03-28 08:46:09.000000 cloudframework-1.0.9/cloudframework.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)        1 2021-03-28 08:46:09.000000 cloudframework-1.0.9/cloudframework.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)       20 2021-03-28 08:46:09.000000 cloudframework-1.0.9/cloudframework.egg-info/requires.txt
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)       15 2021-03-28 08:46:09.000000 cloudframework-1.0.9/cloudframework.egg-info/top_level.txt
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)       38 2021-03-28 08:46:09.621562 cloudframework-1.0.9/setup.cfg
+-rw-r--r--   0 adrianmartinez   (501) staff       (20)      950 2021-03-28 08:46:00.000000 cloudframework-1.0.9/setup.py
```

### Comparing `cloudframework-1.0.8/PKG-INFO` & `cloudframework-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudframework
-Version: 1.0.8
+Version: 1.0.9
 Summary: CloudFramework for Appengine using python language.
 Home-page: https://github.com/CloudFramework-io/appengine-python-core-3.9
 Author: CloudFramework Team
 Author-email: tools@cloudframework.io
 License: UNKNOWN
 Description: This framework has been created to make easier the API creation and backend logic to deploy over GCP Appengine Serverless solution. You are free to use Native python or other libraries when you want. We hope you enjoy it :).
 Platform: UNKNOWN
```

### Comparing `cloudframework-1.0.8/README.md` & `cloudframework-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudframework-1.0.8/cloudframework/CoreFlask.py` & `cloudframework-1.0.9/cloudframework/CoreFlask.py`

 * *Files identical despite different names*

### Comparing `cloudframework-1.0.8/cloudframework/RESTFul.py` & `cloudframework-1.0.9/cloudframework/RESTFul.py`

 * *Files identical despite different names*

### Comparing `cloudframework-1.0.8/cloudframework/lib/DataStore.py` & `cloudframework-1.0.9/cloudframework/lib/DataStore.py`

 * *Files identical despite different names*

### Comparing `cloudframework-1.0.8/cloudframework/python-dist/main.py` & `cloudframework-1.0.9/cloudframework/python-dist/main.py`

 * *Files identical despite different names*

### Comparing `cloudframework-1.0.8/cloudframework.egg-info/PKG-INFO` & `cloudframework-1.0.9/cloudframework.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudframework
-Version: 1.0.8
+Version: 1.0.9
 Summary: CloudFramework for Appengine using python language.
 Home-page: https://github.com/CloudFramework-io/appengine-python-core-3.9
 Author: CloudFramework Team
 Author-email: tools@cloudframework.io
 License: UNKNOWN
 Description: This framework has been created to make easier the API creation and backend logic to deploy over GCP Appengine Serverless solution. You are free to use Native python or other libraries when you want. We hope you enjoy it :).
 Platform: UNKNOWN
```

### Comparing `cloudframework-1.0.8/cloudframework.egg-info/SOURCES.txt` & `cloudframework-1.0.9/cloudframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudframework-1.0.8/setup.py` & `cloudframework-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cloudframework",
-    version="1.0.8",
+    version="1.0.9",
     author="CloudFramework Team",
     author_email="tools@cloudframework.io",
     description="CloudFramework for Appengine using python language.",
     long_description="This framework has been created to make easier the API creation and backend logic to deploy over GCP Appengine Serverless solution. You are free to use Native python or other libraries when you want. We hope you enjoy it :).",
     long_description_content_type="text/markdown",
     url="https://github.com/CloudFramework-io/appengine-python-core-3.9",
     packages=setuptools.find_packages(),
```

