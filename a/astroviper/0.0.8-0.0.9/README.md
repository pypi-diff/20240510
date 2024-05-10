# Comparing `tmp/astroviper-0.0.8.tar.gz` & `tmp/astroviper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroviper-0.0.8.tar", last modified: Wed Dec 13 20:28:24 2023, max compression
+gzip compressed data, was "astroviper-0.0.9.tar", last modified: Thu Feb  1 23:49:41 2024, max compression
```

## Comparing `astroviper-0.0.8.tar` & `astroviper-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.212480 astroviper-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-13 20:28:16.000000 astroviper-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-13 20:28:16.000000 astroviper-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2023-12-13 20:28:24.212480 astroviper-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-13 20:28:16.000000 astroviper-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-12-13 20:28:16.000000 astroviper-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:28:24.212480 astroviper-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.204480 astroviper-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.204480 astroviper-0.0.8/src/astroviper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.204480 astroviper-0.0.8/src/astroviper/_domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/_domain/_image/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_image/_moment_max.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/_domain/_imaging/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10083 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_check_imaging_parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9803 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_fft_norm_img_xds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/_domain/_imaging/_imaging_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_imaging_utils/_make_pb_symmetric.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_imaging_utils/_mosaic_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    18431 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_imaging_utils/_standard_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4417 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_aperture_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15990 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_gridding_convolution_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_imaging_weights.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3479 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_uv_sampling_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3813 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_visibility_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/_domain/_visibility/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6721 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/_domain/_visibility/_phase_shift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/calibration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/flagging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/flagging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/imaging/cube_imaging_niter0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper/visibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:16.000000 astroviper-0.0.8/src/astroviper/visibility/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:28:24.208480 astroviper-0.0.8/src/astroviper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2023-12-13 20:28:24.000000 astroviper-0.0.8/src/astroviper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-13 20:28:24.000000 astroviper-0.0.8/src/astroviper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:28:24.000000 astroviper-0.0.8/src/astroviper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-13 20:28:24.000000 astroviper-0.0.8/src/astroviper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-13 20:28:24.000000 astroviper-0.0.8/src/astroviper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.093510 astroviper-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-01 23:49:33.000000 astroviper-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-01 23:49:33.000000 astroviper-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-02-01 23:49:41.089510 astroviper-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-01 23:49:33.000000 astroviper-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-01 23:49:33.000000 astroviper-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 23:49:41.093510 astroviper-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.081510 astroviper-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.085510 astroviper-0.0.9/src/astroviper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.085510 astroviper-0.0.9/src/astroviper/_domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.085510 astroviper-0.0.9/src/astroviper/_domain/_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_image/_moment_max.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/_domain/_imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10083 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_check_imaging_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_fft.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9803 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_fft_norm_img_xds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_ifft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/_domain/_imaging/_imaging_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_imaging_utils/_make_pb_symmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_imaging_utils/_mosaic_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18431 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_imaging_utils/_standard_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4417 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_aperture_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15990 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_gridding_convolution_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_imaging_weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3479 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_uv_sampling_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3813 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_visibility_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/_domain/_visibility/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6721 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/_domain/_visibility/_phase_shift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/calibration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/flagging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/flagging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/imaging/cube_imaging_niter0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper/visibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:33.000000 astroviper-0.0.9/src/astroviper/visibility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 23:49:41.089510 astroviper-0.0.9/src/astroviper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-02-01 23:49:41.000000 astroviper-0.0.9/src/astroviper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-01 23:49:41.000000 astroviper-0.0.9/src/astroviper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 23:49:41.000000 astroviper-0.0.9/src/astroviper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-01 23:49:41.000000 astroviper-0.0.9/src/astroviper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-01 23:49:41.000000 astroviper-0.0.9/src/astroviper.egg-info/top_level.txt
```

### Comparing `astroviper-0.0.8/LICENSE.txt` & `astroviper-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/PKG-INFO` & `astroviper-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroviper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Astro Visibility and Image Parallel Execution Reduction
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Associated Universities, Inc.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `astroviper-0.0.8/pyproject.toml` & `astroviper-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astroviper"
-version = "0.0.8"
+version = "0.0.9"
 description = "Astro Visibility and Image Parallel Execution Reduction"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">= 3.8, < 3.12"
```

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_check_imaging_parameters.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_check_imaging_parameters.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_fft_norm_img_xds.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_fft_norm_img_xds.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_imaging_utils/_make_pb_symmetric.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_imaging_utils/_make_pb_symmetric.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_imaging_utils/_mosaic_grid.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_imaging_utils/_mosaic_grid.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_imaging_utils/_standard_grid.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_imaging_utils/_standard_grid.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_aperture_grid.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_aperture_grid.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_gridding_convolution_function.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_gridding_convolution_function.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_image.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-def _make_image(input_parms):
+def _make_image(input_params):
     import time
     from xradio.vis.load_processing_set import load_processing_set
 
     start_total = time.time()
     # from astroviper._utils._logger import _get_logger
     # logger = _get_logger()
     # logger.debug(
