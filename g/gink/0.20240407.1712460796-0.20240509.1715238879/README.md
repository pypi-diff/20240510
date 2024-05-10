# Comparing `tmp/gink-0.20240407.1712460796.tar.gz` & `tmp/gink-0.20240509.1715238879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240407.1712460796.tar", last modified: Sun Apr  7 03:33:20 2024, max compression
+gzip compressed data, was "gink-0.20240509.1715238879.tar", last modified: Thu May  9 07:14:42 2024, max compression
```

## Comparing `gink-0.20240407.1712460796.tar` & `gink-0.20240509.1715238879.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:20.165326 gink-0.20240407.1712460796/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-07 03:33:20.165326 gink-0.20240407.1712460796/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:20.149326 gink-0.20240407.1712460796/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:20.153326 gink-0.20240407.1712460796/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:20.157326 gink-0.20240407.1712460796/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18082 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    56470 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/impl/websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:20.161326 gink-0.20240407.1712460796/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10202 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-07 03:33:14.000000 gink-0.20240407.1712460796/gink/tests/test_websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:33:20.161326 gink-0.20240407.1712460796/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-07 03:33:20.000000 gink-0.20240407.1712460796/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-07 03:33:20.000000 gink-0.20240407.1712460796/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:33:20.000000 gink-0.20240407.1712460796/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-07 03:33:20.000000 gink-0.20240407.1712460796/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 03:33:20.000000 gink-0.20240407.1712460796/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:33:20.165326 gink-0.20240407.1712460796/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-07 03:33:16.000000 gink-0.20240407.1712460796/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:42.882508 gink-0.20240509.1715238879/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-05-09 07:14:42.882508 gink-0.20240509.1715238879/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:42.866508 gink-0.20240509.1715238879/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:42.870508 gink-0.20240509.1715238879/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:42.878508 gink-0.20240509.1715238879/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18082 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56473 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/impl/websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:42.882508 gink-0.20240509.1715238879/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-09 07:14:37.000000 gink-0.20240509.1715238879/gink/tests/test_websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:14:42.882508 gink-0.20240509.1715238879/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-05-09 07:14:42.000000 gink-0.20240509.1715238879/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-09 07:14:42.000000 gink-0.20240509.1715238879/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:14:42.000000 gink-0.20240509.1715238879/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 07:14:42.000000 gink-0.20240509.1715238879/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 07:14:42.000000 gink-0.20240509.1715238879/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:14:42.882508 gink-0.20240509.1715238879/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-09 07:14:39.000000 gink-0.20240509.1715238879/setup.py
```

### Comparing `gink-0.20240407.1712460796/LICENSE` & `gink-0.20240509.1715238879/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/PKG-INFO` & `gink-0.20240509.1715238879/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240407.1712460796
+Version: 0.20240509.1715238879
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240407.1712460796/README.md` & `gink-0.20240509.1715238879/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/__init__.py` & `gink-0.20240509.1715238879/gink/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from .impl.sequence import Sequence
 from .impl.box import Box
 from .impl.property import Property
 from .impl.container import Container
 from .impl.muid import Muid
 from .impl.bundle_info import BundleInfo
 from .impl.bundler import Bundler
-from .impl.role import Role
+from .impl.group import Group
 from .impl.key_set import KeySet
 from .impl.graph import Vertex, Verb, Edge
 from .impl.pair_set import PairSet
 from .impl.pair_map import PairMap
 from .impl.utilities import generate_timestamp
 from .impl.builders import ClaimBuilder
 from .impl.tuples import Chain
 
 
 __all__ = ["LmdbStore", "MemoryStore", "Database", "Directory", "Sequence", "Box", "Bundler", "Chain",
-           "Property", "Container", "Muid", "LogBackedStore", "BundleInfo", "AbstractStore", "Role",
+           "Property", "Container", "Muid", "LogBackedStore", "BundleInfo", "AbstractStore", "Group",
            "Vertex", "Verb", "Edge", "KeySet", "PairSet", "PairMap", "generate_timestamp", "ClaimBuilder"]
