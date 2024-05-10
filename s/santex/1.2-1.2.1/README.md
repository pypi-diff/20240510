# Comparing `tmp/santex-1.2.tar.gz` & `tmp/santex-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "santex-1.2.tar", last modified: Tue Apr 30 00:15:51 2024, max compression
+gzip compressed data, was "santex-1.2.1.tar", last modified: Fri May 10 06:22:36 2024, max compression
```

## Comparing `santex-1.2.tar` & `santex-1.2.1.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.312546 santex-1.2/
--rw-r--r--   0 usin8611   (502) staff       (20)    35149 2024-04-29 22:40:04.000000 santex-1.2/LICENSE
--rw-r--r--   0 usin8611   (502) staff       (20)     2895 2024-04-30 00:15:51.311996 santex-1.2/PKG-INFO
--rw-r--r--   0 usin8611   (502) staff       (20)     1625 2024-04-26 05:21:45.000000 santex-1.2/README.md
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.291152 santex-1.2/santex/
--rw-r--r--   0 usin8611   (502) staff       (20)      203 2024-04-18 07:52:49.000000 santex-1.2/santex/__init__.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.298674 santex-1.2/santex/anisotropy/
--rw-r--r--   0 usin8611   (502) staff       (20)       80 2024-03-20 02:12:45.000000 santex-1.2/santex/anisotropy/__init__.py
--rw-r--r--   0 usin8611   (502) staff       (20)    21309 2024-04-29 23:32:30.000000 santex-1.2/santex/anisotropy/anisotropy.py
--rw-r--r--   0 usin8611   (502) staff       (20)     1949 2024-04-26 02:39:07.000000 santex-1.2/santex/anisotropy/map.py
--rw-r--r--   0 usin8611   (502) staff       (20)     8343 2024-04-26 03:25:54.000000 santex-1.2/santex/anisotropy/melt.py
--rw-r--r--   0 usin8611   (502) staff       (20)      790 2024-04-26 01:57:52.000000 santex-1.2/santex/anisotropy/modalAnisotropy.py
--rw-r--r--   0 usin8611   (502) staff       (20)     3002 2024-04-26 03:55:11.000000 santex-1.2/santex/anisotropy/plot_seismic_velocity.py
--rw-r--r--   0 usin8611   (502) staff       (20)     3701 2024-04-26 02:06:53.000000 santex-1.2/santex/anisotropy/plot_vel_grid.py
--rw-r--r--   0 usin8611   (502) staff       (20)      696 2024-04-26 03:15:41.000000 santex-1.2/santex/anisotropy/utils.py
--rw-r--r--   0 usin8611   (502) staff       (20)    10990 2024-04-26 03:17:55.000000 santex-1.2/santex/anisotropy/vtkplotter.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.303837 santex-1.2/santex/ebsd/
--rw-r--r--   0 usin8611   (502) staff       (20)       51 2024-04-26 03:57:28.000000 santex-1.2/santex/ebsd/__init__.py
--rwxr-xr-x   0 usin8611   (502) staff       (20)     2236 2024-04-26 03:22:43.000000 santex-1.2/santex/ebsd/_ctf_parser.py
--rw-r--r--   0 usin8611   (502) staff       (20)     3180 2024-04-24 21:53:17.000000 santex-1.2/santex/ebsd/calcGrainBoundary.py
--rw-r--r--   0 usin8611   (502) staff       (20)    30478 2024-04-29 23:50:25.000000 santex-1.2/santex/ebsd/ebsd.py
--rw-r--r--   0 usin8611   (502) staff       (20)     1077 2024-04-26 03:55:11.000000 santex-1.2/santex/ebsd/melt_tensor.py
--rw-r--r--   0 usin8611   (502) staff       (20)    40972 2024-04-26 02:15:21.000000 santex-1.2/santex/ebsd/odf.py
--rw-r--r--   0 usin8611   (502) staff       (20)     5000 2024-04-26 03:55:11.000000 santex-1.2/santex/ebsd/rotateEBSD.py
--rw-r--r--   0 usin8611   (502) staff       (20)      551 2024-03-20 02:12:45.000000 santex-1.2/santex/ebsd/saveEBSD.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.305106 santex-1.2/santex/isotropy/
--rw-r--r--   0 usin8611   (502) staff       (20)       30 2024-03-20 02:12:45.000000 santex-1.2/santex/isotropy/__init__.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.305534 santex-1.2/santex/isotropy/data/
--rw-r--r--   0 usin8611   (502) staff       (20)    36992 2024-03-25 22:00:33.000000 santex-1.2/santex/isotropy/data/materials.json
--rw-r--r--   0 usin8611   (502) staff       (20)    14900 2024-04-26 03:55:11.000000 santex-1.2/santex/isotropy/isotropy.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.307101 santex-1.2/santex/material/
--rw-r--r--   0 usin8611   (502) staff       (20)       30 2024-03-20 02:12:45.000000 santex-1.2/santex/material/__init__.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.310083 santex-1.2/santex/material/data/
--rw-r--r--   0 usin8611   (502) staff       (20)    36654 2024-04-29 16:14:37.000000 santex-1.2/santex/material/data/derivatives_P.json
--rw-r--r--   0 usin8611   (502) staff       (20)    36845 2024-04-29 16:07:01.000000 santex-1.2/santex/material/data/derivatives_T.json
--rw-r--r--   0 usin8611   (502) staff       (20)    23072 2024-04-02 06:20:18.000000 santex-1.2/santex/material/data/materials_database.json
--rw-r--r--   0 usin8611   (502) staff       (20)    16915 2024-04-29 00:44:37.000000 santex-1.2/santex/material/material.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.311432 santex-1.2/santex/tensor/
--rw-r--r--   0 usin8611   (502) staff       (20)       26 2024-03-20 02:12:45.000000 santex-1.2/santex/tensor/__init__.py
--rw-r--r--   0 usin8611   (502) staff       (20)     3445 2024-04-26 03:55:11.000000 santex-1.2/santex/tensor/tensor.py
-drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-04-30 00:15:51.293147 santex-1.2/santex.egg-info/
--rw-r--r--   0 usin8611   (502) staff       (20)     2895 2024-04-30 00:15:51.000000 santex-1.2/santex.egg-info/PKG-INFO
--rw-r--r--   0 usin8611   (502) staff       (20)     1004 2024-04-30 00:15:51.000000 santex-1.2/santex.egg-info/SOURCES.txt
--rw-r--r--   0 usin8611   (502) staff       (20)        1 2024-04-30 00:15:51.000000 santex-1.2/santex.egg-info/dependency_links.txt
--rw-r--r--   0 usin8611   (502) staff       (20)       91 2024-04-30 00:15:51.000000 santex-1.2/santex.egg-info/requires.txt
--rw-r--r--   0 usin8611   (502) staff       (20)        7 2024-04-30 00:15:51.000000 santex-1.2/santex.egg-info/top_level.txt
--rw-r--r--   0 usin8611   (502) staff       (20)       38 2024-04-30 00:15:51.312621 santex-1.2/setup.cfg
--rw-r--r--   0 usin8611   (502) staff       (20)     1710 2024-04-30 00:15:41.000000 santex-1.2/setup.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.687968 santex-1.2.1/
+-rw-r--r--   0 usin8611   (502) staff       (20)    35149 2024-04-29 22:40:04.000000 santex-1.2.1/LICENSE
+-rw-r--r--   0 usin8611   (502) staff       (20)     2897 2024-05-10 06:22:36.687565 santex-1.2.1/PKG-INFO
+-rw-r--r--   0 usin8611   (502) staff       (20)     1625 2024-04-26 05:21:45.000000 santex-1.2.1/README.md
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.669339 santex-1.2.1/santex/
+-rw-r--r--   0 usin8611   (502) staff       (20)      811 2024-05-10 06:07:37.000000 santex-1.2.1/santex/__init__.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.675200 santex-1.2.1/santex/anisotropy/
+-rw-r--r--   0 usin8611   (502) staff       (20)        0 2024-05-10 05:36:31.000000 santex-1.2.1/santex/anisotropy/__init__.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    21272 2024-05-10 06:11:35.000000 santex-1.2.1/santex/anisotropy/anisotropy.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     1949 2024-04-26 02:39:07.000000 santex-1.2.1/santex/anisotropy/map.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     8343 2024-04-26 03:25:54.000000 santex-1.2.1/santex/anisotropy/melt.py
+-rw-r--r--   0 usin8611   (502) staff       (20)      790 2024-04-26 01:57:52.000000 santex-1.2.1/santex/anisotropy/modalAnisotropy.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3002 2024-04-26 03:55:11.000000 santex-1.2.1/santex/anisotropy/plot_seismic_velocity.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3701 2024-04-26 02:06:53.000000 santex-1.2.1/santex/anisotropy/plot_vel_grid.py
+-rw-r--r--   0 usin8611   (502) staff       (20)      696 2024-05-10 06:15:53.000000 santex-1.2.1/santex/anisotropy/utils.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    10981 2024-05-10 06:15:05.000000 santex-1.2.1/santex/anisotropy/vtkplotter.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.679917 santex-1.2.1/santex/ebsd/
+-rw-r--r--   0 usin8611   (502) staff       (20)        0 2024-05-10 05:36:37.000000 santex-1.2.1/santex/ebsd/__init__.py
+-rwxr-xr-x   0 usin8611   (502) staff       (20)     2236 2024-04-26 03:22:43.000000 santex-1.2.1/santex/ebsd/_ctf_parser.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3180 2024-04-24 21:53:17.000000 santex-1.2.1/santex/ebsd/calcGrainBoundary.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    30455 2024-05-10 06:14:11.000000 santex-1.2.1/santex/ebsd/ebsd.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     1077 2024-04-26 03:55:11.000000 santex-1.2.1/santex/ebsd/melt_tensor.py
+-rw-r--r--   0 usin8611   (502) staff       (20)    40972 2024-04-26 02:15:21.000000 santex-1.2.1/santex/ebsd/odf.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     5000 2024-04-26 03:55:11.000000 santex-1.2.1/santex/ebsd/rotateEBSD.py
+-rw-r--r--   0 usin8611   (502) staff       (20)      551 2024-03-20 02:12:45.000000 santex-1.2.1/santex/ebsd/saveEBSD.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.680809 santex-1.2.1/santex/isotropy/
+-rw-r--r--   0 usin8611   (502) staff       (20)        0 2024-05-10 05:54:34.000000 santex-1.2.1/santex/isotropy/__init__.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.681379 santex-1.2.1/santex/isotropy/data/
+-rw-r--r--   0 usin8611   (502) staff       (20)    36992 2024-03-25 22:00:33.000000 santex-1.2.1/santex/isotropy/data/materials.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    14900 2024-05-10 06:09:47.000000 santex-1.2.1/santex/isotropy/isotropy.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.682497 santex-1.2.1/santex/material/
+-rw-r--r--   0 usin8611   (502) staff       (20)        0 2024-05-10 05:36:47.000000 santex-1.2.1/santex/material/__init__.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.684991 santex-1.2.1/santex/material/data/
+-rw-r--r--   0 usin8611   (502) staff       (20)    36654 2024-04-29 16:14:37.000000 santex-1.2.1/santex/material/data/derivatives_P.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    36845 2024-04-29 16:07:01.000000 santex-1.2.1/santex/material/data/derivatives_T.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    23072 2024-04-02 06:20:18.000000 santex-1.2.1/santex/material/data/materials_database.json
+-rw-r--r--   0 usin8611   (502) staff       (20)    16924 2024-05-10 06:16:11.000000 santex-1.2.1/santex/material/material.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.686210 santex-1.2.1/santex/tensor/
+-rw-r--r--   0 usin8611   (502) staff       (20)        0 2024-05-10 05:36:53.000000 santex-1.2.1/santex/tensor/__init__.py
+-rw-r--r--   0 usin8611   (502) staff       (20)     3445 2024-04-26 03:55:11.000000 santex-1.2.1/santex/tensor/tensor.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.687171 santex-1.2.1/santex.egg-info/
+-rw-r--r--   0 usin8611   (502) staff       (20)     2897 2024-05-10 06:22:36.000000 santex-1.2.1/santex.egg-info/PKG-INFO
+-rw-r--r--   0 usin8611   (502) staff       (20)     1018 2024-05-10 06:22:36.000000 santex-1.2.1/santex.egg-info/SOURCES.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)        1 2024-05-10 06:22:36.000000 santex-1.2.1/santex.egg-info/dependency_links.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)       91 2024-05-10 06:22:36.000000 santex-1.2.1/santex.egg-info/requires.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)        7 2024-05-10 06:22:36.000000 santex-1.2.1/santex.egg-info/top_level.txt
+-rw-r--r--   0 usin8611   (502) staff       (20)       38 2024-05-10 06:22:36.688023 santex-1.2.1/setup.cfg
+-rw-r--r--   0 usin8611   (502) staff       (20)     1712 2024-05-10 06:19:55.000000 santex-1.2.1/setup.py
+drwxr-xr-x   0 usin8611   (502) staff       (20)        0 2024-05-10 06:22:36.686690 santex-1.2.1/tests/
+-rw-r--r--   0 usin8611   (502) staff       (20)     2538 2024-05-06 05:33:45.000000 santex-1.2.1/tests/test.py
```

### Comparing `santex-1.2/LICENSE` & `santex-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `santex-1.2/PKG-INFO` & `santex-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: santex
-Version: 1.2
+Version: 1.2.1
 Summary: SAnTeX is a Python library which calculates seismic anisotropy from full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature. SAnTex facilitates the processing and cleaning of EBSD data and calculation of Orientation Distribution Function (ODF) and Inverse pole figure (IPF)
 Home-page: https://github.com/utpal-singh/SAnTex
 Author: Utpal Singh
 Author-email: utpal_singh@yahoo.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: python,seismic,seismic anisotropy,EBSD,Texture,Crystallography
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `santex-1.2/README.md` & `santex-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/anisotropy/anisotropy.py` & `santex-1.2.1/santex/anisotropy/anisotropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 from .vtkplotter import Plotter
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from .plot_vel_grid import plot_velocity_grid
 from .utils import christoffel_tensor, wave_property
 
