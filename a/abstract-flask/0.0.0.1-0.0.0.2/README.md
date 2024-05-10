# Comparing `tmp/abstract_flask-0.0.0.1.tar.gz` & `tmp/abstract_flask-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_flask-0.0.0.1.tar", last modified: Fri May 10 05:53:36 2024, max compression
+gzip compressed data, was "abstract_flask-0.0.0.2.tar", last modified: Fri May 10 05:58:25 2024, max compression
```

## Comparing `abstract_flask-0.0.0.1.tar` & `abstract_flask-0.0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:53:36.648301 abstract_flask-0.0.0.1/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 05:53:36.648301 abstract_flask-0.0.0.1/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.1/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 05:53:36.648301 abstract_flask-0.0.0.1/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 05:53:31.000000 abstract_flask-0.0.0.1/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:53:36.648301 abstract_flask-0.0.0.1/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:53:36.648301 abstract_flask-0.0.0.1/src/abstract_flask/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.1/src/abstract_flask/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    11215 2024-05-10 01:11:12.000000 abstract_flask-0.0.0.1/src/abstract_flask/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.1/src/abstract_flask/network_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:53:36.648301 abstract_flask-0.0.0.1/src/abstract_flask.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 05:53:36.000000 abstract_flask-0.0.0.1/src/abstract_flask.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 05:53:36.000000 abstract_flask-0.0.0.1/src/abstract_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 05:53:36.000000 abstract_flask-0.0.0.1/src/abstract_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 05:53:36.000000 abstract_flask-0.0.0.1/src/abstract_flask.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 05:53:36.000000 abstract_flask-0.0.0.1/src/abstract_flask.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:58:25.777412 abstract_flask-0.0.0.2/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 05:58:25.777412 abstract_flask-0.0.0.2/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.2/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 05:58:25.777412 abstract_flask-0.0.0.2/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 05:57:35.000000 abstract_flask-0.0.0.2/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:58:25.773412 abstract_flask-0.0.0.2/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:58:25.777412 abstract_flask-0.0.0.2/src/abstract_flask/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.2/src/abstract_flask/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    11215 2024-05-10 01:11:12.000000 abstract_flask-0.0.0.2/src/abstract_flask/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.2/src/abstract_flask/network_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:58:25.777412 abstract_flask-0.0.0.2/src/abstract_flask.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 05:58:25.000000 abstract_flask-0.0.0.2/src/abstract_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 05:58:25.000000 abstract_flask-0.0.0.2/src/abstract_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 05:58:25.000000 abstract_flask-0.0.0.2/src/abstract_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 05:58:25.000000 abstract_flask-0.0.0.2/src/abstract_flask.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 05:58:25.000000 abstract_flask-0.0.0.2/src/abstract_flask.egg-info/top_level.txt
```

### Comparing `abstract_flask-0.0.0.1/PKG-INFO` & `abstract_flask-0.0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_flask-0.0.0.1/setup.py` & `abstract_flask-0.0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_flask',
-    version='0.0.0.1',
+    version='0.0.0.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_flask-0.0.0.1/src/abstract_flask/file_utils.py` & `abstract_flask-0.0.0.2/src/abstract_flask/file_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.1/src/abstract_flask/network_tools.py` & `abstract_flask-0.0.0.2/src/abstract_flask/network_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.1/src/abstract_flask.egg-info/PKG-INFO` & `abstract_flask-0.0.0.2/src/abstract_flask.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

