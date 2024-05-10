# Comparing `tmp/metabotk-0.1.3.tar.gz` & `tmp/metabotk-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.3.tar", max compression
+gzip compressed data, was "metabotk-0.1.31.tar", max compression
```

## Comparing `metabotk-0.1.3.tar` & `metabotk-0.1.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.3/README.md
--rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.3/metabotk/__init__.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.3/metabotk/cli.py
--rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.3/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.3/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.3/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.3/metabotk/imputation.py
--rw-r--r--   0        0        0     6553 2024-05-10 08:22:09.586411 metabotk-0.1.3/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.3/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.3/metabotk/models_handler.py
--rw-r--r--   0        0        0     3282 2024-05-10 08:23:57.189568 metabotk-0.1.3/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.3/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.3/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.3/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.3/metabotk/utils.py
--rw-r--r--   0        0        0     4527 2024-04-19 13:40:45.180792 metabotk-0.1.3/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      715 2024-05-10 08:29:36.255967 metabotk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 metabotk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.31/README.md
+-rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.31/metabotk/__init__.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.31/metabotk/cli.py
+-rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.31/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.31/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.31/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.31/metabotk/imputation.py
+-rw-r--r--   0        0        0     6553 2024-05-10 08:22:09.586411 metabotk-0.1.31/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.31/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.31/metabotk/models_handler.py
+-rw-r--r--   0        0        0     2975 2024-05-10 08:44:45.590191 metabotk-0.1.31/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.31/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.31/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.31/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.31/metabotk/utils.py
+-rw-r--r--   0        0        0     4527 2024-04-19 13:40:45.180792 metabotk-0.1.31/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      716 2024-05-10 08:45:33.867106 metabotk-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 metabotk-0.1.31/PKG-INFO
```

### Comparing `metabotk-0.1.3/metabotk/cli.py` & `metabotk-0.1.31/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/dataset_manager.py` & `metabotk-0.1.31/metabotk/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/dimensionality_reduction.py` & `metabotk-0.1.31/metabotk/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/feature_selection.py` & `metabotk-0.1.31/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/imputation.py` & `metabotk-0.1.31/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/interface.py` & `metabotk-0.1.31/metabotk/interface.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/missing_handler.py` & `metabotk-0.1.31/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/models_handler.py` & `metabotk-0.1.31/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/normalization.py` & `metabotk-0.1.31/metabotk/normalization.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
     This class provides a simple interface to perform normalization on the data using various approaches.
     For now only SERRF is included.
     """
 
     def __init__(
         self,
-        dataset_manager,
+        # dataset_manager,
     ):
         """
         Initialize the class.
         """
-        self._dataset_manager = dataset_manager
+        # self._dataset_manager = dataset_manager
 
     def serrf(
         self,
+        dataset,
         sample_type_column="measurement_group",
         batch_column="batch",
         time_column="time",
         other_columns=None,
         n_correlated_metabolites=10,
         random_state=None,
         threads=1,
@@ -65,17 +66,9 @@
             batch_column=batch_column,
             time_column=time_column,
             other_columns=other_columns,
             n_correlated_metabolites=n_correlated_metabolites,
             random_state=random_state,
             threads=threads,
         )
-        input_dataset = self._dataset_manager.sample_metadata[
-            [
-                self._dataset_manager._sample_id_column,
-                sample_type_column,
-                batch_column,
-                time_column,
-            ]
-        ].merge(self._dataset_manager.data, left_index=True, right_index=True)
-        normalized = serrf_instance.fit_transform(input_dataset, return_data_only=True)
+        normalized = serrf_instance.fit_transform(dataset, return_data_only=True)
         return normalized
```

### Comparing `metabotk-0.1.3/metabotk/outliers_handler.py` & `metabotk-0.1.31/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/providers_handler.py` & `metabotk-0.1.31/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/statistics_handler.py` & `metabotk-0.1.31/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/utils.py` & `metabotk-0.1.31/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/metabotk/visualization_handler.py` & `metabotk-0.1.31/metabotk/visualization_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.3/pyproject.toml` & `metabotk-0.1.31/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.3"
+version = "0.1.31"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
```

### Comparing `metabotk-0.1.3/PKG-INFO` & `metabotk-0.1.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabotk
-Version: 0.1.3
+Version: 0.1.31
 Summary: Python toolkit for working with metabolomics data
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

