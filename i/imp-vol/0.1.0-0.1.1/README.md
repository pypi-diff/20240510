# Comparing `tmp/imp_vol-0.1.0.tar.gz` & `tmp/imp_vol-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imp_vol-0.1.0.tar", last modified: Tue Apr 23 07:23:47 2024, max compression
+gzip compressed data, was "imp_vol-0.1.1.tar", last modified: Fri May 10 02:03:37 2024, max compression
```

## Comparing `imp_vol-0.1.0.tar` & `imp_vol-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        0 2024-04-23 07:23:47.865637 imp_vol-0.1.0/
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)     1074 2024-04-23 04:27:45.000000 imp_vol-0.1.0/LICENSE
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      981 2024-04-23 07:23:47.864346 imp_vol-0.1.0/PKG-INFO
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      342 2024-04-23 04:27:45.000000 imp_vol-0.1.0/README.rst
-drwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        0 2024-04-23 07:23:47.820243 imp_vol-0.1.0/imp_vol/
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)     1399 2024-04-23 07:22:43.000000 imp_vol-0.1.0/imp_vol/__init__.py
-drwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        0 2024-04-23 07:23:47.858618 imp_vol-0.1.0/imp_vol.egg-info/
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      981 2024-04-23 07:23:47.000000 imp_vol-0.1.0/imp_vol.egg-info/PKG-INFO
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      218 2024-04-23 07:23:47.000000 imp_vol-0.1.0/imp_vol.egg-info/SOURCES.txt
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        1 2024-04-23 07:23:47.000000 imp_vol-0.1.0/imp_vol.egg-info/dependency_links.txt
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)       42 2024-04-23 07:23:47.000000 imp_vol-0.1.0/imp_vol.egg-info/requires.txt
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        8 2024-04-23 07:23:47.000000 imp_vol-0.1.0/imp_vol.egg-info/top_level.txt
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)       42 2024-04-23 04:27:45.000000 imp_vol-0.1.0/requirements.txt
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)       38 2024-04-23 07:23:47.866995 imp_vol-0.1.0/setup.cfg
--rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)     1397 2024-04-23 04:27:45.000000 imp_vol-0.1.0/setup.py
+drwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        0 2024-05-10 02:03:37.754452 imp_vol-0.1.1/
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)     1074 2024-04-23 04:27:45.000000 imp_vol-0.1.1/LICENSE
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      981 2024-05-10 02:03:37.752439 imp_vol-0.1.1/PKG-INFO
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      342 2024-04-23 04:27:45.000000 imp_vol-0.1.1/README.rst
+drwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        0 2024-05-10 02:03:37.717629 imp_vol-0.1.1/imp_vol/
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)     1571 2024-05-10 02:01:49.000000 imp_vol-0.1.1/imp_vol/__init__.py
+drwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        0 2024-05-10 02:03:37.747444 imp_vol-0.1.1/imp_vol.egg-info/
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      981 2024-05-10 02:03:37.000000 imp_vol-0.1.1/imp_vol.egg-info/PKG-INFO
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)      218 2024-05-10 02:03:37.000000 imp_vol-0.1.1/imp_vol.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        1 2024-05-10 02:03:37.000000 imp_vol-0.1.1/imp_vol.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)       42 2024-05-10 02:03:37.000000 imp_vol-0.1.1/imp_vol.egg-info/requires.txt
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)        8 2024-05-10 02:03:37.000000 imp_vol-0.1.1/imp_vol.egg-info/top_level.txt
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)       42 2024-04-23 04:27:45.000000 imp_vol-0.1.1/requirements.txt
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)       38 2024-05-10 02:03:37.755663 imp_vol-0.1.1/setup.cfg
+-rwxrwxrwx   0 zenbook   (1000) zenbook   (1000)     1397 2024-05-10 02:03:20.000000 imp_vol-0.1.1/setup.py
```

### Comparing `imp_vol-0.1.0/LICENSE` & `imp_vol-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imp_vol-0.1.0/PKG-INFO` & `imp_vol-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp_vol
-Version: 0.1.0
+Version: 0.1.1
 Home-page: 
 Author: fx-kirin
 Author-email: fx.kirin@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `imp_vol-0.1.0/imp_vol/__init__.py` & `imp_vol-0.1.1/imp_vol/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """imp_vol - """
 import types
 
 import numpy as np
 from scipy.optimize import fsolve
 from scipy.stats import norm
+import scipy
 
 __version__ = "0.1.0"
 __author__ = "fx-kirin <fx.kirin@gmail.com>"
 __all__: list = ["call", "put", "implied_volatility", "OptionCall", "OptionPut"]
 
 
 CONSTS = types.SimpleNamespace()
@@ -33,20 +34,27 @@
     d_1 = (1 / (sigma * (np.sqrt(T)))) * (np.log(S / K) + (r + sigma**2 / 2) * (T))
     d_2 = d_1 - sigma * np.sqrt(T)
     put = norm.cdf(-d_2) * K * np.exp(-r * (T)) - norm.cdf(-d_1) * S
     return put
 
 
 def implied_volatility(S, K, r, T, price, initial_val, option_type: int):
+    """
+        S: 現在の株価
+        K: 権利行使価格
+    """
     match option_type:
         case CONSTS.OptionCall:
             func = call
         case CONSTS.OptionPut:
             func = put
         case _:
             raise RuntimeError(f"{option_type=} is not allowed.")
 
     def isolate_sigma(sigma):
         return func(S, K, r, T, sigma) - price
 
-    iv = fsolve(isolate_sigma, initial_val)[0]
+    result = fsolve(isolate_sigma, initial_val, full_output=True)
+    if result[2] != 1:
+        return np.nan
+    iv = result[0][0]
     return iv
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imp_vol-0.1.0/imp_vol.egg-info/PKG-INFO` & `imp_vol-0.1.1/imp_vol.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp-vol
-Version: 0.1.0
+Version: 0.1.1
 Home-page: 
 Author: fx-kirin
 Author-email: fx.kirin@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `imp_vol-0.1.0/setup.py` & `imp_vol-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         required = []
 
     return required
 
 
 setup(
     name="imp_vol",
-    version="0.1.0",
+    version="0.1.1",
     url="",
     license="MIT",
     author="fx-kirin",
     author_email="fx.kirin@gmail.com",
     description="",
     long_description=read("README.rst"),
     packages=find_packages(exclude=("tests",)),
```