```

### Comparing `gink-0.20240407.1712460796/gink/__main__.py` & `gink-0.20240509.1715238879/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/behavior_pb2.py` & `gink-0.20240509.1715238879/gink/builders/behavior_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='proto/behavior.proto',
   package='gink',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x14proto/behavior.proto\x12\x04gink*\x9d\x01\n\x08\x42\x65havior\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x42OX\x10\x01\x12\x0c\n\x08SEQUENCE\x10\x02\x12\x0b\n\x07KEY_SET\x10\x03\x12\r\n\tDIRECTORY\x10\x04\x12\x0c\n\x08PAIR_SET\x10\x05\x12\x0c\n\x08PAIR_MAP\x10\x06\x12\n\n\x06VERTEX\x10\x07\x12\r\n\tEDGE_TYPE\x10\x08\x12\x0c\n\x08PROPERTY\x10\t\x12\x08\n\x04ROLE\x10\nb\x06proto3'
+  serialized_pb=b'\n\x14proto/behavior.proto\x12\x04gink*\xae\x01\n\x08\x42\x65havior\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x42OX\x10\x01\x12\x0c\n\x08SEQUENCE\x10\x02\x12\x0c\n\x08PAIR_MAP\x10\x03\x12\r\n\tDIRECTORY\x10\x04\x12\x0b\n\x07KEY_SET\x10\x05\x12\t\n\x05GROUP\x10\x06\x12\n\n\x06VERTEX\x10\x07\x12\x0c\n\x08PAIR_SET\x10\x08\x12\x0e\n\nEVENT_TYPE\x10\t\x12\x0c\n\x08PROPERTY\x10\n\x12\r\n\tEDGE_TYPE\x10\x0b\x62\x06proto3'
 )
 
 _BEHAVIOR = _descriptor.EnumDescriptor(
   name='Behavior',
   full_name='gink.Behavior',
   filename=None,
   file=DESCRIPTOR,
@@ -42,73 +42,79 @@
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='SEQUENCE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='KEY_SET', index=3, number=3,
+      name='PAIR_MAP', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='DIRECTORY', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PAIR_SET', index=5, number=5,
+      name='KEY_SET', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PAIR_MAP', index=6, number=6,
+      name='GROUP', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='VERTEX', index=7, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='EDGE_TYPE', index=8, number=8,
+      name='PAIR_SET', index=8, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PROPERTY', index=9, number=9,
+      name='EVENT_TYPE', index=9, number=9,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='ROLE', index=10, number=10,
+      name='PROPERTY', index=10, number=10,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='EDGE_TYPE', index=11, number=11,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
   serialized_start=31,
-  serialized_end=188,
+  serialized_end=205,
 )
 _sym_db.RegisterEnumDescriptor(_BEHAVIOR)
 
 Behavior = enum_type_wrapper.EnumTypeWrapper(_BEHAVIOR)
 UNSPECIFIED = 0
 BOX = 1
 SEQUENCE = 2
-KEY_SET = 3
+PAIR_MAP = 3
 DIRECTORY = 4
-PAIR_SET = 5
-PAIR_MAP = 6
+KEY_SET = 5
+GROUP = 6
 VERTEX = 7
-EDGE_TYPE = 8
-PROPERTY = 9
-ROLE = 10
+PAIR_SET = 8
+EVENT_TYPE = 9
+PROPERTY = 10
+EDGE_TYPE = 11
 
 
 DESCRIPTOR.enum_types_by_name['Behavior'] = _BEHAVIOR
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gink-0.20240407.1712460796/gink/builders/bundle_pb2.py` & `gink-0.20240509.1715238879/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/change_pb2.py` & `gink-0.20240509.1715238879/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/claim_pb2.py` & `gink-0.20240509.1715238879/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/clearance_pb2.py` & `gink-0.20240509.1715238879/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/container_pb2.py` & `gink-0.20240509.1715238879/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/entry_pb2.py` & `gink-0.20240509.1715238879/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/key_pb2.py` & `gink-0.20240509.1715238879/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/log_file_pb2.py` & `gink-0.20240509.1715238879/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/movement_pb2.py` & `gink-0.20240509.1715238879/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/muid_pb2.py` & `gink-0.20240509.1715238879/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/pair_pb2.py` & `gink-0.20240509.1715238879/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/sync_message_pb2.py` & `gink-0.20240509.1715238879/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/builders/value_pb2.py` & `gink-0.20240509.1715238879/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/abstract_store.py` & `gink-0.20240509.1715238879/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/addressable.py` & `gink-0.20240509.1715238879/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/attribution.py` & `gink-0.20240509.1715238879/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/box.py` & `gink-0.20240509.1715238879/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/builders.py` & `gink-0.20240509.1715238879/gink/impl/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         KEY_SET = 3
         DIRECTORY = 4
         PAIR_SET = 5
         PAIR_MAP = 6
         VERTEX = 7
         EDGE_TYPE = 8
         PROPERTY = 9
