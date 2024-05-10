# Comparing `tmp/neurocaps-0.8.8.post5.tar.gz` & `tmp/neurocaps-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.8.8.post5.tar", last modified: Thu May  2 16:14:20 2024, max compression
+gzip compressed data, was "neurocaps-0.8.9.tar", last modified: Fri May 10 00:26:26 2024, max compression
```

## Comparing `neurocaps-0.8.8.post5.tar` & `neurocaps-0.8.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    11310 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2227 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2901 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6324 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2405 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       85 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    44374 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4697 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/analysis/merge.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    22479 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1001 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       94 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1240 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1864 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_TimeseriesExtractor.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_TimeseriesExtractor_additional.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_merge_dicts.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-10 00:25:35.000000 neurocaps-0.8.9/LICENSE.md
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14738 2024-05-10 00:26:26.000000 neurocaps-0.8.9/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    13847 2024-05-10 00:25:35.000000 neurocaps-0.8.9/README.md
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps/_utils/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_check_confound_names.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5249 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/analysis/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       85 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/analysis/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    50365 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/analysis/cap.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4697 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/analysis/merge.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/neurocaps/extraction/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/extraction/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29236 2024-05-10 00:25:35.000000 neurocaps-0.8.9/neurocaps/extraction/timeseriesextractor.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14738 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1001 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/SOURCES.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/dependency_links.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       94 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/requires.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-10 00:26:25.000000 neurocaps-0.8.9/neurocaps.egg-info/top_level.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1235 2024-05-10 00:25:35.000000 neurocaps-0.8.9/pyproject.toml
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-10 00:26:26.000000 neurocaps-0.8.9/setup.cfg
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-10 00:26:26.000000 neurocaps-0.8.9/tests/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_CAP.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_TimeseriesExtractor.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_TimeseriesExtractor_additional.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-10 00:25:36.000000 neurocaps-0.8.9/tests/test_merge_dicts.py
```

### Comparing `neurocaps-0.8.8.post5/LICENSE.md` & `neurocaps-0.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post5/PKG-INFO` & `neurocaps-0.8.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,178 +1,179 @@
-Metadata-Version: 2.1
-Name: neurocaps
-Version: 0.8.8.post5
-Summary: Co-activation patterns Python package
-Author-email: Donisha Smith <donishasmith@outlook.com>
-Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
-Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: seaborn
-Requires-Dist: kneed
-Requires-Dist: nilearn==0.10.2
-Requires-Dist: pybids; platform_system != "Windows"
-
-# neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
-
-**Still in beta but stable.**
-
-# Installation
-
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
-
-To install, using your preferred terminal:
-
-**Installation with pip:**
-
-```bash
-
-pip install neurocaps
-
-```
-
-**From source (Development version):**
-
-```bash
-pip install git+https://github.com/donishadsmith/neurocaps.git
-```
-
-or
-
-```bash
-
-git clone https://github.com/donishadsmith/neurocaps/
-cd neurocaps
-pip install -e .
-
-```
-
-# Usage
- **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
-
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas or the Automated Anatomical Labeling (AAL) atlas**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`.
-
-**Main features for `TimeseriesExtractor` includes:**
-
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
-
-**Main features for `CAP` includes:**
-
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
-
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
-
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
-
-Quick code example:
-
-```python
-
-from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
-"""If an asterisk '*' is after a name, all confounds starting with the 
-term preceding the parameter will be used. in this case, all parameters 
-starting with cosine will be used."""
-confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
-             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
-             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
-             "rot_z","rot_z_derivative1"]
-
-"""If use_confounds is True but no confound_names provided, there are hardcoded 
-confound names that will extract the data from the confound files outputted by fMRIPrep
-`n_acompcor_separate` will use the first 'n' components derived from the separate 
-white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
-combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-
-extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
-                                 confound_names=confounds, n_acompcor_separate=6)
-
-bids_dir = "/path/to/bids/dir"
-
-# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
-pipeline_name = "fmriprep-1.4.0"
-
-# Resting State
-# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
-
-# Task; use parallel processing with `n_cores`
-extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
-                   pipeline_name=pipeline_name, n_cores=10)
-
-cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
-                    n_clusters=6)
-
-cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
-                      standardize = True)
-
-# Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="networks", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
-
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
-                            subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
-
-# Get CAP metrics
-outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
-                                         return_df=True, output_dir=output_dir,
-                                         metrics=["temporal fraction", "persistence"],
-                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
-
-print(outputs["temporal fraction"])
-
-```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
-**DataFrame Output:**
-| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
-| --- | --- | --- | --- | --- | --- | --- | --- | --- |
-| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
-| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
-| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
-| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
-| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
-| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
-| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
-| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
-| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
-| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
-
-# Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder ot conform with the naming conventions of modern fmriprep outputs.
-
-# References
-[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
-
-[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
-
-[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
-
-[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
+# neurocaps
+This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+
+**Still in beta but stable.**
+
+# Installation
+
+**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+
+To install, using your preferred terminal:
+
+**Installation with pip:**
+
+```bash
+
+pip install neurocaps
+
+```
+
+**From source (Development version):**
+
+```bash
+pip install git+https://github.com/donishadsmith/neurocaps.git
+```
+
+or
+
+```bash
+
+git clone https://github.com/donishadsmith/neurocaps/
+cd neurocaps
+pip install -e .
+
+```
+
+# Usage
+**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+Custom Key Structure:
+- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+        
+Example 
+The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+```Python
+parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+ ```
+
+**Main features for `TimeseriesExtractor` includes:**
+
+- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
+- Saving the nested dictionary containing timeseries as a pickle file.
+- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
+- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+
+**Main features for `CAP` includes:**
+
+- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
+- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
+different CAPs across the entire run.
+
+**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+
+Quick code example:
+
+```python
+
+from neurocaps.extraction import TimeseriesExtractor
+from neurocaps.analysis import CAP
+
+"""If an asterisk '*' is after a name, all confounds starting with the 
+term preceding the parameter will be used. in this case, all parameters 
+starting with cosine will be used."""
+confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
+             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
+             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
+             "rot_z","rot_z_derivative1"]
+
+"""If use_confounds is True but no confound_names provided, there are hardcoded 
+confound names that will extract the data from the confound files outputted by fMRIPrep
+`n_acompcor_separate` will use the first 'n' components derived from the separate 
+white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
+combined mask, list them in the `confound_names` parameter"""
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+
+extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
+                                 confound_names=confounds, n_acompcor_separate=6)
+
+bids_dir = "/path/to/bids/dir"
+
+# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
+pipeline_name = "fmriprep-1.4.0"
+
+# Resting State
+# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
+
+# Task; use parallel processing with `n_cores`
+extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
+                   pipeline_name=pipeline_name, n_cores=10)
+
+cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
+                    n_clusters=6)
+
+cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
+                      standardize = True)
+
+# Visualize CAPs
+cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            subplots=True)
+
+cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            subplots=True, xlabel_rotation=90, tight_layout=False, 
+                            hspace = 0.4)
+
+# Get CAP metrics
+outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
+                                         return_df=True, output_dir=output_dir,
+                                         metrics=["temporal fraction", "persistence"],
+                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
+
+print(outputs["temporal fraction"])
+
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+**DataFrame Output:**
+| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
+| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
+| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
+| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
+| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
+| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
+| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
+| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
+| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
+| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
+
+# Testing 
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+
+
+# References
+[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
+
+[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
+
+[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
+
+[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
+
+[^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
+
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.8.8.post5/README.md` & `neurocaps-0.8.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,206 @@
-# neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
-
-**Still in beta but stable.**
-
-# Installation
-
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
-
-To install, using your preferred terminal:
-
-**Installation with pip:**
-
-```bash
-
-pip install neurocaps
-
-```
-
-**From source (Development version):**
-
-```bash
-pip install git+https://github.com/donishadsmith/neurocaps.git
-```
-
-or
-
-```bash
-
-git clone https://github.com/donishadsmith/neurocaps/
-cd neurocaps
-pip install -e .
-
-```
-
-# Usage
- **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
-
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas or the Automated Anatomical Labeling (AAL) atlas**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`.
-
-**Main features for `TimeseriesExtractor` includes:**
-
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
-
-**Main features for `CAP` includes:**
-
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
-
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
-
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
-
-Quick code example:
-
-```python
-
-from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
-"""If an asterisk '*' is after a name, all confounds starting with the 
-term preceding the parameter will be used. in this case, all parameters 
-starting with cosine will be used."""
-confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
-             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
-             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
-             "rot_z","rot_z_derivative1"]
-
-"""If use_confounds is True but no confound_names provided, there are hardcoded 
-confound names that will extract the data from the confound files outputted by fMRIPrep
-`n_acompcor_separate` will use the first 'n' components derived from the separate 
-white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
-combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-
-extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
-                                 confound_names=confounds, n_acompcor_separate=6)
-
-bids_dir = "/path/to/bids/dir"
-
-# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
-pipeline_name = "fmriprep-1.4.0"
-
-# Resting State
-# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
-
-# Task; use parallel processing with `n_cores`
-extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
-                   pipeline_name=pipeline_name, n_cores=10)
-
-cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
-                    n_clusters=6)
-
-cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
-                      standardize = True)
-
-# Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="networks", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
-
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
-                            subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
-
-# Get CAP metrics
-outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
-                                         return_df=True, output_dir=output_dir,
-                                         metrics=["temporal fraction", "persistence"],
-                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
-
-print(outputs["temporal fraction"])
-
-```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
-**DataFrame Output:**
-| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
-| --- | --- | --- | --- | --- | --- | --- | --- | --- |
-| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
-| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
-| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
-| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
-| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
-| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
-| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
-| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
-| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
-| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
-
-# Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder ot conform with the naming conventions of modern fmriprep outputs.
-
-# References
-[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
-
-[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
-
-[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
-
-[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
+Metadata-Version: 2.1
+Name: neurocaps
+Version: 0.8.9
+Summary: Co-activation patterns Python package
+Author-email: Donisha Smith <donishasmith@outlook.com>
+Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: kneed
+Requires-Dist: nilearn==0.10.2
+Requires-Dist: pybids; platform_system != "Windows"
+
+# neurocaps
+This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+
+**Still in beta but stable.**
+
+# Installation
+
+**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+
+To install, using your preferred terminal:
+
+**Installation with pip:**
+
+```bash
+
+pip install neurocaps
+
+```
+
+**From source (Development version):**
+
+```bash
+pip install git+https://github.com/donishadsmith/neurocaps.git
+```
+
+or
+
+```bash
+
+git clone https://github.com/donishadsmith/neurocaps/
+cd neurocaps
+pip install -e .
+
+```
+
+# Usage
+**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+Custom Key Structure:
+- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+        
+Example 
+The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+```Python
+parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+ ```
+
+**Main features for `TimeseriesExtractor` includes:**
+
+- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
+- Saving the nested dictionary containing timeseries as a pickle file.
+- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
+- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+
+**Main features for `CAP` includes:**
+
+- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
+- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
+different CAPs across the entire run.
+
+**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+
+Quick code example:
+
+```python
+
+from neurocaps.extraction import TimeseriesExtractor
+from neurocaps.analysis import CAP
+
+"""If an asterisk '*' is after a name, all confounds starting with the 
+term preceding the parameter will be used. in this case, all parameters 
+starting with cosine will be used."""
+confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
+             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
+             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
+             "rot_z","rot_z_derivative1"]
+
+"""If use_confounds is True but no confound_names provided, there are hardcoded 
+confound names that will extract the data from the confound files outputted by fMRIPrep
+`n_acompcor_separate` will use the first 'n' components derived from the separate 
+white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
+combined mask, list them in the `confound_names` parameter"""
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+
+extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
+                                 confound_names=confounds, n_acompcor_separate=6)
+
+bids_dir = "/path/to/bids/dir"
+
+# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
+pipeline_name = "fmriprep-1.4.0"
+
+# Resting State
+# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
+
+# Task; use parallel processing with `n_cores`
+extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
+                   pipeline_name=pipeline_name, n_cores=10)
+
+cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
+                    n_clusters=6)
+
+cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
+                      standardize = True)
+
+# Visualize CAPs
+cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            subplots=True)
+
+cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            subplots=True, xlabel_rotation=90, tight_layout=False, 
+                            hspace = 0.4)
+
+# Get CAP metrics
+outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
+                                         return_df=True, output_dir=output_dir,
+                                         metrics=["temporal fraction", "persistence"],
+                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
+
+print(outputs["temporal fraction"])
+
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+**DataFrame Output:**
+| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
+| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
+| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
+| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
+| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
+| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
+| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
+| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
+| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
+| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
+
+# Testing 
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+
+
+# References
+[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
+
+[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
+
+[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
+
+[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
+
+[^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
+
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.8.9/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from .._timeseriesextractor_internals._check_parcel_approach import _check_parcel_approach
+
 # A class which is responsible for accessing all CAPMetadata and to keep track of all attributes in CAP
 class _CAPGetter:
     def __init__(self):
         pass
     
     ### Attributes exist when CAP initialized
     @property
@@ -16,14 +18,18 @@
     def groups(self):
         return self._groups
     
     @property
     def parcel_approach(self):
         return self._parcel_approach
     
+    @parcel_approach.setter
+    def parcel_approach(self, parcel_dict):
+        self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_dict, call="setter")
+    
     ### Attributes exist when CAP.get_caps() used
     @property
     def runs(self):
         if hasattr(self, "_runs"): return self._runs
         else: return None
 
     @property
@@ -48,16 +54,16 @@
 
     @property
     def optimal_n_clusters(self):
         if hasattr(self, "_optimal_n_clusters"): return self._optimal_n_clusters
         else: return None
     
     @property
-    def network_caps(self):
-        if hasattr(self, "_network_caps"): return self._network_caps
+    def region_caps(self):
+        if hasattr(self, "_region_caps"): return self._region_caps
         else: return None
 
     @property
     def outer_product(self):
         if hasattr(self, "_outer_product"): return self._outer_product
         else: return None
```

### Comparing `neurocaps-0.8.8.post5/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.8.9/neurocaps/_utils/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,18 @@
     for run in run_list:
 
         run_id = "run-1" if run == None else run
         run = run if run != None else ""
 
         # Get files from specific run
         nifti_file = [nifti_file for nifti_file in nifti_files if run in nifti_file.split("/")[-1]]
-        mask_file = [mask_file for mask_file in mask_files if run in mask_file.split("/")[-1]]
+        if len(mask_files) != 0:
+            mask_file = [mask_file for mask_file in mask_files if run in mask_file.split("/")[-1]]
+        else:
+            mask_file = []
         confound_file = [confound_file for confound_file in confound_files if run in confound_file.split("/")[-1]] if signal_clean_info["use_confounds"] else None
         confound_metadata_file = [confound_metadata_file for confound_metadata_file in confound_metadata_files if run in confound_metadata_file.split("/")[-1]] if signal_clean_info["use_confounds"] and signal_clean_info["n_acompcor_separate"] else None
 
         if verbose: print(f"Running subject: {subj_id}; run: {run_id}; \n {nifti_file}", flush=flush_print)
 
         confound_df = pd.read_csv(confound_file[0], sep="\t") if signal_clean_info["use_confounds"] else None
 
@@ -52,56 +55,89 @@
                 else: invalid_confounds.extend([confound_name])
 
             if len(invalid_confounds) > 0: 
                 if verbose: print(f"Subject {subj_id} did not have the following confounds: {invalid_confounds}", flush=flush_print)
 
             confounds = confound_df[valid_confounds]
             confounds = confounds.fillna(0)
+
+            if signal_clean_info["fd_threshold"]: 
+                censor = True
+                if "framewise_displacement" in confound_df.columns:
+                    fd_array = confound_df["framewise_displacement"].fillna(0).values
+                else:
+                    censor = False
+                    warnings.warn(f"For subject {subj_id}, `fd_threshold` specified but 'framewise_displacement' is not a column in the confound dataframe so removal of volumes after nuisance regression will not be done.")
+            else:
+                censor = False
+
             if verbose: print(f"Confounds used for subject: {subj_id}; run: {run_id} - {confounds.columns}", flush=flush_print)
 
         # Create the masker for extracting time series
-        masker = NiftiLabelsMasker(
-            mask_img=mask_file[0],
-            labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
-            labels=parcel_approach[list(parcel_approach.keys())[0]]["labels"], 
-            resampling_target='data',
-            standardize=signal_clean_info["standardize"],
-            detrend=signal_clean_info["detrend"],
-            low_pass=signal_clean_info["low_pass"],
-            high_pass=signal_clean_info["high_pass"],
-            t_r=tr
-        )
+        if len(mask_file) !=0:
+            masker = NiftiLabelsMasker(
+                mask_img=mask_file[0],
+                labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
+                resampling_target='data',
+                standardize=signal_clean_info["standardize"],
+                detrend=signal_clean_info["detrend"],
+                low_pass=signal_clean_info["low_pass"],
+                high_pass=signal_clean_info["high_pass"],
+                t_r=tr
+            )
+        else:
+            masker = NiftiLabelsMasker(
+                labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
+                resampling_target='data',
+                standardize=signal_clean_info["standardize"],
+                detrend=signal_clean_info["detrend"],
+                low_pass=signal_clean_info["low_pass"],
+                high_pass=signal_clean_info["high_pass"],
+                t_r=tr
+            )
         # Load and discard volumes if needed
         nifti_img = load_img(nifti_file[0])
         if signal_clean_info["dummy_scans"]: 
             nifti_img = index_img(nifti_img, slice(signal_clean_info["dummy_scans"], None))
-            if signal_clean_info["use_confounds"]: confounds.drop(list(range(0,signal_clean_info["dummy_scans"])),axis=0,inplace=True)
+            if signal_clean_info["use_confounds"]: 
+                confounds.drop(list(range(0,signal_clean_info["dummy_scans"])),axis=0,inplace=True)
+                # Truncate the fd_array also
+                if censor:
+                    fd_array = fd_array[signal_clean_info["dummy_scans"]:]
             offset = signal_clean_info["dummy_scans"] 
 
         # Extract timeseries
         timeseries = masker.fit_transform(nifti_img, confounds=confounds) if signal_clean_info["use_confounds"] else masker.fit_transform(nifti_img)
 
+        if censor:
+            censor_volumes = list(np.where(fd_array > signal_clean_info["fd_threshold"])[0])
+
         if event_file:
             event_df = pd.read_csv(event_file[0], sep=None)
             # Get specific timing information for specific condition
             condition_df = event_df[event_df["trial_type"] == condition] 
 
             # Empty list for scans
             scan_list = []
 
             # Convert times into scan numbers to obtain the scans taken when the participant was exposed to the condition of interest; include partial scans
             for i in condition_df.index:
                 onset_scan, duration_scan = int(condition_df.loc[i,"onset"]/tr), math.ceil((condition_df.loc[i,"onset"] + condition_df.loc[i,"duration"])/tr)
                 if signal_clean_info["dummy_scans"]:
                     scan_list.extend([scan - offset for scan in range(onset_scan, duration_scan + 1) if scan not in range(0, signal_clean_info["dummy_scans"])])
                 else:
-                    scan_list.extend(range(onset_scan, duration_scan + 1))
+                    scan_list.extend(list(range(onset_scan, duration_scan + 1)))
+                if censor:
+                    scan_list = [volume for volume in scan_list if volume not in censor_volumes]
 
             # Timeseries with the extracted scans corresponding to condition; set is used to remove overlapping TRs    
             timeseries = timeseries[sorted(list(set(scan_list))),:]
+        else:
+            if censor:
+                timeseries = np.delete(timeseries, censor_volumes, axis=0)
 
         if timeseries.shape[0] == 0:
             warnings.warn(f"Subject {subj_id} timeseries is empty for {run}. Most likely due to condition not existing or TRs correspoonding to the condition being removed by `dummy_scans`.")
         else:
             subject_timeseries[subj_id].update({run_id: timeseries})
     
     if len(subject_timeseries[subj_id].keys()) == 0:
```

### Comparing `neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.8.9/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from ._check_parcel_approach import _check_parcel_approach
 # A class which is responsible for acessing all TimeseriesExtractorGetter and to keep track of all attributes in TimeSeriesExtractor
 class _TimeseriesExtractorGetter:
     def __init__(self):
         pass
     
     #### Exists upon initialization of TimeseriesExtractor
     @property
@@ -13,14 +14,18 @@
     def signal_clean_info(self):
         return self._signal_clean_info
     
     @property
     def parcel_approach(self):
         return self._parcel_approach
     
+    @parcel_approach.setter
+    def parcel_approach(self, parcel_dict):
+        self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_dict, call="setter")
+
     ### Does not exists upon initialization of Timeseries Extractor
 
     # Exist when TimeSeriesExtractor.get_bold() used
     @property
     def task_info(self):
         if hasattr(self, "_task_info"): return self._task_info
         else: return None
@@ -41,15 +46,15 @@
     @property
     def subject_timeseries(self):
         if hasattr(self, "_subject_timeseries"): return self._subject_timeseries
         else: return None
     
     @subject_timeseries.setter
     def subject_timeseries(self, subject_dict):
-        error_message = "Must be a nested dictionary where the first level is the subject id, second level is the run number in the form of 'run-#', and the final level is the timeseris as a numpy array"
+        error_message = "Must be a nested dictionary where the first level is the subject id, second level is the run number in the form of 'run-#', and the final level is the timeseris as a numpy array."
         if isinstance(subject_dict, dict): 
             first_level_indx = list(subject_dict.keys())[0]
             if isinstance(subject_dict[first_level_indx], dict) and len(subject_dict[first_level_indx].keys()) != 0 and "run" in list(subject_dict[first_level_indx].keys())[0]: 
                 run = list(subject_dict[first_level_indx].keys())[0]
                 if isinstance(subject_dict[first_level_indx][run],np.ndarray): 
                     self._subject_timeseries = subject_dict
                 else: raise TypeError(error_message)
```

### Comparing `neurocaps-0.8.8.post5/neurocaps/analysis/cap.py` & `neurocaps-0.8.9/neurocaps/analysis/cap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 from sklearn.cluster import KMeans
 from kneed import KneeLocator
-from .._utils import _CAPGetter, _convert_pickle_to_dict
+from .._utils import _CAPGetter, _convert_pickle_to_dict, _check_parcel_approach
 import numpy as np, re, warnings
 
 class CAP(_CAPGetter):
     def __init__(self, parcel_approach: dict[dict], n_clusters: Union[int, list[int]]=5, cluster_selection_method: str=None, groups: dict=None):
         """
         Initialize the CAP (Co-activation Patterns) analysis class.
 
@@ -60,16 +60,15 @@
             for group_name in self._groups.keys():
                 assert len(self._groups[group_name]) > 0, f"{group_name} has zero subject ids."
             
             # Convert ids to strings
             for group in self._groups.keys():
                 self._groups[group] = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in self._groups[group]]
         
-        valid_parcel_dict = {"Schaefer": {"n_rois" : 400, "yeo_networks": 7},
-                         "AAL": {"version": "SPM12"}}
+        valid_parcel_dict = {"Schaefer", "AAL", "Custom"}
 
         if len(parcel_approach.keys()) > 1:
             raise ValueError(f"Only one parcellation approach can be selected from the following valid options: {valid_parcel_dict.keys()}.\n Example format of `parcel_approach`: {valid_parcel_dict}")
         
         self._parcel_approach = parcel_approach 
 
     def get_caps(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], runs: Union[int, list[int]]=None, random_state: int=None, show_figs: bool=True, standardize: bool=True, epsilon: Union[int,float]=0, **kwargs) -> None:
@@ -222,65 +221,94 @@
         for group in self._groups:
             for subj_id in self._groups[group]:
                 if subj_id in self._subject_table.keys():
                     warnings.warn(f"Subject: {subj_id} appears more than once, only including the first instance of this subject in the analysis.") 
                 else:
                     self._subject_table.update({subj_id : group})
 
-    def visualize_caps(self, output_dir: str=None, plot_options: Union[str, list[str]]="outer product", visual_scope: list[str]="networks", task_title: str=None, show_figs: bool=True, subplots: bool=False, **kwargs):
+    def visualize_caps(self, output_dir: str=None, plot_options: Union[str, list[str]]="outer product", visual_scope: list[str]="regions", task_title: str=None, show_figs: bool=True, subplots: bool=False, **kwargs):
         """ Plotting CAPs
 
         This function produces seaborn heatmaps for each CAP. If groups were given when the CAP class was initialized, plotting will be done for all CAPs for all groups.
 
         Parameters
         ----------
         output_dir: str, default=None
             Directory to save plots in. If None, plots will not be saved.
         plot_options: str or list[str], default="outer product"
             Type of plots to create. Options are "outer product" or "heatmap".
-        visual_scope: str or list[str], default="networks
-            Determines whether plotting is done at the network level or node level. For network level, the value of each nodes in the same networks are averaged together them plotted.
+        visual_scope: str or list[str], default="regions"
+            Determines whether plotting is done at the region level or node level. 
+            For region level, the value of each nodes in the same regions are averaged together them plotted.
+            Options are "regions" or "nodes".
         task_title: str, default=None
             Serves as the title of each plot as well as the name of the saved file if output_dir is given.
         show_figs: bool, default=True
             Display figures or not to display figures.
         subplots: bool, default=True
             Produce subplots for outer product plots.
         kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include "dpi", "format", "figsize", "fontsize", "hspace", "wspace", "xticklabels_size", "yticklabels_size", "shrink", "nrow", "ncol", "suptitle_fontsize", "tight_layout", "rect", "sharey", "xlabel_rotation", "ylabel_rotation", "annot". 
             If `output_dir` is not None and no inputs for dpi and format are given, dpi defaults to 300 and format defaults to "png". If no keywords, "figsize" defaults to (8,6), "fontsize", which adjusts the title size of the individual plots or subplots, defaults to 14, "hspace", which adjusts spacing for subplots, defaults to 0.4, 
             "wspace", which adjusts spacing between subplots, defaults to 0.4, "xticklabels_size" defaults to 8, "yticklabels_size" defaults to 8, shrink, which adjusts the cbar size, defaults to 0.8, "nrow", which is the number of rows for subplot and varies, and "ncol", which is the number of columns for subplot, default varies but max is 5, "suptitle_fontsize", 
             size of the main title when subplot is True, defaults to 0.7, "tight_layout", use tight layout for subplot, defaults to True, "rect", input for the `rect` parameter in tight layout when subplots is True to fix whitespace issues, default is [0, 0.03, 1, 0.95], "sharey", which shares y axis labela for subplots, defaults to True, 
-            "xlabel_rotation", which rotates the labels on the x-axis, defaults to 0, "ylabel_rotation", which rotates the labels on the y-axis, defaults to 0, "annot", which adds values to cells on the outer product heatmap at the network level only, defaults to False .
+            "xlabel_rotation", which rotates the labels on the x-axis, defaults to 0, "ylabel_rotation", which rotates the labels on the y-axis, defaults to 0, "annot", which adds values to cells on the outer product heatmap at the region level only, defaults to False, "linewidths", which specifies the padding between each cell, defaults to 0,
+            and "cmap", which specifies the color pattern of the cells in the plot, defaults to "coolwarm".
     
+         Notes
+        -----
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+        Custom Key Structure:
+        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
+        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+          Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
+        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
+        
+        Example 
+        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
         """
         import os, itertools
 
+        # Check parcel approach
+
+        # Check if parcellation_approach is custom
+        if "Custom" in self.parcel_approach.keys() and ("nodes" not in self.parcel_approach["Custom"].keys() or "regions" not in self.parcel_approach["Custom"].keys()):
+            _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_caps")
+
         # Check labels
         check_caps = self._caps[list(self._caps.keys())[0]]
         check_caps = check_caps[list(check_caps.keys())[0]]
-        if check_caps.shape[0] != len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]): 
-                raise ValueError("Number of rois/labels used for CAPs does not equal the number of rois/labels specified in `parcel_approach`.")
+        if check_caps.shape[0] != len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]): 
+                raise ValueError("Number of rois/nodes used for CAPs does not equal the number of rois/nodes specified in `parcel_approach`.")
 
         if output_dir:
             if not os.path.exists(output_dir):
                 os.makedirs(output_dir)
 
         # Convert to list
         if type(plot_options) == str: plot_options = [plot_options]
         if type(visual_scope) == str: visual_scope = [visual_scope]
 
         # Check inputs for plot_options and visual_scope
         if not any(["heatmap" in plot_options, "outer product" in plot_options]):
             raise ValueError("Valid inputs for `plot_options` are 'heatmap' and 'outer product'.")
         
-        if not any(["networks" in visual_scope, "nodes" in visual_scope]):
-            raise ValueError("Valid inputs for `visual_scope` are 'networks' and 'nodes'.")
+        if not any(["regions" in visual_scope, "nodes" in visual_scope]):
+            raise ValueError("Valid inputs for `visual_scope` are 'regions' and 'nodes'.")
 
-        if "networks" in visual_scope: self._create_networks()
+        if "regions" in visual_scope: self._create_regions()
 
         # Create plot dictionary
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
                         format = kwargs["format"] if kwargs and "format" in kwargs.keys() else "png",
                         figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (8,6),
                         fontsize = kwargs["fontsize"] if kwargs and "fontsize" in kwargs.keys() else 14,
                         hspace = kwargs["hspace"] if kwargs and "hspace" in kwargs.keys() else 0.2,
@@ -293,14 +321,16 @@
                         suptitle_fontsize = kwargs["suptitle_fontsize"] if kwargs and "suptitle_fontsize" in kwargs.keys() else 20,
                         tight_layout = kwargs["tight_layout"] if kwargs and "tight_layout" in kwargs.keys() else True,
                         rect = kwargs["rect"] if kwargs and "rect" in kwargs.keys() else [0, 0.03, 1, 0.95],
                         sharey = kwargs["sharey"] if kwargs and "sharey" in kwargs.keys() else True,
                         xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
                         ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
                         annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
+                        linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
+                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
                         )
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
@@ -310,35 +340,54 @@
         # Initialize outer product attribute
         if "outer product" in plot_options: self._outer_product = {}
 
         distributed_list = list(itertools.product(plot_options,visual_scope,self._groups.keys()))
 
         for plot_option, scope, group in distributed_list:
                 # Get correct labels depending on scope
-                if scope == "networks": cap_dict, columns = self._network_caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["networks"]
-                elif scope == "nodes": cap_dict, columns = self._caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]
+                if scope == "regions": 
+                    if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
+                        cap_dict, columns = self._region_caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]
+                    elif list(self._parcel_approach.keys())[0] == "Custom":
+                        cap_dict, columns = self._region_caps, list(self._parcel_approach["Custom"]["regions"].keys())
+                elif scope == "nodes": 
+                    if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
+                        cap_dict, columns = self._caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]
+                    elif list(self._parcel_approach.keys())[0] == "Custom":
+                        cap_dict, columns = self._caps , [x[0] + " " + x[1] for x in list(itertools.product(["LH", "RH"],self._parcel_approach["Custom"]["regions"].keys()))]
 
                 #  Generate plot for each group
                 if plot_option == "outer product": self._generate_outer_product_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns, subplots=subplots,
                                                                                     output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
                 elif plot_option == "heatmap": self._generate_heatmap_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns,
                                                                             output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
             
-    def _create_networks(self):
-        self._network_caps = {group: {} for group in self._groups.keys()}
+    def _create_regions(self):
+        self._region_caps = {group: {} for group in self._groups.keys()}
         for group in self._groups.keys():
             for cap in self._caps[group].keys():
-                network_caps = {}
-                for network in self._parcel_approach[list(self._parcel_approach.keys())[0]]["networks"]:
-                    if len(network_caps) == 0:
-                        network_caps = np.array([np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]) if network in node])])])
-                    else:
-                        network_caps = np.hstack([network_caps, np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]) if network in node])])])
-            
-                self._network_caps[group].update({cap: network_caps})
+                region_caps = {}
+                if list(self._parcel_approach.keys())[0] != "Custom":
+                    for region in self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]:
+                        if len(region_caps) == 0:
+                            region_caps = np.array([np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in node])])])
+                        else:
+                            region_caps = np.hstack([region_caps, np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in node])])])
+                else:
+                    region_dict = self._parcel_approach["Custom"]["regions"]
+                    region_keys = region_dict.keys()
+                    for region in region_keys:
+                        roi_indxs = np.array(region_dict[region]["lh"] + region_dict[region]["rh"])
+
+                        if len(region_caps) == 0:
+                            region_caps= np.array([np.average(self._caps[group][cap][roi_indxs])])
+                        else:
+                            region_caps= np.hstack([region_caps, np.average(self._caps[group][cap][roi_indxs])])
+
+                self._region_caps[group].update({cap: region_caps})
     
     def _generate_outer_product_plots(self, group, plot_dict, cap_dict, columns, subplots, output_dir, task_title, show_figs, scope):
         from seaborn import heatmap
         import matplotlib.pyplot as plt, os
 
         # Nested dictionary for group
         self._outer_product[group] = {}
@@ -363,41 +412,52 @@
             # Current subplot
             axes_x, axes_y = [0,0] 
 
         # Iterate over CAPs
         for cap in cap_dict[group].keys():
             # Calculate outer product
             self._outer_product[group].update({cap: np.outer(cap_dict[group][cap],cap_dict[group][cap])})
+            # Create labels if nodes requested for scope
+            if scope == "nodes":
+                import collections
+                
+                # Get frequency of each major hemisphere and region in Schaefer, AAL, or Custom atlas
+                if list(self._parcel_approach.keys())[0] == "Schaefer":
+                    frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
+                elif list(self._parcel_approach.keys())[0] == "AAL":
+                    frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
+                elif list(self._parcel_approach.keys())[0] == "Custom":
+                    frequency_dict = {}
+                    for id in columns:
+                        hemisphere_id = "LH" if id.startswith("LH ") else "RH"
+                        region_id = re.split("LH |RH ", id)[-1]
+                        frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
+                # Get the names, which indicate the hemisphere and region
+                names_list = list(frequency_dict.keys())
+                # Create label list the same length as the labels dictionary and substitute each element with an empty string
+                labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
+
+                starting_value = 0
+
+                # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
+                for num, name in enumerate(names_list): 
+                    if num == 0:
+                        labels[0] = name
+                    else:
+                        # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
+                        starting_value += frequency_dict[names_list[num-1]] 
+                        labels[starting_value] = name
+
             if subplots: 
                 ax = axes[axes_y] if nrow == 1 else axes[axes_x,axes_y]
                 # Modify tick labels based on scope
-                if scope == "networks":
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap="coolwarm", xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"])
+                if scope == "regions":
+                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"])
                 else:
-                    # Create Labels
-                    import collections
-                    
-                    if list(self._parcel_approach.keys())[0] == "Schaefer":
-                        frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]]]))
-                    elif list(self._parcel_approach.keys())[0] == "AAL":
-                        frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]])
-                    names_list = list(frequency_dict.keys())
-                    labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]))]
-
-                    shift = 0
-
-                    for num, name in enumerate(names_list):
-                        if num == 0:
-                            labels[0] = name
-                        else:
-                            shift += frequency_dict[names_list[num-1]] 
-                            indx = (frequency_dict[names_list[num]]) + shift - frequency_dict[names_list[num]]
-                            labels[indx] = name
-
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap="coolwarm", cbar_kws={"shrink": plot_dict["shrink"]})
+                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={"shrink": plot_dict["shrink"]})
 
                     ticks = [i for i, label in enumerate(labels) if label]  
 
                     ax.set_xticks(ticks)  
                     ax.set_xticklabels([label for label in labels if label]) 
                     ax.set_yticks(ticks)  
                     ax.set_yticklabels([label for label in labels if label]) 
@@ -421,86 +481,101 @@
                     axes_y += 1
 
             else:
                 # Create new plot for each iteration when not subplot
                 plt.figure(figsize=plot_dict["figsize"])
 
                 plot_title = f"{group} {cap} {task_title}" if task_title else f"{group} {cap}"
-                if scope == "networks": display = heatmap(self._outer_product[group][cap], cmap="coolwarm", xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]})
-                else: display = heatmap(self._outer_product[group][cap], cmap="coolwarm", xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]})
+                if scope == "regions": display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]})
+                else: 
+                    display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]})
+                    ticks = [i for i, label in enumerate(labels) if label]  
+
+                    display.set_xticks(ticks)  
+                    display.set_xticklabels([label for label in labels if label]) 
+                    display.set_yticks(ticks)  
+                    display.set_yticklabels([label for label in labels if label]) 
                 
                 # Set title
                 display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
                 # Modify label sizes
                 display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
                 display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
                 # Save individual plots
                 if output_dir:
                     partial_filename = f"{group}_{cap}_{task_title}" if task_title else f"{group}_{cap}"
-                    full_filename = f"{partial_filename}_outer_product_heatmap-networks.{plot_dict['format']}" if scope == "networks" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
+                    full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
                     display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
         
         # Remove subplots with no data
         if subplots: [fig.delaxes(ax) for ax in axes.flatten() if not ax.has_data()]
 
         # Save subplot
         if subplots and output_dir: 
             partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_outer_product_heatmap-networks.{plot_dict['format']}" if scope == "networks" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
+            full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
         
         # Display figures
         if not show_figs: plt.close()
 
     def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, task_title, show_figs, scope):
         from seaborn import heatmap
         import matplotlib.pyplot as plt, pandas as pd, os
         
         # Initialize new grid
         plt.figure(figsize=plot_dict["figsize"])
 
-        if scope == "networks": display = heatmap(pd.DataFrame(cap_dict[group], index=columns), cmap='coolwarm', cbar_kws={'shrink': plot_dict["shrink"]}) 
+        if scope == "regions": 
+            display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]}) 
         else: 
             # Create Labels
             import collections
             if list(self._parcel_approach.keys())[0] == "Schaefer":
-                frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]]]))
+                frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
             elif list(self._parcel_approach.keys())[0] == "AAL":
-                frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]])
+                frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
+            elif list(self._parcel_approach.keys())[0] == "Custom":
+                    frequency_dict = {}
+                    for id in columns:
+                        hemisphere_id = "LH" if id.startswith("LH ") else "RH"
+                        region_id = re.split("LH |RH ", id)[-1]
+                        frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
             names_list = list(frequency_dict.keys())
-            labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]))]
+            labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
 
-            shift = 0
+            starting_value = 0
 
-            for num, name in enumerate(names_list):
+            # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
+            for num, name in enumerate(names_list): 
                 if num == 0:
                     labels[0] = name
                 else:
-                    shift += frequency_dict[names_list[num-1]] 
-                    indx = (frequency_dict[names_list[num]]) + shift - frequency_dict[names_list[num]]
-                    labels[indx] = name
+                    # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
+                    starting_value += frequency_dict[names_list[num-1]] 
+                    labels[starting_value] = name
 
-            display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), cmap='coolwarm', cbar_kws={'shrink': plot_dict["shrink"]})
+            display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]})
 
             plt.yticks(ticks=[pos for pos, label in enumerate(labels) if label], labels=names_list)  
 
         # Modify label sizes
         display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
         display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
         # Set plot name
         plot_title = f"{group} CAPS {task_title}" if task_title else f"{group} CAPS" 
         display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
         # Save plots
         if output_dir:
             partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_heatmap-networks.{plot_dict['format']}" if scope == "networks" else f"{partial_filename}_heatmap-nodes.{plot_dict['format']}"
+            full_filename = f"{partial_filename}_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_heatmap-nodes.{plot_dict['format']}"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
    
         # Display figures
         if not show_figs: plt.close()
 
     def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, metrics: Union[str, list[str]]=["temporal fraction", "persistence", "counts", "transition frequency"], return_df: bool=True, output_dir: str=None, file_name: str=None) -> dict:
         """Get CAP metrics
```

### Comparing `neurocaps-0.8.8.post5/neurocaps/analysis/merge.py` & `neurocaps-0.8.9/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post5/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.8.9/neurocaps/extraction/timeseriesextractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union
 from .._utils import _TimeseriesExtractorGetter, _check_confound_names, _check_parcel_approach, _extract_timeseries
 import re, os, warnings, json, sys
 
 class TimeseriesExtractor(_TimeseriesExtractorGetter):
     def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=False , low_pass: float=None, high_pass: float=None, 
-                 parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7}}, use_confounds: bool=True, confound_names: list[str]=None, n_acompcor_separate: int=None, dummy_scans: int=None):
+                 parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7}}, use_confounds: bool=True, confound_names: list[str]=None, fd_threshold: float=None,
+                 n_acompcor_separate: int=None, dummy_scans: int=None):
         """Timeseries Extractor Class
         
         Initializes a TimeseriesExtractor to prepare for Co-activation Patterns (CAPs) analysis.
 
         Parameters
         ----------
         space : str, default="MNI152NLin2009cAsym"
@@ -21,77 +22,109 @@
             Signals above cutoff frequency will be filtered out.
         high_pass : float, default=None
             Signals below cutoff frequency will be filtered out.
         parcel_approach : dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7}}
             Approach to use to parcellate bold images. Should be in the form of a nested dictionary where the first key is the atlas.
             Currently only "Schaefer" and "AAL" is supported. For the sub-dictionary for "Schaefer", available options includes "n_rois" and "yeo_networks".
             Please refer to the documentation for Nilearn's `datasets.fetch_atlas_schaefer_2018` for valid inputs. For the subdictionary for "AAL" only "version"
-            is an option. Please refer to the documentation for Nilearn's `datasets.fetch_atlas_aal` for valid inputs.
+            is an option. Please refer to the documentation for Nilearn's `datasets.fetch_atlas_aal` for valid inputs. As of version 0.8.9, you can replace "Schaefer"
+            and "AAL" with "Custom". At minimum, if "Custom" is specified, a subkey, called "maps" specifying the directory location of the parcellation as a Nifti (e.g .nii or .nii.gz)
+            - {"Custom": {"maps": "/location/to/parcellation.nii.gz"}}.
         use_confounds : bool, default=True
             To use confounds when extracting timeseries.
         confound_names : List[str], default=None
             Names of confounds to use in confound files. If None, default confounds are used.
+        fd_threshold : float, default=None
+            Threshold criteria to remove volume after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
+            in the confounds dataframe and `use_confounds` must be true. Additionally, 'framewise_displacemnt' does not need to be specified in the `confound_names` for this to work.
         n_acompcor_separate : int, default = None
             The number of seperate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
             then the first five components derived from the WM mask and the first five components derived from the CSF mask will be used, resulting in ten acompcor components being
             used. If this parameter is not none any acompcor components listed in the confound names will be disregarded in order to locate the first 'n' components derived from the 
             masks. To use the acompcor components derived from the combined masks (WM & CSF) leave this parameter as 'None' and list the specific acompcors of interest in the 
             `confound_names` parameter.
         dummy_scans : float, default=None
-            Remove the first `n` number of volumes before extracting timeseries.
+            Removes the first `n` number of volumes before extracting timeseries.
         
-
-        Notes
-        -----
+        Notes for `confounds_names`
+        --------------------------
         For the `confound_names` parameter, an asterisk ("*") can be used to find the name of confounds that starts with the term preceding the asterisk.
         For instance, "cosine*" will find all confound names in the confound files starting with "cosine".
+
+        Notes for `parcel_approach`
+        ---------------------------
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+        Custom Key Structure:
+        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+        - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+          Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
+          For timeseries extraction, this key is not required.
+        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+        
+        Example 
+        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
         """
         self._space = space
         self._signal_clean_info = {"standardize": standardize, "detrend": detrend, "low_pass": low_pass, "high_pass": high_pass, 
-                                   "dummy_scans": dummy_scans, "use_confounds": use_confounds,  "n_acompcor_separate": n_acompcor_separate}   
+                                   "dummy_scans": dummy_scans, "use_confounds": use_confounds,  "n_acompcor_separate": n_acompcor_separate,
+                                   "fd_threshold": None}   
 
         # Check parcel_apprach
         self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_approach)
 
         if self._signal_clean_info["use_confounds"]:
             self._signal_clean_info["confound_names"] = _check_confound_names(high_pass=high_pass, specified_confound_names=confound_names, n_acompcor_separate=n_acompcor_separate)
