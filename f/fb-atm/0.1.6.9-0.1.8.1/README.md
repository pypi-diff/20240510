# Comparing `tmp/fb_atm-0.1.6.9.tar.gz` & `tmp/fb_atm-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_atm-0.1.6.9.tar", last modified: Fri May 10 19:54:05 2024, max compression
+gzip compressed data, was "fb_atm-0.1.8.1.tar", last modified: Fri May 10 21:01:23 2024, max compression
```

## Comparing `fb_atm-0.1.6.9.tar` & `fb_atm-0.1.8.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:54:05.471115 fb_atm-0.1.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 19:54:05.471115 fb_atm-0.1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-10 19:54:01.000000 fb_atm-0.1.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:54:05.471115 fb_atm-0.1.6.9/fb_atm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 19:54:05.000000 fb_atm-0.1.6.9/fb_atm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-10 19:54:05.000000 fb_atm-0.1.6.9/fb_atm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:54:05.000000 fb_atm-0.1.6.9/fb_atm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 19:54:05.000000 fb_atm-0.1.6.9/fb_atm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:54:05.000000 fb_atm-0.1.6.9/fb_atm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 19:54:05.000000 fb_atm-0.1.6.9/fb_atm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 19:54:05.000000 fb_atm-0.1.6.9/fb_atm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:54:05.471115 fb_atm-0.1.6.9/mahdix/
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-10 19:54:01.000000 fb_atm-0.1.6.9/mahdix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-10 19:54:01.000000 fb_atm-0.1.6.9/mahdix/mat.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:54:05.471115 fb_atm-0.1.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-10 19:54:01.000000 fb_atm-0.1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-10 21:01:19.000000 fb_atm-0.1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/fb_atm/
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-10 21:01:19.000000 fb_atm-0.1.8.1/fb_atm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/fb_atm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-10 21:01:19.000000 fb_atm-0.1.8.1/setup.py
```

### Comparing `fb_atm-0.1.6.9/PKG-INFO` & `fb_atm-0.1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_atm
-Version: 0.1.6.9
+Version: 0.1.8.1
 Summary: An application that informs you of the different modules and very easy to use.
 Home-page: https://www.facebook.com/bk4human
 Author: Mahdi Hasan Shuvo
 Author-email: shvo.mex@gmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/Shuvo-BBHH/
 Project-URL: Bug Reports, https://www.facebook.com/bk4human
```

### Comparing `fb_atm-0.1.6.9/README.md` & `fb_atm-0.1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `fb_atm-0.1.6.9/fb_atm.egg-info/PKG-INFO` & `fb_atm-0.1.8.1/fb_atm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_atm
-Version: 0.1.6.9
+Version: 0.1.8.1
 Summary: An application that informs you of the different modules and very easy to use.
 Home-page: https://www.facebook.com/bk4human
 Author: Mahdi Hasan Shuvo
 Author-email: shvo.mex@gmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/Shuvo-BBHH/
 Project-URL: Bug Reports, https://www.facebook.com/bk4human
```

### Comparing `fb_atm-0.1.6.9/mahdix/__init__.py` & `fb_atm-0.1.8.1/fb_atm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import imp
+
 import re,requests
 from mahdix import *
 import urllib.parse
 from bs4 import BeautifulSoup as bs
 clear()
 class Page:
     def __init__(self):
```

### Comparing `fb_atm-0.1.6.9/setup.py` & `fb_atm-0.1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 long_description='Mahdi Hasan Shuvo'
 setup(
     name="fb_atm",
-    version='0.1.6.9',
+    version='0.1.8.1',
     author="Mahdi Hasan Shuvo",
     author_email="shvo.mex@gmail.com",
     url="https://www.facebook.com/bk4human",
     description="An application that informs you of the different modules and very easy to use.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