-        ROLE = 10
+        GROUP = 10
 else:
     from ..builders.bundle_pb2 import Bundle as BundleBuilder
     from ..builders.sync_message_pb2 import SyncMessage
     from ..builders.change_pb2 import Change as ChangeBuilder
     from ..builders.entry_pb2 import Entry as EntryBuilder
     from ..builders.value_pb2 import Value as ValueBuilder
     from ..builders.key_pb2 import Key as KeyBuilder
```

### Comparing `gink-0.20240407.1712460796/gink/impl/bundle_info.py` & `gink-0.20240509.1715238879/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/bundle_wrapper.py` & `gink-0.20240509.1715238879/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/bundler.py` & `gink-0.20240509.1715238879/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/chain_tracker.py` & `gink-0.20240509.1715238879/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/coding.py` & `gink-0.20240509.1715238879/gink/impl/coding.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 UNSPECIFIED: int = Behavior.UNSPECIFIED  # type: ignore
 SEQUENCE: int = Behavior.SEQUENCE  # type: ignore
 DIRECTORY: int = Behavior.DIRECTORY  # type: ignore
 PROPERTY: int = Behavior.PROPERTY  # type: ignore
 BOX: int = Behavior.BOX  # type: ignore
 VERTEX: int = Behavior.VERTEX  # type: ignore
-ROLE: int = Behavior.ROLE # type: ignore
+GROUP: int = Behavior.GROUP # type: ignore
 EDGE_TYPE: int = Behavior.EDGE_TYPE # type: ignore
 KEY_SET: int = Behavior.KEY_SET # type: ignore
 PAIR_SET: int = Behavior.PAIR_SET # type: ignore
 PAIR_MAP: int = Behavior.PAIR_MAP # type: ignore
 FLOAT_INF = float("inf")
 INT_INF = 0xffffffffffffffff
 ZERO_64: bytes = b"\x00" * 8
@@ -157,15 +157,15 @@
         middle_key: Union[QueueMiddleKey, Muid, UserKey, None, Tuple[Muid, Muid]]
         if behavior in [DIRECTORY, KEY_SET]:
             middle_key = decode_key(builder)
         elif behavior in (BOX, VERTEX):
             middle_key = None
         elif behavior in (SEQUENCE, EDGE_TYPE):
             middle_key = QueueMiddleKey(position or entry_muid.timestamp)
-        elif behavior in (PROPERTY, ROLE):
+        elif behavior in (PROPERTY, GROUP):
             middle_key = Muid.create(context=entry_muid, builder=builder.describing)  # type: ignore
         elif behavior in (PAIR_SET, PAIR_MAP):
             left = Muid.create(context=entry_muid, builder=builder.pair.left)
             rite = Muid.create(context=entry_muid, builder=builder.pair.rite)
             middle_key = (left, rite)
         else:
             raise AssertionError(f"unexpected behavior: {behavior}")
@@ -189,15 +189,15 @@
         expiry_bytes = data[-8:]
         entry_muid = Muid.from_bytes(entry_muid_bytes)
         middle_key: Union[MuTimestamp, UserKey, Muid, None, Tuple[Muid, Muid]]
         if using in [DIRECTORY, KEY_SET]:
             middle_key = decode_key(middle_key_bytes)
         elif using == SEQUENCE:
             middle_key = QueueMiddleKey.from_bytes(middle_key_bytes)
