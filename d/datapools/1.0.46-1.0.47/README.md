# Comparing `tmp/datapools-1.0.46.tar.gz` & `tmp/datapools-1.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.46.tar", last modified: Wed May  8 15:41:37 2024, max compression
+gzip compressed data, was "datapools-1.0.47.tar", last modified: Fri May 10 11:15:49 2024, max compression
```

## Comparing `datapools-1.0.46.tar` & `datapools-1.0.47.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.172133 datapools-1.0.46/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 15:41:28.000000 datapools-1.0.46/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-05-08 15:41:28.000000 datapools-1.0.46/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-08 15:41:28.000000 datapools-1.0.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 15:41:28.000000 datapools-1.0.46/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 15:41:37.172133 datapools-1.0.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-08 15:41:28.000000 datapools-1.0.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.152133 datapools-1.0.46/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:41:37.172133 datapools-1.0.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-08 15:41:28.000000 datapools-1.0.46/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:28.000000 datapools-1.0.46/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-08 15:41:28.000000 datapools-1.0.46/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-08 15:41:28.000000 datapools-1.0.46/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.179207 datapools-1.0.47/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 11:15:37.000000 datapools-1.0.47/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-10 11:15:37.000000 datapools-1.0.47/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-10 11:15:37.000000 datapools-1.0.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 11:15:37.000000 datapools-1.0.47/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-10 11:15:49.179207 datapools-1.0.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 11:15:37.000000 datapools-1.0.47/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.167207 datapools-1.0.47/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.167207 datapools-1.0.47/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.171207 datapools-1.0.47/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.175207 datapools-1.0.47/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.175207 datapools-1.0.47/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.175207 datapools-1.0.47/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.175207 datapools-1.0.47/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.175207 datapools-1.0.47/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.175207 datapools-1.0.47/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.175207 datapools-1.0.47/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.179207 datapools-1.0.47/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.179207 datapools-1.0.47/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.179207 datapools-1.0.47/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-10 11:15:37.000000 datapools-1.0.47/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.179207 datapools-1.0.47/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-10 11:15:49.000000 datapools-1.0.47/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-10 11:15:49.000000 datapools-1.0.47/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:15:49.000000 datapools-1.0.47/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 11:15:49.000000 datapools-1.0.47/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 11:15:49.000000 datapools-1.0.47/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 11:15:49.000000 datapools-1.0.47/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:15:49.179207 datapools-1.0.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 11:15:37.000000 datapools-1.0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:49.179207 datapools-1.0.47/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:15:37.000000 datapools-1.0.47/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-10 11:15:37.000000 datapools-1.0.47/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-10 11:15:37.000000 datapools-1.0.47/tests/test_base.py
```

### Comparing `datapools-1.0.46/HISTORY.md` & `datapools-1.0.47/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Linter. [sergpsu]
+- Google_drive supports structure rules. [sergpsu]
+
+
+1.0.46 (2024-05-08)
+-------------------
+- Release: version 1.0.46 🚀 [sergpsu]
 - Merge pull request #64 from torrentsai/sergpsu-fixes. [S]
 
   Freesound.org
 - Env keys. [sergpsu]
 - Freesound.org plugin. [sergpsu]
```

### Comparing `datapools-1.0.46/LICENSE` & `datapools-1.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/PKG-INFO` & `datapools-1.0.47/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.46
+Version: 1.0.47
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.46/README.md` & `datapools-1.0.47/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/api.py` & `datapools-1.0.47/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/cli.py` & `datapools-1.0.47/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/backend_api.py` & `datapools-1.0.47/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/queues/__init__.py` & `datapools-1.0.47/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/queues/rabbitmq.py` & `datapools-1.0.47/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/queues/types.py` & `datapools-1.0.47/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/session_manager.py` & `datapools-1.0.47/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/stoppable.py` & `datapools-1.0.47/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/storage/base_storage.py` & `datapools-1.0.47/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/storage/file_storage.py` & `datapools-1.0.47/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.47/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.47/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/common/types.py` & `datapools-1.0.47/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/producer/base_producer.py` & `datapools-1.0.47/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/scheduler/scheduler.py` & `datapools-1.0.47/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.47/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.47/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/default/default.py` & `datapools-1.0.47/datapools/worker/plugins/default/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,16 @@
                 new_n_hrefs = len(hrefs)
                 if new_n_hrefs != n_hrefs:
                     expect_changes = True
                 while n_hrefs < new_n_hrefs:
                     try:
                         href = await hrefs[n_hrefs].get_attribute("href", timeout=100)
                         n_hrefs += 1
