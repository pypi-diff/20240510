# Comparing `tmp/metabotk-0.1.1.tar.gz` & `tmp/metabotk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.1.tar", max compression
+gzip compressed data, was "metabotk-0.1.2.tar", max compression
```

## Comparing `metabotk-0.1.1.tar` & `metabotk-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.1/README.md
--rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.1/metabotk/__init__.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.1/metabotk/cli.py
--rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.1/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.1/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.1/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.1/metabotk/imputation.py
--rw-r--r--   0        0        0     6517 2024-05-10 08:09:58.633114 metabotk-0.1.1/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.1/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.1/metabotk/models_handler.py
--rw-r--r--   0        0        0     3281 2024-05-10 07:48:23.295768 metabotk-0.1.1/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.1/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.1/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.1/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.1/metabotk/utils.py
--rw-r--r--   0        0        0     4527 2024-04-19 13:40:45.180792 metabotk-0.1.1/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      715 2024-05-10 08:12:20.335599 metabotk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 metabotk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.2/README.md
+-rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.2/metabotk/__init__.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.2/metabotk/cli.py
+-rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.2/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.2/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.2/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.2/metabotk/imputation.py
+-rw-r--r--   0        0        0     6553 2024-05-10 08:19:01.821150 metabotk-0.1.2/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.2/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.2/metabotk/models_handler.py
+-rw-r--r--   0        0        0     3281 2024-05-10 07:48:23.295768 metabotk-0.1.2/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.2/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.2/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.2/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.2/metabotk/utils.py
+-rw-r--r--   0        0        0     4527 2024-04-19 13:40:45.180792 metabotk-0.1.2/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      715 2024-05-10 08:19:22.701717 metabotk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 metabotk-0.1.2/PKG-INFO
```

### Comparing `metabotk-0.1.1/metabotk/cli.py` & `metabotk-0.1.2/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/dataset_manager.py` & `metabotk-0.1.2/metabotk/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/dimensionality_reduction.py` & `metabotk-0.1.2/metabotk/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/feature_selection.py` & `metabotk-0.1.2/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/imputation.py` & `metabotk-0.1.2/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/interface.py` & `metabotk-0.1.2/metabotk/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from metabotk.statistics_handler import StatisticsHandler
 from metabotk.dataset_manager import DatasetManager
 from metabotk.models_handler import ModelsHandler
 from metabotk.visualization_handler import Visualization
 from metabotk.dimensionality_reduction import DimensionalityReduction
 from metabotk.imputation import ImputationHandler
 from metabotk.feature_selection import FeatureSelection
-import pandas as pd
+from metabotk.normalization import NormalizationHandler
 from typing import List, Dict
 
 
 class MetaboTK(DatasetManager):
     """
     Class for working with metabolomics data
     """
```

### Comparing `metabotk-0.1.1/metabotk/missing_handler.py` & `metabotk-0.1.2/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/models_handler.py` & `metabotk-0.1.2/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/normalization.py` & `metabotk-0.1.2/metabotk/normalization.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/outliers_handler.py` & `metabotk-0.1.2/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/providers_handler.py` & `metabotk-0.1.2/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/statistics_handler.py` & `metabotk-0.1.2/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/utils.py` & `metabotk-0.1.2/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/metabotk/visualization_handler.py` & `metabotk-0.1.2/metabotk/visualization_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.1/pyproject.toml` & `metabotk-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
```

### Comparing `metabotk-0.1.1/PKG-INFO` & `metabotk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabotk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python toolkit for working with metabolomics data
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