-        elif using in (PROPERTY, ROLE):
+        elif using in (PROPERTY, GROUP):
             middle_key = Muid.from_bytes(middle_key_bytes)
         elif using in (PAIR_SET, PAIR_MAP):
             middle_key = (Muid.from_bytes(middle_key_bytes[:16]), Muid.from_bytes(middle_key_bytes[16:]))
         elif using in (BOX, VERTEX, EDGE_TYPE):
             middle_key = None
         else:
             raise ValueError(f"unexpected behavior {using}")
@@ -267,15 +267,15 @@
     muid.put_into(entry_builder.container)  # type: ignore
     entry_builder.deletion = True  # type: ignore
     if behavior in (DIRECTORY, KEY_SET):
         assert isinstance(key, (int, str, bytes))
         encode_key(key, entry_builder.key)  # type: ignore
     elif behavior == BOX:
         assert key is None
-    elif behavior in (PROPERTY, ROLE):
+    elif behavior in (PROPERTY, GROUP):
         assert isinstance(key, Muid)
         key.put_into(entry_builder.describing)
     elif behavior in (PAIR_SET, PAIR_MAP):
         assert isinstance(key, tuple)
         assert isinstance(key[0], Muid) and isinstance(key[1], Muid)
         key[0].put_into(entry_builder.pair.left)
         key[1].put_into(entry_builder.pair.rite)
@@ -292,15 +292,15 @@
     """
     if builder.deletion:  # type: ignore
         return deletion
     if builder.HasField("pointee"):  # type: ignore
         return Muid.create(builder=builder.pointee, context=entry_muid)
     if builder.HasField("value"):  # type: ignore
         return decode_value(builder.value)
-    if builder.behavior in (ROLE, KEY_SET):
+    if builder.behavior in (GROUP, KEY_SET):
         return inclusion
     raise ValueError(f"can't interpret {builder}")
 
 
 def entries_equiv(pair1: PlacementBuilderPair, pair2: PlacementBuilderPair) -> bool:
     """ Checks the contained value/pointee/whatever to see if the entries are equiv.
```

### Comparing `gink-0.20240407.1712460796/gink/impl/connection.py` & `gink-0.20240509.1715238879/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/container.py` & `gink-0.20240509.1715238879/gink/impl/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,13 +263,13 @@
     def size(self, *, as_of: GenericTimestamp = None) -> int:
         """ returns the number of elements contained """
 
     def __len__(self):
         return self.size()
 
     def get_describing(self, as_of: GenericTimestamp=None) -> Iterable[Container]:
-        """ Returns the properties and roles associated with this thing. """
+        """ Returns the properties and groups associated with this thing. """
         as_of = self._database.resolve_timestamp(as_of)
         for found in self._database.get_store().get_by_describing(self._muid, as_of):
             container_muid = Muid.create(found.address, found.builder.container)
             if not found.builder.deletion:
                 yield self._database.get_container(container_muid, behavior=found.builder.behavior)
```

### Comparing `gink-0.20240407.1712460796/gink/impl/database.py` & `gink-0.20240509.1715238879/gink/impl/database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/deferred.py` & `gink-0.20240509.1715238879/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/directory.py` & `gink-0.20240509.1715238879/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/graph.py` & `gink-0.20240509.1715238879/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/key_set.py` & `gink-0.20240509.1715238879/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/listener.py` & `gink-0.20240509.1715238879/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/lmdb_store.py` & `gink-0.20240509.1715238879/gink/impl/lmdb_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .abstract_store import AbstractStore, BundleWrapper, BundleCallback
 from .chain_tracker import ChainTracker
 from .lmdb_utilities import to_last_with_prefix
 from .utilities import generate_timestamp, create_claim
 from .coding import (encode_key, create_deleting_entry, PlacementBuilderPair, decode_muts, wrap_change,
                      Placement, encode_muts, QueueMiddleKey, DIRECTORY, SEQUENCE, serialize,
                      ensure_entry_is_valid, deletion, Deletion, decode_entry_occupant, RemovalKey,
-                     LocationKey, PROPERTY, BOX, ROLE, decode_value, EDGE_TYPE, PAIR_MAP, PAIR_SET, KEY_SET,
+                     LocationKey, PROPERTY, BOX, GROUP, decode_value, EDGE_TYPE, PAIR_MAP, PAIR_SET, KEY_SET,
                      normalize_entry_builder, VERTEX)
 
 
 class LmdbStore(AbstractStore):
     """
     """
 