-from .. import Material
-from .. import EBSD
-
 from scipy.interpolate import griddata
 import math
 
 class Anisotropy:
     """
     Anisotropy class for representing anisotropic material properties.
 
@@ -240,15 +237,15 @@
             print("Max Vs2: ", maxvs2)
             print("Min Vs2: ", minvs2)
             print("Max vs anisotropy percent: ", max_vs_anisotropy_percent)
             print("Min vs anisotropy percent: ", min_vs_anisotropy_percent)
             print("P wave anisotropy percent: ", p_wave_anisotropy_percent)
             print("S1 Wave anisotropy percent: ", s1_wave_anisotropy_percent)
             print("S2 Wave anisotropy percent: ", s2_wave_anisotropy_percent)
-            print("Velocity difference: ", maxdvs)
+            print("Velocity difference, maxdvs: ", maxdvs)
             print("Vp/Vs1 ratio: ", AVpVs1)
             return {
                 'maxvp': maxvp,
                 'minvp': minvp,
                 'maxvs1': maxvs1,
                 'minvs1': minvs1,
                 'maxvs2': maxvs2,
```

### Comparing `santex-1.2/santex/anisotropy/map.py` & `santex-1.2.1/santex/anisotropy/map.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/anisotropy/melt.py` & `santex-1.2.1/santex/anisotropy/melt.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/anisotropy/modalAnisotropy.py` & `santex-1.2.1/santex/anisotropy/modalAnisotropy.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/anisotropy/plot_seismic_velocity.py` & `santex-1.2.1/santex/anisotropy/plot_seismic_velocity.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/anisotropy/plot_vel_grid.py` & `santex-1.2.1/santex/anisotropy/plot_vel_grid.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/anisotropy/utils.py` & `santex-1.2.1/santex/anisotropy/utils.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/anisotropy/vtkplotter.py` & `santex-1.2.1/santex/anisotropy/vtkplotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from vtk import (
     vtkStructuredGrid, vtkPoints, vtkFloatArray,
     vtkStructuredGridGeometryFilter, vtkPolyDataMapper,
     vtkActor, vtkRenderer, vtkRenderWindow,
     vtkRenderWindowInteractor
 )
-from ..tensor.tensor import Tensor
+from santex import Tensor
 from .utils import christoffel_tensor, wave_property
 
 tensor = Tensor()
 class Plotter:
     """
     A class for plotting seismic wave velocities in 3D using VTK.
