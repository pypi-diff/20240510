# Comparing `tmp/crawlee-0.0.3b8.tar.gz` & `tmp/crawlee-0.0.3b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.3b8.tar", max compression
+gzip compressed data, was "crawlee-0.0.3b9.tar", max compression
```

## Comparing `crawlee-0.0.3b8.tar` & `crawlee-0.0.3b9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0    11355 2024-05-02 14:47:54.291449 crawlee-0.0.3b8/LICENSE
--rw-r--r--   0        0        0       17 2024-05-02 14:47:54.291449 crawlee-0.0.3b8/README.md
--rw-r--r--   0        0        0     6385 2024-05-02 14:48:15.307610 crawlee-0.0.3b8/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-02 14:47:54.291449 crawlee-0.0.3b8/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.291449 crawlee-0.0.3b8/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0      774 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/blocked.py
--rw-r--r--   0        0        0     3341 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1950 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     4668 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     5262 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/globs.py
--rw-r--r--   0        0        0     2056 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0     1585 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      470 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/__init__.py
--rw-r--r--   0        0        0     9224 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/base_dataset_client.py
--rw-r--r--   0        0        0     1904 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/base_dataset_collection_client.py
--rw-r--r--   0        0        0     3495 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/base_key_value_store_client.py
--rw-r--r--   0        0        0     2046 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
--rw-r--r--   0        0        0     5662 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/base_request_queue_client.py
--rw-r--r--   0        0        0     2013 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/base_request_queue_collection_client.py
--rw-r--r--   0        0        0     1823 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/base_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/py.typed
--rw-r--r--   0        0        0      735 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/base_storage_client/types.py
--rw-r--r--   0        0        0      186 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    25030 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     4696 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2145 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/basic_crawler/errors.py
--rw-r--r--   0        0        0     2279 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0     2798 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0       86 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     5392 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      524 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0     1246 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/configuration.py
--rw-r--r--   0        0        0      272 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/enqueue_strategy.py
--rw-r--r--   0        0        0       91 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2683 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1303 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     1857 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     4283 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       38 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     2834 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/log_config.py
--rw-r--r--   0        0        0       55 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/__init__.py
--rw-r--r--   0        0        0     5471 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/base_resource_client.py
--rw-r--r--   0        0        0     2769 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/base_resource_collection_client.py
--rw-r--r--   0        0        0    17305 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/dataset_client.py
--rw-r--r--   0        0        0     1450 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/dataset_collection_client.py
--rw-r--r--   0        0        0    19187 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/key_value_store_client.py
--rw-r--r--   0        0        0     1534 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/key_value_store_collection_client.py
--rw-r--r--   0        0        0    11318 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/py.typed
--rw-r--r--   0        0        0    22665 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/request_queue_client.py
--rw-r--r--   0        0        0     1518 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/memory_storage_client/request_queue_collection_client.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/py.typed
--rw-r--r--   0        0        0     6670 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/request.py
--rw-r--r--   0        0        0       67 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8084 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0     1651 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      150 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     7048 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15692 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     5004 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0     6486 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/models.py
--rw-r--r--   0        0        0        0 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2593 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2775 2024-05-02 14:47:54.295449 crawlee-0.0.3b8/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25855 2024-05-02 14:47:54.299450 crawlee-0.0.3b8/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-05-02 14:47:54.299450 crawlee-0.0.3b8/src/crawlee/types.py
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 crawlee-0.0.3b8/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/LICENSE
+-rw-r--r--   0        0        0       17 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/README.md
+-rw-r--r--   0        0        0     6385 2024-05-09 08:13:08.325150 crawlee-0.0.3b9/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/blocked.py
+-rw-r--r--   0        0        0     3341 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1950 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     4668 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     5262 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/globs.py
+-rw-r--r--   0        0        0     2056 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0     1585 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      470 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/__init__.py
+-rw-r--r--   0        0        0     9224 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_client.py
+-rw-r--r--   0        0        0     1904 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_collection_client.py
+-rw-r--r--   0        0        0     3495 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_client.py
+-rw-r--r--   0        0        0     2046 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
+-rw-r--r--   0        0        0     5662 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_client.py
+-rw-r--r--   0        0        0     2013 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_collection_client.py
+-rw-r--r--   0        0        0     1823 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/base_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/py.typed
+-rw-r--r--   0        0        0      735 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/base_storage_client/types.py
+-rw-r--r--   0        0        0      186 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    25030 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     4696 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2145 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/errors.py
+-rw-r--r--   0        0        0     2279 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0     2798 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0       86 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     5392 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      524 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0     1246 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/configuration.py
+-rw-r--r--   0        0        0      272 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/enqueue_strategy.py
+-rw-r--r--   0        0        0       91 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2682 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1303 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     1857 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     4283 2024-05-09 08:12:46.925110 crawlee-0.0.3b9/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       38 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     2834 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/log_config.py
+-rw-r--r--   0        0        0       55 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/__init__.py
+-rw-r--r--   0        0        0     5471 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/base_resource_client.py
+-rw-r--r--   0        0        0     2769 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/base_resource_collection_client.py
+-rw-r--r--   0        0        0    17305 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_client.py
+-rw-r--r--   0        0        0     1450 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_collection_client.py
+-rw-r--r--   0        0        0    19187 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/key_value_store_client.py
+-rw-r--r--   0        0        0     1534 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/key_value_store_collection_client.py
+-rw-r--r--   0        0        0    11318 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/py.typed
+-rw-r--r--   0        0        0    22665 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/request_queue_client.py
+-rw-r--r--   0        0        0     1518 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/memory_storage_client/request_queue_collection_client.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/py.typed
+-rw-r--r--   0        0        0     6670 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/request.py
+-rw-r--r--   0        0        0       67 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8084 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0     1651 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      150 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     7048 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15692 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     5004 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0     6486 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/models.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2593 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2775 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25855 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-05-09 08:12:46.929110 crawlee-0.0.3b9/src/crawlee/types.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 crawlee-0.0.3b9/PKG-INFO
```

### Comparing `crawlee-0.0.3b8/LICENSE` & `crawlee-0.0.3b9/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/pyproject.toml` & `crawlee-0.0.3b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.3b8"
+version = "0.0.3b9"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/blocked.py` & `crawlee-0.0.3b9/src/crawlee/_utils/blocked.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.3b9/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/crypto.py` & `crawlee-0.0.3b9/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.3b9/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.3b9/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/file.py` & `crawlee-0.0.3b9/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/globs.py` & `crawlee-0.0.3b9/src/crawlee/_utils/globs.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.3b9/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/math.py` & `crawlee-0.0.3b9/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.3b9/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.3b9/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/requests.py` & `crawlee-0.0.3b9/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/system.py` & `crawlee-0.0.3b9/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/_utils/wait.py` & `crawlee-0.0.3b9/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.3b9/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.3b9/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.3b9/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/autoscaling/types.py` & `crawlee-0.0.3b9/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/base_dataset_client.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/base_dataset_collection_client.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/base_key_value_store_client.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/base_key_value_store_collection_client.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/base_request_queue_client.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/base_request_queue_collection_client.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/base_storage_client.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/base_storage_client/types.py` & `crawlee-0.0.3b9/src/crawlee/base_storage_client/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.3b9/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.3b9/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/basic_crawler/errors.py` & `crawlee-0.0.3b9/src/crawlee/basic_crawler/errors.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.3b9/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/basic_crawler/types.py` & `crawlee-0.0.3b9/src/crawlee/basic_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/beautifulsoup_crawler/types.py` & `crawlee-0.0.3b9/src/crawlee/beautifulsoup_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/configuration.py` & `crawlee-0.0.3b9/src/crawlee/configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/events/event_manager.py` & `crawlee-0.0.3b9/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.3b9/src/crawlee/events/local_event_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class LocalEventManager(EventManager):
     """Local event manager for emitting system info events."""
 
     def __init__(
         self,
         *,
-        system_info_interval: timedelta = timedelta(seconds=60),
+        system_info_interval: timedelta = timedelta(seconds=1),
     ) -> None:
         """Create a new instance.
 
         Args:
             system_info_interval: Interval at which `SystemInfo` events are emitted.
             close_timeout: Optional timeout for closing the event manager.
         """
