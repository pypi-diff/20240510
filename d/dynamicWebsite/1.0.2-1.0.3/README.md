# Comparing `tmp/dynamicwebsite-1.0.2.tar.gz` & `tmp/dynamicwebsite-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicwebsite-1.0.2.tar", last modified: Sat Apr 27 15:27:11 2024, max compression
+gzip compressed data, was "dynamicwebsite-1.0.3.tar", last modified: Fri May 10 21:41:41 2024, max compression
```

## Comparing `dynamicwebsite-1.0.2.tar` & `dynamicwebsite-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-27 15:27:06.000000 dynamicwebsite-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 15:27:11.000000 dynamicwebsite-1.0.2/dynamicWebsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-04-27 15:27:06.000000 dynamicwebsite-1.0.2/dynamicWebsite.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-27 15:27:06.000000 dynamicwebsite-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 15:27:11.032208 dynamicwebsite-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:41:41.799135 dynamicwebsite-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-10 21:41:41.799135 dynamicwebsite-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-10 21:41:37.000000 dynamicwebsite-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:41:41.799135 dynamicwebsite-1.0.3/dynamicWebsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-10 21:41:41.000000 dynamicwebsite-1.0.3/dynamicWebsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-10 21:41:41.000000 dynamicwebsite-1.0.3/dynamicWebsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:41:41.000000 dynamicwebsite-1.0.3/dynamicWebsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 21:41:41.000000 dynamicwebsite-1.0.3/dynamicWebsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 21:41:41.000000 dynamicwebsite-1.0.3/dynamicWebsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-05-10 21:41:37.000000 dynamicwebsite-1.0.3/dynamicWebsite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-10 21:41:37.000000 dynamicwebsite-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:41:41.799135 dynamicwebsite-1.0.3/setup.cfg
```

### Comparing `dynamicwebsite-1.0.2/PKG-INFO` & `dynamicwebsite-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: dynamicWebsite
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>, riyapuri0710 <riyapuri0710@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/dynamicWebsite
 Keywords: website,dynamic website,update website,live website,change website,websocket
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: randomisedString
 Requires-Dist: cryptography
 Requires-Dist: Flask
+Requires-Dist: flask_sock
+Requires-Dist: turbo_flask
+Requires-Dist: rateLimitedQueues
 
-# dynamicWebsite v1.0.2
+# dynamicWebsite v1.0.3
 
 ```pip install dynamicWebsite --upgrade```
 
 ###### <br>A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 <br>To install: 
 ```
```

### Comparing `dynamicwebsite-1.0.2/README.md` & `dynamicwebsite-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# dynamicWebsite v1.0.2
+# dynamicWebsite v1.0.3
 
 ```pip install dynamicWebsite --upgrade```
 
 ###### <br>A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 <br>To install: 
 ```
```

### Comparing `dynamicwebsite-1.0.2/dynamicWebsite.egg-info/PKG-INFO` & `dynamicwebsite-1.0.3/dynamicWebsite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: dynamicWebsite
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>, riyapuri0710 <riyapuri0710@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/dynamicWebsite
 Keywords: website,dynamic website,update website,live website,change website,websocket
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: randomisedString
 Requires-Dist: cryptography
 Requires-Dist: Flask
+Requires-Dist: flask_sock
+Requires-Dist: turbo_flask
+Requires-Dist: rateLimitedQueues
 
-# dynamicWebsite v1.0.2
+# dynamicWebsite v1.0.3
 
 ```pip install dynamicWebsite --upgrade```
 
 ###### <br>A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 <br>To install: 
 ```
```

### Comparing `dynamicwebsite-1.0.2/dynamicWebsite.py` & `dynamicwebsite-1.0.3/dynamicWebsite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __packagename__ = "dynamicWebsite"
 
 
 def updatePackage():
     from time import sleep
     from json import loads
     import http.client
@@ -35,16 +35,17 @@
     from enum import Enum
     from json import dumps, loads
     from threading import Thread
     from time import sleep, time
     from cryptography.fernet import Fernet
     from flask import request, Response
     from flask_sock import Sock
-    from randomisedString import Generator as StringGen
     from turbo_flask import Turbo
+    from randomisedString import Generator as StringGen
+    from rateLimitedQueues import Manager as QueueManager
 
 
 class Errors:
     """
     Contains all Error classes that will be used by the package
     """
     class ViewerDisconnected(Exception):
```

### Comparing `dynamicwebsite-1.0.2/pyproject.toml` & `dynamicwebsite-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynamicWebsite"
-version = "1.0.2"
+version = "1.0.3"
 description = "A simple way to host web server bundled with websocket to send and receive live data, from client to server, and pass live HTML changes from server to client without having to refresh the page."
 
 readme = "README.md"
 authors = [{ name = "Bhindi", email = "bhaskarpanja93@gmail.com" },
            { name = "riyapuri0710", email = "riyapuri0710@gmail.com" }]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["website", "dynamic website", "update website", "live website", "change website", "websocket"]
 requires-python = ">=3.6"
-dependencies = ["randomisedString", "cryptography", "Flask"]
+dependencies = ["randomisedString", "cryptography", "Flask", "flask_sock", "turbo_flask", "rateLimitedQueues"]
 
 [project.urls]
 Homepage = "https://github.com/BhaskarPanja93/dynamicWebsite"
```

