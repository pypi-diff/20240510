# Comparing `tmp/watchmen_storage_mongodb-16.6.8.tar.gz` & `tmp/watchmen_storage_mongodb-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mongodb-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_storage_mongodb-16.6.9.tar", max compression
```

## Comparing `watchmen_storage_mongodb-16.6.8.tar` & `watchmen_storage_mongodb-16.6.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/LICENSE
--rw-r--r--   0        0        0      460 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      210 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/__init__.py
--rw-r--r--   0        0        0      703 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/codes_options.py
--rw-r--r--   0        0        0     1308 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/data_source_mongo.py
--rw-r--r--   0        0        0     2540 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/document_defs_helper.py
--rw-r--r--   0        0        0    18081 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/document_defs_mongo.py
--rw-r--r--   0        0        0     2541 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/document_mongo.py
--rw-r--r--   0        0        0     5632 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/engine_mongo.py
--rw-r--r--   0        0        0      509 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/sort_build.py
--rw-r--r--   0        0        0    21761 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/storage_mongo.py
--rw-r--r--   0        0        0     2120 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/storage_mongo_configuration.py
--rw-r--r--   0        0        0    11657 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/topic_document_generate.py
--rw-r--r--   0        0        0    24666 2024-01-08 07:58:02.536594 watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/where_build.py
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 watchmen_storage_mongodb-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.267323 watchmen_storage_mongodb-16.6.9/LICENSE
+-rw-r--r--   0        0        0      460 2024-02-01 01:32:37.267323 watchmen_storage_mongodb-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      210 2024-02-01 01:32:37.267323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/__init__.py
+-rw-r--r--   0        0        0      703 2024-02-01 01:32:37.267323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/codes_options.py
+-rw-r--r--   0        0        0     1308 2024-02-01 01:32:37.267323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/data_source_mongo.py
+-rw-r--r--   0        0        0     2540 2024-02-01 01:32:37.267323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/document_defs_helper.py
+-rw-r--r--   0        0        0    18081 2024-02-01 01:32:37.267323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/document_defs_mongo.py
+-rw-r--r--   0        0        0     2541 2024-02-01 01:32:37.271323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/document_mongo.py
+-rw-r--r--   0        0        0     5632 2024-02-01 01:32:37.271323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/engine_mongo.py
+-rw-r--r--   0        0        0      509 2024-02-01 01:32:37.271323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/sort_build.py
+-rw-r--r--   0        0        0    21761 2024-02-01 01:32:37.271323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/storage_mongo.py
+-rw-r--r--   0        0        0     2120 2024-02-01 01:32:37.271323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/storage_mongo_configuration.py
+-rw-r--r--   0        0        0    11657 2024-02-01 01:32:37.271323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/topic_document_generate.py
+-rw-r--r--   0        0        0    24666 2024-02-01 01:32:37.271323 watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/where_build.py
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 watchmen_storage_mongodb-16.6.9/PKG-INFO
```

### Comparing `watchmen_storage_mongodb-16.6.8/LICENSE` & `watchmen_storage_mongodb-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/codes_options.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/codes_options.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/data_source_mongo.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/data_source_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/document_defs_helper.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/document_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/document_defs_mongo.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/document_defs_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/document_mongo.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/document_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/engine_mongo.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/engine_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/storage_mongo.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/storage_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/storage_mongo_configuration.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/storage_mongo_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/topic_document_generate.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/topic_document_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/src/watchmen_storage_mongodb/where_build.py` & `watchmen_storage_mongodb-16.6.9/src/watchmen_storage_mongodb/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.6.8/PKG-INFO` & `watchmen_storage_mongodb-16.6.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mongodb
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
 Requires-Dist: pymongo (>=4.1.0,<5.0.0)
-Requires-Dist: watchmen-storage (==16.6.8)
+Requires-Dist: watchmen-storage (==16.6.9)
```