```

### Comparing `santex-1.2/santex/ebsd/_ctf_parser.py` & `santex-1.2.1/santex/ebsd/_ctf_parser.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/ebsd/calcGrainBoundary.py` & `santex-1.2.1/santex/ebsd/calcGrainBoundary.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/ebsd/ebsd.py` & `santex-1.2.1/santex/ebsd/ebsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # sage/ebsd/ebsd.py
 
 from ._ctf_parser import Ctf
 import matplotlib.pyplot as plt 
-from tabulate import tabulate
 import os
 
 import numpy as np 
 import pandas as pd 
-from ..tensor import Tensor
+from ..tensor.tensor import Tensor
 from scipy.spatial.transform import Rotation
 
 from .calcGrainBoundary import assign_to_grains_parallel
 import plotly.express as px
 
 from .melt_tensor import calcMelttensor
 from .rotateEBSD import apply_custom_rotation_to_dataframe, apply_custom_rotation_to_dataframe_noxy
```

### Comparing `santex-1.2/santex/ebsd/melt_tensor.py` & `santex-1.2.1/santex/ebsd/melt_tensor.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/ebsd/odf.py` & `santex-1.2.1/santex/ebsd/odf.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/ebsd/rotateEBSD.py` & `santex-1.2.1/santex/ebsd/rotateEBSD.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/ebsd/saveEBSD.py` & `santex-1.2.1/santex/ebsd/saveEBSD.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/isotropy/data/materials.json` & `santex-1.2.1/santex/isotropy/data/materials.json`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/isotropy/isotropy.py` & `santex-1.2.1/santex/isotropy/isotropy.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/material/data/derivatives_P.json` & `santex-1.2.1/santex/material/data/derivatives_P.json`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/material/data/derivatives_T.json` & `santex-1.2.1/santex/material/data/derivatives_T.json`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/material/data/materials_database.json` & `santex-1.2.1/santex/material/data/materials_database.json`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex/material/material.py` & `santex-1.2.1/santex/material/material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import numpy as np
 import pandas as pd
 from tabulate import tabulate
