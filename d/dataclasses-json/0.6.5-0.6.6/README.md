# Comparing `tmp/dataclasses_json-0.6.5.tar.gz` & `tmp/dataclasses_json-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_json-0.6.5.tar", max compression
+gzip compressed data, was "dataclasses_json-0.6.6.tar", max compression
```

## Comparing `dataclasses_json-0.6.5.tar` & `dataclasses_json-0.6.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/LICENSE
--rw-r--r--   0        0        0    23874 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/README.md
--rw-r--r--   0        0        0      495 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/__init__.py
--rw-r--r--   0        0        0      154 2024-04-29 10:52:29.165597 dataclasses_json-0.6.5/dataclasses_json/__version__.py
--rw-r--r--   0        0        0     5990 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/api.py
--rw-r--r--   0        0        0     3527 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/cfg.py
--rw-r--r--   0        0        0    18719 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/core.py
--rw-r--r--   0        0        0    15997 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/mm.py
--rw-r--r--   0        0        0        0 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/py.typed
--rw-r--r--   0        0        0     3313 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/stringcase.py
--rw-r--r--   0        0        0    10452 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/undefined.py
--rw-r--r--   0        0        0     5852 2024-04-29 10:52:11.241776 dataclasses_json-0.6.5/dataclasses_json/utils.py
--rw-r--r--   0        0        0     1147 2024-04-29 10:52:29.161597 dataclasses_json-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    25035 1970-01-01 00:00:00.000000 dataclasses_json-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-10 10:41:34.968307 dataclasses_json-0.6.6/LICENSE
+-rw-r--r--   0        0        0    23874 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/README.md
+-rw-r--r--   0        0        0      495 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/__init__.py
+-rw-r--r--   0        0        0      154 2024-05-10 10:41:55.068642 dataclasses_json-0.6.6/dataclasses_json/__version__.py
+-rw-r--r--   0        0        0     5990 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/api.py
+-rw-r--r--   0        0        0     3527 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/cfg.py
+-rw-r--r--   0        0        0    18719 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/core.py
+-rw-r--r--   0        0        0    15997 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/mm.py
+-rw-r--r--   0        0        0        0 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/py.typed
+-rw-r--r--   0        0        0     3313 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/stringcase.py
+-rw-r--r--   0        0        0    10452 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/undefined.py
+-rw-r--r--   0        0        0     5852 2024-05-10 10:41:34.972307 dataclasses_json-0.6.6/dataclasses_json/utils.py
+-rw-r--r--   0        0        0     1147 2024-05-10 10:41:55.068642 dataclasses_json-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    25035 1970-01-01 00:00:00.000000 dataclasses_json-0.6.6/PKG-INFO
```

### Comparing `dataclasses_json-0.6.5/LICENSE` & `dataclasses_json-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/README.md` & `dataclasses_json-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/dataclasses_json/api.py` & `dataclasses_json-0.6.6/dataclasses_json/api.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/dataclasses_json/cfg.py` & `dataclasses_json-0.6.6/dataclasses_json/cfg.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/dataclasses_json/core.py` & `dataclasses_json-0.6.6/dataclasses_json/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,18 +227,18 @@
 
     return cls(**init_kwargs)
 
 
 def _decode_type(type_, value, infer_missing):
     if _has_decoder_in_global_config(type_):
         return _get_decoder_in_global_config(type_)(value)
-    if is_dataclass(type_) or is_dataclass(type_):
-        return _decode_dataclass(type_, value, infer_missing)
     if _is_supported_generic(type_):
         return _decode_generic(type_, value, infer_missing)
+    if is_dataclass(type_) or is_dataclass(value):
+        return _decode_dataclass(type_, value, infer_missing)
     return _support_extended_types(type_, value)
 
 
 def _support_extended_types(field_type, field_value):
     if _issubclass_safe(field_type, datetime):
         # FIXME this is a hack to deal with mm already decoding
         # the issue is we want to leverage mm fields' missing argument
```

### Comparing `dataclasses_json-0.6.5/dataclasses_json/mm.py` & `dataclasses_json-0.6.6/dataclasses_json/mm.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/dataclasses_json/stringcase.py` & `dataclasses_json-0.6.6/dataclasses_json/stringcase.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/dataclasses_json/undefined.py` & `dataclasses_json-0.6.6/dataclasses_json/undefined.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/dataclasses_json/utils.py` & `dataclasses_json-0.6.6/dataclasses_json/utils.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.5/pyproject.toml` & `dataclasses_json-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclasses-json"
-version = "0.6.5"
+version = "0.6.6"
 description = "Easily serialize dataclasses to and from JSON."
 authors = ["Charles Li <charles.dt.li@gmail.com>"]
 maintainers = ['Charles Li <charles.dt.li@gmail.com>', 'Georgiy Zubrienko <gzu@ecco.com>', 'Vitaliy Savitskiy <visa@ecco.com>', 'Matthias Als <mata@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/lidatong/dataclasses-json'
```

### Comparing `dataclasses_json-0.6.5/PKG-INFO` & `dataclasses_json-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-json
-Version: 0.6.5
+Version: 0.6.6
 Summary: Easily serialize dataclasses to and from JSON.
 Home-page: https://github.com/lidatong/dataclasses-json
 License: MIT
 Author: Charles Li
 Author-email: charles.dt.li@gmail.com
 Maintainer: Charles Li
 Maintainer-email: charles.dt.li@gmail.com
```

