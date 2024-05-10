# Comparing `tmp/rHDPE_Data_Analysis-1.0.8.tar.gz` & `tmp/rHDPE_Data_Analysis-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rHDPE_Data_Analysis-1.0.8.tar", last modified: Fri May  3 14:36:05 2024, max compression
+gzip compressed data, was "rHDPE_Data_Analysis-1.0.9.tar", last modified: Fri May 10 12:34:32 2024, max compression
```

## Comparing `rHDPE_Data_Analysis-1.0.8.tar` & `rHDPE_Data_Analysis-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:36:05.959198 rHDPE_Data_Analysis-1.0.8/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-03 14:36:05.958242 rHDPE_Data_Analysis-1.0.8/PKG-INFO
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:36:05.919841 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:36:05.935718 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2750 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)    16419 2023-08-07 12:36:28.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py
--rw-r--r--   0 philsmith   (501) staff       (20)     8459 2024-05-02 13:58:33.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
--rw-r--r--   0 philsmith   (501) staff       (20)     2284 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     9607 2024-04-29 13:43:44.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    43760 2024-05-01 16:22:46.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:36:05.951977 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2071 2024-05-03 14:35:41.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)     1690 2024-05-03 09:44:18.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     4957 2024-05-03 11:51:35.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    38486 2024-05-03 14:34:12.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/__init__.py
--rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 11:22:18.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-03 14:36:05.927467 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis.egg-info/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-03 14:36:05.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis.egg-info/PKG-INFO
--rw-r--r--   0 philsmith   (501) staff       (20)      861 2024-05-03 14:36:05.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis.egg-info/SOURCES.txt
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-05-03 14:36:05.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis.egg-info/dependency_links.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-05-03 14:36:05.000000 rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis.egg-info/top_level.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-05-03 14:36:05.959360 rHDPE_Data_Analysis-1.0.8/setup.cfg
--rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-05-03 14:35:41.000000 rHDPE_Data_Analysis-1.0.8/setup.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-10 12:34:32.930685 rHDPE_Data_Analysis-1.0.9/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-10 12:34:32.930147 rHDPE_Data_Analysis-1.0.9/PKG-INFO
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-10 12:34:32.902055 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-10 12:34:32.917451 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     1853 2024-05-10 12:31:39.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     9850 2024-05-10 12:26:38.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/DSC_plotting.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     6266 2023-02-20 12:24:52.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/Deprecated.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1876 2024-05-09 15:47:40.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    12558 2024-05-09 16:50:22.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    17868 2024-05-10 12:28:11.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      147 2023-11-15 16:51:57.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/DSC_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-10 12:34:32.924477 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2750 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    16419 2023-08-07 12:36:28.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     8459 2024-05-02 13:58:33.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     2284 2024-05-02 13:57:15.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     9805 2024-05-09 15:05:09.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    44079 2024-05-07 16:06:14.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-10 12:34:32.929283 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2071 2024-05-03 14:35:41.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1690 2024-05-03 09:44:18.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     4957 2024-05-03 11:51:35.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    38486 2024-05-03 14:34:12.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/__init__.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 11:22:18.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-10 12:34:32.910115 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis.egg-info/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-10 12:34:32.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis.egg-info/PKG-INFO
+-rw-r--r--   0 philsmith   (501) staff       (20)     1202 2024-05-10 12:34:32.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-05-10 12:34:32.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-05-10 12:34:32.000000 rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis.egg-info/top_level.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-05-10 12:34:32.930827 rHDPE_Data_Analysis-1.0.9/setup.cfg
+-rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-05-10 12:33:51.000000 rHDPE_Data_Analysis-1.0.9/setup.py
```

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
     # Add f for probably faulty experimental data.
     # Add r for repetitions.
     # Add p for virgin specimen that (erroneously) contains significant PP.
     # Add n for noisy.
     # Add a for additive data.
     # Add e for ebm trial sprectra.
     # Add u for Unilever FTIRs.
+    # Add b for blends.
 
     specimens = {40:[0, 1, 2], 41:[0, 1, 2, 3, 4, 5]}
 
     for f in file_data:
 
         if f[0] in specimens.keys():
 
@@ -243,18 +244,24 @@
 
         if f[0] >= 301 and f[0] <= 400:
 
             f[3] = f[3] + "e"
 
     for f in file_data:
 
-        if f[0] >= 401 and f[0] <= 500:
+        if f[0] >= 401 and f[0] <= 499:
 
             f[3] = f[3] + "u"
 
+    for f in file_data:
+
+        if f[0] >= 500 and f[0] <= 599:
+
+            f[3] = f[3] + "b"
+
 def read_files_and_preprocess( directory, data_directory, merge_groups ):
     '''Read files and preprocess data.'''
 
     file_data, data = extract_raw_data( directory, data_directory )
 
     standardise_data( data )
 
@@ -361,14 +368,18 @@
 
             files_to_remove.append( i )
 
         elif s.find( "u" ) > -0.5:
 
             files_to_remove.append( i )
 
+        elif s.find( "b" ) > -0.5:
+
+            files_to_remove.append( i )
+
     files_to_remove.reverse()
 
     for r in files_to_remove:
 
         file_data.pop( r )
         data[1].pop( r )
```

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,16 +338,17 @@
 
     feature_names, features = gu.csv_to_df_to_array_and_column_titles( ip.output_directory + "FTIR/Features/Specimen_Features.csv" )
 
     sample, sample_array, samples_present, samples_present_array = gu.sample_data_from_file_data( file_data )
 
     if not ip.sample_mask:
 
