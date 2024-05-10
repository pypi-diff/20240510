# Comparing `tmp/masscube-0.0.8.tar.gz` & `tmp/masscube-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masscube-0.0.8.tar", last modified: Mon Apr 22 21:50:04 2024, max compression
+gzip compressed data, was "masscube-0.0.9.tar", last modified: Tue Apr 23 18:26:52 2024, max compression
```

## Comparing `masscube-0.0.8.tar` & `masscube-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.188064 masscube-0.0.8/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.8/LICENSE
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-22 21:50:04.187880 masscube-0.0.8/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.8/README.md
--rw-r--r--   0 jiemoniu   (501) staff       (20)      962 2024-04-22 21:49:49.000000 masscube-0.0.8/pyproject.toml
--rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-04-22 21:50:04.188097 masscube-0.0.8/setup.cfg
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.183512 masscube-0.0.8/src/
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.186805 masscube-0.0.8/src/masscube/
--rw-r--r--   0 jiemoniu   (501) staff       (20)      124 2024-03-20 21:39:26.000000 masscube-0.0.8/src/masscube/__init__.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    17856 2024-04-22 20:04:50.000000 masscube-0.0.8/src/masscube/alignment.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    15266 2024-04-02 00:57:05.000000 masscube-0.0.8/src/masscube/annotation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2820 2024-04-17 22:13:13.000000 masscube-0.0.8/src/masscube/feature_evaluation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     8772 2024-04-03 20:16:56.000000 masscube-0.0.8/src/masscube/feature_grouping.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.8/src/masscube/feature_table_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.8/src/masscube/network.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     4075 2024-04-18 05:25:59.000000 masscube-0.0.8/src/masscube/normalization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    12247 2024-04-22 20:19:43.000000 masscube-0.0.8/src/masscube/params.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    10980 2024-04-19 09:37:18.000000 masscube-0.0.8/src/masscube/peak_detect.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    30273 2024-04-17 21:14:22.000000 masscube-0.0.8/src/masscube/raw_data_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     5479 2024-04-11 22:19:50.000000 masscube-0.0.8/src/masscube/stats.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.8/src/masscube/utils_functions.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    12826 2024-04-17 21:34:57.000000 masscube-0.0.8/src/masscube/visualization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    13228 2024-04-22 20:22:02.000000 masscube-0.0.8/src/masscube/workflows.py
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-22 21:50:04.187651 masscube-0.0.8/src/masscube.egg-info/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/SOURCES.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/dependency_links.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      141 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/entry_points.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      129 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/requires.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-04-22 21:50:04.000000 masscube-0.0.8/src/masscube.egg-info/top_level.txt
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-23 18:26:52.376619 masscube-0.0.9/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.9/LICENSE
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-23 18:26:52.376402 masscube-0.0.9/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.9/README.md
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      962 2024-04-23 18:26:42.000000 masscube-0.0.9/pyproject.toml
+-rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-04-23 18:26:52.376654 masscube-0.0.9/setup.cfg
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-23 18:26:52.372383 masscube-0.0.9/src/
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-23 18:26:52.375065 masscube-0.0.9/src/masscube/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      160 2024-04-22 22:01:20.000000 masscube-0.0.9/src/masscube/__init__.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    17852 2024-04-23 17:55:36.000000 masscube-0.0.9/src/masscube/alignment.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    15266 2024-04-02 00:57:05.000000 masscube-0.0.9/src/masscube/annotation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2820 2024-04-17 22:13:13.000000 masscube-0.0.9/src/masscube/feature_evaluation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     8877 2024-04-23 00:20:17.000000 masscube-0.0.9/src/masscube/feature_grouping.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.9/src/masscube/feature_table_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.9/src/masscube/network.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     4080 2024-04-23 00:57:30.000000 masscube-0.0.9/src/masscube/normalization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    12248 2024-04-23 17:57:24.000000 masscube-0.0.9/src/masscube/params.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    11004 2024-04-22 23:35:50.000000 masscube-0.0.9/src/masscube/peak_detect.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    30273 2024-04-17 21:14:22.000000 masscube-0.0.9/src/masscube/raw_data_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     5489 2024-04-23 17:55:13.000000 masscube-0.0.9/src/masscube/stats.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.9/src/masscube/utils_functions.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    12826 2024-04-17 21:34:57.000000 masscube-0.0.9/src/masscube/visualization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    13266 2024-04-23 18:25:26.000000 masscube-0.0.9/src/masscube/workflows.py
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-23 18:26:52.376123 masscube-0.0.9/src/masscube.egg-info/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-23 18:26:52.000000 masscube-0.0.9/src/masscube.egg-info/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-04-23 18:26:52.000000 masscube-0.0.9/src/masscube.egg-info/SOURCES.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-04-23 18:26:52.000000 masscube-0.0.9/src/masscube.egg-info/dependency_links.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      141 2024-04-23 18:26:52.000000 masscube-0.0.9/src/masscube.egg-info/entry_points.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      129 2024-04-23 18:26:52.000000 masscube-0.0.9/src/masscube.egg-info/requires.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-04-23 18:26:52.000000 masscube-0.0.9/src/masscube.egg-info/top_level.txt
```

### Comparing `masscube-0.0.8/LICENSE` & `masscube-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/PKG-INFO` & `masscube-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.8
+Version: 0.0.9
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `masscube-0.0.8/README.md` & `masscube-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/pyproject.toml` & `masscube-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masscube"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Accurate and fast data processing for metabolomics"
```

