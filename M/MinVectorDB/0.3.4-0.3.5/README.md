# Comparing `tmp/minvectordb-0.3.4.tar.gz` & `tmp/minvectordb-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minvectordb-0.3.4.tar", last modified: Thu May  9 03:09:00 2024, max compression
+gzip compressed data, was "minvectordb-0.3.5.tar", last modified: Fri May 10 08:59:39 2024, max compression
```

## Comparing `minvectordb-0.3.4.tar` & `minvectordb-0.3.5.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.262261 minvectordb-0.3.4/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.3.4/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.261760 minvectordb-0.3.4/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    16875 2024-05-09 03:09:00.000000 minvectordb-0.3.4/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)     1632 2024-05-09 03:09:00.000000 minvectordb-0.3.4/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-05-09 03:09:00.000000 minvectordb-0.3.4/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       54 2024-05-09 03:09:00.000000 minvectordb-0.3.4/MinVectorDB.egg-info/entry_points.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.3.4/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      257 2024-05-09 03:09:00.000000 minvectordb-0.3.4/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-05-09 03:09:00.000000 minvectordb-0.3.4/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    16875 2024-05-09 03:09:00.262018 minvectordb-0.3.4/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    15477 2024-05-09 02:55:06.000000 minvectordb-0.3.4/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.253192 minvectordb-0.3.4/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)     1100 2024-05-09 02:07:57.000000 minvectordb-0.3.4/min_vec/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.254078 minvectordb-0.3.4/min_vec/api/
--rw-r--r--   0 guobingming   (501) staff       (20)      273 2024-04-23 05:39:11.000000 minvectordb-0.3.4/min_vec/api/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    31907 2024-05-09 02:43:57.000000 minvectordb-0.3.4/min_vec/api/client_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)    13492 2024-05-09 02:42:23.000000 minvectordb-0.3.4/min_vec/api/high_level.py
--rw-r--r--   0 guobingming   (501) staff       (20)    25069 2024-05-09 02:32:24.000000 minvectordb-0.3.4/min_vec/api/http_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)    14874 2024-05-08 06:54:12.000000 minvectordb-0.3.4/min_vec/api/low_level.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.254313 minvectordb-0.3.4/min_vec/computational_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.3.4/min_vec/computational_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.3.4/min_vec/computational_layer/engines.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.254877 minvectordb-0.3.4/min_vec/configs/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.3.4/min_vec/configs/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2670 2024-05-04 07:03:32.000000 minvectordb-0.3.4/min_vec/configs/config.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3548 2024-05-04 10:58:46.000000 minvectordb-0.3.4/min_vec/configs/parameters_validator.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.257433 minvectordb-0.3.4/min_vec/core_components/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.3.4/min_vec/core_components/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      707 2024-05-04 11:43:20.000000 minvectordb-0.3.4/min_vec/core_components/counter.py
--rw-r--r--   0 guobingming   (501) staff       (20)      501 2024-05-04 11:46:53.000000 minvectordb-0.3.4/min_vec/core_components/cross_lock.py
--rw-r--r--   0 guobingming   (501) staff       (20)     8893 2024-05-08 06:48:31.000000 minvectordb-0.3.4/min_vec/core_components/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1236 2024-05-04 10:58:46.000000 minvectordb-0.3.4/min_vec/core_components/id_checker.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1570 2024-05-04 10:58:46.000000 minvectordb-0.3.4/min_vec/core_components/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1548 2024-05-04 11:43:20.000000 minvectordb-0.3.4/min_vec/core_components/limited_dict.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3294 2024-05-04 11:43:20.000000 minvectordb-0.3.4/min_vec/core_components/limited_sort.py
--rw-r--r--   0 guobingming   (501) staff       (20)    10511 2024-05-08 08:43:01.000000 minvectordb-0.3.4/min_vec/core_components/metadata_kv.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3785 2024-05-04 10:58:46.000000 minvectordb-0.3.4/min_vec/core_components/scaler.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1390 2024-05-04 11:43:20.000000 minvectordb-0.3.4/min_vec/core_components/thread_safe_list.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.258480 minvectordb-0.3.4/min_vec/execution_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.3.4/min_vec/execution_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2679 2024-05-03 07:00:59.000000 minvectordb-0.3.4/min_vec/execution_layer/cluster_worker.py
--rw-r--r--   0 guobingming   (501) staff       (20)    20844 2024-05-08 09:01:11.000000 minvectordb-0.3.4/min_vec/execution_layer/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6743 2024-05-08 06:53:32.000000 minvectordb-0.3.4/min_vec/execution_layer/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)      409 2024-04-26 02:40:02.000000 minvectordb-0.3.4/min_vec/execution_layer/session.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.258793 minvectordb-0.3.4/min_vec/storage_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.3.4/min_vec/storage_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    18716 2024-05-04 11:43:20.000000 minvectordb-0.3.4/min_vec/storage_layer/storage.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.259270 minvectordb-0.3.4/min_vec/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.3.4/min_vec/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4022 2024-05-03 07:43:27.000000 minvectordb-0.3.4/min_vec/utils/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-05-09 03:09:00.262300 minvectordb-0.3.4/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1485 2024-05-09 02:07:57.000000 minvectordb-0.3.4/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.259621 minvectordb-0.3.4/test/
--rw-r--r--   0 guobingming   (501) staff       (20)      315 2024-05-03 07:00:59.000000 minvectordb-0.3.4/test/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.260075 minvectordb-0.3.4/test/docker_tests/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:04:25.000000 minvectordb-0.3.4/test/docker_tests/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3038 2024-05-03 13:31:22.000000 minvectordb-0.3.4/test/docker_tests/test_client_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3029 2024-05-08 06:55:47.000000 minvectordb-0.3.4/test/docker_tests/test_docker_api.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-09 03:09:00.261252 minvectordb-0.3.4/test/standard_tests/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:03:57.000000 minvectordb-0.3.4/test/standard_tests/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1601 2024-04-24 13:16:55.000000 minvectordb-0.3.4/test/standard_tests/test_hmvdb_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)     7588 2024-05-08 06:48:31.000000 minvectordb-0.3.4/test/standard_tests/test_http_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1591 2024-04-23 10:40:50.000000 minvectordb-0.3.4/test/standard_tests/test_smvdb_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)    18258 2024-05-08 06:52:06.000000 minvectordb-0.3.4/test/standard_tests/test_smvdb_save_and_query.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.204750 minvectordb-0.3.5/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.3.5/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.204180 minvectordb-0.3.5/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    16904 2024-05-10 08:59:39.000000 minvectordb-0.3.5/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1740 2024-05-10 08:59:39.000000 minvectordb-0.3.5/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-05-10 08:59:39.000000 minvectordb-0.3.5/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       63 2024-05-10 08:59:39.000000 minvectordb-0.3.5/MinVectorDB.egg-info/entry_points.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.3.5/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      271 2024-05-10 08:59:39.000000 minvectordb-0.3.5/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-05-10 08:59:39.000000 minvectordb-0.3.5/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    16904 2024-05-10 08:59:39.204493 minvectordb-0.3.5/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    15477 2024-05-09 02:55:06.000000 minvectordb-0.3.5/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.193046 minvectordb-0.3.5/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)     1120 2024-05-09 06:25:15.000000 minvectordb-0.3.5/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.193280 minvectordb-0.3.5/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)      273 2024-04-23 05:39:11.000000 minvectordb-0.3.5/min_vec/api/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.194356 minvectordb-0.3.5/min_vec/api/http_api/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-05-09 03:46:14.000000 minvectordb-0.3.5/min_vec/api/http_api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    31907 2024-05-09 05:31:16.000000 minvectordb-0.3.5/min_vec/api/http_api/client_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    25030 2024-05-09 03:47:12.000000 minvectordb-0.3.5/min_vec/api/http_api/http_api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.195247 minvectordb-0.3.5/min_vec/api/native_api/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-05-09 03:46:23.000000 minvectordb-0.3.5/min_vec/api/native_api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    13503 2024-05-09 03:47:12.000000 minvectordb-0.3.5/min_vec/api/native_api/high_level.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    14874 2024-05-09 06:20:30.000000 minvectordb-0.3.5/min_vec/api/native_api/low_level.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.195627 minvectordb-0.3.5/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.3.5/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.3.5/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.196310 minvectordb-0.3.5/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.3.5/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2748 2024-05-09 10:25:01.000000 minvectordb-0.3.5/min_vec/configs/config.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3548 2024-05-04 10:58:46.000000 minvectordb-0.3.5/min_vec/configs/parameters_validator.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.199129 minvectordb-0.3.5/min_vec/core_components/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.3.5/min_vec/core_components/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      707 2024-05-04 11:43:20.000000 minvectordb-0.3.5/min_vec/core_components/counter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      501 2024-05-04 11:46:53.000000 minvectordb-0.3.5/min_vec/core_components/cross_lock.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     9672 2024-05-10 08:48:50.000000 minvectordb-0.3.5/min_vec/core_components/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1236 2024-05-04 10:58:46.000000 minvectordb-0.3.5/min_vec/core_components/id_checker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1570 2024-05-04 10:58:46.000000 minvectordb-0.3.5/min_vec/core_components/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1548 2024-05-04 11:43:20.000000 minvectordb-0.3.5/min_vec/core_components/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3294 2024-05-04 11:43:20.000000 minvectordb-0.3.5/min_vec/core_components/limited_sort.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    10511 2024-05-08 08:43:01.000000 minvectordb-0.3.5/min_vec/core_components/metadata_kv.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3785 2024-05-04 10:58:46.000000 minvectordb-0.3.5/min_vec/core_components/scaler.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1390 2024-05-04 11:43:20.000000 minvectordb-0.3.5/min_vec/core_components/thread_safe_list.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.200592 minvectordb-0.3.5/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.3.5/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2679 2024-05-09 14:59:21.000000 minvectordb-0.3.5/min_vec/execution_layer/cluster_worker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    20844 2024-05-09 14:59:50.000000 minvectordb-0.3.5/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6743 2024-05-09 15:00:19.000000 minvectordb-0.3.5/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      409 2024-04-26 02:40:02.000000 minvectordb-0.3.5/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.200918 minvectordb-0.3.5/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.3.5/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    18758 2024-05-09 15:12:29.000000 minvectordb-0.3.5/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.201409 minvectordb-0.3.5/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.3.5/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4022 2024-05-03 07:43:27.000000 minvectordb-0.3.5/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-05-10 08:59:39.204789 minvectordb-0.3.5/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1494 2024-05-09 06:25:15.000000 minvectordb-0.3.5/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.201765 minvectordb-0.3.5/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)      346 2024-05-09 05:31:25.000000 minvectordb-0.3.5/test/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.202437 minvectordb-0.3.5/test/docker_tests/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:04:25.000000 minvectordb-0.3.5/test/docker_tests/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2973 2024-05-10 08:52:36.000000 minvectordb-0.3.5/test/docker_tests/test_client_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3029 2024-05-08 06:55:47.000000 minvectordb-0.3.5/test/docker_tests/test_docker_api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-10 08:59:39.203719 minvectordb-0.3.5/test/standard_tests/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:03:57.000000 minvectordb-0.3.5/test/standard_tests/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1601 2024-04-24 13:16:55.000000 minvectordb-0.3.5/test/standard_tests/test_hmvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     7606 2024-05-09 05:31:25.000000 minvectordb-0.3.5/test/standard_tests/test_http_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1591 2024-04-23 10:40:50.000000 minvectordb-0.3.5/test/standard_tests/test_smvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    19027 2024-05-10 08:56:34.000000 minvectordb-0.3.5/test/standard_tests/test_smvdb_save_and_query.py
```

### Comparing `minvectordb-0.3.4/LICENSE` & `minvectordb-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/MinVectorDB.egg-info/PKG-INFO` & `minvectordb-0.3.5/MinVectorDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.3.4
+Version: 0.3.5
 Summary: A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,15 @@
 Requires-Dist: flask>=2.0.1
 Requires-Dist: PyYAML>=5.4.1
 Requires-Dist: waitress>=2.0.0
 Requires-Dist: pytest>=7.4.4
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: httpx[http2]>=0.19.0
+Requires-Dist: pandas>=1.3.3
 
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.4 Summary: A pure Python-
+Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.5 Summary: A pure Python-
 implemented, lightweight, server-optional, multi-end compatible, vector
 database deployable locally or remotely. Home-page: https://github.com/
 BirchKwok/MinVectorDB Author: Birch Kwok Author-email: birchkwok@gmail.com
 Keywords: vector database Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development Classifier: Topic :: Scientific/Engineering Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