-            
-    def get_bold(self, bids_dir: str, session: Union[int,str]=None, runs: list[int]=None, task: str="rest", condition: str=None, tr: Union[int, float]=None, 
-                 run_subjects: list[str]=None, exclude_subjects: list[str]= None, pipeline_name: str=None, n_cores: Union[bool, int]=None, verbose: bool=True, flush_print: bool=False) -> None: 
+            self._signal_clean_info["fd_threshold"] = fd_threshold
+
+    def get_bold(self, bids_dir: str, task: str, session: Union[int,str]=None, runs: list[int]=None, condition: str=None, tr: Union[int, float]=None, 
+                 run_subjects: list[str]=None, exclude_subjects: list[str]= None, pipeline_name: str=None, n_cores: Union[bool, int]=None, verbose: bool=True, flush_print: bool=False,
+                 exclude_niftis: list[str]=None) -> None: 
         """Get Bold Data
 
         Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
 
         Parameters
         ----------
         bids_dir : str
             Path to a BIDS compliant directory. 
+        task : str, default="rest"
+            Task name.
         session : int, default=None
             Session to extract timeseries from. Only a single session can be extracted at a time. 
         runs : list[int], default=None
             Run number to extract timeseries data from. Extracts all runs if unspecified.
-        task : str, default="rest"
-            Task name.
         condition : str, default=None
             Specific condition in the task to extract from. Only a single condition can be extracted at a time.
         tr : int or float, default=None
             Repetition time.
-        run_subjects : List[str], default=None
+        run_subjects : list[str], default=None
             List of subject IDs to process. Processes all subjects if None.
-        exclude_subjects : List[str], default=None
+        exclude_subjects : list[str], default=None
             List of subject IDs to exclude.  
         pipeline_name: str, default=None
             The name of the pipeline folder in the derivatives folder containing the preprocessed data. If None, BIDSLayout will use the name of dset_dir with derivatives=True. This parameter
             should be used if their are multiple pipelines in the derivatives folder.
         n_cores: bool or int, default=None
             The number of CPU cores to use for multiprocessing. If true, all available cores will be used.
         verbose: bool, default=True
             Print subject specific information such as confounds being extracted and id and run of subject being processed during timeseries extraction.
         flush_print: bool, default=False
             Flush the printed subject specific infomation produced during the timeseries extraction process.
+        exclude_niftis: list[str], default=None
+            Exclude certain preprocessed nifti files to prevent the timeseries of that file from being extracted. Used if there are specific runs across differnt participants that need to be
+            excluded.
         """
         import bids, multiprocessing
 
         if sys.platform == "win32":
             raise SystemError("Cannot use this method on Windows devices since it relies on the `pybids` module which is only compatable with POSIX systems.")
 
         # Update attributes
