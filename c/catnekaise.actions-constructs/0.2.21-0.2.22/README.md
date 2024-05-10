# Comparing `tmp/catnekaise.actions-constructs-0.2.21.tar.gz` & `tmp/catnekaise.actions-constructs-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnekaise.actions-constructs-0.2.21.tar", last modified: Mon Apr 22 13:50:43 2024, max compression
+gzip compressed data, was "catnekaise.actions-constructs-0.2.22.tar", last modified: Fri May 10 11:31:45 2024, max compression
```

## Comparing `catnekaise.actions-constructs-0.2.21.tar` & `catnekaise.actions-constructs-0.2.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:50:43.660018 catnekaise.actions-constructs-0.2.21/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-04-22 13:50:43.660018 catnekaise.actions-constructs-0.2.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29028 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:50:43.660018 catnekaise.actions-constructs-0.2.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:50:43.660018 catnekaise.actions-constructs-0.2.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:50:43.660018 catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-04-22 13:50:43.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 13:50:43.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:50:43.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 13:50:43.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 13:50:43.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:50:43.660018 catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/
--rw-r--r--   0 runner    (1001) docker     (127)   220715 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:50:43.660018 catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   111893 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.21.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:50:32.000000 catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29028 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)   220715 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111894 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.22.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/py.typed
```

### Comparing `catnekaise.actions-constructs-0.2.21/LICENSE` & `catnekaise.actions-constructs-0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `catnekaise.actions-constructs-0.2.21/PKG-INFO` & `catnekaise.actions-constructs-0.2.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.actions-constructs
-Version: 0.2.21
+Version: 0.2.22
 Summary: CDK Constructs for integrating GitHub Actions and AWS.
 Home-page: https://github.com/catnekaise/actions-constructs.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/actions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.actions-constructs-0.2.21/README.md` & `catnekaise.actions-constructs-0.2.22/README.md`

 * *Files identical despite different names*

### Comparing `catnekaise.actions-constructs-0.2.21/setup.py` & `catnekaise.actions-constructs-0.2.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "catnekaise.actions-constructs",
-    "version": "0.2.21",
+    "version": "0.2.22",
     "description": "CDK Constructs for integrating GitHub Actions and AWS.",
     "license": "Apache-2.0",
     "url": "https://github.com/catnekaise/actions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Jonsén<djonser1@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "catnekaise_actions_constructs",
         "catnekaise_actions_constructs._jsii"
     ],
     "package_data": {
         "catnekaise_actions_constructs._jsii": [
-            "actions-constructs@0.2.21.jsii.tgz"
+            "actions-constructs@0.2.22.jsii.tgz"
         ],
         "catnekaise_actions_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.82.0, <3.0.0",
         "catnekaise.cdk-iam-utilities>=0.0.13, <0.0.14",
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

### Comparing `catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/PKG-INFO` & `catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.actions-constructs
-Version: 0.2.21
+Version: 0.2.22
 Summary: CDK Constructs for integrating GitHub Actions and AWS.
 Home-page: https://github.com/catnekaise/actions-constructs.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/actions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.actions-constructs-0.2.21/src/catnekaise.actions_constructs.egg-info/SOURCES.txt` & `catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/catnekaise.actions_constructs.egg-info/SOURCES.txt
 src/catnekaise.actions_constructs.egg-info/dependency_links.txt
 src/catnekaise.actions_constructs.egg-info/requires.txt
 src/catnekaise.actions_constructs.egg-info/top_level.txt
 src/catnekaise_actions_constructs/__init__.py
 src/catnekaise_actions_constructs/py.typed
 src/catnekaise_actions_constructs/_jsii/__init__.py
-src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.21.jsii.tgz
+src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.22.jsii.tgz
```

### Comparing `catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/__init__.py` & `catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `catnekaise.actions-constructs-0.2.21/src/catnekaise_actions_constructs/_jsii/__init__.py` & `catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import catnekaise_cdk_iam_utilities._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@catnekaise/actions-constructs",
-    "0.2.21",
+    "0.2.22",
     __name__[0:-6],
-    "actions-constructs@0.2.21.jsii.tgz",
+    "actions-constructs@0.2.22.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