@@ -12,15 +12,16 @@
 Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: numpy>=1.17.0 Requires-Dist: spinesUtils>=0.3.13 Requires-Dist:
 msgpack>=1.0.2 Requires-Dist: scikit-learn>=1.0.0 Requires-Dist:
 cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
 pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: jaxlib>=0.4.25
 Requires-Dist: flask>=2.0.1 Requires-Dist: PyYAML>=5.4.1 Requires-Dist:
 waitress>=2.0.0 Requires-Dist: pytest>=7.4.4 Requires-Dist: tqdm>=4.62.3
-Requires-Dist: setuptools>=68.0.0 Requires-Dist: httpx[http2]>=0.19.0
+Requires-Dist: setuptools>=68.0.0 Requires-Dist: httpx[http2]>=0.19.0 Requires-
+Dist: pandas>=1.3.3
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
     ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
        ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
  _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _t_e_s_t_i_n_g_]_[_D_o_c_k_e_r
                                     _b_u_i_l_d_]
 â¡ **Server-optional, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
```

### Comparing `minvectordb-0.3.4/MinVectorDB.egg-info/SOURCES.txt` & `minvectordb-0.3.5/MinVectorDB.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 MinVectorDB.egg-info/dependency_links.txt
 MinVectorDB.egg-info/entry_points.txt
 MinVectorDB.egg-info/not-zip-safe
 MinVectorDB.egg-info/requires.txt
 MinVectorDB.egg-info/top_level.txt
 min_vec/__init__.py
 min_vec/api/__init__.py
