# Comparing `tmp/o2sclpy-0.928.tar.gz` & `tmp/o2sclpy-0.929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "o2sclpy-0.928.tar", last modified: Tue Jul 18 05:21:58 2023, max compression
+gzip compressed data, was "o2sclpy-0.929.tar", last modified: Fri May 10 15:35:41 2024, max compression
```

## Comparing `o2sclpy-0.928.tar` & `o2sclpy-0.929.tar`

### file list

```diff
@@ -1,36 +1,53 @@
-drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.762675 o2sclpy-0.928/
--rw-r--r--   0 awsteiner2   (502) staff       (20)    35141 2023-05-23 14:43:12.000000 o2sclpy-0.928/LICENSE
--rw-r--r--   0 awsteiner2   (502) staff       (20)       16 2023-05-23 14:43:12.000000 o2sclpy-0.928/MANIFEST.in
--rw-r--r--   0 awsteiner2   (502) staff       (20)      618 2023-07-18 05:21:58.762190 o2sclpy-0.928/PKG-INFO
--rw-r--r--   0 awsteiner2   (502) staff       (20)      113 2023-05-23 14:43:12.000000 o2sclpy-0.928/README.md
-drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.726865 o2sclpy-0.928/bin/
--rwxr-xr-x   0 awsteiner2   (502) staff       (20)     1244 2023-07-09 04:54:59.000000 o2sclpy-0.928/bin/o2graph
-drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.757562 o2sclpy-0.928/o2sclpy/
--rw-r--r--   0 awsteiner2   (502) staff       (20)     4434 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/__init__.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)   280045 2023-07-14 04:26:24.000000 o2sclpy-0.928/o2sclpy/base.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)     2562 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/cap_cout.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)     2054 2023-07-17 04:23:20.000000 o2sclpy-0.928/o2sclpy/doc_data.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)   132582 2023-07-14 04:26:27.000000 o2sclpy-0.928/o2sclpy/eos.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    21774 2023-07-09 05:04:03.000000 o2sclpy-0.928/o2sclpy/gmm.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    68275 2023-07-14 04:26:25.000000 o2sclpy-0.928/o2sclpy/hdf.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)     7022 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/hdf_add.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    16357 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/interpm.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    11217 2023-07-09 04:58:47.000000 o2sclpy-0.928/o2sclpy/kde.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    13264 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/link_o2scl.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    61878 2023-07-14 04:26:26.000000 o2sclpy-0.928/o2sclpy/nuclei.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)   230878 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/o2graph_plotter.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    78526 2023-07-14 04:26:25.000000 o2sclpy-0.928/o2sclpy/other.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    76508 2023-07-14 04:26:26.000000 o2sclpy-0.928/o2sclpy/part.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    95211 2023-07-10 18:55:03.000000 o2sclpy-0.928/o2sclpy/plot_base.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    21777 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/plot_info.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    30657 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/utils.py
--rw-r--r--   0 awsteiner2   (502) staff       (20)    33623 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/yt_plot_base.py
-drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.761493 o2sclpy-0.928/o2sclpy.egg-info/
--rw-r--r--   0 awsteiner2   (502) staff       (20)      618 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/PKG-INFO
--rw-r--r--   0 awsteiner2   (502) staff       (20)      591 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/SOURCES.txt
--rw-r--r--   0 awsteiner2   (502) staff       (20)        1 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/dependency_links.txt
--rw-r--r--   0 awsteiner2   (502) staff       (20)        1 2023-06-06 03:54:51.000000 o2sclpy-0.928/o2sclpy.egg-info/not-zip-safe
--rw-r--r--   0 awsteiner2   (502) staff       (20)       36 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/requires.txt
--rw-r--r--   0 awsteiner2   (502) staff       (20)        8 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/top_level.txt
--rw-r--r--   0 awsteiner2   (502) staff       (20)       38 2023-07-18 05:21:58.762861 o2sclpy-0.928/setup.cfg
--rw-r--r--   0 awsteiner2   (502) staff       (20)     1090 2023-07-17 04:23:20.000000 o2sclpy-0.928/setup.py
+drwxrwxr-x   0 awsteiner  (1000) awsteiner  (1000)        0 2024-05-10 15:35:41.332153 o2sclpy-0.929/
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    35141 2024-04-04 21:48:53.000000 o2sclpy-0.929/LICENSE
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)       16 2024-04-04 21:48:53.000000 o2sclpy-0.929/MANIFEST.in
+-rw-r--r--   0 awsteiner  (1000) awsteiner  (1000)    41473 2024-05-10 15:35:41.331153 o2sclpy-0.929/PKG-INFO
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)      106 2024-05-01 17:45:24.000000 o2sclpy-0.929/README.md
+drwxrwxr-x   0 awsteiner  (1000) awsteiner  (1000)        0 2024-05-10 15:35:41.316153 o2sclpy-0.929/bin/
+-rwxrwxr-x   0 awsteiner  (1000) awsteiner  (1000)     1244 2024-04-04 21:48:53.000000 o2sclpy-0.929/bin/o2graph
+drwxrwxr-x   0 awsteiner  (1000) awsteiner  (1000)        0 2024-05-10 15:35:41.329153 o2sclpy-0.929/o2sclpy/
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     4440 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/__init__.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)   279023 2024-05-08 18:25:45.000000 o2sclpy-0.929/o2sclpy/base.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     3382 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/bl_gltf_import.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     6571 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/bl_gltf_six.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     3013 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/bl_gltf_yaw.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     2562 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/cap_cout.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     2641 2024-05-08 17:41:11.000000 o2sclpy-0.929/o2sclpy/doc_data.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)   143559 2024-05-08 18:25:46.000000 o2sclpy-0.929/o2sclpy/eos.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    21774 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/gmm.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    68254 2024-05-08 18:25:46.000000 o2sclpy-0.929/o2sclpy/hdf.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    16942 2024-05-08 17:41:11.000000 o2sclpy-0.929/o2sclpy/interpm.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    11156 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/kde.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    13257 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/link_o2scl.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    61518 2024-05-08 18:25:46.000000 o2sclpy-0.929/o2sclpy/nuclei.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     1304 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/o2graph.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)   260897 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/o2graph_plotter.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    83300 2024-05-08 18:25:46.000000 o2sclpy-0.929/o2sclpy/other.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    64828 2024-05-08 18:25:46.000000 o2sclpy-0.929/o2sclpy/part.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)   102608 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/plot_base.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    23579 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/plot_info.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    98190 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/td_plot_base.py
+drwxrwxr-x   0 awsteiner  (1000) awsteiner  (1000)        0 2024-05-10 15:35:41.331153 o2sclpy-0.929/o2sclpy/test/
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     6924 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_cpp_class.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     3660 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_den_plot.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     4682 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_gmm.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     2553 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_interpm.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     6395 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_kde.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     1431 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_lib_settings.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     4218 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_table.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     2516 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_table3d.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     2814 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_table_units.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     3114 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_tensor.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     4233 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_tensor_grid.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     2080 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/test/test_ug.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    57098 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/utils.py
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)    37025 2024-05-01 17:45:24.000000 o2sclpy-0.929/o2sclpy/yt_plot_base.py
+drwxrwxr-x   0 awsteiner  (1000) awsteiner  (1000)        0 2024-05-10 15:35:41.331153 o2sclpy-0.929/o2sclpy.egg-info/
+-rw-r--r--   0 awsteiner  (1000) awsteiner  (1000)    41473 2024-05-10 15:35:41.000000 o2sclpy-0.929/o2sclpy.egg-info/PKG-INFO
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)     1045 2024-05-10 15:35:41.000000 o2sclpy-0.929/o2sclpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)        1 2024-05-10 15:35:41.000000 o2sclpy-0.929/o2sclpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)       52 2024-05-10 15:35:41.000000 o2sclpy-0.929/o2sclpy.egg-info/entry_points.txt
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)       62 2024-05-10 15:35:41.000000 o2sclpy-0.929/o2sclpy.egg-info/requires.txt
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)        8 2024-05-10 15:35:41.000000 o2sclpy-0.929/o2sclpy.egg-info/top_level.txt
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)      791 2024-05-08 17:41:11.000000 o2sclpy-0.929/pyproject.toml
+-rw-rw-r--   0 awsteiner  (1000) awsteiner  (1000)       38 2024-05-10 15:35:41.332153 o2sclpy-0.929/setup.cfg
```

### Comparing `o2sclpy-0.928/LICENSE` & `o2sclpy-0.929/LICENSE`

 * *Files identical despite different names*

### Comparing `o2sclpy-0.928/bin/o2graph` & `o2sclpy-0.929/bin/o2graph`

 * *Files identical despite different names*

### Comparing `o2sclpy-0.928/o2sclpy/__init__.py` & `o2sclpy-0.929/o2sclpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2023, Andrew W. Steiner
+#  Copyright (C) 2006-2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -25,23 +25,23 @@
 # and plotting of HDF5 files (especially those generated by O2scl).
 #
 
 from o2sclpy.doc_data import *
 from o2sclpy.link_o2scl import *
 from o2sclpy.utils import *
 from o2sclpy.plot_base import *
+from o2sclpy.td_plot_base import *
 from o2sclpy.yt_plot_base import *
 from o2sclpy.o2graph_plotter import *
 from o2sclpy.plot_info import *
 from o2sclpy.base import *
 from o2sclpy.part import *
 from o2sclpy.nuclei import *
 from o2sclpy.eos import *
 from o2sclpy.hdf import *
-from o2sclpy.hdf_add import *
 from o2sclpy.other import *
 from o2sclpy.cap_cout import *
 from o2sclpy.interpm import *
 from o2sclpy.gmm import *
 from o2sclpy.kde import *
 
 """
@@ -92,11 +92,11 @@
               * Ensure the 'clf' command clears the yt objects?
               * New yt_path option to move along a path determined by
                 an o2scl table object?
               * Anti-alias text objects in yt (also anti-alias line 
                 sources?)
     """
 
-    def empty_class():
+    def empty_class(x):
         print(' ')
```

### Comparing `o2sclpy-0.928/o2sclpy/base.py` & `o2sclpy-0.929/o2sclpy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
   ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2023, Andrew W. Steiner
+  Copyright (C) 2020-2024, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -1615,15 +1615,15 @@
         ret=self.real()+self.imag()*1j
         return ret
 
 class lib_settings_class:
     """
     Python interface for O₂scl class ``lib_settings_class``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/lib_settings_class.html .
+    https://awsteiner.org/code/o2scl/html/class/lib_settings_class.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -1747,24 +1747,14 @@
         """
         func=self._link.o2scl.o2scl_lib_settings_class_ncurses_support
         func.restype=ctypes.c_bool
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
-    def gsl2_support(self):
-        """
-        | Returns: a Python boolean
-        """
-        func=self._link.o2scl.o2scl_lib_settings_class_gsl2_support
-        func.restype=ctypes.c_bool
-        func.argtypes=[ctypes.c_void_p]
-        ret=func(self._ptr)
-        return ret
-
     def armadillo_support(self):
         """
         | Returns: a Python boolean
         """
         func=self._link.o2scl.o2scl_lib_settings_class_armadillo_support
         func.restype=ctypes.c_bool
         func.argtypes=[ctypes.c_void_p]
@@ -1877,17 +1867,17 @@
         ret=func(self._ptr)
         ret2=convert_units(self._link,ret)
         return ret2
 
 
 class table:
     """
-    Python interface for O\ :sub:`2`\ scl class ``table``,
+    Python interface for O2scl class ``table``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/table.html .
+    https://awsteiner.org/code/o2scl/html/class/table.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -2735,17 +2725,17 @@
         for i in range(0,self.get_ncolumns()):
             dct[self.get_column_name(i)]=self.get(self.get_column_name(i),
                                                   row)
         return dct
 
 class table_units(table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``table_units``,
+    Python interface for O2scl class ``table_units``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/table_units.html .
+    https://awsteiner.org/code/o2scl/html/class/table_units.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class table_units
 
         | Parameters:
@@ -2866,17 +2856,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_bool]
         ret=func(self._ptr,col_,unit_,err_on_fail)
         return ret
 
 
 class uniform_grid:
     """
-    Python interface for O\ :sub:`2`\ scl class ``uniform_grid``,
+    Python interface for O2scl class ``uniform_grid``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid.html .
+    https://awsteiner.org/code/o2scl/html/class/uniform_grid.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -3015,17 +3005,17 @@
         ret=numpy.zeros((self.get_npoints()))
         for i in range(0,self.get_npoints()):
             ret[i]=v[i]
         return ret
 
 class uniform_grid_end(uniform_grid):
     """
-    Python interface for O\ :sub:`2`\ scl class ``uniform_grid_end``,
+    Python interface for O2scl class ``uniform_grid_end``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid_end.html .
+    https://awsteiner.org/code/o2scl/html/class/uniform_grid_end.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class uniform_grid_end
 
         | Parameters:
@@ -3081,17 +3071,17 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_size_t]
         return cls(link,f(start,end,n_bins))
 
 
 class uniform_grid_width(uniform_grid):
     """
-    Python interface for O\ :sub:`2`\ scl class ``uniform_grid_width``,
+    Python interface for O2scl class ``uniform_grid_width``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid_width.html .
+    https://awsteiner.org/code/o2scl/html/class/uniform_grid_width.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class uniform_grid_width
 
         | Parameters:
@@ -3147,17 +3137,17 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_size_t]
         return cls(link,f(start,width,n_bins))
 
 
 class uniform_grid_end_width(uniform_grid):
     """
-    Python interface for O\ :sub:`2`\ scl class ``uniform_grid_end_width``,
+    Python interface for O2scl class ``uniform_grid_end_width``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid_end_width.html .
+    https://awsteiner.org/code/o2scl/html/class/uniform_grid_end_width.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class uniform_grid_end_width
 
         | Parameters:
@@ -3213,17 +3203,17 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_double]
         return cls(link,f(start,end,width))
 
 
 class uniform_grid_log_end(uniform_grid):
     """
-    Python interface for O\ :sub:`2`\ scl class ``uniform_grid_log_end``,
+    Python interface for O2scl class ``uniform_grid_log_end``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid_log_end.html .
+    https://awsteiner.org/code/o2scl/html/class/uniform_grid_log_end.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class uniform_grid_log_end
 
         | Parameters:
@@ -3279,17 +3269,17 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_size_t]
         return cls(link,f(start,end,n_bins))
 
 
 class uniform_grid_log_width(uniform_grid):
     """
-    Python interface for O\ :sub:`2`\ scl class ``uniform_grid_log_width``,
+    Python interface for O2scl class ``uniform_grid_log_width``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid_log_width.html .
+    https://awsteiner.org/code/o2scl/html/class/uniform_grid_log_width.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class uniform_grid_log_width
 
         | Parameters:
@@ -3345,17 +3335,17 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_size_t]
         return cls(link,f(start,width,n_bins))
 
 
 class uniform_grid_log_end_width(uniform_grid):
     """
-    Python interface for O\ :sub:`2`\ scl class ``uniform_grid_log_end_width``,
+    Python interface for O2scl class ``uniform_grid_log_end_width``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid_log_end_width.html .
+    https://awsteiner.org/code/o2scl/html/class/uniform_grid_log_end_width.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class uniform_grid_log_end_width
 
         | Parameters:
@@ -3413,15 +3403,15 @@
         return cls(link,f(start,end,width))
 
 
 class table3d:
     """
     Python interface for O₂scl class ``table3d``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/table3d.html .
+    https://awsteiner.org/code/o2scl/html/class/table3d.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4049,15 +4039,15 @@
         return
 
 
 class index_spec:
     """
     Python interface for O₂scl class ``index_spec``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/index_spec.html .
+    https://awsteiner.org/code/o2scl/html/class/index_spec.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4246,15 +4236,15 @@
         return
 
 
 class ix_index:
     """
     Python interface for O₂scl class ``ix_index``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_index.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_index.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4318,15 +4308,15 @@
         return cls(link,f(ix))
 
 
 class ix_fixed:
     """
     Python interface for O₂scl class ``ix_fixed``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_fixed.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_fixed.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4390,15 +4380,15 @@
         return cls(link,f(ix,ix2))
 
 
 class ix_sum:
     """
     Python interface for O₂scl class ``ix_sum``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_sum.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_sum.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4462,15 +4452,15 @@
         return cls(link,f(ix))
 
 
 class ix_trace:
     """
     Python interface for O₂scl class ``ix_trace``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_trace.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_trace.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4534,15 +4524,15 @@
         return cls(link,f(ix,ix2))
 
 
 class ix_reverse:
     """
     Python interface for O₂scl class ``ix_reverse``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_reverse.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_reverse.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4606,15 +4596,15 @@
         return cls(link,f(ix))
 
 
 class ix_range:
     """
     Python interface for O₂scl class ``ix_range``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_range.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_range.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4678,15 +4668,15 @@
         return cls(link,f(ix,start,end))
 
 
 class ix_interp:
     """
     Python interface for O₂scl class ``ix_interp``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_interp.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_interp.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4750,15 +4740,15 @@
         return cls(link,f(ix,v))
 
 
 class ix_grid:
     """
     Python interface for O₂scl class ``ix_grid``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_grid.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_grid.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4822,15 +4812,15 @@
         return cls(link,f(ix,start,end,n_bins,log))
 
 
 class ix_gridw:
     """
     Python interface for O₂scl class ``ix_gridw``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/ix_gridw.html .
+    https://awsteiner.org/code/o2scl/html/class/ix_gridw.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -4892,17 +4882,17 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t,ctypes.c_double,ctypes.c_double,ctypes.c_double,ctypes.c_bool]
         return cls(link,f(ix,start,end,width,log))
 
 
 class tensor:
     """
-    Python interface for O\ :sub:`2`\ scl class ``tensor``,
+    Python interface for O2scl class ``tensor``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/tensor.html .
+    https://awsteiner.org/code/o2scl/html/class/tensor.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -5311,17 +5301,17 @@
         svst=std_vector_size_t(self._link)
         svst.init_py(index)
         self.resize_vector(len(svst),svst)
         return
 
 class tensor_int:
     """
-    Python interface for O\ :sub:`2`\ scl class ``tensor``,
+    Python interface for O2scl class ``tensor``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/tensor.html .
+    https://awsteiner.org/code/o2scl/html/class/tensor.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -5708,17 +5698,17 @@
         svst=std_vector_size_t(self._link)
         svst.init_py(index)
         self.resize_vector(svst)
         return
 
 class tensor_size_t:
     """
-    Python interface for O\ :sub:`2`\ scl class ``tensor``,
+    Python interface for O2scl class ``tensor``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/tensor.html .
+    https://awsteiner.org/code/o2scl/html/class/tensor.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -6082,17 +6072,17 @@
         svst=std_vector_size_t(self._link)
         svst.init_py(index)
         self.resize_vector(svst)
         return
 
 class tensor_grid(tensor):
     """
-    Python interface for O\ :sub:`2`\ scl class ``tensor_grid``,
+    Python interface for O2scl class ``tensor_grid``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/tensor_grid.html .
+    https://awsteiner.org/code/o2scl/html/class/tensor_grid.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class tensor_grid
 
         | Parameters:
@@ -6470,15 +6460,15 @@
         self.resize_vector(len(svst),svst)
         return
 
 class find_constants_const_entry:
     """
     Python interface for O₂scl class ``find_constants<>::const_entry``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/find_constants<>::const_entry.html .
+    https://awsteiner.org/code/o2scl/html/class/find_constants<>::const_entry.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -6767,15 +6757,15 @@
         return
 
 
 class find_constants:
     """
     Python interface for O₂scl class ``find_constants<>``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/find_constants<>.html .
+    https://awsteiner.org/code/o2scl/html/class/find_constants<>.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -6855,15 +6845,15 @@
         return
 
 
 class convert_units_der_unit:
     """
     Python interface for O₂scl class ``convert_units<>::der_unit``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/convert_units<>::der_unit.html .
+    https://awsteiner.org/code/o2scl/html/class/convert_units<>::der_unit.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -7130,17 +7120,17 @@
         self.A=A
         self.mol=mol
         self.cd=cd
         return
 
 class convert_units:
     """
-    Python interface for O\ :sub:`2`\ scl class ``convert_units``,
+    Python interface for O2scl class ``convert_units``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/convert_units.html .
+    https://awsteiner.org/code/o2scl/html/class/convert_units.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -7415,15 +7405,15 @@
         self.add_unit_internal(du)
         return
 
 class columnify:
     """
     Python interface for O₂scl class ``columnify``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/columnify.html .
+    https://awsteiner.org/code/o2scl/html/class/columnify.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -7532,15 +7522,15 @@
         return func(self._ptr)
 
 
 class format_float:
     """
     Python interface for O₂scl class ``format_float``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/format_float.html .
+    https://awsteiner.org/code/o2scl/html/class/format_float.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -7680,15 +7670,15 @@
         return strt.to_bytes()
 
 
 class interp_vec:
     """
     Python interface for O₂scl class ``interp_vec<std::vector<double>>``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/interp_vec<std::vector<double>>.html .
+    https://awsteiner.org/code/o2scl/html/class/interp_vec<std::vector<double>>.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -7807,15 +7797,15 @@
         return ret
 
 
 class interp_krige_optim_rbf_noise:
     """
     Python interface for O₂scl class ``interp_krige_optim<std::vector<double>,std::vector<double>,covar_funct_rbf_noise>``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/interp_krige_optim<std::vector<double>,std::vector<double>,covar_funct_rbf_noise>.html .
+    https://awsteiner.org/code/o2scl/html/class/interp_krige_optim<std::vector<double>,std::vector<double>,covar_funct_rbf_noise>.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -8017,15 +8007,15 @@
         return
 
 
 class terminal:
     """
     Python interface for O₂scl class ``terminal``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/terminal.html .
+    https://awsteiner.org/code/o2scl/html/class/terminal.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -8401,15 +8391,15 @@
         return strt.to_bytes()
 
 
 class gen_test_number:
     """
     Python interface for O₂scl class ``gen_test_number<double>``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/gen_test_number<double>.html .
+    https://awsteiner.org/code/o2scl/html/class/gen_test_number<double>.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -8486,15 +8476,15 @@
         return ret
 
 
 class funct_string:
     """
     Python interface for O₂scl class ``funct_string``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/funct_string.html .
+    https://awsteiner.org/code/o2scl/html/class/funct_string.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -8583,15 +8573,15 @@
         return cls(link,f(expr_,var_))
 
 
 class comm_option_s:
     """
     Python interface for O₂scl class ``comm_option_s``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/comm_option_s.html .
+    https://awsteiner.org/code/o2scl/html/class/comm_option_s.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -8800,15 +8790,15 @@
         return
 
 
 class cmd_line_arg:
     """
     Python interface for O₂scl class ``cmd_line_arg``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/cmd_line_arg.html .
+    https://awsteiner.org/code/o2scl/html/class/cmd_line_arg.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -8937,15 +8927,15 @@
         return
 
 
 class cli:
     """
     Python interface for O₂scl class ``cli``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/cli.html .
+    https://awsteiner.org/code/o2scl/html/class/cli.html .
     
     """
 
     _ptr=0
     _link=0
     _owner=True
 
@@ -9306,44 +9296,38 @@
     func.restype=ctypes.c_void_p
     func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int,ctypes.c_bool]
     ret=func(t._ptr,spec_,verbose,err_on_fail)
     ten=tensor_grid(link,ret)
     ten._owner=True
     return ten
 
-def fermi_function(link,E,mu,T,limit=40.0):
+def fermi_function(link,x):
     """
         | Parameters:
         | *link* :class:`linker` object
-        | *E*: ``double``
-        | *mu*: ``double``
-        | *T*: ``double``
-        | *limit*: ``double``
+        | *x*: ``double``
         | Returns: ``ctypes.c_double`` object
     """
     func=link.o2scl.o2scl_fermi_function_wrapper
     func.restype=ctypes.c_double
-    func.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_double,ctypes.c_double]
-    ret=func(E,mu,T,limit)
+    func.argtypes=[ctypes.c_double]
+    ret=func(x)
     return ret
 
-def bose_function(link,E,mu,T,limit=40.0):
+def bose_function(link,x):
     """
         | Parameters:
         | *link* :class:`linker` object
-        | *E*: ``double``
-        | *mu*: ``double``
-        | *T*: ``double``
-        | *limit*: ``double``
+        | *x*: ``double``
         | Returns: ``ctypes.c_double`` object
     """
     func=link.o2scl.o2scl_bose_function_wrapper
     func.restype=ctypes.c_double
-    func.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_double,ctypes.c_double]
-    ret=func(E,mu,T,limit)
+    func.argtypes=[ctypes.c_double]
+    ret=func(x)
     return ret
 
 def quadratic_extremum_x(link,x1,x2,x3,y1,y2,y3):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *x1*: ``double``
```

### Comparing `o2sclpy-0.928/o2sclpy/cap_cout.py` & `o2sclpy-0.929/o2sclpy/cap_cout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2023, Andrew W. Steiner
+#  Copyright (C) 2006-2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
```

### Comparing `o2sclpy-0.928/o2sclpy/doc_data.py` & `o2sclpy-0.929/o2sclpy/doc_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 from o2sclpy.utils import terminal_py
 
 ter=terminal_py()
 
-version='0.928'
+version='0.929'
 
-cmaps=[('Perceptually Uniform Sequential',
-        ['viridis','plasma','inferno','magma']),
-       ('Sequential', 
-        ['Greys','Purples','Blues','Greens','Oranges','Reds',
-         'YlOrBr','YlOrRd','OrRd','PuRd','RdPu','BuPu',
-         'GnBu','PuBu','YlGnBu','PuBuGn','BuGn','YlGn']),
-       ('Sequential (2)', 
-        ['binary','gist_yarg','gist_gray','gray','bone','pink',
-         'spring','summer','autumn','winter','cool','Wistia',
-         'hot','afmhot','gist_heat','copper']),
-       ('Diverging', 
-        ['PiYG','PRGn','BrBG','PuOr','RdGy','RdBu',
-         'RdYlBu','RdYlGn','Spectral','coolwarm','bwr','seismic']),
-       ('Qualitative', 
-        ['Pastel1','Pastel2','Paired','Accent',
-         'Dark2','Set1','Set2','Set3',
-         'tab10','tab20','tab20b','tab20c']),
-       ('Miscellaneous', 
-        ['flag','prism','ocean','gist_earth','terrain','gist_stern',
-         'gnuplot','gnuplot2','CMRmap','cubehelix','brg','hsv',
-         'gist_rainbow','rainbow','jet','nipy_spectral','gist_ncar'])]
+cmaps = [('Perceptually uniform sequential', [
+            'viridis', 'plasma', 'inferno', 'magma', 'cividis']),
+         ('Sequential', [
+            'Greys', 'Purples', 'Blues', 'Greens', 'Oranges', 'Reds',
+            'YlOrBr', 'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu',
+            'GnBu', 'PuBu', 'YlGnBu', 'PuBuGn', 'BuGn', 'YlGn']),
+         ('Sequential (2)', [
+            'binary', 'gist_yarg', 'gist_gray', 'gray', 'bone', 'pink',
+            'spring', 'summer', 'autumn', 'winter', 'cool', 'Wistia',
+            'hot', 'afmhot', 'gist_heat', 'copper']),
+         ('Diverging', [
+            'PiYG', 'PRGn', 'BrBG', 'PuOr', 'RdGy', 'RdBu',
+            'RdYlBu', 'RdYlGn', 'Spectral', 'coolwarm', 'bwr', 'seismic']),
+         ('Cyclic', ['twilight', 'twilight_shifted', 'hsv']),
+         ('Qualitative', [
+            'Pastel1', 'Pastel2', 'Paired', 'Accent',
+            'Dark2', 'Set1', 'Set2', 'Set3',
+            'tab10', 'tab20', 'tab20b', 'tab20c']),
+         ('Miscellaneous', [
+            'flag', 'prism', 'ocean', 'gist_earth', 'terrain', 'gist_stern',
+            'gnuplot', 'gnuplot2', 'CMRmap', 'cubehelix', 'brg',
+            'gist_rainbow', 'rainbow', 'jet', 'turbo', 'nipy_spectral',
+            'gist_ncar'])]
+"""
+List of cmaps for 'help cmaps'
+"""
+
+yt_cmaps=[('Perceptually uniform sequential (yt)',
+        ['cmyt.apricity','cmyt.arbre','cmyt.dusk','cmyt.kelp',
+         'cmyt.octarine']),
+       ('Monochromatic sequential (yt)', 
+        ['cmyt.pixel_blue','cmyt.pixel_green','cmyt.pixel_red']),
+       ('Miscellaneous (yt)', 
+        ['cmyt.algae','cmyt.pastel','cmyt.xray'])]
 """
 List of cmaps for 'help cmaps'
 """
 
 new_cmaps=[('O2sclpy cmaps',
             ['jet2','pastel2','reds2','greens2','blues2'])]
 """
```

### Comparing `o2sclpy-0.928/o2sclpy/eos.py` & `o2sclpy-0.929/o2sclpy/eos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
   ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2023, Andrew W. Steiner
+  Copyright (C) 2020-2024, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -26,17 +26,17 @@
 from o2sclpy.utils import force_bytes
 
 from o2sclpy.base import *
 from o2sclpy.part import *
 
 class eos_base:
     """
