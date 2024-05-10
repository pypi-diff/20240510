# Comparing `tmp/em_mmt-0.1.1.tar.gz` & `tmp/em_mmt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "em_mmt-0.1.1.tar", max compression
+gzip compressed data, was "em_mmt-0.1.2.tar", max compression
```

## Comparing `em_mmt-0.1.1.tar` & `em_mmt-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-09 19:28:06.353713 em_mmt-0.1.1/README.md
--rw-r--r--   0        0        0       21 2024-05-10 16:19:35.737031 em_mmt-0.1.1/em_mmt/__init__.py
--rw-r--r--   0        0        0    49639 2024-05-10 16:20:08.968280 em_mmt-0.1.1/em_mmt/em_mmt.py
--rw-r--r--   0        0        0      532 2024-05-10 16:19:30.355803 em_mmt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 em_mmt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-09 19:28:06.353713 em_mmt-0.1.2/README.md
+-rw-r--r--   0        0        0       21 2024-05-10 19:28:39.051326 em_mmt-0.1.2/em_mmt/__init__.py
+-rw-r--r--   0        0        0    50826 2024-05-10 19:28:54.319408 em_mmt-0.1.2/em_mmt/em_mmt.py
+-rw-r--r--   0        0        0      532 2024-05-10 19:29:08.219485 em_mmt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 em_mmt-0.1.2/PKG-INFO
```

### Comparing `em_mmt-0.1.1/em_mmt/em_mmt.py` & `em_mmt-0.1.2/em_mmt/em_mmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8-*-
 
 ###### MMT IndeX #######
-## Version 0.1.1 ##
+## Version 0.1.2 ##
 
 # Standard library imports
 import os
 import sys
 import time
 import re
 from itertools import combinations, permutations
@@ -617,14 +617,23 @@
 
         # Prepare arguments for each pair
         args_list = [
             (data, metric, pairs[i], pre_period, post_period, plots, exp_details)
             for i in range(len(pairs))
         ]
 
+        print("Estimating cycle time...")
+        ts0 = time.time()
+        _ = self.calculate_causal_impact_for_pair(args_list[0])
+        ts1 = time.time()
+        totalPTime = (ts0-ts1)/60
+        totalPTimeCore = (totalPTime*len(args_list))/num_processes
+
+        print(f"Estimated total time per core is {np.round_(totalPTimeCore,2)} min or {np.round_(totalPTimeCore/60,2)} hr")
+
         # Create a Pool of workers and map the function to the arguments
         with multiprocessing.Pool(processes=num_processes) as pool:
             results = list(tqdm(pool.imap(self.calculate_causal_impact_for_pair, args_list), total=len(args_list), desc="Processing", ascii=False, ncols=75))
     
         return results
 
     ########################################
@@ -901,17 +910,26 @@
             # Determine the pairs to be tested based on the resuls of the matching
             self.pairs = [None] * len(self.shortest_distances)
             print("Number of market pairs: ", len(self.pairs))
 
             for i in range(len(self.pairs)):
                 self.pairs[i] = [self.shortest_distances.loc[i, 'DMA'], self.shortest_distances.loc[i, 'BestControl']]
 
-            print("The first five pairs:")
-            for i in range(0,5):
-                print("Pair: ", self.pairs[i])
+            try:
+                if len(self.pairs) >= 5:
+                    print("The first five pairs:")
+                    for i in range(0,5):
+                        print("Pair: ", self.pairs[i])
+                else:
+                    print(f"The first {len(self.pairs)} pairs:")
+                    for i in range(len(self.pairs)):
+                        print("Pair: ", self.pairs[i])
+            except Exception as e:
+                print("Function::Print Pairs failed: %s", e)
+                sys.exit(1)
 
             print("######## Determining Casual Impact ########")
 
             # User chose not to use multiprocessing
             if not parallel_processing:
 
                 back_test = self.causal_impact_iter(data = self.df.copy(),
@@ -1032,17 +1050,26 @@
             # Determine the pairs to be tested based on the resuls of the matching
             self.pairs = [None] * len(self.data_pairs)
             print("Number of market pairs: ", len(self.pairs))
 
             for i in range(len(self.pairs)):
                 self.pairs[i] = [self.data_pairs.loc[i, 'Exposed'], self.data_pairs.loc[i, 'Control']]
 
-            print("The first five pairs:")
-            for i in range(0,5):
-                print("Pair: ", self.pairs[i])
+            try:
+                if len(self.pairs) >= 5:
+                    print("The first five pairs:")
+                    for i in range(0,5):
+                        print("Pair: ", self.pairs[i])
+                else:
+                    print(f"The first {len(self.pairs)} pairs:")
+                    for i in range(len(self.pairs)):
+                        print("Pair: ", self.pairs[i])
+            except Exception as e:
+                print("Function::Print Pairs failed: %s", e)
+                sys.exit(1)
 
             print("######## Determining Casual Impact ########")
 
             # User chose not to use multiprocessing
             if not parallel_processing:
 
                 back_test = self.causal_impact_iter(data = self.df.copy(),
```

### Comparing `em_mmt-0.1.1/pyproject.toml` & `em_mmt-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "em-mmt"
-version = "0.1.1"
+version = "0.1.2"
 description = "This is a wrapper that combines Dynamic Time Warping and Casual Impact into one library."
 authors = ["Marcus Hilliard <marcus.hilliard@essencemediacom.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.2.2"
```

### Comparing `em_mmt-0.1.1/PKG-INFO` & `em_mmt-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: em-mmt
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a wrapper that combines Dynamic Time Warping and Casual Impact into one library.
 Author: Marcus Hilliard
 Author-email: marcus.hilliard@essencemediacom.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

