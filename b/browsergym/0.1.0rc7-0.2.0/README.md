# Comparing `tmp/browsergym-0.1.0rc7.tar.gz` & `tmp/browsergym-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browsergym-0.1.0rc7.tar", last modified: Mon Mar 25 15:48:51 2024, max compression
+gzip compressed data, was "browsergym-0.2.0.tar", last modified: Thu May  9 21:19:23 2024, max compression
```

## Comparing `browsergym-0.1.0rc7.tar` & `browsergym-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:48:51.212250 browsergym-0.1.0rc7/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-25 15:48:37.000000 browsergym-0.1.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-03-25 15:48:51.212250 browsergym-0.1.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-03-25 15:48:37.000000 browsergym-0.1.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:48:51.212250 browsergym-0.1.0rc7/browsergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-03-25 15:48:51.000000 browsergym-0.1.0rc7/browsergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-25 15:48:51.000000 browsergym-0.1.0rc7/browsergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:48:51.000000 browsergym-0.1.0rc7/browsergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-25 15:48:51.000000 browsergym-0.1.0rc7/browsergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:48:51.000000 browsergym-0.1.0rc7/browsergym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-25 15:48:37.000000 browsergym-0.1.0rc7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 15:48:51.212250 browsergym-0.1.0rc7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:23.267976 browsergym-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-09 21:19:10.000000 browsergym-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-09 21:19:23.267976 browsergym-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-09 21:19:10.000000 browsergym-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:19:23.267976 browsergym-0.2.0/browsergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-09 21:19:23.000000 browsergym-0.2.0/browsergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 21:19:23.000000 browsergym-0.2.0/browsergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:19:23.000000 browsergym-0.2.0/browsergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 21:19:23.000000 browsergym-0.2.0/browsergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:19:23.000000 browsergym-0.2.0/browsergym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-09 21:19:10.000000 browsergym-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:19:23.267976 browsergym-0.2.0/setup.cfg
```

### Comparing `browsergym-0.1.0rc7/LICENSE` & `browsergym-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsergym-0.1.0rc7/PKG-INFO` & `browsergym-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: browsergym
-Version: 0.1.0rc7
+Version: 0.2.0
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: browsergym-core==0.1.0rc7
-Requires-Dist: browsergym-miniwob==0.1.0rc7
-Requires-Dist: browsergym-webarena==0.1.0rc7
-Requires-Dist: browsergym-workarena==0.1.0rc7
+Requires-Dist: browsergym-core==0.2.0
+Requires-Dist: browsergym-miniwob==0.2.0
+Requires-Dist: browsergym-webarena==0.2.0
+Requires-Dist: browsergym-workarena==0.2.0
 
 # BrowserGym: a Gym Environment for Web Task Automation
 
 [[Setup]](#setup) ♦ [[Usage]](#usage) ♦ [[Demo]](#demo)
 
 This package provides `browsergym`, a gym environment for web task automation in the Chromium browser.
```

### Comparing `browsergym-0.1.0rc7/README.md` & `browsergym-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `browsergym-0.1.0rc7/browsergym.egg-info/PKG-INFO` & `browsergym-0.2.0/browsergym.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: browsergym
-Version: 0.1.0rc7
+Version: 0.2.0
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: browsergym-core==0.1.0rc7
-Requires-Dist: browsergym-miniwob==0.1.0rc7
-Requires-Dist: browsergym-webarena==0.1.0rc7
-Requires-Dist: browsergym-workarena==0.1.0rc7
+Requires-Dist: browsergym-core==0.2.0
+Requires-Dist: browsergym-miniwob==0.2.0
+Requires-Dist: browsergym-webarena==0.2.0
+Requires-Dist: browsergym-workarena==0.2.0
 
 # BrowserGym: a Gym Environment for Web Task Automation
 
 [[Setup]](#setup) ♦ [[Usage]](#usage) ♦ [[Demo]](#demo)
 
 This package provides `browsergym`, a gym environment for web task automation in the Chromium browser.
```

### Comparing `browsergym-0.1.0rc7/pyproject.toml` & `browsergym-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
 ]
-version="0.1.0rc7"
+version="0.2.0"
 dependencies = [
-    "browsergym-core==0.1.0rc7",
-    "browsergym-miniwob==0.1.0rc7",
-    "browsergym-webarena==0.1.0rc7",
-    "browsergym-workarena==0.1.0rc7",
+    "browsergym-core==0.2.0",
+    "browsergym-miniwob==0.2.0",
+    "browsergym-webarena==0.2.0",
+    "browsergym-workarena==0.2.0",
 ]
 
 [tool.setuptools]
 packages = []  # meta distribution, packages are included as dependencies
 
 [tool.black]
 line-length = 100
```

