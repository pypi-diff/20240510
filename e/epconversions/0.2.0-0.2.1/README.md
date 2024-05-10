# Comparing `tmp/epconversions-0.2.0.tar.gz` & `tmp/epconversions-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epconversions-0.2.0.tar", last modified: Thu Nov  2 17:26:45 2023, max compression
+gzip compressed data, was "epconversions-0.2.1.tar", last modified: Fri May 10 16:45:00 2024, max compression
```

## Comparing `epconversions-0.2.0.tar` & `epconversions-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2023-11-02 17:26:45.764824 epconversions-0.2.0/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      159 2023-10-31 00:59:32.000000 epconversions-0.2.0/AUTHORS.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1307 2023-10-31 00:59:32.000000 epconversions-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)       89 2023-10-31 00:59:32.000000 epconversions-0.2.0/HISTORY.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)    16725 2023-10-31 00:59:32.000000 epconversions-0.2.0/LICENSE
--rw-r--r--   0 santoshphilip   (501) staff       (20)      262 2023-10-31 00:59:32.000000 epconversions-0.2.0/MANIFEST.in
--rw-r--r--   0 santoshphilip   (501) staff       (20)     4911 2023-11-02 17:26:45.764914 epconversions-0.2.0/PKG-INFO
--rw-r--r--   0 santoshphilip   (501) staff       (20)     4040 2023-11-02 17:26:24.000000 epconversions-0.2.0/README.rst
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2023-11-02 17:26:45.762740 epconversions-0.2.0/docs/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      614 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/Makefile
--rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/authors.rst
--rwxr-xr-x   0 santoshphilip   (501) staff       (20)     4986 2023-11-02 17:26:24.000000 epconversions-0.2.0/docs/conf.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)       33 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/contributing.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      355 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/epconversions.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/history.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      313 2023-11-02 17:26:24.000000 epconversions-0.2.0/docs/index.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1178 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/installation.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      811 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/make.bat
--rw-r--r--   0 santoshphilip   (501) staff       (20)       76 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/modules.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)       27 2023-10-31 00:59:32.000000 epconversions-0.2.0/docs/readme.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1394 2023-11-02 17:26:24.000000 epconversions-0.2.0/docs/usage.rst
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2023-11-02 17:26:45.763154 epconversions-0.2.0/epconversions/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      134 2023-11-02 17:26:24.000000 epconversions-0.2.0/epconversions/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)    38050 2023-11-02 17:26:24.000000 epconversions-0.2.0/epconversions/epconversions.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2023-11-02 17:26:45.764078 epconversions-0.2.0/epconversions.egg-info/
--rw-r--r--   0 santoshphilip   (501) staff       (20)     4911 2023-11-02 17:26:45.000000 epconversions-0.2.0/epconversions.egg-info/PKG-INFO
--rw-r--r--   0 santoshphilip   (501) staff       (20)      582 2023-11-02 17:26:45.000000 epconversions-0.2.0/epconversions.egg-info/SOURCES.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2023-11-02 17:26:45.000000 epconversions-0.2.0/epconversions.egg-info/dependency_links.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2023-11-02 17:26:45.000000 epconversions-0.2.0/epconversions.egg-info/not-zip-safe
--rw-r--r--   0 santoshphilip   (501) staff       (20)       14 2023-11-02 17:26:45.000000 epconversions-0.2.0/epconversions.egg-info/top_level.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)      428 2023-11-02 17:26:45.765219 epconversions-0.2.0/setup.cfg
--rwxr-xr-x   0 santoshphilip   (501) staff       (20)     1359 2023-11-02 17:26:24.000000 epconversions-0.2.0/setup.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2023-11-02 17:26:45.764551 epconversions-0.2.0/tests/
--rw-r--r--   0 santoshphilip   (501) staff       (20)       43 2023-10-31 00:59:32.000000 epconversions-0.2.0/tests/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)    20946 2023-11-02 17:26:24.000000 epconversions-0.2.0/tests/test_epconversions.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.889674 epconversions-0.2.1/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      159 2023-10-28 22:26:04.000000 epconversions-0.2.1/AUTHORS.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1307 2023-10-31 21:07:15.000000 epconversions-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      257 2024-05-10 16:44:22.000000 epconversions-0.2.1/HISTORY.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    16725 2023-10-28 22:40:28.000000 epconversions-0.2.1/LICENSE
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      262 2023-10-28 22:26:04.000000 epconversions-0.2.1/MANIFEST.in
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     5079 2024-05-10 16:45:00.889816 epconversions-0.2.1/PKG-INFO
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     4040 2023-11-02 16:39:14.000000 epconversions-0.2.1/README.rst
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.885993 epconversions-0.2.1/docs/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      614 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/Makefile
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.879892 epconversions-0.2.1/docs/_build/
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.879966 epconversions-0.2.1/docs/_build/html/
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.886935 epconversions-0.2.1/docs/_build/html/_static/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      286 2023-10-28 22:37:04.000000 epconversions-0.2.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       90 2023-10-28 22:37:04.000000 epconversions-0.2.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       90 2023-10-28 22:37:04.000000 epconversions-0.2.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/authors.rst
+-rwxr-xr-x   0 santoshphilip   (501) staff       (20)     4986 2023-11-02 17:04:04.000000 epconversions-0.2.1/docs/conf.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       33 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/contributing.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      355 2023-11-02 17:09:16.000000 epconversions-0.2.1/docs/epconversions.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/history.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      313 2023-11-01 18:58:46.000000 epconversions-0.2.1/docs/index.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1178 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/installation.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      811 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/make.bat
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       76 2023-11-02 17:09:16.000000 epconversions-0.2.1/docs/modules.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       27 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/readme.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1394 2023-11-02 16:42:00.000000 epconversions-0.2.1/docs/usage.rst
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.887379 epconversions-0.2.1/epconversions/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      134 2024-05-10 16:44:22.000000 epconversions-0.2.1/epconversions/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    38143 2024-05-10 05:41:36.000000 epconversions-0.2.1/epconversions/epconversions.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.888794 epconversions-0.2.1/epconversions.egg-info/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     5079 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/PKG-INFO
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      685 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/SOURCES.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/dependency_links.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/not-zip-safe
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       14 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/top_level.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      428 2024-05-10 16:45:00.890120 epconversions-0.2.1/setup.cfg
+-rwxr-xr-x   0 santoshphilip   (501) staff       (20)     1359 2024-05-10 16:44:22.000000 epconversions-0.2.1/setup.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.889286 epconversions-0.2.1/tests/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       43 2023-10-28 22:15:52.000000 epconversions-0.2.1/tests/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    21368 2024-05-10 05:41:59.000000 epconversions-0.2.1/tests/test_epconversions.py
```

### Comparing `epconversions-0.2.0/CONTRIBUTING.rst` & `epconversions-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/LICENSE` & `epconversions-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/PKG-INFO` & `epconversions-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epconversions
-Version: 0.2.0
+Version: 0.2.1
 Summary: Unit conversions for E+
 Home-page: https://github.com/pyenergyplus/epconversions
 Author: Santosh Philip
 Author-email: santosh@noemail.com
 License: MIT license
 Keywords: epconversions
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -170,11 +170,22 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+
+
+2024-05-10
+----------
+
+fixed issue #16
+
+:Problem: convert2ip and convert2si do not convert strings to floats
+:Solution: strings are converted to floats if possible
+
+
 0.1.0 (2023-10-28)
 ------------------
 
 * First release on PyPI.
