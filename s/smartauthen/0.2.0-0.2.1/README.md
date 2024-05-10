# Comparing `tmp/smartauthen-0.2.0.tar.gz` & `tmp/smartauthen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartauthen-0.2.0.tar", last modified: Wed May  8 04:42:14 2024, max compression
+gzip compressed data, was "smartauthen-0.2.1.tar", last modified: Fri May 10 08:57:17 2024, max compression
```

## Comparing `smartauthen-0.2.0.tar` & `smartauthen-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:42:14.860929 smartauthen-0.2.0/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 04:17:22.000000 smartauthen-0.2.0/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)      184 2024-05-08 04:32:58.000000 smartauthen-0.2.0/MANIFEST.in
--rw-r--r--   0 smart     (1000) smart     (1000)     7575 2024-05-08 04:42:14.860929 smartauthen-0.2.0/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     6349 2024-05-08 04:38:18.000000 smartauthen-0.2.0/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)        0 2024-05-08 04:34:42.000000 smartauthen-0.2.0/requirements.txt
--rw-r--r--   0 smart     (1000) smart     (1000)     1395 2024-05-08 04:42:14.864262 smartauthen-0.2.0/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      485 2024-05-08 04:36:42.000000 smartauthen-0.2.0/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:42:14.854262 smartauthen-0.2.0/smartauthen/
--rw-r--r--   0 smart     (1000) smart     (1000)      511 2024-05-08 04:24:45.000000 smartauthen-0.2.0/smartauthen/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     2161 2024-05-08 04:27:21.000000 smartauthen-0.2.0/smartauthen/auth.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:42:14.860929 smartauthen-0.2.0/smartauthen.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     7575 2024-05-08 04:42:14.000000 smartauthen-0.2.0/smartauthen.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      291 2024-05-08 04:42:14.000000 smartauthen-0.2.0/smartauthen.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 04:42:14.000000 smartauthen-0.2.0/smartauthen.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 04:42:14.000000 smartauthen-0.2.0/smartauthen.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-08 04:42:14.000000 smartauthen-0.2.0/smartauthen.egg-info/top_level.txt
--rw-r--r--   0 smart     (1000) smart     (1000)      121 2024-05-08 04:37:32.000000 smartauthen-0.2.0/tox.ini
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-10 08:57:17.721671 smartauthen-0.2.1/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 04:17:22.000000 smartauthen-0.2.1/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)      184 2024-05-08 04:32:58.000000 smartauthen-0.2.1/MANIFEST.in
+-rw-r--r--   0 smart     (1000) smart     (1000)     7572 2024-05-10 08:57:17.721671 smartauthen-0.2.1/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     6346 2024-05-10 08:56:30.000000 smartauthen-0.2.1/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)        0 2024-05-08 04:34:42.000000 smartauthen-0.2.1/requirements.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)     1395 2024-05-10 08:57:17.725005 smartauthen-0.2.1/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      485 2024-05-08 04:36:42.000000 smartauthen-0.2.1/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-10 08:57:17.718338 smartauthen-0.2.1/smartauthen/
+-rw-r--r--   0 smart     (1000) smart     (1000)      511 2024-05-10 08:55:36.000000 smartauthen-0.2.1/smartauthen/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     2161 2024-05-08 04:27:21.000000 smartauthen-0.2.1/smartauthen/auth.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-10 08:57:17.721671 smartauthen-0.2.1/smartauthen.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     7572 2024-05-10 08:57:17.000000 smartauthen-0.2.1/smartauthen.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      291 2024-05-10 08:57:17.000000 smartauthen-0.2.1/smartauthen.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-10 08:57:17.000000 smartauthen-0.2.1/smartauthen.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-10 08:57:17.000000 smartauthen-0.2.1/smartauthen.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-10 08:57:17.000000 smartauthen-0.2.1/smartauthen.egg-info/top_level.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)      121 2024-05-08 04:37:32.000000 smartauthen-0.2.1/tox.ini
```

### Comparing `smartauthen-0.2.0/LICENSE` & `smartauthen-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartauthen-0.2.0/PKG-INFO` & `smartauthen-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartauthen
-Version: 0.2.0
+Version: 0.2.1
 Summary: Smart, simple, lightweight, secure cross-platform authentication for any application.
 Home-page: https://github.com/smartlegionlab/smartauthen/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartauthen/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartauthen/releases