-    Python interface for O2scl class eos_base.
+    Python interface for O2scl class ``eos_base``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_base.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_base.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -100,19 +100,416 @@
         """
         func=self._link.o2scl.o2scl_eos_base_set_def_thermo
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,value._ptr)
         return
 
 
+class eos_leptons:
+    """
+    Python interface for O2scl class ``eos_leptons``.
+    See
+    https://awsteiner.org/code/o2scl/html/class/eos_leptons.html .
+    """
+
+    _ptr=0
+    _link=0
+    _owner=True
+
+    def __init__(self,link,pointer=0):
+        """
+        Init function for class eos_leptons
+
+        | Parameters:
+        | *link* :class:`linker` object
+        | *pointer* ``ctypes.c_void_p`` pointer
+
+        """
+
+        if pointer==0:
+            f=link.o2scl.o2scl_create_eos_leptons
+            f.restype=ctypes.c_void_p
+            f.argtypes=[]
+            self._ptr=f()
+        else:
+            self._ptr=pointer
+            self._owner=False
+        self._link=link
+        return
+
+    def __del__(self):
+        """
+        Delete function for class eos_leptons
+        """
+
+        if self._owner==True:
+            f=self._link.o2scl.o2scl_free_eos_leptons
+            f.argtypes=[ctypes.c_void_p]
+            f(self._ptr)
+            self._owner=False
+            self._ptr=0
+        return
+
+    def __copy__(self):
+        """
+        Shallow copy function for class eos_leptons
+        
+        Returns: eos_leptons object
+        """
+
+        new_obj=type(self)(self._link,self._ptr)
+        return new_obj
+
+    def get_th(self):
+        """
+        Get object of type :class:`o2scl::thermo`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_th
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=thermo(self._link,ptr)
+        return obj
+
+    def set_th(self,value):
+        """
+        Set object of type :class:`o2scl::thermo`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_th
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_e(self):
+        """
+        Get object of type :class:`o2scl::fermion`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_e
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=fermion(self._link,ptr)
+        return obj
+
+    def set_e(self,value):
+        """
+        Set object of type :class:`o2scl::fermion`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_e
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_mu(self):
+        """
+        Get object of type :class:`o2scl::fermion`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_mu
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=fermion(self._link,ptr)
+        return obj
+
+    def set_mu(self,value):
+        """
+        Set object of type :class:`o2scl::fermion`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_mu
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_ph(self):
+        """
+        Get object of type :class:`o2scl::boson`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_ph
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=boson(self._link,ptr)
+        return obj
+
+    def set_ph(self,value):
+        """
+        Set object of type :class:`o2scl::boson`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_ph
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_ed(self):
+        """
+        Get object of type :class:`o2scl::part_deriv_press`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_ed
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=part_deriv_press(self._link,ptr)
+        return obj
+
+    def set_ed(self,value):
+        """
+        Set object of type :class:`o2scl::part_deriv_press`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_ed
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_mud(self):
+        """
+        Get object of type :class:`o2scl::part_deriv_press`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_mud
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=part_deriv_press(self._link,ptr)
+        return obj
+
+    def set_mud(self,value):
+        """
+        Set object of type :class:`o2scl::part_deriv_press`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_mud
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_phd(self):
+        """
+        Get object of type :class:`o2scl::part_deriv_press`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_phd
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=part_deriv_press(self._link,ptr)
+        return obj
+
+    def set_phd(self,value):
+        """
+        Set object of type :class:`o2scl::part_deriv_press`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_phd
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    @property
+    def include_muons(self):
+        """
+        Property of type ``ctypes.c_bool``
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_get_include_muons
+        func.restype=ctypes.c_bool
+        func.argtypes=[ctypes.c_void_p]
+        return func(self._ptr)
+
+    @include_muons.setter
+    def include_muons(self,value):
+        """
+        Setter function for eos_leptons::include_muons .
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_include_muons
+        func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
+        func(self._ptr,value)
+        return
+
+    @property
+    def include_deriv(self):
+        """
+        Property of type ``ctypes.c_bool``
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_get_include_deriv
+        func.restype=ctypes.c_bool
+        func.argtypes=[ctypes.c_void_p]
+        return func(self._ptr)
+
+    @include_deriv.setter
+    def include_deriv(self,value):
+        """
+        Setter function for eos_leptons::include_deriv .
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_include_deriv
+        func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
+        func(self._ptr,value)
+        return
+
+    @property
+    def pde_from_density(self):
+        """
+        Property of type ``ctypes.c_bool``
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_get_pde_from_density
+        func.restype=ctypes.c_bool
+        func.argtypes=[ctypes.c_void_p]
+        return func(self._ptr)
+
+    @pde_from_density.setter
+    def pde_from_density(self,value):
+        """
+        Setter function for eos_leptons::pde_from_density .
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_pde_from_density
+        func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
+        func(self._ptr,value)
+        return
+
+    @property
+    def verbose(self):
+        """
+        Property of type ``ctypes.c_int``
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_get_verbose
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p]
+        return func(self._ptr)
+
+    @verbose.setter
+    def verbose(self,value):
+        """
+        Setter function for eos_leptons::verbose .
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_verbose
+        func.argtypes=[ctypes.c_void_p,ctypes.c_int]
+        func(self._ptr,value)
+        return
+
+    @property
+    def err_nonconv(self):
+        """
+        Property of type ``ctypes.c_bool``
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_get_err_nonconv
+        func.restype=ctypes.c_bool
+        func.argtypes=[ctypes.c_void_p]
+        return func(self._ptr)
+
+    @err_nonconv.setter
+    def err_nonconv(self,value):
+        """
+        Setter function for eos_leptons::err_nonconv .
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_err_nonconv
+        func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
+        func(self._ptr,value)
+        return
+
+    def get_frel(self):
+        """
+        Get object of type :class:`o2scl::fermion_rel`
+        """
+        func1=self._link.o2scl.o2scl_eos_leptons_get_frel
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=fermion_rel(self._link,ptr)
+        return obj
+
+    def set_frel(self,value):
+        """
+        Set object of type :class:`o2scl::fermion_rel`
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_set_frel
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def default_acc(self):
+        """
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_default_acc
+        func.argtypes=[ctypes.c_void_p]
+        func(self._ptr)
+        return
+
+    def improved_acc(self):
+        """
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_improved_acc
+        func.argtypes=[ctypes.c_void_p]
+        func(self._ptr)
+        return
+
+    def ld_acc(self):
+        """
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_ld_acc
+        func.argtypes=[ctypes.c_void_p]
+        func(self._ptr)
+        return
+
+    def fp_25_acc(self):
+        """
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_fp_25_acc
+        func.argtypes=[ctypes.c_void_p]
+        func(self._ptr)
+        return
+
+    def pair_mu(self,T):
+        """
+        | Parameters:
+        | *T*: ``double``
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_pair_mu
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        ret=func(self._ptr,T)
+        return ret
+
+    def pair_mu_eq(self,T):
+        """
+        | Parameters:
+        | *T*: ``double``
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_pair_mu_eq
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        ret=func(self._ptr,T)
+        return ret
+
+    def pair_density(self,T):
+        """
+        | Parameters:
+        | *T*: ``double``
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_pair_density
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        ret=func(self._ptr,T)
+        return ret
+
+    def pair_density_eq(self,nq,T):
+        """
+        | Parameters:
+        | *nq*: ``double``
+        | *T*: ``double``
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_eos_leptons_pair_density_eq
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
+        ret=func(self._ptr,nq,T)
+        return ret
+
+
 class eos_had_base(eos_base):
     """
-    Python interface for O2scl class eos_had_base.
+    Python interface for O2scl class ``eos_had_base``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_base.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_base
 
@@ -767,17 +1164,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,nb,delta)
         return ret
 
 
 class eos_had_eden_base(eos_had_base):
     """
-    Python interface for O2scl class eos_had_eden_base.
+    Python interface for O2scl class ``eos_had_eden_base``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_eden_base.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_eden_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_eden_base
 
@@ -820,17 +1217,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_pres_base(eos_had_base):
     """
-    Python interface for O2scl class eos_had_pres_base.
+    Python interface for O2scl class ``eos_had_pres_base``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_pres_base.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_pres_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_pres_base
 
@@ -873,17 +1270,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_temp_base(eos_had_base):
     """
-    Python interface for O2scl class eos_had_temp_base.
+    Python interface for O2scl class ``eos_had_temp_base``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_temp_base.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_temp_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_temp_base
 
@@ -956,17 +1353,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double,ctypes.c_void_p]
         ret=func(self._ptr,n._ptr,p._ptr,T,th._ptr)
         return ret
 
 
 class eos_had_temp_eden_base(eos_had_temp_base):
     """
-    Python interface for O2scl class eos_had_temp_eden_base.
+    Python interface for O2scl class ``eos_had_temp_eden_base``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_temp_eden_base.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_temp_eden_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_temp_eden_base
 
@@ -1009,17 +1406,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_temp_pres_base(eos_had_temp_base):
     """
-    Python interface for O2scl class eos_had_temp_pres_base.
+    Python interface for O2scl class ``eos_had_temp_pres_base``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_temp_pres_base.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_temp_pres_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_temp_pres_base
 
@@ -1062,17 +1459,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_skyrme(eos_had_temp_eden_base):
     """
-    Python interface for O2scl class eos_had_skyrme.
+    Python interface for O2scl class ``eos_had_skyrme``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_skyrme.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_skyrme.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_skyrme
 
         | Parameters:
@@ -1454,17 +1851,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,value._ptr)
         return
 
 
 class eos_had_apr(eos_had_temp_eden_base):
     """
-    Python interface for O2scl class eos_had_apr.
+    Python interface for O2scl class ``eos_had_apr``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_apr.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_apr.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_apr
 
         | Parameters:
@@ -1546,17 +1943,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
         func(self._ptr,value)
         return
 
 
 class eos_had_rmf(eos_had_temp_pres_base):
     """
-    Python interface for O2scl class eos_had_rmf.
+    Python interface for O2scl class ``eos_had_rmf``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_rmf.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_had_rmf.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_rmf
 
         | Parameters:
@@ -2109,17 +2506,17 @@
         rho_conv=ctypes.c_double(rho)
         ret=func(self._ptr,ctypes.byref(sig_conv),ctypes.byref(ome_conv),ctypes.byref(rho_conv))
         return ret,sig_conv.value,ome_conv.value,rho_conv.value
 
 
 class eos_quark(eos_base):
     """
-    Python interface for O2scl class eos_quark.
+    Python interface for O2scl class ``eos_quark``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_quark.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_quark.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_quark
 
         | Parameters:
@@ -2161,17 +2558,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_quark_bag(eos_quark):
     """
-    Python interface for O2scl class eos_quark_bag.
+    Python interface for O2scl class ``eos_quark_bag``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_quark_bag.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_quark_bag.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_quark_bag
 
         | Parameters:
@@ -2233,17 +2630,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
 
 class eos_quark_njl(eos_quark):
     """
-    Python interface for O2scl class eos_quark_njl.
+    Python interface for O2scl class ``eos_quark_njl``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_quark_njl.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_quark_njl.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_quark_njl
 
         | Parameters:
@@ -2405,17 +2802,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
         func(self._ptr,value)
         return
 
 
 class eos_tov:
     """
-    Python interface for O2scl class eos_tov.
+    Python interface for O2scl class ``eos_tov``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_tov.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -2577,17 +2974,17 @@
         nb_conv=ctypes.c_double(0)
         func(self._ptr,pr,ctypes.byref(ed_conv),ctypes.byref(nb_conv))
         return ed_conv.value,nb_conv.value
 
 
 class eos_tov_buchdahl(eos_tov):
     """
-    Python interface for O2scl class eos_tov_buchdahl.
+    Python interface for O2scl class ``eos_tov_buchdahl``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_buchdahl.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_tov_buchdahl.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_buchdahl
 
         | Parameters:
@@ -2744,17 +3141,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,r,beta)
         return ret
 
 
 class eos_tov_polytrope(eos_tov):
     """
-    Python interface for O2scl class eos_tov_polytrope.
+    Python interface for O2scl class ``eos_tov_polytrope``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_polytrope.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_tov_polytrope.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_polytrope
 
         | Parameters:
@@ -2807,17 +3204,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         func(self._ptr,coeff,index)
         return
 
 
 class eos_tov_linear(eos_tov):
     """
-    Python interface for O2scl class eos_tov_linear.
+    Python interface for O2scl class ``eos_tov_linear``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_linear.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_tov_linear.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_linear
 
         | Parameters:
@@ -2870,17 +3267,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         func(self._ptr,cs2,eps0)
         return
 
 
 class eos_tov_interp(eos_tov):
     """
-    Python interface for O2scl class eos_tov_interp.
+    Python interface for O2scl class ``eos_tov_interp``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_interp.html .
+    https://awsteiner.org/code/o2scl/html/class/eos_tov_interp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_interp
 
         | Parameters:
@@ -3093,17 +3490,17 @@
         func.argtypes=[ctypes.c_void_p]
         func(self._ptr)
         return
 
 
 class tov_solve:
     """
-    Python interface for O2scl class tov_solve.
+    Python interface for O2scl class ``tov_solve``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/tov_solve.html .
+    https://awsteiner.org/code/o2scl/html/class/tov_solve.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -3795,17 +4192,17 @@
         func.argtypes=[ctypes.c_void_p]
         sp=shared_ptr_table_units(self._link,func(self._ptr))
         return sp
 
 
 class tov_love:
     """
-    Python interface for O2scl class tov_love.
+    Python interface for O2scl class ``tov_love``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/tov_love.html .
+    https://awsteiner.org/code/o2scl/html/class/tov_love.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -4041,17 +4438,17 @@
         lambda_cgs_conv=ctypes.c_double(0)
         ret=func(self._ptr,ctypes.byref(yR_conv),ctypes.byref(beta_conv),ctypes.byref(k2_conv),ctypes.byref(lambda_km5_conv),ctypes.byref(lambda_cgs_conv))
         return ret,yR_conv.value,beta_conv.value,k2_conv.value,lambda_km5_conv.value,lambda_cgs_conv.value
 
 
 class nstar_cold:
     """
-    Python interface for O2scl class nstar_cold.
+    Python interface for O2scl class ``nstar_cold``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nstar_cold.html .
+    https://awsteiner.org/code/o2scl/html/class/nstar_cold.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -4472,17 +4869,17 @@
         func.argtypes=[ctypes.c_void_p]
         sp=shared_ptr_table_units(self._link,func(self._ptr))
         return sp
 
 
 class nucleus_rmf:
     """
-    Python interface for O2scl class nucleus_rmf.
+    Python interface for O2scl class ``nucleus_rmf``.
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucleus_rmf.html .
+    https://awsteiner.org/code/o2scl/html/class/nucleus_rmf.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
```

### Comparing `o2sclpy-0.928/o2sclpy/gmm.py` & `o2sclpy-0.929/o2sclpy/gmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2023, Andrew W. Steiner
+#  Copyright (C) 2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
```

### Comparing `o2sclpy-0.928/o2sclpy/hdf.py` & `o2sclpy-0.929/o2sclpy/hdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
   ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2023, Andrew W. Steiner
+  Copyright (C) 2020-2024, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -28,15 +28,15 @@
 from o2sclpy.base import *
 from o2sclpy.other import *
 
 class hdf_file:
     """
     Python interface for O2scl class ``hdf_file``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/hdf_file.html .
+    https://awsteiner.org/code/o2scl/html/class/hdf_file.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -759,15 +759,15 @@
         return
 
 
 class acol_manager:
     """
     Python interface for O2scl class ``acol_manager``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/acol_manager.html .
+    https://awsteiner.org/code/o2scl/html/class/acol_manager.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1602,15 +1602,15 @@
         return
 
 
 class cloud_file:
     """
     Python interface for O2scl class ``cloud_file``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/cloud_file.html .
+    https://awsteiner.org/code/o2scl/html/class/cloud_file.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
```

### Comparing `o2sclpy-0.928/o2sclpy/interpm.py` & `o2sclpy-0.929/o2sclpy/interpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2022-2023, Mahamudul Hasan Anik, Satyajit Roy, and
+#  Copyright (C) 2022-2024, Mahamudul Hasan Anik, Satyajit Roy, and
 #  Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
@@ -142,42 +142,52 @@
 
         return
     
     def eval(self,v):
         """
         Evaluate the GP at point ``v``.
         """
+
+        # AWS, 3/27/24: Keep in mind that o2scl::interpm_python.eval()
+        # expects the return type to be a numpy array. 
         yp=self.gp.predict([v])
         if self.outformat=='list':
+            if self.verbose>1:
+                print('interpm_sklearn_gp::eval(): list mode type(yp),v,yp:',
+                      type(yp),v,yp)
             return yp[0].tolist()
         if yp.ndim==1:
             if self.verbose>1:
