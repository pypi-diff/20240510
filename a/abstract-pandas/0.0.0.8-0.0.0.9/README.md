# Comparing `tmp/abstract_pandas-0.0.0.8.tar.gz` & `tmp/abstract_pandas-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.8.tar", last modified: Sat May  4 03:11:59 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.9.tar", last modified: Sun May  5 07:38:06 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.8.tar` & `abstract_pandas-0.0.0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:11:59.154282 abstract_pandas-0.0.0.8/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-04 03:11:59.154282 abstract_pandas-0.0.0.8/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.8/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-04 03:11:59.154282 abstract_pandas-0.0.0.8/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-05-04 03:11:54.000000 abstract_pandas-0.0.0.8/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:11:59.154282 abstract_pandas-0.0.0.8/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:11:59.154282 abstract_pandas-0.0.0.8/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/class_manager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    15968 2024-05-04 03:09:19.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5669 2024-05-04 03:11:47.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/geo_pandas.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/geo_spec.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      290 2024-05-03 07:49:52.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/test_sol.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.8/src/abstract_pandas/time_module.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:11:59.154282 abstract_pandas-0.0.0.8/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-04 03:11:59.000000 abstract_pandas-0.0.0.8/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      544 2024-05-04 03:11:59.000000 abstract_pandas-0.0.0.8/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-04 03:11:59.000000 abstract_pandas-0.0.0.8/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-04 03:11:59.000000 abstract_pandas-0.0.0.8/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-04 03:11:59.000000 abstract_pandas-0.0.0.8/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.9/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-05-05 07:37:55.000000 abstract_pandas-0.0.0.9/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.519038 abstract_pandas-0.0.0.9/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       54 2024-05-05 03:13:48.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/depriciated.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     6291 2024-05-05 07:04:33.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/excel_classes.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    23630 2024-05-05 07:26:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8967 2024-05-05 07:35:43.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7154 2024-05-05 07:23:50.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2731 2024-05-05 06:13:53.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/landManager.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      515 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.8/PKG-INFO` & `abstract_pandas-0.0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
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

### Comparing `abstract_pandas-0.0.0.8/setup.py` & `abstract_pandas-0.0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
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

### Comparing `abstract_pandas-0.0.0.8/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.9/src/abstract_pandas/excel_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abstract_webgui import *
+from abstract_gui import *
 import os
 from openpyxl import load_workbook
 import pandas as pd
 from os.path import isfile,splitext,basename,dirname,isdir,exists,join
 MAX_CELLS = 400  # Example limit
 
 from abstract_utilities import make_list
```

### Comparing `abstract_pandas-0.0.0.8/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
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