-min_vec/api/client_api.py
-min_vec/api/high_level.py
-min_vec/api/http_api.py
-min_vec/api/low_level.py
+min_vec/api/http_api/__init__.py
+min_vec/api/http_api/client_api.py
+min_vec/api/http_api/http_api.py
+min_vec/api/native_api/__init__.py
+min_vec/api/native_api/high_level.py
+min_vec/api/native_api/low_level.py
 min_vec/computational_layer/__init__.py
 min_vec/computational_layer/engines.py
 min_vec/configs/__init__.py
 min_vec/configs/config.py
 min_vec/configs/parameters_validator.py
 min_vec/core_components/__init__.py
 min_vec/core_components/counter.py
```

### Comparing `minvectordb-0.3.4/PKG-INFO` & `minvectordb-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.3.4
+Version: 0.3.5
 Summary: A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,15 @@
 Requires-Dist: flask>=2.0.1
 Requires-Dist: PyYAML>=5.4.1
 Requires-Dist: waitress>=2.0.0
 Requires-Dist: pytest>=7.4.4
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: httpx[http2]>=0.19.0
+Requires-Dist: pandas>=1.3.3
 
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.4 Summary: A pure Python-
+Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.5 Summary: A pure Python-
 implemented, lightweight, server-optional, multi-end compatible, vector
 database deployable locally or remotely. Home-page: https://github.com/
 BirchKwok/MinVectorDB Author: Birch Kwok Author-email: birchkwok@gmail.com
 Keywords: vector database Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development Classifier: Topic :: Scientific/Engineering Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
