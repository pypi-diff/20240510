# Comparing `tmp/effluent-1.4.1.tar.gz` & `tmp/effluent-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effluent-1.4.1.tar", last modified: Fri Feb 16 12:57:48 2024, max compression
+gzip compressed data, was "effluent-1.4.2.tar", last modified: Fri May 10 05:59:26 2024, max compression
```

## Comparing `effluent-1.4.1.tar` & `effluent-1.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-16 12:57:48.482117 effluent-1.4.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2024-02-16 12:57:35.000000 effluent-1.4.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3518 2024-02-16 12:57:48.482117 effluent-1.4.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2365 2024-02-16 12:57:35.000000 effluent-1.4.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-16 12:57:35.000000 effluent-1.4.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1227 2024-02-16 12:57:48.482117 effluent-1.4.1/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-16 12:57:48.478117 effluent-1.4.1/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-16 12:57:48.478117 effluent-1.4.1/src/effluent/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      205 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3532 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/eos.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20732 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4994 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2287 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/numerics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6606 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/roms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/script.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9082 2024-02-16 12:57:35.000000 effluent-1.4.1/src/effluent/solver.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-16 12:57:48.478117 effluent-1.4.1/src/effluent.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3518 2024-02-16 12:57:48.000000 effluent-1.4.1/src/effluent.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-16 12:57:48.000000 effluent-1.4.1/src/effluent.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-16 12:57:48.000000 effluent-1.4.1/src/effluent.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-02-16 12:57:48.000000 effluent-1.4.1/src/effluent.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2024-02-16 12:57:48.000000 effluent-1.4.1/src/effluent.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2024-02-16 12:57:48.000000 effluent-1.4.1/src/effluent.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-16 12:57:48.478117 effluent-1.4.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-02-16 12:57:35.000000 effluent-1.4.1/tests/test_eos.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2727 2024-02-16 12:57:35.000000 effluent-1.4.1/tests/test_examples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14188 2024-02-16 12:57:35.000000 effluent-1.4.1/tests/test_io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1060 2024-02-16 12:57:35.000000 effluent-1.4.1/tests/test_numerics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2282 2024-02-16 12:57:35.000000 effluent-1.4.1/tests/test_roms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7844 2024-02-16 12:57:35.000000 effluent-1.4.1/tests/test_solver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-10 05:59:26.806170 effluent-1.4.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2024-05-10 05:59:17.000000 effluent-1.4.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3518 2024-05-10 05:59:26.806170 effluent-1.4.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2365 2024-05-10 05:59:17.000000 effluent-1.4.2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-05-10 05:59:17.000000 effluent-1.4.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1227 2024-05-10 05:59:26.806170 effluent-1.4.2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-10 05:59:26.802170 effluent-1.4.2/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-10 05:59:26.806170 effluent-1.4.2/src/effluent/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      205 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3532 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/eos.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20733 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4952 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2287 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/numerics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6606 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/roms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/script.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9082 2024-05-10 05:59:17.000000 effluent-1.4.2/src/effluent/solver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-10 05:59:26.806170 effluent-1.4.2/src/effluent.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3518 2024-05-10 05:59:26.000000 effluent-1.4.2/src/effluent.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-05-10 05:59:26.000000 effluent-1.4.2/src/effluent.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-10 05:59:26.000000 effluent-1.4.2/src/effluent.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-10 05:59:26.000000 effluent-1.4.2/src/effluent.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2024-05-10 05:59:26.000000 effluent-1.4.2/src/effluent.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2024-05-10 05:59:26.000000 effluent-1.4.2/src/effluent.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-10 05:59:26.806170 effluent-1.4.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-05-10 05:59:17.000000 effluent-1.4.2/tests/test_eos.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2727 2024-05-10 05:59:17.000000 effluent-1.4.2/tests/test_examples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14188 2024-05-10 05:59:17.000000 effluent-1.4.2/tests/test_io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1060 2024-05-10 05:59:17.000000 effluent-1.4.2/tests/test_numerics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2282 2024-05-10 05:59:17.000000 effluent-1.4.2/tests/test_roms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7844 2024-05-10 05:59:17.000000 effluent-1.4.2/tests/test_solver.py
```

### Comparing `effluent-1.4.1/LICENSE` & `effluent-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/PKG-INFO` & `effluent-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effluent
-Version: 1.4.1
+Version: 1.4.2
 Summary: Simulate effluent discharges from wastewater pipes
 Home-page: https://github.com/pnsaevik/effluent
 Author: Pål Næverlid Sævik
 Author-email: paal.naeverlid.saevik@hi.no
 Project-URL: Documentation, https://effluent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/pnsaevik/effluent/blob/main/CHANGELOG.md
 Keywords: pipes turbulent jets plumes ocean
```

### Comparing `effluent-1.4.1/README.md` & `effluent-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/setup.cfg` & `effluent-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/src/effluent/eos.py` & `effluent-1.4.2/src/effluent/eos.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/src/effluent/io.py` & `effluent-1.4.2/src/effluent/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         file,
         sep=',',
         header=0,
         skipinitialspace=True,
         skip_blank_lines=True,
         comment='#',
         converters=dict(time=np.datetime64),
+
     )
 
 
 class Ambient:
     """
     Data about the ambient ocean.
```

### Comparing `effluent-1.4.1/src/effluent/model.py` & `effluent-1.4.2/src/effluent/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 """
 
 import numpy as np
 import logging
 import tomli as toml
 import effluent.io
 import effluent.solver
-import effluent.io
-import effluent.solver
 import xarray as xr
 
 logger = logging.getLogger(__name__)
 
 
 class Model:
```

### Comparing `effluent-1.4.1/src/effluent/numerics.py` & `effluent-1.4.2/src/effluent/numerics.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/src/effluent/roms.py` & `effluent-1.4.2/src/effluent/roms.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/src/effluent/script.py` & `effluent-1.4.2/src/effluent/script.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/src/effluent/solver.py` & `effluent-1.4.2/src/effluent/solver.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/src/effluent.egg-info/PKG-INFO` & `effluent-1.4.2/src/effluent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effluent
-Version: 1.4.1
+Version: 1.4.2
 Summary: Simulate effluent discharges from wastewater pipes
 Home-page: https://github.com/pnsaevik/effluent
 Author: Pål Næverlid Sævik
 Author-email: paal.naeverlid.saevik@hi.no
 Project-URL: Documentation, https://effluent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/pnsaevik/effluent/blob/main/CHANGELOG.md
 Keywords: pipes turbulent jets plumes ocean
```

### Comparing `effluent-1.4.1/src/effluent.egg-info/SOURCES.txt` & `effluent-1.4.2/src/effluent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/tests/test_eos.py` & `effluent-1.4.2/tests/test_eos.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/tests/test_examples.py` & `effluent-1.4.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/tests/test_io.py` & `effluent-1.4.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/tests/test_numerics.py` & `effluent-1.4.2/tests/test_numerics.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/tests/test_roms.py` & `effluent-1.4.2/tests/test_roms.py`

 * *Files identical despite different names*

### Comparing `effluent-1.4.1/tests/test_solver.py` & `effluent-1.4.2/tests/test_solver.py`

 * *Files identical despite different names*

