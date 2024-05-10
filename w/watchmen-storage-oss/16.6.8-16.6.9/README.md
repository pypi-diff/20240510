# Comparing `tmp/watchmen_storage_oss-16.6.8.tar.gz` & `tmp/watchmen_storage_oss-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_oss-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage_oss-16.6.9.tar", max compression
```

## Comparing `watchmen_storage_oss-16.6.8.tar` & `watchmen_storage_oss-16.6.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.552594 watchmen_storage_oss-16.6.8/LICENSE
--rw-r--r--   0        0        0      449 2024-01-08 07:58:02.552594 watchmen_storage_oss-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      112 2024-01-08 07:58:02.552594 watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/__init__.py
--rw-r--r--   0        0        0     1299 2024-01-08 07:58:02.552594 watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/data_source_oss.py
--rw-r--r--   0        0        0      495 2024-01-08 07:58:02.552594 watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/object_defs_oss.py
--rw-r--r--   0        0        0     1657 2024-01-08 07:58:02.556594 watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/object_storage_service.py
--rw-r--r--   0        0        0     9337 2024-01-08 07:58:02.556594 watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/storage_oss.py
--rw-r--r--   0        0        0     1836 2024-01-08 07:58:02.556594 watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/storage_oss_configuration.py
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/LICENSE
+-rw-r--r--   0        0        0      449 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      112 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/__init__.py
+-rw-r--r--   0        0        0     1299 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/data_source_oss.py
+-rw-r--r--   0        0        0      495 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/object_defs_oss.py
+-rw-r--r--   0        0        0     1657 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/object_storage_service.py
+-rw-r--r--   0        0        0     9337 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/storage_oss.py
+-rw-r--r--   0        0        0     1836 2024-02-01 01:32:37.287323 watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/storage_oss_configuration.py
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage_oss-16.6.8/LICENSE` & `watchmen_storage_oss-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/data_source_oss.py` & `watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/data_source_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/object_storage_service.py` & `watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/object_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/storage_oss.py` & `watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/storage_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.6.8/src/watchmen_storage_oss/storage_oss_configuration.py` & `watchmen_storage_oss-16.6.9/src/watchmen_storage_oss/storage_oss_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.6.8/PKG-INFO` & `watchmen_storage_oss-16.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-oss
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
 Requires-Dist: oss2 (==2.15.0)
-Requires-Dist: watchmen-storage (==16.6.8)
+Requires-Dist: watchmen-storage (==16.6.9)
```