### Comparing `masscube-0.0.8/src/masscube/alignment.py` & `masscube-0.0.9/src/masscube/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,24 +48,24 @@
         # check if the file exists
         if not os.path.exists(txt_file_names[i]):
             problematic_files.append(file_name)
             continue
         
         # read feature table
         current_table = pd.read_csv(txt_file_names[i], low_memory=False, sep="\t")
-        current_table = current_table[current_table["MS2"].notna()|(current_table["peak_height"] > parameters.int_tol*3)]
+        current_table = current_table[current_table["MS2"].notna()|(current_table["length"] > 5)]
         # sort current table by peak height from high to low
         current_table = current_table.sort_values(by="peak_height", ascending=False)
         current_table.index = range(len(current_table))
         new_feature_idx = []
 
-        mz_seq = np.array(feature_table["m/z"], dtype=float)
-        rt_seq = np.array(feature_table["RT"], dtype=float)
-        mz_to_be_matched = np.array(current_table["m/z"], dtype=float)
-        rt_to_be_matched = np.array(current_table["RT"], dtype=float)
+        mz_seq = np.array(feature_table["m/z"], dtype=np.float64)
+        rt_seq = np.array(feature_table["RT"], dtype=np.float64)
+        mz_to_be_matched = np.array(current_table["m/z"], dtype=np.float64)
+        rt_to_be_matched = np.array(current_table["RT"], dtype=np.float64)
         labeled_v = np.ones(len(feature_table), dtype=bool)
         
         # compare the m/z and RT of the features
         for j in range(len(current_table)):
             v = np.logical_and(np.abs(mz_seq - mz_to_be_matched[j]) < mz_tol, np.abs(rt_seq - rt_to_be_matched[j]) < rt_tol)
             # check if the feature is already in the aligned feature table using tolerance
             # including parameters.align_mz_tol and parameters.align_rt_tol
```

### Comparing `masscube-0.0.8/src/masscube/annotation.py` & `masscube-0.0.9/src/masscube/annotation.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/src/masscube/feature_evaluation.py` & `masscube-0.0.9/src/masscube/feature_evaluation.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/src/masscube/feature_grouping.py` & `masscube-0.0.9/src/masscube/feature_grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
     """
 
     # sort ROI by m/z from high to low
     d.rois.sort(key=lambda x: x.mz)
 
     roi_to_label = np.ones(len(d.rois), dtype=bool)
 
-    # isotopes can't be parent or child
+    # isotopes or rois with length < 4 can't be parent or child
     for idx, r in enumerate(d.rois):
-        if r.is_isotope:
+        if r.is_isotope or len(r.scan_idx_seq) < 4:
             roi_to_label[idx] = False
     
     # find in-source fragments
     for idx in range(len(d.rois)-1, -1, -1):
 
         r = d.rois[idx]
 
@@ -134,17 +134,17 @@
     d: MSData object
         An MSData object that contains the detected rois to be grouped.
     """
 
     d.rois.sort(key=lambda x: x.mz)
     roi_to_label = np.ones(len(d.rois), dtype=bool)
 
