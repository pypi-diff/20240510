# Comparing `tmp/metabotk-0.1.31.tar.gz` & `tmp/metabotk-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.31.tar", max compression
+gzip compressed data, was "metabotk-0.1.33.tar", max compression
```

## Comparing `metabotk-0.1.31.tar` & `metabotk-0.1.33.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.31/README.md
--rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.31/metabotk/__init__.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.31/metabotk/cli.py
--rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.31/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.31/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.31/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.31/metabotk/imputation.py
--rw-r--r--   0        0        0     6553 2024-05-10 08:22:09.586411 metabotk-0.1.31/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.31/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.31/metabotk/models_handler.py
--rw-r--r--   0        0        0     2975 2024-05-10 08:44:45.590191 metabotk-0.1.31/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.31/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.31/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.31/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.31/metabotk/utils.py
--rw-r--r--   0        0        0     4527 2024-04-19 13:40:45.180792 metabotk-0.1.31/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      716 2024-05-10 08:45:33.867106 metabotk-0.1.31/pyproject.toml
--rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 metabotk-0.1.31/PKG-INFO
+-rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.33/README.md
+-rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.33/metabotk/__init__.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.33/metabotk/cli.py
+-rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.33/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.33/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.33/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.33/metabotk/imputation.py
+-rw-r--r--   0        0        0     6549 2024-05-10 08:47:44.397753 metabotk-0.1.33/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.33/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.33/metabotk/models_handler.py
+-rw-r--r--   0        0        0     2975 2024-05-10 10:04:08.418203 metabotk-0.1.33/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.33/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.33/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.33/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.33/metabotk/utils.py
+-rw-r--r--   0        0        0     4826 2024-05-10 10:04:05.970144 metabotk-0.1.33/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      716 2024-05-10 10:05:14.923804 metabotk-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 metabotk-0.1.33/PKG-INFO
```

### Comparing `metabotk-0.1.31/metabotk/cli.py` & `metabotk-0.1.33/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/dataset_manager.py` & `metabotk-0.1.33/metabotk/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/dimensionality_reduction.py` & `metabotk-0.1.33/metabotk/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/feature_selection.py` & `metabotk-0.1.33/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/imputation.py` & `metabotk-0.1.33/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/interface.py` & `metabotk-0.1.33/metabotk/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             self._imputation_ = ImputationHandler(self)
         return self._imputation_
 
     @property
     def normalization(self):
         """Lazy initialization of NormalizationHandler instance."""
         if not hasattr(self, "_normalization_"):
-            self._normalization_ = NormalizationHandler(self)
+            self._normalization_ = NormalizationHandler()
         return self._normalization_
 
     @property
     def feature_selection(self):
         """Lazy initialization of FeatureSelection instance."""
         if not hasattr(self, "_feature_selection_"):
             self._feature_selection_ = FeatureSelection(self)
```

### Comparing `metabotk-0.1.31/metabotk/missing_handler.py` & `metabotk-0.1.33/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/models_handler.py` & `metabotk-0.1.33/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/normalization.py` & `metabotk-0.1.33/metabotk/normalization.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/outliers_handler.py` & `metabotk-0.1.33/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/providers_handler.py` & `metabotk-0.1.33/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/statistics_handler.py` & `metabotk-0.1.33/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/utils.py` & `metabotk-0.1.33/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.31/metabotk/visualization_handler.py` & `metabotk-0.1.33/metabotk/visualization_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """Instance of DataManager class"""
 
         self.dimensionality_reduction = DimensionalityReduction(
             data_manager=self.data_manager
         )
         """Instance of DimensionalityReduction class"""
 
-    def plot_pca(self, pca=None, x="PC1", y="PC2", hue=None, savepath=None):
+    def plot_pca(self, pca=None, x="PC1", y="PC2", hue=None, style=None, savepath=None):
         """
         Plot the results of principal component analysis (PCA).
 
         This function plots the PCA results using seaborn's scatterplot function.
         If no PCA data is provided, it will compute the PCA with 3 components
         and plot the results.
 
@@ -44,47 +44,52 @@
             using the `get_pca` function from the `DimensionalityReduction` class.
         x: str, default='PC1'
             Name of the X-axis.
         y: str, default='PC2'
             Name of the Y-axis.
         hue: str, optional
             Column name in sample metadata DataFrame to color the points by.
+        style: str, optional
+            Column name in sample metadata DataFrame to shape the points by.
         savepath: str, optional
             Path to save the plot as an image file. If not provided, the plot
             will not be saved.
 
         Returns
         -------
         plot: seaborn.axisgrid.FacetGrid
             Seaborn scatterplot object.
         """
         if not pca:
             print("PCA not found, computing now with 3 components...")
             pca = self.dimensionality_reduction.get_pca(n_components=3)
-        plot = sns.scatterplot(data=pca, x=x, y=y, hue=hue)
+        plot = sns.scatterplot(data=pca, x=x, y=y, hue=hue, style=style)
         if savepath:
             plot.figure.savefig(savepath)
         return plot
 
     def plot_pca_grid(
         self,
         pca: pd.DataFrame = None,
         hue: Optional[str] = None,
+        style: Optional[str] = None,
         savepath: Optional[str] = None,
     ) -> sns.axisgrid.PairGrid:
         """
         Plot PCA results in a grid using seaborn's pairplot.
 
         Parameters
         ----------
         pca: pandas.DataFrame, optional
             DataFrame with PCA results. If not provided, it will be computed
             using the `get_pca` function from the `DimensionalityReduction` class.
         hue: str, optional
             Column name in sample metadata DataFrame to color the points by.
+        style: str, optional
+            Column name in sample metadata DataFrame to shape the points by.
         savepath: str, optional
             Path to save the plot as an image file. If not provided, the plot
             will not be saved.
 
         Returns
         -------
         plot: seaborn.axisgrid.PairGrid
@@ -93,14 +98,15 @@
         if pca is None:
             print("PCA not found, computing now with 3 components...")
             pca = self.dimensionality_reduction.get_pca(n_components=3)
         plot = sns.pairplot(
             data=pca,
             vars=[col for col in pca.columns if col.startswith("PC")],
             hue=hue,
+            style=style,
             diag_kind="kde",
             diag_kws={"linewidth": 0, "shade": False},
         )
 
         if savepath:
             plot.fig.savefig(savepath)
```

### Comparing `metabotk-0.1.31/pyproject.toml` & `metabotk-0.1.33/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.31"
+version = "0.1.33"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
```

### Comparing `metabotk-0.1.31/PKG-INFO` & `metabotk-0.1.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabotk
-Version: 0.1.31
+Version: 0.1.33
 Summary: Python toolkit for working with metabolomics data
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