-                print('interpm_sklearn_gp::eval(): type(yp),v,yp:',
+                print('interpm_sklearn_gp::eval(): ndim=1 mode type(yp),v,yp:',
                       type(yp),v,yp)
             return numpy.ascontiguousarray(yp)
         if self.verbose>1:
-            print('interpm_sklearn_gp::eval(): type(yp[0]),v,yp[0]:',
+            print('interpm_sklearn_gp::eval(): array mode type(yp[0]),v,yp[0]:',
                   type(yp[0]),v,yp[0])
         return numpy.ascontiguousarray(yp[0])
 
     def eval_unc(self,v):
         """
         Evaluate the GP and its uncertainty at point ``v``.
+
+        # AWS, 3/27/24: Keep in mind that
+        # o2scl::interpm_python.eval_unc() expects the return type to
+        # be a tuple of numpy arrays. 
         """
         yp,std=self.gp.predict([v],return_std=True)
         if self.outformat=='list':
             return yp[0].tolist(),std[0].tolist()
         if yp.ndim==1:
             if self.verbose>1:
-                print('interpm_sklearn_gp::eval(): type(yp),v,yp:',
+                print('interpm_sklearn_gp::eval_unc(): type(yp),v,yp:',
                       type(yp),v,yp)
             return (numpy.ascontiguousarray(yp),
                     numpy.ascontiguousarray(std))
         if self.verbose>1:
-            print('interpm_sklearn_gp::eval(): type(yp[0]),v,yp[0]:',
+            print('interpm_sklearn_gp::eval_unc(): type(yp[0]),v,yp[0]:',
                   type(yp[0]),v,yp[0])
         return (numpy.ascontiguousarray(yp[0]),
                 numpy.ascontiguousarray(std[0]))
 
 class interpm_tf_dnn:
     """
     Interpolate one or many multimensional data sets using 
@@ -243,21 +253,21 @@
             dct[arr2[0]]=arr2[1]
 
         return dct
     
     def set_data(self,in_data,out_data,outformat='numpy',verbose=0,
                  activations=['relu','relu'],
                  batch_size=None,epochs=100,
-                 transform='default',test_size=0.0,evaluate=False,
+                 transform='none',test_size=0.0,evaluate=False,
                  hlayers=[8,8],loss='mean_squared_error'):
         """
         Set the input and output data to train the interpolator
 
         some activation functions: 
-        relu [0,\infty]
+        relu [0,\\infty]
         sigmoid [0,1]
         tanh [-1,1]
 
         transformations:
         quantile transforms to [0,1]
         MinMaxScaler transforms to [a,b]
         """
@@ -279,21 +289,23 @@
 
         self.outformat=outformat
         self.verbose=verbose
         self.transform=transform
 
         from sklearn.preprocessing import QuantileTransformer
         from sklearn.preprocessing import MinMaxScaler
-        if self.transform!='none':
-            if activation=='tanh':
-                self.SS1=MinMaxScaler(feature_range=(-1,1))
-                self.SS2=MinMaxScaler(feature_range=(-1,1))
-            else:
-                self.SS1=QuantileTransformer()
-                self.SS2=QuantileTransformer()
+        if self.transform=='moto':
+            self.SS1=MinMaxScaler(feature_range=(-1,1))
+            self.SS2=MinMaxScaler(feature_range=(-1,1))
+        
+            in_data_trans=self.SS1.fit_transform(in_data)
+            out_data_trans=self.SS2.fit_transform(out_data)
+        elif self.transform=='quant':
+            self.SS1=QuantileTransformer()
+            self.SS2=QuantileTransformer()
         
             in_data_trans=self.SS1.fit_transform(in_data)
             out_data_trans=self.SS2.fit_transform(out_data)
         else:
             in_data_trans=in_data
             out_data_trans=out_data
 
@@ -341,16 +353,17 @@
         if self.verbose>0:
             print('nd_in,nd_out:',nd_in,nd_out)
             print('  Training DNN model.')
             
         try:
             nl=len(hlayers)
             na=len(activations)
-            layers=[tf.keras.layers.Dense(hlayers[0],input_shape=(nd_in,),
-                                          activation=activations[0])]
+            inp=tf.keras.Input(shape=(nd_in,))
+            layers=[inp,tf.keras.layers.Dense(hlayers[0],
+                                              activation=activations[0])]
             if self.verbose>0:
                 print('Layer: dense',hlayers[0],nd_in,activations[0])
             for i in range(1,nl):
                 act=activations[i%na]
                 layers.append(tf.keras.layers.Dense(hlayers[i],
                                                     activation=act))
                 if self.verbose>0:
```

### Comparing `o2sclpy-0.928/o2sclpy/kde.py` & `o2sclpy-0.929/o2sclpy/kde.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2023, Andrew W. Steiner
+#  Copyright (C) 2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -305,16 +305,14 @@
     
     def set_data_str(self,in_data,weights,options):
         """
         Set the input and output data to train the interpolator,
         using a string to specify the keyword arguments.
         """
 
-        print('Here in kde_scipy::set_data_str().')
-        
         try:
             dct=self.string_to_dict(options)
             if self.verbose>1:
                 print('String:',options,'Dictionary:',dct)
     
             print('weights shape:',weights,numpy.shape(weights))
```

### Comparing `o2sclpy-0.928/o2sclpy/link_o2scl.py` & `o2sclpy-0.929/o2sclpy/link_o2scl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2023, Andrew W. Steiner
+#  Copyright (C) 2006-2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -55,20 +55,20 @@
     """
 
     backend=''
     """
     Backend specification from command-line
     """
 
-    o2scl_addl_libs=[]
+    o2scl_addl_libs = []
     """
     Additional library list from command-line or environment variables
     """
 
-    o2scl_addl=[]
+    o2scl_addl = []
     """
     List of additional library objects
     """
 
     verbose=0
     """
     If greater than 0, output more information about the linker.
@@ -284,15 +284,15 @@
                 
         self.backend=if_yt_then_Agg(self.backend,argv)
         
         return self.backend
 
 def build_o2scl(verbose=1,release=True):
     """
-    This function attempts to automatically build O\ :sub:`2`\ scl using 
+    This function attempts to automatically build O2scl using 
     homebrew on OSX and snap on Linux.
 
     This function is in ``link_o2scl.py``.
     """
     
     print('Would you like to try to automatically install O2scl '+
           '(requires sudo)?')
```

### Comparing `o2sclpy-0.928/o2sclpy/nuclei.py` & `o2sclpy-0.929/o2sclpy/nuclei.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
   ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2023, Andrew W. Steiner
+  Copyright (C) 2020-2024, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -25,17 +25,17 @@
 from abc import abstractmethod
 from o2sclpy.utils import force_bytes
 
 from o2sclpy.part import *
 
 class nucleus(part):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucleus``,
+    Python interface for O2scl class ``nucleus``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucleus.html .
+    https://awsteiner.org/code/o2scl/html/class/nucleus.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucleus
 
         | Parameters:
@@ -177,17 +177,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
 
 class nucmass_info:
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_info``,
+    Python interface for O2scl class ``nucmass_info``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_info.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_info.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -332,17 +332,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p]
         ret=func(self._ptr,s_)
         return ret
 
 
 class nucmass:
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass``,
+    Python interface for O2scl class ``nucmass``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -664,17 +664,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,Z,N)
         return ret
 
 
 class nucmass_table(nucmass):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_table``,
+    Python interface for O2scl class ``nucmass_table``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_table.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_table.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_table
 
@@ -777,17 +777,17 @@
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
 
 class nucmass_fit_base(nucmass):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_fit_base``,
+    Python interface for O2scl class ``nucmass_fit_base``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_fit_base.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_fit_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_fit_base
 
@@ -850,17 +850,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
         func(self._ptr,value)
         return
 
 
 class nucmass_semi_empirical(nucmass_fit_base):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_semi_empirical``,
+    Python interface for O2scl class ``nucmass_semi_empirical``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_semi_empirical.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_semi_empirical.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_semi_empirical
 
         | Parameters:
@@ -1028,17 +1028,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,Z,N)
         return ret
 
 
 class nucmass_ame(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_ame``,
+    Python interface for O2scl class ``nucmass_ame``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_ame.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_ame.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_ame
 
         | Parameters:
@@ -1080,17 +1080,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dz_table(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_dz_table``,
+    Python interface for O2scl class ``nucmass_dz_table``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dz_table.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_dz_table.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dz_table
 
         | Parameters:
@@ -1132,17 +1132,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dz_fit(nucmass_fit_base):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_dz_fit``,
+    Python interface for O2scl class ``nucmass_dz_fit``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dz_fit.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_dz_fit.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dz_fit
 
         | Parameters:
@@ -1184,17 +1184,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dz_fit_33(nucmass_fit_base):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_dz_fit_33``,
+    Python interface for O2scl class ``nucmass_dz_fit_33``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dz_fit_33.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_dz_fit_33.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dz_fit_33
 
         | Parameters:
@@ -1236,17 +1236,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_frdm(nucmass_fit_base):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_frdm``,
+    Python interface for O2scl class ``nucmass_frdm``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_frdm.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_frdm.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_frdm
 
         | Parameters:
@@ -1808,17 +1808,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
 
 class nucmass_mnmsk(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_mnmsk``,
+    Python interface for O2scl class ``nucmass_mnmsk``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_mnmsk.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_mnmsk.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_mnmsk
 
         | Parameters:
@@ -1860,17 +1860,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_mnmsk_exp(nucmass_mnmsk):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_mnmsk_exp``,
+    Python interface for O2scl class ``nucmass_mnmsk_exp``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_mnmsk_exp.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_mnmsk_exp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_mnmsk_exp
 
         | Parameters:
@@ -1912,17 +1912,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_gen(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_gen``,
+    Python interface for O2scl class ``nucmass_gen``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_gen.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_gen.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_gen
 
         | Parameters:
@@ -1964,17 +1964,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dglg(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_dglg``,
+    Python interface for O2scl class ``nucmass_dglg``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dglg.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_dglg.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dglg
 
         | Parameters:
@@ -2016,17 +2016,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_hfb(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_hfb``,
+    Python interface for O2scl class ``nucmass_hfb``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_hfb.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_hfb.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_hfb
 
         | Parameters:
@@ -2068,17 +2068,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_hfb_sp(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_hfb_sp``,
+    Python interface for O2scl class ``nucmass_hfb_sp``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_hfb_sp.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_hfb_sp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_hfb_sp
 
         | Parameters:
@@ -2120,17 +2120,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_ktuy(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_ktuy``,
+    Python interface for O2scl class ``nucmass_ktuy``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_ktuy.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_ktuy.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_ktuy
 
         | Parameters:
@@ -2172,17 +2172,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_sdnp(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_sdnp``,
+    Python interface for O2scl class ``nucmass_sdnp``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_sdnp.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_sdnp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_sdnp
 
         | Parameters:
@@ -2224,17 +2224,17 @@
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_wlw(nucmass_table):
     """
-    Python interface for O\ :sub:`2`\ scl class ``nucmass_wlw``,
+    Python interface for O2scl class ``nucmass_wlw``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_wlw.html .
+    https://awsteiner.org/code/o2scl/html/class/nucmass_wlw.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_wlw
 
         | Parameters:
```

### Comparing `o2sclpy-0.928/o2sclpy/o2graph_plotter.py` & `o2sclpy-0.929/o2sclpy/o2graph_plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2023, Andrew W. Steiner
+#  Copyright (C) 2006-2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -28,32 +28,37 @@
 
 # For wrapping help text
 import textwrap
 
 # For code.interact() in 'python' command
 import code 
 
+# For system type detection
+import platform
+
 from o2sclpy.doc_data import cmaps, new_cmaps, extra_types
-from o2sclpy.doc_data import acol_help_topics
+from o2sclpy.doc_data import acol_help_topics, version
 from o2sclpy.doc_data import o2graph_help_topics, acol_types
 from o2sclpy.utils import parse_arguments, string_to_dict, terminal_py
-from o2sclpy.utils import force_bytes, default_plot
-from o2sclpy.utils import is_number
+from o2sclpy.utils import force_bytes, default_plot, cross
+from o2sclpy.utils import is_number, arrow, icosphere
 from o2sclpy.utils import length_without_colors, wrap_line, screenify_py
-from o2sclpy.utils import string_equal_dash
+from o2sclpy.utils import string_equal_dash, latex_to_png
 from o2sclpy.utils import force_string, remove_spaces
 from o2sclpy.plot_base import plot_base
 from o2sclpy.yt_plot_base import yt_plot_base
+from o2sclpy.td_plot_base import td_plot_base, o2scl_get_type
 from o2sclpy.plot_info import marker_list, markers_plot, colors_near
 from o2sclpy.plot_info import cmap_list_func, cmaps_plot, xkcd_colors_list
 from o2sclpy.plot_info import colors_plot, color_list
 from o2sclpy.doc_data import version
 from o2sclpy.hdf import *
 from o2sclpy.base import *
 from o2sclpy.kde import *
+from yt.visualization._commons import get_canvas
 
 base_list=[
     ["addcbar",plot_base.addcbar.__doc__],
     ["arrow",plot_base.arrow.__doc__],
     ["backend",
      ("Documentation for backend\n\n"+
       "Select the matplotlib backend to use.\n\n"+
@@ -74,27 +79,29 @@
     ["colors",plot_base.colors.__doc__],
     ["ellipse",plot_base.ellipse.__doc__],
     ["error-point",plot_base.error_point.__doc__],
     ["eval","Documentation for eval\n\n"+
      "Run the python eval() function.\n\n"+
      "<python code>\n\n"+
      "Take the python code given and execute it using eval(). "+
-     "For example, 'o2graph -eval \"print(numpy.pi)\"'."],
+     "For example::\n\no2graph -eval \"print(numpy.pi)\""],
     ["exec","Documentation for exec\n\n"+
      "Run the python code specified in a file.\n\n"+
      "<filename>\n\n"+
      "Take the python code given and execute it using execfile()."],
+    ["gltf","Produce a GLTF file (experimental)\n\n"+
+     "Produce a GLTF file with the current set of 3D objects."+
+     "\n\n<file name>\n\n"+
+     "Desc."],
     ["image","Documentation for image\n\n"+
      "Plot a png file in a matplotlib window.\n\n"+
      "<png file>\n\n"+
      "This command reads a png file, fills a plotting canvas "+
      "and then calls matplotlib.pyplot.show()."],
     ["inset",plot_base.inset.__doc__],
-    ["kde-plot",0],
-    ["kde-2d-plot",0],
     ["line",plot_base.line.__doc__],
     ["modax",plot_base.modax.__doc__],
     ["mp4",0],
     ["o2scl-addl-libs",
      "Specify a list of list of additional libraries to load."],
     ["o2scl-cpp-lib",
      "Specify the location of the standard C++ library."],
@@ -117,22 +124,39 @@
     ["show",plot_base.show.__doc__],
     ["subadj","Documentation for subadj\n\n"+
      "Adjust spacing of subplots\n\n"+
      "<kwargs>\n\n"+
      "Adjust the spacing for subplots after using the 'subplots' "+
      "command. All arguments are keyword arguments. The kwargs "+
      "for 'subadj' are left, right, bottom, top, "+
-     "wspace, and hspace. This just a wrapper to the "+
+     "wspace, and hspace. This command is a wrapper to the "+
      "pyplot.subplots_adjust() function. Note that, unlike the "+
      "margin settings for the fig_dict parameter, the values "+
      "'right' and 'top' are defined relative to the lower-left "+
      "corner, so a small right margin is 'right=0.99'. The "+
      "subplots_adjust() function requires right>left and "+
      "top>bottom."],
     ["subplots",plot_base.subplots.__doc__],
+    ["td-axis","Documentation for td-axis\n\n"+
+     "Create a 3D axis (experimental).\n\n"+
+     "<x label> <y label> <z label> [png file prefix]\n\n"+
+     "This command creates a default axis with three arrows "+
+     "and three axis labels using LaTeX to convert mathematical "+
+     "expressions to texture images. The textures are named "+
+     "[prefix/]xtitle.png, [prefix/]ytitle.png, and "+
+     "[prefix/]ztitle.png. The mesh objects for the arrows are "+
+     "named x_axis, y_axis, and z_axis, respectively. The "+
+     "coordinate system is always right-handed."],
+    ["td-axis-label",td_plot_base.td_axis_label.__doc__],
+    ["td-arrow",td_plot_base.td_arrow.__doc__],
+    ["td-den-plot",td_plot_base.td_den_plot.__doc__],
+    ["td-icos",td_plot_base.td_icos.__doc__],
+    ["td-pgram",td_plot_base.td_pgram.__doc__],
+    ["td-mat",td_plot_base.td_mat.__doc__],
+    ["td-scatter",td_plot_base.td_scatter.__doc__],
     ["text",plot_base.text.__doc__],
     ["textbox",plot_base.textbox.__doc__],
     ["ttext",plot_base.ttext.__doc__],
     ["xlimits",plot_base.xlimits.__doc__],
     ["xtitle",plot_base.xtitle.__doc__],
     ["ylimits",plot_base.ylimits.__doc__],
     ["ytitle",plot_base.ytitle.__doc__],
@@ -161,14 +185,16 @@
     ["prob_dens_mdim_amr","plot",0],
     ["size_t[]","plot1",0],
     ["table","errorbar",0],
     ["table","hist-plot",0],
     ["table","hist2d-plot",0],
     ["table","plot",0],
     ["table","to-kde",0],
+    ["table","kde-plot",0],
+    ["table","kde-2d-plot",0],
     ["table","plot1",0],
     ["table","plot-color",0],
     ["table","rplot",0],
     ["table","scatter",0],
     ["table","yt-scatter",0],
     ["table","yt-vertex-list",0],
     ["table3d","den-plot",0],
@@ -177,14 +203,15 @@
     ["tensor","den-plot",0],
     ["tensor<int>","den-plot",0],
     ["tensor<size_t>","den-plot",0],
     ["tensor_grid","den-plot",0],
     ["tensor_grid","den-plot-anim",0],
     ["tensor_grid","yt-add-vol",0],
     ["vector<contour_line>","plot",0],
+    ["vec_vec_double","plot",0],
 ]
 
 param_list=[
     ["colbar","If true, den-plot adds a color legend (default False)."],
     ["editor","If true, open the plot editor."],
     ["fig_dict",("Dictionary for figure properties. The default value is "+
                  "blank and implies ('fig_size_x=6.0, fig_size_y=6.0, "+
@@ -204,14 +231,15 @@
                  "created (which is done by 'subplots' or automatically "+
                  "when the first object is added to the plot) in order "+
                  "to have any effect.")],
     ["font","Font scaling for text objects (default 16)."],
     ["logx","If true, use a logarithmic x-axis (default False)."],
     ["logy","If true, use a logarithmic y-axis (default False)."],
     ["logz","If true, use a logarithmic z-axis (default False)."],
+    ["td_wdir",""],
     ["usetex","If true, use LaTeX for text rendering (default True)."],
     ["verbose","Verbosity parameter (default 1)."],
     ["xhi","Upper limit for x-axis (function if starts with '(')."],
     ["xlo","Lower limit for x-axis (function if starts with '(')."],
     ["xset","If true, x-axis limits have been set (default False)."],
     ["yhi","Upper limit for y-axis (function if starts with '(')."],
     ["ylo","Lower limit for y-axis (function if starts with '(')."],
@@ -262,27 +290,31 @@
 ]
 """
 List of yt parameters for o2sclpy
 
 A list of 2-element entries, name and description
 """
 
-def doc_replacements(s,ter,amp,link,script=False):
+def doc_replacements(s,ter,amp,link,script=False,verbose=0):
     """
     Make some replacements from RST formatting to the terminal screen.
 
     This function is in ``o2graph_plotter.py``.
     """
 
     amt=acol_manager(link,amp)
 
     if script:
         s=(force_string(amt.get_exec_color())+s+
            force_string(amt.get_default_color()))
         return s
+
+    if verbose>2:
+        print('Function doc_replacements():')
+        print(' s=',s)
     
     # Replace commands in base_list
     for i in range(0,len(base_list)):
         s=s.replace('``'+base_list[i][0]+'``',
                     force_string(amt.get_command_color())+
                     base_list[i][0]+
                     force_string(amt.get_default_color()))
@@ -353,29 +385,20 @@
     s=s.replace(' :math:`',' ')
     s=s.replace('` ',' ')
     s=s.replace('`.','.')
     s=s.replace('`',',')
                     
     return s
 
-def o2scl_get_type(o2scl,amp,link):
-    """
-    Get the type of the current object stored in the acol_manager
-    pointer
-    """
-
-    amt=acol_manager(link,amp)
-    return amt.get_type()
-
 def reformat_python_docs(cmd,doc_str,amp,link,
                          return_short=False,verbose=0):
     """
     Reformat a python documentation string
     """
-    
+
     amt=acol_manager(link,amp)
     
     reflist=doc_str.split('\n')
     
     for i in range(0,len(reflist)):
         reflist[i]=remove_spaces(reflist[i])
         if verbose>1:
@@ -441,15 +464,15 @@
         print('Long description:')
         last_pgh_colons=False
         for j in range(3,len(reflist2)):
             if len(reflist2[j])>0:
                 if last_pgh_colons:
                     long_help=doc_replacements(reflist2[j].replace('\n',' '),
                                                ter,amp,link,script=True)
-                    tmplist=long_help.split(' \ ')
+                    tmplist=long_help.split(' \\ ')
                 else:
                     long_help=doc_replacements(reflist2[j].replace('\n',' '),
                                                ter,amp,link)
                     tmplist=wrap_line(long_help,ncols-1)
                 if j!=3:
                     print('')
                 for k in range(0,len(tmplist)):
@@ -556,23 +579,39 @@
           force_string(amt.get_default_color())+' '+parm_desc)
     
     print('Short description:',short)
 
     if len(reflist3)>2:
         print('')
         print('Long description:')
+        last_pgh_colons=False
         for j in range(2,len(reflist3)):
             if len(reflist3[j])>0:
-                long_help=doc_replacements(reflist3[j].replace('\n',' '),
-                                           ter,amp,link)
-                tmplist=wrap_line(long_help,ncols-1)
-                if j!=3:
+                if last_pgh_colons:
+                    long_help=doc_replacements(reflist3[j].replace('\n',' '),
+                                               ter,amp,link,script=True)
+                    tmplist=long_help.split(' \\ ')
+                else:
+                    long_help=doc_replacements(reflist3[j].replace('\n',' '),
+                                               ter,amp,link)
+                    tmplist=wrap_line(long_help,ncols-1)
+                if j!=2:
                     print('')
                 for k in range(0,len(tmplist)):
-                    print(tmplist[k])
+                    if last_pgh_colons:
+                        if k!=len(tmplist)-1:
+                            print(' ',tmplist[k],'\\')
+                        else:
+                            print(' ',tmplist[k])
+                    else:
+                        print(tmplist[k])
+                if long_help[-2:]=='::':
+                    last_pgh_colons=True
+                else:
+                    last_pgh_colons=False
                     
     return
 
 def table_get_column(o2scl,amp,link,name,return_pointer=False):
     """
     Return a column from the current table object stored
     in the acol_manager object 'amp'
@@ -580,15 +619,15 @@
 
     amt=acol_manager(link,amp)
     tab=amt.get_table_obj()
     col=tab[force_bytes(name)]
 
     return col
 
-class o2graph_plotter(yt_plot_base):
+class o2graph_plotter(td_plot_base):
     """
     A plotting class for the o2graph script. This class is a child of the
     :py:class:`o2sclpy.plot_base` class.
 
     This class is not necessarily intended to be instantiated by the 
     end user. 
 
@@ -617,45 +656,45 @@
                 line[1]=o2graph_plotter.yt_path_func.__doc__
             elif line[0]=="yt-render":
                 line[1]=o2graph_plotter.yt_render.__doc__
             elif line[0]=="yt-text":
                 line[1]=o2graph_plotter.yt_text.__doc__
             elif line[0]=="mp4":
                 line[1]=o2graph_plotter.mp4.__doc__
-            elif line[0]=="kde-plot":
-                line[1]=o2graph_plotter.kde_plot.__doc__
-            elif line[0]=="kde-2d-plot":
-                line[1]=o2graph_plotter.kde_2d_plot.__doc__
             elif line[0]=="yt-tf":
                 line[1]=o2graph_plotter.yt_tf_func.__doc__
         for line in extra_list:
-            if line[1]=="to-kde":
-                line[2]=o2graph_plotter.to_kde.__doc__
             if line[1]=="den-plot":
                 line[2]=o2graph_plotter.den_plot_o2graph.__doc__
-            if line[1]=="den-plot-rgb":
+            elif line[1]=="den-plot-rgb":
                 line[2]=o2graph_plotter.den_plot_rgb_o2graph.__doc__
-            if line[1]=="den-plot-anim":
+            elif line[1]=="den-plot-anim":
                 line[2]=o2graph_plotter.den_plot_anim.__doc__
-            if line[1]=="errorbar":
+            elif line[1]=="errorbar":
                 line[2]=o2graph_plotter.errorbar.__doc__
             elif line[1]=="hist-plot":
                 line[2]=o2graph_plotter.hist_plot.__doc__
             elif line[1]=="hist2d-plot":
                 line[2]=o2graph_plotter.hist2d_plot.__doc__
+            elif line[1]=="kde-plot":
+                line[2]=o2graph_plotter.kde_plot.__doc__
+            elif line[1]=="kde-2d-plot":
+                line[2]=o2graph_plotter.kde_2d_plot.__doc__
             elif line[1]=="plot":
                 line[2]=o2graph_plotter.plot_o2graph.__doc__
             elif line[1]=="plot1":
                 line[2]=o2graph_plotter.plot1.__doc__
             elif line[1]=="plot-color":
                 line[2]=o2graph_plotter.plot_color.__doc__
             elif line[1]=="rplot":
                 line[2]=o2graph_plotter.rplot.__doc__
             elif line[1]=="scatter":
                 line[2]=o2graph_plotter.scatter.__doc__
+            elif line[1]=="to-kde":
+                line[2]=o2graph_plotter.to_kde.__doc__
             elif line[1]=="yt-add-vol":
                 line[2]=o2graph_plotter.yt_add_vol.__doc__
             elif line[1]=="yt-anim":
                 line[2]=o2graph_plotter.yt_anim.__doc__
             elif line[1]=="yt-scatter":
                 line[2]=o2graph_plotter.yt_scatter.__doc__
             elif line[1]=="yt-vertex-list":
@@ -673,26 +712,29 @@
 
         # First determine if it's an o2graph or yt parameter
         match=False
         for line in param_list:
             if args[0]==line[0]:
                 match=True
                 if self.verbose>2:
-                    print('Parameter',args[0],'is o2graph parameter.')
+                    print('Parameter',args[0],'is an o2graph parameter.')
                 
         for line in yt_param_list:
             if args[0]==line[0]:
                 match=True
                 if self.verbose>2:
                     print('Parameter',args[0],'is a yt parameter.')
 
         # If it's an o2graph or yt parameter, then call the parent
-        # set() function
+        # set() function or set the variable
         if match==True:
-            self.set(args[0],args[1])
+            if args[0]=='td_wdir':
+                self.td_wdir=args[1]
+            else:
+                self.set(args[0],args[1])
 
         # If we're modifying the verbose parameter, then make sure
         # both the o2graph and the acol version match. Otherwise, if
         # it's only an o2graph or yt parameter, then just return.
         if (match==True and 
             force_bytes(args[0])!=b'verbose'):
             return
@@ -805,55 +847,341 @@
         return
 
     def to_kde(self,o2scl,amp,link,args):
         """Documentation for o2graph command ``to-kde``:
 
         For objects of type ``table``:
 
-        Convert columns in a table to a KDE
+        Convert columns in a table to a KDE (unfinished)
 
         Command-line arguments: ``<options or 'none'> 
         <column 1> [column 2] ...``
 
         Desc.
         """
+
+        # Note that this command is more complicated because acol uses
+        # Python to compute the KDE and thus the o2graph version has
+        # to be different to bypass the C++ stage.
         
         curr_type=o2scl_get_type(o2scl,amp,self.link2)
         amt=acol_manager(self.link2,amp)
-        print('here')
+        print('Command to-kde is not yet finished.')
         quit()
         #if curr_type==b'table':
         #else:
 
-    def mp4(self,args):
-        """
-        Documentation for o2graph command ``mp4``:
+    def mp4(self,args,loop=False,vf=''):
+        """Documentation for o2graph command ``mp4``:
 
         Create an mp4 file from a series of images.
 
         Command-line arguments: ``<pattern> <output>``
 
-        Typical patterns are "prefix%02dsuffix" and outputs
-        are "out.mp4"
+        Typical patterns are "prefix%02dsuffix" and outputs are
+        "out.mp4". If the "mp4" suffix is omitted, it is automatically
+        added.
+
+        A typical video filter is e.g. vf='eq=brightness=0.5:contrast=10'.
+
+        This command requires the installation of ``ffmpeg``. 
         """
         if len(args)<2:
-            print('Command mpg needs more arguments.')
+            print('Command mp4 needs more arguments.')
             return
         pattern=args[0]
         output=args[1]
         if output[-4:]!='.mp4':
             output=output+'.mp4'
+
+        # -y means overwrite output without asking
+        # -r 10 means set the framerate to 10 frames per second
+        # -vcodec sets the video codec
+        # -pix_fmt sets the pixel format
+            
         cmd=('ffmpeg -y -r 10 -f image2 -i '+pattern+
-             ' -vcodec libx264 '+
-             '-crf 25 -pix_fmt yuv420p '+output)
-        print('Executing ',cmd)
+             ' -vcodec libx264')
+        if vf!='':
+            cmd=cmd+' -vf '+vf
+        if loop==True:
+            cmd=cmd+' -stream_loop -1'
+            
+        cmd=cmd+' -crf 25 -pix_fmt yuv420p '+output
+        
+        print('o2graph_plottter::mp4(): Executing "'+cmd+'".')
         os.system(cmd)
         
         return
         
+    def bl_yaw_mp4(self, n_frames: int, mp4_file: str,
+                   blender_cmd: str = '', o2sclpy_dir: str = '',
+                   vf: str = '', cam_dist: float = 5.0,
+                   light_energy : float = 800,
+                   light_dist : float = 5.8,
+                   bg_color : str = '', cam_type : str = '',
+                   res=(0,0), blend_file : str = ''):
+        """
+        This command requires Blender, the associated python package,
+        ``bpy``, and the installation of ``ffmpeg``. 
+
+        vf='eq=contrast=1')
+        """
+
+        import tempfile
+        
+        gltf_file_name='o2sclpy.gltf'
+        print('Writing GLTF to',self.td_wdir+'/'+gltf_file_name)
+
+        self.to.write_gltf(self.td_wdir,gltf_file_name)
+        
+        py_file_name=self.td_wdir+'/o2sclpy.py'
+        print('Writing Python script to',py_file_name)
+
+        # Try to find o2sclpy by finding the numpy directory
+        if o2sclpy_dir=='':
+            o2sclpy_dir=numpy.__path__[0][:-5]+'o2sclpy/'
+            print('Setting o2sclpy_dir to:',o2sclpy_dir)
+            
+        orig_script=(o2sclpy_dir+'bl_gltf_yaw.py')
+        
+        print('Original script at:',orig_script)
+
+        if bg_color=='':
+            bg_color='(0,0,0,0)'
+            
+        if cam_type=='':
+            cam_type='PERSP'
+            
+        rep_list={'BG_COLOR': bg_color,
+                  'LIGHT_DIST': str(light_dist),
+                  'LIGHT_ENERGY': str(light_energy),
+                  'GLTF_PATH': gltf_file_name,
+                  'N_FRAMES': str(n_frames),
+                  'CAM_DIST': str(cam_dist),
+                  'RES_X': str(res[0]),
+                  'RES_Y': str(res[1]),
+                  'BLEND_FILE': str(blend_file),
+                  'CAMERA_TYPE': str(cam_type)}
+        print('Making replacements:',rep_list)
+
+        forig=open(orig_script,'r')
+        lines=forig.readlines()
+        frep=open(py_file_name,'w')
+        for line in lines:
+            line=line.replace('BG_COLOR',rep_list['BG_COLOR'])
+            line=line.replace('LIGHT_DIST',rep_list['LIGHT_DIST'])
+            line=line.replace('LIGHT_ENERGY',rep_list['LIGHT_ENERGY'])
+            line=line.replace('GLTF_PATH',rep_list['GLTF_PATH'])
+            line=line.replace('N_FRAMES',rep_list['N_FRAMES'])
+            line=line.replace('CAM_DIST',rep_list['CAM_DIST'])
+            line=line.replace('RES_X',rep_list['RES_X'])
+            line=line.replace('RES_Y',rep_list['RES_Y'])
+            line=line.replace('BLEND_FILE',rep_list['BLEND_FILE'])
+            line=line.replace('CAMERA_TYPE',rep_list['CAMERA_TYPE'])
+            frep.write(line)
+        forig.close()
+        frep.close()
+
+        if blender_cmd=='':
+            if not 'O2GRAPH_BLENDER_CMD' in os.environ:
+                if platform.system()=='Darwin':
+                    blender_cmd=('/Applications/Blender.app'+
+                                 '/Contents/MacOS/Blender')
+                    print('Blender command not specified, presuming MacOS',
+                          'default')
+                    print(' ',blender_cmd,'.')
+                else:
+                    blender_cmd='/usr/bin/blender'
+                    print('Blender command not specified, presuming Linux',
+                          'default')
+                    print(' ',blender_cmd,'.')
+            else:
+                blender_cmd=os.environ['O2GRAPH_BLENDER_CMD']
+        
+        cmd=('cd '+self.td_wdir+' && '+blender_cmd+' -b -P o2sclpy.py')
+        print('Executing:',cmd)
+        os.system(cmd)
+
+        print('Creating mp4')
+        self.mp4([self.td_wdir+'/bl_gltf_yaw_%03d.png',mp4_file],
+                 vf=vf)
+
+        return
+        
+    def bl_six_mp4(self, n_frames: int, mp4_file: str,
+                   blender_cmd: str = '', o2sclpy_dir: str = '',
+                   vf: str = '', cam_dist: float = 5.0,
+                   light_energy : float = 800,
+                   light_dist : float = 5.8,
+                   bg_color : str = '', cam_type : str = '',
+                   res=(0,0), blend_file : str = ''):
+        """
+        
+        This command requires the Blender python package,
+        ``bpy`` and the installation of ``ffmpeg``. 
+        """
+
+        import tempfile
+        
+        gltf_file_name='o2sclpy.gltf'
+        print('Writing GLTF to',self.td_wdir+'/'+gltf_file_name)
+
+        self.to.write_gltf(self.td_wdir,gltf_file_name)
+        
+        py_file_name=self.td_wdir+'/o2sclpy.py'
+        print('Writing Python script to',py_file_name)
+
+        # Try to find o2sclpy by finding the numpy directory
+        if o2sclpy_dir=='':
+            o2sclpy_dir=numpy.__path__[0][:-5]+'o2sclpy/'
+            print('Setting o2sclpy_dir to:',o2sclpy_dir)
+            
+        orig_script=(o2sclpy_dir+'bl_gltf_six.py')
+        
+        print('Original script at:',orig_script)
+
+        if bg_color=='':
+            bg_color='(0,0,0,0)'
+            
+        if cam_type=='':
+            cam_type='ORTHO'
+            
+        rep_list={'BG_COLOR': bg_color,
+                  'LIGHT_DIST': str(light_dist),
+                  'LIGHT_ENERGY': str(light_energy),
+                  'GLTF_PATH': gltf_file_name,
+                  'N_FRAMES': str(n_frames),
+                  'CAM_DIST': str(cam_dist),
+                  'RES_X': str(res[0]),
+                  'RES_Y': str(res[1]),
+                  'BLEND_FILE': str(blend_file),
+                  'CAMERA_TYPE': str(cam_type)}
+        print('Making replacements:',rep_list)
+
+        forig=open(orig_script,'r')
+        lines=forig.readlines()
+        frep=open(py_file_name,'w')
+        for line in lines:
+            line=line.replace('BG_COLOR',rep_list['BG_COLOR'])
+            line=line.replace('LIGHT_DIST',rep_list['LIGHT_DIST'])
+            line=line.replace('LIGHT_ENERGY',rep_list['LIGHT_ENERGY'])
+            line=line.replace('GLTF_PATH',rep_list['GLTF_PATH'])
+            line=line.replace('N_FRAMES',rep_list['N_FRAMES'])
+            line=line.replace('CAM_DIST',rep_list['CAM_DIST'])
+            line=line.replace('RES_X',rep_list['RES_X'])
+            line=line.replace('RES_Y',rep_list['RES_Y'])
+            line=line.replace('BLEND_FILE',rep_list['BLEND_FILE'])
+            line=line.replace('CAMERA_TYPE',rep_list['CAMERA_TYPE'])
+            frep.write(line)
+        forig.close()
+        frep.close()
+
+        if blender_cmd=='':
+            if not 'O2GRAPH_BLENDER_CMD' in os.environ:
+                if platform.system()=='Darwin':
+                    blender_cmd=('/Applications/Blender.app'+
+                                 '/Contents/MacOS/Blender')
+                    print('Blender command not specified, presuming MacOS',
+                          'default')
+                    print(' ',blender_cmd,'.')
+                else:
+                    blender_cmd='/usr/bin/blender'
+                    print('Blender command not specified, presuming Linux',
+                          'default')
+                    print(' ',blender_cmd,'.')
+            else:
+                blender_cmd=os.environ['O2GRAPH_BLENDER_CMD']
+        
+        cmd=('cd '+self.td_wdir+' && '+blender_cmd+' -b -P o2sclpy.py')
+        print('Executing:',cmd)
+        os.system(cmd)
+
+        print('Creating mp4')
+        self.mp4([self.td_wdir+'/bl_gltf_six_%03d.png',mp4_file],
+                 vf=vf)
+
+        #vf='eq=contrast=1')
+        
+        return
+        
+    def bl_import(self, gltf_path: str='',
+                  blender_cmd: str = '', o2sclpy_dir: str = '',
+                  cam_dist: float = 5.0,
+                  light_energy : float = 800,
+                  light_dist : float = 5.8,
+                  bg_color : str = '', cam_type : str = '',
+                  res=(0,0), blend_file : str = ''):
+        """This command requires the Blender python package, ``bpy``.
+        """
+
+        gltf_file_name=gltf_path
+        print('Reading GLTF from',gltf_file_name)
+
+        py_file_name=self.td_wdir+'/o2sclpy.py'
+        print('Writing Python script to',py_file_name)
+
+        # Try to find o2sclpy by finding the numpy directory
+        if o2sclpy_dir=='':
+            o2sclpy_dir=numpy.__path__[0][:-5]+'o2sclpy/'
+            print('Setting o2sclpy_dir to:',o2sclpy_dir)
+            
+        orig_script=(o2sclpy_dir+'bl_gltf_import.py')
+        
+        print('Original script at:',orig_script)
+
+        if bg_color=='':
+            bg_color='(0,0,0,0)'
+
+        if cam_type=='':
+            cam_type='PERSP'
+            
+        rep_list={'BG_COLOR': bg_color,
+                  'LIGHT_DIST': str(light_dist),
+                  'LIGHT_ENERGY': str(light_energy),
+                  'GLTF_PATH': gltf_file_name,
+                  'CAM_DIST': str(cam_dist),
+                  'CAMERA_TYPE': str(cam_type)}
+        print('Making replacements:',rep_list)
+
+        forig=open(orig_script,'r')
+        lines=forig.readlines()
+        frep=open(py_file_name,'w')
+        for line in lines:
+            line=line.replace('BG_COLOR',rep_list['BG_COLOR'])
+            line=line.replace('LIGHT_DIST',rep_list['LIGHT_DIST'])
+            line=line.replace('LIGHT_ENERGY',rep_list['LIGHT_ENERGY'])
+            line=line.replace('GLTF_PATH',rep_list['GLTF_PATH'])
+            line=line.replace('CAM_DIST',rep_list['CAM_DIST'])
+            line=line.replace('CAMERA_TYPE',rep_list['CAMERA_TYPE'])
+            frep.write(line)
+        forig.close()
+        frep.close()
+
+        if blender_cmd=='':
+            if not 'O2GRAPH_BLENDER_CMD' in os.environ:
+                if platform.system()=='Darwin':
+                    blender_cmd=('/Applications/Blender.app'+
+                                 '/Contents/MacOS/Blender')
+                    print('Blender command not specified, presuming MacOS',
+                          'default')
+                    print(' ',blender_cmd,'.')
+                else:
+                    blender_cmd='/usr/bin/blender'
+                    print('Blender command not specified, presuming Linux',
+                          'default')
+                    print(' ',blender_cmd,'.')
+            else:
+                blender_cmd=os.environ['O2GRAPH_BLENDER_CMD']
+        
+        cmd=('cd '+self.td_wdir+' && '+blender_cmd+' -P o2sclpy.py')
+        print('Executing:',cmd)
+        os.system(cmd)
+
+        return
+        
     def den_plot_o2graph(self,o2scl,amp,link,args):
         """Documentation for o2graph command ``den-plot``:
 
         For objects of type ``table3d``:
 
         Create a density plot from a slice of a table3d
 
@@ -1067,15 +1395,18 @@
 
         Create a density plot from a specified slice
 
         Command-line arguments: ``<slice r> <slice g> <slice b> [kwargs]``
 
         Create a density plot from the three specified slices. This
         command uses imshow(). To directly create a .png file with no
-        axes, use make-png instead.
+        axes, use make-png instead. For example::
+
+            o2graph -create table3d x "grid:0,1,0.01" y "grid:0,1,0.01" \\
+            r "x" -function "y" g -function 0 b -den-plot-rgb r g b -show
         """
 
         curr_type=o2scl_get_type(o2scl,amp,self.link2)
         amt=acol_manager(self.link2,amp)
 
         kwstring=''
         if curr_type!=b'table3d':
@@ -1085,20 +1416,40 @@
             
         slice_r=args[0]
         slice_g=args[1]
         slice_b=args[2]
         if len(args)>=4:
             kwstring=args[3]
 
-        dctt=string_to_dict(kwstring)
-        self.den_plot(amt.get_table3d_obj(),slice_r,slice_g,slice_b,
-                      **dctt)
+        dctt=string_to_dict2(kwstring,list_of_bools=['renorm'])
+        self.den_plot_rgb(amt.get_table3d_obj(),slice_r,slice_g,slice_b,
+                          **dctt)
 
         return
 
+    def gltf_o2graph(self,o2scl,amp,link,args):
+        """Documentation for o2graph command ``gltf``:
+
+        Write a GLTF file from 3D objects (experimental)
+
+        Command-line arguments: ``<prefix> [kwargs]``
+
+        Write a GLTF file from 3D objects.
+        """
+        prefix=args[0]
+        if len(args)>=2:
+            kwstring=args[1]
+
+        if self.verbose>2:
+            print('Writing gltf to directory',self.td_wdir,
+                  'and file',prefix+'.')
+        self.to.write_gltf(self.td_wdir,prefix,verbose=self.verbose)
+
+        return
+    
     def make_png_o2graph(self,o2scl,amp,link,args):
         """
         Documentation for o2graph command ``make-png``:
         
         For objects of type ``table3d``:
 
         Command-line arguments: ``<slice r> <slice g> <slice b> [kwargs]``
@@ -1141,19 +1492,32 @@
 
         For objects of type ``table``:
 
         Plot a KDE of one column
 
         Command-line arguments: ``<column> [plot kwargs] [kde kwargs]``
 
-        Useful plot kwargs are all the usual plotting kwargs, plus
-        x_min=0, x_max=0, y_mult=1, and n_points=201.
+        This command takes the column of the table, computes a
+        one-dimensional KDE, and then uses that KDE to fill two
+        vectors, an x and y vector to plot the data. Useful plot
+        kwargs are all the usual plotting kwargs, plus x_min=0,
+        x_max=0, y_mult=1, and n_points=201. If x_max is less than
+        x_min then the limits on the x vector are either taken from
+        the parameters ``xlo`` and ``xhi`` if they are set, or 
+        otherwise computed from the minimum and maximum of the data.
+        Otherwise, if x_max is smaller than x_min, then those 
+        values are used as the limits for the KDE (which need not
+        correspond to ``xlo`` and ``xhi``). The number of points
+        between x_min and x_max is determined by the n_points parameter. 
+        The y vector is multiplied by y_mult before plotting. 
+        
 
         Useful KDE kwargs are kernel='gaussian', metric='euclidean',
         transform='unit', and bandwidth='none'.
+
         """
         curr_type=o2scl_get_type(o2scl,amp,link)
 
         if curr_type==b'table':
             
             amt=acol_manager(link,amp)
             tab=amt.get_table_obj()
@@ -1178,14 +1542,19 @@
                                          list_of_floats=['x_min','x_max',
                                                          'y_mult'])
                 x_min=dct_plot.pop('x_min',0)
                 x_max=dct_plot.pop('x_max',0)
                 y_mult=dct_plot.pop('y_mult',1)
                 n_points=dct_plot.pop('n_points',201)
 
+            if n_points<2:
+                print('o2graph_plotter::kde_plot():',
+                      'Value n_points too small, fixing to 2.'),
+                n_points=2
+
             # If x_min and x_max are not set, then determine them,
             # either from the plot limits or from the minimum
             # and maximum of the data
             if x_min>=x_max:
                 if self.xset==False:
                     # Determine min and max of data
                     x_min=x[0,0]
@@ -1194,15 +1563,20 @@
                         if x[i,0]<x_min:
                             x_min=x[i,0]
                         if x[i,0]>x_max:
                             x_max=x[i,0]
                 else:
                     x_min=self.xlo
                     x_max=self.xhi
-            print('x_min,x_max,n_points,y_mult:',x_min,x_max,n_points,y_mult)
+
+            if self.verbose>0:
+                print('o2graph_plotter::kde_plot():'),
+                print(('  x_min,x_max,n_points,y_mult: '+
+                       '%7.6e %7.6e %d %7.6e') % (x_min,x_max,n_points,
+                                                  y_mult))
 
             # Use sklearn and a reasonable guess for the bandwidth,
             # between 1.0e-2 and 1.0e+2. Note that the KDE is
             # rescaled by default. 
             k=kde_sklearn()
             bw_array=[10**(float(i)/4.0-2.0) for i in range(0,17)]
 
@@ -1228,89 +1602,153 @@
                 self.plot([xa,ya],**dct_plot)
                 
         else:
             print("Command 'kde-plot' not supported for type",
                   curr_type,".")
             return
         
-        # End of function o2graph_plotter::plot_o2graph()
+        # End of function o2graph_plotter::kde_plot()
         return
 
     def kde_2d_plot(self,o2scl,amp,args,link):
         """Documentation for o2graph command ``kde-2d-plot``:
 
         For objects of type ``table``:
 
         Plot a KDE of two columns
 
-        Command-line arguments: ``<column x> <column y> [options]``
+        Command-line arguments: ``<column x> <column y> [plot kwargs]
+        [kde kwargs]``
 
-        Desc.
+        This command converts the two columns to a matrix and two
+        vectors which define the x and y grids. Useful plot kwargs are
+        all the usual plotting kwargs, plus x_min=0, x_max=0, y_min=0,
+        y_max=0, z_mult=1, and n_points=201. Similar to the command
+        ``kde-plot``, if x_max is less than x_min then the limits on
+        the x grid are either taken from the parameters ``xlo`` and
+        ``xhi`` if they are set, or otherwise computed from the
+        minimum and maximum of the specified x column. Otherwise, if
+        x_max is smaller than x_min, then those values are used as the
+        limits for the KDE (which need not correspond to ``xlo`` and
+        ``xhi``). The same holds for y_min, y_max, and the y grid. The
+        number of points between x_min and x_max and between y_min and
+        y_max is determined by the n_points parameter. The z vector is
+        multiplied by y_mult before plotting.
+
+        Useful KDE kwargs are kernel='gaussian', metric='euclidean',
+        transform='unit', and bandwidth='none'.
         """
         curr_type=o2scl_get_type(o2scl,amp,link)
 
         if curr_type==b'table':
             
             amt=acol_manager(link,amp)
             tab=amt.get_table_obj()
 
             # Copy the table data to a numpy array
             x=numpy.zeros((tab.get_nlines(),2))
             for i in range(0,tab.get_nlines()):
                 x[i,0]=tab.get(args[0],i)
                 x[i,1]=tab.get(args[1],i)
 
-            x0_min=x[0,0]
-            x0_max=x[0,0]
-            x1_min=x[0,1]
-            x1_max=x[0,1]
-            for i in range(1,tab.get_nlines()):
-                if x[i,0]<x0_min:
-                    x0_min=x[i,0]
-                if x[i,0]>x0_max:
-                    x0_max=x[i,0]
-                if x[i,1]<x1_min:
-                    x1_min=x[i,1]
-                if x[i,1]>x1_max:
-                    x1_max=x[i,1]
-                
+            # Set defaults
+            x_min=0
+            x_max=0
+            y_min=0
+            y_max=0
+            n_points=201
+            z_mult=1
+            
+            # Convert kwargs to string so we can extract
+            # n_points, x_min, and x_max
+            dct_plot={}
+            if len(args)>=3:
+                dct_plot=string_to_dict2(args[2],
+                                         list_of_ints=['n_points'],
+                                         list_of_floats=['x_min','x_max',
+                                                         'y_min','y_max',
+                                                         'z_mult'])
+                x_min=dct_plot.pop('x_min',0)
+                x_max=dct_plot.pop('x_max',0)
+                y_min=dct_plot.pop('y_min',0)
+                y_max=dct_plot.pop('y_max',0)
+                z_mult=dct_plot.pop('z_mult',1)
+                n_points=dct_plot.pop('n_points',201)
+
+            # If x_min and x_max are not set, then determine them,
+            # either from the plot limits or from the minimum
+            # and maximum of the data 
+            if x_min>=x_max:
+                if self.xset==False:
+                    # Determine min and max of data
+                    x_min=x[0,0]
+                    x_max=x[0,0]
+                    for i in range(1,tab.get_nlines()):
+                        if x[i,0]<x_min:
+                            x_min=x[i,0]
+                        if x[i,0]>x_max:
+                            x_max=x[i,0]
+                else:
+                    x_min=self.xlo
+                    x_max=self.xhi
+
+            if y_min>=y_max:
+                if self.yset==False:
+                    # Determine min and max of data
+                    y_min=x[0,1]
+                    y_max=x[0,1]
+                    for i in range(1,tab.get_nlines()):
+                        if x[i,1]<y_min:
+                            y_min=x[i,1]
+                        if x[i,1]>y_max:
+                            y_max=x[i,1]
+                else:
+                    y_min=self.ylo
+                    y_max=self.yhi
+                    
+            if self.verbose>0:
+                print('o2graph_plotter::kde_2d_plot():'),
+                print(('  x_min,x_max,y_min,y_max,n_points,z_mult: '+
+                       '%7.6e %7.6e\n  %7.6e %7.6e %d %7.6e') %
+                      (x_min,x_max,y_min,y_max,n_points,z_mult))
+
             k=kde_sklearn()
             bw_array=[10**(float(i)/4.0-2.0) for i in range(0,17)]
 
-            if len(args)>2:
-                k.set_data_str(x,bw_array,args[1])
+            if len(args)>4:
+                k.set_data_str(x,bw_array,args[3])
             else:
                 k.set_data_str(x,bw_array,'')
 
             x0a=[]
-            x0p=x0_min
-            for i in range(0,201):
+            x0p=x_min
+            for i in range(0,n_points):
                 x0a.append(x0p)
-                x0p=x0p+(x0_max-x0_min)/200.0
+                x0p=x0p+(x_max-x_min)/float(n_points-1)
             x1a=[]
-            x1p=x1_min
-            for i in range(0,201):
+            x1p=y_min
+            for i in range(0,n_points):
                 x1a.append(x1p)
-                x1p=x1p+(x1_max-x1_min)/200.0
-            z=numpy.zeros((200,200))
-            for i in range(0,201):
-                for j in range(0,201):
-                    z[i,j]=k.pdf([x0a[i],x1a[j]])
+                x1p=x1p+(y_max-y_min)/float(n_points-1)
+            z=numpy.zeros((n_points,n_points))
+            for i in range(0,n_points):
+                for j in range(0,n_points):
+                    z[i,j]=k.pdf([x0a[i],x1a[j]])*z_mult
 
             if len(args)<3:
                 self.den_plot([x0a,x1a,z])
             else:
-                self.den_plot([x0a,x1a,z],**string_to_dict(args[2]))
+                self.den_plot([x0a,x1a,z],**dct_plot)
                 
         else:
             print("Command 'kde-2d-plot' not supported for type",
                   curr_type,".")
             return
         
-        # End of function o2graph_plotter::plot_o2graph()
+        # End of function o2graph_plotter::kde_2d_plot()
         return
 
     def plot_o2graph(self,o2scl,amp,args,link):
         """Documentation for o2graph command ``plot``:
 
         For objects of type ``table``:
 
@@ -1318,18 +1756,20 @@
 
         Command-line arguments: ``<x> <y> [kwargs]``
 
         Plot column <y> versus
         column <x>. Some useful kwargs are color (c), dashes,
         linestyle (ls), linewidth (lw), marker, markeredgecolor (mec),
         markeredgewidth (mew), markerfacecolor (mfc),
-        markerfacecoloralt (mfcalt), markersize (ms). For example:
-        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
-        lw=0,marker='+' -show\". This command uses the matplotlib
-        plot() function, see
+        markerfacecoloralt (mfcalt), markersize (ms). For example::
+
+            o2graph -create table x grid:0,10,0.2 -function "sin(x)" y \\
+            -plot x y "lw=0,marker=+" -show 
+
+        This command uses the matplotlib plot() function, see
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
         for information and keyword arguments. This command does not
         yet support the matplotlib format parameter.
 
         For objects of type ``vec_vec_double``:
 
         Plot one or two columns.
@@ -1338,18 +1778,20 @@
 
         Plot vector with index [index y] versus vector with index
         <index x>. Alternatively, if the second argument is the
         string 'none', plot the vector with index <index x>.
         Some useful kwargs are color (c), dashes, linestyle
         (ls), linewidth (lw), marker, markeredgecolor (mec),
         markeredgewidth (mew), markerfacecolor (mfc),
-        markerfacecoloralt (mfcalt), markersize (ms). For example:
-        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
-        lw=0,marker='+' -show\". This command uses the matplotlib
-        plot() function, see
+        markerfacecoloralt (mfcalt), markersize (ms). For example::
+        
+            o2graph -create vec_vec_double grid:0,10,0.2 "func:51:sin(i)" \\
+            -plot 0 1 "lw=0,marker=+" -show
+
+        This command uses the matplotlib plot() function, see
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
         for information and keyword arguments. This command does not
         yet support the matplotlib format parameter.
 
         For objects of type ``hist``:
 
         Plot the histogram
@@ -1357,53 +1799,58 @@
         Command-line arguments: ``[kwargs]``
 
         Plot the histogram weights as a function of the bin
         representative values. Some useful kwargs (which apply for all
         three object types) are color (c), dashes, linestyle (ls),
         linewidth (lw), marker, markeredgecolor (mec), markeredgewidth
         (mew), markerfacecolor (mfc), markerfacecoloralt (mfcalt),
-        markersize (ms). For example: \"o2graph -create x 0 10 0.2
-        -function sin(x) y -plot x y lw=0,marker='+' -show\". This
-        command uses the matplotlib plot() function, see
+        markersize (ms). For example::
+
+            o2graph -create table x grid:0,10,0.01 \\
+            -function "abs(sin(x))" y -to-hist y 20 \\
+            -plot "lw=0,marker=+" -show
+
+        This command uses the matplotlib plot() function, see
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
         for information and keyword arguments. This command does not
         yet support the matplotlib format parameter.
 
         For objects of type ``vector<contour_line>``:
 
         Plot the contour lines.
 
         Command-line arguments: ``[kwargs]``
 
         Plot the set of contour lines. Some useful kwargs (which apply
         for all three object types) are color (c), dashes, linestyle
         (ls), linewidth (lw), marker, markeredgecolor (mec),
         markeredgewidth (mew), markerfacecolor (mfc),
-        markerfacecoloralt (mfcalt), markersize (ms). For example:
-        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
-        lw=0,marker='+' -show\". This command uses the matplotlib
-        plot() function, see
+        markerfacecoloralt (mfcalt), markersize (ms). For example::
+        
+            o2graph -create table3d x grid:0,1,0.02 y grid:0,1,0.02 z \\
+            "(exp(-(x-0.2)^2/0.1)+exp(-(x-0.9)^2/0.1))*exp(-(y-0.4)^2/0.1)" \\
+            -contours 0.5 z -plot "lw=2" -show 
+
+        This command uses the matplotlib plot() function, see
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
         for information and keyword arguments. This command does not
         yet support the matplotlib format parameter.
 
         For objects of type ``prob_dens_mdim_amr``:
 
         Plot the probability distribution.
 
         Command-line arguments: ``[kwargs]``
 
         Plot the set of contour lines. Some useful kwargs (which apply
         for all three object types) are color (c), dashes, linestyle
         (ls), linewidth (lw), marker, markeredgecolor (mec),
         markeredgewidth (mew), markerfacecolor (mfc),
-        markerfacecoloralt (mfcalt), markersize (ms). For example:
-        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
-        lw=0,marker='+' -show\". This command uses the matplotlib
-        plot() function, see
+        markerfacecoloralt (mfcalt), markersize (ms). This command
+        uses the matplotlib plot() function, see
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
         for information and keyword arguments. This command does not
         yet support the matplotlib format parameter.
 
         """
 
         curr_type=o2scl_get_type(o2scl,amp,self.link2)
@@ -1422,22 +1869,26 @@
 
             # End of section for 'table' type
             
         elif curr_type==b'vec_vec_double':
             
             amt=acol_manager(self.link2,amp)
             vvd=amt.get_vvdouble_obj()
-            
-            if len(args)<2 or args[1]=='none':
+
+            if len(args)<2:
                 self.plot([vvd,int(args[0])])
             elif len(args)<3:
                 self.plot([vvd,int(args[0]),int(args[1])])
             else:
-                self.plot([vvd,int(args[0]),int(args[1])],
-                          **string_to_dict(args[2]))
+                if args[1]=='none':
+                    self.plot([vvd,int(args[0])],
+                              **string_to_dict(args[2]))
+                else:
+                    self.plot([vvd,int(args[0]),int(args[1])],
+                              **string_to_dict(args[2]))
 
             failed=False
 
             # End of section for 'vec_vec_double' type
             
         elif curr_type==b'hist':
 
@@ -1506,20 +1957,20 @@
                 wy=m2.weight
                 w=right-left
                 h=upper-lower
                 print('%d %7.6e %7.6e %7.6e %7.6e %7.6e %7.6e' %
                       (i,left,lower,w,h,fvy,wy))
 
                 if len(args)<4:
-                    r=patches.Rectangle((left,lower),w,h,0.0,
+                    r=patches.Rectangle((left,lower),w,h,angle=0.0,
                                         alpha=1,fill=None,lw=1)
                     self.axes.add_patch(r)
                 else:
                     strtemp='alpha='+str(fvy.value)+','+args[3]
-                    r=patches.Rectangle((left,lower),w,h,0.0,
+                    r=patches.Rectangle((left,lower),w,h,angle=0.0,
                                         **string_to_dict(strtemp))
                     self.axes.add_patch(r)
                             
             # End of section for 'prob_dens_mdim_amr' type
         elif curr_type==b'vector<contour_line>':
 
             amt=acol_manager(self.link2,amp)
@@ -1571,35 +2022,39 @@
         #if self.yset==True:
         #    self.axes.set_ylim(self.ylo,self.yhi)
                                  
         # End of function o2graph_plotter::plot_o2graph()
         return
                                  
     def plot_color(self,o2scl,amp,link,args):
-        """
-        Documentation for o2graph command ``plot-color``:
+        """Documentation for o2graph command ``plot-color``:
 
         For objects of type ``table``:
 
         Plot three columns, using the third for the color
 
         Command-line arguments: ``<x> <y> <c> <cmap> [kwargs]``
 
         Plot column <y> versus
         column <x> using column <c> to specify the line color.
         Some useful kwargs are color (c), dashes,
         linestyle (ls), linewidth (lw), marker, markeredgecolor (mec),
         markeredgewidth (mew), markerfacecolor (mfc),
-        markerfacecoloralt (mfcalt), markersize (ms). For example:
-        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
-        lw=0,marker='+' -show\". This command uses the matplotlib
-        plot() function, see
+        markerfacecoloralt (mfcalt), markersize (ms). For example::
+
+            o2graph -create x 0 10 0.2 -function sin(x) y -plot x y \\
+            lw=0,marker='+' -show
+
+        This command uses the matplotlib plot() function, see
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
         for information and keyword arguments. This command does not
         yet support the matplotlib format parameter.
+
+        If a cmyt colormap is used, then the ``cmyt`` Python package is
+        required.
         """
         
         if len(args)<4:
             raise ValueError('Function plot_color() requires four values '+
                              'for the args list.')
         
         curr_type=o2scl_get_type(o2scl,amp,self.link2)
@@ -1611,14 +2066,16 @@
             amt=acol_manager(self.link2,amp)
             tab=amt.get_table_obj()
             xv=tab[force_bytes(args[0])]
             yv=tab[force_bytes(args[1])]
             zv=tab[force_bytes(args[2])]
             
             cmap=args[3]
+            if args[3][0:5]=='cmyt.':
+                import cmyt
 
             if failed==False:
 
                 if self.logx:
                     for i in range(0,len(xv)):
                         xv[i]=math.log10(xv)
                 if self.logy:
@@ -2661,35 +3118,37 @@
                 self.zlo=gridz[0]
                 self.zhi=gridz[nz-1]
                 self.zset=True
                 print('o2graph_plotter:yt-add-vol: axis limits:\n ',
                       '%7.6e %7.6e %7.6e %7.6e %7.6e %7.6e' % (
                           self.xlo,self.xhi,
                           self.ylo,self.yhi,self.zlo,self.zhi))
-            
+
             arr=numpy.ctypeslib.as_array(data,shape=(nx,ny,nz))
+            arr3=arr.reshape((nx,ny,nz))
+            
             self.yt_volume_data.append(numpy.copy(arr))
             # Rescale to the internal coordinate system
             bbox=numpy.array([[(gridx[0]-self.xlo)/(self.xhi-self.xlo),
                                (gridx[nx-1]-self.xlo)/(self.xhi-self.xlo)],
                               [(gridy[0]-self.ylo)/(self.yhi-self.ylo),
                                (gridy[ny-1]-self.ylo)/(self.yhi-self.ylo)],
                               [(gridz[0]-self.zlo)/(self.zhi-self.zlo),
                                (gridz[nz-1]-self.zlo)/(self.zhi-self.zlo)]])
             self.yt_volume_bbox.append(numpy.copy(bbox))
-            arr2=self.yt_volume_data[len(self.yt_volume_data)-1]
             bbox2=self.yt_volume_bbox[len(self.yt_volume_bbox)-1]
 
             func=yt.load_uniform_grid
-            self.yt_data_sources.append(func(dict(density=arr2),
-                                             arr2.shape,bbox=bbox2))
+            self.yt_data_sources.append(func(dict(density=arr3),
+                                             (nx,ny,nz),bbox=bbox2))
             ds=self.yt_data_sources[len(self.yt_data_sources)-1]
 
-            self.yt_vols.append(create_volume_source(ds,field=('gas',
-                                                               'density')))
+            cvs=create_volume_source
+            self.yt_vols.append(cvs(ds,field=('gas','density')))
+                                              
             vol=self.yt_vols[len(self.yt_vols)-1]
             vol.log_field=False
 
             # Setup the transfer function
             if self.yt_tf!=0:
                 vol.set_transfer_function(self.yt_tf)
                 print(self.yt_tf)
@@ -2824,14 +3283,15 @@
         If the third argument has an additional ``r`` suffix, then the
         animation will be reversed, so that the first frame
         corresponds to the largest value of the grid for the
         associated index.
 
         Experimental.
 
+        This command requires the installation of ``ffmpeg``. 
         """
 
         import matplotlib.pyplot as plot
         
         curr_type=o2scl_get_type(o2scl,amp,self.link2)
 
         if curr_type==b'tensor_grid':
@@ -3072,31 +3532,21 @@
                 # End of loop, continue to next frame
 
             # Now after loop, compile frames into a movie
             prefix='/tmp/dpa_'
             suffix='.png'
             mov_fname=args[3]
             if n_frames>=1000:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%04d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
+                self.mp4([prefix+'%04d'+suffix,mov_fname])
             elif n_frames>=100:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%03d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
+                self.mp4([prefix+'%03d'+suffix,mov_fname])
             elif n_frames>=10:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%02d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
+                self.mp4([prefix+'%02d'+suffix,mov_fname])
             else:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%01d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
-            print('ffmpeg command:',cmd)
-            os.system(cmd)
+                self.mp4([prefix+'%01d'+suffix,mov_fname])
 
             # End of "if curr_type==b'tensor_grid':"
                 
         # End of function o2graph_plotter::den_plot_anim()
         return
         
     def help_func(self,o2scl,amp,link,args):
@@ -3141,25 +3591,26 @@
         # extra list
         if match==False:
             for line in extra_list:
                 if ((curr_type==line[0] or
                      curr_type==force_bytes(line[0])) and
                     cmd==line[1]):
                     match=True
-                    reformat_python_docs_type(curr_type,cmd,line[2],amp,self.link2)
+                    reformat_python_docs_type(curr_type,cmd,line[2],amp,
+                                              self.link2)
 
         # Handle the case of an o2graph command from the
         # extra list without a matching type
         if match==False:
             for line in extra_list:
                 if cmd==line[1]:
                     match=True
                     print('\n'+str_line)
-                    #print('here2')
-                    reformat_python_docs_type(line[0],cmd,line[2],amp,self.link2)
+                    reformat_python_docs_type(line[0],cmd,line[2],amp,
+                                              self.link2)
                     
         # If we haven't matched yet, check for get/set parameters
         if match==False:
             for line in param_list:
                 if cmd==line[0]:
                     match=True
                     print('O2graph parameter modified by the get and set',
@@ -3245,15 +3696,14 @@
                                            self.link2,True)
                 full_list.append([force_bytes(line2[0]),
                                   force_bytes(short)])
 
             if curr_type!='':
                 for line in extra_list:
                     if force_bytes(line[0])==curr_type:
-                        #print('here3')
                         short=reformat_python_docs_type(curr_type,line[1],
                                                         line[2],amp,
                                                         self.link2,True)
                         full_list.append([force_bytes(line[1]),
                                           force_bytes(short)])
 
             full_list2=sorted(full_list,key=lambda x: x[0])
@@ -4121,18 +4571,17 @@
         
         """
         
         import matplotlib.pyplot as plot
         
         if len(self.yt_ann)==0:
             
-            # No animation and no annotation, so just call
-            # scene.save()
+            # No annotation, so just call scene.save()
             print('o2graph:yt_save_annotate: Calling yt_scene.save()',
-                  'with filename',fname)
+                  'with filename',fname,self.yt_sigma_clip)
             self.yt_scene.save(fname,sigma_clip=self.yt_sigma_clip)
             
         else:
 
             # This segment of code is based off of yt's save_annotate()
             # function.
             self.yt_scene.render()
@@ -4149,16 +4598,16 @@
             if self.verbose>1:
                 print('Done adding annotations:')
             #self.text(0.1,0.9,'x',color='w',fontsize=self.font*1.25,
                 #transform=tf)
             self.canvas_flag=False
             #axt.axes.text(0.1,0.9,'test',color='w',transform=tf,
             #fontsize=self.font*1.25)
-            from yt.visualization._mpl_imports import FigureCanvasAgg
-            canvast=FigureCanvasAgg(self.yt_scene._render_figure)
+            canvast=get_canvas(self.yt_scene._render_figure,
+                               fname)
             self.yt_scene._render_figure.canvas=canvast
             #self.yt_scene._render_figure.tight_layout(pad=0.0)
             plot.subplots_adjust(left=0.0,bottom=0.0,
                                  right=1.0,top=1.0)
             if self.verbose>0:
                 print('o2graph:yt-render: Calling',
                       'savefig() with annotations and file',fname,'.')
@@ -4372,14 +4821,16 @@
         each frame will be stored. If yt_path is not empty and a movie
         filename is given, then ffmpeg will be used to combine the
         frames into an mp4 file.
 
         The keyword argument ``mov_fname`` specifies the output
         movie file (if an animation is specified with ``yt-path``).
         If empty, the filename ``o2graph.mp4`` is used. 
+
+        This command requires the installation of ``ffmpeg``. 
         """
 
         if self.yt_scene==0:
             print('Cannot perform a yt render without a scene.')
             return
         
         # AWS 10/14/19 the call to save() below does
@@ -4434,18 +4885,22 @@
                     print('yaw: camera pos, foc:',pos,foc)
                     print('yaw: camera nor, wid:',nor,wid)
                     
                     for ifr in range(0,n_frames_move):
                         
                         i_frame=i_frame+1
                         
-                        print(self.yt_camera)
-                        print('normal_vector:',self.yt_camera.normal_vector)
-                        print('north_vector:',self.yt_camera.north_vector)
-                        print('origin:',self.yt_camera.lens.origin)
+                        if self.verbose>=2:
+                            print(self.yt_camera)
+                            print('normal_vector:',
+                                  self.yt_camera.normal_vector)
+                            print('north_vector:',
+                                  self.yt_camera.north_vector)
+                            print('origin:',
+                                  self.yt_camera.lens.origin)
 
                         # We can't use the yt yaw() function because
                         # it modifies the camera properties in an
                         # undocumented way. 
                         
                         from yt.units.yt_array import YTArray
                         rv=YTArray([0,0,1])
@@ -4471,18 +4926,19 @@
                         # Move camera
                         self.yt_camera.position=[pos[0],pos[1],pos[2]]
                         self.yt_camera.focus=[foc[0],foc[1],foc[2]]
                         self.yt_camera.north_vector=[nor[0],nor[1],nor[2]]
                         self.yt_camera.width=[wid[0],wid[1],wid[2]]
                         self.yt_camera.switch_orientation()
                             
-                        print('Camera width [%0.6e,%0.6e,%0.6e]' %
-                              (self.yt_camera.width[0],
-                               self.yt_camera.width[1],
-                               self.yt_camera.width[2]))
+                        if self.verbose>=2:
+                            print('Camera width [%0.6e,%0.6e,%0.6e]' %
+                                  (self.yt_camera.width[0],
+                                   self.yt_camera.width[1],
+                                   self.yt_camera.width[2]))
                             
                         # Update text objects
                         self.yt_update_text()
 
                         # Save new frame
                         fname2=self._make_fname(prefix,suffix,
                                                 i_frame,n_frames)
@@ -4745,35 +5201,21 @@
             # -r is rate (in frames/sec), -f is format, -vcodec is
             # video codec (apparently 420p works well with quicktime),
             # -pix_fmt sepcifies the pixel format, -crf is the quality
             # (15-25 recommended) -y forces overwrite of the movie
             # file if it already exists
             
             if n_frames>=1000:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%04d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
+                self.mp4([prefix+'%04d'+suffix,mov_fname],loop=loop)
             elif n_frames>=100:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%03d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
+                self.mp4([prefix+'%03d'+suffix,mov_fname],loop=loop)
             elif n_frames>=10:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%02d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
+                self.mp4([prefix+'%02d'+suffix,mov_fname],loop=loop)
             else:
-                cmd=('ffmpeg -y -r 10 -f image2 -i '+
-                     prefix+'%01d'+suffix+' -vcodec libx264 '+
-                     '-crf 25 -pix_fmt yuv420p '+mov_fname)
-
-            if loop==True:
-                cmd=cmd+' -stream_loop -1'
-                
-            print('ffmpeg command:',cmd)
-            os.system(cmd)
+                self.mp4([prefix+'%01d'+suffix,mov_fname],loop=loop)
 
             # End of else for 'if len(self.yt_path)==0:'
             
         # End of function o2graph_plotter::yt_render()
         return
 
     def parse_string_list(self,strlist,o2scl,amp,link):
@@ -4872,15 +5314,16 @@
                     if self.verbose>2:
                         print('Process set.')
                         print('args:',strlist[ix:ix_next])
                         
                     if ix_next-ix<3:
                         print('Not enough parameters for set option.')
                     else:
-                        self.set_wrapper(o2scl,amp,self.link2,strlist[ix+1:ix_next])
+                        self.set_wrapper(o2scl,amp,self.link2,
+                                         strlist[ix+1:ix_next])
                         
                 elif cmd_name=='ell-max':
 
                     if self.verbose>2:
                         print('Process ell-max.')
                         print('args:',strlist[ix:ix_next])
                         
@@ -4959,15 +5402,16 @@
                     if self.verbose>2:
                         print('Process yt-scatter.')
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<4:
                         print('Not enough parameters for yt-scatter.')
                     else:
-                        self.yt_scatter(o2scl,amp,self.link2,strlist[ix+1:ix_next])
+                        self.yt_scatter(o2scl,amp,
+                                        self.link2,strlist[ix+1:ix_next])
                                                     
                 elif cmd_name=='yt-path':
 
                     if self.verbose>2:
                         print('Process yt-path.')
                         print('args:',strlist[ix:ix_next])
 
@@ -5074,14 +5518,36 @@
                         y1=float(eval(strlist[ix+2]))
                         z1=float(eval(strlist[ix+3]))
                         x2=float(eval(strlist[ix+4]))
                         y2=float(eval(strlist[ix+5]))
                         z2=float(eval(strlist[ix+6]))
                         self.yt_line([x1,y1,z1],[x2,y2,z2])
                                                     
+                elif cmd_name=='yt-point':
+
+                    if self.verbose>2:
+                        print('Process yt-point.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix<5:
+                        print('Not enough parameters for yt-point.')
+                    elif ix_next-ix>5:
+                        x1=float(eval(strlist[ix+1]))
+                        y1=float(eval(strlist[ix+2]))
+                        z1=float(eval(strlist[ix+3]))
+                        rad=float(eval(strlist[ix+4]))
+                        self.yt_point([x1,y1,z1],rad,
+                                      **string_to_dict(strlist[ix+5]))
+                    else:
+                        x1=float(eval(strlist[ix+1]))
+                        y1=float(eval(strlist[ix+2]))
+                        z1=float(eval(strlist[ix+3]))
+                        rad=float(eval(strlist[ix+4]))
+                        self.yt_point([x1,y1,z1],rad)
+                                                    
                 elif cmd_name=='yt-box':
 
                     if self.verbose>2:
                         print('Process yt-box.')
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<7:
@@ -5168,15 +5634,253 @@
                             tstr=("<class 'yt.visualization.volume_"+
                                   "rendering.render_source.")
                             print('yt-source-list',icnt,key,
                                   str(type(value)).replace(tstr,"<class '..."))
                             icnt=icnt+1
                         if icnt==0:
                             print('No yt sources.')
-                    
+
+                elif cmd_name=='td-arrow':
+
+                    if self.verbose>2:
+                        print('Process td-arrow.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix>=9:
+                        self.td_arrow(float(strlist[ix+1]),
+                                      float(strlist[ix+2]),
+                                      float(strlist[ix+3]),
+                                      float(strlist[ix+4]),
+                                      float(strlist[ix+5]),
+                                      float(strlist[ix+6]),
+                                      strlist[ix+7],
+                                      mat=strlist[ix+8])
+                    elif ix_next-ix>=8:
+                        self.td_arrow(float(strlist[ix+1]),
+                                      float(strlist[ix+2]),
+                                      float(strlist[ix+3]),
+                                      float(strlist[ix+4]),
+                                      float(strlist[ix+5]),
+                                      float(strlist[ix+6]),
+                                      strlist[ix+7])
+                    else:
+                        print('Not enough arguments for td-arrow.')
+
+                elif cmd_name=='td-axis-label':
+
+                    if self.verbose>2:
+                        print('Process td-axis-label.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix>=4:
+                        self.td_axis_label(strlist[ix+1],
+                                           strlist[ix+2],
+                                           **string_to_dict2
+                                           (strlist[ix+3],
+                                            list_of_floats=['rough','metal']))
+                    elif ix_next-ix>=3:
+                        self.td_axis_label(strlist[ix+1],
+                                           strlist[ix+2])
+                    else:
+                        print('Not enough arguments for td-axis-label.')
+
+                elif cmd_name=='td-axis':
+
+                    if self.verbose>2:
+                        print('Process td-axis.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix>=5:
+                        prefix=strlist[ix+4]
+                        self.td_arrow(0,0,0,1,0,0,'x_axis')
+                        self.td_arrow(0,0,0,0,1,0,'y_axis')
+                        self.td_arrow(0,0,0,0,0,1,'z_axis')
+                        self.td_axis_label('x',strlist[ix+1],
+                                           png_file=prefix+'xtitle.png')
+                        self.td_axis_label('y',strlist[ix+2],
+                                           png_file=prefix+'ytitle.png')
+                        self.td_axis_label('z',strlist[ix+3],
+                                           png_file=prefix+'ztitle.png')
+                    elif ix_next-ix>=4:
+                        self.td_arrow(0,0,0,1,0,0,'x_axis')
+                        self.td_arrow(0,0,0,0,1,0,'y_axis')
+                        self.td_arrow(0,0,0,0,0,1,'z_axis')
+                        self.td_axis_label('x',strlist[ix+1])
+                        self.td_axis_label('y',strlist[ix+2])
+                        self.td_axis_label('z',strlist[ix+3])
+                    else:
+                        print('Not enough arguments for td-axis.')
+                        
+                elif cmd_name=='td-den-plot':
+
+                    if self.verbose>2:
+                        print('Process td-den-plot.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix==2:
+                        self.td_den_plot(o2scl,amp,[strlist[ix+1]])
+                    elif ix_next-ix>=3:
+                        self.td_den_plot(o2scl,amp,[strlist[ix+1]],
+                                         **string_to_dict2(strlist[ix+2]))
+                    else:
+                        print('Not enough arguments for td-den-plot.')
+
+                elif cmd_name=='td-scatter':
+
+                    if self.verbose>2:
+                        print('Process td-scatter.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix==4:
+                        self.td_scatter(o2scl,amp,[strlist[ix+1],
+                                                   strlist[ix+2],
+                                                   strlist[ix+3]])
+                    elif ix_next-ix==5:
+                        self.td_scatter(o2scl,amp,
+                                        [strlist[ix+1],strlist[ix+2],
+                                         strlist[ix+3]],
+                                        **string_to_dict2(strlist[ix+4],
+                                                          list_of_ints=
+                                                          ['n_subdiv'],
+                                                          list_of_floats=
+                                                          ['r']))
+                    elif ix_next-ix==7:
+                        self.td_scatter(o2scl,amp,[strlist[ix+1],
+                                                   strlist[ix+2],
+                                                   strlist[ix+3],
+                                                   strlist[ix+4],
+                                                   strlist[ix+5],
+                                                   strlist[ix+6]])
+                    elif ix_next-ix>=8:
+                        self.td_scatter(o2scl,amp,
+                                        [strlist[ix+1],strlist[ix+2],
+                                         strlist[ix+3],strlist[ix+4],
+                                         strlist[ix+5],strlist[ix+6]],
+                                         **string_to_dict2(strlist[ix+7],
+                                                           list_of_ints=
+                                                           ['n_subdiv'],
+                                                           list_of_floats=
+                                                           ['r']))
+                    else:
+                        print('Not enough arguments for td-scatter.')
+
+                elif cmd_name=='td-icos':
+
+                    if self.verbose>2:
+                        print('Process td-icos.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix==4:
+                        self.td_icos([strlist[ix+1],strlist[ix+2],
+                                      strlist[ix+3]])
+                    elif ix_next-ix>=5:
+                        self.td_icos([strlist[ix+1],strlist[ix+2],
+                                      strlist[ix+3]],
+                                     **string_to_dict2(strlist[ix+4],
+                                                       list_of_ints=
+                                                       ['n_subdiv'],
+                                                       list_of_floats=
+                                                       ['r']))
+                    else:
+                        print('Not enough arguments for td-icos.')
+
+                elif cmd_name=='td-pgram':
+
+                    if self.verbose>2:
+                        print('Process td-pgram.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix==10:
+                        self.td_pgram(float(strlist[ix+1]),
+                                      float(strlist[ix+2]),
+                                      float(strlist[ix+3]),
+                                      float(strlist[ix+4]),
+                                      float(strlist[ix+5]),
+                                      float(strlist[ix+6]),
+                                      float(strlist[ix+7]),
+                                      float(strlist[ix+8]),
+                                      float(strlist[ix+9]))
+                    elif ix_next-ix>=11:
+                        self.td_pgram(float(strlist[ix+1]),
+                                      float(strlist[ix+2]),
+                                      float(strlist[ix+3]),
+                                      float(strlist[ix+4]),
+                                      float(strlist[ix+5]),
+                                      float(strlist[ix+6]),
+                                      float(strlist[ix+7]),
+                                      float(strlist[ix+8]),
+                                      float(strlist[ix+9]),
+                                      **string_to_dict2(strlist[ix+10],
+                                                        list_of_bools=
+                                                        ['force_rect',
+                                                         'match_txt']))
+                    else:
+                        print('Not enough arguments for td-pgram.')
+
+                elif cmd_name=='td-mat':
+
+                    if self.verbose>2:
+                        print('Process td-mat.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix==5:
+                        self.td_mat(strlist[ix+1],
+                                    float(strlist[ix+2]),
+                                    float(strlist[ix+3]),
+                                    float(strlist[ix+4]))
+                    elif ix_next-ix>=6:
+                        self.td_mat(strlist[ix+1],
+                                    float(strlist[ix+2]),
+                                    float(strlist[ix+3]),
+                                    float(strlist[ix+4]),
+                                    **string_to_dict2(strlist[ix+5],
+                                                      list_of_bools=
+                                                      ['ds'],
+                                                      list_of_floats=
+                                                      ['metal','rough',
+                                                       'alpha','efr',
+                                                       'efg','efb']))
+                    else:
+                        print('Not enough arguments for td-mat.')
+
+                elif cmd_name=='bl-yaw-mp4':
+
+                    if self.verbose>2:
+                        print('Process bl-yaw-mp4.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix>=3:
+                        self.bl_yaw_mp4(int(strlist[ix+1]),
+                                        strlist[ix+2])
+                    else:
+                        print('Not enough arguments for bl-yaw-mp4.')
+
+                elif cmd_name=='bl-import':
+
+                    if self.verbose>2:
+                        print('Process bl-import.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix>=2:
+                        self.bl_import(strlist[ix+1])
+                    else:
+                        print('Not enough arguments for bl-import.')
+
+                elif cmd_name=='bl-six-mp4':
+
+                    if self.verbose>2:
+                        print('Process bl-six-mp4.')
+                        print('args:',strlist[ix:ix_next])
+
+                    if ix_next-ix>=3:
+                        self.bl_six_mp4(int(strlist[ix+1]),
+                                        strlist[ix+2])
+                    else:
+                        print('Not enough arguments for bl-six-mp4.')
+
                 elif cmd_name=='yt-axis':
 
                     if self.verbose>2:
                         print('Process yt-axis.')
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<2:
@@ -5216,15 +5920,16 @@
 
                 elif cmd_name=='plot':
                     
                     if self.verbose>2:
                         print('Process plot.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.plot_o2graph(o2scl,amp,strlist[ix+1:ix_next],self.link2)
+                    self.plot_o2graph(o2scl,amp,strlist[ix+1:ix_next],
+                                      self.link2)
 
                 elif cmd_name=='plot-color':
                     
                     if self.verbose>2:
                         print('Process plot-color.')
                         print('args:',strlist[ix:ix_next])
 
@@ -5300,15 +6005,15 @@
                 elif cmd_name=='kde-2d-plot':
                     
                     if self.verbose>2:
                         print('Process kde-2d-plot.')
                         print('args:',strlist[ix:ix_next])
 
                     self.kde_2d_plot(o2scl,amp,strlist[ix+1:ix_next],
-                                  self.link2)
+                                     self.link2)
                 
                 elif cmd_name=='to-kde':
                     
                     if self.verbose>2:
                         print('Process to-kde.')
                         print('args:',strlist[ix:ix_next])
 
@@ -5320,14 +6025,23 @@
                     if self.verbose>2:
                         print('Process den-plot-rgb.')
                         print('args:',strlist[ix:ix_next])
 
                     self.den_plot_rgb_o2graph(o2scl,amp,self.link2,
                                               strlist[ix+1:ix_next])
                 
+                elif cmd_name=='gltf':
+
+                    if self.verbose>2:
+                        print('Process gltf.')
+                        print('args:',strlist[ix:ix_next])
+
+                    self.gltf_o2graph(o2scl,amp,self.link2,
+                                              strlist[ix+1:ix_next])
+                
                 elif cmd_name=='den-plot-anim':
                     
                     if self.verbose>2:
                         print('Process den-plot-anim.')
                         print('args:',strlist[ix:ix_next])
 
                     self.den_plot_anim(o2scl,amp,self.link2,
@@ -5799,28 +6513,14 @@
                         print('args:',strlist[ix:ix_next])
                 else:
                     if self.verbose>2:
                         print('Process acol command '+cmd_name+'.')
                         print('args:',strlist[ix:ix_next])
                     self.gen_acol(o2scl,amp,self.link2,cmd_name,
                                   strlist[ix+1:ix_next])
-                    # AWS, 3/9/23: I had to take this out, I think
-                    # because it's not supported in the older version
-                    # of HDF5 which is used in Ubuntu, but at some
-                    # point I can put it back.
-                    #
-                    # if (cmd_name=='v' or cmd_name=='version'):
-                    #     try:
-                    #         import h5py
-                    #     except:
-                    #         print('\n(Import h5py failed.)')
-                    #     else:
-                    #         vv=h5py.h5.get_libversion()
-                    #         print('\nHDF5 version from h5py:',
-                    #               vv[0],vv[1],vv[2])
                     
                 # Increment to the next option
                 ix=ix_next
                 
             if self.verbose>2:
                 print('Going to next argument in parse_string_list().')
```

### Comparing `o2sclpy-0.928/o2sclpy/other.py` & `o2sclpy-0.929/o2sclpy/other.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
   ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2023, Andrew W. Steiner
+  Copyright (C) 2020-2024, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -27,15 +27,15 @@
 
 from o2sclpy.base import *
 
 class slack_messenger:
     """
     Python interface for O2scl class ``slack_messenger``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/slack_messenger.html .
+    https://awsteiner.org/code/o2scl/html/class/slack_messenger.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -270,15 +270,15 @@
         return cls(link,f(p_channel_,p_username_,p_url_,p_mpi_time))
 
 
 class quadratic_real_coeff_gsl:
     """
     Python interface for O2scl class ``quadratic_real_coeff_gsl``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/quadratic_real_coeff_gsl.html .
+    https://awsteiner.org/code/o2scl/html/class/quadratic_real_coeff_gsl.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -358,15 +358,15 @@
         return ret
 
 
 class quadratic_real_coeff_gsl2:
     """
     Python interface for O2scl class ``quadratic_real_coeff_gsl2<>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/quadratic_real_coeff_gsl2<>.html .
+    https://awsteiner.org/code/o2scl/html/class/quadratic_real_coeff_gsl2<>.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -446,15 +446,15 @@
         return ret
 
 
 class cubic_real_coeff_cern:
     """
     Python interface for O2scl class ``cubic_real_coeff_cern<>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/cubic_real_coeff_cern<>.html .
+    https://awsteiner.org/code/o2scl/html/class/cubic_real_coeff_cern<>.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -538,15 +538,15 @@
         return ret,r1_conv.value
 
 
 class cubic_real_coeff_gsl:
     """
     Python interface for O2scl class ``cubic_real_coeff_gsl``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/cubic_real_coeff_gsl.html .
+    https://awsteiner.org/code/o2scl/html/class/cubic_real_coeff_gsl.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -630,15 +630,15 @@
         return ret,r1_conv.value
 
 
 class quartic_real_coeff_cern:
     """
     Python interface for O2scl class ``quartic_real_coeff_cern<>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/quartic_real_coeff_cern<>.html .
+    https://awsteiner.org/code/o2scl/html/class/quartic_real_coeff_cern<>.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -726,15 +726,15 @@
         return ret
 
 
 class fermi_dirac_integ_gsl:
     """
     Python interface for O2scl class ``fermi_dirac_integ_gsl``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/fermi_dirac_integ_gsl.html .
+    https://awsteiner.org/code/o2scl/html/class/fermi_dirac_integ_gsl.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -842,15 +842,15 @@
         return ret
 
 
 class bessel_K_exp_integ_gsl:
     """
     Python interface for O2scl class ``bessel_K_exp_integ_gsl``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/bessel_K_exp_integ_gsl.html .
+    https://awsteiner.org/code/o2scl/html/class/bessel_K_exp_integ_gsl.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -934,15 +934,15 @@
         return ret
 
 
 class hist:
     """
     Python interface for O2scl class ``hist``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/hist.html .
+    https://awsteiner.org/code/o2scl/html/class/hist.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1246,15 +1246,15 @@
         return
 
 
 class hist_2d:
     """
     Python interface for O2scl class ``hist_2d``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/hist_2d.html .
+    https://awsteiner.org/code/o2scl/html/class/hist_2d.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1602,15 +1602,15 @@
         return
 
 
 class contour_line:
     """
     Python interface for O2scl class ``contour_line``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/contour_line.html .
+    https://awsteiner.org/code/o2scl/html/class/contour_line.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1731,15 +1731,15 @@
         return
 
 
 class vector_contour_line:
     """
     Python interface for O2scl class ``std::vector<contour_line>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/std::vector<contour_line>.html .
+    https://awsteiner.org/code/o2scl/html/class/std::vector<contour_line>.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1839,15 +1839,15 @@
         return self.length()
      
 
 class contour:
     """
     Python interface for O2scl class ``contour``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/contour.html .
+    https://awsteiner.org/code/o2scl/html/class/contour.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1984,19 +1984,214 @@
         """
         func=self._link.o2scl.o2scl_contour_calc_contours
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,clines._ptr)
         return
 
 
+class prob_dens_func:
+    """
+    Python interface for O2scl class ``prob_dens_func``,
+    See
+    https://awsteiner.org/code/o2scl/html/class/prob_dens_func.html .
+    """
+
+    _ptr=0
+    _link=0
+    _owner=True
+
+    def __init__(self,link,pointer=0):
+        """
+        Init function for class prob_dens_func
+
+        | Parameters:
+        | *link* :class:`linker` object
+        | *pointer* ``ctypes.c_void_p`` pointer
+
+        """
+
+        if pointer==0:
+            f=link.o2scl.o2scl_create_prob_dens_func
+            f.restype=ctypes.c_void_p
+            f.argtypes=[]
+            self._ptr=f()
+        else:
+            self._ptr=pointer
+            self._owner=False
+        self._link=link
+        return
+
+    def __del__(self):
+        """
+        Delete function for class prob_dens_func
+        """
+
+        if self._owner==True:
+            f=self._link.o2scl.o2scl_free_prob_dens_func
+            f.argtypes=[ctypes.c_void_p]
+            f(self._ptr)
+            self._owner=False
+            self._ptr=0
+        return
+
+    def __copy__(self):
+        """
+        Shallow copy function for class prob_dens_func
+        
+        Returns: prob_dens_func object
+        """
+
+        new_obj=type(self)(self._link,self._ptr)
+        return new_obj
+
+    def pdf(self,x):
+        """
+        | Parameters:
+        | *x*: ``double``
+        | Returns: a Python float
+        """
+        func=self._link.o2scl.o2scl_prob_dens_func_pdf
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        ret=func(self._ptr,x)
+        return ret
+
+    def log_pdf(self,x):
+        """
+        | Parameters:
+        | *x*: ``double``
+        | Returns: a Python float
+        """
+        func=self._link.o2scl.o2scl_prob_dens_func_log_pdf
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        ret=func(self._ptr,x)
+        return ret
+
+    def cdf(self,x):
+        """
+        | Parameters:
+        | *x*: ``double``
+        | Returns: a Python float
+        """
+        func=self._link.o2scl.o2scl_prob_dens_func_cdf
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        ret=func(self._ptr,x)
+        return ret
+
+    def invert_cdf(self,x):
+        """
+        | Parameters:
+        | *x*: ``double``
+        | Returns: a Python float
+        """
+        func=self._link.o2scl.o2scl_prob_dens_func_invert_cdf
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        ret=func(self._ptr,x)
+        return ret
+
+    def entropy(self):
+        """
+        | Returns: a Python float
+        """
+        func=self._link.o2scl.o2scl_prob_dens_func_entropy
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        return ret
+
+    def __getitem__(self):
+        """
+        """
+        func=self._link.o2scl.o2scl_prob_dens_func_getitem
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        return ret
+
+
+class prob_dens_gaussian(prob_dens_func):
+    """
+    Python interface for O2scl class ``prob_dens_gaussian``,
+    See
+    https://awsteiner.org/code/o2scl/html/class/prob_dens_gaussian.html .
+    """
+
+    def __init__(self,link,pointer=0):
+        """
+        Init function for class prob_dens_gaussian
+
+        | Parameters:
+        | *link* :class:`linker` object
+        | *pointer* ``ctypes.c_void_p`` pointer
+
+        """
+
+        if pointer==0:
+            f=link.o2scl.o2scl_create_prob_dens_gaussian
+            f.restype=ctypes.c_void_p
+            f.argtypes=[]
+            self._ptr=f()
+        else:
+            self._ptr=pointer
+            self._owner=False
+        self._link=link
+        return
+
+    def __del__(self):
+        """
+        Delete function for class prob_dens_gaussian
+        """
+
+        if self._owner==True:
+            f=self._link.o2scl.o2scl_free_prob_dens_gaussian
+            f.argtypes=[ctypes.c_void_p]
+            f(self._ptr)
+            self._owner=False
+            self._ptr=0
+        return
+
+    def __copy__(self):
+        """
+        Shallow copy function for class prob_dens_gaussian
+        
+        Returns: prob_dens_gaussian object
+        """
+
+        new_obj=type(self)(self._link,self._ptr)
+        return new_obj
+
+    def set_center(self,cent):
+        """
+        | Parameters:
+        | *cent*: ``double``
+        """
+        func=self._link.o2scl.o2scl_prob_dens_gaussian_set_center
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        func(self._ptr,cent)
+        return
+
+    def set_sigma(self,sigma):
+        """
+        | Parameters:
+        | *sigma*: ``double``
+        """
+        func=self._link.o2scl.o2scl_prob_dens_gaussian_set_sigma
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
+        func(self._ptr,sigma)
+        return
+
+
 class prob_dens_mdim:
     """
     Python interface for O2scl class ``prob_dens_mdim<std::vector<double>>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/prob_dens_mdim<std::vector<double>>.html .
+    https://awsteiner.org/code/o2scl/html/class/prob_dens_mdim<std::vector<double>>.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -2089,15 +2284,15 @@
         return
 
 
 class prob_dens_mdim_biv_gaussian(prob_dens_mdim):
     """
     Python interface for O2scl class ``prob_dens_mdim_biv_gaussian<std::vector<double>>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/prob_dens_mdim_biv_gaussian<std::vector<double>>.html .
+    https://awsteiner.org/code/o2scl/html/class/prob_dens_mdim_biv_gaussian<std::vector<double>>.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class prob_dens_mdim_biv_gaussian
 
         | Parameters:
@@ -2182,15 +2377,15 @@
         return ret
 
 
 class prob_dens_mdim_gaussian(prob_dens_mdim):
     """
     Python interface for O2scl class ``prob_dens_mdim_gaussian<>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/prob_dens_mdim_gaussian<>.html .
+    https://awsteiner.org/code/o2scl/html/class/prob_dens_mdim_gaussian<>.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class prob_dens_mdim_gaussian
 
         | Parameters:
@@ -2246,15 +2441,15 @@
         return ret
 
 
 class hypercube:
     """
     Python interface for O2scl class ``prob_dens_mdim_amr<>::hypercube``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/prob_dens_mdim_amr<>::hypercube.html .
+    https://awsteiner.org/code/o2scl/html/class/prob_dens_mdim_amr<>::hypercube.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -2422,15 +2617,15 @@
         return
 
 
 class std_vector_hypercube:
     """
     Python interface for O2scl class ``std::vector<prob_dens_mdim_amr<>::hypercube>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/std::vector<prob_dens_mdim_amr<>::hypercube>.html .
+    https://awsteiner.org/code/o2scl/html/class/std::vector<prob_dens_mdim_amr<>::hypercube>.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -2522,15 +2717,15 @@
         return
 
 
 class prob_dens_mdim_amr(prob_dens_mdim):
     """
     Python interface for O2scl class ``prob_dens_mdim_amr<>``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/prob_dens_mdim_amr<>.html .
+    https://awsteiner.org/code/o2scl/html/class/prob_dens_mdim_amr<>.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class prob_dens_mdim_amr
 
         | Parameters:
```

### Comparing `o2sclpy-0.928/o2sclpy/part.py` & `o2sclpy-0.929/o2sclpy/part.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
   ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2023, Andrew W. Steiner
+  Copyright (C) 2020-2024, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -432,17 +432,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,ax._ptr)
         return
 
 
 class fermion(part):
     """
-    Python interface for O\ :sub:`2`\ scl class ``fermion``,
+    Python interface for O2scl class ``fermion``,
     which is a typedef of ``fermion_tl<double>``. See
-    https://neutronstars.utk.edu/code/o2scl-dev/part/html/class/fermion_tl.html
+    https://awsteiner.org/code/o2scl-dev/part/html/class/fermion_tl.html
     .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class fermion
 
@@ -527,15 +527,15 @@
         return
 
 
 class quark(fermion):
     """
     Python interface for O2scl class ``quark``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/quark.html .
+    https://awsteiner.org/code/o2scl/html/class/quark.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class quark
 
         | Parameters:
@@ -1263,15 +1263,15 @@
         return
 
 
 class boson(part):
     """
     Python interface for O2scl class ``boson``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/boson.html .
+    https://awsteiner.org/code/o2scl/html/class/boson.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class boson
 
         | Parameters:
@@ -1335,15 +1335,15 @@
         return
 
 
 class boson_rel:
     """
     Python interface for O2scl class ``boson_rel``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/boson_rel.html .
+    https://awsteiner.org/code/o2scl/html/class/boson_rel.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -2225,426 +2225,14 @@
         func=self._link.o2scl.o2scl_deriv_thermo_base_squared_sound_speed
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
         ret=func(self._ptr,p._ptr,T)
         return ret
 
 
-class fermion_deriv_rel:
-    """
-    Python interface for class :ref:`fermion_deriv_rel <o2scl:fermion_deriv_rel_tl>`.
-    """
-
-    _ptr=0
-    _link=0
-    _owner=True
-
-    def __init__(self,link,pointer=0):
-        """
-        Init function for class fermion_deriv_rel
-
-        | Parameters:
-        | *link* :class:`linker` object
-        | *pointer* ``ctypes.c_void_p`` pointer
-
-        """
-
-        if pointer==0:
-            f=link.o2scl.o2scl_create_fermion_deriv_rel
-            f.restype=ctypes.c_void_p
-            f.argtypes=[]
-            self._ptr=f()
-        else:
-            self._ptr=pointer
-            self._owner=False
-        self._link=link
-        return
-
-    def __del__(self):
-        """
-        Delete function for class fermion_deriv_rel
-        """
-
-        if self._owner==True:
-            f=self._link.o2scl.o2scl_free_fermion_deriv_rel
-            f.argtypes=[ctypes.c_void_p]
-            f(self._ptr)
-            self._owner=False
-            self._ptr=0
-        return
-
-    def __copy__(self):
-        """
-        Shallow copy function for class fermion_deriv_rel
-        
-        Returns: fermion_deriv_rel object
-        """
-
-        new_obj=type(self)(self._link,self._ptr)
-        return new_obj
-
-    @property
-    def exp_limit(self):
-        """
-        Property of type ``ctypes.c_double``
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_get_exp_limit
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @exp_limit.setter
-    def exp_limit(self,value):
-        """
-        Setter function for fermion_deriv_rel::exp_limit .
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_set_exp_limit
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
-        func(self._ptr,value)
-        return
-
-    @property
-    def deg_limit(self):
-        """
-        Property of type ``ctypes.c_double``
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_get_deg_limit
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @deg_limit.setter
-    def deg_limit(self,value):
-        """
-        Setter function for fermion_deriv_rel::deg_limit .
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_set_deg_limit
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
-        func(self._ptr,value)
-        return
-
-    @property
-    def upper_limit_fac(self):
-        """
-        Property of type ``ctypes.c_double``
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_get_upper_limit_fac
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @upper_limit_fac.setter
-    def upper_limit_fac(self,value):
-        """
-        Setter function for fermion_deriv_rel::upper_limit_fac .
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_set_upper_limit_fac
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
-        func(self._ptr,value)
-        return
-
-    def get_unc(self):
-        """
-        Get object of type :class:`fermion_deriv`
-        """
-        func1=self._link.o2scl.o2scl_fermion_deriv_rel_get_unc
-        func1.restype=ctypes.c_void_p
-        func1.argtypes=[ctypes.c_void_p]
-        ptr=func1(self._ptr)
-        obj=fermion_deriv(self._link,ptr)
-        return obj
-
-    def set_unc(self,value):
-        """
-        Set object of type :class:`fermion_deriv`
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_set_unc
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        func(self._ptr,value._ptr)
-        return
-
-    @property
-    def method(self):
-        """
-        Property of type ``ctypes.c_int``
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_get_method
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @method.setter
-    def method(self,value):
-        """
-        Setter function for fermion_deriv_rel::method .
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_set_method
-        func.argtypes=[ctypes.c_void_p,ctypes.c_int]
-        func(self._ptr,value)
-        return
-
-    @property
-    def last_method(self):
-        """
-        Property of type ``ctypes.c_int``
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_get_last_method
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @last_method.setter
-    def last_method(self,value):
-        """
-        Setter function for fermion_deriv_rel::last_method .
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_set_last_method
-        func.argtypes=[ctypes.c_void_p,ctypes.c_int]
-        func(self._ptr,value)
-        return
-
-    @property
-    def err_nonconv(self):
-        """
-        Property of type ``ctypes.c_bool``
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_get_err_nonconv
-        func.restype=ctypes.c_bool
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @err_nonconv.setter
-    def err_nonconv(self,value):
-        """
-        Setter function for fermion_deriv_rel::err_nonconv .
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_set_err_nonconv
-        func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
-        func(self._ptr,value)
-        return
-
-    def nu_from_n(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_nu_from_n
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-    def calc_density(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_calc_density
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-    def pair_density(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_pair_density
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-    def calc_mu(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_calc_mu
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-    def pair_mu(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_rel_pair_mu
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-
-class fermion_deriv_nr:
-    """
-    Python interface for class :ref:`fermion_deriv_nr <o2scl:fermion_deriv_nr_tl>`.
-    """
-
-    _ptr=0
-    _link=0
-    _owner=True
-
-    def __init__(self,link,pointer=0):
-        """
-        Init function for class fermion_deriv_nr
-
-        | Parameters:
-        | *link* :class:`linker` object
-        | *pointer* ``ctypes.c_void_p`` pointer
-
-        """
-
-        if pointer==0:
-            f=link.o2scl.o2scl_create_fermion_deriv_nr
-            f.restype=ctypes.c_void_p
-            f.argtypes=[]
-            self._ptr=f()
-        else:
-            self._ptr=pointer
-            self._owner=False
-        self._link=link
-        return
-
-    def __del__(self):
-        """
-        Delete function for class fermion_deriv_nr
-        """
-
-        if self._owner==True:
-            f=self._link.o2scl.o2scl_free_fermion_deriv_nr
-            f.argtypes=[ctypes.c_void_p]
-            f(self._ptr)
-            self._owner=False
-            self._ptr=0
-        return
-
-    def __copy__(self):
-        """
-        Shallow copy function for class fermion_deriv_nr
-        
-        Returns: fermion_deriv_nr object
-        """
-
-        new_obj=type(self)(self._link,self._ptr)
-        return new_obj
-
-    @property
-    def flimit(self):
-        """
-        Property of type ``ctypes.c_double``
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_get_flimit
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @flimit.setter
-    def flimit(self,value):
-        """
-        Setter function for fermion_deriv_nr::flimit .
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_set_flimit
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
-        func(self._ptr,value)
-        return
-
-    def get_unc(self):
-        """
-        Get object of type :class:`fermion_deriv`
-        """
-        func1=self._link.o2scl.o2scl_fermion_deriv_nr_get_unc
-        func1.restype=ctypes.c_void_p
-        func1.argtypes=[ctypes.c_void_p]
-        ptr=func1(self._ptr)
-        obj=fermion_deriv(self._link,ptr)
-        return obj
-
-    def set_unc(self,value):
-        """
-        Set object of type :class:`fermion_deriv`
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_set_unc
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        func(self._ptr,value._ptr)
-        return
-
-    def calc_density_zerot(self,f):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_calc_density_zerot
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        func(self._ptr,f._ptr)
-        return
-
-    def calc_mu_zerot(self,f):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_calc_mu_zerot
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        func(self._ptr,f._ptr)
-        return
-
-    def nu_from_n(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_nu_from_n
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-    def calc_density(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_calc_density
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-    def calc_mu(self,f,T):
-        """
-        | Parameters:
-        | *f*: :class:`fermion_deriv` object
-        | *T*: ``double``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_fermion_deriv_nr_calc_mu
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        ret=func(self._ptr,f._ptr,T)
-        return ret
-
-
 class classical_deriv_thermo:
     """
     Python interface for class :ref:`classical_deriv_thermo <o2scl:classical_deriv_thermo_tl>`.
     """
 
     _ptr=0
     _link=0
@@ -2717,15 +2305,15 @@
         return
 
 
 class fermion_mag_zerot:
     """
     Python interface for O2scl class ``fermion_mag_zerot``,
     See
-    https://neutronstars.utk.edu/code/o2scl/html/class/fermion_mag_zerot.html .
+    https://awsteiner.org/code/o2scl/html/class/fermion_mag_zerot.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
```

### Comparing `o2sclpy-0.928/o2sclpy/plot_base.py` & `o2sclpy-0.929/o2sclpy/plot_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2023, Andrew W. Steiner
+#  Copyright (C) 2006-2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -167,25 +167,29 @@
     """
     Right panel axis for the editor
     """
     link2=0
     """
     Link to the O2scl library DLL
     """
+    usetex=True
+    """
+    If true, then use LaTeX for text objects (default True)
+    """
     
     def __init__(self):
-        """
-        Desc
+        """The plot_base init method, which only calls
+        plot_base::new_cmaps().
         """
         self.new_cmaps()
     
     def colors(self,args=[]):
         """Documentation for o2graph command ``colors``:
 
-        Show color information
+        Show color information.
 
         Command-line arguments: ``list`` or ``plot [filename]`` or 
         ``near <color> [filename]`` or ``xkcd``.
 
         The ``colors`` command outputs or plots information about
         matplotlib colors.
 
@@ -205,14 +209,23 @@
         figure is written to the specified file. To determine 
         which colors are "nearest", the sum of the absolute
         values of the differences in the RGB values are used.
 
         Finally, if the "xkcd" argument is given, then all 
         949 xkcd colors are listed along with their HTML
         hexadecimal RBG values.
+
+        Color arguments in o2graph supports the (r,g,b) format, the
+        [r,g,b,a] format, the HTML format, the grayscale single-value
+        format, and the XKCD colors. For (r,g,b) colors, parentheses
+        must be used, and the r, g, and b numbers should be from 0.0
+        to 1.0. For [r,g,b,a] colors, square brackets must be used and
+        the r, g, b, and a numbers should be from 0.0 to 1.0. The HTML
+        format is #RRGGBB where RR, GG, and BB are two-digit
+        hexadecimal values.
         """
 
         if len(args)>=1 and args[0]=='list':
             color_list()
             return
 
         if len(args)>=1 and args[0]=='plot':
@@ -237,35 +250,50 @@
 
         print('Arguments for command "colors" not understood.')
         return
     
     def cmap(self,cmap_name,col_list=[]):
         """Documentation for o2graph command ``cmap``:
 
-        Create a continuous colormap.
+        Create a continuous colormap or list colormaps.
 
         Command-line arguments: ``<cmap name> <color 1> <color 2> 
         [color3]...`` or ``<cmap name> "sharp" <color 1> <color 2>
         [color3 color4]...`` or ``list`` or ``plot [filename]``
 
-        Create a new color map named <cmap name> which consists of
-        equal-sized gradients between the specified list of at least
-        two colors. Matplotlib colors, (r,g,b) colors, [r,g,b,a] colors,
+        In the first form, this command creates a new color map named
+        <cmap name> which consists of equal-sized gradients between
+        the specified list of at least two colors. In the second form,
+        when the keyword sharp is given, the color map consists of
+        gradients between each pair of colors with a sharp transition
+        between successive pairs.
+
+        Matplotlib colors, (r,g,b) colors, [r,g,b,a] colors,
         and xkcd colors are all allowed. For example::
 
-          o2graph -cmap c forestgreen "(0.5,0.5,0.7)" "xkcd:light red" \\
-          -create table3d x grid:0,40,1 y grid:0,40,1 z "x+y" \\
-          -den-plot z cmap=c -show
+          o2graph -cmap c forestgreen "[0.5,0.5,0.7,0.5]" \\
+          "xkcd:light red" -create table3d x grid:0,40,1 y grid:0,40,1 \\
+          z "x+y" -den-plot z cmap=c -show
 
         or::
 
           o2graph -cmap c sharp "(0.5,0.5,0.7)" "xkcd:light red" \\
           green "(0,0,0)" -create table3d x grid:0,40,1 y grid:0,40,1 \\
           z "x+y" -den-plot z cmap=c -show
 
+        In the third form, the cmap command lists all of the 
+        available colormaps. Finally, in the fourth form, the 
+        cmap command plots all available colormaps, optionally storing
+        this plot in a file, e.g.::
+
+          o2graph -cmap plot cmap_plot.png
+
+        To get more information on the available colors, see::
+
+          o2graph -colors list 
         """
 
         if self.verbose>1:
             print('cmap name:',cmap_name,'list:',col_list)
 
         if cmap_name=='list':
         
@@ -439,16 +467,19 @@
         cmapr_obj=cmap_obj.reversed()
         #plot.register_cmap(cmap=cmapr_obj)
         matplotlib.colormaps.register(cmap=cmapr_obj)
         
         return
         
     def new_cmaps(self):
-        """
-        Add a few new colormaps
+        """Add a few new colormaps. This function is called by
+        plot_base::__init__().
+
+        This function adds the colormaps 'jet2' 'pastel2', 'reds2',
+        'greens2', and 'blues2'.
         """
 
         import matplotlib.pyplot as plot
         import matplotlib
         from matplotlib.colors import LinearSegmentedColormap
 
         if 'jet2' not in plot.colormaps():
@@ -546,16 +577,17 @@
             matplotlib.colormaps.register(cmap=blues2_r)
             #plot.register_cmap(cmap=blues2_r)
 
         # End of function plot_base::new_cmaps()
         return
 
     def set(self,name,value):
-        """
-        Set the value of parameter named ``name`` to value ``value``
+        """Set the value of parameter named ``name`` to value ``value``. The
+        documentation for the o2graph command ``set`` is given in
+        O₂scl.
         """
         
         import matplotlib.pyplot as plot
 
         if name=='logx':
             if value=='False' or value=='0':
                 self.logx=False
@@ -682,82 +714,82 @@
         if self.verbose>0:
             print('Set',name,'to',value)
             
         # End of function plot_base::set()
         return
 
     def get(self,name):
-        """
-        Output the value of parameter named ``name``
+        """Output the value of parameter named ``name``. The documentation
+        for the o2graph command ``get`` is given in O₂scl.
         """
         if name=='colbar':
-            print('The value of colbar is',self.colbar,'.')
+            print('The value of colbar is'+str(self.colbar)+'.')
         if name=='logx':
-            print('The value of logx is',self.logx,'.')
+            print('The value of logx is'+str(self.logx)+'.')
         if name=='logy':
-            print('The value of logy is',self.logy,'.')
+            print('The value of logy is'+str(self.logy)+'.')
         if name=='logz':
-            print('The value of logz is',self.logz,'.')
+            print('The value of logz is'+str(self.logz)+'.')
         if name=='verbose':
-            print('The value of verbose is',self.verbose,'.')
+            print('The value of verbose is'+str(self.verbose)+'.')
         if name=='xhi':
-            print('The value of xhi is',self.xhi,'.')
+            print('The value of xhi is'+str(self.xhi)+'.')
         if name=='xlo':
-            print('The value of xlo is',self.xlo,'.')
+            print('The value of xlo is'+str(self.xlo)+'.')
         if name=='xset':
-            print('The value of xset is',self.xset,'.')
+            print('The value of xset is'+str(self.xset)+'.')
         if name=='yhi':
-            print('The value of yhi is',self.yhi,'.')
+            print('The value of yhi is'+str(self.yhi)+'.')
         if name=='ylo':
-            print('The value of ylo is',self.ylo,'.')
+            print('The value of ylo is'+str(self.ylo)+'.')
         if name=='yset':
-            print('The value of yset is',self.yset,'.')
+            print('The value of yset is'+str(self.yset)+'.')
         if name=='zhi':
-            print('The value of zhi is',self.zhi,'.')
+            print('The value of zhi is'+str(self.zhi)+'.')
         if name=='zlo':
-            print('The value of zlo is',self.zlo,'.')
+            print('The value of zlo is'+str(self.zlo)+'.')
         if name=='zset':
-            print('The value of zset is',self.zset,'.')
+            print('The value of zset is'+str(self.zset)+'.')
         if name=='fig_dict':
-            print('The value of fig_dict is',self.fig_dict,'.')
+            print('The value of fig_dict is'+str(self.fig_dict)+'.')
         if name=='yt_axis':
-            print('The value of yt_axis is',self.yt_axis,'.')
+            print('The value of yt_axis is'+str(self.yt_axis)+'.')
         if name=='yt_axis_color':
-            print('The value of yt_axis_color is',self.yt_axis_color,'.')
+            print('The value of yt_axis_color is'+str(self.yt_axis_color)+'.')
         if name=='yt_axis_labels_flat':
             print('The value of yt_axis_labels_flat is',
                   self.yt_axis_labels_flat,'.')
         if name=='yt_axis_resolution':
             print('The value of yt_axis_resolution is',
                   self.yt_axis_resolution,'.')
         if name=='yt_focus':
-            print('The value of yt_focus is',self.yt_focus,'.')
+            print('The value of yt_focus is'+str(self.yt_focus)+'.')
         if name=='yt_sigma_clip':
-            print('The value of yt_sigma_clip is',self.yt_sigma_clip,'.')
+            print('The value of yt_sigma_clip is'+str(self.yt_sigma_clip)+'.')
         if name=='yt_position':
-            print('The value of yt_position is',self.yt_position,'.')
+            print('The value of yt_position is'+str(self.yt_position)+'.')
         if name=='yt_path':
-            print('The value of yt_path is',self.yt_path,'.')
+            print('The value of yt_path is'+str(self.yt_path)+'.')
         # End of function plot_base::get()
         return
 
     def xlimits(self,xlo,xhi):
-        """
-        Documentation for o2graph command ``xlimits``:
+        """Documentation for o2graph command ``xlimits``:
 
         Set the x-axis limits
 
         Command-line arguments: ``<x low> <x high>``
 
-        The xlimits command sets ``xlo`` and ``xhi`` to the specified limits
-        and sets ``xset`` to True. If a plotting canvas is currently open,
-        then the x-limits on the current axis are modified. Future
-        plots are also plot with the specified x-limits. If <low> and
-        <high> are identical then ``xset`` is set to False and the x
-        limits are automatically set by matplotlib.
+        The xlimits command sets ``xlo`` and ``xhi`` to the specified
+        limits and sets ``xset`` to True. If a plotting canvas is
+        currently open, then the x-limits on the current axis are
+        modified. Future plots are also plot with the specified
+        x-limits. If <low> and <high> are identical then ``xset`` is
+        set to False and the x limits are automatically set by
+        matplotlib.
         """
         if xlo==xhi:
             self.xset=False
             return
         self.xlo=xlo
         self.xhi=xhi
         self.xset=True
@@ -809,18 +841,16 @@
         """Documentation for o2graph command ``zlimits``:
 
         Set the z-axis limits
 
         Command-line arguments: ``<z low> <z high>``
 
         The ``zlimits`` command sets ``zlo`` and ``zhi`` to the
-        specified limits and sets ``zset`` to True. 
-        If <low> and <high> are identical then ``zset`` is set
-        to False.
-
+        specified limits and sets ``zset`` to True. If <low> and
+        <high> are identical then ``zset`` is set to False.
         """
         if zlo==zhi:
             self.zset=False
             return
         self.zlo=zlo
         self.zhi=zhi
         self.zset=True
@@ -838,16 +868,16 @@
 
         Plot a line from ``(x1,y1)`` to ``(xy,y2)``. Some useful
         kwargs are color (c), dashes, linestyle (ls), linewidth (lw),
         marker, markeredgecolor (mec), markeredgewidth (mew),
         markerfacecolor (mfc), markerfacecoloralt (mfcalt), markersize
         (ms). For example::
 
-            o2graph -line 0.05 0.05 0.95 0.95 lw=0,marker='+' \\
-            -show
+            o2graph -line 0.05 0.05 0.95 0.95 \\
+            lw=2,marker='+',ms=10,c=xkcd:'light purple' -show
 
         """
         if self.verbose>2:
             print('Line',x1,y1,x2,y1)
         if self.canvas_flag==False:
             self.canvas()
             
@@ -875,53 +905,65 @@
         ``arrow`` command uses axes.annotate() to generate an arrow
         with an empty string as the first argument to annotate(). The
         o2graph argument <arrow properties> is the python dictionary
         for the 'arrowprops' argument to annotate(). The arrowstyle
         and connectionstyle attributes should be listed along with
         other arrowprops attributes. Examples for arrowprops are::
 
-            * arrowstyle=->,connectionstyle=arc3
-            * arrowstyle=-|>,connectionstyle=arc,fc=red,ec=blue
+            * arrowstyle=->,connectionstyle=arc3 \\
+            * arrowstyle=-|>,connectionstyle=arc,fc=red,ec=blue \\
             * arrowstyle=-|>,connectionstyle=arc,head_length=4.0,
-              head_width=1.0
+              head_width=1.0 \\
             * arrowstyle=->,connectionstyle=arc3,head_length=4.0,
-              head_width=1.0,rad=-0.1 
+              head_width=1.0,rad=-0.1 \\
             * arrowstyle=fancy,connectionstyle=arc3,head_length=4.0,
-              head_width=1.0,rad=-0.1
+              head_width=1.0,rad=-0.1 \\
         
         Summary for arrowstyle argument (angleB is renamed to 
         as_angleB)::
 
-            Name    Attributes
-            -       None
-            ->      head_length=0.4,head_width=0.2
-            -[      widthB=1.0,lengthB=0.2,as_angleB=None
-            |-      widthA=1.0,widthB=1.0
-            -|      head_length=0.4,head_width=0.2
-            <-      head_length=0.4,head_width=0.2
-            <|      head_length=0.4,head_width=0.2
-            fancy   head_length=0.4,head_width=0.4,tail_width=0.4
-            simple  head_length=0.5,head_width=0.5,tail_width=0.2
-            wedge   tail_width=0.3,shrink_factor=0.5
+            Name    Attributes \\
+            -       None \\
+            ->      head_length=0.4,head_width=0.2 \\
+            -[      widthB=1.0,lengthB=0.2,as_angleB=None \\
+            |-      widthA=1.0,widthB=1.0 \\
+            -|      head_length=0.4,head_width=0.2 \\
+            <-      head_length=0.4,head_width=0.2 \\
+            <|      head_length=0.4,head_width=0.2 \\
+            fancy   head_length=0.4,head_width=0.4,tail_width=0.4 \\
+            simple  head_length=0.5,head_width=0.5,tail_width=0.2 \\
+            wedge   tail_width=0.3,shrink_factor=0.5 \\
         
         (note that fancy, simple or wedge require arc3 or angle3 connection 
         styles)
 
         Summary for connectionstyle argument (angleB is renamed to 
         cs_angleB)::
 
-            Name    Attributes
-            * angle   angleA=90,cs_angleB=0,rad=0.0
-            * angle3  angleA=90,cs_angleB=0
-            * arc     angleA=0,cs_angleB=0,armA=None,armB=None,rad=0.0
-            * arc3    rad=0.0
-            * bar     armA=0.0,armB=0.0,fraction=0.3,angle=None
+            Name    Attributes \\
+            * angle   angleA=90,cs_angleB=0,rad=0.0 \\
+            * angle3  angleA=90,cs_angleB=0 \\
+            * arc     angleA=0,cs_angleB=0,armA=None,armB=None,rad=0.0 \\
+            * arc3    rad=0.0 \\
+            * bar     armA=0.0,armB=0.0,fraction=0.3,angle=None \\
 
         See https://matplotlib.org/2.0.2/users/annotations.html for more.
+        For example::
 
+            o2graph -xlimits 0 1 -ylimits 0 1.2 \\
+            -arrow 0.2 0.2 0.8 0.2 \\
+            arrowstyle='->',connectionstyle=arc3 \\
+            -arrow 0.2 0.4 0.8 0.4 \\
+            arrowstyle='-|>',connectionstyle=arc,fc=red,ec=blue \\
+            -arrow 0.2 0.6 0.8 0.6 \\
+            arrowstyle='-|>',connectionstyle=arc,head_length=4.0,head_width=1.0 \\
+            -arrow 0.2 0.8 0.8 0.8 \\
+            arrowstyle='->',connectionstyle=arc3,head_length=4.0,head_width=1.0,rad=-0.1 \\
+            -arrow 0.2 1.0 0.8 1.0 arrowstyle=fancy,connectionstyle=arc3,head_length=4.0,head_width=1.0,rad=-0.1 \\
+            -show
         """
         if self.verbose>2:
             print('Arrow',x1,y1,x2,y1,arrowprops)
         if self.canvas_flag==False:
             self.canvas()
         if isinstance(x1,str):
             x1=float(eval(x1))
@@ -934,22 +976,41 @@
         self.axes.annotate("",xy=(x2,y2),xycoords='data',
                            xytext=(x1,y1),textcoords='data',
                            arrowprops=string_to_dict(arrowprops))
         # End of function plot_base::arrow()
         return
 
     def point(self,xval,yval,**kwargs):
-        """
-        Documentation for o2graph command ``point``:
+        """Documentation for o2graph command ``point``:
 
         Plot a single point.
 
-        Command-line arguments: ``<x> <y> [kwargs]``
+        Command-line arguments: ``<x> <y> <kwargs>``
+
+        Plot a single point. Some useful kwargs are color, marker,
+        markeredgecolor (mec), markeredgewidth (mew), and markersize
+        (ms). Note that the 'marker' keyword argument to specify the
+        marker type must be specified. For example::
+
+            o2graph -xlimits 0 1 -ylimits 0 1 -point 0.5 0.5 \\
+            marker='o',ms=10,c='xkcd:sea green',mec=blue,mew=2 -show
+
+        or::
+
+            o2graph -xlimits 0 1 -ylimits 0 1 -point 0.5 0.5 \\
+            marker='$\\int_0^{\\infty}x^2~dx$',ms=300,c=green,mec=red -show
+
+        To list the marker types, use::
+
+            o2graph -help markers
+
+        or::
+
+            o2graph -help markers-plot
 
-        Plot a single point.
         """
         if self.verbose>2:
             print('point',xval,yval,kwargs)
         if self.canvas_flag==False:
             self.canvas()
         if isinstance(xval,str):
             xval=float(eval(xval))
@@ -969,26 +1030,26 @@
         Documentation for o2graph command ``error-point``:
 
         Plot a single point with errorbars.
 
         Command-line arguments: ``<x> <y> [<x err> <yerr>] or 
         [<x lo> <x hi> <y lo> <y hi>]``
 
-        Some useful kwargs for the ``error-point`` command are:
+        Some useful kwargs for the ``error-point`` command are::
         
-        keyword    description                      default value
-        ecolor     error bar color                   None
-        capsize    cap size in points                None
-        barsabove  plot error bars on top of point   False
-        lolims     y value is lower limit            False
-        uplims     y value is upper limit            False
-        xlolims    x value is lower limit            False
-        xuplims    x value is upper limit            False
-        errorevery draw error bars on subset of data 1
-        capthick   thickness of error bar cap        None
+            keyword    description                       default value \\
+            ecolor     error bar color                   None \\
+            capsize    cap size in points                None \\
+            barsabove  plot error bars on top of point   False \\
+            lolims     y value is lower limit            False \\
+            uplims     y value is upper limit            False \\
+            xlolims    x value is lower limit            False \\
+            xuplims    x value is upper limit            False \\
+            errorevery draw error bars on subset of data 1 \\
+            capthick   thickness of error bar cap        None
 
         See also ``errorbar`` for for plotting columns from a table object
 
         """
         if err1=='None' or err1=='none':
             err1=None
         if err2=='None' or err2=='none':
@@ -1050,27 +1111,37 @@
             self.axes.set_xlim(self.xlo,self.xhi)
         if self.yset==True:
             self.axes.set_ylim(self.ylo,self.yhi)
         # End of function plot_base::point()
         return
 
     def rect(self,x1,y1,x2,y2,angle=0,**kwargs):
-        """
-        Documentation for o2graph command ``rect``:
+        """Documentation for o2graph command ``rect``:
 
         Plot a rectangle.
 
         Command-line arguments: ``<x1> <y1> <x2> <y2> [angle] [kwargs]``
 
         Plot a rectange from (x1,y1) to (xy,y2) with rotation angle
         <angle>. By default, the rectangle has no border, but the
         linewidth ('lw') and edgecolor kwargs can be used to specify
         one if desired. Some useful kwargs are alpha, color, edgecolor
-        (ec), facecolor (fc), fill, hatch, linestyle (ls), linewidth
-        (lw).
+        (ec), facecolor (fc), fill, hatch ('/', '\\', '|', '-', '+',
+        'x', 'o', 'O', '.', '*'), linestyle (ls), linewidth (lw). In
+        order to specify keyword arguments, an angle must be also
+        specified.
+
+        For example::
+
+            o2graph -xlimits 0 0.8 -ylimits 0 0.6 \\
+            -text 0.55 0.35 "blah" -rect 0.2 0.2 0.5 0.5 \\
+            -rect 0.3 0.3 0.7 0.4 0 \\
+            fc=green,alpha=0.5,ls=-.,ec='xkcd:burnt orange',lw=2,hatch='///' \\
+            -show
+
         """
         import matplotlib.patches as patches
 
         if self.verbose>2:
             print('Rect',x1,y1,x2,y1)
         if self.canvas_flag==False:
             self.canvas()
@@ -1090,15 +1161,15 @@
         lower=y1
         if y2<y1:
             lower=y2
         w=abs(x1-x2)
         h=abs(y1-y2)
         if self.canvas_flag==False:
             self.canvas()
-        r=patches.Rectangle((left,lower),w,h,angle,**kwargs)
+        r=patches.Rectangle((left,lower),w,h,angle=angle,**kwargs)
         self.axes.add_patch(r)
         # End of function plot_base::rect()
         return
 
     def ellipse(self,x,y,w,h,angle=0,**kwargs):
         """
         Documentation for o2graph command ``ellipse``:
@@ -1108,15 +1179,19 @@
         Command-line arguments: ``<x> <y> <w> <h> [angle] [kwargs]``
 
         Plot an ellipse centered at (x,y) with width w and height h,
         optionally rotated by the specified angle. By default, the
         ellipse has no border, but the linewidth ('lw') and edgecolor
         kwargs can be used to specify one if desired. Some useful
         kwargs are alpha, color, edgecolor (ec), facecolor (fc), fill,
-        hatch, linestyle (ls), linewidth (lw).
+        hatch, linestyle (ls), linewidth (lw). For example::
+
+            o2graph -ellipse 0.5 0.5 0.8 0.2 45 \\
+            fc='#ccccff',ec=black,lw=2,hatch='|||',ls=':' -show
+        
         """
         import matplotlib.patches as patches
 
         if self.verbose>2:
             print('Ellipse',x,y,w,h,angle)
         if self.canvas_flag==False:
             self.canvas()
@@ -1128,15 +1203,15 @@
             w=float(eval(w))
         if isinstance(h,str):
             h=float(eval(h))
         if isinstance(angle,str):
             angle=float(eval(angle))
         if self.canvas_flag==False:
             self.canvas()
-        r=patches.Ellipse((x,y),w,h,angle,**kwargs)
+        r=patches.Ellipse((x,y),w,h,angle=angle,**kwargs)
         self.axes.add_patch(r)
         # End of function plot_base::ellipse()
         return
 
     def show(self):
         """
         Documentation for o2graph command ``show``:
@@ -1415,17 +1490,17 @@
         plot.show()
         
         # End of function plot_base::show()
         return
 
     def save(self,filename):
         """
-        Save plot to file named ``filename``. If the verbose parameter is
-        greater than zero, then this function prints the filename to
-        the screen.
+        Save plot to file named ``filename``, using the extension to set
+        the file type. If the verbose parameter is greater than zero,
+        then this function prints the filename to the screen.
         """
         
         import matplotlib.pyplot as plot
         
         if self.verbose>0:
             print('Saving as',filename,'.')
         plot.savefig(filename)
@@ -1437,24 +1512,27 @@
 
         Plot text in the data coordinates.
 
         Command-line arguments: ``<x> <y> <text> [kwargs]``
 
         The ``text`` command plots text in the data coordinates
         defined by the current axes with the font size determined by
-        the value of the parameter 'font'. LaTeX is used for text
+        the value of the parameter ``font``. LaTeX is used for text
         rendering by default, but this setting can be changed using,
-        e.g. '-set usetex 0'. Some useful kwargs are fontfamily,
-        fontstyle, fontsize, color, backgroundcolor, rotation,
-        horizontalalignment (ha), and verticalalignment (va). Note
-        that you must disable LaTeX rendering to change fontfamily or
-        fontstyle.
+        e.g. '-set usetex 0'. Some useful kwargs are fontfamily
+        ('serif', 'sans-serif', 'cursive', 'fantasy', 'monospace'),
+        fontstyle ('normal', 'italic', 'oblique'), fontsize, color,
+        backgroundcolor, rotation, horizontalalignment (ha), and
+        verticalalignment (va). Note that you must disable LaTeX
+        rendering to change fontfamily or fontstyle.
 
         If <x> or <y> are strings, then they are passed through the
-        ``eval()`` function and converted to floating-point numbers.
+        ``eval()`` function and converted to floating-point numbers. A
+        figure and axes are created using
+        :py:func:`o2sclpy.plot_base.canvas()`, if necessary.
         """
         if self.canvas_flag==False:
             self.canvas()
             
         ha_present=False
         for key in kwargs:
             if key=='ha' or key=='horizontalalignment':
@@ -1477,14 +1555,22 @@
             kwargs=dict(kwargs,fontsize=self.font)
 
         if isinstance(tx,str):
             tx=float(eval(tx))
         if isinstance(ty,str):
             ty=float(eval(ty))
 
+        import matplotlib.pyplot as plot
+        if self.usetex==False or self.usetex==0:
+            print('false')
+            plot.rc('text',usetex=False)
+        else:
+            print('true')
+            plot.rc('text',usetex=True)
+        
         self.axes.text(tx,ty,textstr,**kwargs)
         
         # End of function plot_base::text()
         return
 
     def textbox(self,tx,ty,strt,boxprops='',**kwargs):
         """Documentation for o2graph command ``textbox``:
@@ -1502,15 +1588,14 @@
         bounding box with the specified properties. Typical bbox
         properties are boxstyle (Circle, DArrow, LArrow, RArrow,
         Round, Round4, Roundtooth, Sawtooth, Square), alpha, color,
         edgecolor (ec), facecolor (fc), fill, hatch ({'/', '\', '|',
         '-', '+', 'x', 'o', 'O', '.', '*'}), linestyle (ls), and
         linewidth (lw). The keyword arguments are for the text
         properties, and follow those of the text command.
-
         """
         if self.canvas_flag==False:
             self.canvas()
 
         ha_present=False
         for key in kwargs:
             if key=='ha':
@@ -1547,33 +1632,29 @@
     def ttext(self,tx,ty,textstr,**kwargs):
         """Documentation for o2graph command ``ttext``:
 
         Plot text in window coordinates [(0,0) to (1,1)].
 
         Command-line arguments: ``<x> <y> <text> [kwargs]``
 
-        The ttext command plots text in the window coordinates
+        The ``ttext`` command plots text in the window coordinates
         [typically (0,0) to (1,1)] with the font size determined by
-        the value of the parameter font. LaTeX is used for text
+        the value of the parameter ``font``. LaTeX is used for text
         rendering by default, but this setting can be changed using,
         e.g. '-set usetex 0'. Some useful kwargs are fontfamily,
         fontstyle, fontsize, color, backgroundcolor, rotation,
         horizontalalignment (ha), and verticalalignment (va).
         Specifying fontsize overrides the font parameter. Note that
         you must disable LaTeX rendering to change fontfamily or
         fontstyle.
 
-        Plot text in the native coordinate system using a transAxes
-        transformation. This function uses the class font size and and
-        centering in the horizontal and vertical directions by
-        default. A figure and axes are created using
-        :py:func:`o2sclpy.plot_base.canvas()`, if they have not been
-        created already. If ``tx`` and ``ty`` are strings, then they
-        are passed through the ``eval()`` function and converted to
-        floating-point numbers.
+        If <x> or <y> are strings, then they are passed through the
+        ``eval()`` function and converted to floating-point numbers. A
+        figure and axes are created using
+        :py:func:`o2sclpy.plot_base.canvas()`, if necessary.
 
         """
         if self.canvas_flag==False:
             self.canvas()
             
         ha_present=False
         for key in kwargs:
@@ -1741,28 +1822,36 @@
         else:
             self.axes=self.axes_dict[name]
         
         # End of function plot_base::selax()
         return
 
     def inset(self,left,bottom,width,height,**kwargs):
-        """
-        Documentation for o2graph command ``inset``:
+        """Documentation for o2graph command ``inset``:
         
         Add a new set of axes
         
         Command-line arguments: ``<left> <bottom> <width> <height>
         [kwargs]``
 
-        This command creates a new set of axes, adds the new axes
-        to the list of axes, and sets the new axes as the current.
-        The axes object is named 'inset0' for the first inset, then
-        'inset1', and so on.
+        This command creates a new set of axes, adds the new axes to
+        the list of axes, and sets the new axes as the current. The
+        values <left>, <bottom>, <width>, and <height> refer to a
+        normalized coordinate system where the lower-left hand corner
+        of the figure is (0,0) and the upper-right hand corner is
+        (1,1). The axes object is named 'inset0' for the first inset,
+        then 'inset1', and so on. For example::
+
+            o2graph -inset 0.5 0.2 0.4 0.4 -selax main \\
+            -line 100 100 900 900 -selax inset0 \\
+            -line 0.1 0.9 0.9 0.1 -show
         """
-
+        if self.canvas_flag==False:
+            self.canvas()
+            
         # Create a unique axes label i.e. inset0
         ifound=9
         for i in range(0,8):
             if ifound==9:
                 axname="inset"+str(i)
                 if axname not in self.axes_dict:
                     ifound=i
@@ -1782,36 +1871,40 @@
         """
         Documentation for o2graph command ``modax``:
 
         Modify current axes properties.
 
         Command-line arguments: ``[kwargs]``
 
-        alpha            float>0      alpha value for region inside axes 
-        labelsize        float>0      font size for labels 
-        x_loc            b,t,tb       placement of x-axis (bottom, top, or both)
-        x_major_loc      float>0      linear increment for x-axis major ticks 
-        x_minor_loc      float>0      linear increment for x-axis minor ticks 
-        x_minor_tick_dir in,out,inout direction of x-axis minor ticks 
-        x_minor_tick_len float>0      length of x-axis minor ticks 
-        x_minor_tick_wid float>0      width of x-axis minor ticks 
-        x_tick_dir       in,out,inout direction of x-axis major ticks 
-        x_tick_len       float>0      length of x-axis major ticks 
-        x_tick_wid       float>0      width of x-axis major ticks 
-        x_visible        T/F          set x-axis visible or invisible 
-        y_loc            l,r,lr       placement of y-axis (left, right, or both)
-        y_major_loc      float>0      linear increment for x-axis major ticks 
-        y_minor_loc      float>0      linear increment for x-axis minor ticks 
-        y_minor_tick_dir in,out,inout direction of y-axis minor ticks 
-        y_minor_tick_len float>0      length of y-axis minor ticks 
-        y_minor_tick_wid float>0      width of y-axis minor ticks 
-        y_tick_dir       in,out,inout direction of y-axis major ticks 
-        y_tick_len       float>0      length of y-axis major ticks 
-        y_tick_wid       float>0      width of y-axis major ticks 
-        y_visible        T/F          set y-axis visible or invisible
+        The axis properties which can be modified are::
+
+            Property         Values       Description \\
+            alpha            float>0      alpha value for region inside axes \\
+            labelsize        float>0      font size for labels \\
+            x_loc            b,t,tb       placement of x-axis (bottom, top, or both) \\
+            x_major_loc      float>0      linear increment for x-axis major ticks \\
+            x_minor_loc      float>0      linear increment for x-axis minor ticks \\
+            x_minor_tick_dir in,out,inout direction of x-axis minor ticks \\
+            x_minor_tick_len float>0      length of x-axis minor ticks \\
+            x_minor_tick_wid float>0      width of x-axis minor ticks \\
+            x_tick_dir       in,out,inout direction of x-axis major ticks \\
+            x_tick_len       float>0      length of x-axis major ticks \\
+            x_tick_wid       float>0      width of x-axis major ticks \\
+            x_visible        T/F          set x-axis visible or invisible \\
+            y_loc            l,r,lr       placement of y-axis (left, right, or both) \\
+            y_major_loc      float>0      linear increment for x-axis major ticks \\
+            y_minor_loc      float>0      linear increment for x-axis minor ticks \\
+            y_minor_tick_dir in,out,inout direction of y-axis minor ticks \\
+            y_minor_tick_len float>0      length of y-axis minor ticks \\
+            y_minor_tick_wid float>0      width of y-axis minor ticks \\
+            y_tick_dir       in,out,inout direction of y-axis major ticks \\
+            y_tick_len       float>0      length of y-axis major ticks \\
+            y_tick_wid       float>0      width of y-axis major ticks \\
+            y_visible        T/F          set y-axis visible or invisible \\
+
         """
 
         import matplotlib.pyplot as plot
         
         if 'x_major_loc' in kwargs:
             self.axes.get_xaxis().set_major_locator(plot.MultipleLocator
                                         (float(kwargs['x_major_loc'])))
@@ -1907,42 +2000,45 @@
         if 'y_minor_tick_wid' in kwargs:
             self.axes.tick_params('y',which='minor',
                                   width=float(kwargs['y_minor_tick_wid']))
         return
     
     def addcbar(self,left,bottom,width,height,image='last',cmap='',**kwargs):
         """Documentation for o2graph command ``addcbar``:
-
+        
         Add a color bar.
         
         Command-line arguments: ``<left> <bottom> <width> <height>
         [kwargs]``
 
         Add a new colorbar or a colorbar from the most recently
         created image at the location specified by ``left``,
-        ``bottom``, ``width`` and ``height``. If the image keyword is
-        'last', then the last density plot (e.g. from command
-        ``den-plot``) or two-dimensional histogram plot (e.g. from
-        command ``hist2d-plot``) is used. If the image keyword is
-        'new', then a colormap must be specified using the 'cmap'
-        keyword and the color map is used to create the colorbar.
-
+        ``bottom``, ``width`` and ``height``. This command has a
+        keyword ``image`` which specifies the image which the colorbar
+        should refer to. If the image keyword is 'last', then the last
+        density plot (e.g. from command ``den-plot``) or
+        two-dimensional histogram plot (e.g. from command
+        ``hist2d-plot``) is used. If the image keyword is 'new', then
+        a colormap must be specified using the 'cmap' keyword and the
+        color map is used to create the colorbar.
         """
 
         import matplotlib.pyplot as plot
         
         # Create a unique axes label i.e. cbar0
         ifound=9
         for i in range(0,8):
             if ifound==9:
                 axname="cbar"+str(i)
                 if axname not in self.axes_dict:
                     ifound=i
         axname="cbar"+str(ifound)
-        
+        if cmap[0:5]=='cmyt.':
+            import cmyt
+                
         if image=='last':
             self.axes=self.fig.add_axes([left,bottom,width,height])
             self.axes_dict[axname]=self.axes
             print('Created new axes named',axname)
             cbar=self.fig.colorbar(self.last_image,cax=self.axes,**kwargs)
             cbar.ax.tick_params(labelsize=self.font*0.8)
         elif image=='new':
@@ -1963,34 +2059,38 @@
             print('Invalid value of image in addcbar().')
             return
         
         # End of function plot_base::addcbar()
         return
 
     def canvas(self):
-        """
-        Documentation for o2graph command ``canvas``:
+        """Documentation for o2graph command ``canvas``:
 
         Create a plotting canvas.
 
         Command-line arguments: (No arguments.)
 
-        Create an empty plotting canvas. For example 'o2graph
-        -canvas -show'. Typically, 'o2graph' creates
-        the canvas automatically so explicitly using this command
-        is unnecessary.
+        Create an empty plotting canvas. For example 'o2graph -canvas
+        -show'. Typically, 'o2graph' creates the canvas automatically
+        when the first object is plotted so explicitly using this
+        command is unnecessary.
 
         This function creates a default figure using default_plot()
         and axis object using the xtitle and ytitle for the
         axis titles and xlo, xhi, ylo, and yhi for the axis limits.
         """
         if self.verbose>2:
             print('Canvas',self.fig_dict)
 
         dct=string_to_dict(self.fig_dict)
+        if 'dpi' in dct.keys():
+            import matplotlib.pyplot as plot
+            plot.rcParams['figure.dpi']=dct['dpi']
+            del dct['dpi']
+            
         if 'fontsize' not in dct.keys():
             dct['fontsize']=self.font
         if self.editor:
             (self.fig,self.axes,self.ax_left_panel,
              self.ax_right_panel)=default_plot(**dct,editor=True)
         else:
             (self.fig,self.axes)=default_plot(**dct)
@@ -2037,16 +2137,19 @@
         The argument list ``args`` can be of the form ``[table,column
         name 1, column name 2]`` or ``[table_units,column name
         1,column name 2]`` or ``[shared_ptr_table_units, column name
         1, column name 2]`` or ``[hist]`` or ``[vec_vec_double,
         column index 1]`` or ``[vec_vec_double, column index1, column
         index 2]``. Otherwise, ``args[0]`` and ``args[1]`` are
         interpreted as arrays to be directly sent to the
-        ``matplotlib.pyplot.plot()`` function.
+        matplotlib.pyplot.plot() function.
 
+        The documentation for the o2graph ``plot`` command is 
+        in the docstring for
+        :py:func:`o2sclpy.o2graph_plotter.plot_o2graph()`.
         """
 
         if len(args)<2:
             print('Failed, not enough information to plot.')
             return
 
         if (str(type(args[0]))=='<class \'o2sclpy.base.table\'>' or
@@ -2077,27 +2180,27 @@
 
         elif str(type(args[0]))=='<class \'o2sclpy.base.std_vector_vector\'>':
             
             failed=False
 
             if len(args)>2:
                 vvd=args[0]
-                n1=len(vvd[args[1]])
-                n2=len(vvd[args[2]])
+                n1=len(vvd[int(args[1])])
+                n2=len(vvd[int(args[2])])
                 if n1<n2:
-                    xv=vvd[args[1]][0:n1]
-                    yv=vvd[args[2]][0:n1]
+                    xv=vvd[int(args[1])][0:n1]
+                    yv=vvd[int(args[2])][0:n1]
                 else:
-                    xv=vvd[args[1]][0:n2]
-                    yv=vvd[args[2]][0:n2]
+                    xv=vvd[int(args[1])][0:n2]
+                    yv=vvd[int(args[2])][0:n2]
             else:
                 vvd=args[0]
-                n1=len(vvd[args[1]])
+                n1=len(vvd[int(args[1])])
                 xv=[i for i in range(0,n1)]
-                yv=vvd[args[1]]
+                yv=vvd[int(args[1])]
 
         else:
 
             failed=False
             
             xv=args[0]
             yv=args[1]
@@ -2122,32 +2225,42 @@
                 self.axes.set_xlim(self.xlo,self.xhi)
             if self.yset==True:
                 self.axes.set_ylim(self.ylo,self.yhi)
                             
         return
 
     def den_plot(self,args,**kwargs):
-        """
-        Create a density plot from a matrix, a slice of a table3d object,
+        """Create a density plot from a matrix, a slice of a table3d object,
         or a hist_2d object.
 
         The argument list ``args`` can be of the form ``[numpy
         matrix]`` or ``[table3d,slice name]`` or ``[hist_2d]``.
+
+        The documentation for the o2graph ``den-plot`` command is in
+        the docstring for
+        :py:func:`o2sclpy.o2graph_plotter.den_plot_o2graph()`.
+
+        If a cmyt colormap is used, then the ``cmyt`` Python package is
+        required.
         """
         
         if len(args)<1:
             print('Failed, not enough information to plot.')
             return
 
         val=kwargs.pop('pcm',None)
         if val==True:
             pcm=True
         else:
             pcm=False
 
+        # If necessary, import cmyt for the cmyt colormaps
+        if 'cmap' in kwargs and kwargs['cmap'][0:5]=='cmyt.':
+            import cmyt
+            
         extent_from_grid=False
             
         if str(type(args[0]))=='<class \'o2sclpy.base.table3d\'>':
 
             table3d=args[0]
             slice_name=args[1]
             nxt=table3d.get_nx()
@@ -2363,25 +2476,31 @@
             cbar.ax.tick_params('both',length=6,width=1,which='major')
             cbar.ax.tick_params(labelsize=self.font*0.8)
                 
         return
     
     def den_plot_rgb(self,table3d,slice_r,slice_g,slice_b,
                      make_png='',renorm=False,**kwargs):
-        """
-        Density plot from a ``table3d`` object using three slices
+        """Density plot from a ``table3d`` object using three slices
         to specify the red, green, and blue values.
 
         If make_png is non-empty, then a .png is created, with no
         axes, and stored in a file given the specified name.
         In the case a .png file is to be created and renorm is 
         True, then the data is renormalized to ensure the minimum
         is 0 and the maximum is 255. Otherwise, the data is 
         set to 0 if it is less than 0 and set to 255 when it is
         greater than 255. 
+
+        The documentation for the o2graph ``den-plot-rgb`` command is
+        in the docstring for
+        :py:func:`o2sclpy.o2graph_plotter.den_plot_rgb_o2graph()`.
+
+        If the make_png keyword argument is specified, then ``Pillow``
+        Python package is required.
         """
 
         nxt=table3d.get_nx()
         nyt=table3d.get_ny()
         xgrid=[table3d.get_grid_x(i) for i in range(0,nxt)]
         ygrid=[table3d.get_grid_y(i) for i in range(0,nyt)]
 
@@ -2452,15 +2571,15 @@
                         if sl_all[j,i,0]>max_val:
                             max_val=sl_all[j,i,0]
                         if sl_all[j,i,1]>max_val:
                             max_val=sl_all[j,i,1]
                         if sl_all[j,i,2]>max_val:
                             max_val=sl_all[j,i,2]
 
-                print('o2graph::make-png(): Minimum is',
+                print('o2graph::den_plot_rgb (make-png)(): Minimum is',
                       min_val,'maximum is',max_val,'.')
                         
                 for i in range(0,nxt):
                     for j in range(0,nyt):
                         pixels[i,j]=(int(256*(sl_all[j,i,0]-min_val)/
                                          (max_val-min_val)),
                                      int(256*(sl_all[j,i,1]-min_val)/
@@ -2489,14 +2608,45 @@
             try:
                 im.save(make_png,optimize=True)
             except Exception as e:
                 print('Exception in den_plot_rgb() save image',e)
                 raise
             return
         
+        if renorm:
+            min_val=sl_all[0,0,0]
+            max_val=sl_all[0,0,0]
+            
+            for i in range(0,nxt):
+                for j in range(0,nyt):
+                    if sl_all[j,i,0]<min_val:
+                        min_val=sl_all[j,i,0]
+                    if sl_all[j,i,1]<min_val:
+                        min_val=sl_all[j,i,1]
+                    if sl_all[j,i,2]<min_val:
+                        min_val=sl_all[j,i,2]
+                    if sl_all[j,i,0]>max_val:
+                        max_val=sl_all[j,i,0]
+                    if sl_all[j,i,1]>max_val:
+                        max_val=sl_all[j,i,1]
+                    if sl_all[j,i,2]>max_val:
+                        max_val=sl_all[j,i,2]
+
+            print('o2graph::den_plot_rgb(): Minimum is',
+                  min_val,'maximum is',max_val,'.')
+                        
+            for i in range(0,nxt):
+                for j in range(0,nyt):
+                    sl_all[j,i,0]=((sl_all[j,i,0]-min_val)/
+                                   (max_val-min_val))
+                    sl_all[j,i,1]=((sl_all[j,i,1]-min_val)/
+                                   (max_val-min_val))
+                    sl_all[j,i,2]=((sl_all[j,i,2]-min_val)/
+                                   (max_val-min_val))
+                    
         if self.canvas_flag==False:
             self.canvas()
 
         # The imshow() function doesn't work with a log axis, so we
         # set the scales back to linear and manually take the log
         self.axes.set_xscale('linear')
         self.axes.set_yscale('linear')
@@ -2543,17 +2693,23 @@
             cbar=self.fig.colorbar(self.last_image,ax=self.axes)
             cbar.ax.tick_params('both',length=6,width=1,which='major')
             cbar.ax.tick_params(labelsize=self.font*0.8)
 
         return
 
     def make_png(self,table3d,slice_r,slice_g,slice_b,fname,**kwargs):
-        """
-        Create png from a ``table3d`` object using three slices
+        """Create png from a ``table3d`` object using three slices
         to specify the red, green, and blue values.
+
+        The documentation for the o2graph ``make-png`` command is in
+        the docstring for
+        :py:func:`o2sclpy.o2graph_plotter.make_png_o2graph()`.
+
+        This command requires the ``Pillow`` Python package.
+
         """
         
         nxt=table3d.get_nx()
         nyt=table3d.get_ny()
         xgrid=[table3d.get_grid_x(i) for i in range(0,nxt)]
         ygrid=[table3d.get_grid_y(i) for i in range(0,nyt)]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `o2sclpy-0.928/o2sclpy/plot_info.py` & `o2sclpy-0.929/o2sclpy/plot_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2023, Andrew W. Steiner
+#  Copyright (C) 2006-2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -21,15 +21,15 @@
 #
 
 import sys
 import numpy
 import textwrap
 
 from o2sclpy.utils import default_plot, string_to_dict, terminal_py
-from o2sclpy.doc_data import cmaps, new_cmaps
+from o2sclpy.doc_data import cmaps, new_cmaps, yt_cmaps
 
 def marker_list():
     """ 
     Print a list of matplotlib markers which work in o2graph
     command-line arguments.
     """
     print('Matplotlib markers supported by O2graph:')
@@ -109,15 +109,15 @@
            [5,"5",'right caret'],
            [6,"6",'up caret'],
            [7,"7",'down caret'],
            [8,"8",'left shifted caret'],
            [9,"9",'right shifted caret'],
            [10,"10",'up shifted caret'],
            [11,"11",'down shifted caret'],
-           ['$x^2$',"\$x^2\$",'math example']]
+           ['$x^2$',"\\$x^2\\$",'math example']]
     nmark=len(mlist)
     ncols=2
     nrows=(nmark+(nmark%2))/ncols
     fig_dict=('left_margin=0.01,top_margin=0.01,'+
               'right_margin=0.01,'+
               'bottom_margin=0.01,'+
               'fontsize=10,ticks_in=False,'+
@@ -138,15 +138,15 @@
             axes.text((col_ctr+0.25)/(ncols),
                       float(nrows-row_ctr)/(nrows+1),
                       entry[1],family='monospace',
                       va='center',ha='center',fontsize=16)
             plot.rc('text',usetex=True)
             axes.text((col_ctr+0.37)/(ncols),
                       float(nrows-row_ctr)/(nrows+1),
-                      entry[2].replace('_','\_'),
+                      entry[2].replace('_','\\_'),
                       va='center',ha='left',fontsize=16)
         row_ctr=row_ctr+1
         if row_ctr>=nrows:
             row_ctr=0
             col_ctr=col_ctr+1
         axes.text(0.5,0.835,r'$ \mathrm{O}_2\mathrm{sc'+
                   'lpy~markers~summary} $',
@@ -268,15 +268,19 @@
 
         # AWS, 10/16/22: This replacement was necessary with
         # usetex=True, but now usetex=False, so we remove it
         #col_fixpound=str(col).replace('#','\\#')
         
         #title=(r'$ \mathrm{O}_2\mathrm{sc'+
         #'lpy~list~of~colors~near~'+col+'}: $')
-        title=r'$ O_{2}sclpy~list~of~colors~near~'+str(col)+': $'
+
+        # AWS, 10/16/23: took latex out of the title
+        # because it was causing errors in matplotlib
+        
+        title=r'O2sclpy list of colors near '+str(col)+':'
                
         #print('title',title)
 
         if len(selected)>80:
             selected=selected[0:80]
     
         if len(selected)>0:
@@ -354,26 +358,56 @@
 def cmap_list_func():
     """ 
     List the matplotlib and o2sclpy colormaps.
     """
     print('Matplotlib colormaps:')
     ter=terminal_py()
     print(ter.horiz_line())
+    
+    inc_yt=False
+    try:
+        import cmyt
+    except:
+        pass
+    else:
+        inc_yt=True
+        
     for category, cmap_list in cmaps:
         list2=''
+        i=0
         for name in cmap_list:
-            list2+=name+' '
+            if i>0:
+                list2+=', '
+            list2+=name
+            i=i+1
         str_list=textwrap.wrap(category+': '+list2,79)
         for i in range (0,len(str_list)):
             print(str_list[i])
         print(' ')
+    if inc_yt==True:
+        for category, cmap_list in yt_cmaps:
+            list2=''
+            i=0
+            for name in cmap_list:
+                if i>0:
+                    list2+=', '
+                list2+=name
+                i=i+1
+            str_list=textwrap.wrap(category+': '+list2,79)
+            for i in range (0,len(str_list)):
+                print(str_list[i])
+            print(' ')
     for category, cmap_list in new_cmaps:
         list2=''
+        i=0
         for name in cmap_list:
-            list2+=name+' '
+            if i>0:
+                list2+=', '
+            list2+=name
+            i=i+1
         str_list=textwrap.wrap(category+': '+list2,79)
         for i in range (0,len(str_list)):
             print(str_list[i])
         print(' ')
     print('Remember that colormaps can all be',
           'reversed by using a "_r" suffix.')
     print(' ')
@@ -388,28 +422,40 @@
     """
     print('Generating colormap summary figure.')
                         
     import matplotlib.pyplot as plot
     import matplotlib.patches as patches
     
     # An internal implementation of
-    # https://matplotlib.org/3.1.0/gallery/
+    # https://matplotlib.org/stable/gallery/
     # color/colormap_reference.html
                         
     #self.left_margin=0.01
     #self.right_margin=0.01
     #self.top_margin=0.01
     #self.bottom_margin=0.01
     gradient=numpy.linspace(0,1,256)
     gradient=numpy.vstack((gradient,gradient))
-                        
+
+    inc_yt=False
+    try:
+        import cmyt
+    except:
+        pass
+    else:
+        inc_yt=True
+    
     nrows=0
     for category, cmap_list in cmaps:
         for name in cmap_list:
             nrows=nrows+1
+    if inc_yt==True:
+        for category, cmap_list in yt_cmaps:
+            for name in cmap_list:
+                nrows=nrows+1
     for category, cmap_list in new_cmaps:
         for name in cmap_list:
             nrows=nrows+1
     ncols=3
     while nrows%ncols!=0:
         nrows=nrows+1
     nrows=int((nrows)/ncols)
@@ -434,34 +480,51 @@
                         
     row_ctr=0
     col_ctr=0
     for category, cmap_list in cmaps:
         for name in cmap_list:
             ax=axes[row_ctr][col_ctr]
             ax.imshow(gradient,aspect='auto',
-                             cmap=plot.get_cmap(name))
-            r=patches.Rectangle((0.32,0.1),0.36,0.8,0,
+                      cmap=plot.get_cmap(name))
+            r=patches.Rectangle((0.32,0.1),0.36,0.8,angle=0,
                                 fc=(1,1,1,0.7),lw=0,
                                 fill=True,
                                 transform=ax.transAxes)
             ax.add_patch(r)
             ax.text(0.5,0.45,name,
                                 va='center',ha='center',
                                 fontsize=10,color=(0,0,0),
                                 transform=ax.transAxes)
             row_ctr=row_ctr+1
             if row_ctr>=nrows:
                 row_ctr=0
                 col_ctr=col_ctr+1
+    if inc_yt==True:
+        for category, cmap_list in yt_cmaps:
+            for name in cmap_list:
+                ax=axes[row_ctr][col_ctr]
+                ax.imshow(gradient,aspect='auto',
+                          cmap=plot.get_cmap(name))
+                r=patches.Rectangle((0.32,0.1),0.36,0.8,
+                                    angle=0,fc=(1,1,1,0.7),lw=0,
+                                    fill=True,transform=ax.transAxes)
+                ax.add_patch(r)
+                ax.text(0.5,0.45,name,va='center',ha='center',
+                        fontsize=8,color=(0,0,0),transform=ax.transAxes)
+                row_ctr=row_ctr+1
+                if row_ctr>=nrows:
+                    row_ctr=0
+                    col_ctr=col_ctr+1
     for category, cmap_list in new_cmaps:
         for name in cmap_list:
             ax=axes[row_ctr][col_ctr]
             ax.imshow(gradient,aspect='auto',
                       cmap=plot.get_cmap(name))
-            r=patches.Rectangle((0.32,0.1),0.36,0.8,0,fc=(1,1,1,0.7),lw=0,
+            r=patches.Rectangle((0.32,0.1),0.36,0.8,
+                                angle=0,fc=(1,1,1,0.7),lw=0,
                                 fill=True,transform=ax.transAxes)
             ax.add_patch(r)
             ax.text(0.5,0.45,name,va='center',ha='center',
                     fontsize=8,color=(0,0,0),transform=ax.transAxes)
             row_ctr=row_ctr+1
             if row_ctr>=nrows:
                 row_ctr=0
@@ -532,15 +595,16 @@
 
     axes.set_xlim(0,X)
     axes.set_ylim(0,Y+header)
     axes.set_axis_off()
                             
     fig.subplots_adjust(left=0,right=1,top=1,bottom=0,
                         hspace=0,wspace=0)
-    axes.text(X*0.5,(Y+header)*0.965,r'$ \mathrm{O}_{2}\mathrm{sclpy~colors~summary} $',
+    axes.text(X*0.5,(Y+header)*0.965,
+              r'$ \mathrm{O}_{2}\mathrm{sclpy~colors~summary} $',
               fontsize=16,ha='center')
 
     if fname!='':
         plot.savefig(fname)
         print('Created image file '+fname+'.')
     import matplotlib
     if (matplotlib.get_backend()!='Agg' and
```

### Comparing `o2sclpy-0.928/o2sclpy/yt_plot_base.py` & `o2sclpy-0.929/o2sclpy/yt_plot_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2023, Andrew W. Steiner
+#  Copyright (C) 2006-2024, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -19,17 +19,14 @@
 #  
 #  -------------------------------------------------------------------
 #
 import math
 import numpy
 import os
 
-# For system type detection
-import platform
-
 from o2sclpy.utils import parse_arguments, string_to_dict
 from o2sclpy.utils import force_bytes, default_plot, get_str_array
 from o2sclpy.utils import string_to_color
 from o2sclpy.plot_base import plot_base
 
 class yt_plot_base(plot_base):
     """
@@ -159,48 +156,85 @@
                                       keyname=self.yt_text_objects[i][0])
         
         # End of function plot_base::yt_update_text()
         return
 
     def yt_line(self,point1,point2,color=[1.0,1.0,1.0,0.5],
                 coords='user',keyname='o2sclpy_line'):
-        """
+        """Documentation for o2graph command ``yt-line``:
+
         Plot a line in a yt volume visualization.
-        """
 
+        Command-line arguments: ``x1 y1 z1 x2 y2 z2 [kwargs]``
+
+        Plot a line between point (x1,y1,z1) and (x2,y2,z2) in a yt
+        visualization. Possible kwargs are color=[1.0,1.0,1.0,0.5]
+        coords='user' and keyname='o2sclpy_line'. The possible values
+        for coords are 'user', which refers the user-specified
+        coordinate system, and 'internal', which is always between
+        (0,0,0) and (1,1,1). See ``o2graph -help colors``
+        for information on the color kwarg.
+
+        If the x, y, and z limits have not yet been set, then this
+        command uses the line coordinates to set them. If the x
+        coordinates of the endpoints are equal to x0 and the x limits
+        have not yet been set, then the x limits are x0-1 and x0+1.
+        Similarly for the y and z coordinates. If a yt scene has noet
+        yet been created, then an empty volume and scene will be
+        created.
+
+        o2graph -set xlo 0 -set xhi 2 -set ylo 0 -set yhi 2 \
+        -set zhi 0 -set zhi 2 \
+        -yt-line 0.2 1.0 0.0 1.0 1.0 2.0 color=#FF0000 \
+        -yt-line 1.0 1.0 2.0 1.8 1.0 0.0 "color=(0,0,1)" \
+        -yt-line 0.6 1.0 1.0 1.4 1.0 1.0 "color=xkcd:rose" \
+        -set yt_sigma_clip 1 \
+        -yt-path yaw 100 1.0 \
+        -yt-render "/tmp/ytl_*.png" mov_fname=yt_line.mp4
+        """
+        
         from yt.visualization.volume_rendering.api \
             import LineSource
 
         x1=point1[0]
         x2=point2[0]
         y1=point1[1]
         y2=point2[1]
         z1=point1[2]
         z2=point2[2]
         
         if self.xset==False:
-            if x1<x2:
+            if x1==x2:
+                self.xlo=x1-1
+                self.xhi=x2+1
+            elif x1<x2:
                 self.xlo=x1
                 self.xhi=x2
             else:
                 self.xlo=x2
                 self.xhi=x1
             print('Set xlimits to',self.xlo,self.xhi)
             self.xset=True
         if self.yset==False:
-            if y1<y2:
+            if y1==y2:
+                self.ylo=y1-1
+                self.yhi=y2+1
+            elif y1<y2:
                 self.ylo=y1
                 self.yhi=y2
             else:
                 self.ylo=y2
                 self.yhi=y1
             print('Set ylimits to',self.ylo,self.yhi)
             self.yset=True
         if self.zset==False:
-            if z1<z2:
+            if z1==z2:
+                self.zlo=z1-1
+                self.zhi=z2+1
+            elif z1<z2:
                 self.zlo=z1
                 self.zhi=z2
             else:
                 self.zlo=z2
                 self.zhi=z1
             print('Set zlimits to',self.zlo,self.zhi)
             self.zset=True
@@ -223,29 +257,82 @@
 
         # Convert color to [r,g,b,a] for yt
         from matplotlib.colors import to_rgba
         colt=to_rgba(color)
         colt2=[colt[0],colt[1],colt[2],colt[3]]
         colors=[colt2]
         
-        vertices=numpy.array([[[(x1-self.xlo)/(self.xhi-self.xlo),
-                                (y1-self.ylo)/(self.yhi-self.ylo),
-                                (z1-self.zlo)/(self.zhi-self.zlo)],
-                               [(x2-self.xlo)/(self.xhi-self.xlo),
-                                (y2-self.ylo)/(self.yhi-self.ylo),
-                                (z2-self.zlo)/(self.zhi-self.zlo)]]])
+        vertices=numpy.array([[[x1,y1,z1],[x2,y2,z2]]])
         colors=numpy.array([colt2])
         ls=LineSource(vertices,colors)
         print('o2graph:yt-line: Adding line source.')
         kname=self.yt_unique_keyname(keyname)
         self.yt_scene.add_source(ls,keyname=kname)
 
         # End of function plot_base::yt_line()
         return
         
+    def yt_point(self,point1,rad,color=[1.0,1.0,1.0,0.5],
+                coords='user',keyname='o2sclpy_point'):
+        """
+        Plot a point in a yt volume visualization.
+        """
+
+        from yt.visualization.volume_rendering.api \
+            import PointSource
+
+        x1=point1[0]
+        y1=point1[1]
+        z1=point1[2]
+        
+        if self.xset==False:
+            self.xlo=x1-1
+            self.xhi=x1+1
+            print('Set xlimits to',self.xlo,self.xhi)
+            self.xset=True
+        if self.yset==False:
+            self.ylo=y1-1
+            self.yhi=y1+1
+            print('Set ylimits to',self.ylo,self.yhi)
+            self.yset=True
+        if self.zset==False:
+            self.zlo=z1-1
+            self.zhi=z1+1
+            print('Set zlimits to',self.zlo,self.zhi)
+            self.zset=True
+        
+        icnt=0
+        if self.yt_scene!=0:
+            for key, value in self.yt_scene.sources.items():
+                icnt=icnt+1
+        if icnt==0:
+            self.yt_def_vol()
+
+        # Coordinate transformation
+        if coords!='internal':
+            x1=(x1-self.xlo)/(self.xhi-self.xlo)
+            y1=(y1-self.ylo)/(self.yhi-self.ylo)
+            z1=(z1-self.zlo)/(self.zhi-self.zlo)
+
+        # Convert color to [r,g,b,a] for yt
+        from matplotlib.colors import to_rgba
+        colt=to_rgba(color)
+        colors=numpy.array([[colt[0],colt[1],colt[2],colt[3]]])
+        
+        point_array=numpy.array([[(x1-self.xlo)/(self.xhi-self.xlo),
+                                  (y1-self.ylo)/(self.yhi-self.ylo),
+                                  (z1-self.zlo)/(self.zhi-self.zlo)]])
+        ps=PointSource(point_array,colors,radii=int(rad))
+        print('o2graph:yt-point: Adding point source.')
+        kname=self.yt_unique_keyname(keyname)
+        self.yt_scene.add_source(ps,keyname=kname)
+
+        # End of function plot_base::yt_point()
+        return
+        
     def yt_arrow(self,point1,point2,color=[1.0,1.0,1.0,0.5],n_lines=40,
                  frac_length=0.05,radius=0.0125,coords='user',
                  keyname='o2sclpy_arrow'):
         """
         Plot an arrow in a yt volume visualization. 
         """
         
@@ -675,15 +762,16 @@
         self.yt_camera.north_vector=[0.0,0.0,1.0]
         self.yt_camera.switch_orientation()
         self.yt_created_camera=True
         # End of function plot_base::yt_create_camera()
         return
     
     def yt_text_to_points(self,veco,vecx,vecy,text,dpi=100,font=30,
-                          textcolor=(1,1,1,0.5),show=False,filename=''):
+                          textcolor=(1,1,1,0.5),show=False,filename='',
+                          facecolor=(0,0,0)):
         """
         Take three 3D vectors 'veco' (origin), 'vecx' (x direction) and
         'vecy' (y direction), and a string of text ('text'), and
         return a numpy array of shape (6,npoints) which has entries
         (x,y,z,r,g,b). The values r, g, and b are between 0 and 1.
 
         The alpha value of 'textcolor' is also used for the alpha value
@@ -707,16 +795,16 @@
         """
         
         import matplotlib.pyplot as plot
         
         plot.rc('text',usetex=True)
         fig=plot.figure(1,figsize=(6.4,4.8),dpi=dpi)
         axes=plot.axes([0,0,1,1])
-        fig.set_facecolor((0,0,0))
-        axes.set_facecolor((0,0,0))
+        fig.set_facecolor(facecolor)
+        axes.set_facecolor(facecolor)
 
         from matplotlib.colors import to_rgba
         alpha=to_rgba(textcolor)[3]
         
         axes.text(0.5,0.5,text,fontsize=font,ha='center',va='center',
                   color=textcolor)
         
@@ -725,21 +813,26 @@
             print("Saving render of text '"+text+
                   "' in file named "+filename+'.')
             plot.savefig(filename)
         if show:
             plot.show()
             
         X=numpy.array(fig.canvas.renderer._renderer)
+        #print("shapex:",numpy.shape(X))
         Y=[]
         Y2=[]
 
         # Note that the array is flipped, so ymax is obtained
         # from the width and xmax is obtained from the height
-        ymax=int(fig.get_dpi()*fig.get_figwidth())
-        xmax=int(fig.get_dpi()*fig.get_figheight())
+        #ymax=int(fig.get_dpi()*fig.get_figwidth())
+        #xmax=int(fig.get_dpi()*fig.get_figheight())
+        
+        xmax=numpy.shape(X)[0]
+        ymax=numpy.shape(X)[1]
+        #print('xmax,ymax',xmax,ymax)
         
         for i in range(0,xmax):
             for j in range(0,ymax):
                 if X[i,j,0]!=0 or X[i,j,1]!=0 or X[i,j,2]!=0:
                     xold=2.0*(i-float(xmax)/2)/float(xmax)
                     yold=2.0*(j-float(ymax)/2)/float(ymax)
                     vecnew=[veco[0]-vecy[0]*xold+vecx[0]*yold,
@@ -902,14 +995,16 @@
         """
         Create a default yt volume source for rendering other objects
         """
         import yt
         from yt.visualization.volume_rendering.api \
             import create_volume_source
 
+        yt.set_log_level("warning")
+        
         if self.verbose>0:
             print('No volume object, adding yt volume.')
             
         self.yt_tf=yt.ColorTransferFunction((0,1),grey_opacity=False)
         self.yt_tf.add_gaussian(2.0,0.1,[0,0,0,0])
             
         arr=numpy.zeros(shape=(2,2,2))
```

### Comparing `o2sclpy-0.928/o2sclpy.egg-info/SOURCES.txt` & `o2sclpy-0.929/o2sclpy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 bin/o2graph
 o2sclpy/__init__.py
 o2sclpy/base.py
+o2sclpy/bl_gltf_import.py
+o2sclpy/bl_gltf_six.py
+o2sclpy/bl_gltf_yaw.py
 o2sclpy/cap_cout.py
 o2sclpy/doc_data.py
 o2sclpy/eos.py
 o2sclpy/gmm.py
 o2sclpy/hdf.py
-o2sclpy/hdf_add.py
 o2sclpy/interpm.py
 o2sclpy/kde.py
 o2sclpy/link_o2scl.py
 o2sclpy/nuclei.py
+o2sclpy/o2graph.py
 o2sclpy/o2graph_plotter.py
 o2sclpy/other.py
 o2sclpy/part.py
 o2sclpy/plot_base.py
 o2sclpy/plot_info.py
+o2sclpy/td_plot_base.py
 o2sclpy/utils.py
 o2sclpy/yt_plot_base.py
 o2sclpy.egg-info/PKG-INFO
 o2sclpy.egg-info/SOURCES.txt
 o2sclpy.egg-info/dependency_links.txt
-o2sclpy.egg-info/not-zip-safe
+o2sclpy.egg-info/entry_points.txt
 o2sclpy.egg-info/requires.txt
-o2sclpy.egg-info/top_level.txt
+o2sclpy.egg-info/top_level.txt
+o2sclpy/test/test_cpp_class.py
+o2sclpy/test/test_den_plot.py
+o2sclpy/test/test_gmm.py
+o2sclpy/test/test_interpm.py
+o2sclpy/test/test_kde.py
+o2sclpy/test/test_lib_settings.py
+o2sclpy/test/test_table.py
+o2sclpy/test/test_table3d.py
+o2sclpy/test/test_table_units.py
+o2sclpy/test/test_tensor.py
+o2sclpy/test/test_tensor_grid.py
+o2sclpy/test/test_ug.py
```

