# Comparing `tmp/watchmen_storage_mysql-16.6.8.tar.gz` & `tmp/watchmen_storage_mysql-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mysql-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage_mysql-16.6.9.tar", max compression
```

## Comparing `watchmen_storage_mysql-16.6.8.tar` & `watchmen_storage_mysql-16.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.544594 watchmen_storage_mysql-16.6.8/LICENSE
--rw-r--r--   0        0        0      485 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      258 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/__init__.py
--rw-r--r--   0        0        0     2906 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/data_source_mysql.py
--rw-r--r--   0        0        0     2197 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/script_builder_mysql.py
--rw-r--r--   0        0        0     5302 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/storage_mysql.py
--rw-r--r--   0        0        0     2187 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/storage_mysql_configuration.py
--rw-r--r--   0        0        0     8699 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/table_creator.py
--rw-r--r--   0        0        0    12016 2024-01-08 07:58:02.548594 watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/where_build.py
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 watchmen_storage_mysql-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.275323 watchmen_storage_mysql-16.6.9/LICENSE
+-rw-r--r--   0        0        0      485 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      258 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/__init__.py
+-rw-r--r--   0        0        0     2906 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/data_source_mysql.py
+-rw-r--r--   0        0        0     2197 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/script_builder_mysql.py
+-rw-r--r--   0        0        0     5302 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/storage_mysql.py
+-rw-r--r--   0        0        0     2187 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/storage_mysql_configuration.py
+-rw-r--r--   0        0        0     8699 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/table_creator.py
+-rw-r--r--   0        0        0    12016 2024-02-01 01:32:37.279323 watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/where_build.py
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 watchmen_storage_mysql-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage_mysql-16.6.8/LICENSE` & `watchmen_storage_mysql-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/data_source_mysql.py` & `watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/data_source_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/script_builder_mysql.py` & `watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/script_builder_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/storage_mysql.py` & `watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/storage_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/storage_mysql_configuration.py` & `watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/storage_mysql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/table_creator.py` & `watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.6.8/src/watchmen_storage_mysql/where_build.py` & `watchmen_storage_mysql-16.6.9/src/watchmen_storage_mysql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.6.8/PKG-INFO` & `watchmen_storage_mysql-16.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mysql
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
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: cryptography (>=36.0.2,<37.0.0)
-Requires-Dist: watchmen-storage-rds (==16.6.8)
+Requires-Dist: watchmen-storage-rds (==16.6.9)
```

