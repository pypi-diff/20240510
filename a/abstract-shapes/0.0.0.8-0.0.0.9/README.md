# Comparing `tmp/abstract_shapes-0.0.0.8.tar.gz` & `tmp/abstract_shapes-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_shapes-0.0.0.8.tar", last modified: Wed May  8 21:49:29 2024, max compression
+gzip compressed data, was "abstract_shapes-0.0.0.9.tar", last modified: Wed May  8 21:50:27 2024, max compression
```

## Comparing `abstract_shapes-0.0.0.8.tar` & `abstract_shapes-0.0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:49:29.083185 abstract_shapes-0.0.0.8/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      527 2024-05-08 21:49:29.083185 abstract_shapes-0.0.0.8/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.8/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-08 21:49:29.083185 abstract_shapes-0.0.0.8/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      933 2024-05-08 21:49:24.000000 abstract_shapes-0.0.0.8/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:49:29.083185 abstract_shapes-0.0.0.8/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:49:29.083185 abstract_shapes-0.0.0.8/src/abstract_shapes/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      120 2024-05-08 21:40:35.000000 abstract_shapes-0.0.0.8/src/abstract_shapes/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2565 2024-05-08 21:37:06.000000 abstract_shapes-0.0.0.8/src/abstract_shapes/abstractShapeManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3664 2024-05-08 21:34:26.000000 abstract_shapes-0.0.0.8/src/abstract_shapes/cardinalDirections.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5311 2024-05-08 21:39:03.000000 abstract_shapes-0.0.0.8/src/abstract_shapes/direction.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2297 2024-05-08 20:51:19.000000 abstract_shapes-0.0.0.8/src/abstract_shapes/fileAssociations.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3398 2024-05-08 21:49:05.000000 abstract_shapes-0.0.0.8/src/abstract_shapes/file_associations.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3377 2024-05-08 21:36:00.000000 abstract_shapes-0.0.0.8/src/abstract_shapes/transform.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:49:29.083185 abstract_shapes-0.0.0.8/src/abstract_shapes.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      527 2024-05-08 21:49:29.000000 abstract_shapes-0.0.0.8/src/abstract_shapes.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      497 2024-05-08 21:49:29.000000 abstract_shapes-0.0.0.8/src/abstract_shapes.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-08 21:49:29.000000 abstract_shapes-0.0.0.8/src/abstract_shapes.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       24 2024-05-08 21:49:29.000000 abstract_shapes-0.0.0.8/src/abstract_shapes.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-08 21:49:29.000000 abstract_shapes-0.0.0.8/src/abstract_shapes.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:50:27.706601 abstract_shapes-0.0.0.9/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      527 2024-05-08 21:50:27.706601 abstract_shapes-0.0.0.9/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.9/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-08 21:50:27.706601 abstract_shapes-0.0.0.9/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      933 2024-05-08 21:50:22.000000 abstract_shapes-0.0.0.9/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:50:27.702601 abstract_shapes-0.0.0.9/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:50:27.702601 abstract_shapes-0.0.0.9/src/abstract_shapes/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      119 2024-05-08 21:50:03.000000 abstract_shapes-0.0.0.9/src/abstract_shapes/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2565 2024-05-08 21:37:06.000000 abstract_shapes-0.0.0.9/src/abstract_shapes/abstractShapeManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3664 2024-05-08 21:34:26.000000 abstract_shapes-0.0.0.9/src/abstract_shapes/cardinalDirections.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5311 2024-05-08 21:39:03.000000 abstract_shapes-0.0.0.9/src/abstract_shapes/direction.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2297 2024-05-08 20:51:19.000000 abstract_shapes-0.0.0.9/src/abstract_shapes/fileAssociations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3398 2024-05-08 21:49:05.000000 abstract_shapes-0.0.0.9/src/abstract_shapes/file_associations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3377 2024-05-08 21:36:00.000000 abstract_shapes-0.0.0.9/src/abstract_shapes/transform.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:50:27.706601 abstract_shapes-0.0.0.9/src/abstract_shapes.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      527 2024-05-08 21:50:27.000000 abstract_shapes-0.0.0.9/src/abstract_shapes.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      497 2024-05-08 21:50:27.000000 abstract_shapes-0.0.0.9/src/abstract_shapes.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-08 21:50:27.000000 abstract_shapes-0.0.0.9/src/abstract_shapes.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       24 2024-05-08 21:50:27.000000 abstract_shapes-0.0.0.9/src/abstract_shapes.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-08 21:50:27.000000 abstract_shapes-0.0.0.9/src/abstract_shapes.egg-info/top_level.txt
```

### Comparing `abstract_shapes-0.0.0.8/PKG-INFO` & `abstract_shapes-0.0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.8
+Version: 0.0.0.9
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_shapes-0.0.0.8/setup.py` & `abstract_shapes-0.0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_shapes',
-    version='0.0.0.8',
+    version='0.0.0.9',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_shapes-0.0.0.8/src/abstract_shapes/abstractShapeManager.py` & `abstract_shapes-0.0.0.9/src/abstract_shapes/abstractShapeManager.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.8/src/abstract_shapes/cardinalDirections.py` & `abstract_shapes-0.0.0.9/src/abstract_shapes/cardinalDirections.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.8/src/abstract_shapes/direction.py` & `abstract_shapes-0.0.0.9/src/abstract_shapes/direction.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.8/src/abstract_shapes/fileAssociations.py` & `abstract_shapes-0.0.0.9/src/abstract_shapes/fileAssociations.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.8/src/abstract_shapes/file_associations.py` & `abstract_shapes-0.0.0.9/src/abstract_shapes/file_associations.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.8/src/abstract_shapes/transform.py` & `abstract_shapes-0.0.0.9/src/abstract_shapes/transform.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.8/src/abstract_shapes.egg-info/PKG-INFO` & `abstract_shapes-0.0.0.9/src/abstract_shapes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.8
+Version: 0.0.0.9
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

