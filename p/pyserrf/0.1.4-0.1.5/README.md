# Comparing `tmp/pyserrf-0.1.4.tar.gz` & `tmp/pyserrf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserrf-0.1.4.tar", max compression
+gzip compressed data, was "pyserrf-0.1.5.tar", max compression
```

## Comparing `pyserrf-0.1.4.tar` & `pyserrf-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      706 2024-05-09 16:37:05.507311 pyserrf-0.1.4/README.md
--rw-r--r--   0        0        0      574 2024-05-09 16:36:27.382444 pyserrf-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-09 16:35:29.205036 pyserrf-0.1.4/pyserrf/__init__.py
--rw-r--r--   0        0        0     4457 2024-05-09 16:46:10.288319 pyserrf-0.1.4/pyserrf/cross_validation.py
--rw-r--r--   0        0        0     4304 2024-05-09 16:46:06.092216 pyserrf-0.1.4/pyserrf/read_data.py
--rwxr-xr-x   0        0        0      343 2024-05-09 07:48:10.466322 pyserrf-0.1.4/pyserrf/run.py
--rw-r--r--   0        0        0    21525 2024-05-09 16:20:21.673546 pyserrf-0.1.4/pyserrf/serrf.py
--rw-r--r--   0        0        0     6689 2024-05-09 15:20:31.455760 pyserrf-0.1.4/pyserrf/utils.py
--rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 pyserrf-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      706 2024-05-09 16:37:05.507311 pyserrf-0.1.5/README.md
+-rw-r--r--   0        0        0      574 2024-05-09 17:37:16.604043 pyserrf-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4442 2024-05-09 17:26:26.747085 pyserrf-0.1.5/pyserrf/CV.py
+-rw-r--r--   0        0        0       70 2024-05-09 16:35:29.205036 pyserrf-0.1.5/pyserrf/__init__.py
+-rw-r--r--   0        0        0     4457 2024-05-09 16:46:10.288319 pyserrf-0.1.5/pyserrf/cross_validation.py
+-rw-r--r--   0        0        0     4304 2024-05-09 16:46:06.092216 pyserrf-0.1.5/pyserrf/read_data.py
+-rwxr-xr-x   0        0        0      343 2024-05-09 07:48:10.466322 pyserrf-0.1.5/pyserrf/run.py
+-rw-r--r--   0        0        0    18453 2024-05-09 17:33:16.965810 pyserrf-0.1.5/pyserrf/serrf.py
+-rw-r--r--   0        0        0      169 2024-05-09 17:33:30.162153 pyserrf-0.1.5/pyserrf/test2.py
+-rw-r--r--   0        0        0     6689 2024-05-09 17:32:28.008534 pyserrf-0.1.5/pyserrf/utils.py
+-rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 pyserrf-0.1.5/PKG-INFO
```

### Comparing `pyserrf-0.1.4/README.md` & `pyserrf-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyserrf-0.1.4/pyproject.toml` & `pyserrf-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyserrf"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python implementation of the Systematic Error Removal Using Random Forest algorithm"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `pyserrf-0.1.4/pyserrf/cross_validation.py` & `pyserrf-0.1.5/pyserrf/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pyserrf-0.1.4/pyserrf/read_data.py` & `pyserrf-0.1.5/pyserrf/read_data.py`

 * *Files identical despite different names*

