# Comparing `tmp/abstract_flask-0.0.0.5.tar.gz` & `tmp/abstract_flask-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_flask-0.0.0.5.tar", last modified: Fri May 10 08:14:42 2024, max compression
+gzip compressed data, was "abstract_flask-0.0.0.6.tar", last modified: Fri May 10 08:20:32 2024, max compression
```

## Comparing `abstract_flask-0.0.0.5.tar` & `abstract_flask-0.0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.007147 abstract_flask-0.0.0.5/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.5/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 08:14:42.007147 abstract_flask-0.0.0.5/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 08:14:37.000000 abstract_flask-0.0.0.5/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/src/abstract_flask/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.5/src/abstract_flask/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    12502 2024-05-10 08:14:11.000000 abstract_flask-0.0.0.5/src/abstract_flask/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.5/src/abstract_flask/network_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:14:42.003147 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 08:14:42.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 08:14:41.000000 abstract_flask-0.0.0.5/src/abstract_flask.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.6/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 08:20:27.000000 abstract_flask-0.0.0.6/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.410655 abstract_flask-0.0.0.6/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/src/abstract_flask/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.6/src/abstract_flask/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12493 2024-05-10 08:20:20.000000 abstract_flask-0.0.0.6/src/abstract_flask/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.6/src/abstract_flask/network_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/top_level.txt
```

### Comparing `abstract_flask-0.0.0.5/PKG-INFO` & `abstract_flask-0.0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.5
+Version: 0.0.0.6
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_flask-0.0.0.5/setup.py` & `abstract_flask-0.0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_flask',
-    version='0.0.0.5',
+    version='0.0.0.6',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_flask-0.0.0.5/src/abstract_flask/file_utils.py` & `abstract_flask-0.0.0.6/src/abstract_flask/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         return cls._instances[cls]
 class fileManager(metaclass=SingletonMeta):
     def __init__(self, allowed_extentions=None):
         if not hasattr(self, 'initialized'):
             self.initialized = True
             self.allowed_extentions = allowed_extentions or {'ods','csv','xls','xlsx','xlsb'}        
 class AbsManager(metaclass=SingletonMeta):
-    def __init__(self, allowed_extentions=None):
+    def __init__(self, base_path=None):
         if not hasattr(self, 'initialized'):
             self.initialized = True
             self.base_path = base_path or os.getcwd()
     def _make_dir(self, path):
         """ Create directory if it doesn't exist. """
         os.makedirs(path, exist_ok=True)
         return path
```

### Comparing `abstract_flask-0.0.0.5/src/abstract_flask/network_tools.py` & `abstract_flask-0.0.0.6/src/abstract_flask/network_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.5/src/abstract_flask.egg-info/PKG-INFO` & `abstract_flask-0.0.0.6/src/abstract_flask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.5
+Version: 0.0.0.6
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

