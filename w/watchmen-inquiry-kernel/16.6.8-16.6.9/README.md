# Comparing `tmp/watchmen_inquiry_kernel-16.6.8.tar.gz` & `tmp/watchmen_inquiry_kernel-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_kernel-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_inquiry_kernel-16.6.9.tar", max compression
```

## Comparing `watchmen_inquiry_kernel-16.6.8.tar` & `watchmen_inquiry_kernel-16.6.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/LICENSE
--rw-r--r--   0        0        0     1310 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/__init__.py
--rw-r--r--   0        0        0      112 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/common/__init__.py
--rw-r--r--   0        0        0       47 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/common/exception.py
--rw-r--r--   0        0        0      622 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/common/settings.py
--rw-r--r--   0        0        0      289 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/common/utils.py
--rw-r--r--   0        0        0       86 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1847 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/meta/enum_service.py
--rw-r--r--   0        0        0     1404 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/meta/report_service.py
--rw-r--r--   0        0        0     2358 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/meta/subject_service.py
--rw-r--r--   0        0        0       82 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/schema/__init__.py
--rw-r--r--   0        0        0     2178 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/schema/report_schema.py
--rw-r--r--   0        0        0    12544 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/schema/subject_schema.py
--rw-r--r--   0        0        0      104 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1769 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/storage/report_data_service.py
--rw-r--r--   0        0        0     1496 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/storage/subject_data_service.py
--rw-r--r--   0        0        0    55853 2024-01-08 07:58:02.508594 watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/storage/subject_storage.py
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/LICENSE
+-rw-r--r--   0        0        0     1310 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/__init__.py
+-rw-r--r--   0        0        0      112 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/common/__init__.py
+-rw-r--r--   0        0        0       47 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/common/exception.py
+-rw-r--r--   0        0        0      622 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/common/settings.py
+-rw-r--r--   0        0        0      289 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/common/utils.py
+-rw-r--r--   0        0        0       86 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1847 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/meta/enum_service.py
+-rw-r--r--   0        0        0     1404 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/meta/report_service.py
+-rw-r--r--   0        0        0     2358 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/meta/subject_service.py
+-rw-r--r--   0        0        0       82 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/schema/__init__.py
+-rw-r--r--   0        0        0     2178 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/schema/report_schema.py
+-rw-r--r--   0        0        0    12544 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/schema/subject_schema.py
+-rw-r--r--   0        0        0      104 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1769 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/storage/report_data_service.py
+-rw-r--r--   0        0        0     1496 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/storage/subject_data_service.py
+-rw-r--r--   0        0        0    55853 2024-02-01 01:32:37.243322 watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/storage/subject_storage.py
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.6.9/PKG-INFO
```

### Comparing `watchmen_inquiry_kernel-16.6.8/LICENSE` & `watchmen_inquiry_kernel-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/pyproject.toml` & `watchmen_inquiry_kernel-16.6.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-kernel"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-kernel = "16.6.8"
-watchmen-pipeline-kernel = "16.6.8"
-watchmen-inquiry-trino = { version = "16.6.8", optional = true }
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
-watchmen-storage-oss = { version = "16.6.8", optional = true }
-watchmen-storage-s3 = { version = "16.6.8", optional = true }
+watchmen-data-kernel = "16.6.9"
+watchmen-pipeline-kernel = "16.6.9"
+watchmen-inquiry-trino = { version = "16.6.9", optional = true }
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
+watchmen-storage-oracle = { version = "16.6.9", optional = true }
+watchmen-storage-mongodb = { version = "16.6.9", optional = true }
+watchmen-storage-mssql = { version = "16.6.9", optional = true }
+watchmen-storage-postgresql = { version = "16.6.9", optional = true }
+watchmen-storage-oss = { version = "16.6.9", optional = true }
+watchmen-storage-s3 = { version = "16.6.9", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/common/settings.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/meta/enum_service.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/meta/enum_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/meta/report_service.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/meta/report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/meta/subject_service.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/meta/subject_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/schema/report_schema.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/schema/report_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/schema/subject_schema.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/schema/subject_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/storage/report_data_service.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/storage/report_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/storage/subject_data_service.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/storage/subject_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/src/watchmen_inquiry_kernel/storage/subject_storage.py` & `watchmen_inquiry_kernel-16.6.9/src/watchmen_inquiry_kernel/storage/subject_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.6.8/PKG-INFO` & `watchmen_inquiry_kernel-16.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-kernel
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,17 +16,17 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-data-kernel (==16.6.8)
-Requires-Dist: watchmen-inquiry-trino (==16.6.8) ; extra == "trino"
-Requires-Dist: watchmen-pipeline-kernel (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.6.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.6.8) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.6.9)
+Requires-Dist: watchmen-inquiry-trino (==16.6.9) ; extra == "trino"
+Requires-Dist: watchmen-pipeline-kernel (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.6.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.6.9) ; extra == "s3"
```

