# Comparing `tmp/mfprocess-1.0.8.tar.gz` & `tmp/mfprocess-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-1.0.8.tar", last modified: Thu May  9 14:29:46 2024, max compression
+gzip compressed data, was "mfprocess-1.0.9.tar", last modified: Thu May  9 14:36:21 2024, max compression
```

## Comparing `mfprocess-1.0.8.tar` & `mfprocess-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:29:46.655682 mfprocess-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 14:29:42.000000 mfprocess-1.0.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 14:29:46.655682 mfprocess-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 14:29:42.000000 mfprocess-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:29:46.655682 mfprocess-1.0.8/mfprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 14:29:42.000000 mfprocess-1.0.8/mfprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-09 14:29:42.000000 mfprocess-1.0.8/mfprocess/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:29:46.655682 mfprocess-1.0.8/mfprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 14:29:46.000000 mfprocess-1.0.8/mfprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 14:29:46.000000 mfprocess-1.0.8/mfprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:29:46.000000 mfprocess-1.0.8/mfprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 14:29:46.000000 mfprocess-1.0.8/mfprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 14:29:46.000000 mfprocess-1.0.8/mfprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:29:46.655682 mfprocess-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 14:29:44.000000 mfprocess-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:36:21.308143 mfprocess-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 14:36:16.000000 mfprocess-1.0.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 14:36:21.308143 mfprocess-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 14:36:16.000000 mfprocess-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:36:21.304143 mfprocess-1.0.9/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 14:36:16.000000 mfprocess-1.0.9/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-09 14:36:16.000000 mfprocess-1.0.9/mfprocess/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:36:21.308143 mfprocess-1.0.9/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 14:36:21.000000 mfprocess-1.0.9/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 14:36:21.000000 mfprocess-1.0.9/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:36:21.000000 mfprocess-1.0.9/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 14:36:21.000000 mfprocess-1.0.9/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 14:36:21.000000 mfprocess-1.0.9/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:36:21.308143 mfprocess-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 14:36:19.000000 mfprocess-1.0.9/setup.py
```

### Comparing `mfprocess-1.0.8/LICENCE` & `mfprocess-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-1.0.8/PKG-INFO` & `mfprocess-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.8
+Version: 1.0.9
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.8/mfprocess/functions.py` & `mfprocess-1.0.9/mfprocess/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import pycountry
 import time
 import openai
 import urllib.parse
 import json
 import datetime
+try:
+ from google.colab import drive
+except:
+   print("You are not in Colab")
 
 def input_path(message=""):  #translate copy path of windows
   
   raw_s=input(message) if message=="" else message
   raw_s=raw_s.replace(r'"','')
   return "/content/drive/Shareddrives/"+'/'.join(raw_s.split("\\")[2:])
```

### Comparing `mfprocess-1.0.8/mfprocess.egg-info/PKG-INFO` & `mfprocess-1.0.9/mfprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.8
+Version: 1.0.9
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.8/setup.py` & `mfprocess-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '1.0.8',  #'0.0.4',   #
+    version= '1.0.9',  #'0.0.4',   #
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

