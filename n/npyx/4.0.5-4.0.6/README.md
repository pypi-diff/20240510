# Comparing `tmp/npyx-4.0.5.tar.gz` & `tmp/npyx-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npyx-4.0.5.tar", last modified: Mon Apr 22 11:02:45 2024, max compression
+gzip compressed data, was "npyx-4.0.6.tar", last modified: Fri May 10 15:01:07 2024, max compression
```

## Comparing `npyx-4.0.5.tar` & `npyx-4.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-04-22 11:02:45.179843 npyx-4.0.5/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2024-02-11 14:12:15.000000 npyx-4.0.5/LICENSE.md
--rw-r--r--   0 maxime    (1000) maxime    (1000)    30898 2024-04-22 11:02:45.179843 npyx-4.0.5/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    29668 2024-04-22 10:53:30.000000 npyx-4.0.5/README.md
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-04-22 11:02:45.175843 npyx-4.0.5/npyx/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1471 2024-04-22 11:01:11.000000 npyx-4.0.5/npyx/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    85263 2024-02-27 10:59:36.000000 npyx-4.0.5/npyx/behav.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-04-22 11:02:45.179843 npyx-4.0.5/npyx/c4/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      508 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     9201 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/acg_augmentations.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    13330 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/acg_vs_firing_rate.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    32139 2024-03-01 00:01:51.000000 npyx-4.0.5/npyx/c4/dataset_init.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    24536 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/dl_transforms.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    22124 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/dl_utils.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6388 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/encode_features.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1990 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/misc.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     6941 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/monkey_dataset_init.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    28400 2024-03-01 00:02:14.000000 npyx-4.0.5/npyx/c4/plots_functions.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    31845 2024-02-29 23:37:28.000000 npyx-4.0.5/npyx/c4/predict_cell_types.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    15717 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/run_baseline_classifier.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    47830 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/run_deep_classifier.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1353 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/c4/waveform_augmentations.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/circuitProphyler.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)   129915 2024-03-03 23:17:47.000000 npyx-4.0.5/npyx/corr.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    44562 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/datasets.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    60076 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/feat.py
--rwxrwxr-x   0 maxime    (1000) maxime    (1000)    19790 2024-04-22 11:00:43.000000 npyx-4.0.5/npyx/gl.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    42648 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/h5.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/histo.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    19397 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/info.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    50713 2024-04-22 10:53:30.000000 npyx-4.0.5/npyx/inout.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/merger.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/metrics.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     5812 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/ml.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/model.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)   140300 2024-03-06 12:50:32.000000 npyx-4.0.5/npyx/plot.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    40419 2024-03-04 14:38:20.000000 npyx-4.0.5/npyx/plot_utils.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/preprocess.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    42651 2024-02-23 17:35:21.000000 npyx-4.0.5/npyx/spk_t.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    49919 2024-02-27 11:48:15.000000 npyx-4.0.5/npyx/spk_wvf.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    14577 2024-02-26 16:17:13.000000 npyx-4.0.5/npyx/stats.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2024-02-11 14:12:15.000000 npyx-4.0.5/npyx/testing.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    68517 2024-03-03 23:13:38.000000 npyx-4.0.5/npyx/utils.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-04-22 11:02:45.179843 npyx-4.0.5/npyx.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    30898 2024-04-22 11:02:45.000000 npyx-4.0.5/npyx.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      921 2024-04-22 11:02:45.000000 npyx-4.0.5/npyx.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       37 2024-04-22 11:02:45.000000 npyx-4.0.5/npyx.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      110 2024-04-22 11:02:45.000000 npyx-4.0.5/npyx.egg-info/entry_points.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      260 2024-04-22 11:02:45.000000 npyx-4.0.5/npyx.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2024-04-22 11:02:45.000000 npyx-4.0.5/npyx.egg-info/top_level.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2024-04-22 11:02:45.179843 npyx-4.0.5/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2011 2024-04-22 10:52:17.000000 npyx-4.0.5/setup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-05-10 15:01:07.061298 npyx-4.0.6/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    35149 2024-02-11 14:12:15.000000 npyx-4.0.6/LICENSE.md
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    30179 2024-05-10 15:01:07.057298 npyx-4.0.6/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    29668 2024-04-22 10:53:30.000000 npyx-4.0.6/README.md
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-05-10 15:01:07.057298 npyx-4.0.6/npyx/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1471 2024-05-10 15:00:00.000000 npyx-4.0.6/npyx/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    85263 2024-02-27 10:59:36.000000 npyx-4.0.6/npyx/behav.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-05-10 15:01:07.057298 npyx-4.0.6/npyx/c4/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      508 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     9201 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/acg_augmentations.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    13330 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/acg_vs_firing_rate.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    32139 2024-03-01 00:01:51.000000 npyx-4.0.6/npyx/c4/dataset_init.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    24536 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/dl_transforms.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    22124 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/dl_utils.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6388 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/encode_features.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1990 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/misc.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     6941 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/monkey_dataset_init.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    28400 2024-03-01 00:02:14.000000 npyx-4.0.6/npyx/c4/plots_functions.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    34252 2024-04-27 00:55:56.000000 npyx-4.0.6/npyx/c4/predict_cell_types.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    15717 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/run_baseline_classifier.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    47830 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/run_deep_classifier.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1353 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/c4/waveform_augmentations.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    55561 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/circuitProphyler.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)   129915 2024-03-03 23:17:47.000000 npyx-4.0.6/npyx/corr.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    44562 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/datasets.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    60076 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/feat.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)    19790 2024-04-22 11:00:43.000000 npyx-4.0.6/npyx/gl.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    42648 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/h5.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/histo.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    19397 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/info.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    54833 2024-05-10 14:58:05.000000 npyx-4.0.6/npyx/inout.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    12770 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/merger.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    37349 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/metrics.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     5812 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/ml.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16904 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/model.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)   140300 2024-03-06 12:50:32.000000 npyx-4.0.6/npyx/plot.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    40419 2024-03-04 14:38:20.000000 npyx-4.0.6/npyx/plot_utils.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    38393 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/preprocess.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    42651 2024-02-23 17:35:21.000000 npyx-4.0.6/npyx/spk_t.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    49919 2024-02-27 11:48:15.000000 npyx-4.0.6/npyx/spk_wvf.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    14577 2024-02-26 16:17:13.000000 npyx-4.0.6/npyx/stats.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     3415 2024-02-11 14:12:15.000000 npyx-4.0.6/npyx/testing.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    68517 2024-03-03 23:13:38.000000 npyx-4.0.6/npyx/utils.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2024-05-10 15:01:07.057298 npyx-4.0.6/npyx.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    30179 2024-05-10 15:01:06.000000 npyx-4.0.6/npyx.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      921 2024-05-10 15:01:07.000000 npyx-4.0.6/npyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       37 2024-05-10 15:01:06.000000 npyx-4.0.6/npyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      110 2024-05-10 15:01:06.000000 npyx-4.0.6/npyx.egg-info/entry_points.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      260 2024-05-10 15:01:06.000000 npyx-4.0.6/npyx.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        5 2024-05-10 15:01:06.000000 npyx-4.0.6/npyx.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2024-05-10 15:01:07.061298 npyx-4.0.6/setup.cfg
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2011 2024-04-22 10:52:17.000000 npyx-4.0.6/setup.py
```

### Comparing `npyx-4.0.5/LICENSE.md` & `npyx-4.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/PKG-INFO` & `npyx-4.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,20 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 4.0.5
+Version: 4.0.6
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: ipython
-Requires-Dist: numpy
-Requires-Dist: scipy==1.10.0
-Requires-Dist: pandas
-Requires-Dist: numba
-Requires-Dist: statsmodels
-Requires-Dist: matplotlib
-Requires-Dist: cmcrameri
-Requires-Dist: opencv-python
-Requires-Dist: scikit-learn
-Requires-Dist: imbalanced-learn
-Requires-Dist: networkx
-Requires-Dist: psutil
-Requires-Dist: joblib>=1.3
-Requires-Dist: tqdm
-Requires-Dist: h5py
-Requires-Dist: seaborn
 Provides-Extra: c4
