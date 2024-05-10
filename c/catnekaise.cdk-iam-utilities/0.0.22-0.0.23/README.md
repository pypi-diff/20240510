# Comparing `tmp/catnekaise.cdk-iam-utilities-0.0.22.tar.gz` & `tmp/catnekaise.cdk-iam-utilities-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnekaise.cdk-iam-utilities-0.0.22.tar", last modified: Mon Apr 22 13:51:11 2024, max compression
+gzip compressed data, was "catnekaise.cdk-iam-utilities-0.0.23.tar", last modified: Fri May 10 06:47:57 2024, max compression
```

## Comparing `catnekaise.cdk-iam-utilities-0.0.22.tar` & `catnekaise.cdk-iam-utilities-0.0.23.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:51:11.000746 catnekaise.cdk-iam-utilities-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-22 13:51:10.996746 catnekaise.cdk-iam-utilities-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:51:11.000746 catnekaise.cdk-iam-utilities-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:51:10.996746 catnekaise.cdk-iam-utilities-0.0.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:51:10.996746 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-22 13:51:10.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-22 13:51:10.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:51:10.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 13:51:10.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 13:51:10.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:51:10.996746 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise_cdk_iam_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)   175274 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise_cdk_iam_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:51:10.996746 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise_cdk_iam_utilities/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise_cdk_iam_utilities/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95916 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.22.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:51:00.000000 catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise_cdk_iam_utilities/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:47:57.267717 catnekaise.cdk-iam-utilities-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-10 06:47:57.267717 catnekaise.cdk-iam-utilities-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:47:57.267717 catnekaise.cdk-iam-utilities-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:47:57.263717 catnekaise.cdk-iam-utilities-0.0.23/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:47:57.263717 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-10 06:47:57.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-10 06:47:57.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:47:57.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 06:47:57.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 06:47:57.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:47:57.263717 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise_cdk_iam_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)   175274 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise_cdk_iam_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:47:57.267717 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise_cdk_iam_utilities/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise_cdk_iam_utilities/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95916 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.23.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:47:46.000000 catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise_cdk_iam_utilities/py.typed
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.22/LICENSE` & `catnekaise.cdk-iam-utilities-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `catnekaise.cdk-iam-utilities-0.0.22/PKG-INFO` & `catnekaise.cdk-iam-utilities-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.cdk-iam-utilities
-Version: 0.0.22
+Version: 0.0.23
 Summary: Experimental utilities intended for AWS CDK IAM
 Home-page: https://github.com/catnekaise/cdk-iam-utilities.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/cdk-iam-utilities.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.22/setup.py` & `catnekaise.cdk-iam-utilities-0.0.23/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "catnekaise.cdk-iam-utilities",
-    "version": "0.0.22",
+    "version": "0.0.23",
     "description": "Experimental utilities intended for AWS CDK IAM",
     "license": "Apache-2.0",
     "url": "https://github.com/catnekaise/cdk-iam-utilities.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Jonsén<djonser1@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "catnekaise_cdk_iam_utilities",
         "catnekaise_cdk_iam_utilities._jsii"
     ],
     "package_data": {
         "catnekaise_cdk_iam_utilities._jsii": [
-            "cdk-iam-utilities@0.0.22.jsii.tgz"
+            "cdk-iam-utilities@0.0.23.jsii.tgz"
         ],
         "catnekaise_cdk_iam_utilities": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.82.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO` & `catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.cdk-iam-utilities
-Version: 0.0.22
+Version: 0.0.23
 Summary: Experimental utilities intended for AWS CDK IAM
 Home-page: https://github.com/catnekaise/cdk-iam-utilities.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/cdk-iam-utilities.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt` & `catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/catnekaise.cdk_iam_utilities.egg-info/SOURCES.txt
 src/catnekaise.cdk_iam_utilities.egg-info/dependency_links.txt
 src/catnekaise.cdk_iam_utilities.egg-info/requires.txt
 src/catnekaise.cdk_iam_utilities.egg-info/top_level.txt
 src/catnekaise_cdk_iam_utilities/__init__.py
 src/catnekaise_cdk_iam_utilities/py.typed
 src/catnekaise_cdk_iam_utilities/_jsii/__init__.py
-src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.22.jsii.tgz
+src/catnekaise_cdk_iam_utilities/_jsii/cdk-iam-utilities@0.0.23.jsii.tgz
```

### Comparing `catnekaise.cdk-iam-utilities-0.0.22/src/catnekaise_cdk_iam_utilities/__init__.py` & `catnekaise.cdk-iam-utilities-0.0.23/src/catnekaise_cdk_iam_utilities/__init__.py`

 * *Files identical despite different names*

