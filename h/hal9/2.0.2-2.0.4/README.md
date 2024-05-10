# Comparing `tmp/hal9-2.0.2.tar.gz` & `tmp/hal9-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.0.2.tar", max compression
+gzip compressed data, was "hal9-2.0.4.tar", max compression
```

## Comparing `hal9-2.0.2.tar` & `hal9-2.0.4.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     2896 2024-05-10 19:26:15.741412 hal9-2.0.2/README.md
--rw-r--r--   0        0        0       23 2024-05-10 19:26:15.677413 hal9-2.0.2/hal9/__init__.py
--rw-r--r--   0        0        0     1163 2024-05-10 19:26:15.677413 hal9-2.0.2/hal9/api.py
--rw-r--r--   0        0        0      941 2024-05-10 19:26:15.677413 hal9-2.0.2/hal9/cli.py
--rw-r--r--   0        0        0      365 2024-05-10 19:26:15.677413 hal9-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 hal9-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2896 2024-05-10 21:00:10.665875 hal9-2.0.4/README.md
+-rw-r--r--   0        0        0       86 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/__init__.py
+-rw-r--r--   0        0        0     1033 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/create.py
+-rw-r--r--   0        0        0      719 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/run.py
+-rw-r--r--   0        0        0       70 2024-05-10 21:00:10.597875 hal9-2.0.4/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      403 2024-05-10 21:00:10.597875 hal9-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 hal9-2.0.4/PKG-INFO
```

### Comparing `hal9-2.0.2/README.md` & `hal9-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hal9-2.0.2/hal9/cli.py` & `hal9-2.0.4/hal9/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import click
 from collections import OrderedDict
-from hal9.api import *
+from hal9.create import create as api_create
+from hal9.run import run as api_run
+from hal9.deploy import deploy as api_deploy
 
 @click.group()
 def cli():
     """
     Create and Deploy Generative Applications
 
     Use this tool to create apps from templates that use Generative AI,
@@ -16,25 +18,25 @@
 @click.argument('path')
 def create(path):
     """
     Create Project
 
     PATH: The path for the new project. Required argument.
     """
-    print(f'Creating: {path}')
+    api_create(path, "openai")
 
 @click.command()
 @click.argument('path')
 def run(path):
     """
     Run Project
 
     PATH: The path to the project. Required argument.
     """
-    print(f'Running {path}')
+    api_run(path)
 
 @click.command()
 @click.argument('path')
 def deploy(path):
     """
     Deploy Project
```

### Comparing `hal9-2.0.2/PKG-INFO` & `hal9-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.0.2
+Version: 2.0.4
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