-    # isotopes and in-source fragments cannot be the parent
+    # isotopes, in-source fragments, and rois with length < 4 can't be parent or child
     for idx, r in enumerate(d.rois):
-        if r.is_isotope or r.is_in_source_fragment:
+        if r.is_isotope or r.is_in_source_fragment or len(r.scan_idx_seq) < 4:
             roi_to_label[idx] = False
 
     if d.params.ion_mode.lower() == "positive":
         default_adduct = "[M+H]+"
         adduct_mass_diffence = _ADDUCT_MASS_DIFFERENCE_POS_AGAINST_H
         adduct_mass_diffence['[2M+H]+'] = r.mz - 1.007276
         adduct_mass_diffence['[3M+H]+'] = 2*(r.mz - 1.007276)
```

### Comparing `masscube-0.0.8/src/masscube/feature_table_utils.py` & `masscube-0.0.9/src/masscube/feature_table_utils.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/src/masscube/network.py` & `masscube-0.0.9/src/masscube/network.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/src/masscube/normalization.py` & `masscube-0.0.9/src/masscube/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     v : numpy array
         The normalization factor.
     """
 
     # change all zeros to ones
     v[v == 0] = 1
 
-    return np.array(array / v, dtype=int)
+    return np.array(array / v, dtype=np.int64)
 
 
 def find_reference_sample(array, method='number'):
     """
     A function to find the reference sample for normalization.
     Note, samples are in columns and features are in rows.
```

### Comparing `masscube-0.0.8/src/masscube/params.py` & `masscube-0.0.9/src/masscube/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.rt_range = [0.0, 1000.0]       # RT range in minutes, list of two floats
         self.ion_mode = "positive"          # Ionization mode, "positive" or "negative", character string
 
         # Feature detection
         self.mz_tol_ms1 = 0.01              # m/z tolerance for MS1, default is 0.01
         self.mz_tol_ms2 = 0.015             # m/z tolerance for MS2, default is 0.015
         self.int_tol = 30000                # Intensity tolerance, default is 30000 for Orbitrap and 1000 for other instruments, integer
-        self.roi_gap = 10                   # Gap within a feature, default is 10 (i.e. 10 consecutive scans without signal), integer
+        self.roi_gap = 20                   # Gap within a feature, default is 10 (i.e. 10 consecutive scans without signal), integer
         self.min_ion_num = 10               # Minimum scan number a feature, default is 10, integer
 
         # Parameters for feature alignment
         self.align_mz_tol = 0.01            # m/z tolerance for MS1, default is 0.01
         self.align_rt_tol = 0.2             # RT tolerance, default is 0.2
 
         # Parameters for feature annotation
@@ -176,15 +176,15 @@
             if "qc" in sample_groups_pre:
                 sample_groups = ["qc"] + sample_groups
             if "blank" in sample_groups_pre:
                 sample_groups = sample_groups + ["blank"]
 
             sample_table_new = pd.DataFrame(columns=sample_table.columns)
             for i in range(len(sample_groups)):
-                sample_table_new = pd.concat([sample_table_new, sample_table[sample_table.iloc[:, 1].str.contains(sample_groups[i])]])
+                sample_table_new = pd.concat([sample_table_new, sample_table[sample_table.iloc[:, 1].str.lower() == sample_groups[i]]])
             self.sample_names = list(sample_table_new.iloc[:, 0])
             self.sample_groups = sample_groups
             self.individual_sample_groups = []
             for name in self.sample_names:
                 self.individual_sample_groups.append(sample_table_new[sample_table_new.iloc[:, 0] == name].iloc[0, 1])
 
         # STEP 6: set output
