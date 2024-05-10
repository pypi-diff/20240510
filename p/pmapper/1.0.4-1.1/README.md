# Comparing `tmp/pmapper-1.0.4.tar.gz` & `tmp/pmapper-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmapper-1.0.4.tar", last modified: Mon Nov 13 12:38:49 2023, max compression
+gzip compressed data, was "dist/pmapper-1.1.tar", last modified: Fri May 10 21:34:52 2024, max compression
```

## Comparing `pmapper-1.0.4.tar` & `pmapper-1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-11-13 12:38:49.000000 pmapper-1.0.4/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    14064 2023-11-13 12:38:49.000000 pmapper-1.0.4/PKG-INFO
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    14064 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      494 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      145 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       36 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-11-13 12:38:49.000000 pmapper-1.0.4/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2095 2020-08-19 11:56:09.000000 pmapper-1.0.4/pmapper/smarts_features.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3341 2019-10-27 09:29:24.000000 pmapper-1.0.4/pmapper/get_pharm_counts.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2838 2023-03-22 13:10:53.000000 pmapper-1.0.4/pmapper/utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    43863 2023-03-22 13:09:37.000000 pmapper-1.0.4/pmapper/pharmacophore.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      379 2023-11-13 12:36:11.000000 pmapper-1.0.4/pmapper/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-11-13 12:38:49.000000 pmapper-1.0.4/pmapper/speedtest/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2019-11-28 20:48:52.000000 pmapper-1.0.4/pmapper/speedtest/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)   639575 2019-11-28 15:39:27.000000 pmapper-1.0.4/pmapper/speedtest/confs.pkl
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2280 2020-03-22 21:10:06.000000 pmapper-1.0.4/pmapper/speedtest/pmapper_speed_test.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1958 2020-08-19 11:56:09.000000 pmapper-1.0.4/pmapper/customize.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3387 2019-10-27 09:29:24.000000 pmapper-1.0.4/pmapper/smarts_features.fdef
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11285 2023-11-13 12:36:11.000000 pmapper-1.0.4/README.md
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2019-11-28 20:54:08.000000 pmapper-1.0.4/MANIFEST.in
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1287 2023-11-13 12:10:30.000000 pmapper-1.0.4/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-10 21:34:52.000000 pmapper-1.1/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2019-10-27 09:29:24.000000 pmapper-1.1/LICENSE.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    14190 2024-05-10 21:34:52.000000 pmapper-1.1/PKG-INFO
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper.egg-info/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)    14190 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      506 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      145 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       36 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2024-05-10 21:34:52.000000 pmapper-1.1/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2130 2024-05-10 21:22:51.000000 pmapper-1.1/pmapper/smarts_features.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3341 2019-10-27 09:29:24.000000 pmapper-1.1/pmapper/get_pharm_counts.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2838 2023-03-22 13:10:53.000000 pmapper-1.1/pmapper/utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    43863 2023-03-22 13:09:37.000000 pmapper-1.1/pmapper/pharmacophore.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      377 2024-05-10 21:32:18.000000 pmapper-1.1/pmapper/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-10 21:34:52.000000 pmapper-1.1/pmapper/speedtest/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2019-11-28 20:48:52.000000 pmapper-1.1/pmapper/speedtest/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)   639575 2019-11-28 15:39:27.000000 pmapper-1.1/pmapper/speedtest/confs.pkl
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2280 2020-03-22 21:10:06.000000 pmapper-1.1/pmapper/speedtest/pmapper_speed_test.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1958 2020-08-19 11:56:09.000000 pmapper-1.1/pmapper/customize.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3387 2019-10-27 09:29:24.000000 pmapper-1.1/pmapper/smarts_features.fdef
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11389 2024-05-10 21:32:01.000000 pmapper-1.1/README.md
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2019-11-28 20:54:08.000000 pmapper-1.1/MANIFEST.in
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1287 2023-11-13 12:10:30.000000 pmapper-1.1/setup.py
```

### Comparing `pmapper-1.0.4/PKG-INFO` & `pmapper-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmapper
-Version: 1.0.4
+Version: 1.1
 Summary: pmapper: 3D pharmacophore hashes and fingerprints
 Home-page: https://github.com/DrrDom/pmapper
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # Pmapper - 3D pharmacophore signatures and fingerprints
         
@@ -41,14 +41,17 @@
         - add `get_subpharmacophore` function
         - fix `get_mirror_pharmacophore` function to use the same bin step and cached args as for the source pharmacophore instance  
         
         **1.0.4**
         - fix installation of dependency `networkx`
         - add citations on examples of `pmapper` descriptors used for machine learning
         