-from ..isotropy import Isotropy
+from ..isotropy.isotropy import Isotropy
 
 class Material:
     def __init__(self, database_path=os.path.join(os.path.dirname(__file__), 'data/materials_database.json'), database_path2=os.path.join(os.path.dirname(__file__), 'data/derivatives_P.json'), database_path3=os.path.join(os.path.dirname(__file__),'data/derivatives_T.json')):
         """
         Initialize a Material object with data loaded from JSON files.
 
         Parameters:
```

### Comparing `santex-1.2/santex/tensor/tensor.py` & `santex-1.2.1/santex/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `santex-1.2/santex.egg-info/PKG-INFO` & `santex-1.2.1/santex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: santex
-Version: 1.2
+Version: 1.2.1
 Summary: SAnTeX is a Python library which calculates seismic anisotropy from full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature. SAnTex facilitates the processing and cleaning of EBSD data and calculation of Orientation Distribution Function (ODF) and Inverse pole figure (IPF)
 Home-page: https://github.com/utpal-singh/SAnTex
 Author: Utpal Singh
 Author-email: utpal_singh@yahoo.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: python,seismic,seismic anisotropy,EBSD,Texture,Crystallography
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `santex-1.2/santex.egg-info/SOURCES.txt` & `santex-1.2.1/santex.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 santex/isotropy/data/materials.json
 santex/material/__init__.py
 santex/material/material.py
 santex/material/data/derivatives_P.json
 santex/material/data/derivatives_T.json
 santex/material/data/materials_database.json
 santex/tensor/__init__.py
-santex/tensor/tensor.py
+santex/tensor/tensor.py
+tests/test.py
```

### Comparing `santex-1.2/setup.py` & `santex-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2'
+VERSION = '1.2.1'
 DESCRIPTION = "SAnTeX is a Python library which calculates seismic anisotropy from full elastic tensor of rocks from modal mineral composition, crystallographic orientation, and a crystal stiffness tensor catalogue that accounts for the dependency of elasticity with pressure and temperature. SAnTex facilitates the processing and cleaning of EBSD data and calculation of Orientation Distribution Function (ODF) and Inverse pole figure (IPF)"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='santex',
```

