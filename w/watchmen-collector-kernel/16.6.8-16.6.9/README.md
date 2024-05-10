# Comparing `tmp/watchmen_collector_kernel-16.6.8.tar.gz` & `tmp/watchmen_collector_kernel-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_collector_kernel-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_collector_kernel-16.6.9.tar", max compression
```

## Comparing `watchmen_collector_kernel-16.6.8.tar` & `watchmen_collector_kernel-16.6.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/LICENSE
--rw-r--r--   0        0        0     1197 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/__init__.py
--rw-r--r--   0        0        0       59 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/__init__.py
--rw-r--r--   0        0        0     2381 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/collector_cache_manger.py
--rw-r--r--   0        0        0      905 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/collector_cache_service.py
--rw-r--r--   0        0        0     1191 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/collector_topic_cache.py
--rw-r--r--   0        0        0     1906 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/model_config_cache.py
--rw-r--r--   0        0        0     1393 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/module_config_cache.py
--rw-r--r--   0        0        0     4390 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/table_config_cache.py
--rw-r--r--   0        0        0      563 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/common/__init__.py
--rw-r--r--   0        0        0      320 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/common/constants.py
--rw-r--r--   0        0        0       49 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/common/exception.py
--rw-r--r--   0        0        0     1746 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/common/settings.py
--rw-r--r--   0        0        0      845 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/__init__.py
--rw-r--r--   0        0        0      530 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/change_data_json.py
--rw-r--r--   0        0        0       99 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/change_data_json_history.py
--rw-r--r--   0        0        0      355 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/change_data_record.py
--rw-r--r--   0        0        0      106 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/change_data_record_history.py
--rw-r--r--   0        0        0      322 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/collector_model_config.py
--rw-r--r--   0        0        0      250 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/collector_module_config.py
--rw-r--r--   0        0        0     2969 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/collector_table_config.py
--rw-r--r--   0        0        0      264 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/competitive_lock.py
--rw-r--r--   0        0        0     1619 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/condition.py
--rw-r--r--   0        0        0     1479 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/scheduled_task.py
--rw-r--r--   0        0        0       93 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/scheduled_task_history.py
--rw-r--r--   0        0        0      196 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/status.py
--rw-r--r--   0        0        0      479 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/trigger_event.py
--rw-r--r--   0        0        0      213 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/trigger_model.py
--rw-r--r--   0        0        0      193 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/trigger_module.py
--rw-r--r--   0        0        0      251 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/trigger_table.py
--rw-r--r--   0        0        0      742 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/__init__.py
--rw-r--r--   0        0        0     2358 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/criteria_builder.py
--rw-r--r--   0        0        0     3555 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/data_capture.py
--rw-r--r--   0        0        0    15571 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/extract_source.py
--rw-r--r--   0        0        0      728 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/extract_spi.py
--rw-r--r--   0        0        0     2452 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/extract_utils.py
--rw-r--r--   0        0        0      924 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/lock_helper.py
--rw-r--r--   0        0        0     2235 2024-01-08 07:58:02.492594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/model_config_service.py
--rw-r--r--   0        0        0     2027 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/module_config_service.py
--rw-r--r--   0        0        0     3962 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/table_config_service.py
--rw-r--r--   0        0        0     4673 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/task_service.py
--rw-r--r--   0        0        0    10852 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/trigger_collector.py
--rw-r--r--   0        0        0    17784 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/trigger_event_helper.py
--rw-r--r--   0        0        0     1369 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1774 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
--rw-r--r--   0        0        0    12089 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_json_service.py
--rw-r--r--   0        0        0     1845 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
--rw-r--r--   0        0        0    10458 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_record_service.py
--rw-r--r--   0        0        0     4541 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/collector_model_config_service.py
--rw-r--r--   0        0        0     3807 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/collector_module_config_service.py
--rw-r--r--   0        0        0     7705 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/collector_table_config_service.py
--rw-r--r--   0        0        0     3154 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/competitive_lock_service.py
--rw-r--r--   0        0        0     1586 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
--rw-r--r--   0        0        0    10206 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/scheduled_task_service.py
--rw-r--r--   0        0        0     6836 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_event_service.py
--rw-r--r--   0        0        0     3760 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_model_service.py
--rw-r--r--   0        0        0     3377 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_module_service.py
--rw-r--r--   0        0        0     3915 2024-01-08 07:58:02.496594 watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_table_service.py
--rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/LICENSE
+-rw-r--r--   0        0        0     1197 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/__init__.py
+-rw-r--r--   0        0        0       59 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/__init__.py
+-rw-r--r--   0        0        0     2381 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/collector_cache_manger.py
+-rw-r--r--   0        0        0      905 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/collector_cache_service.py
+-rw-r--r--   0        0        0     1191 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/collector_topic_cache.py
+-rw-r--r--   0        0        0     1906 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/model_config_cache.py
+-rw-r--r--   0        0        0     1393 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/module_config_cache.py
+-rw-r--r--   0        0        0     4390 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/table_config_cache.py
+-rw-r--r--   0        0        0      563 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/common/__init__.py
+-rw-r--r--   0        0        0      320 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/common/constants.py
+-rw-r--r--   0        0        0       49 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/common/exception.py
+-rw-r--r--   0        0        0     1746 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/common/settings.py
+-rw-r--r--   0        0        0      845 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/__init__.py
+-rw-r--r--   0        0        0      530 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/change_data_json.py
+-rw-r--r--   0        0        0       99 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/change_data_json_history.py
+-rw-r--r--   0        0        0      355 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/change_data_record.py
+-rw-r--r--   0        0        0      106 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/change_data_record_history.py
+-rw-r--r--   0        0        0      322 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/collector_model_config.py
+-rw-r--r--   0        0        0      250 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/collector_module_config.py
+-rw-r--r--   0        0        0     2969 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/collector_table_config.py
+-rw-r--r--   0        0        0      264 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/competitive_lock.py
+-rw-r--r--   0        0        0     1619 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/condition.py
+-rw-r--r--   0        0        0     1479 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/scheduled_task.py
+-rw-r--r--   0        0        0       93 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/scheduled_task_history.py
+-rw-r--r--   0        0        0      196 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/status.py
+-rw-r--r--   0        0        0      479 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/trigger_event.py
+-rw-r--r--   0        0        0      213 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/trigger_model.py
+-rw-r--r--   0        0        0      193 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/trigger_module.py
+-rw-r--r--   0        0        0      251 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/trigger_table.py
+-rw-r--r--   0        0        0      742 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/__init__.py
+-rw-r--r--   0        0        0     2358 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/criteria_builder.py
+-rw-r--r--   0        0        0     3555 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/data_capture.py
+-rw-r--r--   0        0        0    15571 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/extract_source.py
+-rw-r--r--   0        0        0      728 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/extract_spi.py
+-rw-r--r--   0        0        0     2452 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/extract_utils.py
+-rw-r--r--   0        0        0      924 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/lock_helper.py
+-rw-r--r--   0        0        0     2235 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/model_config_service.py
+-rw-r--r--   0        0        0     2027 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/module_config_service.py
+-rw-r--r--   0        0        0     3962 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/table_config_service.py
+-rw-r--r--   0        0        0     4673 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/task_service.py
+-rw-r--r--   0        0        0    10852 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/trigger_collector.py
+-rw-r--r--   0        0        0    17784 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/trigger_event_helper.py
+-rw-r--r--   0        0        0     1369 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1774 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
+-rw-r--r--   0        0        0    12089 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_json_service.py
+-rw-r--r--   0        0        0     1845 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
+-rw-r--r--   0        0        0    10458 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_record_service.py
+-rw-r--r--   0        0        0     4555 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/collector_model_config_service.py
+-rw-r--r--   0        0        0     3821 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/collector_module_config_service.py
+-rw-r--r--   0        0        0     7705 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/collector_table_config_service.py
+-rw-r--r--   0        0        0     3154 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/competitive_lock_service.py
+-rw-r--r--   0        0        0     1586 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
+-rw-r--r--   0        0        0    10206 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/scheduled_task_service.py
+-rw-r--r--   0        0        0     6836 2024-02-01 01:32:37.227322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_event_service.py
+-rw-r--r--   0        0        0     3760 2024-02-01 01:32:37.231322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_model_service.py
+-rw-r--r--   0        0        0     3377 2024-02-01 01:32:37.231322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_module_service.py
+-rw-r--r--   0        0        0     3915 2024-02-01 01:32:37.231322 watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_table_service.py
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.6.9/PKG-INFO
```

### Comparing `watchmen_collector_kernel-16.6.8/LICENSE` & `watchmen_collector_kernel-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/pyproject.toml` & `watchmen_collector_kernel-16.6.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-collector-kernel"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_collector_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.3"
-watchmen-data-kernel = "16.6.8"
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
-watchmen-storage-oss = { version = "16.6.8", optional = true }
-watchmen-storage-s3 = { version = "16.6.8", optional = true }
+watchmen-data-kernel = "16.6.9"
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

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/collector_cache_manger.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/collector_cache_manger.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/collector_cache_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/collector_cache_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/collector_topic_cache.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/collector_topic_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/model_config_cache.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/model_config_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/module_config_cache.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/module_config_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/cache/table_config_cache.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/cache/table_config_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/common/__init__.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/common/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/common/settings.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/__init__.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/change_data_json.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/change_data_json.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/collector_table_config.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/collector_table_config.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/condition.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/condition.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/model/scheduled_task.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/model/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/__init__.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/criteria_builder.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/criteria_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/data_capture.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/data_capture.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/extract_source.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/extract_source.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/extract_spi.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/extract_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/extract_utils.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/extract_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/lock_helper.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/lock_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/model_config_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/model_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/module_config_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/module_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/table_config_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/table_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/task_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/trigger_collector.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/trigger_collector.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/service/trigger_event_helper.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/service/trigger_event_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/__init__.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_json_history_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_json_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_json_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_json_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_record_history_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_record_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/change_data_record_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/change_data_record_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/collector_model_config_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/collector_model_config_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from watchmen_auth import PrincipalService
 from watchmen_collector_kernel.model import CollectorModelConfig
 from watchmen_meta.common import TupleService, TupleShaper
 from watchmen_meta.common.storage_service import StorableId
 from watchmen_model.common import Storable, TenantId, CollectorModelConfigId
 from watchmen_storage import EntityName, EntityRow, EntityShaper, TransactionalStorageSPI, SnowflakeGenerator, \