@@ -12,15 +12,16 @@
 Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: numpy>=1.17.0 Requires-Dist: spinesUtils>=0.3.13 Requires-Dist:
 msgpack>=1.0.2 Requires-Dist: scikit-learn>=1.0.0 Requires-Dist:
 cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
 pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: jaxlib>=0.4.25
 Requires-Dist: flask>=2.0.1 Requires-Dist: PyYAML>=5.4.1 Requires-Dist:
 waitress>=2.0.0 Requires-Dist: pytest>=7.4.4 Requires-Dist: tqdm>=4.62.3
-Requires-Dist: setuptools>=68.0.0 Requires-Dist: httpx[http2]>=0.19.0
+Requires-Dist: setuptools>=68.0.0 Requires-Dist: httpx[http2]>=0.19.0 Requires-
+Dist: pandas>=1.3.3
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
     ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
        ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
  _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _t_e_s_t_i_n_g_]_[_D_o_c_k_e_r
                                     _b_u_i_l_d_]
 â¡ **Server-optional, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
```

### Comparing `minvectordb-0.3.4/README.md` & `minvectordb-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/__init__.py` & `minvectordb-0.3.5/min_vec/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = '0.3.4'
+__version__ = '0.3.5'
 
 
 class MinVectorDB:
     """
     Create a MinVectorDB instance.
 
     Parameters:
@@ -16,16 +16,16 @@
             otherwise return a MinVectorDBHTTPClient instance.
     """
     from pathlib import Path
     from typing import Union
 
     def __new__(cls, root_path: Union[str, Path]):
         from pathlib import Path
