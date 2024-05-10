# Comparing `tmp/watchmen_storage_postgresql-16.6.8.tar.gz` & `tmp/watchmen_storage_postgresql-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_postgresql-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage_postgresql-16.6.9.tar", max compression
```

## Comparing `watchmen_storage_postgresql-16.6.8.tar` & `watchmen_storage_postgresql-16.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.556594 watchmen_storage_postgresql-16.6.8/LICENSE
--rw-r--r--   0        0        0      478 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      309 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/__init__.py
--rw-r--r--   0        0        0     3557 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/data_source_postgresql.py
--rw-r--r--   0        0        0     2485 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/script_builder_postgresql.py
--rw-r--r--   0        0        0     7620 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/storage_postgresql.py
--rw-r--r--   0        0        0     2272 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
--rw-r--r--   0        0        0     7816 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/table_creator.py
--rw-r--r--   0        0        0    12722 2024-01-08 07:58:02.560594 watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/where_build.py
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.287323 watchmen_storage_postgresql-16.6.9/LICENSE
+-rw-r--r--   0        0        0      478 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      309 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/__init__.py
+-rw-r--r--   0        0        0     3557 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/data_source_postgresql.py
+-rw-r--r--   0        0        0     2485 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/script_builder_postgresql.py
+-rw-r--r--   0        0        0     7620 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/storage_postgresql.py
+-rw-r--r--   0        0        0     2272 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
+-rw-r--r--   0        0        0     7816 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/table_creator.py
+-rw-r--r--   0        0        0    12722 2024-02-01 01:32:37.291323 watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/where_build.py
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage_postgresql-16.6.8/LICENSE` & `watchmen_storage_postgresql-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/data_source_postgresql.py` & `watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/data_source_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/script_builder_postgresql.py` & `watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/script_builder_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/storage_postgresql.py` & `watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/storage_postgresql_configuration.py` & `watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/storage_postgresql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/table_creator.py` & `watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.6.8/src/watchmen_storage_postgresql/where_build.py` & `watchmen_storage_postgresql-16.6.9/src/watchmen_storage_postgresql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.6.8/PKG-INFO` & `watchmen_storage_postgresql-16.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-postgresql
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
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
-Requires-Dist: watchmen-storage-rds (==16.6.8)
+Requires-Dist: watchmen-storage-rds (==16.6.9)
```

