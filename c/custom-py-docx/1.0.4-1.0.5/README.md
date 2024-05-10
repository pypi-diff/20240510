# Comparing `tmp/custom_py_docx-1.0.4.tar.gz` & `tmp/custom_py_docx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_py_docx-1.0.4.tar", max compression
+gzip compressed data, was "custom_py_docx-1.0.5.tar", max compression
```

## Comparing `custom_py_docx-1.0.4.tar` & `custom_py_docx-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1477 2023-07-31 16:16:08.070960 custom_py_docx-1.0.4/LICENSE
--rw-r--r--   0        0        0     7318 2023-07-31 16:23:50.420958 custom_py_docx-1.0.4/README.md
--rw-r--r--   0        0        0       93 2023-07-31 16:33:29.670956 custom_py_docx-1.0.4/custom_py_docx/__init__.py
--rw-r--r--   0        0        0     6055 2023-07-31 16:16:08.070960 custom_py_docx-1.0.4/custom_py_docx/document.py
--rw-r--r--   0        0        0      878 2023-07-31 16:33:11.270956 custom_py_docx-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     8258 1970-01-01 00:00:00.000000 custom_py_docx-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1477 2024-05-10 19:03:07.631825 custom_py_docx-1.0.5/LICENSE
+-rw-r--r--   0        0        0     7318 2024-05-10 19:03:07.631825 custom_py_docx-1.0.5/README.md
+-rw-r--r--   0        0        0       93 2024-05-10 19:03:07.631825 custom_py_docx-1.0.5/custom_py_docx/__init__.py
+-rw-r--r--   0        0        0     6055 2024-05-10 19:03:07.631825 custom_py_docx-1.0.5/custom_py_docx/document.py
+-rw-r--r--   0        0        0      878 2024-05-10 19:03:07.635825 custom_py_docx-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8309 1970-01-01 00:00:00.000000 custom_py_docx-1.0.5/PKG-INFO
```

### Comparing `custom_py_docx-1.0.4/LICENSE` & `custom_py_docx-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.4/README.md` & `custom_py_docx-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.4/custom_py_docx/document.py` & `custom_py_docx-1.0.5/custom_py_docx/document.py`

 * *Files identical despite different names*

### Comparing `custom_py_docx-1.0.4/pyproject.toml` & `custom_py_docx-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "custom_py_docx"
-version = "1.0.4"
+version = "1.0.5"
 license="BSD"
 description = "Library to create DOCX facility using python-docx"
 authors = ["Renato Pinheiro <renato.dev.pinheiro@gmail.com>"]
 readme = "README.md"
 
 packages = [{include = "custom_py_docx"}]
```

### Comparing `custom_py_docx-1.0.4/PKG-INFO` & `custom_py_docx-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: custom-py-docx
-Version: 1.0.4
+Name: custom_py_docx
+Version: 1.0.5
 Summary: Library to create DOCX facility using python-docx
 License: BSD
 Author: Renato Pinheiro
 Author-email: renato.dev.pinheiro@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: babel (==2.12.1)
 Requires-Dist: docxcompose (==1.4.0)
 Requires-Dist: lxml (==4.9.2)
 Requires-Dist: numpy (==1.24.3)
 Requires-Dist: packaging (==23.1)
 Requires-Dist: pandas (==2.0.1)
 Requires-Dist: plotly (==5.14.1)
```