+        **1.1**
+        - change SMARTS pattern to avoid matching positively charge nitrogen atoms as H-bond acceptors
+        
         ## Examples
         
         ### Load modules
         ```python
         from pmapper.pharmacophore import Pharmacophore as P
         from rdkit import Chem
         from rdkit.Chem import AllChem
```

### Comparing `pmapper-1.0.4/pmapper.egg-info/PKG-INFO` & `pmapper-1.1/pmapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmapper
-Version: 1.0.4
+Version: 1.1
 Summary: pmapper: 3D pharmacophore hashes and fingerprints
 Home-page: https://github.com/DrrDom/pmapper
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # Pmapper - 3D pharmacophore signatures and fingerprints
         
@@ -41,14 +41,17 @@
         - add `get_subpharmacophore` function
         - fix `get_mirror_pharmacophore` function to use the same bin step and cached args as for the source pharmacophore instance  
         
         **1.0.4**
         - fix installation of dependency `networkx`
         - add citations on examples of `pmapper` descriptors used for machine learning
         
+        **1.1**
+        - change SMARTS pattern to avoid matching positively charge nitrogen atoms as H-bond acceptors
+        
         ## Examples
         
         ### Load modules
         ```python
         from pmapper.pharmacophore import Pharmacophore as P
         from rdkit import Chem
         from rdkit.Chem import AllChem
```

### Comparing `pmapper-1.0.4/pmapper/smarts_features.txt` & `pmapper-1.1/pmapper/smarts_features.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # HBD
 [#7!H0&!$(N-[SX4](=O)(=O)[CX4](F)(F)F)] D
 [#8!H0&!$([OH][C,S,P]=O)] D
 [#16!H0] D
 
 # HBA
-[#7&!$([nX3])&!$([NX3]-*=[!#6])&!$([NX3]-[a])&!$([NX4])&!$(N=C([C,N])N)] A
+[#7&!$([nX3])&!$([NX3]-*=[!#6])&!$([NX3]-[a])&!$([NX4])&!$(N=C([C,N])N)&!$([NX3]([CX4])([CX4,#1])[CX4,#1])] A
 [$([O])&!$([OX2](C)C=O)&!$(*(~a)~a)] A
 
 # positive
 # [+,+2,+3,+4] P
 # [$(CC)](=[N+0])[N+0] P
 # [$(C(N+0)(N+0)=[N+0])] P
 # [$([n+0]1cc[nH]c1)] P
```

### Comparing `pmapper-1.0.4/pmapper/get_pharm_counts.py` & `pmapper-1.1/pmapper/get_pharm_counts.py`

 * *Files identical despite different names*

### Comparing `pmapper-1.0.4/pmapper/utils.py` & `pmapper-1.1/pmapper/utils.py`

 * *Files identical despite different names*

### Comparing `pmapper-1.0.4/pmapper/pharmacophore.py` & `pmapper-1.1/pmapper/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `pmapper-1.0.4/pmapper/speedtest/confs.pkl` & `pmapper-1.1/pmapper/speedtest/confs.pkl`

 * *Files identical despite different names*

### Comparing `pmapper-1.0.4/pmapper/speedtest/pmapper_speed_test.py` & `pmapper-1.1/pmapper/speedtest/pmapper_speed_test.py`

 * *Files identical despite different names*

### Comparing `pmapper-1.0.4/pmapper/customize.py` & `pmapper-1.1/pmapper/customize.py`

 * *Files identical despite different names*

### Comparing `pmapper-1.0.4/pmapper/smarts_features.fdef` & `pmapper-1.1/pmapper/smarts_features.fdef`

 * *Files identical despite different names*

### Comparing `pmapper-1.0.4/README.md` & `pmapper-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 - add `get_subpharmacophore` function
 - fix `get_mirror_pharmacophore` function to use the same bin step and cached args as for the source pharmacophore instance  
 
 **1.0.4**
 - fix installation of dependency `networkx`
 - add citations on examples of `pmapper` descriptors used for machine learning
 
+**1.1**
+- change SMARTS pattern to avoid matching positively charge nitrogen atoms as H-bond acceptors
+
 ## Examples
 
 ### Load modules
 ```python
 from pmapper.pharmacophore import Pharmacophore as P
 from rdkit import Chem
 from rdkit.Chem import AllChem
```

### Comparing `pmapper-1.0.4/setup.py` & `pmapper-1.1/setup.py`

 * *Files identical despite different names*