-    #     "Processing chunk " + str(input_parms["chunk_id"]) + " " + str(logger.level)
+    #     "Processing chunk " + str(input_params["chunk_id"]) + " " + str(logger.level)
     # )
 
     start_0 = time.time()
     import numpy as np
     from astroviper._domain._visibility._phase_shift import _phase_shift_vis_ds
     from astroviper._domain._imaging._make_imaging_weights import _make_imaging_weights
     from astroviper._domain._imaging._make_gridding_convolution_function import (
@@ -25,158 +25,158 @@
     from astroviper._domain._imaging._fft_norm_img_xds import _fft_norm_img_xds
 
     from xradio.vis.load_processing_set import load_processing_set
     import xarray as xr
     # print("0. Imports",time.time()-start_0)
 
     start_1 = time.time()
-    grid_parms = input_parms["grid_parms"]
+    grid_params = input_params["grid_params"]
 
-    shift_parms = {}
-    shift_parms["new_phase_direction"] = grid_parms["phase_direction"]
-    shift_parms["common_tangent_reprojection"] = True
+    shift_params = {}
+    shift_params["new_phase_direction"] = grid_params["phase_direction"]
+    shift_params["common_tangent_reprojection"] = True
 
-    if input_parms["grid_parms"]["frequency"] is not None:
-        image_freq_coord = input_parms["grid_parms"]["frequency"]
+    if input_params["grid_params"]["frequency"] is not None:
+        image_freq_coord = input_params["grid_params"]["frequency"]
     else:
-        image_freq_coord = input_parms["task_coords"]["frequency"]["data"]
+        image_freq_coord = input_params["task_coords"]["frequency"]["data"]
 
-    if input_parms["grid_parms"]["polarization"] is not None:
-        image_polarization_coord = input_parms["grid_parms"]["polarization"]
+    if input_params["grid_params"]["polarization"] is not None:
+        image_polarization_coord = input_params["grid_params"]["polarization"]
     else:
-        image_polarization_coord = input_parms["task_coords"]["polarization"]["data"]
+        image_polarization_coord = input_params["task_coords"]["polarization"]["data"]
 
-    if input_parms["grid_parms"]["time"] is not None:
-        image_time_coord = input_parms["grid_parms"]["time"]
+    if input_params["grid_params"]["time"] is not None:
+        image_time_coord = input_params["grid_params"]["time"]
     else:
-        image_time_coord = input_parms["task_coords"]["time"]["data"]
+        image_time_coord = input_params["task_coords"]["time"]["data"]
 
     img_xds = make_empty_sky_image(
-        phase_center=grid_parms["phase_direction"]["data"],
-        image_size=grid_parms["image_size"],
-        cell_size=grid_parms["cell_size"],
+        phase_center=grid_params["phase_direction"]["data"],
+        image_size=grid_params["image_size"],
+        cell_size=grid_params["cell_size"],
         chan_coords=image_freq_coord,
         pol_coords=image_polarization_coord,
         time_coords=image_time_coord,
     )
     img_xds.attrs["data_groups"] = {"mosaic": {}}
 
     # print("1. Empty Image",time.time()-start_1)
 
     gcf_xds = xr.Dataset()
 
 
 
-    for ms_v4_name, slice_description in input_parms["data_selection"].items():
+    for ms_v4_name, slice_description in input_params["data_selection"].items():
         start_2 = time.time()
  
-        if input_parms["input_data"] is None:
+        if input_params["input_data"] is None:
             ps = load_processing_set(
-                    ps_name=input_parms["input_data_store"],
+                    ps_name=input_params["input_data_store"],
                     sel_parms={ms_v4_name: slice_description},
                 )
             ms_xds = ps.get(0)
         else:
-            img_xds = input_parms["input_data"][ms_v4_name] #In memory
+            img_xds = input_params["input_data"][ms_v4_name] #In memory
 
         # print("2. Load",time.time()-start_2)
 
         start_3 = time.time()
         data_group_out = _phase_shift_vis_ds(
-            ms_xds, shift_parms=shift_parms, sel_parms={}
+            ms_xds, shift_parms=shift_params, sel_parms={}
         )
         # print("3. phase_shift",time.time()-start_3)
 
         start_4 = time.time()
         data_group_out = _make_imaging_weights(
             ms_xds,
-            grid_parms=grid_parms,
+            grid_parms=grid_params,
             imaging_weights_parms={"weighting": "briggs", "robust": 0.6},
             sel_parms={"data_group_in": data_group_out},
         )
 
-        gcf_parms = {}
-        gcf_parms["function"] = "casa_airy"
-        gcf_parms["list_dish_diameters"] = np.array([10.7])
-        gcf_parms["list_blockage_diameters"] = np.array([0.75])
+        gcf_params = {}
+        gcf_params["function"] = "casa_airy"
+        gcf_params["list_dish_diameters"] = np.array([10.7])
+        gcf_params["list_blockage_diameters"] = np.array([0.75])
 
         # print("4. Phase_shift ",time.time()-start_4)
 
         start_4_1 = time.time()
         # print(ms_xds.attrs['antenna_xds'])
         unique_ant_indx = ms_xds.attrs["antenna_xds"].DISH_DIAMETER.values
         unique_ant_indx[unique_ant_indx == 12.0] = 0
 
-        gcf_parms["unique_ant_indx"] = unique_ant_indx.astype(int)
-        gcf_parms["phase_direction"] = grid_parms["phase_direction"]
+        gcf_params["unique_ant_indx"] = unique_ant_indx.astype(int)
+        gcf_params["phase_direction"] = grid_params["phase_direction"]
         _make_gridding_convolution_function(
             gcf_xds,
             ms_xds,
-            gcf_parms,
-            grid_parms,
+            gcf_params,
+            grid_params,
             sel_parms={"data_group_in": data_group_out},
         )
         # print("4.1 make_gridding_convolution_function ",time.time()-start_4_1)
 
         start_4_2 = time.time()
         _make_aperture_grid(
             ms_xds,
             gcf_xds,
             img_xds,
             vis_sel_parms={"data_group_in": data_group_out},
             img_sel_parms={"data_group_in": "mosaic"},
-            grid_parms=grid_parms,
+            grid_parms=grid_params,
         )
 
         _make_uv_sampling_grid(
             ms_xds,
             gcf_xds,
             img_xds,
             vis_sel_parms={"data_group_in": data_group_out},
             img_sel_parms={"data_group_in": "mosaic"},
-            grid_parms=grid_parms,
+            grid_parms=grid_params,
         )
 
         _make_visibility_grid(
             ms_xds,
             gcf_xds,
             img_xds,
             vis_sel_parms={"data_group_in": data_group_out},
             img_sel_parms={"data_group_in": "mosaic"},
-            grid_parms=grid_parms,
+            grid_parms=grid_params,
         )
 
         # print("4.2 rest ",time.time()-start_4_2)
     
 
     start_5 = time.time()
     _fft_norm_img_xds(
         img_xds,
         gcf_xds,
-        grid_parms,
+        grid_params,
         norm_parms={},
         sel_parms={"data_group_in": "mosaic", "data_group_out": "mosaic"},
     )
     # print("5. fft norm",time.time()-start_5)
 
     # Tranform uv-space -> lm-space (sky)
 
     start_6 = time.time()
     parallel_dims_chunk_id = dict(
-        zip(input_parms["parallel_dims"], input_parms["chunk_indices"])
+        zip(input_params["parallel_dims"], input_params["chunk_indices"])
     )
 
     from xradio.image._util._zarr.zarr_low_level import (
         pad_array_with_nans,
         write_binary_blob_to_disk,
     )
     import os
 
-    if input_parms["to_disk"]:
-        for data_varaible, meta in input_parms["zarr_meta"].items():
+    if input_params["to_disk"]:
+        for data_varaible, meta in input_params["zarr_meta"].items():
             dims = meta["dims"]
             dtype = meta["dtype"]
             data_varaible_name = meta["name"]
             chunks = meta["chunks"]
             shape = meta["shape"]
             chunk_name = ""
             if data_varaible_name in img_xds:
@@ -195,16 +195,16 @@
                     )
                 else:
                     array = img_xds[data_varaible_name].values
 
                 write_binary_blob_to_disk(
                     array,
                     file_path=os.path.join(
-                        input_parms["image_file"], data_varaible_name, chunk_name
+                        input_params["image_file"], data_varaible_name, chunk_name
                     ),
-                    compressor=input_parms["compressor"],
+                    compressor=input_params["compressor"],
                 )
     else:
         return img_xds
     # print("6. to disk",time.time()-start_6)
