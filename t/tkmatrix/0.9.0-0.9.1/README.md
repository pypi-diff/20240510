# Comparing `tmp/tkmatrix-0.9.0.tar.gz` & `tmp/tkmatrix-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmatrix-0.9.0.tar", last modified: Thu May  9 07:17:26 2024, max compression
+gzip compressed data, was "tkmatrix-0.9.1.tar", last modified: Fri May 10 13:10:41 2024, max compression
```

## Comparing `tkmatrix-0.9.0.tar` & `tkmatrix-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.671708 tkmatrix-0.9.0/tkmatrix/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/tkmatrix/custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/custom_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/custom_algorithms/custom_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/inject_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/inject_rv_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/programmatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/rv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/tkmatrix/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/tests/test_tkmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    44005 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/tkmatrix_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/tkmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:10:41.797885 tkmatrix-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-10 13:10:41.797885 tkmatrix-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:10:41.797885 tkmatrix-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:10:41.793885 tkmatrix-0.9.1/tkmatrix/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:10:41.797885 tkmatrix-0.9.1/tkmatrix/custom_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/custom_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/custom_algorithms/custom_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/inject_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/inject_rv_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/programmatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/rv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:10:41.797885 tkmatrix-0.9.1/tkmatrix/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/tests/test_tkmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44005 2024-05-10 13:10:30.000000 tkmatrix-0.9.1/tkmatrix/tkmatrix_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:10:41.793885 tkmatrix-0.9.1/tkmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-10 13:10:41.000000 tkmatrix-0.9.1/tkmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-10 13:10:41.000000 tkmatrix-0.9.1/tkmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:10:41.000000 tkmatrix-0.9.1/tkmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-10 13:10:41.000000 tkmatrix-0.9.1/tkmatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 13:10:41.000000 tkmatrix-0.9.1/tkmatrix.egg-info/top_level.txt
```

### Comparing `tkmatrix-0.9.0/LICENSE` & `tkmatrix-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/PKG-INFO` & `tkmatrix-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.9.0
+Version: 0.9.1
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.9.0/README.md` & `tkmatrix-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/setup.py` & `tkmatrix-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.9.0"
+version = "0.9.1"
 setuptools.setup(
     name="tkmatrix",
     version=version,
     author="M. Dévora-Pajares & F.J. Pozuelos",
     author_email="mdevorapajares@protonmail.com",
     description="ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets",
     long_description=long_description,
@@ -21,15 +21,15 @@
     ],
     python_requires='>=3.10',
     install_requires=['argparse==1.4.0',
                         'beautifulsoup4==4.9.3',
                         'configparser==5.0.1',
                         "corner==2.1.0",
                         "ellc==1.8.5",
-                        "lcbuilder==0.18.0",
+                        "lcbuilder==0.18.1",
                         "mock==4.0.3",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "seaborn==0.11.1",
                         'setuptools>=41.0.0',
                         "sklearn==0.0"
     ]
 )
```

### Comparing `tkmatrix-0.9.0/tkmatrix/__main__.py` & `tkmatrix-0.9.1/tkmatrix/__main__.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py` & `tkmatrix-0.9.1/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/custom_algorithms/custom_search.py` & `tkmatrix-0.9.1/tkmatrix/custom_algorithms/custom_search.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/inject_model.py` & `tkmatrix-0.9.1/tkmatrix/inject_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/inject_rv_model.py` & `tkmatrix-0.9.1/tkmatrix/inject_rv_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/programmatic.py` & `tkmatrix-0.9.1/tkmatrix/programmatic.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/properties.yaml` & `tkmatrix-0.9.1/tkmatrix/properties.yaml`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/rv.py` & `tkmatrix-0.9.1/tkmatrix/rv.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/tests/test_tkmatrix.py` & `tkmatrix-0.9.1/tkmatrix/tests/test_tkmatrix.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix/tkmatrix_class.py` & `tkmatrix-0.9.1/tkmatrix/tkmatrix_class.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.0/tkmatrix.egg-info/PKG-INFO` & `tkmatrix-0.9.1/tkmatrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.9.0
+Version: 0.9.1
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.9.0/tkmatrix.egg-info/SOURCES.txt` & `tkmatrix-0.9.1/tkmatrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

