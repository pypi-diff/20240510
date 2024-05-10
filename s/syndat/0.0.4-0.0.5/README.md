# Comparing `tmp/syndat-0.0.4.tar.gz` & `tmp/syndat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndat-0.0.4.tar", last modified: Mon May  6 13:41:48 2024, max compression
+gzip compressed data, was "syndat-0.0.5.tar", last modified: Fri May 10 12:59:36 2024, max compression
```

## Comparing `syndat-0.0.4.tar` & `syndat-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 13:41:44.000000 syndat-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 13:41:48.673997 syndat-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-06 13:41:44.000000 syndat-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:41:48.673997 syndat-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 13:41:46.000000 syndat-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/syndat/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/syndat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-06 13:41:44.000000 syndat-0.0.4/tests/test_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 13:41:44.000000 syndat-0.0.4/tests/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-06 13:41:44.000000 syndat-0.0.4/tests/test_jsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-10 12:59:32.000000 syndat-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 12:59:36.206779 syndat-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-10 12:59:32.000000 syndat-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:59:36.206779 syndat-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 12:59:34.000000 syndat-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/syndat/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/syndat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-10 12:59:32.000000 syndat-0.0.5/tests/test_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-10 12:59:32.000000 syndat-0.0.5/tests/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-10 12:59:32.000000 syndat-0.0.5/tests/test_jsd.py
```

### Comparing `syndat-0.0.4/LICENSE` & `syndat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syndat-0.0.4/README.md` & `syndat-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `syndat-0.0.4/setup.py` & `syndat-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='syndat',
-    version='v0.0.4',
+    version='v0.0.5',
     packages=['syndat'],
     url='https://github.com/SCAI-BIO/syndat',
     license='CC BY-NC-ND 4.0.',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

### Comparing `syndat-0.0.4/syndat/quality.py` & `syndat-0.0.5/syndat/quality.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Union
 
+import logging
 import pandas
 import pandas as pd
 import numpy as np
 import scipy.spatial.distance
 
 from sklearn import ensemble
 from sklearn.model_selection import cross_val_score
 
 from syndat.domain import AggregationMethod
 
 
+
 def auc(real: pandas.DataFrame, synthetic: pandas.DataFrame, n_folds=10, score: bool = True) -> float:
     """
     Computes the Differentiation Complexity Score / ROC AUC score of a classifier trained to differentiate between real
     and synthetic data.
 
     :param real: The real data.
     :param synthetic: The synthetic data
@@ -55,15 +57,18 @@
     for col in real:
         # delete empty cells
         real_wo_missing = real[col].dropna()
         # binning
         col_dtype_real = real[col].dtype
         col_dtype_synthetic = synthetic[col].dtype
         if col_dtype_real != col_dtype_synthetic:
-            raise TypeError(f'Real data at col {col} is dtype {col_dtype_real} but synthetic is {col_dtype_synthetic}.')
+            logging.warning(f'Real data at col {col} is dtype {col_dtype_real} but synthetic is {col_dtype_synthetic}. '
+                            f'Evaluation will be done based on the assumed data type of the real data.')
+            for col_synth in synthetic.columns:
+                synthetic[col_synth] = synthetic[col_synth].astype(real[col_synth].dtype)
         if col_dtype_real == "int64" or col_dtype_real == "object":
             # categorical column
             real_binned = np.bincount(real[col])
             virtual_binned = np.bincount(synthetic[col])
         else:
             # get optimal amount of bins
             n_bins = np.histogram_bin_edges(real_wo_missing, bins='auto')
@@ -75,26 +80,26 @@
         if len(real_binned) != len(virtual_binned):
             padding_size = np.abs(len(real_binned) - len(virtual_binned))
             if len(real_binned) > len(virtual_binned):
                 virtual_binned = np.pad(virtual_binned, (0, padding_size))
             else:
                 real_binned = np.pad(real_binned, (0, padding_size))
         # compute jsd
-        jsd = scipy.spatial.distance.jensenshannon(real_binned, virtual_binned)
+        jsd = scipy.spatial.distance.jensenshannon(real_binned, virtual_binned, 2)
         jsd_dict[col] = jsd
     if not aggregate_results:
         return jsd_dict
     if aggregate_results and aggregation_method == AggregationMethod.AVERAGE:
         jsd_aggregated = np.mean(np.array(list(jsd_dict.values())))
     elif aggregate_results and aggregation_method == AggregationMethod.MEDIAN:
         jsd_aggregated = np.median(np.array(list(jsd_dict.values())))
     if not score:
         return jsd_aggregated
     else:
-        return (1 - jsd_aggregated) * 100
+        return int((1 - jsd_aggregated) * 100)
 
 
 def correlation(real: pandas.DataFrame, synthetic: pandas.DataFrame, score=True) -> float:
     """
     Computes the correlation similarity of real and synthetic data.
 
     :param real: The real data.
```

### Comparing `syndat-0.0.4/syndat/visualization.py` & `syndat-0.0.5/syndat/visualization.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,35 @@
     :param real: The real data
     :param synthetic: The synthetic data
     :param store_destination: Path to the folder where the results should be stored.
     """
     for column_name in real.columns:
         matplotlib.use('Agg')
         real_col = real[column_name].to_numpy()
-        virtual_col = synthetic[column_name].to_numpy()
+        synthetic_col = synthetic[column_name].to_numpy()
         plt.figure()
         plt.title(column_name)
-        patient_types = np.concatenate([np.zeros(real_col.size), np.ones(virtual_col.size)])
+        patient_types = np.concatenate([np.zeros(real_col.size), np.ones(synthetic_col.size)])
         df = pd.DataFrame(data={"type": np.where(patient_types == 0, "real", "synthetic"),
-                                "value": np.concatenate([real_col, virtual_col])})
+                                "value": np.concatenate([real_col, synthetic_col])})
         if real_col.dtype == str or real_col.dtype == object:
             ax = sns.countplot(data=df, x="value", hue="type", order=df['value'].value_counts().index)
         elif np.sum(real_col) % 1 == 0 and np.max(real_col) < 10:
             ax = sns.countplot(data=df, x="value", hue="type")
         else:
-            df = pd.DataFrame(data={"real": real_col, "synthetic": virtual_col})
+            if len(real_col) != len(synthetic_col):
+                # Determine the length of the longest column
+                max_length = max(len(real_col), len(synthetic_col))
+                # Fill the shorter column with NaN values to match the length of the longest column
+                real_col = np.pad(real_col, pad_width=(0, max_length - len(real_col)), mode='constant',
+                                  constant_values=np.nan)
+                synthetic_col = np.pad(synthetic_col, pad_width=(0, max_length - len(synthetic_col)), mode='constant',
+                                       constant_values=np.nan)
+            # create df with now equal values
+            df = pd.DataFrame(data={"real": real_col, "synthetic": synthetic_col})
             ax = sns.violinplot(data=df)
             # remove y-labels as they are redundant with the table headers
             ax.set_xticks([])
             table(ax, df.describe().round(2), loc='bottom', colLoc='center', bbox=[0, -0.55, 1, 0.5],
                   colWidths=[.5, .5])
         fig = ax.get_figure()
         matplotlib.pyplot.close()
```

### Comparing `syndat-0.0.4/tests/test_auc.py` & `syndat-0.0.5/tests/test_auc.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.4/tests/test_correlation.py` & `syndat-0.0.5/tests/test_correlation.py`

 * *Files identical despite different names*