```

### Comparing `masscube-0.0.8/src/masscube/peak_detect.py` & `masscube-0.0.9/src/masscube/peak_detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,17 +92,17 @@
 
 def cut_roi(r, int_tol=1000):
     """
     Function to cut an ROI by providing the start and end positions.
     """
 
     r.int_seq = np.array(r.int_seq)
-    # r.noise_level = calculate_noise_level(r.int_seq)
+    r.noise_level = calculate_noise_level(r.int_seq)
 
-    if  len(r.int_seq) < 10 or r.peak_height < 3*int_tol or np.max(r.int_seq)/np.mean(r.int_seq) < 3:
+    if  len(r.int_seq) < 10 or r.peak_height < 3*int_tol or (np.max(r.int_seq)/np.mean(r.int_seq) < 3 and r.noise_level > 0.5):
         return [r]
 
     ss = gaussian_filter1d(r.int_seq, sigma=1.5)
     peaks, _ = find_peaks(ss, prominence=np.max(ss)*0.05, distance=5)
 
     peaks = peaks[r.int_seq[peaks] > 2*int_tol]
```

### Comparing `masscube-0.0.8/src/masscube/raw_data_utils.py` & `masscube-0.0.9/src/masscube/raw_data_utils.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/src/masscube/stats.py` & `masscube-0.0.9/src/masscube/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     Returns
     -------
     feature_table : pandas DataFrame
     """
     
     v = [params.sample_names[i] for i in range(len(params.individual_sample_groups)) if params.individual_sample_groups[i] not in ['qc', 'blank']]
-    data_array = np.array(feature_table[v], dtype=int)
+    data_array = np.array(feature_table[v], dtype=np.int64)
 
     s = len(params.sample_groups) - 2
     v = np.array([i for i in params.individual_sample_groups if i not in ['qc', 'blank']])
 
     if s == 2:
         p_values = t_test(data_array, v)
     elif s > 2:
@@ -146,15 +146,15 @@
         Whether to transform the data.
     gapFillingRatio : float
         The ratio for gap-filling.
     output_dir : str
         The output directory.
     """
 
-    X = np.array(data_array, dtype=float)
+    X = np.array(data_array, dtype=np.float64)
 
     # drop the columns with all zeros
     X = X[~np.all(X == 0, axis=1), :]
 
     # Gap-filling
     for i, vec in enumerate(X):
         if not np.all(vec):
```

### Comparing `masscube-0.0.8/src/masscube/utils_functions.py` & `masscube-0.0.9/src/masscube/utils_functions.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/src/masscube/visualization.py` & `masscube-0.0.9/src/masscube/visualization.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.8/src/masscube/workflows.py` & `masscube-0.0.9/src/masscube/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .stats import statistical_analysis
 from .feature_table_utils import calculate_fill_percentage
 
 
 # 1. Untargeted feature detection for a single file
 def feature_detection(file_name, params=None, cal_g_score=True, cal_a_score=True,
                       anno_isotope=True, anno_adduct=True, anno_in_source_fragment=True, 
-                      annotation=False, ms2_library_path=None, output_dir=None):
+                      annotation=False, ms2_library_path=None, output_dir=None, cut_roi=True):
     """
     Untargeted feature detection from a single file (.mzML or .mzXML).
 
     Parameters
     ----------
     file_name : str
         Path to the raw file.
@@ -75,15 +75,16 @@
         # read raw data
         d.read_raw_data(file_name, params)
 
         # detect region of interests (ROIs)
         d.find_rois()
 
         # cut ROIs
-        d.cut_rois()
+        if cut_roi:
+            d.cut_rois()
 
         # label short ROIs, find the best MS2, and sort ROIs by m/z
         d.summarize_roi(cal_g_score=cal_g_score, cal_a_score=cal_a_score)
 
         # # annotate isotopes, adducts, and in-source fragments
         if anno_isotope:
             annotate_isotope(d)
```

### Comparing `masscube-0.0.8/src/masscube.egg-info/PKG-INFO` & `masscube-0.0.9/src/masscube.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.8
+Version: 0.0.9
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `masscube-0.0.8/src/masscube.egg-info/SOURCES.txt` & `masscube-0.0.9/src/masscube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

