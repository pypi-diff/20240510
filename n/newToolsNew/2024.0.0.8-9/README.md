# Comparing `tmp/newToolsNew-2024.0.0.8.tar.gz` & `tmp/newToolsNew-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newToolsNew-2024.0.0.8.tar", last modified: Thu May  9 13:19:14 2024, max compression
+gzip compressed data, was "newToolsNew-9.tar", last modified: Thu May  9 13:21:46 2024, max compression
```

## Comparing `newToolsNew-2024.0.0.8.tar` & `newToolsNew-9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:19:14.338225 newToolsNew-2024.0.0.8/
--rw-rw-rw-   0        0        0      268 2024-05-09 13:19:14.336231 newToolsNew-2024.0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 13:19:14.329249 newToolsNew-2024.0.0.8/newToolsNew.egg-info/
--rw-rw-rw-   0        0        0      268 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      101 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 13:19:14.333238 newToolsNew-2024.0.0.8/newUtils/
--rw-rw-rw-   0        0        0      875 2024-05-09 12:56:12.000000 newToolsNew-2024.0.0.8/newUtils/logger.py
--rw-rw-rw-   0        0        0       42 2024-05-09 13:19:14.338225 newToolsNew-2024.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-05-09 13:19:09.000000 newToolsNew-2024.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:21:46.720554 newToolsNew-9/
+-rw-rw-rw-   0        0        0      259 2024-05-09 13:21:46.718560 newToolsNew-9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 13:21:46.702603 newToolsNew-9/newToolsNew.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-05-09 13:21:46.000000 newToolsNew-9/newToolsNew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-09 13:21:46.000000 newToolsNew-9/newToolsNew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:21:46.000000 newToolsNew-9/newToolsNew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-09 13:21:46.000000 newToolsNew-9/newToolsNew.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2024-05-09 13:21:46.000000 newToolsNew-9/newToolsNew.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 13:21:46.000000 newToolsNew-9/newToolsNew.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 13:21:46.712575 newToolsNew-9/newUtils/
+-rw-rw-rw-   0        0        0      128 2024-05-09 12:36:22.000000 newToolsNew-9/newUtils/__init__.py
+-rw-rw-rw-   0        0        0      875 2024-05-09 12:56:12.000000 newToolsNew-9/newUtils/logger.py
+-rw-rw-rw-   0        0        0     1113 2024-05-09 13:11:06.000000 newToolsNew-9/newUtils/wechatRobot.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:21:46.720554 newToolsNew-9/setup.cfg
+-rw-rw-rw-   0        0        0      797 2024-05-09 13:21:42.000000 newToolsNew-9/setup.py
```

### Comparing `newToolsNew-2024.0.0.8/newUtils/logger.py` & `newToolsNew-9/newUtils/logger.py`

 * *Files identical despite different names*

### Comparing `newToolsNew-2024.0.0.8/setup.py` & `newToolsNew-9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python 
 # -*- coding:utf-8 -*-
 # @time     : 2024/5/9 17:47
 # @Author   : new
 # @File      : setup.py
 from setuptools import setup, find_packages
 
-GFICLEE_VERSION = '2024.0.0.8'
+GFICLEE_VERSION = '9'
 
 setup(
     name='newToolsNew',
     version=GFICLEE_VERSION,
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