@@ -116,22 +149,22 @@
             subj_id_list = sorted([subj_id for subj_id in subj_id_list if subj_id not in exclude_subjects])
 
         if run_subjects: 
             run_subjects = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in run_subjects]
             subj_id_list = sorted([subj_id for subj_id in subj_id_list if subj_id in run_subjects])
 
         # Setup extraction
-        self._setup_extraction(layout=layout, subj_id_list=subj_id_list)
+        self._setup_extraction(layout=layout, subj_id_list=subj_id_list, exclude_niftis=exclude_niftis)
 
         if n_cores:
             if n_cores == True:
                 self._n_cores = multiprocessing.cpu_count()
             else:
                 if n_cores > multiprocessing.cpu_count():
-                    raise ValueError(f"More cores specified than available - Number of cores specified: {n_cores}; Max cores available: {multiprocessing.cpu_count()}")
+                    raise ValueError(f"More cores specified than available - Number of cores specified: {n_cores}; Max cores available: {multiprocessing.cpu_count()}.")
                 else:
                     self._n_cores = n_cores
             
             # Generate list of tuples for each subject
             args_list = [(subj_id, self._subject_info[subj_id]["nifti_files"],self._subject_info[subj_id]["mask_files"],self._subject_info[subj_id]["event_files"],
                           self._subject_info[subj_id]["confound_files"], self._subject_info[subj_id]["confound_metadata_files"], self._subject_info[subj_id]["run_list"],
                           self._subject_info[subj_id]["tr"], condition, self._parcel_approach, self._signal_clean_info, verbose, flush_print
@@ -158,15 +191,15 @@
                                                        tr=self._subject_info[subj_id]["tr"], condition=condition, parcel_approach=self._parcel_approach, signal_clean_info=self._signal_clean_info,
                                                        verbose=verbose, flush_print=flush_print)
             
                 # Aggregate new timeseries
                 if isinstance(subject_timeseries, dict): self._subject_timeseries.update(subject_timeseries)
         
     # Get valid subjects to iterate through
-    def _setup_extraction(self, layout, subj_id_list):
+    def _setup_extraction(self, layout, subj_id_list, exclude_niftis):
        for subj_id in subj_id_list:
             if self._task_info["session"]:
                 nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"],extension = "nii.gz", subject=subj_id))
                 bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "json", subject=subj_id))
                 event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
                 confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject=subj_id))
                 confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "json", subject=subj_id))