-        from min_vec.api.high_level import MinVectorDBLocalClient
-        from min_vec.api.client_api import MinVectorDBHTTPClient
+        from min_vec.api.native_api.high_level import MinVectorDBLocalClient
+        from min_vec.api.http_api.client_api import MinVectorDBHTTPClient
 
         if isinstance(root_path, Path):
             root_path = root_path.as_posix()
 
         if root_path.startswith('http://') or root_path.startswith('https://'):
             instance = MinVectorDBHTTPClient(url=root_path)
         else:
```

### Comparing `minvectordb-0.3.4/min_vec/api/client_api.py` & `minvectordb-0.3.5/min_vec/api/http_api/client_api.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/api/high_level.py` & `minvectordb-0.3.5/min_vec/api/native_api/high_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import partial
 from pathlib import Path
 from typing import Union
 
 import pandas as pd
 from spinesUtils.asserts import ParameterTypeAssert
 
-from min_vec.api.low_level import StandaloneMinVectorDB
+from min_vec.api.native_api.low_level import StandaloneMinVectorDB
 from min_vec.api import logger
 from min_vec.utils.utils import unavailable_if_deleted
 
 
 class _Register:
     """
     A class for registering the collections to local database path.
```

### Comparing `minvectordb-0.3.4/min_vec/api/http_api.py` & `minvectordb-0.3.5/min_vec/api/http_api/http_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import msgpack
 import yaml
 
 from flask import Flask, request, jsonify, Response
 from waitress import serve
 
-from min_vec.api.high_level import MinVectorDBLocalClient
-from min_vec.core_components.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
+from min_vec.api.native_api.high_level import MinVectorDBLocalClient
+from min_vec.core_components.filter import Filter
 from min_vec.core_components.limited_dict import LimitedDict
 
 app = Flask(__name__)
 
 
 data_dict = LimitedDict(max_size=1000)
```

### Comparing `minvectordb-0.3.4/min_vec/api/low_level.py` & `minvectordb-0.3.5/min_vec/api/native_api/low_level.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/computational_layer/engines.py` & `minvectordb-0.3.5/min_vec/computational_layer/engines.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/configs/config.py` & `minvectordb-0.3.5/min_vec/configs/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
     @property
     def MVDB_QUERY_CACHE_SIZE(self):
         return self.get_env_variable('MVDB_QUERY_CACHE_SIZE', 10000, int, [int])
 
     @property
     def MVDB_DATALOADER_BUFFER_SIZE(self):
-        return self.get_env_variable('MVDB_DATALOADER_BUFFER_SIZE', 20, int, [int, None])
+        size = self.get_env_variable('MVDB_DATALOADER_BUFFER_SIZE', 20, int, [int, None])
+        if size is None or size < 1:
+            return 1
+        return size
 
     @property
     def MVDB_DELAY_NUM(self):
         return self.get_env_variable('MVDB_DELAY_NUM', 1000, int, [int])
 
     def get_all_configs(self):
         return {
```

### Comparing `minvectordb-0.3.4/min_vec/configs/parameters_validator.py` & `minvectordb-0.3.5/min_vec/configs/parameters_validator.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/counter.py` & `minvectordb-0.3.5/min_vec/core_components/counter.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/filter.py` & `minvectordb-0.3.5/min_vec/core_components/filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,47 @@
 from typing import Union
 
 import numpy as np
 from spinesUtils.asserts import raise_if
 
 
 class MatchField:
-    def __init__(self, value, comparator=operator.eq):
+    def __init__(self, value, comparator=operator.eq, all_comparators=False):
         """
         Initialize a MatchField instance with a specific value and comparator.
             .. versionadded:: 0.3.0
 
         Parameters:
