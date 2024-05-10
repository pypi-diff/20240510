# Comparing `tmp/hal9-2.0.0.tar.gz` & `tmp/hal9-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.0.0.tar", max compression
+gzip compressed data, was "hal9-2.0.1.tar", max compression
```

## Comparing `hal9-2.0.0.tar` & `hal9-2.0.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      117 2024-05-08 22:33:23.124203 hal9-2.0.0/README.md
--rw-r--r--   0        0        0       24 2024-05-08 22:33:23.124203 hal9-2.0.0/hal9/__init__.py
--rw-r--r--   0        0        0      957 2024-05-08 22:33:23.124203 hal9-2.0.0/hal9/core.py
--rw-r--r--   0        0        0      304 2024-05-08 22:33:23.124203 hal9-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 hal9-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-05-10 19:22:26.770618 hal9-2.0.1/README.md
+-rw-r--r--   0        0        0       23 2024-05-10 19:22:26.770618 hal9-2.0.1/hal9/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-10 19:22:26.770618 hal9-2.0.1/hal9/api.py
+-rw-r--r--   0        0        0      941 2024-05-10 19:22:26.770618 hal9-2.0.1/hal9/cli.py
+-rw-r--r--   0        0        0      365 2024-05-10 19:22:26.770618 hal9-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 hal9-2.0.1/PKG-INFO
```

### Comparing `hal9-2.0.0/hal9/core.py` & `hal9-2.0.1/hal9/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 import requests
 import time
 import tempfile
 import sys
 import runpy
 
-def create(template :str) -> str:
-    """Create an app for the given template
+def create(path :str, template :str) -> str:
+    """Create an application
 
     Parameters
     ----------
+    path : str 
+            Path to the application.
     template : str 
-            The template to use to create the project.
+            The template to use.
     """
 
-def deploy(project :str, destination :str) -> str:
-    """Deploy project to given destination
+    print(f'Project created! {name}')
+
+def run(path :str) -> str:
+    """Run an application
+
+    Parameters
+    ----------
+    path : str 
+            Path to the application.
+    """
+
+    print(f'Project created! {name}')
+
+def deploy(path :str, target :str) -> str:
+    """Deploy an application
 
     Parameters
     ----------
-    project : str 
-            The project name used to deploy the app.
-    destination : str 
-            The deployment destination, defaults to Hal9.
+    path : str 
+            Path to the application.
+    target : str 
+            The deployment target, defaults to 'hal9.com'.
     """
 
     response = requests.post('https://api.hal9.com/api/v1/deploy', json = {
         'name': 'name',
         'title': 'title',
         'description': 'description',
         'access': 'access',
```

### Comparing `hal9-2.0.0/PKG-INFO` & `hal9-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Python Component
 
 ## Contributing
```