@@ -174,37 +207,44 @@
             else:
                 nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
                 bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "json", subject=subj_id))
                 event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
                 confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "tsv", subject=subj_id))
                 confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "json", subject=subj_id))
                 mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
+            
+            # Remove excluded file from the nifti_files list, which will prevent it from being processed
+            if exclude_niftis and len(nifti_files) != 0:
+                nifti_files = [nifti_file for nifti_file in nifti_files if os.path.basename(nifti_file) not in exclude_niftis]
 
             # Generate a list of runs to iterate through based on runs in nifti_files
             if self._task_info["runs"]:
                 check_runs = [f"run-{run}" for run in self._task_info["runs"]] 
             elif len(nifti_files) != 0:
-                if "run-" in nifti_files[0].split("/")[-1]:
-                    check_runs = [re.search("run-(\\S+?)[-_]",x.split("/")[-1])[0][:-1] for x in nifti_files]
+                if "run-" in os.path.basename(nifti_files[0]):
+                    check_runs = [re.search("run-(\\S+?)[-_]",os.path.basename(x))[0][:-1] for x in nifti_files]
                 else:
                    check_runs = [] 
             else:
                 check_runs = []
 
             # Generate a list of runs to iterate through based on runs in nifti_files
             if not self._task_info["session"] and len(nifti_files) != 0:
