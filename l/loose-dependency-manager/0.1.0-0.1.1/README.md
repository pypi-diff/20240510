# Comparing `tmp/loose_dependency_manager-0.1.0.tar.gz` & `tmp/loose_dependency_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loose_dependency_manager-0.1.0.tar", max compression
+gzip compressed data, was "loose_dependency_manager-0.1.1.tar", max compression
```

## Comparing `loose_dependency_manager-0.1.0.tar` & `loose_dependency_manager-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1056 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/LICENSE
--rw-r--r--   0        0        0     2170 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/__init__.py
--rw-r--r--   0        0        0       59 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/__main__.py
--rw-r--r--   0        0        0        0 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/__init__.py
--rw-r--r--   0        0        0      190 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/config/__init__.py
--rw-r--r--   0        0        0      335 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/config/_dependency.py
--rw-r--r--   0        0        0      757 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/config/_installer.py
--rw-r--r--   0        0        0      215 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/config/_scheme.py
--rw-r--r--   0        0        0      175 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/factory/__init__.py
--rw-r--r--   0        0        0      250 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/factory/_factory.py
--rw-r--r--   0        0        0     1280 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/factory/_github.py
--rw-r--r--   0        0        0      678 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/factory/_http.py
--rw-r--r--   0        0        0      103 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/factory/_https.py
--rw-r--r--   0        0        0       92 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/__init__.py
--rw-r--r--   0        0        0      365 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/_dependency.py
--rw-r--r--   0        0        0     2842 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/_installer.py
--rw-r--r--   0        0        0      204 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/strategy/__init__.py
--rw-r--r--   0        0        0      632 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/strategy/_create.py
--rw-r--r--   0        0        0      943 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/strategy/_parallel.py
--rw-r--r--   0        0        0      447 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/strategy/_sequential.py
--rw-r--r--   0        0        0      549 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/installer/strategy/_strategy.py
--rw-r--r--   0        0        0      192 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/parse.py
--rw-r--r--   0        0        0      114 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/scheme/__init__.py
--rw-r--r--   0        0        0     1037 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/scheme/_github.py
--rw-r--r--   0        0        0     1022 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/scheme/_http.py
--rw-r--r--   0        0        0      401 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/api/scheme/_scheme.py
--rw-r--r--   0        0        0      342 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/cli.py
--rw-r--r--   0        0        0       89 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/commands/__init__.py
--rw-r--r--   0        0        0      362 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/commands/_command.py
--rw-r--r--   0        0        0      686 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/commands/_install.py
--rw-r--r--   0        0        0      202 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/component.py
--rw-r--r--   0        0        0      126 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/logger/__init__.py
--rw-r--r--   0        0        0     1304 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/logger/_click_logger.py
--rw-r--r--   0        0        0      831 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/logger/_logger.py
--rw-r--r--   0        0        0      428 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/logger/_noop_logger.py
--rw-r--r--   0        0        0        0 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/utils/__init__.py
--rw-r--r--   0        0        0       64 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/utils/mapping/__init__.py
--rw-r--r--   0        0        0      620 2024-05-09 17:53:25.841286 loose_dependency_manager-0.1.0/ldm/utils/mapping/_subscriptable.py
--rw-r--r--   0        0        0     1862 2024-05-09 17:53:25.845286 loose_dependency_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3593 1970-01-01 00:00:00.000000 loose_dependency_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2170 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/config/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/config/_dependency.py
+-rw-r--r--   0        0        0      757 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/config/_installer.py
+-rw-r--r--   0        0        0      215 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/config/_scheme.py
+-rw-r--r--   0        0        0      175 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/factory/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/factory/_factory.py
+-rw-r--r--   0        0        0     1280 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/factory/_github.py
+-rw-r--r--   0        0        0      678 2024-05-09 18:31:25.786013 loose_dependency_manager-0.1.1/ldm/api/factory/_http.py
+-rw-r--r--   0        0        0      103 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/factory/_https.py
+-rw-r--r--   0        0        0       92 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/_dependency.py
+-rw-r--r--   0        0        0     2842 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/_installer.py
+-rw-r--r--   0        0        0      204 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/strategy/__init__.py
+-rw-r--r--   0        0        0      632 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/strategy/_create.py
+-rw-r--r--   0        0        0      943 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/strategy/_parallel.py
+-rw-r--r--   0        0        0      447 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/strategy/_sequential.py
+-rw-r--r--   0        0        0      549 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/installer/strategy/_strategy.py
+-rw-r--r--   0        0        0      192 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/parse.py
+-rw-r--r--   0        0        0      114 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/scheme/__init__.py
+-rw-r--r--   0        0        0     1037 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/scheme/_github.py
+-rw-r--r--   0        0        0     1022 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/scheme/_http.py
+-rw-r--r--   0        0        0      401 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/api/scheme/_scheme.py
+-rw-r--r--   0        0        0      423 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/cli.py
+-rw-r--r--   0        0        0       89 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/commands/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/commands/_command.py
+-rw-r--r--   0        0        0      686 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/commands/_install.py
+-rw-r--r--   0        0        0      202 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/component.py
+-rw-r--r--   0        0        0      126 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/logger/__init__.py
+-rw-r--r--   0        0        0     1304 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/logger/_click_logger.py
+-rw-r--r--   0        0        0      831 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/logger/_logger.py
+-rw-r--r--   0        0        0      428 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/logger/_noop_logger.py
+-rw-r--r--   0        0        0        0 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/utils/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/utils/mapping/__init__.py
+-rw-r--r--   0        0        0      620 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/ldm/utils/mapping/_subscriptable.py
+-rw-r--r--   0        0        0     1862 2024-05-09 18:31:25.790013 loose_dependency_manager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3593 1970-01-01 00:00:00.000000 loose_dependency_manager-0.1.1/PKG-INFO
```

### Comparing `loose_dependency_manager-0.1.0/LICENSE` & `loose_dependency_manager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/README.md` & `loose_dependency_manager-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/config/_installer.py` & `loose_dependency_manager-0.1.1/ldm/api/config/_installer.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/factory/_github.py` & `loose_dependency_manager-0.1.1/ldm/api/factory/_github.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/factory/_http.py` & `loose_dependency_manager-0.1.1/ldm/api/factory/_http.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/installer/_installer.py` & `loose_dependency_manager-0.1.1/ldm/api/installer/_installer.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/installer/strategy/_create.py` & `loose_dependency_manager-0.1.1/ldm/api/installer/strategy/_create.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/installer/strategy/_parallel.py` & `loose_dependency_manager-0.1.1/ldm/api/installer/strategy/_parallel.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/installer/strategy/_strategy.py` & `loose_dependency_manager-0.1.1/ldm/api/installer/strategy/_strategy.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/scheme/_github.py` & `loose_dependency_manager-0.1.1/ldm/api/scheme/_github.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/api/scheme/_http.py` & `loose_dependency_manager-0.1.1/ldm/api/scheme/_http.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/commands/_install.py` & `loose_dependency_manager-0.1.1/ldm/commands/_install.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/logger/_click_logger.py` & `loose_dependency_manager-0.1.1/ldm/logger/_click_logger.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/logger/_logger.py` & `loose_dependency_manager-0.1.1/ldm/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/ldm/utils/mapping/_subscriptable.py` & `loose_dependency_manager-0.1.1/ldm/utils/mapping/_subscriptable.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.1.0/pyproject.toml` & `loose_dependency_manager-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loose-dependency-manager"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tool for managing code dependencies in a loosely-coupled way."
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
   'Natural Language :: English',
   'Topic :: Software Development',
   'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `loose_dependency_manager-0.1.0/PKG-INFO` & `loose_dependency_manager-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loose-dependency-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool for managing code dependencies in a loosely-coupled way.
 License: MIT
 Author: 01Joseph-Hwang10
 Author-email: joseph95501@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