-	EntityCriteriaExpression, ColumnNameLiteral, EntitySort, EntitySortMethod
+	EntityCriteriaExpression, ColumnNameLiteral, EntitySortMethod, EntitySortColumn
 
 
 class CollectorModelConfigShaper(EntityShaper):
 	def serialize(self, config: CollectorModelConfig) -> EntityRow:
 		return TupleShaper.serialize_tenant_based(config, {
 			'model_id': config.modelId,
 			'model_name': config.modelName,
@@ -112,15 +112,15 @@
 			self.close_transaction()
 
 	def find_by_module_id(self, module_id: str) -> Optional[List[CollectorModelConfig]]:
 		# noinspection PyTypeChecker
 		return self.storage.find(self.get_entity_finder(
 			criteria=[
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='module_id'), right=module_id)],
-			sort=EntitySort(name='priority', method=EntitySortMethod.ASC)
+			sort=[EntitySortColumn(name='priority', method=EntitySortMethod.ASC)]
 		))
 
 
 def get_collector_model_config_service(storage: TransactionalStorageSPI,
                                        snowflake_generator: SnowflakeGenerator,
                                        principal_service: PrincipalService
                                        ) -> CollectorModelConfigService:
```

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/collector_module_config_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/collector_module_config_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from watchmen_auth import PrincipalService
 from watchmen_collector_kernel.model import CollectorModuleConfig
 from watchmen_meta.common import TupleService, TupleShaper
 from watchmen_meta.common.storage_service import StorableId
 from watchmen_model.common import Storable, TenantId, CollectorModelConfigId
 from watchmen_storage import EntityName, EntityRow, EntityShaper, TransactionalStorageSPI, SnowflakeGenerator, \
-	EntityCriteriaExpression, ColumnNameLiteral, EntitySort, EntitySortMethod
+	EntityCriteriaExpression, ColumnNameLiteral, EntitySortMethod, EntitySortColumn
 
 
 class CollectorModuleConfigShaper(EntityShaper):
 	def serialize(self, config: CollectorModuleConfig) -> EntityRow:
 		return TupleShaper.serialize_tenant_based(config, {
 			'module_id': config.moduleId,
 			'module_name': config.moduleName,
@@ -79,15 +79,15 @@
 			self.close_transaction()
 
 	def find_by_tenant(self, tenant_id: TenantId) -> Optional[List[CollectorModuleConfig]]:
 		# noinspection PyTypeChecker
 		return self.storage.find(self.get_entity_finder(
 			criteria=[
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tenant_id'), right=tenant_id)],
-			sort=EntitySort(name='priority', method=EntitySortMethod.ASC)
+			sort=[EntitySortColumn(name='priority', method=EntitySortMethod.ASC)]
 		))
 
 	def find_by_name(self, module_name: str) -> Optional[CollectorModuleConfig]:
 		self.begin_transaction()
 		try:
 			return self.storage.find_one(self.get_entity_finder(
 				criteria=[
```

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/collector_table_config_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/collector_table_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/competitive_lock_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/competitive_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/scheduled_task_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/scheduled_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_event_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_event_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_model_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_model_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_module_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_module_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/src/watchmen_collector_kernel/storage/trigger_table_service.py` & `watchmen_collector_kernel-16.6.9/src/watchmen_collector_kernel/storage/trigger_table_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.6.8/PKG-INFO` & `watchmen_collector_kernel-16.6.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-collector-kernel
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
-Requires-Dist: watchmen-data-kernel (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.6.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.6.8) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.6.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.6.9) ; extra == "s3"
```