@@ -280,15 +280,15 @@
             trxn: Trxn) -> Iterable[ChangeBuilder]:
         """ Figures out which specific reset method to call to reset a container. """
         behavior = self._get_behavior(container, trxn)
         if behavior == VERTEX:
             for change in self._get_vertex_reset_changes(container, to_time, trxn):
                 yield change
             return
-        if behavior in (DIRECTORY, BOX, ROLE, KEY_SET, PROPERTY):
+        if behavior in (DIRECTORY, BOX, GROUP, KEY_SET, PROPERTY):
             for change in self._get_keyed_reset(container, to_time, trxn, seen, None, behavior):
                 yield change
             return
         if behavior in (SEQUENCE, EDGE_TYPE):
             for change in self._get_sequence_reset(container, to_time, trxn, seen):
                 yield change
             return
@@ -901,15 +901,15 @@
             builder: EntryBuilder):
         retaining = bool(decode_muts(bytes(txn.get(b"entries", db=self._retentions))))
         ensure_entry_is_valid(builder=builder, context=new_info, offset=offset)
         placement_key = Placement.from_builder(builder, new_info, offset)
         entry_muid = placement_key.placer
         container_muid = placement_key.container
         serialized_placement_key = bytes(placement_key)
-        if builder.behavior in (Behavior.DIRECTORY, Behavior.BOX, Behavior.PROPERTY, Behavior.ROLE):
+        if builder.behavior in (Behavior.DIRECTORY, Behavior.BOX, Behavior.PROPERTY, Behavior.GROUP):
             found_entry = self.get_entry_by_key(container_muid, placement_key.middle)
             if found_entry:
                 if retaining:
                     removal_key = bytes(container_muid) + bytes(found_entry.address) + bytes(entry_muid)
                     txn.put(removal_key, b"", db=self._removals)
                 else:
                     self._remove_entry(found_entry.address, txn)
```

### Comparing `gink-0.20240407.1712460796/gink/impl/lmdb_utilities.py` & `gink-0.20240509.1715238879/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/log_backed_store.py` & `gink-0.20240509.1715238879/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/memory_store.py` & `gink-0.20240509.1715238879/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/muid.py` & `gink-0.20240509.1715238879/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/pair_map.py` & `gink-0.20240509.1715238879/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/pair_set.py` & `gink-0.20240509.1715238879/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/property.py` & `gink-0.20240509.1715238879/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/role.py` & `gink-0.20240509.1715238879/gink/impl/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-""" Contains the `Role` Container class. """
+""" Contains the `Group` Container class. """
 from __future__ import annotations
 from typing import Optional, Union, Set, Iterable
 
 from .typedefs import GenericTimestamp
 from .container import Container
 from .coding import deletion, inclusion
 from .muid import Muid
 from .database import Database
 from .bundler import Bundler
 from .builders import Behavior
 
 
-class Role(Container):
-    BEHAVIOR = Behavior.ROLE
+class Group(Container):
+    BEHAVIOR = Behavior.GROUP
 
     def __init__(self, *, contents: Optional[Set[Union[Muid, Container]]]=None,
                  muid: Optional[Muid] = None, database=None):
         """
-        Constructor for a role definition.
+        Constructor for a group definition.
 
         muid: the global id of this directory, created on the fly if None
         db: database send commits through, or last db instance created if None
         """
         database = database or Database.get_last()
         bundler = Bundler()
         if muid is None:
