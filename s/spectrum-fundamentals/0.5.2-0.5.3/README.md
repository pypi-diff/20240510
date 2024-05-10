# Comparing `tmp/spectrum_fundamentals-0.5.2.tar.gz` & `tmp/spectrum_fundamentals-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.5.2.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.5.3.tar", max compression
```

## Comparing `spectrum_fundamentals-0.5.2.tar` & `spectrum_fundamentals-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1102 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/LICENSE
--rw-r--r--   0        0        0     2611 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/README.rst
--rw-r--r--   0        0        0     2464 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      939 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0    20512 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1377 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0    12541 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    19686 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    34826 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1563 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    23723 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    26034 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0    17026 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-10 06:54:47.221579 spectrum_fundamentals-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2611 2024-05-10 06:54:47.221579 spectrum_fundamentals-0.5.3/README.rst
+-rw-r--r--   0        0        0     2464 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    20512 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1377 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0    12541 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    19686 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    34826 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1563 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    23723 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    26034 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0    17026 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2024-05-10 06:54:47.225579 spectrum_fundamentals-0.5.3/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.3/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.5.2/LICENSE` & `spectrum_fundamentals-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/README.rst` & `spectrum_fundamentals-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/pyproject.toml` & `spectrum_fundamentals-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.5.2"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.5.3"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamental functions, annotation pipeline and constants for oktoberfest"
 authors = ["Wilhelmlab at Technical University of Munich"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
```

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Initialize fundamentals."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/annotation/annotation.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/charge.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     304.2071: "[UNIMOD:2016]",
     144.1020: "[UNIMOD:214]",
     304.2053: "[UNIMOD:730]",
     8.0141: "[UNIMOD:259]",
     10.0082: "[UNIMOD:267]",
     79.9663: "[UNIMOD:21]",
     -18.0105: "[UNIMOD:23]",
-    57.0214: "[UNIMOD:4]",
+    57.0215: "[UNIMOD:4]",
     15.9949: "[UNIMOD:35]",
     42.0105: "[UNIMOD:1]",
 }
 # these are only used for prosit_grpc, oktoberfest uses the masses from MOD_MASSES
 AA_MOD_MASSES = {
     "K[UNIMOD:737]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:737]"],
     "M[UNIMOD:35]": AA_MASSES["M"] + MOD_MASSES["[UNIMOD:35]"],
```

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/fragments.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/percolator.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.5.3/spectrum_fundamentals/mod_string.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.2/PKG-INFO` & `spectrum_fundamentals-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_fundamentals
-Version: 0.5.2
+Version: 0.5.3
 Summary: Fundamental functions, annotation pipeline and constants for oktoberfest
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: Wilhelmlab at Technical University of Munich
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