+                        if href is None:
+                            continue
 
                         full_local_url = BasePlugin.get_local_url(href, session_meta["url"])
                         if full_local_url:
                             # strict constraint on urls, else may get endless recursions etc
                             full_local_url = canonicalize_url(full_local_url)
                             logger.info(full_local_url)
```

### Comparing `datapools-1.0.46/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.47/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.47/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
                 copyright_owner_tag = None
                 date = None
 
                 # looking for the owner page link
                 links = await sound.locator("a").all()
                 for link in links:
                     href = await link.get_attribute("href")
+                    if href is None:
+                        continue
                     href_parts = href.split("/")  # expecting "/people/username/" structure
                     if (
                         len(href_parts) == 4
                         and href_parts[0] == ""
                         and href_parts[1] == "people"
                         and href_parts[3] == ""
                     ):
@@ -100,27 +102,27 @@
 
                 if platform_tag is None and copyright_owner_tag is None:
                     logger.info("no tag available")
                     continue
 
                 # searching for date div
                 date_div = sound.locator(".text-light-grey.h-spacing-left-1.d-none.d-lg-block.no-text-wrap").first
-                date = await date_div.text_content()
-                logger.info(f"{date=}")
-                if date is None:
+                raw_date = await date_div.text_content()
+                logger.info(f"{raw_date=}")
+                if raw_date is None:
                     logger.error("date not found")
                     continue
 
                 # expect date in "April 8th, 2024" format
                 # removing "rd," or "th," => "April 8 2024"
-                date = date.replace("rd,", "").replace("th,", "")
+                raw_date = raw_date.replace("rd,", "").replace("th,", "")
                 try:
-                    date = int(datetime.timestamp(datetime.strptime(date, "%B %d %Y")))
+                    date = int(datetime.timestamp(datetime.strptime(raw_date, "%B %d %Y")))
                 except ValueError:
-                    logger.error(f"Unexpected date format {date=}")
+                    logger.error(f"Unexpected date format {raw_date=}")
                     continue
 
                 # downloading audio content
                 player = sound.locator(".bw-player").first
                 mp3_url = await player.get_attribute("data-mp3")  # TODO: also ogg available as "data-ogg"
 
                 full_mp3_url = BasePlugin.get_local_url(mp3_url, session_meta["url"])
```

### Comparing `datapools-1.0.46/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.47/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 import os
 
 # import asyncio
 # import io
 import traceback
-from typing import Optional
+from typing import Optional, List
 
 from google.auth.api_key import Credentials
 
 # from google.auth.transport.requests import Request
 # from google.oauth2.credentials import Credentials
 # from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import CrawlerContent, DatapoolContentType
+from ....common.types import CrawlerContent, DatapoolContentType, CrawlerDemoUser
 from ..base_plugin import BasePlugin, BasePluginException, WorkerTask, BaseTag
 
 # from googleapiclient.http import MediaIoBaseDownload
 
 
 # from googleapiclient.errors import HttpError
 
 
 # If modifying these scopes, delete the file token.json.
 # SCOPES = ['https://www.googleapis.com/auth/drive.metadata.readonly']
 
+PARSING_RULES_FILENAME = "FILES_STRUCTURE.txt"
+RULE_ANY_PART = "*"
+RULE_USER_PART = "{user}"
+
 
 class GoogleDrivePlugin(BasePlugin):
     tag_id: Optional[BaseTag] = None
+    rules: List[str]
+    demo_mode: bool
 
-    def __init__(self, ctx, api_key=None):
+    def __init__(self, ctx, demo_mode=False, api_key=None):
         super().__init__(ctx)
         if not api_key:
             api_key = os.environ.get("GOOGLE_DRIVE_API_KEY")
         self.creds = Credentials(api_key)
+        self.demo_mode = demo_mode
 
     # https://drive.google.com/drive/folders/1CPDmula2V83KWOocJR9jVvsTk6tVSpKd?usp=sharing
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
         if u.netloc == "drive.google.com":
@@ -51,120 +58,133 @@
         u = self.parse_url(task.url)
         folder_id = u.path.split("/")[3]
 
         try:
             with build("drive", "v3", credentials=self.creds) as drive:
                 self.tag_id = await self.find_license(folder_id, drive)
                 if self.tag_id:
