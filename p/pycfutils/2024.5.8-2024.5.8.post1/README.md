# Comparing `tmp/pycfutils-2024.5.8.tar.gz` & `tmp/pycfutils-2024.5.8.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycfutils-2024.5.8.tar", last modified: Wed May  8 01:14:56 2024, max compression
+gzip compressed data, was "pycfutils-2024.5.8.post1.tar", last modified: Wed May  8 08:09:41 2024, max compression
```

## Comparing `pycfutils-2024.5.8.tar` & `pycfutils-2024.5.8.post1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.799760 pycfutils-2024.5.8/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1073 2024-05-07 19:43:39.000000 pycfutils-2024.5.8/LICENSE
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1500 2024-05-08 01:14:56.795742 pycfutils-2024.5.8/PKG-INFO
--rw-r--r--   0 cfati     (1000) cfati     (1000)      535 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/README.md
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.412886 pycfutils-2024.5.8/pycfutils/
--rw-r--r--   0 cfati     (1000) cfati     (1000)       76 2024-05-07 23:18:00.000000 pycfutils-2024.5.8/pycfutils/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1615 2024-05-07 17:48:58.000000 pycfutils-2024.5.8/pycfutils/common.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3033 2024-05-07 20:10:54.000000 pycfutils-2024.5.8/pycfutils/ctypes.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.542884 pycfutils-2024.5.8/pycfutils/gui/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1376 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/gui/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2052 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/gui/constants.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.281890 pycfutils-2024.5.8/pycfutils/include/
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.747972 pycfutils-2024.5.8/pycfutils/include/pycfutils/
--rw-r--r--   0 cfati     (1000) cfati     (1000)      921 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/include/pycfutils/cinterface.h
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     2291 2024-05-07 17:48:58.000000 pycfutils-2024.5.8/pycfutils/keyboard.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.773740 pycfutils-2024.5.8/pycfutils/src/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3553 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/src/cinterface_win.cpp
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.662208 pycfutils-2024.5.8/pycfutils/tests/
--rw-r--r--   0 cfati     (1000) cfati     (1000)       76 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/tests/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2583 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/tests/test_common.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      809 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/tests/test_ctypes.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      403 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/tests/test_gui.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      382 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/pycfutils/tests/test_keyboard.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.494884 pycfutils-2024.5.8/pycfutils.egg-info/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1500 2024-05-08 01:14:56.000000 pycfutils-2024.5.8/pycfutils.egg-info/PKG-INFO
--rw-r--r--   0 cfati     (1000) cfati     (1000)      567 2024-05-08 01:14:56.000000 pycfutils-2024.5.8/pycfutils.egg-info/SOURCES.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)        1 2024-05-08 01:14:56.000000 pycfutils-2024.5.8/pycfutils.egg-info/dependency_links.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)       10 2024-05-08 01:14:56.000000 pycfutils-2024.5.8/pycfutils.egg-info/top_level.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)       38 2024-05-08 01:14:56.800743 pycfutils-2024.5.8/setup.cfg
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     4539 2024-05-08 01:06:57.000000 pycfutils-2024.5.8/setup.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 01:14:56.720463 pycfutils-2024.5.8/vs/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1423 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/vs/vs.sln
--rw-r--r--   0 cfati     (1000) cfati     (1000)     8443 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/vs/vs.vcxproj
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1161 2024-05-07 23:17:59.000000 pycfutils-2024.5.8/vs/vs.vcxproj.filters
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:41.282786 pycfutils-2024.5.8.post1/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1073 2024-05-07 19:43:39.000000 pycfutils-2024.5.8.post1/LICENSE
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1506 2024-05-08 08:09:41.274787 pycfutils-2024.5.8.post1/PKG-INFO
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      535 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/README.md
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:40.856483 pycfutils-2024.5.8.post1/pycfutils/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       76 2024-05-07 23:18:00.000000 pycfutils-2024.5.8.post1/pycfutils/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1615 2024-05-07 17:48:58.000000 pycfutils-2024.5.8.post1/pycfutils/common.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     3018 2024-05-08 08:01:05.000000 pycfutils-2024.5.8.post1/pycfutils/ctypes.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:40.988683 pycfutils-2024.5.8.post1/pycfutils/gui/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1376 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/gui/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2052 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/gui/constants.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:40.738738 pycfutils-2024.5.8.post1/pycfutils/include/
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:41.210787 pycfutils-2024.5.8.post1/pycfutils/include/pycfutils/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      921 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/include/pycfutils/cinterface.h
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     2291 2024-05-07 17:48:58.000000 pycfutils-2024.5.8.post1/pycfutils/keyboard.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:41.242786 pycfutils-2024.5.8.post1/pycfutils/src/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     3553 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/src/cinterface_win.cpp
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:41.110789 pycfutils-2024.5.8.post1/pycfutils/tests/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       76 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/tests/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2583 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/tests/test_common.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      809 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/tests/test_ctypes.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      403 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/tests/test_gui.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      382 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/pycfutils/tests/test_keyboard.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:40.935370 pycfutils-2024.5.8.post1/pycfutils.egg-info/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1506 2024-05-08 08:09:40.000000 pycfutils-2024.5.8.post1/pycfutils.egg-info/PKG-INFO
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      567 2024-05-08 08:09:40.000000 pycfutils-2024.5.8.post1/pycfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)        1 2024-05-08 08:09:40.000000 pycfutils-2024.5.8.post1/pycfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       10 2024-05-08 08:09:40.000000 pycfutils-2024.5.8.post1/pycfutils.egg-info/top_level.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       38 2024-05-08 08:09:41.283790 pycfutils-2024.5.8.post1/setup.cfg
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     4545 2024-05-08 08:03:29.000000 pycfutils-2024.5.8.post1/setup.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-08 08:09:41.177787 pycfutils-2024.5.8.post1/vs/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1423 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/vs/vs.sln
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     8443 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/vs/vs.vcxproj
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1161 2024-05-07 23:17:59.000000 pycfutils-2024.5.8.post1/vs/vs.vcxproj.filters
```

### Comparing `pycfutils-2024.5.8/LICENSE` & `pycfutils-2024.5.8.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/PKG-INFO` & `pycfutils-2024.5.8.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfutils
-Version: 2024.5.8
+Version: 2024.5.8.post1
 Summary: PyCFUtils (Cristi Fati's Utils for Python (&& more)) - a collection of (cool) scripts / utilities
 Home-page: https://github.com/CristiFati/pycfutils
 Download-URL: https://pypi.org/project/pycfutils
 Author: Cristi Fati
 Author-email: fati_utcluj@yahoo.com
 Maintainer: Cristi Fati
 Maintainer-email: fati_utcluj@yahoo.com
```

### Comparing `pycfutils-2024.5.8/README.md` & `pycfutils-2024.5.8.post1/README.md`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/common.py` & `pycfutils-2024.5.8.post1/pycfutils/common.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/ctypes.py` & `pycfutils-2024.5.8.post1/pycfutils/ctypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import ctypes as cts
 import sys
 from typing import Any, Optional
 
-cts.c_bool = 1
 try:
     _CLS_CDATA = cts.c_int.__mro__[-2]
 except Exception:
     _CLS_CDATA = None
 
 
 __all__ = ("to_string",)
```

### Comparing `pycfutils-2024.5.8/pycfutils/gui/__init__.py` & `pycfutils-2024.5.8.post1/pycfutils/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/gui/constants.py` & `pycfutils-2024.5.8.post1/pycfutils/gui/constants.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/include/pycfutils/cinterface.h` & `pycfutils-2024.5.8.post1/pycfutils/include/pycfutils/cinterface.h`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/keyboard.py` & `pycfutils-2024.5.8.post1/pycfutils/keyboard.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/src/cinterface_win.cpp` & `pycfutils-2024.5.8.post1/pycfutils/src/cinterface_win.cpp`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/tests/test_common.py` & `pycfutils-2024.5.8.post1/pycfutils/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils/tests/test_ctypes.py` & `pycfutils-2024.5.8.post1/pycfutils/tests/test_ctypes.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/pycfutils.egg-info/PKG-INFO` & `pycfutils-2024.5.8.post1/pycfutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfutils
-Version: 2024.5.8
+Version: 2024.5.8.post1
 Summary: PyCFUtils (Cristi Fati's Utils for Python (&& more)) - a collection of (cool) scripts / utilities
 Home-page: https://github.com/CristiFati/pycfutils
 Download-URL: https://pypi.org/project/pycfutils
 Author: Cristi Fati
 Author-email: fati_utcluj@yahoo.com
 Maintainer: Cristi Fati
 Maintainer-email: fati_utcluj@yahoo.com
```

### Comparing `pycfutils-2024.5.8/pycfutils.egg-info/SOURCES.txt` & `pycfutils-2024.5.8.post1/pycfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/setup.py` & `pycfutils-2024.5.8.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from setuptools.command.sdist import sdist
 from setuptools.extension import Library
 from wheel.bdist_wheel import bdist_wheel
 
 _IS_WIN = sys.platform[:3].lower() == "win"
 
 _NAME = "pycfutils"
-_VERSION = "2024.05.08"
+_VERSION = "2024.05.08.post1"
 
 if _IS_WIN:
     _EXT = ".dll"
     _SUF = "win"
 else:
     _EXT = ".so"
     _SUF = "nix"
```

### Comparing `pycfutils-2024.5.8/vs/vs.sln` & `pycfutils-2024.5.8.post1/vs/vs.sln`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/vs/vs.vcxproj` & `pycfutils-2024.5.8.post1/vs/vs.vcxproj`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.8/vs/vs.vcxproj.filters` & `pycfutils-2024.5.8.post1/vs/vs.vcxproj.filters`

 * *Files identical despite different names*