-    # print("Done chunk",input_parms['chunk_id'],time.time()-start_total)
+    # print("Done chunk",input_params['chunk_id'],time.time()-start_total)
     # print("***"*20)
```

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_imaging_weights.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_imaging_weights.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_uv_sampling_grid.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_uv_sampling_grid.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_imaging/_make_visibility_grid.py` & `astroviper-0.0.9/src/astroviper/_domain/_imaging/_make_visibility_grid.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/_domain/_visibility/_phase_shift.py` & `astroviper-0.0.9/src/astroviper/_domain/_visibility/_phase_shift.py`

 * *Files identical despite different names*

### Comparing `astroviper-0.0.8/src/astroviper/imaging/cube_imaging_niter0.py` & `astroviper-0.0.9/src/astroviper/imaging/cube_imaging_niter0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from numcodecs import Blosc
 
 
 def cube_imaging_niter0(
     ps_name,
     image_name,
-    grid_parms,
+    grid_params,
     n_chunks,
     data_variables=["sky", "point_spread_function", "primary_beam"],
     intents=["OBSERVE_TARGET#ON_SOURCE"],
     compressor=Blosc(cname="lz4", clevel=5),
 ):
     import numpy as np
     import xarray as xr
@@ -23,34 +23,34 @@
     import zarr
 
     # Get metadata
     ps = read_processing_set(ps_name, intents=intents)
     summary_df = ps.summary()
 
     # Get phase center of mosaic if field_id given.