-        ip.sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 24]
+        # ip.sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 24]
         # ip.sample_mask = [301, 303, 306, 308, 309, 312, 313, 315, 318, 320, 324, 325]
+        ip.sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 24, 500, 502, 504, 506, 508, 510, 512, 514, 516, 518]
 
     sample_mask = ip.sample_mask
 
     sample_mask = gu.remove_redundant_samples( sample_mask, samples_present )
 
     if not ip.feature_selection:
 
@@ -587,15 +588,16 @@
     plot_mean_features = True
 
     resin_data = gu.get_list_of_resins_data( directory )
 
     sample, sample_array, samples_present, samples_present_array = gu.sample_data_from_file_data( file_data )
 
     # sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8]
-    sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 401, 402, 403, 404, 405, 406, 407, 408, 409, 410, 411, 412, 413, 414, 415, 416]
+    # sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 401, 402, 403, 404, 405, 406, 407, 408, 409, 410, 411, 412, 413, 414, 415, 416]
+    sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 500, 502, 504, 506, 508, 510, 512, 514, 516, 518]
 
     sample_mask = gu.remove_redundant_samples( sample_mask, samples_present )
 
     pp_integrals = [835, 845, 993, 1005, 2950, 2970]
 
     features = []
```

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Analysis.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Analysis/Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis/Global_Utilities.py` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis/Global_Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.8/rHDPE_Data_Analysis.egg-info/SOURCES.txt` & `rHDPE_Data_Analysis-1.0.9/rHDPE_Data_Analysis.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 setup.py
 rHDPE_Data_Analysis/Global_Utilities.py
 rHDPE_Data_Analysis/__init__.py
 rHDPE_Data_Analysis.egg-info/PKG-INFO
 rHDPE_Data_Analysis.egg-info/SOURCES.txt
 rHDPE_Data_Analysis.egg-info/dependency_links.txt
 rHDPE_Data_Analysis.egg-info/top_level.txt
+rHDPE_Data_Analysis/DSC_Analysis/Analysis.py
+rHDPE_Data_Analysis/DSC_Analysis/DSC_plotting.py
+rHDPE_Data_Analysis/DSC_Analysis/Deprecated.py
+rHDPE_Data_Analysis/DSC_Analysis/Input_Parameters_Class.py
+rHDPE_Data_Analysis/DSC_Analysis/Preprocessing.py
+rHDPE_Data_Analysis/DSC_Analysis/Utilities.py
+rHDPE_Data_Analysis/DSC_Analysis/__init__.py
 rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
 rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py
 rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
 rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
 rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
 rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
 rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
```