-                if "ses-" in nifti_files[0].split("/")[-1]:
-                    check_sessions = [re.search("ses-(\\S+?)[-_]",x.split("/")[-1])[0][:-1] for x in nifti_files]
+                if "ses-" in os.path.basename(nifti_files[0]):
+                    check_sessions = [re.search("ses-(\\S+?)[-_]",os.path.basename(x))[0][:-1] for x in nifti_files]
                     if len(list(set(check_sessions))) > 1:
-                        raise ValueError(f"`session` not specified but subject {subj_id} has more than one session : {sorted(list(set(check_sessions)))}. In order to continue timeseries extraction, the specific session to extract must be specified")
+                        raise ValueError(f"`session` not specified but subject {subj_id} has more than one session : {sorted(list(set(check_sessions)))}. In order to continue timeseries extraction, the specific session to extract must be specified.")
 
-            if len(nifti_files) == 0 or len(mask_files) == 0:
-                warnings.warn(f"Skipping subject: {subj_id} due to missing nifti or mask files.")
+            if len(nifti_files) == 0:
+                warnings.warn(f"Skipping subject: {subj_id} due to missing nifti files.")
                 continue
-
+            
+            if len(mask_files) == 0:
+                warnings.warn(f"Subject: {subj_id} is missing mask file but timeseries extraction will continue.")
+                
             if self._signal_clean_info["use_confounds"]:
                 if len(confound_files) == 0:
                     warnings.warn(f"Skipping subject: {subj_id} due to missing confound files.")
                     continue
                 if len(confound_metadata_files) == 0 and self._signal_clean_info["n_acompcor_separate"]:
                     warnings.warn(f"Skipping subject: {subj_id} due to missing confound metadata to locate the first six components of the white-matter and cerobrospinal fluid masks seperately.")
                     continue
