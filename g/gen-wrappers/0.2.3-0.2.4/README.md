# Comparing `tmp/gen_wrappers-0.2.3.tar.gz` & `tmp/gen_wrappers-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.2.3.tar", last modified: Fri May  3 21:09:16 2024, max compression
+gzip compressed data, was "gen_wrappers-0.2.4.tar", last modified: Fri May 10 14:33:48 2024, max compression
```

## Comparing `gen_wrappers-0.2.3.tar` & `gen_wrappers-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:16.092317 gen_wrappers-0.2.3/
--rw-rw-rw-   0        0        0      847 2024-05-03 21:09:16.091307 gen_wrappers-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:15.966972 gen_wrappers-0.2.3/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.3/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:15.990488 gen_wrappers-0.2.3/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.3/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6713 2024-05-03 20:01:50.000000 gen_wrappers-0.2.3/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.3/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.3/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:16.013755 gen_wrappers-0.2.3/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.3/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.2.3/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.3/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3028 2024-05-03 21:08:54.000000 gen_wrappers-0.2.3/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.3/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:16.037522 gen_wrappers-0.2.3/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.3/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9441 2024-05-02 21:06:52.000000 gen_wrappers-0.2.3/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.2.3/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.3/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:16.060960 gen_wrappers-0.2.3/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.3/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.3/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.3/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.3/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:16.089311 gen_wrappers-0.2.3/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-03 21:09:15.000000 gen_wrappers-0.2.3/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-03 21:09:15.000000 gen_wrappers-0.2.3/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:09:15.000000 gen_wrappers-0.2.3/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-03 21:09:15.000000 gen_wrappers-0.2.3/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 21:09:15.000000 gen_wrappers-0.2.3/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 21:09:16.092317 gen_wrappers-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-03 21:08:58.000000 gen_wrappers-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:48.476581 gen_wrappers-0.2.4/
+-rw-rw-rw-   0        0        0      847 2024-05-10 14:33:48.474774 gen_wrappers-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:48.248159 gen_wrappers-0.2.4/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.4/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:48.299317 gen_wrappers-0.2.4/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.4/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6713 2024-05-03 20:01:50.000000 gen_wrappers-0.2.4/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.4/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.4/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:48.342206 gen_wrappers-0.2.4/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.4/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.4/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.4/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3028 2024-05-03 21:08:54.000000 gen_wrappers-0.2.4/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.4/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:48.382654 gen_wrappers-0.2.4/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.4/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9441 2024-05-02 21:06:52.000000 gen_wrappers-0.2.4/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.2.4/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.4/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:48.415204 gen_wrappers-0.2.4/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.4/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.4/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.4/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.4/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:48.471439 gen_wrappers-0.2.4/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-10 14:33:48.000000 gen_wrappers-0.2.4/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-10 14:33:48.000000 gen_wrappers-0.2.4/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:33:48.000000 gen_wrappers-0.2.4/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-10 14:33:48.000000 gen_wrappers-0.2.4/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 14:33:48.000000 gen_wrappers-0.2.4/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:33:48.477912 gen_wrappers-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-10 14:32:50.000000 gen_wrappers-0.2.4/setup.py
```

### Comparing `gen_wrappers-0.2.3/PKG-INFO` & `gen_wrappers-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.2.3
+Version: 0.2.4
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.3/creator/auto/creator_auto.py` & `gen_wrappers-0.2.4/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/auto/request_auto.py` & `gen_wrappers-0.2.4/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/auto/response_auto.py` & `gen_wrappers-0.2.4/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/base/base_request.py` & `gen_wrappers-0.2.4/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/base/base_response.py` & `gen_wrappers-0.2.4/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.2.4/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.2.4/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.2.4/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.2.4/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.2.4/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.2.4/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.2.3
+Version: 0.2.4
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.3/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.2.4/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.3/setup.py` & `gen_wrappers-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.2.3',
+    version='0.2.4',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

