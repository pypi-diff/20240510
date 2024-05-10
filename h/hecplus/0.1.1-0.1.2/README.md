# Comparing `tmp/hecplus-0.1.1.tar.gz` & `tmp/hecplus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hecplus-0.1.1.tar", last modified: Fri May 10 00:07:36 2024, max compression
+gzip compressed data, was "hecplus-0.1.2.tar", last modified: Fri May 10 00:14:39 2024, max compression
```

## Comparing `hecplus-0.1.1.tar` & `hecplus-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 00:07:36.486310 hecplus-0.1.1/
--rw-rw-rw-   0        0        0     1084 2024-05-09 23:34:27.000000 hecplus-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1298 2024-05-10 00:07:36.482303 hecplus-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-05-10 00:06:41.000000 hecplus-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 00:07:36.458680 hecplus-0.1.1/hecplus/
--rw-rw-rw-   0        0        0      438 2024-05-10 00:05:55.000000 hecplus-0.1.1/hecplus/__init__.py
--rw-rw-rw-   0        0        0     9375 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hechms.py
--rw-rw-rw-   0        0        0    13480 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hechms_basin.py
--rw-rw-rw-   0        0        0    12500 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hecras.py
--rw-rw-rw-   0        0        0     3381 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hecras_controller.py
--rw-rw-rw-   0        0        0     9735 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hecras_flow_unsteady.py
--rw-rw-rw-   0        0        0    33515 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hecras_geom.py
--rw-rw-rw-   0        0        0     1845 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hecras_plan.py
--rw-rw-rw-   0        0        0    20021 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hecras_results.py
--rw-rw-rw-   0        0        0     1101 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_class_hecras_review.py
--rw-rw-rw-   0        0        0    19332 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_functions_hec.py
--rw-rw-rw-   0        0        0     5547 2024-05-09 23:34:27.000000 hecplus-0.1.1/hecplus/pb_functions_hechms.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:07:36.479370 hecplus-0.1.1/hecplus.egg-info/
--rw-rw-rw-   0        0        0     1298 2024-05-10 00:07:36.000000 hecplus-0.1.1/hecplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2024-05-10 00:07:36.000000 hecplus-0.1.1/hecplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 00:07:36.000000 hecplus-0.1.1/hecplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-10 00:07:36.000000 hecplus-0.1.1/hecplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 00:07:36.000000 hecplus-0.1.1/hecplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 00:07:36.487789 hecplus-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1697 2024-05-10 00:05:18.000000 hecplus-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:14:39.547032 hecplus-0.1.2/
+-rw-rw-rw-   0        0        0     1084 2024-05-09 23:34:27.000000 hecplus-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1178 2024-05-10 00:14:39.542616 hecplus-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2024-05-10 00:13:17.000000 hecplus-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 00:14:39.520615 hecplus-0.1.2/hecplus/
+-rw-rw-rw-   0        0        0      438 2024-05-10 00:14:18.000000 hecplus-0.1.2/hecplus/__init__.py
+-rw-rw-rw-   0        0        0     9375 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hechms.py
+-rw-rw-rw-   0        0        0    13480 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hechms_basin.py
+-rw-rw-rw-   0        0        0    12500 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hecras.py
+-rw-rw-rw-   0        0        0     3381 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hecras_controller.py
+-rw-rw-rw-   0        0        0     9735 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hecras_flow_unsteady.py
+-rw-rw-rw-   0        0        0    33515 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hecras_geom.py
+-rw-rw-rw-   0        0        0     1845 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hecras_plan.py
+-rw-rw-rw-   0        0        0    20021 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hecras_results.py
+-rw-rw-rw-   0        0        0     1101 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_class_hecras_review.py
+-rw-rw-rw-   0        0        0    19332 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_functions_hec.py
+-rw-rw-rw-   0        0        0     5547 2024-05-09 23:34:27.000000 hecplus-0.1.2/hecplus/pb_functions_hechms.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:14:39.540022 hecplus-0.1.2/hecplus.egg-info/
+-rw-rw-rw-   0        0        0     1178 2024-05-10 00:14:39.000000 hecplus-0.1.2/hecplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2024-05-10 00:14:39.000000 hecplus-0.1.2/hecplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 00:14:39.000000 hecplus-0.1.2/hecplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-10 00:14:39.000000 hecplus-0.1.2/hecplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 00:14:39.000000 hecplus-0.1.2/hecplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 00:14:39.547032 hecplus-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1395 2024-05-10 00:13:49.000000 hecplus-0.1.2/setup.py
```

### Comparing `hecplus-0.1.1/LICENSE` & `hecplus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/PKG-INFO` & `hecplus-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: hecplus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Helper functions for working with Hydrologic Engineering Center (HEC) softwares
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: hec,hecras,hechms
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dsplus>=0.4.9
 Requires-Dist: pandas>=2.0
 Requires-Dist: h5py>=3.10.0
 Requires-Dist: pydsstools>=2.3.1
 
 This package contains helper functions for working with Hydrologic Engineering Center (HEC) softwares.
 