@@ -220,25 +260,25 @@
                     curr_list = []
                     # Assess is any of these returns True
                     curr_list.append(any([run in file for file in nifti_files]))
                     if self._task_info["condition"]: curr_list.append(any([run in file for file in event_files]))
                     if self._signal_clean_info["use_confounds"]:
                         curr_list.append(any([run in file for file in confound_files]))
                         if self._signal_clean_info["n_acompcor_separate"]: curr_list.append(any([run in file for file in confound_metadata_files]))
-                    curr_list.append(any([run in file for file in mask_files]))
+                    if len(mask_files) != 0: curr_list.append(any([run in file for file in mask_files]))
                     # Append runs that contain all needed files
                     if all(curr_list): run_list.append(run)
                 
                 # Skip subject if no run has all needed files present
                 if len(run_list) != len(check_runs) or len(run_list) == 0:
                     if len(run_list) == 0:
                         if self._task_info["condition"]: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, confound tsv file, confound json file being from the same run.")
                         else: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, event file, confound tsv file, confound json file being from the same run.")
                         continue
-                    else: warnings.warn(f"Subject: {subj_id} only has the following runs available: {', '.join(run_list)}")
+                    else: warnings.warn(f"Subject: {subj_id} only has the following runs available: {', '.join(run_list)}.")
             else:
                 run_list = [None]
             # Add subject list to subject attribute. These are subjects that will be ran
             self._subject_ids.append(subj_id)
 
             # Get repetition time for the subject
             tr = self._task_info["tr"] if self._task_info["tr"] else json.load(open(bold_metadata_files[0]))["RepetitionTime"]
