# Comparing `tmp/watchmen_storage-16.6.8.tar.gz` & `tmp/watchmen_storage-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage-16.6.9.tar", max compression
```

## Comparing `watchmen_storage-16.6.8.tar` & `watchmen_storage-16.6.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/LICENSE
--rw-r--r--   0        0        0      442 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/pyproject.toml
--rw-r--r--   0        0        0     2349 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5947 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1853 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0     1154 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0      163 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/sql_analysis/__init__.py
--rw-r--r--   0        0        0    10962 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/sql_analysis/ast_visitor.py
--rw-r--r--   0        0        0     2833 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/sql_analysis/parse_sql.py
--rw-r--r--   0        0        0     1441 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/sql_analysis/topic_generator.py
--rw-r--r--   0        0        0     7572 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0     1125 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/storage_based_worker_id_service.py
--rw-r--r--   0        0        0      721 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     6209 2024-01-08 07:58:02.560594 watchmen_storage-16.6.8/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4717 2024-01-08 07:58:02.564594 watchmen_storage-16.6.8/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2024-01-08 07:58:02.564594 watchmen_storage-16.6.8/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 watchmen_storage-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/LICENSE
+-rw-r--r--   0        0        0      442 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0     2349 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5947 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1853 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0     1154 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0      163 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/sql_analysis/__init__.py
+-rw-r--r--   0        0        0    10962 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/sql_analysis/ast_visitor.py
+-rw-r--r--   0        0        0     2833 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/sql_analysis/parse_sql.py
+-rw-r--r--   0        0        0     1441 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/sql_analysis/topic_generator.py
+-rw-r--r--   0        0        0     7572 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0     1125 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/storage_based_worker_id_service.py
+-rw-r--r--   0        0        0      721 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     6209 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4717 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2024-02-01 01:32:37.295323 watchmen_storage-16.6.9/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 watchmen_storage-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage-16.6.8/LICENSE` & `watchmen_storage-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/__init__.py` & `watchmen_storage-16.6.9/src/watchmen_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.6.9/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.6.9/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.6.9/src/watchmen_storage/free_storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.6.9/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/settings.py` & `watchmen_storage-16.6.9/src/watchmen_storage/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.6.9/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/sql_analysis/ast_visitor.py` & `watchmen_storage-16.6.9/src/watchmen_storage/sql_analysis/ast_visitor.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/sql_analysis/parse_sql.py` & `watchmen_storage-16.6.9/src/watchmen_storage/sql_analysis/parse_sql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/sql_analysis/topic_generator.py` & `watchmen_storage-16.6.9/src/watchmen_storage/sql_analysis/topic_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.6.9/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/storage_based_worker_id_service.py` & `watchmen_storage-16.6.9/src/watchmen_storage/storage_based_worker_id_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.6.9/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.6.9/src/watchmen_storage/storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.6.9/src/watchmen_storage/storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.6.9/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.6.8/PKG-INFO` & `watchmen_storage-16.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage
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
 Requires-Dist: boto3 (==1.24.45)
-Requires-Dist: watchmen-model (==16.6.8)
+Requires-Dist: watchmen-model (==16.6.9)
```

