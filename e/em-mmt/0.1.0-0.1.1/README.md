# Comparing `tmp/em_mmt-0.1.0.tar.gz` & `tmp/em_mmt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "em_mmt-0.1.0.tar", max compression
+gzip compressed data, was "em_mmt-0.1.1.tar", max compression
```

## Comparing `em_mmt-0.1.0.tar` & `em_mmt-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-09 19:28:06.353713 em_mmt-0.1.0/README.md
--rw-r--r--   0        0        0       21 2024-05-10 02:10:33.799448 em_mmt-0.1.0/em_mmt/__init__.py
--rw-r--r--   0        0        0    49790 2024-05-10 03:29:31.257637 em_mmt-0.1.0/em_mmt/em_mmt.py
--rw-r--r--   0        0        0      444 2024-05-09 22:49:54.846858 em_mmt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 em_mmt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-09 19:28:06.353713 em_mmt-0.1.1/README.md
+-rw-r--r--   0        0        0       21 2024-05-10 16:19:35.737031 em_mmt-0.1.1/em_mmt/__init__.py
+-rw-r--r--   0        0        0    49639 2024-05-10 16:20:08.968280 em_mmt-0.1.1/em_mmt/em_mmt.py
+-rw-r--r--   0        0        0      532 2024-05-10 16:19:30.355803 em_mmt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 em_mmt-0.1.1/PKG-INFO
```

### Comparing `em_mmt-0.1.0/em_mmt/em_mmt.py` & `em_mmt-0.1.1/em_mmt/em_mmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8-*-
 
 ###### MMT IndeX #######
-## Version 0.1 ##
+## Version 0.1.1 ##
 
 # Standard library imports
 import os
 import sys
 import time
 import re
 from itertools import combinations, permutations
@@ -201,16 +201,14 @@
     def check_pair_inputs(self, data=None):
         if data is None:
             raise ValueError("ERROR: No data is provided")
         if 'Control' not in data.columns:
             raise ValueError("ERROR: Control variable not found in input data")
         if 'Exposed' not in data.columns:
             raise ValueError("ERROR: Exposed variable not found in input data")
-        if ['Exposed', 'Control'] != list(data.columns):
-            raise ValueError("ERROR: Exposed and Control variables out of order in input data")
         if data['Control'].isna().any():
             raise ValueError("ERROR: NAs found in the Control variable")
         if data['Exposed'].isna().any():
             raise ValueError("ERROR: NAs found in the Exposed variable")
         if data['Control'].isnull().any():
             raise ValueError("ERROR: NULLs found in the Control variable")
         if data['Exposed'].isnull().any():
```

### Comparing `em_mmt-0.1.0/PKG-INFO` & `em_mmt-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: em-mmt
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: This is a wrapper that combines Dynamic Time Warping and Casual Impact into one library.
 Author: Marcus Hilliard
 Author-email: marcus.hilliard@essencemediacom.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