@@ -265,86 +305,127 @@
         if output_dir:
             if not os.path.exists(output_dir):
                 os.makedirs(output_dir)
         
         with open(os.path.join(output_dir,file_name + ".pkl"), "wb") as f:
             pickle.dump(self._subject_timeseries,f)
 
-    def visualize_bold(self, subj_id: Union[int,str], run: int, roi_indx: Union[int, list[int]]=None, network: str=None, show_figs: bool=True, output_dir: str=None, file_name: str=None, **kwargs):
+    def visualize_bold(self, subj_id: Union[int,str], run: int, roi_indx: Union[int, list[int]]=None, region: str=None, show_figs: bool=True, output_dir: str=None, file_name: str=None, **kwargs):
         """Plot Bold Data
 
         Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
 
         Parameters
         ----------
         subj_id: str
             Subject ID, as a string, to plot.
         run: int
             The run to plot.
         roi_indx: int or list[int], default=None
             The indices of the Schaefer nodes to plot. See self.node_indices for valid node names and indices.
-        network: str, default=None
-            The Schaefer network to plot. If not None, all nodes in the specified Schaefer network will be averaged then plotted. See self.atlas_networks for valid network names.
+        region: str, default=None
+            The region of the parcellation to plot. If not None, all nodes in the specified region will be averaged then plotted. See `regions` in self.parcel_approach 
+            for valid regions names.
         show_figs: bool, defaults=True
             Whether to show figires or not to show figures
         output_dir : str
             Directory to save the file to.
         file_name : str
             Name of the file with the extension to signify the file type.
         kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include "dpi" and "figsize". If output_dir is not None and no inputs for dpi and format are given,
             dpi defaults to 300. If "figsize" has no input, figure sizes defaults to (8,6).
 
         Raises
         ------
         ValueError
-            If both `roi_indx` and `network` are specified.
+            If both `roi_indx` and `region` are specified.
         AssertionError
             If `file_name` does not contain an extension to signify the file type.
+
+        Notes
+        -----
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+        Custom Key Structure:
+        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
+        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+          Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
+        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
+        
+        Example 
+        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
         """
     
         import matplotlib.pyplot as plt, numpy as np
 
         if isinstance(subj_id,int): subj_id = str(subj_id)
 
