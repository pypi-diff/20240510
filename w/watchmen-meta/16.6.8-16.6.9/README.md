# Comparing `tmp/watchmen_meta-16.6.8.tar.gz` & `tmp/watchmen_meta-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_meta-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_meta-16.6.9.tar", max compression
```

## Comparing `watchmen_meta-16.6.8.tar` & `watchmen_meta-16.6.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/LICENSE
--rw-r--r--   0        0        0     1015 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/src/watchmen_meta/__init__.py
--rw-r--r--   0        0        0      496 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/src/watchmen_meta/admin/__init__.py
--rw-r--r--   0        0        0     5952 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/src/watchmen_meta/admin/enumeration_service.py
--rw-r--r--   0        0        0     3925 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/src/watchmen_meta/admin/pipeline_graphic_service.py
--rw-r--r--   0        0        0     6482 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/src/watchmen_meta/admin/pipeline_service.py
--rw-r--r--   0        0        0     4502 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/src/watchmen_meta/admin/space_service.py
--rw-r--r--   0        0        0     6568 2024-01-08 07:58:02.512594 watchmen_meta-16.6.8/src/watchmen_meta/admin/topic_service.py
--rw-r--r--   0        0        0     3740 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/admin/topic_snapshot_lock_service.py
--rw-r--r--   0        0        0     4882 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py
--rw-r--r--   0        0        0     3894 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/admin/user_group_service.py
--rw-r--r--   0        0        0     4658 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/admin/user_service.py
--rw-r--r--   0        0        0      108 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/analysis/__init__.py
--rw-r--r--   0        0        0     3024 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/analysis/pipeline_index_service.py
--rw-r--r--   0        0        0     5553 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/analysis/topic_index_service.py
--rw-r--r--   0        0        0       73 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/auth/__init__.py
--rw-r--r--   0        0        0     2731 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/auth/auth_helper.py
--rw-r--r--   0        0        0      726 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/__init__.py
--rw-r--r--   0        0        0       48 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/exception.py
--rw-r--r--   0        0        0      418 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/last_visit_service.py
--rw-r--r--   0        0        0     6252 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/operation_service.py
--rw-r--r--   0        0        0     4540 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/package_version_service.py
--rw-r--r--   0        0        0     7835 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/settings.py
--rw-r--r--   0        0        0     7488 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/storage_service.py
--rw-r--r--   0        0        0     6683 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/tuple_service.py
--rw-r--r--   0        0        0     6212 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/common/user_based_tuple_service.py
--rw-r--r--   0        0        0      267 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/console/__init__.py
--rw-r--r--   0        0        0     2289 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/console/connected_space_graphic_service.py
--rw-r--r--   0        0        0     6726 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/console/connected_space_service.py
--rw-r--r--   0        0        0     3570 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/console/dashboard_service.py
--rw-r--r--   0        0        0     5922 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/console/report_service.py
--rw-r--r--   0        0        0     5405 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/console/subject_service.py
--rw-r--r--   0        0        0      158 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/dqc/__init__.py
--rw-r--r--   0        0        0     2929 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/dqc/catalog_service.py
--rw-r--r--   0        0        0     2492 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/dqc/monitor_rule_lock_service.py
--rw-r--r--   0        0        0     4433 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/dqc/monitor_rule_service.py
--rw-r--r--   0        0        0      101 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/gui/__init__.py
--rw-r--r--   0        0        0     3389 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/gui/favorite_service.py
--rw-r--r--   0        0        0     3665 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/gui/last_snapshot_service.py
--rw-r--r--   0        0        0      277 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/__init__.py
--rw-r--r--   0        0        0     4389 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/data_source_service.py
--rw-r--r--   0        0        0     2718 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/external_writer_service.py
--rw-r--r--   0        0        0     1557 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/key_store_service.py
--rw-r--r--   0        0        0     3847 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/pat_service.py
--rw-r--r--   0        0        0     3076 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/plugin_service.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/sql_query_performance_service.py
--rw-r--r--   0        0        0     1782 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/system/tenant_service.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/webhook/__init__.py
--rw-r--r--   0        0        0     3223 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/webhook/event_definition_service.py
--rw-r--r--   0        0        0     2956 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/webhook/notification_definition_service.py
--rw-r--r--   0        0        0     2185 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/webhook/subscription_event_lock_service.py
--rw-r--r--   0        0        0     2976 2024-01-08 07:58:02.516594 watchmen_meta-16.6.8/src/watchmen_meta/webhook/subscription_event_service.py
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 watchmen_meta-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/LICENSE
+-rw-r--r--   0        0        0     1015 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/__init__.py
+-rw-r--r--   0        0        0      496 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/__init__.py
+-rw-r--r--   0        0        0     5952 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/enumeration_service.py
+-rw-r--r--   0        0        0     3925 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/pipeline_graphic_service.py
+-rw-r--r--   0        0        0     6482 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/pipeline_service.py
+-rw-r--r--   0        0        0     4502 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/space_service.py
+-rw-r--r--   0        0        0     6568 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/topic_service.py
+-rw-r--r--   0        0        0     3740 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/topic_snapshot_lock_service.py
+-rw-r--r--   0        0        0     4882 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py
+-rw-r--r--   0        0        0     3894 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/user_group_service.py
+-rw-r--r--   0        0        0     4658 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/admin/user_service.py
+-rw-r--r--   0        0        0      108 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/analysis/__init__.py
+-rw-r--r--   0        0        0     3024 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/analysis/pipeline_index_service.py
+-rw-r--r--   0        0        0     5553 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/analysis/topic_index_service.py
+-rw-r--r--   0        0        0       73 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/auth/__init__.py
+-rw-r--r--   0        0        0     2731 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/auth/auth_helper.py
+-rw-r--r--   0        0        0      726 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/__init__.py
+-rw-r--r--   0        0        0       48 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/exception.py
+-rw-r--r--   0        0        0      418 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/last_visit_service.py
+-rw-r--r--   0        0        0     6252 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/operation_service.py
+-rw-r--r--   0        0        0     4540 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/package_version_service.py
+-rw-r--r--   0        0        0     7835 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/settings.py
+-rw-r--r--   0        0        0     7488 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/storage_service.py
+-rw-r--r--   0        0        0     6683 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/tuple_service.py
+-rw-r--r--   0        0        0     6212 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/common/user_based_tuple_service.py
+-rw-r--r--   0        0        0      267 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/console/__init__.py
+-rw-r--r--   0        0        0     2289 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/console/connected_space_graphic_service.py
+-rw-r--r--   0        0        0     6726 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/console/connected_space_service.py
+-rw-r--r--   0        0        0     3570 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/console/dashboard_service.py
+-rw-r--r--   0        0        0     5922 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/console/report_service.py
+-rw-r--r--   0        0        0     5405 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/console/subject_service.py
+-rw-r--r--   0        0        0      158 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/dqc/__init__.py
+-rw-r--r--   0        0        0     2929 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/dqc/catalog_service.py
+-rw-r--r--   0        0        0     2492 2024-02-01 01:32:37.247323 watchmen_meta-16.6.9/src/watchmen_meta/dqc/monitor_rule_lock_service.py
+-rw-r--r--   0        0        0     4433 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/dqc/monitor_rule_service.py
+-rw-r--r--   0        0        0      101 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/gui/__init__.py
+-rw-r--r--   0        0        0     3389 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/gui/favorite_service.py
+-rw-r--r--   0        0        0     3665 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/gui/last_snapshot_service.py
+-rw-r--r--   0        0        0      277 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/__init__.py
+-rw-r--r--   0        0        0     4389 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/data_source_service.py
+-rw-r--r--   0        0        0     2718 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/external_writer_service.py
+-rw-r--r--   0        0        0     1557 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/key_store_service.py
+-rw-r--r--   0        0        0     3847 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/pat_service.py
+-rw-r--r--   0        0        0     3076 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/plugin_service.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/sql_query_performance_service.py
+-rw-r--r--   0        0        0     1782 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/system/tenant_service.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/webhook/__init__.py
+-rw-r--r--   0        0        0     3223 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/webhook/event_definition_service.py
+-rw-r--r--   0        0        0     2956 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/webhook/notification_definition_service.py
+-rw-r--r--   0        0        0     2185 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/webhook/subscription_event_lock_service.py
+-rw-r--r--   0        0        0     2976 2024-02-01 01:32:37.251323 watchmen_meta-16.6.9/src/watchmen_meta/webhook/subscription_event_service.py
+-rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 watchmen_meta-16.6.9/PKG-INFO
```

### Comparing `watchmen_meta-16.6.8/LICENSE` & `watchmen_meta-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/pyproject.toml` & `watchmen_meta-16.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "watchmen-meta"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_meta", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pycryptodome = "^3.14.1"
-watchmen-auth = "16.6.8"
-watchmen-storage = "16.6.8"
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
+watchmen-auth = "16.6.9"
+watchmen-storage = "16.6.9"
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
+watchmen-storage-oracle = { version = "16.6.9", optional = true }
+watchmen-storage-mongodb = { version = "16.6.9", optional = true }
+watchmen-storage-mssql = { version = "16.6.9", optional = true }
+watchmen-storage-postgresql = { version = "16.6.9", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/enumeration_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/enumeration_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/pipeline_graphic_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/pipeline_graphic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/pipeline_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/space_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/space_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/topic_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/topic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/topic_snapshot_lock_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/topic_snapshot_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/user_group_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/user_group_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/admin/user_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/admin/user_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/analysis/pipeline_index_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/analysis/pipeline_index_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/analysis/topic_index_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/analysis/topic_index_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/auth/auth_helper.py` & `watchmen_meta-16.6.9/src/watchmen_meta/auth/auth_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/common/__init__.py` & `watchmen_meta-16.6.9/src/watchmen_meta/common/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/common/operation_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/common/operation_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/common/package_version_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/common/package_version_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/common/settings.py` & `watchmen_meta-16.6.9/src/watchmen_meta/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/common/storage_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/common/storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/common/tuple_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/common/tuple_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/common/user_based_tuple_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/common/user_based_tuple_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/console/connected_space_graphic_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/console/connected_space_graphic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/console/connected_space_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/console/connected_space_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/console/dashboard_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/console/dashboard_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/console/report_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/console/report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/console/subject_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/console/subject_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/dqc/catalog_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/dqc/catalog_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/dqc/monitor_rule_lock_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/dqc/monitor_rule_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/dqc/monitor_rule_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/dqc/monitor_rule_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/gui/favorite_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/gui/favorite_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/gui/last_snapshot_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/gui/last_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/system/data_source_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/system/data_source_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/system/external_writer_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/system/external_writer_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/system/key_store_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/system/key_store_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/system/pat_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/system/pat_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/system/plugin_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/system/plugin_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/system/tenant_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/system/tenant_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/webhook/event_definition_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/webhook/event_definition_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/webhook/notification_definition_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/webhook/notification_definition_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/webhook/subscription_event_lock_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/webhook/subscription_event_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/src/watchmen_meta/webhook/subscription_event_service.py` & `watchmen_meta-16.6.9/src/watchmen_meta/webhook/subscription_event_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.6.8/PKG-INFO` & `watchmen_meta-16.6.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-meta
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: postgresql
 Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
-Requires-Dist: watchmen-auth (==16.6.8)
-Requires-Dist: watchmen-storage (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
+Requires-Dist: watchmen-auth (==16.6.9)
+Requires-Dist: watchmen-storage (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
```

