# Comparing `tmp/abstract_flask-0.0.0.4.tar.gz` & `tmp/abstract_flask-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_flask-0.0.0.4.tar", last modified: Fri May 10 07:29:14 2024, max compression
+gzip compressed data, was "abstract_flask-0.0.0.5.tar", last modified: Fri May 10 08:14:42 2024, max compression
```

## Comparing `abstract_flask-0.0.0.4.tar` & `abstract_flask-0.0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.4/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 07:29:08.000000 abstract_flask-0.0.0.4/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/src/abstract_flask/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.4/src/abstract_flask/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    12916 2024-05-10 07:28:48.000000 abstract_flask-0.0.0.4/src/abstract_flask/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.4/src/abstract_flask/network_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.007147 abstract_flask-0.0.0.5/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.5/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 08:14:42.007147 abstract_flask-0.0.0.5/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 08:14:37.000000 abstract_flask-0.0.0.5/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/src/abstract_flask/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.5/src/abstract_flask/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12502 2024-05-10 08:14:11.000000 abstract_flask-0.0.0.5/src/abstract_flask/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.5/src/abstract_flask/network_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 08:14:42.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/top_level.txt
```

### Comparing `abstract_flask-0.0.0.4/PKG-INFO` & `abstract_flask-0.0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.4
+Version: 0.0.0.5
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_flask-0.0.0.4/setup.py` & `abstract_flask-0.0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_flask',
-    version='0.0.0.4',
+    version='0.0.0.5',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_flask-0.0.0.4/src/abstract_flask/file_utils.py` & `abstract_flask-0.0.0.5/src/abstract_flask/file_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,29 @@
 import os,time,random,hashlib,shutil
 from flask import jsonify
 from werkzeug.utils import secure_filename
 from abstract_pandas import get_df,safe_excel_save,is_file
 from werkzeug.datastructures import FileStorage
 import os
-class fileManager:
-    _instance = None
-
+class SingletonMeta(type):
+    _instances = {}
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super(SingletonMeta, cls).__call__(*args, **kwargs)
+        return cls._instances[cls]
+class fileManager(metaclass=SingletonMeta):
     def __init__(self, allowed_extentions=None):
-        if fileManager._instance is not None:
-            raise Exception("This class is a singleton!")
-        else:
-            fileManager._instance = self
-
-        # Base path is the directory of the script if not specified
-        self.allowed_extentions = allowed_extentions or {'ods','csv','xls','xlsx','xlsb'}
-
-    @staticmethod
-    def get_instance(allowed_extentions=None):
-        if fileManager._instance is None:
-            fileManager(allowed_extentions)
-        return fileManager._instance
-
-        
-class AbsManager:
-    _instance = None
-
-    def __init__(self, base_path=None):
-        if AbsManager._instance is not None:
-            raise Exception("This class is a singleton!")
-        else:
-            AbsManager._instance = self
-
-        # Base path is the directory of the script if not specified
-        self.base_path = base_path or os.path.dirname(os.path.abspath(__file__))
-
-    @staticmethod
-    def get_instance(base_path=None):
-        if AbsManager._instance is None:
-            AbsManager(base_path)
-        return AbsManager._instance
-
+        if not hasattr(self, 'initialized'):
+            self.initialized = True
+            self.allowed_extentions = allowed_extentions or {'ods','csv','xls','xlsx','xlsb'}        
+class AbsManager(metaclass=SingletonMeta):
+    def __init__(self, allowed_extentions=None):
+        if not hasattr(self, 'initialized'):
+            self.initialized = True
+            self.base_path = base_path or os.getcwd()
     def _make_dir(self, path):
         """ Create directory if it doesn't exist. """
         os.makedirs(path, exist_ok=True)
         return path
 
     # Basic directories
     def get_base_path(self):
```

### Comparing `abstract_flask-0.0.0.4/src/abstract_flask/network_tools.py` & `abstract_flask-0.0.0.5/src/abstract_flask/network_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.4/src/abstract_flask.egg-info/PKG-INFO` & `abstract_flask-0.0.0.5/src/abstract_flask.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.4
+Version: 0.0.0.5
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