-        if roi_indx !=None and network != None:
-            raise ValueError("`roi_indx` and network can not be used simultaneously.")
+        if roi_indx !=None and region != None:
+            raise ValueError("`roi_indx` and `region` can not be used simultaneously.")
         
         if output_dir:
             if not os.path.exists(output_dir):
                 os.makedirs(output_dir)
             assert "." in file_name, "`file_name` must be specified if `output_dir` is specified and it must contain an extension to signify the file type."
 
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
-                         figsize= kwargs["figsize"] if kwargs and "figsize" in kwargs.keys else (15, 5))
+                         figsize= kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (15, 5))
+        
+        if kwargs:
+            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
+            if len(invalid_kwargs.keys()) > 0:
+                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
         # Obtain the column indices associated with the rois; add logic for roi_indx == 0 since it would be recognized as False
         if roi_indx or roi_indx == 0:
             if type(roi_indx) == int:
                 plot_indxs = roi_indx
             
             elif type(roi_indx) == str:
-                plot_indxs = self._parcel_approach[self._parcel_approach.keys[0]]["labels"].index(roi_indx)
+                # Check if parcellation_approach is custom
+                if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
+                    _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
+                plot_indxs = self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(roi_indx)
             
             elif type(roi_indx) == list:
-                if type(roi_indx[0]) == int:
+                if all([isinstance(indx,int) for indx in roi_indx]):
                     plot_indxs = np.array(roi_indx)
-                elif type(roi_indx[0]) == str:
-                    plot_indxs = np.array([self._parcel_approach[self._parcel_approach.keys[0]]["labels"].index(index) for index in roi_indx])
-        
-        elif network:
-            plot_indxs = np.array([index for index, label in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["labels"]) if network in label])
+                elif all([isinstance(indx,str) for indx in roi_indx]):
+                    # Check if parcellation_approach is custom
+                    if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
+                        _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
+                    plot_indxs = np.array([self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(index) for index in roi_indx])
+                else:
+                    raise ValueError("All elements in `roi_indx` need to be all strings or all integers.")
+                
+        elif region:
+            if "Custom" in self.parcel_approach.keys():
+                if "regions" not in self.parcel_approach["Custom"].keys():
+                    _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
+                else:
+                    plot_indxs =  np.array(self.parcel_approach["Custom"]["regions"][region]["lh"] + self.parcel_approach["Custom"]["regions"][region]["rh"])
+            else:
+                plot_indxs = np.array([index for index, label in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in label])
         
         plt.figure(figsize=plot_dict["figsize"])
 
         if roi_indx or roi_indx == 0: 
             plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs])
-        elif network:  
+        elif region:  
             plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), np.mean(self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs], axis=1))
-            plt.title(network)
+            plt.title(region)
         plt.xlabel("TR")
 
         if output_dir:
             plt.savefig(os.path.join(output_dir,file_name), dpi=plot_dict["dpi"])
 
         if show_figs == False:
             plt.close()
```

### Comparing `neurocaps-0.8.8.post5/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.8.9/neurocaps.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.8.8.post5
+Version: 0.8.9
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -57,17 +57,38 @@
 git clone https://github.com/donishadsmith/neurocaps/
 cd neurocaps
 pip install -e .
 
 ```
 
 # Usage
- **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas or the Automated Anatomical Labeling (AAL) atlas**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`.
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+Custom Key Structure:
+- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+        
+Example 
+The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+```Python
+parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+ ```
 
 **Main features for `TimeseriesExtractor` includes:**
 
 - Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
 - Saving the nested dictionary containing timeseries as a pickle file.
 - Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
 - Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
@@ -125,15 +146,15 @@
 cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
                     n_clusters=6)
 
 cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
                       standardize = True)
 
 # Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="networks", plot_options="outer product", 
+cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3, sharey=True, 
                             subplots=True)
 
 cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4)
@@ -162,17 +183,24 @@
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder ot conform with the naming conventions of modern fmriprep outputs.
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+
 
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
 [^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
 [^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
 
 [^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
+
+[^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
+
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.8.8.post5/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.8.9/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post5/pyproject.toml` & `neurocaps-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurocaps"
-version = "0.8.8post5"
+version = "0.8.9"
 authors = [{name = "Donisha Smith", email = "donishasmith@outlook.com"}]
 description = "Co-activation patterns Python package"
 readme = "README.md"
 requires-python = ">=3.9.0"
 keywords = ["python", "Co-Activation Patterns", "CAPs", "neuroimaging", "fmri", "dfc", "dynamic functional connectivity", "fMRIPrep"]
 classifiers = [
     "Intended Audience :: Education",
```

### Comparing `neurocaps-0.8.8.post5/tests/test_CAP.py` & `neurocaps-0.8.9/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post5/tests/test_TimeseriesExtractor.py` & `neurocaps-0.8.9/tests/test_TimeseriesExtractor_additional.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,13 @@
 import os, pytest
 from neurocaps.extraction import TimeseriesExtractor
 
-def test_TimeseriesExtractor_no_parallel():
-    dir = os.path.dirname(__file__)
-
-    confounds=["Cosine*", "aComp*", "Rot*"]
-
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
-                                    confound_names=confounds)
+# Changing file name in github actions to test different file naming configurations
 
-    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
-
-    pipeline_name = "fmriprep_1.0.0/fmriprep"
-    extractor.get_bold(bids_dir=bids_dir, session='002', task="rest", pipeline_name=pipeline_name, tr=1.2)
-    
-    print(extractor.subject_timeseries, flush=True)
-
-    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 100
-    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
-
-def test_TimeseriesExtractor_no_parallel_no_session():
+def test_TimeseriesExtractor_no_parallel_additional():
     dir = os.path.dirname(__file__)
 
     confounds=["Cosine*", "aComp*", "Rot*"]
 
     parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
 
     extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
@@ -36,10 +17,9 @@
     bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
 
     pipeline_name = "fmriprep_1.0.0/fmriprep"
     extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
     
     print(extractor.subject_timeseries, flush=True)
 
-    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 100
-    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
-
+    assert extractor.subject_timeseries["01"]["run-1"].shape[-1] == 100
+    assert extractor.subject_timeseries["01"]["run-1"].shape[0] == 40
```

### Comparing `neurocaps-0.8.8.post5/tests/test_merge_dicts.py` & `neurocaps-0.8.9/tests/test_merge_dicts.py`

 * *Files identical despite different names*

