# Comparing `tmp/watchmen_storage_mssql-16.6.8.tar.gz` & `tmp/watchmen_storage_mssql-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mssql-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage_mssql-16.6.9.tar", max compression
```

## Comparing `watchmen_storage_mssql-16.6.8.tar` & `watchmen_storage_mssql-16.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.536594 watchmen_storage_mssql-16.6.8/LICENSE
--rw-r--r--   0        0        0      460 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      259 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/__init__.py
--rw-r--r--   0        0        0     2294 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/data_source_mssql.py
--rw-r--r--   0        0        0     2450 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/script_builder_mssql.py
--rw-r--r--   0        0        0     7773 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/storage_mssql.py
--rw-r--r--   0        0        0     2307 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/storage_mssql_configuration.py
--rw-r--r--   0        0        0     7971 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/table_creator.py
--rw-r--r--   0        0        0    12499 2024-01-08 07:58:02.540594 watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/where_build.py
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 watchmen_storage_mssql-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.271323 watchmen_storage_mssql-16.6.9/LICENSE
+-rw-r--r--   0        0        0      460 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/__init__.py
+-rw-r--r--   0        0        0     2294 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/data_source_mssql.py
+-rw-r--r--   0        0        0     2450 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/script_builder_mssql.py
+-rw-r--r--   0        0        0     7773 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/storage_mssql.py
+-rw-r--r--   0        0        0     2307 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/storage_mssql_configuration.py
+-rw-r--r--   0        0        0     7971 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/table_creator.py
+-rw-r--r--   0        0        0    12499 2024-02-01 01:32:37.275323 watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/where_build.py
+-rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 watchmen_storage_mssql-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage_mssql-16.6.8/LICENSE` & `watchmen_storage_mssql-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/data_source_mssql.py` & `watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/data_source_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/script_builder_mssql.py` & `watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/script_builder_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/storage_mssql.py` & `watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/storage_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/storage_mssql_configuration.py` & `watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/storage_mssql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/table_creator.py` & `watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.6.8/src/watchmen_storage_mssql/where_build.py` & `watchmen_storage_mssql-16.6.9/src/watchmen_storage_mssql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.6.8/PKG-INFO` & `watchmen_storage_mssql-16.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mssql
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
 Requires-Dist: pyodbc (>=4.0.32,<5.0.0)
-Requires-Dist: watchmen-storage-rds (==16.6.8)
+Requires-Dist: watchmen-storage-rds (==16.6.9)
```