-Requires-Dist: torch==1.13.1; extra == "c4"
-Requires-Dist: torchvision==0.14.1; extra == "c4"
-Requires-Dist: torchaudio==0.13.1; extra == "c4"
-Requires-Dist: laplace-torch; extra == "c4"
-Requires-Dist: requests; extra == "c4"
-Requires-Dist: dill; extra == "c4"
-Requires-Dist: tabulate; extra == "c4"
+License-File: LICENSE.md
 
 [![PyPI Version](https://img.shields.io/pypi/v/npyx.svg)](https://pypi.org/project/npyx/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5509733.svg)](https://doi.org/10.5281/zenodo.5509733)
 [![License](https://img.shields.io/pypi/l/npyx.svg)](https://github.com/m-beau/NeuroPyxels/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/npyx)](https://pepy.tech/project/npyx)
 # NeuroPyxels: loading, processing and plotting Neuropixels data in Python</h1> <img src="https://raw.githubusercontent.com/m-beau/NeuroPyxels/master/images/NeuroPyxels_logo_final.png" width="150" title="Neuropyxels" alt="Neuropixels" align="right" vspace = "50">
```

### Comparing `npyx-4.0.5/README.md` & `npyx-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/__init__.py` & `npyx-4.0.6/npyx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,12 +52,12 @@
  .behav
  .merger
  .circuitProphyler
  .feat
  .h5
 """
 
-__version__ = "4.0.5"
+__version__ = "4.0.6"
 
 npyx_build = "npyx[c4]" if C4_IMPORTED else "npyx"
 
 print(f"\n\033[32;1m{npyx_build} version {__version__} imported.\033[0m")
```

### Comparing `npyx-4.0.5/npyx/behav.py` & `npyx-4.0.6/npyx/behav.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/acg_augmentations.py` & `npyx-4.0.6/npyx/c4/acg_augmentations.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/acg_vs_firing_rate.py` & `npyx-4.0.6/npyx/c4/acg_vs_firing_rate.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/dataset_init.py` & `npyx-4.0.6/npyx/c4/dataset_init.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/dl_transforms.py` & `npyx-4.0.6/npyx/c4/dl_transforms.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/dl_utils.py` & `npyx-4.0.6/npyx/c4/dl_utils.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/encode_features.py` & `npyx-4.0.6/npyx/c4/encode_features.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/misc.py` & `npyx-4.0.6/npyx/c4/misc.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/monkey_dataset_init.py` & `npyx-4.0.6/npyx/c4/monkey_dataset_init.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/plots_functions.py` & `npyx-4.0.6/npyx/c4/plots_functions.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/predict_cell_types.py` & `npyx-4.0.6/npyx/c4/predict_cell_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 import npyx.corr as corr
 import npyx.datasets as datasets
 from npyx.gl import get_units, load_units_qualities
 from npyx.spk_t import trn, trn_filtered
 from npyx.spk_wvf import wvf_dsmatch
 
+import ast
+ale = ast.literal_eval
+
 from .dataset_init import ArgsNamespace, download_file, extract_and_check
 from .misc import require_advanced_deps
 from .plots_functions import (
     C4_COLORS,
     plot_features_1cell_vertical,
     plot_survival_confidence,
 )
@@ -60,15 +63,16 @@
 
 C4_MESSAGE = (
     "\n"
     "Welcome to the cerebellar cell type classifier of the Cerebellar Cell types Classification Collaboration (C4)!\n"
     "\nYou can use this command ('c4' or 'predict_cell_types') to run the C4 classifier on a phy-compatible dataset (find our preprint here: https://www.biorxiv.org/content/10.1101/2024.01.30.577845v1)."
     "\nTo run the classifier on the phy-compatible dataset in the current working directory, simply run 'c4 -dp .'. To run it on a phy-compatible dataset present elsewhere, run 'c4 -dp path/to/my/dataset'."
     "\nBy default, the classifier will predict the cell types of all the 'good' units of the dataset (as defined in phy by manual curation), and it will not use layer information. To alter this behaviour, see the options below."
-    "\n"
+    "\n\n"
+    "If the results feel off, it might be because of a caching bug (they happen frequently, sorry about that). To solve your problem, try running the classifier again with the option '--again'."
 )
 
 
 def get_n_cores(num_cores):
     max_num_cores = 60
     max_num_cores = min(multiprocessing.cpu_count(), max_num_cores)
     num_cores = min(num_cores, max_num_cores)
@@ -127,15 +131,17 @@
             else:
                 print("\n  >> Please answer y or n!")
     # Remove potential conflicts with previous versions of the tool
     if os.path.exists(os.path.join(data_path, "cluster_cell_types.tsv")):
         os.remove(os.path.join(data_path, "cluster_cell_types.tsv"))
 
 
-def prepare_dataset_from_binary(dp, units, again=False, fp_threshold=0.05, fn_threshold=0.05):
+def prepare_dataset_from_binary(dp, units, again=False,
+                                fp_threshold=0.05, fn_threshold=0.05,
+                                peak_sign="negative"):
     waveforms = []
     acgs_3d = []
     bad_units = []
     for u in tqdm(
         units,
         desc="Preparing waveforms and ACGs for classification",
         position=0,
@@ -163,15 +169,16 @@
             bad_units.append(u)
             continue
 
         try:
             wvf, _, _, _ = wvf_dsmatch(dp, u, t_waveforms=120, again=again)
         except (IndexError, pd.errors.EmptyDataError, ValueError):
             wvf, _, _, _ = wvf_dsmatch(dp, u, t_waveforms=120, again=True)
-        waveforms.append(datasets.preprocess_template(wvf))
+        waveforms.append(datasets.preprocess_template(wvf,
+                                                      peak_sign=peak_sign))
 
         _, acg = corr.crosscorr_vs_firing_rate(t, t, 2000, 1)
         acg, _ = corr.convert_acg_log(acg, 1, 2000)
         acgs_3d.append(acg.ravel() * 10)
 
     if bad_units:
         print(f"Units {str(bad_units)[1:-1]} were skipped because they had too few good spikes.")
@@ -238,15 +245,17 @@
         _acg_mask=None,
         _acg_multi_factor=10,
     )
 
     return dataset, dataset_class.h5_ids.tolist()
 
 
-def aux_prepare_dataset(dp, u, again=False, fp_threshold=0.05, fn_threshold=0.05):
+def aux_prepare_dataset(dp, u, again=False,
+                        fp_threshold=0.05, fn_threshold=0.05,
+                        peak_sign="negative"):
     t = trn(dp, u)
     if len(t) < 100:
         # Bad units
         return [True, [], []]
 
     # We set period_m to None to use the whole recording
     # We catch here and for the waveforms common errors that can be solved by setting again=True in npyx
@@ -267,33 +276,36 @@
         # Bad units
         return [True, [], []]
 
     try:
         wvf, _, _, _ = wvf_dsmatch(dp, u, t_waveforms=120, again=again)
     except (IndexError, pd.errors.EmptyDataError, ValueError, pickle.UnpicklingError):
         wvf, _, _, _ = wvf_dsmatch(dp, u, t_waveforms=120, again=True)
-    waveforms = datasets.preprocess_template(wvf)
+    waveforms = datasets.preprocess_template(wvf,
+                                             peak_sign=peak_sign)
 
     _, acg = corr.crosscorr_vs_firing_rate(t, t, 2000, 1)
     acg, _ = corr.convert_acg_log(acg, 1, 2000)
     acgs_3d = acg.ravel() * 10
 
     return [False, waveforms, acgs_3d]
 
 
-def prepare_dataset_from_binary_parallel(dp, units, again=False, fp_threshold=0.05, fn_threshold=0.05):
+def prepare_dataset_from_binary_parallel(dp, units, again=False,
+                                         fp_threshold=0.05, fn_threshold=0.05,
+                                         peak_sign="negative"):
     waveforms = []
     acgs_3d = []
     bad_units = []
 
     num_cores = get_n_cores(len(units))
 
     with redirect_stdout_fd(open(os.devnull, "w")):
         dataset_results = Parallel(n_jobs=num_cores, prefer="processes")(
-            delayed(aux_prepare_dataset)(dp, u, again, fp_threshold, fn_threshold)
+            delayed(aux_prepare_dataset)(dp, u, again, fp_threshold, fn_threshold, peak_sign)
             for u in tqdm(units, desc="Preparing waveforms and ACGs for classification")
         )
 
     for i in range(len(units)):
         if dataset_results[i][0] is True:
             bad_units.append(units[i])
         else:
@@ -303,14 +315,16 @@
     if bad_units:
         print(f"Units {str(bad_units)[1:-1]} were skipped because they had too few good spikes.")
     acgs_3d = np.array(acgs_3d)
     waveforms = np.array(waveforms)
 
     if len(acgs_3d) == 0:
         raise ValueError("No units were found with the provided parameter choices after quality checks.")
+    
+    # np.save("/home/maxime/Downloads/test_concat_data.npy", np.concatenate((acgs_3d, waveforms), axis=1))
 
     return np.concatenate((acgs_3d, waveforms), axis=1), bad_units
 
 
 def prepare_dataset(args: ArgsNamespace) -> tuple:
     """
     Prepare the dataset for classification.
@@ -328,22 +342,32 @@
     if os.path.isfile(args.data_path) and args.data_path.endswith(".h5"):
         prediction_dataset, good_units = prepare_dataset_from_h5(args.data_path)
 
     # Otherwise we are dealing with a phy output folder
     else:
         # First extract the units from the phy output folder
         if args.units is not None:
-            units = args.units
+            units = [int(u) for u in args.units]
         else:
             units = get_units(args.data_path, args.quality)
 
         if args.parallel:
-            prediction_dataset, bad_units = prepare_dataset_from_binary_parallel(args.data_path, units, args.again)
+            prediction_dataset, bad_units = prepare_dataset_from_binary_parallel(args.data_path,
+                                                                                 units,
+                                                                                 args.again,
+                                                                                 args.fp_threshold,
+                                                                                 args.fn_threshold,
+                                                                                 args.peak_sign)
         else:
-            prediction_dataset, bad_units = prepare_dataset_from_binary(args.data_path, units, args.again)
+            prediction_dataset, bad_units = prepare_dataset_from_binary(args.data_path,
+                                                                        units,
+                                                                        args.again,
+                                                                        args.fp_threshold,
+                                                                        args.fn_threshold,
+                                                                        args.peak_sign)
 
         good_units = [u for u in units if u not in bad_units]
 
     return prediction_dataset, good_units
 
 
 def format_predictions(predictions_matrix: np.ndarray) -> tuple:
@@ -441,14 +465,15 @@
     mli_clustering: bool = False,
     layer: bool = False,
     threshold: float = 2,
     parallel: bool = True,
     again: bool = False,
     fp_threshold: float = 0.05,
     fn_threshold: float = 0.05,
+    waveform_peak_sign: str = "negative",
 ) -> None:
     """
     Predicts the cell types of units in a given dataset using a pre-trained ensemble of classifiers.
 
     Args:
         data_path (str, optional): Path to the ephys dataset folder. Defaults to ".".
         quality (str, optional): Quality of the units to use. Must be either "all" or "good". Defaults to "good".
@@ -469,25 +494,31 @@
         mli_clustering=mli_clustering,
         use_layer=layer,
         threshold=threshold,
         parallel=parallel,
         again=again,
         fp_threshold=fp_threshold,
         fn_threshold=fn_threshold,
+        peak_sign=waveform_peak_sign,
     )
 
     assert args.quality in [
         "all",
         "good",
     ], "Invalid value for 'quality'. Must be either 'all' or 'good'."
 
     assert (args.fp_threshold >= 0) & (args.fp_threshold < 1),\
         "Invalid value for 'fp_threshold'. Must be within [0-1[."
     assert (args.fn_threshold >= 0) & (args.fn_threshold < 1),\
         "Invalid value for 'fn_threshold'. Must be within [0-1[."
+    
+    assert args.peak_sign in ["positive", "negative", "None"],\
+        "Invalid value for 'peak_sign'. Must be 'positive', 'negative', or 'None'."
+    if args.peak_sign == "None":
+        args.peak_sign = None
 
     # Perform some checks on the data folder
     directory_checks(args.data_path)
 
     if args.data_path.endswith(".h5") == False:
         # This function checks the content of cluster_group.tsv file and regenerate this one if it is required.
         load_units_qualities(args.data_path, again=True)
@@ -711,17 +742,17 @@
         default="good",
         help="Units of which quality we should classify. Choose 'all' to classify all units or 'good' to classify only good units. \n Optional argument, default is 'good'.",
     )
 
     parser.add_argument(
         "--units",
         nargs="+",
-        type=int,
+        type=str,
         default=None,
-        help="Which units to classify. If not specified, falls back to all units of 'quality' (all good units by default). Specify the unit IDs as space-separated integers after the '--units' argument.",
+        help="List of units to classify '[u1, u2, u3...]'. If not specified, falls back to all units of 'quality' (all good units by default). Specify the unit IDs as space-separated integers after the '--units' argument.",
     )
     parser.add_argument(
         "--mli_clustering",
         action="store_true",
         help="Divide MLI into two clusters. Optional argument, default is to not use MLI clustering.",
     )
     parser.set_defaults(mli_clustering=False)
@@ -774,29 +805,39 @@
     parser.add_argument(
         "--fn_threshold",
         type=float,
         default="0.05",
         help="False negative rate (a.k.a. AUC fraction of amplitude clipping) threshold. To be deemed classifiable, a unit must feature three minutes of data with less than a fn_threshold fraction of false negative (and fp_threshold false positive) rate. To include more units despite their refractory period violations, increease this threshold. \nOptional argument, default is 0.05.",
     )
 
+    parser.add_argument(
+        "--waveform_peak_sign",
+        type=str,
+        default="negative",
+        help="Use at your own risk - sign of the waveform to make the prediction, among ['negative', 'positive', 'None']. The classifier was trained with waveforms whose peak was always negative. \nOptional argument, default is negative.",
+    )
+
     # Check if no arguments were provided, and if so, print help and exit
     if len(sys.argv) == 1:
         if c4:
             print(C4_MESSAGE)
         else:
             print(
                 "\nNo arguments provided. If you wanted to run the cell types classifier in the current folder, use the following command:"
             )
             print("\npredict_cell_types .\n")
             print("Here is the full help message for the predict_cell_types command:\n")
         parser.print_help()
         sys.exit(0)
 
     args = parser.parse_args()
-    run_cell_types_classifier(**vars(args))
+    args = vars(args)
+    if args['units'] is not None:
+        args['units']=ale(args['units'][0])
+    run_cell_types_classifier(**args)
 
 
 def run_c4():
     main(c4=True)
 
 
 if __name__ == "__main__":
```

### Comparing `npyx-4.0.5/npyx/c4/run_baseline_classifier.py` & `npyx-4.0.6/npyx/c4/run_baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/run_deep_classifier.py` & `npyx-4.0.6/npyx/c4/run_deep_classifier.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/c4/waveform_augmentations.py` & `npyx-4.0.6/npyx/c4/waveform_augmentations.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/circuitProphyler.py` & `npyx-4.0.6/npyx/circuitProphyler.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/corr.py` & `npyx-4.0.6/npyx/corr.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/datasets.py` & `npyx-4.0.6/npyx/datasets.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/feat.py` & `npyx-4.0.6/npyx/feat.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/gl.py` & `npyx-4.0.6/npyx/gl.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/h5.py` & `npyx-4.0.6/npyx/h5.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/info.py` & `npyx-4.0.6/npyx/info.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/inout.py` & `npyx-4.0.6/npyx/inout.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
     assert dp.is_dir(), f"Provided path {dp} is a filename!"
 
     probe_versions = {
         'glx':{3.0:'3A', # option 3
                0.0:'1.0',
                21:'2.0_singleshank',
                24:'2.0_fourshanks',
-               1123:'ultra_high_density'},
+               1123:'ultra_high_density',
+               1030:'NHP_long_primate'},
         'oe':{"Neuropix-3a":'3A', # source_processor_name keys
                 "Neuropix-PXI":'1.0',
                 '?1':'2.0_singleshank', # do not know yet
                 '?2':'2.0_fourshanks'}, # do not know yet
         'int':{'3A':1, '1.0':1,
                '2.0_singleshank':2, '2.0_fourshanks':2,
                'ultra_high_density':3}
@@ -218,15 +219,15 @@
         else:
              glx_probe_version = 'N/A'
 
         if glx_probe_version in probe_versions['glx']:
             meta['probe_version'] = probe_versions['glx'][glx_probe_version]
             meta['probe_version_int'] = probe_versions['int'][meta['probe_version']]
         else:
-            print(f'WARNING probe version {glx_probe_version} not handled - post an issue at www.github.com/m-beau/NeuroPyxels')
+            print(f'WARNING probe version {glx_probe_version} not handled - post an issue at www.github.com/m-beau/NeuroPyxels and provide your .ap.meta file.')
             meta['probe_version'] = glx_probe_version
             meta['probe_version_int'] = 0
             
 
         # Based on probe version,
         # Find the voltage range, gain, encoding
         # and deduce the conversion from units/bit to uV
@@ -237,14 +238,16 @@
             ampFactor=ale(meta_glx["highpass"]['~imroTbl'][1].split(' ')[3]) # typically 500
             #if ampFactor!=500: print(f'\u001b[31mHeads-up, the voltage amplification factor seems to be {ampFactor}, which is not the default (500). Might be normal!')
         elif meta['probe_version'] in ['2.0_singleshank', '2.0_fourshanks']:
             if Vrange!=1e6:
                 print(f'\u001b[31mHeads-up, the voltage range seems to be {Vrange}, which is not the default (10^6). Might be normal!')
             bits_encoding=14
             ampFactor=80 # hardcoded
+        else:
+            raise ValueError(f"Probe version unhandled - bits_encoding unknown.")
         meta['bit_uV_conv_factor']=(Vrange/2**bits_encoding/ampFactor)
 
 
         # find everything else
         for filt_key in ['highpass','lowpass']:
             if filt_key not in meta_glx.keys(): continue
             meta[filt_key]={}
@@ -753,14 +756,108 @@
         rc = cp.asnumpy(rc)
 
     if save: # sync chan saved in extract_syncChan
         np.save(rcp, rc)
 
     return rc
 
+def extract_binary_channel_subset(directory_with_binary,
+                           chanmin,
+                           chanmax,
+                           batch_size_s=500,
+                           filt_suffix='ap'):
+    """Extract subset of channels from binary file into another binary file.
+
+    Saves the extracted subset of channels to another binary file in the same directory,
+    with the same name + the channel range appended to it.
+
+    Arguments:
+        - directory_with_binary: str, path to dataset (will find binary file in there)
+        - chanmin: minimum channel
+        - chanmax: end of channel range to extract, included
+        - batch_size_s: size of data batches loaded and saved, in seconds
+                        If memory error: decrease batch_size_s
+        - filt_suffix: str, 'ap' or 'lf', whether to extract channels from the ap or lfp binary.
+    """
+
+    ## Compute channels to export and define file names
+    binary_fn = get_binary_file_path(directory_with_binary, filt_suffix)
+    assert binary_fn != "not_found",\
+        f"Binary not found at {directory_with_binary}!"
+    target_fname = f'_chan{chanmin}-{chanmax}'.join([binary_fn.name.split(f'.{filt_suffix}.bin')[0], f'.{filt_suffix}.bin'])
+    target_fn = binary_fn.parent / target_fname
+    
+    ## Load binary metadata
+    meta = read_metadata(directory_with_binary)
+    filt_suffix_long = {'ap': 'highpass', 'lf': 'lowpass'}[filt_suffix]
+    fs = meta[filt_suffix_long]['sampling_rate']
+    dtype = np.dtype(meta[filt_suffix_long]['datatype'])
+    item_size = dtype.itemsize
+    Nchans = meta[filt_suffix_long]['n_channels_binaryfile']
+    assert (chanmin < Nchans - 1) & (chanmax < Nchans - 1)
+    
+    ## precompute binary batch time windows
+    filesize_bytes = os.path.getsize(binary_fn)
+    filesize_samples = filesize_bytes / Nchans / item_size
+    assert filesize_samples == int(filesize_samples),\
+        f"It doesn't seem like the binary file {binary_fn} holds a multiple of {Nchans} channels encoded as {item_size} bytes items...!"
+    filesize_samples = int(filesize_samples)
+    
+    batch_size_samples = int(batch_size_s * fs)
+    Nbatch = int(np.ceil(filesize_samples / batch_size_samples))
+    batch_windows = [[i * batch_size_samples,
+                      i * batch_size_samples + batch_size_samples]
+                     for i in range(Nbatch)]
+    batch_windows[-1][-1] = filesize_samples - 1
+
+    ## Run data extraction loop
+
+    # Memory-map binary data
+    memmap_f = np.memmap(binary_fn,
+                         dtype=dtype,
+                         offset=0,
+                         shape=(filesize_samples, Nchans),
+                         mode='r')
+    
+    with open(target_fn, 'wb') as fw:
+        for (t1, t2) in tqdm(batch_windows, desc="Extracting channels"):
+        
+            # Read binary data
+            rawData = memmap_f[t1:t2, chanmin:chanmax + 1]
+        
+            # Write binary data
+            rawData.tofile(fw)
+
+def read_custom_binary(fn, Nchans, dtype='int16'):
+    """
+    Returns a memory map of a neuropixels binary file with a custom number of channels.
+    
+    Arguments:
+    - fn: str, path to binary file
+    - Nchans: int, number of channels of binary file
+    - dtype: str, datatype of saved binary data (original neuropixels 1.0 data: int16)
+
+    Returns:
+    - memmap_f: memory mapped binary file of shape (n_samples, Nchans).
+                Index it as follow to extract data: memmap_f[time1:time2, channel1:channel2].
+                Sampling rate is typically 30_000 Hz, check with source binary file.
+    """
+    dtype = np.dtype(dtype)
+    item_size = dtype.itemsize
+    filesize_bytes = os.path.getsize(fn)
+    filesize_samples = int(filesize_bytes / Nchans / item_size)
+
+    memmap_f = np.memmap(fn,
+                     dtype=dtype,
+                     offset=0,
+                     shape=(filesize_samples, Nchans),
+                     mode='r')
+    
+    return memmap_f
+
 def assert_chan_in_dataset(dp, channels, ignore_ks_chanfilt=False):
     channels = np.array(channels)
     if ignore_ks_chanfilt:
         probe_version = read_metadata(dp)['probe_version']
         cm=chan_map(dp, probe_version=probe_version)
     else:
         cm=chan_map(dp, probe_version='local')
```

### Comparing `npyx-4.0.5/npyx/merger.py` & `npyx-4.0.6/npyx/merger.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/metrics.py` & `npyx-4.0.6/npyx/metrics.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/ml.py` & `npyx-4.0.6/npyx/ml.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/model.py` & `npyx-4.0.6/npyx/model.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/plot.py` & `npyx-4.0.6/npyx/plot.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/plot_utils.py` & `npyx-4.0.6/npyx/plot_utils.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/preprocess.py` & `npyx-4.0.6/npyx/preprocess.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/spk_t.py` & `npyx-4.0.6/npyx/spk_t.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/spk_wvf.py` & `npyx-4.0.6/npyx/spk_wvf.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/stats.py` & `npyx-4.0.6/npyx/stats.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/testing.py` & `npyx-4.0.6/npyx/testing.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx/utils.py` & `npyx-4.0.6/npyx/utils.py`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/npyx.egg-info/PKG-INFO` & `npyx-4.0.6/npyx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,20 @@
 Metadata-Version: 2.1
 Name: npyx
-Version: 4.0.5
+Version: 4.0.6
 Summary: Python routines dealing with Neuropixels data.
 Home-page: https://github.com/Npix-routines/NeuroPyxels
 Author: Maxime Beau
 Author-email: maximebeaujeanroch047@gmail.com
 Keywords: neuropixels,kilosort,phy,data analysis,electrophysiology,neuroscience
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: ipython
-Requires-Dist: numpy
-Requires-Dist: scipy==1.10.0
-Requires-Dist: pandas
-Requires-Dist: numba
-Requires-Dist: statsmodels
-Requires-Dist: matplotlib
-Requires-Dist: cmcrameri
-Requires-Dist: opencv-python
-Requires-Dist: scikit-learn
-Requires-Dist: imbalanced-learn
-Requires-Dist: networkx
-Requires-Dist: psutil
-Requires-Dist: joblib>=1.3
-Requires-Dist: tqdm
-Requires-Dist: h5py
-Requires-Dist: seaborn
 Provides-Extra: c4
-Requires-Dist: torch==1.13.1; extra == "c4"
-Requires-Dist: torchvision==0.14.1; extra == "c4"
-Requires-Dist: torchaudio==0.13.1; extra == "c4"
-Requires-Dist: laplace-torch; extra == "c4"
-Requires-Dist: requests; extra == "c4"
-Requires-Dist: dill; extra == "c4"
-Requires-Dist: tabulate; extra == "c4"
+License-File: LICENSE.md
 
 [![PyPI Version](https://img.shields.io/pypi/v/npyx.svg)](https://pypi.org/project/npyx/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5509733.svg)](https://doi.org/10.5281/zenodo.5509733)
 [![License](https://img.shields.io/pypi/l/npyx.svg)](https://github.com/m-beau/NeuroPyxels/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/npyx)](https://pepy.tech/project/npyx)
 # NeuroPyxels: loading, processing and plotting Neuropixels data in Python</h1> <img src="https://raw.githubusercontent.com/m-beau/NeuroPyxels/master/images/NeuroPyxels_logo_final.png" width="150" title="Neuropyxels" alt="Neuropixels" align="right" vspace = "50">
```

### Comparing `npyx-4.0.5/npyx.egg-info/SOURCES.txt` & `npyx-4.0.6/npyx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `npyx-4.0.5/setup.py` & `npyx-4.0.6/setup.py`

 * *Files identical despite different names*

