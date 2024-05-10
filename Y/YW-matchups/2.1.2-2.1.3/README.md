# Comparing `tmp/YW_matchups-2.1.2.tar.gz` & `tmp/YW_matchups-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YW_matchups-2.1.2.tar", last modified: Wed May  8 00:56:50 2024, max compression
+gzip compressed data, was "YW_matchups-2.1.3.tar", last modified: Fri May 10 01:05:43 2024, max compression
```

## Comparing `YW_matchups-2.1.2.tar` & `YW_matchups-2.1.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-08 00:56:50.151839 YW_matchups-2.1.2/
--rw-r--r--   0 yw         (501) staff       (20)      617 2024-05-08 00:56:50.151586 YW_matchups-2.1.2/PKG-INFO
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-08 00:56:50.148743 YW_matchups-2.1.2/YW_matchups/
--rw-r--r--   0 yw         (501) staff       (20)     3104 2024-05-02 03:17:42.000000 YW_matchups-2.1.2/YW_matchups/AC_acolite.py
--rw-r--r--   0 yw         (501) staff       (20)     3906 2023-12-28 03:02:04.000000 YW_matchups-2.1.2/YW_matchups/AC_l2gen.py
--rw-r--r--   0 yw         (501) staff       (20)     2835 2023-12-26 17:52:26.000000 YW_matchups-2.1.2/YW_matchups/AC_polymer.py
--rw-r--r--   0 yw         (501) staff       (20)      297 2023-12-16 21:20:26.000000 YW_matchups-2.1.2/YW_matchups/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)    10332 2024-05-08 00:54:58.000000 YW_matchups-2.1.2/YW_matchups/run.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-08 00:56:50.149667 YW_matchups-2.1.2/YW_matchups.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)      617 2024-05-08 00:56:50.000000 YW_matchups-2.1.2/YW_matchups.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)      447 2024-05-08 00:56:50.000000 YW_matchups-2.1.2/YW_matchups.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2024-05-08 00:56:50.000000 YW_matchups-2.1.2/YW_matchups.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       28 2024-05-08 00:56:50.000000 YW_matchups-2.1.2/YW_matchups.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)       12 2024-05-08 00:56:50.000000 YW_matchups-2.1.2/YW_matchups.egg-info/top_level.txt
--rw-r--r--   0 yw         (501) staff       (20)       38 2024-05-08 00:56:50.151898 YW_matchups-2.1.2/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)      644 2024-05-08 00:55:44.000000 YW_matchups-2.1.2/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-08 00:56:50.151230 YW_matchups-2.1.2/tests/
--rw-r--r--   0 yw         (501) staff       (20)      822 2023-12-26 16:46:40.000000 YW_matchups-2.1.2/tests/test_acolite_L8.py
--rw-r--r--   0 yw         (501) staff       (20)      853 2023-12-18 19:48:30.000000 YW_matchups-2.1.2/tests/test_acolite_S2.py
--rw-r--r--   0 yw         (501) staff       (20)      673 2023-12-26 18:27:02.000000 YW_matchups-2.1.2/tests/test_l2gen_L8.py
--rw-r--r--   0 yw         (501) staff       (20)      961 2023-12-23 19:30:03.000000 YW_matchups-2.1.2/tests/test_l2gen_S2.py
--rw-r--r--   0 yw         (501) staff       (20)      555 2023-12-31 21:17:41.000000 YW_matchups-2.1.2/tests/test_polymer_L8.py
--rw-r--r--   0 yw         (501) staff       (20)      689 2023-12-17 19:16:32.000000 YW_matchups-2.1.2/tests/test_polymer_S2.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-10 01:05:43.179169 YW_matchups-2.1.3/
+-rw-r--r--   0 yw         (501) staff       (20)      617 2024-05-10 01:05:43.178933 YW_matchups-2.1.3/PKG-INFO
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-10 01:05:43.176853 YW_matchups-2.1.3/YW_matchups/
+-rw-r--r--   0 yw         (501) staff       (20)     3550 2024-05-10 00:53:35.000000 YW_matchups-2.1.3/YW_matchups/AC_acolite.py
+-rw-r--r--   0 yw         (501) staff       (20)     3906 2023-12-28 03:02:04.000000 YW_matchups-2.1.3/YW_matchups/AC_l2gen.py
+-rw-r--r--   0 yw         (501) staff       (20)     2835 2023-12-26 17:52:26.000000 YW_matchups-2.1.3/YW_matchups/AC_polymer.py
+-rw-r--r--   0 yw         (501) staff       (20)      297 2023-12-16 21:20:26.000000 YW_matchups-2.1.3/YW_matchups/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)    10444 2024-05-10 01:04:34.000000 YW_matchups-2.1.3/YW_matchups/run.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-10 01:05:43.177521 YW_matchups-2.1.3/YW_matchups.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)      617 2024-05-10 01:05:43.000000 YW_matchups-2.1.3/YW_matchups.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)      473 2024-05-10 01:05:43.000000 YW_matchups-2.1.3/YW_matchups.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2024-05-10 01:05:43.000000 YW_matchups-2.1.3/YW_matchups.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       28 2024-05-10 01:05:43.000000 YW_matchups-2.1.3/YW_matchups.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)       12 2024-05-10 01:05:43.000000 YW_matchups-2.1.3/YW_matchups.egg-info/top_level.txt
+-rw-r--r--   0 yw         (501) staff       (20)       38 2024-05-10 01:05:43.179221 YW_matchups-2.1.3/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)      644 2024-05-10 01:04:40.000000 YW_matchups-2.1.3/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-10 01:05:43.178637 YW_matchups-2.1.3/tests/
+-rw-r--r--   0 yw         (501) staff       (20)      955 2024-05-10 00:54:21.000000 YW_matchups-2.1.3/tests/test_acolite_L2R.py
+-rw-r--r--   0 yw         (501) staff       (20)      822 2023-12-26 16:46:40.000000 YW_matchups-2.1.3/tests/test_acolite_L8.py
+-rw-r--r--   0 yw         (501) staff       (20)      855 2024-05-09 23:40:36.000000 YW_matchups-2.1.3/tests/test_acolite_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)      673 2023-12-26 18:27:02.000000 YW_matchups-2.1.3/tests/test_l2gen_L8.py
+-rw-r--r--   0 yw         (501) staff       (20)      961 2023-12-23 19:30:03.000000 YW_matchups-2.1.3/tests/test_l2gen_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)      555 2023-12-31 21:17:41.000000 YW_matchups-2.1.3/tests/test_polymer_L8.py
+-rw-r--r--   0 yw         (501) staff       (20)      689 2023-12-17 19:16:32.000000 YW_matchups-2.1.3/tests/test_polymer_S2.py
```

### Comparing `YW_matchups-2.1.2/PKG-INFO` & `YW_matchups-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YW_matchups
-Version: 2.1.2
+Version: 2.1.3
 Summary: Find satellite matchups for aquatic remote sensing
 Author: Yulun Wu
 Author-email: yulunwu8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyproj
```

### Comparing `YW_matchups-2.1.2/YW_matchups/AC_acolite.py` & `YW_matchups-2.1.3/YW_matchups/AC_polymer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,75 @@
 
 
 
-# Tool package for ACOLITE
+# Tool package for POLYMER
 
 
 import netCDF4 as nc4
 import ast
 import numpy as np
 import datetime as dt
 
 
 
 # Get datetime object 
 def get_datetime(sat_file):
     with nc4.Dataset(sat_file,"r") as nc:
-        
         sensor = nc.getncattr('sensor')
-
-        
-        ### full resolution ###
-        # datetime_sat_string = nc.getncattr('isodate')
-        # format_string = '%Y-%m-%dT%H:%M:%S.%f%z'
-        
-        # March 20, 2024 update: prioritize inputfile name instead
         
-        try: 
+        if sensor =='MSI': 
+            datetime_sat_string = nc.getncattr('sensing_time')
+            format_string = '%Y-%m-%d %H:%M:%S'
+            datetime_sat_obj = dt.datetime.strptime(datetime_sat_string, format_string)
+            add_a_day = False
             
-            if sensor=='L8_OLI': raise Exception()
+        elif sensor == 'OLI':
+            l1_dirname = nc.getncattr('l1_dirname')
+            extracted_date = l1_dirname[-23:-15]
+            format_string = '%Y%m%d'
+            datetime_sat_obj = dt.datetime.strptime(extracted_date, format_string)   
+            add_a_day = True
             
