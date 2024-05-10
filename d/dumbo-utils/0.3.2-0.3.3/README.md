# Comparing `tmp/dumbo_utils-0.3.2.tar.gz` & `tmp/dumbo_utils-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_utils-0.3.2.tar", max compression
+gzip compressed data, was "dumbo_utils-0.3.3.tar", max compression
```

## Comparing `dumbo_utils-0.3.2.tar` & `dumbo_utils-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-09-09 14:23:38.733778 dumbo_utils-0.3.2/LICENSE
--rw-r--r--   0        0        0      176 2023-09-09 14:23:38.733778 dumbo_utils-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-09-09 14:23:38.733778 dumbo_utils-0.3.2/dumbo_utils/__init__.py
--rw-r--r--   0        0        0      396 2023-09-09 14:23:38.733778 dumbo_utils-0.3.2/dumbo_utils/console.py
--rw-r--r--   0        0        0      142 2024-03-13 08:52:58.597624 dumbo_utils-0.3.2/dumbo_utils/files.py
--rw-r--r--   0        0        0      227 2024-03-13 08:49:54.365425 dumbo_utils-0.3.2/dumbo_utils/objects.py
--rw-r--r--   0        0        0     6678 2023-09-09 14:23:38.733778 dumbo_utils-0.3.2/dumbo_utils/primitives.py
--rw-r--r--   0        0        0      286 2023-09-09 14:23:38.733778 dumbo_utils-0.3.2/dumbo_utils/url.py
--rw-r--r--   0        0        0      889 2023-09-09 14:23:38.733778 dumbo_utils-0.3.2/dumbo_utils/validation.py
--rw-r--r--   0        0        0      568 2024-03-13 08:50:29.119836 dumbo_utils-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 dumbo_utils-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-17 15:00:05.226957 dumbo_utils-0.3.3/LICENSE
+-rw-r--r--   0        0        0      176 2023-02-17 13:32:21.052107 dumbo_utils-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-01-17 14:30:53.103251 dumbo_utils-0.3.3/dumbo_utils/__init__.py
+-rw-r--r--   0        0        0      396 2023-01-25 11:31:11.894094 dumbo_utils-0.3.3/dumbo_utils/console.py
+-rw-r--r--   0        0        0      142 2024-05-10 16:05:07.398695 dumbo_utils-0.3.3/dumbo_utils/files.py
+-rw-r--r--   0        0        0      227 2023-12-24 09:34:51.410869 dumbo_utils-0.3.3/dumbo_utils/objects.py
+-rw-r--r--   0        0        0     6678 2023-01-25 11:34:14.062908 dumbo_utils-0.3.3/dumbo_utils/primitives.py
+-rw-r--r--   0        0        0      286 2023-05-26 17:30:30.582066 dumbo_utils-0.3.3/dumbo_utils/url.py
+-rw-r--r--   0        0        0      889 2023-01-18 12:09:49.139316 dumbo_utils-0.3.3/dumbo_utils/validation.py
+-rw-r--r--   0        0        0      569 2024-05-10 16:05:44.607269 dumbo_utils-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 dumbo_utils-0.3.3/PKG-INFO
```

### Comparing `dumbo_utils-0.3.2/LICENSE` & `dumbo_utils-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_utils-0.3.2/dumbo_utils/primitives.py` & `dumbo_utils-0.3.3/dumbo_utils/primitives.py`

 * *Files identical despite different names*

### Comparing `dumbo_utils-0.3.2/dumbo_utils/validation.py` & `dumbo_utils-0.3.3/dumbo_utils/validation.py`

 * *Files identical despite different names*

### Comparing `dumbo_utils-0.3.2/pyproject.toml` & `dumbo_utils-0.3.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dumbo-utils"
-version = "0.3.2"
+version = "0.3.3"
 description = "Different utilities to be reused in other projects"
 authors = ["Mario Alviano <mario.alviano@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dumbo_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-rich = "^13.3.1"
-typer = "^0.9.0"
-typeguard = "^4.0.0"
+rich = "^13.7.1"
+typer = "^0.12.3"
+typeguard = "^4.2.1"
 valid8 = "^5.1.2"
-distlib = "^0.3.6"
+distlib = "^0.3.8"
 dataclass-type-validator = "^0.1.2"
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^7.1.0"
-pytest = "^7.3.1"
+coverage = "^7.5.1"
+pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dumbo_utils-0.3.2/PKG-INFO` & `dumbo_utils-0.3.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dumbo-utils
-Version: 0.3.2
+Version: 0.3.3
 Summary: Different utilities to be reused in other projects
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dataclass-type-validator (>=0.1.2,<0.2.0)
-Requires-Dist: distlib (>=0.3.6,<0.4.0)
-Requires-Dist: rich (>=13.3.1,<14.0.0)
-Requires-Dist: typeguard (>=4.0.0,<5.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: distlib (>=0.3.8,<0.4.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: typeguard (>=4.2.1,<5.0.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Requires-Dist: valid8 (>=5.1.2,<6.0.0)
 Description-Content-Type: text/markdown
 
 # dumbo-utils
 
 Different utilities to be reused in other projects
```

