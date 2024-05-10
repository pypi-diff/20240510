# Comparing `tmp/watchmen_storage_s3-16.6.8.tar.gz` & `tmp/watchmen_storage_s3-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_s3-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage_s3-16.6.9.tar", max compression
```

## Comparing `watchmen_storage_s3-16.6.8.tar` & `watchmen_storage_s3-16.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/LICENSE
--rw-r--r--   0        0        0      450 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      180 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/__init__.py
--rw-r--r--   0        0        0     1308 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/data_source_s3.py
--rw-r--r--   0        0        0     1001 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/object_defs_s3.py
--rw-r--r--   0        0        0     5762 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/simple_storage_service.py
--rw-r--r--   0        0        0     9445 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/storage_s3.py
--rw-r--r--   0        0        0     1818 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/storage_s3_configuration.py
--rw-r--r--   0        0        0     2763 2024-01-08 07:58:02.560594 watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/where_build.py
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 watchmen_storage_s3-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/LICENSE
+-rw-r--r--   0        0        0      450 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/__init__.py
+-rw-r--r--   0        0        0     1308 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/data_source_s3.py
+-rw-r--r--   0        0        0     1001 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/object_defs_s3.py
+-rw-r--r--   0        0        0     5762 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/simple_storage_service.py
+-rw-r--r--   0        0        0     9445 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/storage_s3.py
+-rw-r--r--   0        0        0     1818 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/storage_s3_configuration.py
+-rw-r--r--   0        0        0     2763 2024-02-01 01:32:37.295323 watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/where_build.py
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 watchmen_storage_s3-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage_s3-16.6.8/LICENSE` & `watchmen_storage_s3-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/data_source_s3.py` & `watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/data_source_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/object_defs_s3.py` & `watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/object_defs_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/simple_storage_service.py` & `watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/simple_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/storage_s3.py` & `watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/storage_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/storage_s3_configuration.py` & `watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/storage_s3_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.6.8/src/watchmen_storage_s3/where_build.py` & `watchmen_storage_s3-16.6.9/src/watchmen_storage_s3/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.6.8/PKG-INFO` & `watchmen_storage_s3-16.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-s3
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.24.20,<2.0.0)
-Requires-Dist: watchmen-storage (==16.6.8)
+Requires-Dist: watchmen-storage (==16.6.9)
```