-            inputfile = nc.getncattr('inputfile').split('/')[-1]
-            datetime_sat_string = inputfile[11:26]
-            format_string = '%Y%m%dT%H%M%S'
-            
-        except:
-            # nearest second 
-            datetime_sat_string = nc.getncattr('isodate').split('.', 1)[0]
-            format_string = '%Y-%m-%dT%H:%M:%S'
-            
-        datetime_sat_obj = dt.datetime.strptime(datetime_sat_string, format_string)
-    return [datetime_sat_obj, False]
+    return [datetime_sat_obj, add_a_day]
     
     
 
 # Read NC data 
 
 def read_file(sat_file):
     
     with nc4.Dataset(sat_file,"r") as nc:
-        sensor = nc.getncattr('sensor')
-        
-        # S2 wavelengths 
-        if sensor == 'S2A_MSI' or sensor == 'S2B_MSI':
-            column_names = ['B1','B2','B3','B4','B5','B6','B7','B8','B8A','B11','B12']
         
-            if sensor == 'S2A_MSI':
-                bands = [443,492,560,665,704,740,783,833,865,1614,2202] 
-            elif sensor == 'S2B_MSI':
-                bands = [442,492,559,665,704,739,780,833,864,1610,2186]
+        sensor_temp = nc.getncattr('sensor')
         
-        # L8 wavelengths
-        elif sensor == 'L8_OLI':
-            bands = [443, 483, 561, 655, 865, 1609, 2201]
-            column_names = ['B1','B2','B3','B4','B5','B6','B7']
+        if sensor_temp == 'MSI':
+            tile_id = nc.getncattr('L1_TILE_ID')
+            sensor = tile_id[0:3]
+            if sensor == 'S2A' or sensor == 'S2B':
+                column_names = ['B1','B2','B3','B4','B5','B6','B7','B8','B8A','B11']
+                if sensor == 'S2A': sensor = 'S2A_MSI'
+                if sensor == 'S2B': sensor = 'S2B_MSI'
+                
+        elif sensor_temp == 'OLI':
+            sensor = 'L8_OLI'
+            column_names = ['B1','B2','B3','B4','B5']
+                
+        bands = nc.getncattr('bands_rw')
+        bands = ast.literal_eval(bands)
         
         # band names for extracting values
-        band_names = ['rhow_' + str(item) for item in bands]
+        band_names = ['Rw' + str(item) for item in bands]
 
         # dimension
-        global_dims = nc.getncattr('global_dims')
-        # YW: I'm not sure about 0 and 1, but both S2 and PRISMA have square images
-        height = global_dims[0] # equivalent to 'lines' before 
-        width = global_dims[1]  # equivalent to 'pixels' before 
+        width = len(nc.dimensions['width']) # equivalent to 'pixels' before 
+        height = len(nc.dimensions['height']) # equivalent to 'lines' before 
 
         # latlon
-        lat = nc.variables['lat'][:,:]
-        lon = nc.variables['lon'][:,:]
+        lat = nc.variables['latitude'][:,:]
+        lon = nc.variables['longitude'][:,:]
 
         # to store data
         rhow_data = np.ma.empty([len(bands),int(height),int(width)])
 
         for k in range(len(bands)):
             varname = band_names[k]
             rhow_data[k] = nc.variables[varname][:,:]
```

### Comparing `YW_matchups-2.1.2/YW_matchups/AC_l2gen.py` & `YW_matchups-2.1.3/YW_matchups/AC_l2gen.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.2/YW_matchups/run.py` & `YW_matchups-2.1.3/YW_matchups/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 from . import AC_l2gen
 
 
 # make time column and string an option 
 
 
 
-def run(sat_folder=None, is_file=None, AC=None, out_file=None, to_log = True, dt_column = 'GLORIA_time', dt_string = "%Y-%m-%dT%H:%M", output_sd = False):
+def run(sat_folder=None, is_file=None, AC=None, out_file=None, to_log = True, 
+        dt_column='GLORIA_time', dt_string = "%Y-%m-%dT%H:%M", output_sd = False,
+        ACOLITE_L2R=False):
     
     
     ### Settings to be included later 
     time_window_minutes = 720 
     max_dist = 100
     
     
@@ -85,14 +87,15 @@
     print('sat_folder: ' + str(sat_folder))
     print('In-situ file: ' + str(is_file))
     print('AC: ' + str(AC))
     print('out_file: ' + str(out_file))
     print('dt_column: ' + str(dt_column))
     print('dt_string: ' + str(dt_string))
     print('output_sd: ' + str(output_sd))
