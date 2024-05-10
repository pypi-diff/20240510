# Comparing `tmp/iaklogger-1.0.6.tar.gz` & `tmp/iaklogger-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaklogger-1.0.6.tar", last modified: Fri May 10 13:43:18 2024, max compression
+gzip compressed data, was "iaklogger-1.0.7.tar", last modified: Fri May 10 14:33:43 2024, max compression
```

## Comparing `iaklogger-1.0.6.tar` & `iaklogger-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:18.245875 iaklogger-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 13:43:18.245875 iaklogger-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-10 13:43:14.000000 iaklogger-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:18.245875 iaklogger-1.0.6/iaklogger/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 13:43:14.000000 iaklogger-1.0.6/iaklogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-10 13:43:14.000000 iaklogger-1.0.6/iaklogger/iaklogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-10 13:43:14.000000 iaklogger-1.0.6/iaklogger/test_iaklogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:18.245875 iaklogger-1.0.6/iaklogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 13:43:18.245875 iaklogger-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-10 13:43:14.000000 iaklogger-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:43.453414 iaklogger-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 14:33:43.453414 iaklogger-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-10 14:33:34.000000 iaklogger-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:43.453414 iaklogger-1.0.7/iaklogger/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-10 14:33:34.000000 iaklogger-1.0.7/iaklogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-10 14:33:34.000000 iaklogger-1.0.7/iaklogger/iaklogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-10 14:33:34.000000 iaklogger-1.0.7/iaklogger/test_iaklogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:43.453414 iaklogger-1.0.7/iaklogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 14:33:43.000000 iaklogger-1.0.7/iaklogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-10 14:33:43.000000 iaklogger-1.0.7/iaklogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:33:43.000000 iaklogger-1.0.7/iaklogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 14:33:43.000000 iaklogger-1.0.7/iaklogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 14:33:43.457414 iaklogger-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-10 14:33:34.000000 iaklogger-1.0.7/setup.py
```

### Comparing `iaklogger-1.0.6/PKG-INFO` & `iaklogger-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaklogger
-Version: 1.0.6
+Version: 1.0.7
 Summary: Very basic and easy logger
 Home-page: https://github.com/Iakl/iaklogger
 Download-URL: https://github.com/Iakl/iaklogger/archive/refs/tags/v1.0.0.tar.gz
 Author: Iakl
 Author-email: estebaniakl@gmail.com
 License: MIT
 Keywords: logger,easy,print,log,basic,logging
```

### Comparing `iaklogger-1.0.6/README.md` & `iaklogger-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `iaklogger-1.0.6/iaklogger/iaklogger.py` & `iaklogger-1.0.7/iaklogger/iaklogger.py`

 * *Files identical despite different names*

### Comparing `iaklogger-1.0.6/iaklogger/test_iaklogger.py` & `iaklogger-1.0.7/iaklogger/test_iaklogger.py`

 * *Files identical despite different names*

### Comparing `iaklogger-1.0.6/iaklogger.egg-info/PKG-INFO` & `iaklogger-1.0.7/iaklogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaklogger
-Version: 1.0.6
+Version: 1.0.7
 Summary: Very basic and easy logger
 Home-page: https://github.com/Iakl/iaklogger
 Download-URL: https://github.com/Iakl/iaklogger/archive/refs/tags/v1.0.0.tar.gz
 Author: Iakl
 Author-email: estebaniakl@gmail.com
 License: MIT
 Keywords: logger,easy,print,log,basic,logging
```

### Comparing `iaklogger-1.0.6/setup.py` & `iaklogger-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
     name='iaklogger',         # How you named your package folder (MyLib)
     packages=['iaklogger'],   # Chose the same as "name"
-    version='1.0.6',      # Start with a small number and increase it with every change you make
+    version='1.0.7',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Very basic and easy logger',
     long_description='Very basic and easy logger for python. It allows to print logs to the console and/or to a file. It also allows to mute logs by tags, mute all logs, show tags before the message, show time before the message, and set a maximum size for the log file.',
     author='Iakl',                   # Type in your name
     author_email='estebaniakl@gmail.com',      # Type in your E-Mail
```