### Comparing `pyserrf-0.1.4/pyserrf/serrf.py` & `pyserrf-0.1.5/pyserrf/serrf.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,55 +15,42 @@
     untargeted metabolomics data.
     data. The method was developed by the Fan et al. in 2015 [1]_
     (see https://slfan2013.github.io/SERRF-online/).
 
     The class takes as input a pandas DataFrame containing metabolomic data and
     sample metadata, and outputs a pandas DataFrame with the normalized data.
 
-    The class has the following parameters:
-
-    - `sample_type_column` is the name of the column in the sample metadata
-      with the sample type information (i.e qc or normal sample). The default
-      value is 'sampleType'.
-    - `batch_column` is the name of the column in the sample metadata with the
-      batch information. If `None`, all samples are considered as part the same
-      batch. The default value is `None`.
-    - `sample_metadata_columns` is a list with the names of the columns in the
-      sample metadata; it is important to specify all the metadata columns to
-      separate them from the metabolite abundance values.
-      The default value is ['sampleType', 'batch', 'label', 'time'].
-    - `random_state` is the random seed used for all methods with a random
-      component (i.e numpy normal distribution, sklearn random forest regressor).
-      The default value is `None`, which means that a random seed is
-      generated automatically. To obtain reproducible results, set a specific
-      random seed.
-
-    - `n_correlated_metabolites` is the number of metabolites with the highest
-        correlation to the metabolite to be normalized. The default value is 10.
-
-    Attributes:
-    -----------
-    _metabolites : list
-        List with the names of the metabolites.
-    _dataset : pandas DataFrame
-        DataFrame with the metabolomic data and the sample metadata.
-    _metabolite_dict : dict
-        Dictionary with the mapping between the original column names and the
-        new column names (MET_1, MET_2, etc.).
-    corrs_qc : pandas DataFrame
-        DataFrame with the Pearson correlation coefficients between the
-        metabolites and the batch information.
-    corrs_target : pandas DataFrame
-        DataFrame with the Pearson correlation coefficients between the
-        metabolites and the samples.
-    normalized_data : pandas DataFrame
-        DataFrame with the normalized data.
-    normalized_dataset : pandas DataFrame
-        DataFrame with the normalized data and the sample metadata.
-
+    Parameters
+    ----------
+    sample_type_column : str, optional
+        The name of the column in the sample metadata with the sample type
+        information (i.e qc or normal sample). The default value is
+        'sampleType'.
+    batch_column : str, optional
+        The name of the column in the sample metadata with the batch
+        information. If None, all samples are considered as part the same
+        batch. The default value is 'batch'.
+    time_column: str, optional
+        The name of the column in the sample metadata with the injection time
+        information.The default value is 'time'.
+    other_columns : list of str or None, optional
+        A list with the names of other metadata columns in the dataset; it is
+        important to specify all the metadata columns to separate them from
+        the metabolite abundance values. The default value is None
+    random_state : int, RandomState instance, or None, optional
+        The random seed used for all methods with a random component (i.e
+        numpy normal distribution, sklearn random forest regressor). The
+        default value is None, which means that a random seed is generated
+        automatically. To obtain reproducible results, set a specific random
+        seed.
+    n_correlated_metabolites : int, optional
+        The number of metabolites with the highest correlation to the
+        metabolite to be normalized. The default value is 10.
+    threads: int, optional
+        Number of threads to use for parallel processing
     References
     ----------
     .. [1] Fan et al.:
         Systematic Error Removal using Random Forest (SERRF) for Normalizing
         Large-Scale Untargeted Lipidomics Data
         Analytical Chemistry DOI: 10.1021/acs.analchem.8b05592
         https://slfan2013.github.io/SERRF-online/
@@ -77,78 +64,16 @@
         other_columns=None,
         n_correlated_metabolites=10,
         random_state=None,
         threads=1,
     ):
         """
         Initialize the class.
-
-        Parameters
-        ----------
-        sample_type_column : str, optional
-            The name of the column in the sample metadata with the sample type
-            information (i.e qc or normal sample). The default value is
-            'sampleType'.
-        batch_column : str, optional
-            The name of the column in the sample metadata with the batch
-            information. If None, all samples are considered as part the same
-            batch. The default value is 'batch'.
-        time_column: str, optional
-            The name of the column in the sample metadata with the injection time
-            information.The default value is 'time'.
-        other_columns : list of str or None, optional
-            A list with the names of other metadata columns in the dataset; it is
-            important to specify all the metadata columns to separate them from
-            the metabolite abundance values. The default value is None
-        random_state : int, RandomState instance, or None, optional
-            The random seed used for all methods with a random component (i.e
-            numpy normal distribution, sklearn random forest regressor). The
-            default value is None, which means that a random seed is generated
-            automatically. To obtain reproducible results, set a specific random
-            seed.
-        n_correlated_metabolites : int, optional
-            The number of metabolites with the highest correlation to the
-            metabolite to be normalized. The default value is 10.
-
-        Attributes
-        ----------
-        sample_metadata_columns : list of str
-            The list of columns in the sample metadata.
-        sample_type_column : str
-            The name of the column in the sample metadata with the sample type
-            information.
-        batch_column : str or None
-            The name of the column in the sample metadata with the batch
-            information.
-        random_state : int, RandomState instance, or None
-            The random seed used for all methods with a random component.
-        n_correlated_metabolites : int
-            The number of metabolites with the highest correlation to the
-            metabolite to be normalized.
-        _metabolites : list of str
-            List with the names of the metabolites.
-        _dataset : pandas DataFrame
-            DataFrame with the metabolomic data and the sample metadata.
-        _metabolite_dict : dict
-            Dictionary with the mapping between the original column names and
-            the new column names (MET_1, MET_2, etc.).
-        _sample_metadata : pandas DataFrame containing the sample metadata.
-        corrs_qc : pandas DataFrame
-            DataFrame with the Pearson correlation coefficients between the
-            metabolites and the batch information.
-        corrs_target : pandas DataFrame
-            DataFrame with the Pearson correlation coefficients between the
-            metabolites and the samples.
-        normalized_data : pandas DataFrame
-            DataFrame with the normalized data.
-        normalized_dataset : pandas DataFrame
-            DataFrame with the normalized data and the sample metadata.
         """
         # attributes for the preprocessing