-    if isinstance(grid_parms["phase_direction"], int):
+    if isinstance(grid_params["phase_direction"], int):
         ms_xds_name = summary_df.loc[
-            summary_df["field_id"] == grid_parms["phase_direction"]
+            summary_df["field_id"] == grid_params["phase_direction"]
         ].name.values[0]
-        grid_parms["phase_direction"] = ps[ms_xds_name].attrs["field_info"][
+        grid_params["phase_direction"] = ps[ms_xds_name].attrs["field_info"][
             "phase_direction"
         ]
 
     #Make Parallel Coords
     parallel_coords = {}
     ms_xds = ps.get(0)
     parallel_coords["frequency"] = make_parallel_coord(
         coord=ms_xds.frequency, n_chunks=n_chunks
     )
 
     #Create empty image
     img_xds = make_empty_sky_image(
-        phase_center=grid_parms["phase_direction"]["data"],
-        image_size=grid_parms["image_size"],
-        cell_size=grid_parms["cell_size"],
+        phase_center=grid_params["phase_direction"]["data"],
+        image_size=grid_params["image_size"],
+        cell_size=grid_params["cell_size"],
         chan_coords=parallel_coords["frequency"]["data"],
         pol_coords=ms_xds.polarization.values,
         time_coords=[0],
     )
 
     #print(img_xds)
 
@@ -74,33 +74,33 @@
     )
 
     sel_parms = {}
     sel_parms["intents"] = intents
     sel_parms["fields"] = None
 
     input_parms = {}
