# Comparing `tmp/metabotk-0.1.2b0.tar.gz` & `tmp/metabotk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.2b0.tar", max compression
+gzip compressed data, was "metabotk-0.1.3.tar", max compression
```

## Comparing `metabotk-0.1.2b0.tar` & `metabotk-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.2b0/README.md
--rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.2b0/metabotk/__init__.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.2b0/metabotk/cli.py
--rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.2b0/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.2b0/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.2b0/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.2b0/metabotk/imputation.py
--rw-r--r--   0        0        0     6553 2024-05-10 08:22:09.586411 metabotk-0.1.2b0/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.2b0/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.2b0/metabotk/models_handler.py
--rw-r--r--   0        0        0     3282 2024-05-10 08:23:57.189568 metabotk-0.1.2b0/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.2b0/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.2b0/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.2b0/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.2b0/metabotk/utils.py
--rw-r--r--   0        0        0     4527 2024-04-19 13:40:45.180792 metabotk-0.1.2b0/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      716 2024-05-10 08:26:12.721655 metabotk-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 metabotk-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.3/README.md
+-rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.3/metabotk/__init__.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.3/metabotk/cli.py
+-rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.3/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.3/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.3/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.3/metabotk/imputation.py
+-rw-r--r--   0        0        0     6553 2024-05-10 08:22:09.586411 metabotk-0.1.3/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.3/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.3/metabotk/models_handler.py
+-rw-r--r--   0        0        0     3282 2024-05-10 08:23:57.189568 metabotk-0.1.3/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.3/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.3/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.3/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.3/metabotk/utils.py
+-rw-r--r--   0        0        0     4527 2024-04-19 13:40:45.180792 metabotk-0.1.3/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      715 2024-05-10 08:29:36.255967 metabotk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 metabotk-0.1.3/PKG-INFO
```

### Comparing `metabotk-0.1.2b0/metabotk/cli.py` & `metabotk-0.1.3/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/dataset_manager.py` & `metabotk-0.1.3/metabotk/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/dimensionality_reduction.py` & `metabotk-0.1.3/metabotk/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/feature_selection.py` & `metabotk-0.1.3/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/imputation.py` & `metabotk-0.1.3/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/interface.py` & `metabotk-0.1.3/metabotk/interface.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/missing_handler.py` & `metabotk-0.1.3/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/models_handler.py` & `metabotk-0.1.3/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/normalization.py` & `metabotk-0.1.3/metabotk/normalization.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/outliers_handler.py` & `metabotk-0.1.3/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/providers_handler.py` & `metabotk-0.1.3/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/statistics_handler.py` & `metabotk-0.1.3/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/utils.py` & `metabotk-0.1.3/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/metabotk/visualization_handler.py` & `metabotk-0.1.3/metabotk/visualization_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.2b0/pyproject.toml` & `metabotk-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.2b"
+version = "0.1.3"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
```

### Comparing `metabotk-0.1.2b0/PKG-INFO` & `metabotk-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabotk
-Version: 0.1.2b0
+Version: 0.1.3
 Summary: Python toolkit for working with metabolomics data
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