-        # self.sample_metadata_columns = list(sample_metadata_columns)
         self.sample_type_column = sample_type_column
         self.batch_column = batch_column
         self.time_column = time_column
         self.other_columns = other_columns
         # attributes for the analysis
         self.random_state = random_state
         self.threads = threads
@@ -286,15 +211,15 @@
         """
 
         with Pool(
             processes=self.threads,
         ) as p:
             normalized_metabolites = list(
                 tqdm(
-                    p.imap(self._normalize_metabolite_parallel, self._metabolite_ids),
+                    p.imap(self._normalize_metabolite, self._metabolite_ids),
                     total=len(self._metabolite_ids),
                 )
             )
         self.normalized_data = pd.concat(normalized_metabolites, axis=1)
         self.normalized_data.columns = [
             self._metabolite_dict[i] for i in self.normalized_data.columns
         ]
@@ -339,18 +264,15 @@
         """
         qc = group[group[self.sample_type_column] == "qc"]
         target = group[group[self.sample_type_column] != "qc"]
         return qc, target
 
     def _get_corrs_by_sample_type_and_batch(self):
         """
-        Get the correlations by sample type and batch for the given self._dataset data.
-
-        This function calculates the Pearson's r correlation coefficient
-        for the qc and target data for each batch.
+        Get the Spearman's correlations between metabolites grouped by sample type and batch.
 
         Returns
         -------
         corrs_qc : dict
             The correlations for the qc data, keyed by batch.
         corrs_target : dict
             The correlations for the target data, keyed by batch.
@@ -410,14 +332,42 @@
             (prediction + group[metabolite].mean()) / self.qc_dataset[metabolite].mean()
         )
         norm_qc = norm_qc / (norm_qc.median() / self.qc_dataset[metabolite].median())
 
         return norm_qc
 
     def _normalize_target_with_prediction(self, metabolite, group, prediction):
+        """
+        Normalize the target data for the given metabolite using the given prediction.
+
+        The normalization formula is:
+
+        norm_target = target_data / ((prediction + target_data.mean() - prediction.mean())
+                                    / target_dataset.median())
+        norm_target = norm_target / (norm_target.median() / target_dataset.median())
+
+        The normalization is done by dividing the target data by the ratio of the
+        prediction and the median of the target dataset.  The result is then
+        divided by the ratio of the median of the normalized target data and the
+        median of the target dataset.
+
+        Parameters
+        ----------
+        metabolite : str
+            The name of the metabolite to normalize.
+        group : pandas.DataFrame
+            The target data for the given metabolite.
+        prediction : pandas.DataFrame
+            The prediction for the given metabolite.
+
+        Returns
+        -------
+        norm_target : pandas.DataFrame
+            The normalized target data.
+        """
         norm_target = group[metabolite] / (
             (prediction + group[metabolite].mean() - prediction.mean())
             / self.target_dataset[metabolite].median()
         )
         # Set negative values to the original value
         norm_target[norm_target < 0] = group[metabolite].loc[
             norm_target[norm_target < 0].index
@@ -428,18 +378,16 @@
         return norm_target
 
     def _merge_and_normalize(
         self, metabolite, norm_qc, norm_target, target_group, target_prediction
     ):
         """
         TODO: function could probably be simpler, refactor and maybe split
