# Comparing `tmp/molcompview-0.1.0.tar.gz` & `tmp/molcompview-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcompview-0.1.0.tar", last modified: Fri May 10 13:01:42 2024, max compression
+gzip compressed data, was "molcompview-0.1.1.tar", last modified: Fri May 10 21:29:56 2024, max compression
```

## Comparing `molcompview-0.1.0.tar` & `molcompview-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:01:42.895094 molcompview-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 13:01:38.000000 molcompview-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-10 13:01:42.895094 molcompview-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-10 13:01:38.000000 molcompview-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:01:42.891094 molcompview-0.1.0/molcompview/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 13:01:38.000000 molcompview-0.1.0/molcompview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-10 13:01:38.000000 molcompview-0.1.0/molcompview/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-10 13:01:38.000000 molcompview-0.1.0/molcompview/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-10 13:01:38.000000 molcompview-0.1.0/molcompview/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-10 13:01:38.000000 molcompview-0.1.0/molcompview/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:01:42.895094 molcompview-0.1.0/molcompview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-10 13:01:42.000000 molcompview-0.1.0/molcompview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 13:01:42.000000 molcompview-0.1.0/molcompview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:01:42.000000 molcompview-0.1.0/molcompview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 13:01:42.000000 molcompview-0.1.0/molcompview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 13:01:42.000000 molcompview-0.1.0/molcompview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 13:01:42.000000 molcompview-0.1.0/molcompview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:01:42.895094 molcompview-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 13:01:38.000000 molcompview-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:56.595163 molcompview-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 21:29:47.000000 molcompview-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-10 21:29:56.595163 molcompview-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-10 21:29:47.000000 molcompview-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:56.591163 molcompview-0.1.1/molcompview/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:56.595163 molcompview-0.1.1/molcompview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:29:56.595163 molcompview-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 21:29:47.000000 molcompview-0.1.1/setup.py
```

### Comparing `molcompview-0.1.0/LICENSE` & `molcompview-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.0/PKG-INFO` & `molcompview-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcompview
-Version: 0.1.0
+Version: 0.1.1
 Summary: MolCompass Visualization Tool: Visualize your Chemical Space
 Home-page: https://github.com/sergsb/molcompview
 Author: Sergey Sosnin
 Author-email: sergey.sosnin@univie.ac.at
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,24 +25,32 @@
 
 The MolCompass application
 =======
 ### Introduction
 
 <img align="left" src="https://user-images.githubusercontent.com/4963384/218703831-1460bc07-7e9f-417e-9b0c-c9675db5de9f.png"> 
 <p align="justify">
-`MolCompassViewer` is a part of the `MolCompass` project. It is a tool that provides a pretrained parametric t-SNE model for chemical space visualization and the visual validation of QSAR/QSPR models.  
+MolCompassViewer is a part of the MolCompass project. It is a tool that provides a pretrained parametric t-SNE model for chemical space visualization and the visual validation of QSAR/QSPR models.  
 </p>
 
 <br clear="left">
 
 ## Installation
-``pip install molcompview``
+The package can be installed: `pip install molcompview`
 <br>
 
 ## Run
+### Demo
+To run the endocrine receptor example described in the manuscript (coming soon), you may do so by executing the following steps.
+```
+molcompview --demo
+```
+Then, wait some time for the calculation of coordinates. After that stage, the browser will open, and you can view the interactive visualization of the chemical space.
+### Your own dataset
+To run on your own dataset, just use:
 ```
 molcompview <input.csv>
 ```
 <br>
 
 ## Usage
 `MolCompassViewer` intelligently identifies the types of columns within the CSV file, selecting an operational mode based on the presence of specific column types, primarily the molecular structures encoded as SMILES strings.
@@ -52,18 +60,25 @@
 
 * STRUCTURE ONLY:
 Activated when only the SMILES column is identified.
 Focuses on visualizing molecular structures, omitting additional features like color layers and QSAR/QSPR model analyses.
 * ALTERNATIVE:
 Triggered when additional categorical or numerical columns are found alongside the SMILES column, excluding the Ground Truth and Probabilities columns.
 Focuses on exploring the chemical space of compounds, which does not apply to the analysis of models. Users can customize point colors in the visualization based on selected properties.
