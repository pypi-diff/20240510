# Comparing `tmp/eevalue-1.7.0.tar.gz` & `tmp/eevalue-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eevalue-1.7.0.tar", last modified: Tue Oct 18 12:59:25 2022, max compression
+gzip compressed data, was "eevalue-2.0.1.tar", last modified: Fri May 10 18:02:11 2024, max compression
```

## Comparing `eevalue-1.7.0.tar` & `eevalue-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:59:25.394998 eevalue-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-10-18 12:58:58.000000 eevalue-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-18 12:59:25.394998 eevalue-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-10-18 12:58:58.000000 eevalue-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-18 12:58:58.000000 eevalue-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-18 12:59:25.394998 eevalue-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:59:25.390998 eevalue-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:59:25.390998 eevalue-1.7.0/src/eevalue/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-18 12:58:58.000000 eevalue-1.7.0/src/eevalue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8340 2022-10-18 12:58:58.000000 eevalue-1.7.0/src/eevalue/eevalue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:59:25.394998 eevalue-1.7.0/src/eevalue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-18 12:59:25.000000 eevalue-1.7.0/src/eevalue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-18 12:59:25.000000 eevalue-1.7.0/src/eevalue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 12:59:25.000000 eevalue-1.7.0/src/eevalue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-18 12:59:25.000000 eevalue-1.7.0/src/eevalue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:02:11.496014 eevalue-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-10 18:02:00.000000 eevalue-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 18:02:11.496014 eevalue-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-10 18:02:00.000000 eevalue-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-10 18:02:00.000000 eevalue-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-10 18:02:11.496014 eevalue-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:02:11.496014 eevalue-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:02:11.496014 eevalue-2.0.1/src/eevalue/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 18:02:00.000000 eevalue-2.0.1/src/eevalue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-10 18:02:00.000000 eevalue-2.0.1/src/eevalue/eevalue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:02:11.496014 eevalue-2.0.1/src/eevalue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 18:02:11.000000 eevalue-2.0.1/src/eevalue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-10 18:02:11.000000 eevalue-2.0.1/src/eevalue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:02:11.000000 eevalue-2.0.1/src/eevalue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 18:02:11.000000 eevalue-2.0.1/src/eevalue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:02:11.496014 eevalue-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-10 18:02:00.000000 eevalue-2.0.1/tests/test_eevalue.py
```

### Comparing `eevalue-1.7.0/LICENSE` & `eevalue-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eevalue-1.7.0/PKG-INFO` & `eevalue-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eevalue
-Version: 1.7.0
+Version: 2.0.1
 Summary: A package that easily lets you find nearest E-series values and printing values with Si prefixes.
 Home-page: https://github.com/Duckle29/EEValue
 Author: Mikkel Jeppesen
 Author-email: mikkel+pypi@mikkel.cc
 Project-URL: Bug Tracker, https://github.com/Duckle29/EEvalue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `eevalue-1.7.0/README.md` & `eevalue-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `eevalue-1.7.0/setup.cfg` & `eevalue-2.0.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [yapf]
 column_limit = 127
 based_on_style = pep8
 
 [metadata]
 name = eevalue
-version = 1.7.0
+version = 2.0.1
 author = Mikkel Jeppesen
 author_email = mikkel+pypi@mikkel.cc
 description = A package that easily lets you find nearest E-series values and printing values with Si prefixes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Duckle29/EEValue
 project_urls =
```

### Comparing `eevalue-1.7.0/src/eevalue/eevalue.py` & `eevalue-2.0.1/src/eevalue/eevalue.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 from typing import Tuple, Iterable
 import re
 
 
 Si_prefixes = ('y', 'z', 'a', 'f', 'p', 'n', 'µ', 'm', '', 'k', 'M', 'G', 'T', 'P', 'E', 'Z', 'Y')
 
 
-def E_fwd(series: int, idx: int, legacy: bool = True) -> float:
+def E_fwd(series: int, idx: int, legacy: bool = True, round_base: bool = True) -> float:
     """ Returns the value for a given E-series at the given index
 
     Args:
         series (int): The E series to target
         idx (int): The index of the series to get the value of [0 to series-1]
         legacy (bool): If it should return the legacy values for the lower E-series
+        round_base (bool): If result should be rounded.
 
     Returns:
         float: E-series base value
     """
 
     E24_overrides = ((10, 11, 12, 13, 14, 15, 16, 22), (2.7, 3.0, 3.3, 3.6, 3.9, 4.3, 4.7, 8.2))
 
-    calculated_base = (10**idx)**(1 / series)  # The (range)th-root of 10^idx
+    calculated_base = (10 ** idx) ** (1.0 / series)  # The (range)th-root of 10^idx
 
-    if series in [3, 6, 12, 24]:
+    digits = 2
+
+    if series <= 24:
+        digits = 1
         e24_idx = idx * (24 / series)
         if e24_idx in E24_overrides[0] and legacy:
-            base = E24_overrides[1][E24_overrides[0].index(e24_idx)]
-            return base
+            calculated_base = E24_overrides[1][E24_overrides[0].index(e24_idx)]
 
