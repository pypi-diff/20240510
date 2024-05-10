# Comparing `tmp/pms_model_manager-1.1.0.tar.gz` & `tmp/pms_model_manager-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pms_model_manager-1.1.0.tar", max compression
+gzip compressed data, was "pms_model_manager-1.2.0.tar", max compression
```

## Comparing `pms_model_manager-1.1.0.tar` & `pms_model_manager-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      700 2024-03-21 02:31:17.176614 pms_model_manager-1.1.0/README.md
--rw-r--r--   0        0        0      206 2024-03-26 08:13:43.372165 pms_model_manager-1.1.0/pms_model_manager/__init__.py
--rw-r--r--   0        0        0     3469 2024-03-26 08:08:03.868169 pms_model_manager-1.1.0/pms_model_manager/_cli.py
--rw-r--r--   0        0        0     1213 2024-03-21 06:16:46.105779 pms_model_manager-1.1.0/pms_model_manager/_const.py
--rw-r--r--   0        0        0     4054 2024-03-21 01:37:57.107591 pms_model_manager-1.1.0/pms_model_manager/_mlflow_model.py
--rw-r--r--   0        0        0     3385 2024-03-21 01:37:57.107591 pms_model_manager-1.1.0/pms_model_manager/_mlflow_model_collection.py
--rw-r--r--   0        0        0     5490 2024-03-21 01:37:57.107591 pms_model_manager-1.1.0/pms_model_manager/_model_manager.py
--rw-r--r--   0        0        0      310 2024-03-21 01:37:57.107591 pms_model_manager-1.1.0/pms_model_manager/_utils.py
--rw-r--r--   0        0        0       41 2024-03-21 08:41:51.707981 pms_model_manager-1.1.0/pms_model_manager/onnx_utility/__init__.py
--rw-r--r--   0        0        0      256 2024-03-21 06:16:46.105779 pms_model_manager-1.1.0/pms_model_manager/onnx_utility/_const.py
--rw-r--r--   0        0        0      463 2024-03-21 08:41:51.707981 pms_model_manager-1.1.0/pms_model_manager/onnx_utility/_extractor.py
--rw-r--r--   0        0        0      895 2024-03-21 08:43:26.389188 pms_model_manager-1.1.0/pms_model_manager/onnx_utility/_onnx_graph_info.py
--rw-r--r--   0        0        0     1278 2024-03-21 06:16:46.105779 pms_model_manager-1.1.0/pms_model_manager/onnx_utility/_onnx_model_info.py
--rw-r--r--   0        0        0      531 2024-03-26 08:13:43.372165 pms_model_manager-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 pms_model_manager-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      700 2024-03-21 02:31:17.176614 pms_model_manager-1.2.0/README.md
+-rw-r--r--   0        0        0      206 2024-05-09 07:53:25.036559 pms_model_manager-1.2.0/pms_model_manager/__init__.py
+-rw-r--r--   0        0        0     3637 2024-05-09 07:50:26.688506 pms_model_manager-1.2.0/pms_model_manager/_cli.py
+-rw-r--r--   0        0        0     1213 2024-03-21 06:16:46.105779 pms_model_manager-1.2.0/pms_model_manager/_const.py
+-rw-r--r--   0        0        0     4054 2024-03-21 01:37:57.107591 pms_model_manager-1.2.0/pms_model_manager/_mlflow_model.py
+-rw-r--r--   0        0        0     3385 2024-03-21 01:37:57.107591 pms_model_manager-1.2.0/pms_model_manager/_mlflow_model_collection.py
+-rw-r--r--   0        0        0     5490 2024-03-21 01:37:57.107591 pms_model_manager-1.2.0/pms_model_manager/_model_manager.py
+-rw-r--r--   0        0        0      310 2024-03-21 01:37:57.107591 pms_model_manager-1.2.0/pms_model_manager/_utils.py
+-rw-r--r--   0        0        0       41 2024-03-21 08:41:51.707981 pms_model_manager-1.2.0/pms_model_manager/onnx_utility/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-21 06:16:46.105779 pms_model_manager-1.2.0/pms_model_manager/onnx_utility/_const.py
+-rw-r--r--   0        0        0      463 2024-03-21 08:41:51.707981 pms_model_manager-1.2.0/pms_model_manager/onnx_utility/_extractor.py
+-rw-r--r--   0        0        0      895 2024-03-21 08:43:26.389188 pms_model_manager-1.2.0/pms_model_manager/onnx_utility/_onnx_graph_info.py
+-rw-r--r--   0        0        0     1278 2024-03-21 06:16:46.105779 pms_model_manager-1.2.0/pms_model_manager/onnx_utility/_onnx_model_info.py
+-rw-r--r--   0        0        0      531 2024-05-09 07:53:25.036559 pms_model_manager-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 pms_model_manager-1.2.0/PKG-INFO
```

### Comparing `pms_model_manager-1.1.0/README.md` & `pms_model_manager-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pms_model_manager-1.1.0/pms_model_manager/_cli.py` & `pms_model_manager-1.2.0/pms_model_manager/_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import pathlib
-from typing import List, Literal
+from typing import Annotated, List, Literal
 import typer
 import sys
 from enum import Enum
 
 MODEL_NAME = "model"
 ONNX_ALIASES = ["onnx-latest"]
 PACKAGE_DIR = os.path.dirname(os.path.dirname(__file__))