-* NORMAL:
+* FULL:
 Dedicated to the visual analysis of binary QSAR/QSPR models.
 Available when the CSV file comprises SMILES strings along with Ground Truth and predicted probabilities columns, unlocking access to exclusive features for visualizing binary QSAR/QSPR models.
 <img align="left" src="https://github.com/sergsb/molcompview/assets/4963384/4716e786-466a-4412-9f04-b95136bfc1bd.png" width='300px'> 
 
 <br clear="left">
 
+## Applicability domain analysis 
+The applicability domain analysis is possible only in FULL mode for binary classification models. To run this tool, first select a tool from the top left corner of the chemical map, then select an area of interest and release. A new frame will open on the right, displaying statistical parameters and charts calculated exclusively for the selected compounds.
+<img align="left" src="https://github.com/sergsb/molcompview/assets/4963384/43348a05-d700-428d-9112-d11e29d937d4" width='600px'> 
+
+
+<br clear="left">
+
 ## Screenshots
 
 <img align="left" src="https://github.com/sergsb/molcompview/assets/4963384/07be5580-8d21-4f50-b528-80f5b5d0e5f6.png" width='600px'>
```

### Comparing `molcompview-0.1.0/molcompview/actions.py` & `molcompview-0.1.1/molcompview/actions.py`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.0/molcompview/components.py` & `molcompview-0.1.1/molcompview/components.py`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.0/molcompview/functions.py` & `molcompview-0.1.1/molcompview/functions.py`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.0/molcompview/main.py` & `molcompview-0.1.1/molcompview/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import hashlib
 import json
 import sys
 from enum import Enum, IntEnum
 
 __package__ = "molcompview"
 from os.path import isfile, join
-
+from importlib.resources import files, as_file
 import dash_bootstrap_components as dbc
 import base64
 import os
 
 from appdata import AppDataPaths
 
 from . import __x_name__, __y_name__, __smiles_name__, __version__, DatasetState
@@ -88,24 +88,37 @@
         elif len(prob_columns) > 1:
             logging.info("More than one column with values between 0 and 1 found, please specify the column with probabilities")
             return None
         else:
             logging.info("Could not guess the column with probabilities, please specify it manually")
     return guess
 
+
 def main():
-    # Set up the argument parser
     parser = argparse.ArgumentParser(description="Process a CSV file with MolCompass Viewer.")
-    parser.add_argument('file', type=str, help='The path to the CSV file to process')
+    parser.add_argument('file', type=str, nargs='?', default=None, help='The path to the CSV file to process')
+    parser.add_argument('--demo', action='store_true', help='Run with the demo file data/endocrine/er.csv')
     parser.add_argument('--precompute', action='store_true', help='Whether to precompute certain data (default: False)')
     parser.add_argument('--log_level', type=str, default='ERROR', help='Logging level (default: ERROR)')
-    # Parse the arguments
+
     args = parser.parse_args()
-    # Now call your existing main logic with these arguments
-    main_logic(args.file, precompute=args.precompute, log_level=args.log_level)
+
+    # Decide which file to use based on the arguments
+    if args.demo:
+        with as_file(files('molcompview').joinpath(join('data','endocrine-receptor','endocrine.csv'))) as p:
+            file_path = p
+
+    elif args.file:
+        file_path = args.file
+    else:
+        print("Error: No file specified and the --demo flag is not set.")
+        parser.print_help()
+        sys.exit(1)
+
+    main_logic(file_path, precompute=args.precompute, log_level=args.log_level)
 
 def main_logic(file,precompute=False,log_level="ERROR"):
     def make_dropdown(useful_columns):
         return dcc.Dropdown(
             id='dropdown',
             options=[{'label': i, 'value': i} for i in useful_columns],
             value=useful_columns[0]
```

