# Comparing `tmp/trust_plutus_namematch-0.1.0.tar.gz` & `tmp/trust_plutus_namematch-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trust_plutus_namematch-0.1.0.tar", max compression
+gzip compressed data, was "trust_plutus_namematch-0.2.tar", max compression
```

## Comparing `trust_plutus_namematch-0.1.0.tar` & `trust_plutus_namematch-0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-0.1.0/LICENSE
--rw-r--r--   0        0        0      476 2024-05-10 06:52:54.322801 trust_plutus_namematch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      425 2024-05-10 06:51:47.677618 trust_plutus_namematch-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-0.1.0/trust_plutus_namematch/__init__.py
--rw-r--r--   0        0        0     1515 2024-05-10 06:28:57.924280 trust_plutus_namematch-0.1.0/trust_plutus_namematch/match.py
--rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-0.1.0/trust_plutus_namematch/utils/__init__.py
--rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-0.1.0/trust_plutus_namematch/utils/logs.py
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 trust_plutus_namematch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-0.2/LICENSE
+-rw-r--r--   0        0        0      474 2024-05-10 06:54:25.727476 trust_plutus_namematch-0.2/pyproject.toml
+-rw-r--r--   0        0        0      427 2024-05-10 06:53:56.420267 trust_plutus_namematch-0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-0.2/trust_plutus_namematch/__init__.py
+-rw-r--r--   0        0        0     1515 2024-05-10 06:28:57.924280 trust_plutus_namematch-0.2/trust_plutus_namematch/match.py
+-rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-0.2/trust_plutus_namematch/utils/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-0.2/trust_plutus_namematch/utils/logs.py
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 trust_plutus_namematch-0.2/PKG-INFO
```

### Comparing `trust_plutus_namematch-0.1.0/LICENSE` & `trust_plutus_namematch-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trust_plutus_namematch-0.1.0/trust_plutus_namematch/match.py` & `trust_plutus_namematch-0.2/trust_plutus_namematch/match.py`

 * *Files identical despite different names*

### Comparing `trust_plutus_namematch-0.1.0/PKG-INFO` & `trust_plutus_namematch-0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: trust-plutus-namematch
-Version: 0.1.0
+Version: 0.2
 Summary: Name match for fund names from ICRA and MILES
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
 Author: Rolf Lobo
 Requires-Python: ==3.10.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: loga (>=1.0.0,<2.0.0)
 Requires-Dist: numpy (==1.25.2)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: rapidfuzz (==3.9.0)
 Description-Content-Type: text/markdown
 
-# Assumptions: 
-# 1. Column name for Miles and ICRA sheet is "Fund Name"
-# 2. Input and Output file names don't have spaces
-# 3. Sheet names are : "Miles Names" and "ICRA Names"
+#### Assumptions: 
+1. Column name for Miles and ICRA sheet is "Fund Name"
+2. Input and Output file names don't have spaces
+3. Sheet names are : "Miles Names" and "ICRA Names"
 
-Example: 
+#### Example: 
 
 from trust_plutus_namematch.match import NameMatch
 
 nm = NameMatch()
 
 inputPath = "C:\\Users\\rolfl\\Documents\\SchemeNamesDump.xlsx"
 outputPath = "C:\\Users\\rolfl\\Documents\\Result.xlsx"
```