-            value: The value to compare the data attribute with.
+            value (list or tuple or any object that implements comparison functions such as __ eq__): The value to compare the data attribute with.
             comparator: The comparator function to apply to the data attribute.
+            all_comparators: Whether to apply the comparator to all values in the list or tuple.
+                If True, all values in the list or tuple must satisfy the comparison condition.
+                If False, at least one value in the list or tuple must satisfy the comparison condition.
+                    .. versionadded:: 0.3.5
         """
         self.value = value
         self.comparator = comparator
+        self.all_comparators = all_comparators
 
     def match(self, data_value):
         """
         Apply the comparator to compare the data attribute with the specified value.
 
         Parameters:
             data_value: The value of the data attribute to compare.
 
         Returns:
             bool: True if the data attribute matches the specified value, otherwise False.
         """
+        if isinstance(self.value, (list, tuple)):
+            if self.all_comparators:
+                return all([self.comparator(data_value, value) for value in self.value])
+            else:
+                return any([self.comparator(data_value, value) for value in self.value])
+
         return self.comparator(data_value, self.value)
 
 
 class FieldCondition:
     def __init__(self, key, matcher):
         """
         Initialize a FieldCondition instance with a specific key and matcher.
```

### Comparing `minvectordb-0.3.4/min_vec/core_components/id_checker.py` & `minvectordb-0.3.5/min_vec/core_components/id_checker.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/kmeans.py` & `minvectordb-0.3.5/min_vec/core_components/kmeans.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/limited_dict.py` & `minvectordb-0.3.5/min_vec/core_components/limited_dict.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/limited_sort.py` & `minvectordb-0.3.5/min_vec/core_components/limited_sort.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/metadata_kv.py` & `minvectordb-0.3.5/min_vec/core_components/metadata_kv.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/scaler.py` & `minvectordb-0.3.5/min_vec/core_components/scaler.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/core_components/thread_safe_list.py` & `minvectordb-0.3.5/min_vec/core_components/thread_safe_list.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/execution_layer/cluster_worker.py` & `minvectordb-0.3.5/min_vec/execution_layer/cluster_worker.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/execution_layer/matrix_serializer.py` & `minvectordb-0.3.5/min_vec/execution_layer/matrix_serializer.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/execution_layer/query.py` & `minvectordb-0.3.5/min_vec/execution_layer/query.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/min_vec/storage_layer/storage.py` & `minvectordb-0.3.5/min_vec/storage_layer/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,22 +98,17 @@
         for path in [self.collection_chunk_path, self.collection_chunk_indices_path,
                      self.collection_cluster_path, self.collection_cluster_indices_path]:
             path.mkdir(parents=True, exist_ok=True)
 
         self.dimension = dimension
         self.chunk_size = chunk_size
 
-        self.tempfile_storage = TemporaryFileStorage(chunk_size)
-
         self.cluster_last_file_shape = {}
-
         self.cache = LimitedDict(max_size=config.MVDB_DATALOADER_BUFFER_SIZE)
-
         self.quantizer = None
-
         self.lock = ThreadLock()
 
         if warm_up:
             self.warm_up()
 
     def update_quantizer(self, quantizer):
         with self.lock:
@@ -127,17 +122,17 @@
     def warm_up(self):
         """Load the data from the file to the memory."""
         if not self.file_exists():
             return
 
         filenames = self.get_all_files(read_type='all')
 
