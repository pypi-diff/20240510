# Comparing `tmp/watchmen_indicator_kernel-16.6.8.tar.gz` & `tmp/watchmen_indicator_kernel-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_kernel-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_indicator_kernel-16.6.9.tar", max compression
```

## Comparing `watchmen_indicator_kernel-16.6.8.tar` & `watchmen_indicator_kernel-16.6.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1281 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/__init__.py
--rw-r--r--   0        0        0       86 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/common/__init__.py
--rw-r--r--   0        0        0       49 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/common/exception.py
--rw-r--r--   0        0        0      331 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/common/settings.py
--rw-r--r--   0        0        0      552 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/__init__.py
--rw-r--r--   0        0        0      166 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/convergence/__init__.py
--rw-r--r--   0        0        0      332 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/convergence/data_helper.py
--rw-r--r--   0        0        0      775 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/convergence/data_service.py
--rw-r--r--   0        0        0      162 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective/__init__.py
--rw-r--r--   0        0        0      313 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective/data_helper.py
--rw-r--r--   0        0        0    29732 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective/data_service.py
--rw-r--r--   0        0        0      178 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
--rw-r--r--   0        0        0     2678 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
--rw-r--r--   0        0        0    11987 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
--rw-r--r--   0        0        0    21400 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
--rw-r--r--   0        0        0    10799 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
--rw-r--r--   0        0        0     8341 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
--rw-r--r--   0        0        0      397 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/__init__.py
--rw-r--r--   0        0        0     1088 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/bucket.py
--rw-r--r--   0        0        0      979 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/derived_objective.py
--rw-r--r--   0        0        0     1051 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/enum.py
--rw-r--r--   0        0        0      284 2024-01-08 07:58:02.504594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/factor.py
--rw-r--r--   0        0        0     1330 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/indicator.py
--rw-r--r--   0        0        0     3110 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/parameter.py
--rw-r--r--   0        0        0      786 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/subject.py
--rw-r--r--   0        0        0    12305 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/time_frame.py
--rw-r--r--   0        0        0     1074 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/topic.py
--rw-r--r--   0        0        0      457 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1762 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/achievement_task_service.py
--rw-r--r--   0        0        0     8647 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/bucket_service.py
--rw-r--r--   0        0        0     5210 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/convergence_service.py
--rw-r--r--   0        0        0     4619 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/derived_objective_report_service.py
--rw-r--r--   0        0        0     4960 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/derived_objective_service.py
--rw-r--r--   0        0        0     6695 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/indicator_service.py
--rw-r--r--   0        0        0     3177 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/objective_report_service.py
--rw-r--r--   0        0        0     5783 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/objective_service.py
--rw-r--r--   0        0        0       46 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/plugin/__init__.py
--rw-r--r--   0        0        0      678 2024-01-08 07:58:02.508594 watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/plugin/connector.py
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1281 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/__init__.py
+-rw-r--r--   0        0        0       86 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/common/__init__.py
+-rw-r--r--   0        0        0       49 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/common/exception.py
+-rw-r--r--   0        0        0      331 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/common/settings.py
+-rw-r--r--   0        0        0      552 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/__init__.py
+-rw-r--r--   0        0        0      166 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/convergence/__init__.py
+-rw-r--r--   0        0        0      332 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/convergence/data_helper.py
+-rw-r--r--   0        0        0      775 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/convergence/data_service.py
+-rw-r--r--   0        0        0      162 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective/__init__.py
+-rw-r--r--   0        0        0      313 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective/data_helper.py
+-rw-r--r--   0        0        0    29732 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective/data_service.py
+-rw-r--r--   0        0        0      178 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
+-rw-r--r--   0        0        0     2678 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
+-rw-r--r--   0        0        0    11987 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
+-rw-r--r--   0        0        0    21400 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
+-rw-r--r--   0        0        0    10799 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
+-rw-r--r--   0        0        0     8341 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
+-rw-r--r--   0        0        0      397 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/__init__.py
+-rw-r--r--   0        0        0     1088 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/bucket.py
+-rw-r--r--   0        0        0      979 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/derived_objective.py
+-rw-r--r--   0        0        0     1051 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/enum.py
+-rw-r--r--   0        0        0      284 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/factor.py
+-rw-r--r--   0        0        0     1330 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/indicator.py
+-rw-r--r--   0        0        0     3110 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/parameter.py
+-rw-r--r--   0        0        0      786 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/subject.py
+-rw-r--r--   0        0        0    12305 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/time_frame.py
+-rw-r--r--   0        0        0     1074 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/topic.py
+-rw-r--r--   0        0        0      457 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1762 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/achievement_task_service.py
+-rw-r--r--   0        0        0     8647 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/bucket_service.py
+-rw-r--r--   0        0        0     5210 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/convergence_service.py
+-rw-r--r--   0        0        0     4619 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/derived_objective_report_service.py
+-rw-r--r--   0        0        0     4960 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/derived_objective_service.py
+-rw-r--r--   0        0        0     6695 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/indicator_service.py
+-rw-r--r--   0        0        0     3177 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/objective_report_service.py
+-rw-r--r--   0        0        0     5783 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/objective_service.py
+-rw-r--r--   0        0        0       46 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/plugin/__init__.py
+-rw-r--r--   0        0        0      678 2024-02-01 01:32:37.239323 watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/plugin/connector.py
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.6.9/PKG-INFO
```

### Comparing `watchmen_indicator_kernel-16.6.8/pyproject.toml` & `watchmen_indicator_kernel-16.6.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-indicator-kernel"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.6.8"
-watchmen-inquiry-trino = { version = "16.6.8", optional = true }
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
-watchmen-storage-oss = { version = "16.6.8", optional = true }
-watchmen-storage-s3 = { version = "16.6.8", optional = true }
+watchmen-inquiry-kernel = "16.6.9"
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

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/__init__.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/convergence/data_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/convergence/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective/data_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/data_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/bucket.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/bucket.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/derived_objective.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/derived_objective.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/enum.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/enum.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/indicator.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/indicator.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/parameter.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/subject.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/subject.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/time_frame.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/time_frame.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/data/utils/topic.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/data/utils/topic.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/achievement_task_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/achievement_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/bucket_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/bucket_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/convergence_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/convergence_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/derived_objective_report_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/derived_objective_report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/derived_objective_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/derived_objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/indicator_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/indicator_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/objective_report_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/objective_report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/meta/objective_service.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/meta/objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/src/watchmen_indicator_kernel/plugin/connector.py` & `watchmen_indicator_kernel-16.6.9/src/watchmen_indicator_kernel/plugin/connector.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.6.8/PKG-INFO` & `watchmen_indicator_kernel-16.6.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-indicator-kernel
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,16 +16,16 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.6.8)
-Requires-Dist: watchmen-inquiry-trino (==16.6.8) ; extra == "trino"
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.6.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.6.8) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.6.9)
+Requires-Dist: watchmen-inquiry-trino (==16.6.9) ; extra == "trino"
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.6.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.6.9) ; extra == "s3"
```