+                    self.rules = await self.find_parsing_rules(folder_id, drive)
+                    logger.info(f"{self.rules=}")
+
                     async for msg in self.scan_folder(folder_id, drive):
                         yield msg
         except Exception as e:
             logger.error(f"GoogleDrivePlugin exception {e}")
             logger.error(traceback.format_exc())
 
     def _get_download_url(self, file_id):
         # this url can be placed on site for preview
         return f"https://drive.google.com/uc?id={file_id}"
 
         # return f"https://www.googleapis.com/drive/v3/files/{file_id}?alt=media&key={self.creds.token}"
 
     async def find_license(self, folder_id, drive):
         try:
-            license = (
+            files_res = (
                 drive.files()
                 .list(
                     q=f"name='{BasePlugin.license_filename}' and '{folder_id}' in parents",
                     pageSize=1,
                     fields="files(id)",
                 )
                 .execute()
             )
-            file_id = license.get("files")[0]["id"]
+            file_id = files_res.get("files")[0]["id"]
 
             url = self._get_download_url(file_id)
-            # headers = { "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
-            #             "Accept-Encoding":"gzip, deflate, br",
-            #             "Accept-Language":"en-US,en;q=0.5",
-            #             "Connection":"keep-alive",
-            #             "Sec-Fetch-Dest":"document",
-            #             "Sec-Fetch-Mode":"navigate",
-            #             "Sec-Fetch-Site":"none",
-            #             "Sec-Fetch-User":"?1",
-            #             "TE":"trailers",
-            #             "Upgrade-Insecure-Requests":"1",
-            #             "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/118.0"
-            # }
             headers = {}
             tag_id = await self.download(url, headers)
             logger.info(f"download {tag_id=}")
             tag_id = await BasePlugin.parse_tag_in(tag_id.decode())
             logger.info(f"{tag_id=}")
             return tag_id
 
-            # file = drive.files().get( fileId=file_id ).execute()
+        except Exception:
+            pass
 
-            # logger.info( f'downloading file {file_id} {file["name"]}')
-            # fileRequest = drive.files().get_media(fileId=file_id)
-            # fh = io.BytesIO()
-            # downloader = MediaIoBaseDownload(fh, fileRequest)
-            # done = False
-            # while done is False:
-            #     status, done = downloader.next_chunk()
-            # fh.seek(0)
-            # tag_id = fh.read().strip()
-            # tag_id = await BasePlugin.parse_tag_in(tag_id)
+    async def find_parsing_rules(self, folder_id, drive):
+        try:
+            files_res = (
+                drive.files()
+                .list(
+                    q=f"name='{PARSING_RULES_FILENAME}' and '{folder_id}' in parents",
+                    pageSize=1,
+                    fields="files(id)",
+                )
+                .execute()
+            )
+            file_id = files_res.get("files")[0]["id"]
 
-            # logger.info( f'{tag_id=}')
+            url = self._get_download_url(file_id)
+            headers = {}
+            rules = await self.download(url, headers)
+            rules = rules.decode()
+            logger.info(f"downloaded {rules=}")
+
+            res = []
+            for rule in rules.split("\n"):
+                rule = rule.strip()
+                if rule:
+                    rule_parts = rule.split("/")
+                    for i in range(0, len(rule_parts)):
+                        part = rule_parts[i]
+                        if part == RULE_ANY_PART or part == RULE_USER_PART or (part == "" and i == 0):
+                            pass
+                        else:
+                            raise Exception(f"Invalid rule {rule_parts=}")
+                    res.append(rule_parts)
+            return res
 
-            # return tag_id
         except Exception:
             pass
 
-    async def scan_folder(self, folder_id, drive):
+    async def scan_folder(self, folder_id, drive, parent_path="/"):
         logger.info(f"scanning folder {folder_id}")
         # print(folder_id)
         # this gives us a list of all folders with that name
         # folder = drive.files().get( fileId=folder_id ).execute()
         # print(type(folder))
 
         page_token = None
         while True:
             results = (
                 drive.files()
                 .list(
                     q="'" + folder_id + "' in parents",
-                    pageSize=10,
+                    pageSize=100,
                     pageToken=page_token,
-                    fields="nextPageToken, files(id, name)",
+                    fields="nextPageToken, files(id, name, mimeType)",
                 )
                 .execute()
             )
             items = results.get("files", [])
+
             page_token = results.get("nextPageToken", None)
 
-            # Now we can loop through each file in that folder, and do whatever (in this case, download them and open them as images in OpenCV)
-            for f in range(0, len(items)):
-                # print( items[f])
+            for item in items:
+                # logger.info(f"{item=}")
 
-                file_id = items[f].get("id")
-                logger.info(f"{file_id=}")
+                if parent_path == "/" and (
+                    item["name"] == BasePlugin.license_filename or item["name"] == PARSING_RULES_FILENAME
+                ):
+                    continue
 
-                file = drive.files().get(fileId=file_id).execute()
-                logger.info(f"{file['mimeType']=}")
+                file_id = item["id"]
+                logger.info(f"{file_id=}")
 
-                if file["mimeType"] == "application/vnd.google-apps.folder":
-                    async for yielded in self.scan_folder(file_id, drive):
+                if item["mimeType"] == "application/vnd.google-apps.folder":
+                    async for yielded in self.scan_folder(file_id, drive, f'{parent_path}{item["name"]}/'):
                         yield yielded
                 else:
                     try:
-                        datapool_content_type = BasePlugin.get_content_type_by_mime_type(file["mimeType"])
+                        datapool_content_type = BasePlugin.get_content_type_by_mime_type(item["mimeType"])
                     except BasePluginException:
-                        logger.error(f'Not supported mime type {file["mimeType"]}')
+                        logger.error(f'Not supported mime type {item["mimeType"]}')
 
-                    logger.info(f'downloading file {file_id} {file["name"]}')
+                    logger.info(f'downloading file {file_id} {item["name"]}')
                     # TODO: this works too, but is getting blocked  when running from lsrv2
                     # fileRequest = drive.files().get_media(fileId=file_id)
                     # fh = io.BytesIO()
                     # downloader = MediaIoBaseDownload(fh, fileRequest)
                     # done = False
                     # while done is False:
                     #     status, done = downloader.next_chunk()
@@ -172,29 +192,59 @@
                     # content = fh.read()
                     # direct url seems to work better than API access
                     url = self._get_download_url(file_id)
                     content = await self.download(url)
                     if content is not None:
                         logger.info(f"file size={len(content)}")
 
-                        image_tag = None
+                        if self.demo_mode:
+                            path = f"{parent_path}{item['name']}"
+                            logger.info(f"{path=}")
+
+                            # if file full path matches any structural rule, then trying to create demo user from the match info
+                            match = self._match_structure_rules(path)
+                            if match and "user" in match:
+                                short_tag_id = BasePlugin.gen_demo_tag(match["user"])
+                                yield CrawlerDemoUser(
+                                    user_name=match["user"], short_tag_id=short_tag_id, platform="drive.google.com"
+                                )
+
+                        author_tag = None
                         if datapool_content_type == DatapoolContentType.Image:
-                            image_tag = BasePlugin.parse_image_tag(content)
+                            author_tag = BasePlugin.parse_image_tag(content)
 
                         # obj_url = f'https://drive.google.com/file/d/{file_id}/view'
                         obj_url = url
                         storage_id = BaseStorage.gen_id(obj_url)
                         await self.ctx.storage.put(storage_id, content)
 
                         yield CrawlerContent(
-                            tag_id=str(image_tag) if image_tag is not None else None,
-                            tag_keepout=image_tag.is_keepout() if image_tag is not None else None,
+                            tag_id=str(author_tag) if author_tag is not None else None,
+                            tag_keepout=author_tag.is_keepout() if author_tag is not None else None,
                             copyright_tag_id=str(self.tag_id),
                             copyright_tag_keepout=self.tag_id.is_keepout(),
                             type=datapool_content_type,
                             storage_id=storage_id,
                             url=obj_url,
                         )
 
                 # baseImage = cv2.imdecode(np.fromstring(fhContents, dtype=np.uint8), cv2.IMREAD_COLOR)
             if page_token is None:
                 break
+
+    def _match_structure_rules(self, path):
+        # self.rules is [
+        #     ["*" | "{user}"...],
+        #     ["*" | "{user}"...],
+        # ]
+        if self.rules is not None:
+            path_parts = path.split("/")
+            n = len(path_parts)
+            for rule_parts in self.rules:
+                if len(rule_parts) != n:
+                    continue
+
+                res = {}
+                for i in range(0, n):
+                    if rule_parts[i] == RULE_USER_PART:
+                        res["user"] = path_parts[i]
+                return res
```

### Comparing `datapools-1.0.46/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.47/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.47/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.47/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.47/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.47/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.47/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools/worker/worker.py` & `datapools-1.0.47/datapools/worker/worker.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/datapools.egg-info/PKG-INFO` & `datapools-1.0.47/datapools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.46
+Version: 1.0.47
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.46/datapools.egg-info/SOURCES.txt` & `datapools-1.0.47/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/setup.py` & `datapools-1.0.47/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.46/tests/test_base.py` & `datapools-1.0.47/tests/test_base.py`

 * *Files identical despite different names*