### Comparing `molcompview-0.1.0/molcompview.egg-info/PKG-INFO` & `molcompview-0.1.1/molcompview.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcompview
-Version: 0.1.0
+Version: 0.1.1
 Summary: MolCompass Visualization Tool: Visualize your Chemical Space
 Home-page: https://github.com/sergsb/molcompview
 Author: Sergey Sosnin
 Author-email: sergey.sosnin@univie.ac.at
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,24 +25,32 @@
 
 The MolCompass application
 =======
 ### Introduction
 
 <img align="left" src="https://user-images.githubusercontent.com/4963384/218703831-1460bc07-7e9f-417e-9b0c-c9675db5de9f.png"> 
 <p align="justify">
-`MolCompassViewer` is a part of the `MolCompass` project. It is a tool that provides a pretrained parametric t-SNE model for chemical space visualization and the visual validation of QSAR/QSPR models.  
+MolCompassViewer is a part of the MolCompass project. It is a tool that provides a pretrained parametric t-SNE model for chemical space visualization and the visual validation of QSAR/QSPR models.  
 </p>
 
 <br clear="left">
 
 ## Installation
-``pip install molcompview``
+The package can be installed: `pip install molcompview`
 <br>
 
 ## Run
+### Demo
+To run the endocrine receptor example described in the manuscript (coming soon), you may do so by executing the following steps.
+```
+molcompview --demo
+```
+Then, wait some time for the calculation of coordinates. After that stage, the browser will open, and you can view the interactive visualization of the chemical space.
+### Your own dataset
+To run on your own dataset, just use:
 ```
 molcompview <input.csv>
 ```
 <br>
 
 ## Usage
 `MolCompassViewer` intelligently identifies the types of columns within the CSV file, selecting an operational mode based on the presence of specific column types, primarily the molecular structures encoded as SMILES strings.
@@ -52,18 +60,25 @@
 
 * STRUCTURE ONLY:
 Activated when only the SMILES column is identified.
 Focuses on visualizing molecular structures, omitting additional features like color layers and QSAR/QSPR model analyses.
 * ALTERNATIVE:
 Triggered when additional categorical or numerical columns are found alongside the SMILES column, excluding the Ground Truth and Probabilities columns.
 Focuses on exploring the chemical space of compounds, which does not apply to the analysis of models. Users can customize point colors in the visualization based on selected properties.
-* NORMAL:
+* FULL:
 Dedicated to the visual analysis of binary QSAR/QSPR models.
 Available when the CSV file comprises SMILES strings along with Ground Truth and predicted probabilities columns, unlocking access to exclusive features for visualizing binary QSAR/QSPR models.
 <img align="left" src="https://github.com/sergsb/molcompview/assets/4963384/4716e786-466a-4412-9f04-b95136bfc1bd.png" width='300px'> 
 
 <br clear="left">
 
+## Applicability domain analysis 
+The applicability domain analysis is possible only in FULL mode for binary classification models. To run this tool, first select a tool from the top left corner of the chemical map, then select an area of interest and release. A new frame will open on the right, displaying statistical parameters and charts calculated exclusively for the selected compounds.
+<img align="left" src="https://github.com/sergsb/molcompview/assets/4963384/43348a05-d700-428d-9112-d11e29d937d4" width='600px'> 
+
+
+<br clear="left">
+
 ## Screenshots
 
 <img align="left" src="https://github.com/sergsb/molcompview/assets/4963384/07be5580-8d21-4f50-b528-80f5b5d0e5f6.png" width='600px'>
```

### Comparing `molcompview-0.1.0/setup.py` & `molcompview-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_packages
 
 setup(
     python_requires='>=3.6',  # Your supported Python ranges
     name = "molcompview",
-    version = "0.1.0",
+    version = "0.1.1",
     include_package_data=False,
     packages=find_packages(),
     install_requires=[
         'molcomplib',
         'rdkit',
         'appdata',  
         'numpy',
```