@@ -60,15 +60,15 @@
 - Windows: 7/8/10.
 - Termux (Android).
 
 ***
 
 ## What's new?
 
-___smartauthen v0.2.0___
+___smartauthen v0.2.1___
 
 ***
 
 ## Description:
 
 ___smartauthen___ - Smart, simple, lightweight, secure cross-platform authentication for any application.
 
@@ -118,15 +118,15 @@
 
 ***
 
 ## Install and Use:
 
 ### Install:
 
-- `pip3 install smartauthen`
+- `pip install smartauthen`
 
 #### Use:
 
 ```python
 from smartauthen import SmartAuth
 
 smart_auth = SmartAuth()
@@ -161,15 +161,15 @@
 
 ***
 
 #### Test coverage:
 
 Coverage 100% !!!
 
-![coverage img](https://github.com/smartlegionlab/smartauthen/raw/master/data/images/smartauthen.png)
+![coverage img](https://github.com/smartlegionlab/smartauth/raw/master/data/images/smartauthen.png)
 
 
 ***
 
 ## Disclaimer of liability:
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
```

### Comparing `smartauthen-0.2.0/README.md` & `smartauthen-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 - Windows: 7/8/10.
 - Termux (Android).
 
 ***
 
 ## What's new?
 
-___smartauthen v0.2.0___
+___smartauthen v0.2.1___
 
 ***
 
 ## Description:
 
 ___smartauthen___ - Smart, simple, lightweight, secure cross-platform authentication for any application.
 
@@ -91,15 +91,15 @@
 
 ***
 
 ## Install and Use:
 
 ### Install:
 
-- `pip3 install smartauthen`
+- `pip install smartauthen`
 
 #### Use:
 
 ```python
 from smartauthen import SmartAuth
 
 smart_auth = SmartAuth()
@@ -134,15 +134,15 @@
 
 ***
 
 #### Test coverage:
 
 Coverage 100% !!!
 
-![coverage img](https://github.com/smartlegionlab/smartauthen/raw/master/data/images/smartauthen.png)
+![coverage img](https://github.com/smartlegionlab/smartauth/raw/master/data/images/smartauthen.png)
 
 
 ***
 
 ## Disclaimer of liability:
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
```

### Comparing `smartauthen-0.2.0/setup.cfg` & `smartauthen-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `smartauthen-0.2.0/smartauthen/auth.py` & `smartauthen-0.2.1/smartauthen/auth.py`

 * *Files identical despite different names*

### Comparing `smartauthen-0.2.0/smartauthen.egg-info/PKG-INFO` & `smartauthen-0.2.1/smartauthen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartauthen
-Version: 0.2.0
+Version: 0.2.1
 Summary: Smart, simple, lightweight, secure cross-platform authentication for any application.
 Home-page: https://github.com/smartlegionlab/smartauthen/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartauthen/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartauthen/releases
@@ -60,15 +60,15 @@
 - Windows: 7/8/10.
 - Termux (Android).
 
 ***
 
 ## What's new?
 
-___smartauthen v0.2.0___
+___smartauthen v0.2.1___
 
 ***
 
 ## Description:
 
 ___smartauthen___ - Smart, simple, lightweight, secure cross-platform authentication for any application.
 
@@ -118,15 +118,15 @@
 
 ***
 
 ## Install and Use:
 
 ### Install:
 
-- `pip3 install smartauthen`
+- `pip install smartauthen`
 
 #### Use:
 
 ```python
 from smartauthen import SmartAuth
 
 smart_auth = SmartAuth()
@@ -161,15 +161,15 @@
 
 ***
 
 #### Test coverage:
 
 Coverage 100% !!!
 
-![coverage img](https://github.com/smartlegionlab/smartauthen/raw/master/data/images/smartauthen.png)
+![coverage img](https://github.com/smartlegionlab/smartauth/raw/master/data/images/smartauthen.png)
 
 
 ***
 
 ## Disclaimer of liability:
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
```