```

### Comparing `crawlee-0.0.3b8/src/crawlee/events/types.py` & `crawlee-0.0.3b9/src/crawlee/events/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.3b9/src/crawlee/http_clients/base_http_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/http_clients/httpx_client.py` & `crawlee-0.0.3b9/src/crawlee/http_clients/httpx_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.3b9/src/crawlee/http_crawler/http_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/log_config.py` & `crawlee-0.0.3b9/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/base_resource_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/base_resource_collection_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/dataset_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/dataset_collection_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/key_value_store_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/key_value_store_collection_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/memory_storage_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/request_queue_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/memory_storage_client/request_queue_collection_client.py` & `crawlee-0.0.3b9/src/crawlee/memory_storage_client/request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/request.py` & `crawlee-0.0.3b9/src/crawlee/request.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/sessions/models.py` & `crawlee-0.0.3b9/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/sessions/session.py` & `crawlee-0.0.3b9/src/crawlee/sessions/session.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.3b9/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storage_client_manager.py` & `crawlee-0.0.3b9/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storages/base_storage.py` & `crawlee-0.0.3b9/src/crawlee/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storages/dataset.py` & `crawlee-0.0.3b9/src/crawlee/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.3b9/src/crawlee/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storages/models.py` & `crawlee-0.0.3b9/src/crawlee/storages/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storages/request_list.py` & `crawlee-0.0.3b9/src/crawlee/storages/request_list.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storages/request_provider.py` & `crawlee-0.0.3b9/src/crawlee/storages/request_provider.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/storages/request_queue.py` & `crawlee-0.0.3b9/src/crawlee/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/src/crawlee/types.py` & `crawlee-0.0.3b9/src/crawlee/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b8/PKG-INFO` & `crawlee-0.0.3b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.3b8
+Version: 0.0.3b9
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

