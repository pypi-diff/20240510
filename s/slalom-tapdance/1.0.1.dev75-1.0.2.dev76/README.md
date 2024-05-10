# Comparing `tmp/slalom_tapdance-1.0.1.dev75.tar.gz` & `tmp/slalom_tapdance-1.0.2.dev76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev75.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.2.dev76.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev75.tar` & `slalom_tapdance-1.0.2.dev76.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-10 19:28:08.355472 slalom_tapdance-1.0.1.dev75/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/install_helper.py
--rw-r--r--   0        0        0    38838 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/states.py
--rw-r--r--   0        0        0    11998 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev75/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 19:32:28.992904 slalom_tapdance-1.0.2.dev76/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-10 19:32:44.120804 slalom_tapdance-1.0.2.dev76/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38838 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/states.py
+-rw-r--r--   0        0        0    11998 2024-05-10 19:32:28.996904 slalom_tapdance-1.0.2.dev76/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.2.dev76/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev75/LICENSE` & `slalom_tapdance-1.0.2.dev76/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/pyproject.toml` & `slalom_tapdance-1.0.2.dev76/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.75"
+version = "1.0.2-dev.76"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev75/tapdance/cli.py` & `slalom_tapdance-1.0.2.dev76/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/tapdance/config.py` & `slalom_tapdance-1.0.2.dev76/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/tapdance/docker.py` & `slalom_tapdance-1.0.2.dev76/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/tapdance/install_helper.py` & `slalom_tapdance-1.0.2.dev76/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/tapdance/plans.py` & `slalom_tapdance-1.0.2.dev76/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/tapdance/states.py` & `slalom_tapdance-1.0.2.dev76/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/tapdance/syncs.py` & `slalom_tapdance-1.0.2.dev76/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev75/PKG-INFO` & `slalom_tapdance-1.0.2.dev76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev75
+Version: 1.0.2.dev76
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

