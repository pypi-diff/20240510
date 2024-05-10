# Comparing `tmp/FairFRU-0.2.6.tar.gz` & `tmp/FairFRU-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FairFRU-0.2.6.tar", last modified: Wed Mar 20 13:24:35 2024, max compression
+gzip compressed data, was "FairFRU-0.2.7.tar", last modified: Fri May 10 14:50:16 2024, max compression
```

## Comparing `FairFRU-0.2.6.tar` & `FairFRU-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 13:24:35.989786 FairFRU-0.2.6/
-drwxrwxrwx   0        0        0        0 2024-03-20 13:24:35.962900 FairFRU-0.2.6/FairFRU/
--rw-rw-rw-   0        0        0     1922 2024-03-20 13:23:28.000000 FairFRU-0.2.6/FairFRU/FRSpy.py
--rw-rw-rw-   0        0        0      186 2023-12-06 16:42:13.000000 FairFRU-0.2.6/FairFRU/__init__.py
--rw-rw-rw-   0        0        0     3191 2024-03-20 13:23:30.000000 FairFRU-0.2.6/FairFRU/fuzzy_rough_regions.py
--rw-rw-rw-   0        0        0     3143 2024-03-20 11:15:09.000000 FairFRU-0.2.6/FairFRU/fuzzy_rough_uncertainty.py
--rw-rw-rw-   0        0        0     2569 2024-03-20 13:23:26.000000 FairFRU-0.2.6/FairFRU/h5file_create_array.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:24:35.982783 FairFRU-0.2.6/FairFRU.egg-info/
--rw-rw-rw-   0        0        0      690 2024-03-20 13:24:35.000000 FairFRU-0.2.6/FairFRU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-03-20 13:24:35.000000 FairFRU-0.2.6/FairFRU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 13:24:35.000000 FairFRU-0.2.6/FairFRU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-20 13:24:35.000000 FairFRU-0.2.6/FairFRU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      690 2024-03-20 13:24:35.987011 FairFRU-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-11-23 14:54:33.000000 FairFRU-0.2.6/README.md
--rw-rw-rw-   0        0        0     1091 2023-11-23 14:55:13.000000 FairFRU-0.2.6/license.txt
--rw-rw-rw-   0        0        0       42 2024-03-20 13:24:35.990783 FairFRU-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      450 2024-03-20 13:24:16.000000 FairFRU-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:50:16.262193 FairFRU-0.2.7/
+drwxrwxrwx   0        0        0        0 2024-05-10 14:50:16.233661 FairFRU-0.2.7/FairFRU/
+-rw-rw-rw-   0        0        0     1922 2024-03-20 13:23:28.000000 FairFRU-0.2.7/FairFRU/FRSpy.py
+-rw-rw-rw-   0        0        0      186 2023-12-06 16:42:13.000000 FairFRU-0.2.7/FairFRU/__init__.py
+-rw-rw-rw-   0        0        0     3313 2024-05-10 14:45:36.000000 FairFRU-0.2.7/FairFRU/fuzzy_rough_regions.py
+-rw-rw-rw-   0        0        0     3143 2024-03-20 11:15:09.000000 FairFRU-0.2.7/FairFRU/fuzzy_rough_uncertainty.py
+-rw-rw-rw-   0        0        0     2569 2024-03-20 13:23:26.000000 FairFRU-0.2.7/FairFRU/h5file_create_array.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:50:16.255192 FairFRU-0.2.7/FairFRU.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-05-10 14:50:16.000000 FairFRU-0.2.7/FairFRU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-10 14:50:16.000000 FairFRU-0.2.7/FairFRU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:50:16.000000 FairFRU-0.2.7/FairFRU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 14:50:16.000000 FairFRU-0.2.7/FairFRU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      690 2024-05-10 14:50:16.259192 FairFRU-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-11-23 14:54:33.000000 FairFRU-0.2.7/README.md
+-rw-rw-rw-   0        0        0     1091 2023-11-23 14:55:13.000000 FairFRU-0.2.7/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:50:16.263206 FairFRU-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      450 2024-05-10 14:48:39.000000 FairFRU-0.2.7/setup.py
```

### Comparing `FairFRU-0.2.6/FairFRU/FRSpy.py` & `FairFRU-0.2.7/FairFRU/FRSpy.py`

 * *Files identical despite different names*

### Comparing `FairFRU-0.2.6/FairFRU/fuzzy_rough_regions.py` & `FairFRU-0.2.7/FairFRU/fuzzy_rough_regions.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     Writearray(df.iloc[:,:-1], 0.5).sim_array(h5file = h5file, group = group, hide_progress = hide_progress)
 
     h5file.close()
 
     h5file = open_file(file_name, mode="r")
     frregions = FRSpy(target, membership).regions(file_name,'full', hide_progress = hide_progress)
 
-    with open('full_mem.pickle', 'wb') as handle:
+    file_name_pickle = os.path.join(path, 'full_mem.pickle')
+    with open(file_name_pickle, 'wb') as handle:
       pickle.dump(frregions, handle, protocol=pickle.HIGHEST_PROTOCOL)
     h5file.close()
 
     h5file = h5py.File(file_name, mode="a")
     del h5file['full']
     h5file.close()
 
@@ -70,15 +71,16 @@
     group = h5file.create_group("/", s_attr, 'Distances after removing '+s_attr)
     Writearray(dataset, 0.5).sim_array(h5file = h5file, group = group, hide_progress = hide_progress)
 
     h5file.close()
     h5file = open_file(file_name, mode="r")
 
     frregions = FRSpy(target, membership).regions(file_name,s_attr, hide_progress = hide_progress)
-    with open(s_attr+'_mem.pickle', 'wb') as handle:
+    file_name_pickle = os.path.join(path, s_attr+'_mem.pickle')
+    with open(file_name_pickle, 'wb') as handle:
       pickle.dump(frregions, handle, protocol=pickle.HIGHEST_PROTOCOL)
     h5file.close()
 
     h5file = h5py.File(file_name, mode="a")
     del h5file[s_attr]
     h5file.close()
```

### Comparing `FairFRU-0.2.6/FairFRU/fuzzy_rough_uncertainty.py` & `FairFRU-0.2.7/FairFRU/fuzzy_rough_uncertainty.py`

 * *Files identical despite different names*

### Comparing `FairFRU-0.2.6/FairFRU/h5file_create_array.py` & `FairFRU-0.2.7/FairFRU/h5file_create_array.py`

 * *Files identical despite different names*

### Comparing `FairFRU-0.2.6/FairFRU.egg-info/PKG-INFO` & `FairFRU-0.2.7/FairFRU.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FairFRU
-Version: 0.2.6
+Version: 0.2.7
 Summary: A bias measure using the fuzzy rough set theory
 Author: Lisa Koutsoviti, Gonzalo Napoles
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Using fuzzy-rough sets to measure bias in pattern classification problems
```

### Comparing `FairFRU-0.2.6/PKG-INFO` & `FairFRU-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FairFRU
-Version: 0.2.6
+Version: 0.2.7
 Summary: A bias measure using the fuzzy rough set theory
 Author: Lisa Koutsoviti, Gonzalo Napoles
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Using fuzzy-rough sets to measure bias in pattern classification problems
```

### Comparing `FairFRU-0.2.6/license.txt` & `FairFRU-0.2.7/license.txt`

 * *Files identical despite different names*