-        for filename in filenames:
-            data, indices = self.read(filename)
-            data, indices = self.read(filename)
+        for idx, filename in enumerate(filenames):
+            if idx + 1 <= config.MVDB_DATALOADER_BUFFER_SIZE:
+                data, indices = self.read(filename, filenames)
 
     def _return_if_in_memory(self, filename):
         res = self.cache.get(filename, None)
 
         if res is None:
             return None
 
@@ -171,14 +166,15 @@
             filenames = self.get_all_files('chunk') + self.get_all_files('cluster', None)
         else:
             raise ValueError('read_type must be "chunk" or "cluster" or "all"')
 
         return filenames
 
     def _read(self, filename):
+        """Read data from the specified filename if it exists."""
         if not self.file_exists():
             return
 
         if 'chunk' in filename:
             data_path = self.collection_chunk_path
             indices_path = self.collection_chunk_indices_path
         else:
```

### Comparing `minvectordb-0.3.4/min_vec/utils/utils.py` & `minvectordb-0.3.5/min_vec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/setup.py` & `minvectordb-0.3.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 reqs = read_requirements(Path('.').parent.joinpath("requirements.txt"))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.3.4",
+    version="0.3.5",
     description='A pure Python-implemented, lightweight, server-optional, '
                 'multi-end compatible, vector database deployable locally or remotely.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
@@ -37,11 +37,11 @@
     url='https://github.com/BirchKwok/MinVectorDB',
     author='Birch Kwok',
     author_email='birchkwok@gmail.com',
     install_requires=reqs,
     zip_safe=False,
     entry_points={
         'console_scripts': [
-            'min_vec=min_vec.api.http_api:main',
+            'min_vec=min_vec.api.http_api.http_api:main',
         ],
     },
 )
```

### Comparing `minvectordb-0.3.4/test/docker_tests/test_client_api.py` & `minvectordb-0.3.5/test/docker_tests/test_client_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import concurrent.futures
 
-import pytest
-
 from test import MinVectorDB, MinVectorDBHTTPClient
-from min_vec.api.client_api import ExecutionError
 
 
 def test_initialization():
     db = MinVectorDB('http://localhost:7637')
 
     assert isinstance(db, MinVectorDBHTTPClient)
```

### Comparing `minvectordb-0.3.4/test/docker_tests/test_docker_api.py` & `minvectordb-0.3.5/test/docker_tests/test_docker_api.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/test/standard_tests/test_hmvdb_initial.py` & `minvectordb-0.3.5/test/standard_tests/test_hmvdb_initial.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/test/standard_tests/test_http_api.py` & `minvectordb-0.3.5/test/standard_tests/test_http_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
-from min_vec.api.http_api import app
-from min_vec.api.client_api import pack_data
+from min_vec.api.http_api.http_api import app
+from min_vec.api.http_api.client_api import pack_data
 
 
 @pytest.fixture()
 def test_client():
     app.config.update({
         "TESTING": True,
     })
```

### Comparing `minvectordb-0.3.4/test/standard_tests/test_smvdb_initial.py` & `minvectordb-0.3.5/test/standard_tests/test_smvdb_initial.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.4/test/standard_tests/test_smvdb_save_and_query.py` & `minvectordb-0.3.5/test/standard_tests/test_smvdb_save_and_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,7 +617,34 @@
         ]
     ))
 
     assert len(n) == len(d) == 5
     assert list(d) == sorted(d, key=lambda s: -s)
     assert all(i in database._id_filter for i in n)
     assert all(0 <= i < 6 for i in n)
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+        must=[
+            FieldCondition(key='test', matcher=MatchField(['test_0', 'test_00'], all_comparators=True)),
+        ],
+        any=[
+            IDCondition(MatchID([1, 2, 3, 4, 5])),
+        ]
+    ))
+
+    assert len(n) == len(d) == 0
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+        must=[
+            FieldCondition(key='test', matcher=MatchField(['test_0', 'test_00'], all_comparators=False)),
+        ],
+        any=[
+            IDCondition(MatchID([1, 2, 3, 4, 5])),
+        ]
+    ))
+
+    assert len(n) == len(d) == 5
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(0 <= i < 6 for i in n)
```