-        calculated_base = round(calculated_base, 1)
-    else:
-        calculated_base = round(calculated_base, 2)
+    if round_base:
+        calculated_base = round(calculated_base, digits)
 
     return calculated_base
 
 
 def E_inv(series: int, val: float) -> float:
     """Returns the exact (continous) index for a given value on a given series.
 
@@ -137,63 +139,98 @@
 
 
 class EEValue(float):
     """ Class that provides EE friendly numbers
     Provides with automatic prefixing and standard value fitting
     """
 
-    def __new__(cls, value, precision=2):
+    def __new__(cls, value, precision=2, unit=''):
         if isinstance(value, str):
             value = eestr_to_float(value)
 
         new_cls = super(EEValue, EEValue).__new__(cls, value)
         new_cls.precision = precision
         new_cls.base, new_cls.exponent = get_base(float(value))
+        new_cls.unit = unit
         return new_cls
 
-    def E(cls, series: int = 96, mode: str = 'round', legacy: bool = True) -> 'EEValue':
+    def E(cls, series: int = 96, mode: str = 'round',
+          legacy: bool = True, give_error: bool = False) -> 'EEValue':
         """Get an E series value for the EEValue
 
         Args:
-            series (int, optional): The series to get the value from. Defaults to 96.
-            mode (str, optional): Which way to round. Can be: 'ceil', 'floor' or 'round'. Defaults to 'round'.
-            legacy (bool, optional): If you want to use the legacy substituations in E24 and lower ranges. Defaults to True.
+           series (int, optional): The series to get the value from. Defaults to 96.
+           mode (str, optional): Which way to round. Can be: 'ceil', 'floor' or 'round'. Defaults to 'round'.
+           legacy (bool, optional): If you want to use the legacy substituations in E24 and lower ranges. Defaults to True.
+           give_error (bool, optional): If you want to return the error from the original value as a factor. Defaults to False.
 
         Raises:
             ValueError: Raises if invalid mode is supplied
 
         Returns:
             EEValue: An EEValue of the desired E series value
         """
-        exponent = max(-8, min(cls.exponent, 8))
+        # exponent = max(-24, min(cls.exponent, 24))
+        exponent = cls.exponent
 
         idx = E_inv(series, cls.base)
+        calculated_base = E_fwd(series, idx, False, False)
 
         if mode == "round":
-            idx = round(idx)
-            if series in [3, 6, 12, 24]:
-                vals = (abs(cls.base - E_fwd(series, idx - 1, legacy)), abs(cls.base - E_fwd(series, idx, legacy)),
-                        abs(cls.base - E_fwd(series, idx + 1, legacy)))
-                idx += vals.index(min(vals)) - 1
+            val_distances = (
+                abs(cls.base - E_fwd(series, int(idx) - 1, legacy)),
+                abs(cls.base - E_fwd(series, int(idx), legacy)),
+                abs(cls.base - E_fwd(series, int(idx) + 1, legacy))
+            )
+            val_bases = (
+                E_fwd(series, int(idx) - 1, legacy),
+                E_fwd(series, int(idx), legacy),
+                E_fwd(series, int(idx) + 1, legacy)
+            )
+            base = val_bases[val_distances.index(min(val_distances))]
 
-        elif mode == "ceil":
-            idx = ceil(idx)
         elif mode == "floor":
-            idx = floor(idx)
+            base = E_fwd(series, floor(idx))
+            while base > calculated_base:
+                base = E_fwd(series, floor(idx))
+                idx -= 1
+                if idx < series * -1:
+                    raise ValueError("Runaway floor")
+
+        elif mode == "ceil":
+            base = E_fwd(series, floor(idx))
+            while base < calculated_base:
+                base = E_fwd(series, ceil(idx))
+                idx += 1
+                if idx > series:
+                    raise ValueError("Runaway ceil")
         else:
             raise ValueError('Mode has to be either "round", "ceil" or "floor". {} is not a valid mode'.format(mode))
 
-        return EEValue(E_fwd(series, idx, legacy) * 10**exponent)
+        res = EEValue(base * 10**exponent, precision=cls.precision, unit=cls.unit)
+
+        # Because E24 and lower series have some legacy values. This is necesary to ensure you get expected behaviour.
+        if mode == 'floor' and res > cls:
+            res = EEValue(E_fwd(series, idx-1, legacy) * 10**exponent, precision=cls.precision, unit=cls.unit)
+
+        if mode == 'ceil' and res < cls:
+            res = EEValue(E_fwd(series, idx+1, legacy) * 10**exponent, precision=cls.precision, unit=cls.unit)
+
+        if give_error:
+            error = res / cls
+            return error, res
+
+        return res
 
     def __str__(cls):
         exponent = max(-24, min(cls.exponent, 24))
         idx = exponent // 3 + 8
         prefix = Si_prefixes[idx]
         val = float(cls) / 10**((idx - 8) * 3)  # We do this to keep to 3 orders of magnitude
-        return "{:.{}f} {}".format(val, cls.precision, prefix)
+        return "{:.{}f} {}{}".format(val, cls.precision, prefix, cls.unit)
 
     def __repr__(cls):
         return "EEValue({})".format(float(cls))
 
     def re_wrap(self, A, B, res):
         precision = A.precision
         if B.__class__.__name__ == 'EEValue':
```

### Comparing `eevalue-1.7.0/src/eevalue.egg-info/PKG-INFO` & `eevalue-2.0.1/src/eevalue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eevalue
-Version: 1.7.0
+Version: 2.0.1
 Summary: A package that easily lets you find nearest E-series values and printing values with Si prefixes.
 Home-page: https://github.com/Duckle29/EEValue
 Author: Mikkel Jeppesen
 Author-email: mikkel+pypi@mikkel.cc
 Project-URL: Bug Tracker, https://github.com/Duckle29/EEvalue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