+    print('ACOLITE_L2R: ' + str(ACOLITE_L2R))
     if to_log: print('log_file: ' + str(log_file))
     
     # Settings 
     print('window_size: ' + str(window_size))
     print('time_window_minutes: ' + str(time_window_minutes))
     print('max_dist: ' + str(max_dist))
     
@@ -108,14 +111,15 @@
     ### find all NC files 
     
     # Keywords for .nc files 
     if AC=='POLYMER' or AC=='L2gen': 
         AC_file = '*.nc'
     elif AC=='ACOLITE':
         AC_file = '*L2W.nc'
+        if ACOLITE_L2R: AC_file = '*L2R.nc'
     else: 
         sys.exit('Unknown AC algorithm')
     
     # Find them in the directory and subdirectory 
     # https://stackoverflow.com/questions/18394147/how-to-do-a-recursive-sub-folder-search-and-return-files-in-a-list
     sat_files = [y for x in os.walk(sat_folder) for y in glob.glob(os.path.join(x[0], AC_file))]
     
@@ -149,28 +153,27 @@
         # this is okay because L8 doesn't visit the same place two days in a row
         if add_a_day: tw_minutes = tw_minutes + 1440
 
 
         # Indices of in-situ data that match the sat datetime  
         is_matches = [ind for ind, s in enumerate(dt_is_obj) if abs((dt_sat_obj - s).total_seconds()/60) <= tw_minutes]
         
-        
+
         # If there are no matching records, skip to next satellite file.
         if len(is_matches)==0:
             print("No matches for this file within the time limit. Next...\n\n")
             continue
         elif len(is_matches) > 1:
             print('Number of matchups: ' + str(len(is_matches)))
-        
-        
+
         ### Read NC data, for different AC
         if AC=='POLYMER': 
             sat_data = AC_polymer.read_file(sat_file)
         elif AC=='ACOLITE':
-            sat_data = AC_acolite.read_file(sat_file)
+            sat_data = AC_acolite.read_file(sat_file, ACOLITE_L2R)
         elif AC=='L2gen':
             sat_data = AC_l2gen.read_file(sat_file)
         
         
         ### Loop through indices and row numbers of in-situ matchups
         
         for ind, row in enumerate(is_matches):
```

### Comparing `YW_matchups-2.1.2/YW_matchups.egg-info/PKG-INFO` & `YW_matchups-2.1.3/YW_matchups.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YW-matchups
-Version: 2.1.2
+Version: 2.1.3
 Summary: Find satellite matchups for aquatic remote sensing
 Author: Yulun Wu
 Author-email: yulunwu8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyproj
```

### Comparing `YW_matchups-2.1.2/setup.py` & `YW_matchups-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='YW_matchups',
-    version='2.1.2',
+    version='2.1.3',
     author='Yulun Wu',
     author_email='yulunwu8@gmail.com',
     description='Find satellite matchups for aquatic remote sensing',
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `YW_matchups-2.1.2/tests/test_acolite_L8.py` & `YW_matchups-2.1.3/tests/test_acolite_L8.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.2/tests/test_acolite_S2.py` & `YW_matchups-2.1.3/tests/test_acolite_S2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # sat_file = '/Users/yw/Desktop/230613 AEC paper/231130 POLYMER/test_output_S2_60m.nc'
 
 
 # sat_folder = '/Users/yw/Desktop/230613 AEC paper/231130 POLYMER'
 
 sat_folder = '/Volumes/San2T/GLORIA/ACed/S2_Tmart_ACOLITE/S2A_MSIL1C_20150912T101403_N0204_R022_T32TPR_20150912T101724'
-sat_folder = '/Users/yw/Downloads'
+# sat_folder = '/Users/yw/Downloads'
 
 
 
 is_file = '/Users/yw/Desktop/230613 AEC paper/231130 POLYMER/test_in_situ.csv'
 out_file = '/Users/yw/Desktop/230613 AEC paper/231130 POLYMER/test_out.csv'
```

### Comparing `YW_matchups-2.1.2/tests/test_l2gen_L8.py` & `YW_matchups-2.1.3/tests/test_l2gen_L8.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.2/tests/test_l2gen_S2.py` & `YW_matchups-2.1.3/tests/test_l2gen_S2.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.2/tests/test_polymer_L8.py` & `YW_matchups-2.1.3/tests/test_polymer_L8.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.2/tests/test_polymer_S2.py` & `YW_matchups-2.1.3/tests/test_polymer_S2.py`

 * *Files identical despite different names*

