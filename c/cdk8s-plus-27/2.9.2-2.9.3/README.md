# Comparing `tmp/cdk8s-plus-27-2.9.2.tar.gz` & `tmp/cdk8s-plus-27-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-27-2.9.2.tar", last modified: Wed May  8 12:10:09 2024, max compression
+gzip compressed data, was "cdk8s-plus-27-2.9.3.tar", last modified: Fri May 10 12:08:22 2024, max compression
```

## Comparing `cdk8s-plus-27-2.9.2.tar` & `cdk8s-plus-27-2.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:10:09.651530 cdk8s-plus-27-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-08 12:10:09.651530 cdk8s-plus-27-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:10:09.651530 cdk8s-plus-27-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:10:09.643530 cdk8s-plus-27-2.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:10:09.643530 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/
--rw-r--r--   0 runner    (1001) docker     (127)  1174767 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:10:09.643530 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1320954 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/_jsii/cdk8s-plus-27@2.9.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:10:09.647529 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)  2838922 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:09:59.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:10:09.643530 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-08 12:10:09.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 12:10:09.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:10:09.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 12:10:09.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 12:10:09.000000 cdk8s-plus-27-2.9.2/src/cdk8s_plus_27.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:08:22.584236 cdk8s-plus-27-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-10 12:08:22.584236 cdk8s-plus-27-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:08:22.584236 cdk8s-plus-27-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:08:22.572236 cdk8s-plus-27-2.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:08:22.576237 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/
+-rw-r--r--   0 runner    (1001) docker     (127)  1174767 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:08:22.576237 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1320959 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/_jsii/cdk8s-plus-27@2.9.3.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:08:22.580237 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)  2838922 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:08:12.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:08:22.576237 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-10 12:08:22.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-10 12:08:22.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:08:22.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 12:08:22.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 12:08:22.000000 cdk8s-plus-27-2.9.3/src/cdk8s_plus_27.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-27-2.9.2/LICENSE` & `cdk8s-plus-27-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.2/PKG-INFO` & `cdk8s-plus-27-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-27
-Version: 2.9.2
+Version: 2.9.3
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-27-2.9.2/README.md` & `cdk8s-plus-27-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.2/setup.py` & `cdk8s-plus-27-2.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-27",
-    "version": "2.9.2",
+    "version": "2.9.3",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "cdk8s_plus_27",
         "cdk8s_plus_27._jsii",
         "cdk8s_plus_27.k8s"
     ],
     "package_data": {
         "cdk8s_plus_27._jsii": [
-            "cdk8s-plus-27@2.9.2.jsii.tgz"
+            "cdk8s-plus-27@2.9.3.jsii.tgz"
         ],
         "cdk8s_plus_27": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/__init__.py` & `cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.2/src/cdk8s_plus_27/k8s/__init__.py` & `cdk8s-plus-27-2.9.3/src/cdk8s_plus_27/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.2/src/cdk8s_plus_27.egg-info/PKG-INFO` & `cdk8s-plus-27-2.9.3/src/cdk8s_plus_27.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-27
-Version: 2.9.2
+Version: 2.9.3
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