-        Merges the qc and target data and normalizes the data using the same
-        formula as normalize_qc_and_target.
 
-        The normalization is done separately on the qc and target data.
+        Merges the qc and target data and replaces outliers in the target data.
 
         Parameters
         ----------
         metabolite : str
             The name of the metabolite to normalize.
         norm_qc : pandas Series
             The normalized qc data.
@@ -452,22 +400,22 @@
 
         Returns
         -------
         norm : pandas Series
             The normalized data.
         """
         norm = pd.concat([norm_qc, norm_target]).sort_index()
-
         outliers = utils.detect_outliers(data=norm, threshold=3)
         outliers = outliers[outliers]
         outliers_in_target = outliers.index.intersection(norm_target.index)
 
         # Replace outlier values in the target data with the mean of the outlier
         # values in the target data minus the mean of the predicted values for the
         # target data
+
         replaced_outliers = (
             target_group[metabolite]
             - (
                 (target_prediction + target_group[metabolite].mean())
                 - (self.target_dataset[metabolite].median())
             )
         ).loc[outliers_in_target]
@@ -483,17 +431,14 @@
         norm = pd.concat([norm_qc, norm_target]).sort_index()
         # MANCA FUNZIONE PER RIMPIAZZARE INF O NAN - ORIGINALE QUA SOTTO:
         # norm[!is.finite(norm)] =
         # rnorm(length(norm[!is.finite(norm)]), sd = sd(norm[is.finite(norm)], na.rm = TRUE) * 0.01)
 
         return norm
 
-    def _normalize_metabolite_parallel(self, metabolite):
-        return self._normalize_metabolite(metabolite)
-
     def _normalize_metabolite(self, metabolite):
         """
         Normalizes the given metabolite
         Parameters
         ----------
         metabolite : str
             The name of the metabolite to normalize.
@@ -540,17 +485,16 @@
                 qc_prediction, target_prediction = utils.predict_values(
                     qc_data_x, qc_data_y, target_data_x, random_state=self.random_state
                 )
                 norm_qc = self._normalize_qc_with_prediction(
                     metabolite, qc_group, qc_prediction
                 )
                 norm_target = self._normalize_target_with_prediction(
-                    metabolite, qc_group, qc_prediction
+                    metabolite, target_group, target_prediction
                 )
-
                 norm = self._merge_and_normalize(
                     metabolite, norm_qc, norm_target, target_group, target_prediction
                 )
 
             normalized_metabolite.append(norm)
 
         normalized_metabolite = pd.concat(normalized_metabolite)
```

### Comparing `pyserrf-0.1.4/pyserrf/utils.py` & `pyserrf-0.1.5/pyserrf/utils.py`

 * *Files identical despite different names*

### Comparing `pyserrf-0.1.4/PKG-INFO` & `pyserrf-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserrf
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python implementation of the Systematic Error Removal Using Random Forest algorithm
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