-This package is still in the beta stage. The current version only works with HEC-HMS and HEC-RAS. Please expect frequent updates to fix bugs and add functionalities.
+This package is still in the beta stage. The current version works with HEC-HMS and HEC-RAS. Please expect frequent updates to fix bugs and add functionalities. A full documentation will be added soon.
 
 # Installation
 
 ```bash
 pip install hecplus
 ```
```

### Comparing `hecplus-0.1.1/hecplus/pb_class_hechms.py` & `hecplus-0.1.2/hecplus/pb_class_hechms.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hechms_basin.py` & `hecplus-0.1.2/hecplus/pb_class_hechms_basin.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hecras.py` & `hecplus-0.1.2/hecplus/pb_class_hecras.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hecras_controller.py` & `hecplus-0.1.2/hecplus/pb_class_hecras_controller.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hecras_flow_unsteady.py` & `hecplus-0.1.2/hecplus/pb_class_hecras_flow_unsteady.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hecras_geom.py` & `hecplus-0.1.2/hecplus/pb_class_hecras_geom.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hecras_plan.py` & `hecplus-0.1.2/hecplus/pb_class_hecras_plan.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hecras_results.py` & `hecplus-0.1.2/hecplus/pb_class_hecras_results.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_class_hecras_review.py` & `hecplus-0.1.2/hecplus/pb_class_hecras_review.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_functions_hec.py` & `hecplus-0.1.2/hecplus/pb_functions_hec.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus/pb_functions_hechms.py` & `hecplus-0.1.2/hecplus/pb_functions_hechms.py`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/hecplus.egg-info/PKG-INFO` & `hecplus-0.1.2/hecplus.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: hecplus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Helper functions for working with Hydrologic Engineering Center (HEC) softwares
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: hec,hecras,hechms
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dsplus>=0.4.9
 Requires-Dist: pandas>=2.0
 Requires-Dist: h5py>=3.10.0
 Requires-Dist: pydsstools>=2.3.1
 
 This package contains helper functions for working with Hydrologic Engineering Center (HEC) softwares.
 
-This package is still in the beta stage. The current version only works with HEC-HMS and HEC-RAS. Please expect frequent updates to fix bugs and add functionalities.
+This package is still in the beta stage. The current version works with HEC-HMS and HEC-RAS. Please expect frequent updates to fix bugs and add functionalities. A full documentation will be added soon.
 
 # Installation
 
 ```bash
 pip install hecplus
 ```
```

### Comparing `hecplus-0.1.1/hecplus.egg-info/SOURCES.txt` & `hecplus-0.1.2/hecplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hecplus-0.1.1/setup.py` & `hecplus-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,19 @@
     # py_modules=['dsplus'],
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
-        'License :: OSI Approved :: MIT License',
-        # 'Operating System :: OS Independent',
-        'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
         # 'Programming Language :: Python :: Implementation :: CPython',
         # 'Programming Language :: Python :: Implementation :: PyPy',
-        # 'Intended Audience :: Developers',
-        # 'Intended Audience :: Information Technology',
-        # 'Intended Audience :: Education',
+        'License :: OSI Approved :: MIT License',
+        'Development Status :: 4 - Beta',
+        # 'Operating System :: OS Independent',
         'Topic :: Scientific/Engineering :: Hydrology',
     ],
     python_requires='>=3.10',
     install_requires=[
         'dsplus>=0.4.9',
         'pandas>=2.0',
         'h5py>=3.10.0',
```