-    input_parms["grid_parms"] = grid_parms
+    input_parms["grid_params"] = grid_params
     input_parms["zarr_meta"] = zarr_meta
     input_parms["to_disk"] = True
-    input_parms["grid_parms"]["polarization"] = ms_xds.polarization.values
-    input_parms["grid_parms"]["frequency"] = None
-    input_parms["grid_parms"]["time"] = [0]
+    input_parms["grid_params"]["polarization"] = ms_xds.polarization.values
+    input_parms["grid_params"]["frequency"] = None
+    input_parms["grid_params"]["time"] = [0]
     input_parms["compressor"] = compressor
     input_parms["image_file"] = image_name
     input_parms["input_data_store"]=ps_name
 
     from graphviper.graph_tools.coordinate_utils import interpolate_data_coords_onto_parallel_coords
     node_task_data_mapping = interpolate_data_coords_onto_parallel_coords(parallel_coords, ps)
 
     #Create Map Graph
     graph = map(
         input_data=ps,
         node_task_data_mapping=node_task_data_mapping,
         node_task=_make_image,
-        input_parms=input_parms,
+        input_params=input_parms,
         in_memory_compute=False
     )
     input_parms = {}
 
     #Compute cube
     dask.compute(graph)
```

### Comparing `astroviper-0.0.8/src/astroviper.egg-info/PKG-INFO` & `astroviper-0.0.9/src/astroviper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroviper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Astro Visibility and Image Parallel Execution Reduction
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Associated Universities, Inc.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `astroviper-0.0.8/src/astroviper.egg-info/SOURCES.txt` & `astroviper-0.0.9/src/astroviper.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 src/astroviper.egg-info/dependency_links.txt
 src/astroviper.egg-info/requires.txt
 src/astroviper.egg-info/top_level.txt
 src/astroviper/_domain/__init__.py
 src/astroviper/_domain/_image/_moment_max.py
 src/astroviper/_domain/_imaging/__init__.py
 src/astroviper/_domain/_imaging/_check_imaging_parameters.py
+src/astroviper/_domain/_imaging/_fft.py
 src/astroviper/_domain/_imaging/_fft_norm_img_xds.py
+src/astroviper/_domain/_imaging/_ifft.py
 src/astroviper/_domain/_imaging/_make_aperture_grid.py
 src/astroviper/_domain/_imaging/_make_gridding_convolution_function.py
 src/astroviper/_domain/_imaging/_make_image.py
 src/astroviper/_domain/_imaging/_make_imaging_weights.py
 src/astroviper/_domain/_imaging/_make_uv_sampling_grid.py
 src/astroviper/_domain/_imaging/_make_visibility_grid.py
 src/astroviper/_domain/_imaging/_imaging_utils/_make_pb_symmetric.py
```