```

### Comparing `epconversions-0.2.0/README.rst` & `epconversions-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/docs/Makefile` & `epconversions-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/docs/conf.py` & `epconversions-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/docs/installation.rst` & `epconversions-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/docs/make.bat` & `epconversions-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/docs/usage.rst` & `epconversions-0.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.0/epconversions/epconversions.py` & `epconversions-0.2.1/epconversions/epconversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Santosh Philip
+# Copyright (c) 2023-2024 Santosh Philip
 # =======================================================================
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 
 """Conversion functions for EnergyPlus"""
@@ -997,14 +997,18 @@
     """does the conversions
 
     :param val: val is converted
     :param conv: this is the conversion factor or rule
     :param reverse: if True, use 1/conv or reverse of the rule
     :returns new_value: the converted value
     """
+    try:
+        val = float(val)
+    except (ValueError, TypeError) as e:
+        pass
     if reverse:
         try:
             conv = 1 / conv  # type: ignore
         except TypeError:
             pass
     try:
         if conv == ["1.8", "(plus", "32)"]:
```

### Comparing `epconversions-0.2.0/epconversions.egg-info/PKG-INFO` & `epconversions-0.2.1/epconversions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epconversions
-Version: 0.2.0
+Version: 0.2.1
 Summary: Unit conversions for E+
 Home-page: https://github.com/pyenergyplus/epconversions
 Author: Santosh Philip
 Author-email: santosh@noemail.com
 License: MIT license
 Keywords: epconversions
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -170,11 +170,22 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+
+
+2024-05-10
+----------
+
+fixed issue #16
+
+:Problem: convert2ip and convert2si do not convert strings to floats
+:Solution: strings are converted to floats if possible
+
+
 0.1.0 (2023-10-28)
 ------------------
 
 * First release on PyPI.
```

### Comparing `epconversions-0.2.0/setup.py` & `epconversions-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="epconversions",
     name="epconversions",
     packages=find_packages(include=["epconversions", "epconversions.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/pyenergyplus/epconversions",
-    version="0.2.0",
+    version="0.2.1",
     zip_safe=False,
 )
```

### Comparing `epconversions-0.2.0/tests/test_epconversions.py` & `epconversions-0.2.1/tests/test_epconversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Santosh Philip
+# Copyright (c) 2023-2024 Santosh Philip
 # =======================================================================
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 """pytest for epconversions"""
 import pytest
@@ -118,14 +118,22 @@
             None,
             True,
             None,
             (30, "unknown"),
         ),  # val, siunit, ipunit, unitstr, wrapin, expected
         # unitstr=True, wrapin='[X]'
         (
+            "3",
+            "m",
+            None,
+            True,
+            "[X]",
+            (3 * 3.28083989501312, "[ft]"),
+        ),  # val, siunit, ipunit, unitstr, wrapin, expected
+        (
             3,
             "m",
             None,
             True,
             "[X]",
             (3 * 3.28083989501312, "[ft]"),
         ),  # val, siunit, ipunit, unitstr, wrapin, expected
@@ -258,14 +266,22 @@
             "ft",
             None,
             True,
             "[X]",
             ("autocalculate", "[m]"),
         ),  # val, ipunit, siunit, unitstr, wrapin, expected
         (
+            "3",
+            "lb/MWh",
+            "g/MJ",
+            True,
+            "[X]",
+            (3 / 7.93664091373665, "[g/MJ]"),
+        ),  # val, ipunit, siunit, unitstr, wrapin, expected
+        (
             3,
             "lb/MWh",
             "g/MJ",
             True,
             "[X]",
             (3 / 7.93664091373665, "[g/MJ]"),
         ),  # val, ipunit, siunit, unitstr, wrapin, expected
```