@@ -55,14 +55,15 @@
 
 
 @app.command()
 def up(
     model_name: str,
     model_directory: str,
     ext: ExtensionType = ExtensionType.none,
+    force_yes: Annotated[bool, typer.Option("--force_yes")] = False,
 ):
     # check model path is valid.
     model_dir = pathlib.Path(model_directory)
     assert model_dir.exists(), f"ERROR, the file is not exist."
     assert model_dir.is_dir(), f"ERROR, the path({model_dir}) is NOT directory."
 
     # confirm upload
@@ -86,18 +87,21 @@
     elif ext == ExtensionType.plan:
         raise NotImplementedError()
         typer.echo(f"Model[{model_name}] tags")
         for tag in tags.items():
             typer.echo(f" - tag[{tag[0]}]: {tag[1]}")
     else:
         typer.echo("The extension is not provided. skip extracting tags from the file.")
-    is_upload = typer.confirm("Are you sure you want to upload it?")
-    if is_upload is not True:
-        typer.echo("Upload canceled.")
-        return
+    if force_yes is True:
+        typer.echo("Skip confirm.")
+    else:
+        is_upload = typer.confirm("Are you sure you want to upload it?")
+        if is_upload is not True:
+            typer.echo("Upload canceled.")
+            return
 
     # upload onnx
     typer.echo("Upload start")
     manager = pmm.ModelManager(model_directory)
     res = manager.upload(
         model_name=model_name,
         model_dir=model_directory,
```

### Comparing `pms_model_manager-1.1.0/pms_model_manager/_const.py` & `pms_model_manager-1.2.0/pms_model_manager/_const.py`

 * *Files identical despite different names*

### Comparing `pms_model_manager-1.1.0/pms_model_manager/_mlflow_model.py` & `pms_model_manager-1.2.0/pms_model_manager/_mlflow_model.py`

 * *Files identical despite different names*

### Comparing `pms_model_manager-1.1.0/pms_model_manager/_mlflow_model_collection.py` & `pms_model_manager-1.2.0/pms_model_manager/_mlflow_model_collection.py`

 * *Files identical despite different names*

### Comparing `pms_model_manager-1.1.0/pms_model_manager/_model_manager.py` & `pms_model_manager-1.2.0/pms_model_manager/_model_manager.py`

 * *Files identical despite different names*

### Comparing `pms_model_manager-1.1.0/pms_model_manager/onnx_utility/_onnx_graph_info.py` & `pms_model_manager-1.2.0/pms_model_manager/onnx_utility/_onnx_graph_info.py`

 * *Files identical despite different names*

### Comparing `pms_model_manager-1.1.0/pms_model_manager/onnx_utility/_onnx_model_info.py` & `pms_model_manager-1.2.0/pms_model_manager/onnx_utility/_onnx_model_info.py`

 * *Files identical despite different names*

### Comparing `pms_model_manager-1.1.0/pyproject.toml` & `pms_model_manager-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pms-model-manager"
-version = "1.1.0"
+version = "1.2.0"
 description = "lib for pms"
 authors = ["HyeongSeok Kim <tiryul@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 mlflow = "2.11.1"
```

### Comparing `pms_model_manager-1.1.0/PKG-INFO` & `pms_model_manager-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pms-model-manager
-Version: 1.1.0
+Version: 1.2.0
 Summary: lib for pms
 Author: HyeongSeok Kim
 Author-email: tiryul@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