-            muid = Container._create(Behavior.ROLE, database=database, bundler=bundler)
+            muid = Container._create(Behavior.GROUP, database=database, bundler=bundler)
         Container.__init__(self, muid=muid, database=database)
         if contents:
             raise NotImplementedError()
         if len(bundler):
             self._database.commit(bundler)
 
     def include(self, what: Union[Muid, Container], *,
@@ -41,15 +41,15 @@
     def exclude(self, what: Union[Muid, Container], *,
                 bundler: Optional[Bundler]=None, comment: Optional[str]=None):
         if isinstance(what, Container):
             what = what._muid
         return self._add_entry(key=what, value=deletion, bundler=bundler, comment=comment)
 
     def dumps(self, as_of: GenericTimestamp = None) -> str:
-        """ Dumps the contents of this role to a string.
+        """ Dumps the contents of this group to a string.
         """
         identifier = repr(str(self._muid))
         result = f"""{self.__class__.__name__}({identifier}, contents="""
         result += "{"
         stuffing = [repr(_) for _ in self.get_member_ids(as_of=as_of)]
         as_one_line = result + ",".join(stuffing) + "})"
         if len(as_one_line) < 80:
@@ -57,15 +57,15 @@
         result += "\n\t"
         result += ",\n\t".join(stuffing) + "})"
         return result
 
     def size(self, *, as_of: GenericTimestamp = None) -> int:
         ts = self._database.resolve_timestamp(as_of)
         iterable = self._database.get_store().get_keyed_entries(
-            container=self._muid, as_of=ts, behavior=Behavior.ROLE)
+            container=self._muid, as_of=ts, behavior=Behavior.GROUP)
         count = 0
         for entry_pair in iterable:
             if not entry_pair.builder.deletion:
                 count += 1
         return count
 
     def __len__(self):
@@ -77,15 +77,15 @@
 
     def __contains__(self, thing: Union[Muid, Container]) -> bool:
         return self.contains(thing)
 
     def get_member_ids(self, *, as_of: GenericTimestamp = None) -> Iterable[Muid]:
         as_of = self._database.resolve_timestamp(as_of)
         iterable = self._database.get_store().get_keyed_entries(
-            container=self._muid, as_of=as_of, behavior=Behavior.ROLE)
+            container=self._muid, as_of=as_of, behavior=Behavior.GROUP)
         for entry_pair in iterable:
             if entry_pair.builder.deletion:  # type: ignore
                 continue
             yield Muid.create(builder=entry_pair.builder.describing, context=entry_pair.address)
 
     def get_members(self, *, as_of: GenericTimestamp = None) -> Set[Container]:
         """ Returns pairs of (muid, contents) for the sequence at the given time.
@@ -95,8 +95,8 @@
     def contains(self, what: Union[Muid, Container], *, as_of: GenericTimestamp = None) -> bool:
         ts = self._database.resolve_timestamp(as_of)
         if isinstance(what, Container):
             what = what._muid
         found = self._database.get_store().get_entry_by_key(self.get_muid(), key=what, as_of=ts)
         return bool(found and not found.builder.deletion)
 
-Database.register_container_type(Role)
+Database.register_container_type(Group)
```

### Comparing `gink-0.20240407.1712460796/gink/impl/selectable_console.py` & `gink-0.20240509.1715238879/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/sequence.py` & `gink-0.20240509.1715238879/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/tuples.py` & `gink-0.20240509.1715238879/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/typedefs.py` & `gink-0.20240509.1715238879/gink/impl/typedefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 EPOCH = 0
 
 
 class Deletion: # pylint: disable=too-few-public-methods
     """ Used internally to indicate that a key/value assocation has been removed. """
 
 class Inclusion:
-    """ Used to indicate adding something to a set or role. """
+    """ Used to indicate adding something to a set or group. """
```

### Comparing `gink-0.20240407.1712460796/gink/impl/utilities.py` & `gink-0.20240509.1715238879/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/watcher.py` & `gink-0.20240509.1715238879/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/impl/websocket_connection.py` & `gink-0.20240509.1715238879/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_box.py` & `gink-0.20240509.1715238879/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_chain_tracker.py` & `gink-0.20240509.1715238879/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_change_set_info.py` & `gink-0.20240509.1715238879/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_code_values.py` & `gink-0.20240509.1715238879/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_container.py` & `gink-0.20240509.1715238879/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_database.py` & `gink-0.20240509.1715238879/gink/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_demo.py` & `gink-0.20240509.1715238879/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_directory.py` & `gink-0.20240509.1715238879/gink/tests/test_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,14 @@
             assert as_dict == {"foo": "bar", "zoo": "bear", 99: 101}, as_dict
 
 def test_reset():
     """ tests that the reset(time) functionality works """
     for store in [LmdbStore(), MemoryStore()]:
         # TODO: implement reset in memory store
         with store:
-            # pylint: disable=unsupported-assignment-operation, unsupported-role-test
             database = Database(store=store)
             gdi = Directory.get_global_instance(database=database)
             gdi["foo"] = "bar"
             gdi["bar"] = "foo"
             gdi[7] = {"cheese": "wiz", "foo": [True, False, None]}
             gdi["nope"] = Directory()
             gdi["nope"][33] = [1, 2]  # type: ignore
```

### Comparing `gink-0.20240407.1712460796/gink/tests/test_graph.py` & `gink-0.20240509.1715238879/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_key_set.py` & `gink-0.20240509.1715238879/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_lmdb_store.py` & `gink-0.20240509.1715238879/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_logbackedstore.py` & `gink-0.20240509.1715238879/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_muid.py` & `gink-0.20240509.1715238879/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_names.py` & `gink-0.20240509.1715238879/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_pair_map.py` & `gink-0.20240509.1715238879/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_pair_set.py` & `gink-0.20240509.1715238879/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_property.py` & `gink-0.20240509.1715238879/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_role.py` & `gink-0.20240509.1715238879/gink/tests/test_role.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from .. import *
 from contextlib import closing
 
 def test_basics():
-    """ Test the basic include/exclude functionality of roles works as expected. """
+    """ Test the basic include/exclude functionality of groups works as expected. """
     for store in [LmdbStore(), MemoryStore(), ]:
         with closing(store):
             store = LmdbStore()
             database = Database(store=store)
             gd = Directory.get_global_instance(database=database)
             ad = Directory()
-            role = Role()
-            assert gd not in role
-            role.include(gd)
-            assert gd in role
+            group = Group()
+            assert gd not in group
+            group.include(gd)
+            assert gd in group
             mark = database.get_now()
-            assert not role.contains(gd, as_of=-1)
-            role.include(ad)
-            assert len(role) == 2
-            assert role.size(as_of=-1) == 1
-            members = set(role.get_members())
+            assert not group.contains(gd, as_of=-1)
+            group.include(ad)
+            assert len(group) == 2
+            assert group.size(as_of=-1) == 1
+            members = set(group.get_members())
             assert members == {ad, gd}
-            role.exclude(gd)
-            assert role.get_members() == {ad}
-            role.reset(mark)
-            assert role.get_members() == {gd}
+            group.exclude(gd)
+            assert group.get_members() == {ad}
+            group.reset(mark)
+            assert group.get_members() == {gd}
```

### Comparing `gink-0.20240407.1712460796/gink/tests/test_sequence.py` & `gink-0.20240509.1715238879/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_store.py` & `gink-0.20240509.1715238879/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink/tests/test_websocket_connection.py` & `gink-0.20240509.1715238879/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240407.1712460796/gink.egg-info/PKG-INFO` & `gink-0.20240509.1715238879/gink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240407.1712460796
+Version: 0.20240509.1715238879
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240407.1712460796/gink.egg-info/SOURCES.txt` & `gink-0.20240509.1715238879/gink.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 gink/impl/connection.py
 gink/impl/container.py
 gink/impl/database.py
 gink/impl/deferred.py
 gink/impl/directory.py
 gink/impl/dummy.py
 gink/impl/graph.py
+gink/impl/group.py
 gink/impl/key_set.py
 gink/impl/listener.py
 gink/impl/lmdb_store.py
 gink/impl/lmdb_utilities.py
 gink/impl/log_backed_store.py
 gink/impl/memory_store.py
 gink/impl/muid.py
 gink/impl/pair_map.py
 gink/impl/pair_set.py
 gink/impl/property.py
-gink/impl/role.py
 gink/impl/selectable_console.py
 gink/impl/sequence.py
 gink/impl/tuples.py
 gink/impl/typedefs.py
 gink/impl/utilities.py
 gink/impl/watcher.py
 gink/impl/websocket_connection.py
```

### Comparing `gink-0.20240407.1712460796/setup.py` & `gink-0.20240509.1715238879/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240407.1712460796',
+    version='0.20240509.1715238879',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

