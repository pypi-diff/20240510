# Comparing `tmp/yamcs_client-1.9.6.tar.gz` & `tmp/yamcs_client-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs_client-1.9.6.tar", last modified: Thu Apr 18 08:39:38 2024, max compression
+gzip compressed data, was "yamcs_client-1.9.7.tar", last modified: Fri May 10 14:29:46 2024, max compression
```

## Comparing `yamcs_client-1.9.6.tar` & `yamcs_client-1.9.7.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.252878 yamcs_client-1.9.6/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs_client-1.9.6/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs_client-1.9.6/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-04-18 08:39:38.252608 yamcs_client-1.9.6/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs_client-1.9.6/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2024-04-18 08:39:38.252928 yamcs_client-1.9.6/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1730 2023-11-03 10:38:04.000000 yamcs_client-1.9.6/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.197042 yamcs_client-1.9.6/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.198778 yamcs_client-1.9.6/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.200385 yamcs_client-1.9.6/src/yamcs/api/
--rw-r--r--   0 fdi        (503) staff       (20)    13519 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/annotations_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     3573 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/exception_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     5033 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/httpbody_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    13148 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/api/websocket_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.201274 yamcs_client-1.9.6/src/yamcs/archive/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/archive/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    46715 2024-04-17 19:59:36.000000 yamcs_client-1.9.6/src/yamcs/archive/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     8466 2024-04-18 06:39:27.000000 yamcs_client-1.9.6/src/yamcs/archive/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.201991 yamcs_client-1.9.6/src/yamcs/client/
--rw-r--r--   0 fdi        (503) staff       (20)     1495 2024-03-04 11:15:08.000000 yamcs_client-1.9.6/src/yamcs/client/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     5326 2024-03-18 13:20:14.000000 yamcs_client-1.9.6/src/yamcs/client/activities.py
--rw-r--r--   0 fdi        (503) staff       (20)    24029 2024-03-01 16:53:25.000000 yamcs_client-1.9.6/src/yamcs/client/core.py
--rw-r--r--   0 fdi        (503) staff       (20)       22 2024-04-18 08:16:10.000000 yamcs_client-1.9.6/src/yamcs/clientversion.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.203987 yamcs_client-1.9.6/src/yamcs/core/
--rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/core/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7290 2024-03-01 16:04:02.000000 yamcs_client-1.9.6/src/yamcs/core/auth.py
--rw-r--r--   0 fdi        (503) staff       (20)     4665 2024-02-25 21:21:09.000000 yamcs_client-1.9.6/src/yamcs/core/context.py
--rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/core/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4234 2023-04-16 19:38:09.000000 yamcs_client-1.9.6/src/yamcs/core/futures.py
--rw-r--r--   0 fdi        (503) staff       (20)    12888 2024-04-18 06:48:13.000000 yamcs_client-1.9.6/src/yamcs/core/helpers.py
--rw-r--r--   0 fdi        (503) staff       (20)     1611 2023-04-16 20:00:45.000000 yamcs_client-1.9.6/src/yamcs/core/pagination.py
--rw-r--r--   0 fdi        (503) staff       (20)     7817 2024-03-16 08:21:22.000000 yamcs_client-1.9.6/src/yamcs/core/subscriptions.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.204803 yamcs_client-1.9.6/src/yamcs/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/filetransfer/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    11570 2024-04-17 21:42:57.000000 yamcs_client-1.9.6/src/yamcs/filetransfer/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    15610 2024-04-17 21:47:07.000000 yamcs_client-1.9.6/src/yamcs/filetransfer/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.205750 yamcs_client-1.9.6/src/yamcs/link/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/link/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     8258 2024-04-17 21:22:59.000000 yamcs_client-1.9.6/src/yamcs/link/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     1996 2024-02-24 17:03:41.000000 yamcs_client-1.9.6/src/yamcs/link/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.206534 yamcs_client-1.9.6/src/yamcs/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/mdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    15401 2024-03-01 15:24:22.000000 yamcs_client-1.9.6/src/yamcs/mdb/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    13254 2024-02-24 16:11:30.000000 yamcs_client-1.9.6/src/yamcs/mdb/model.py
--rw-r--r--   0 fdi        (503) staff       (20)    12970 2024-02-24 16:07:18.000000 yamcs_client-1.9.6/src/yamcs/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.206801 yamcs_client-1.9.6/src/yamcs/protobuf/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.207536 yamcs_client-1.9.6/src/yamcs/protobuf/actions/
--rw-r--r--   0 fdi        (503) staff       (20)     4545 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/actions/actions_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.208397 yamcs_client-1.9.6/src/yamcs/protobuf/activities/
--rw-r--r--   0 fdi        (503) staff       (20)    17234 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    38288 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.209937 yamcs_client-1.9.6/src/yamcs/protobuf/alarms/
--rw-r--r--   0 fdi        (503) staff       (20)    29047 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    40124 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.211784 yamcs_client-1.9.6/src/yamcs/protobuf/archive/
--rw-r--r--   0 fdi        (503) staff       (20)    33962 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/archive_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    53220 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/index_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    43577 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    19316 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.212188 yamcs_client-1.9.6/src/yamcs/protobuf/audit/
--rw-r--r--   0 fdi        (503) staff       (20)    11973 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/audit/audit_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.212681 yamcs_client-1.9.6/src/yamcs/protobuf/auth/
--rw-r--r--   0 fdi        (503) staff       (20)     8446 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/auth/auth_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.213122 yamcs_client-1.9.6/src/yamcs/protobuf/buckets/
--rw-r--r--   0 fdi        (503) staff       (20)    34808 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/buckets/buckets_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.215006 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/
--rw-r--r--   0 fdi        (503) staff       (20)    12415 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/clearance_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    41600 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commanding_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    47775 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commands_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    33253 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/commanding/queues_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.215305 yamcs_client-1.9.6/src/yamcs/protobuf/config/
--rw-r--r--   0 fdi        (503) staff       (20)    17412 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/config/config_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.215799 yamcs_client-1.9.6/src/yamcs/protobuf/cop1/
--rw-r--r--   0 fdi        (503) staff       (20)    34928 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/cop1/cop1_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.216244 yamcs_client-1.9.6/src/yamcs/protobuf/database/
--rw-r--r--   0 fdi        (503) staff       (20)     8255 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/database/database_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.217338 yamcs_client-1.9.6/src/yamcs/protobuf/events/
--rw-r--r--   0 fdi        (503) staff       (20)     9301 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/events/events_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    30677 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/events/events_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.217692 yamcs_client-1.9.6/src/yamcs/protobuf/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)    80380 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.219027 yamcs_client-1.9.6/src/yamcs/protobuf/iam/
--rw-r--r--   0 fdi        (503) staff       (20)    73419 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/iam/iam_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    10014 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/iam/sessions_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.220243 yamcs_client-1.9.6/src/yamcs/protobuf/instances/
--rw-r--r--   0 fdi        (503) staff       (20)    19968 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    32345 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.220628 yamcs_client-1.9.6/src/yamcs/protobuf/links/
--rw-r--r--   0 fdi        (503) staff       (20)    31906 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/links/links_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.221391 yamcs_client-1.9.6/src/yamcs/protobuf/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)   280528 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/mdb/mdb_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.224140 yamcs_client-1.9.6/src/yamcs/protobuf/packets/
--rw-r--r--   0 fdi        (503) staff       (20)     6029 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    46220 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.225528 yamcs_client-1.9.6/src/yamcs/protobuf/plists/
--rw-r--r--   0 fdi        (503) staff       (20)     4238 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    18747 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.226769 yamcs_client-1.9.6/src/yamcs/protobuf/processing/
--rw-r--r--   0 fdi        (503) staff       (20)    37572 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    86589 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/processing/processing_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.227713 yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/
--rw-r--r--   0 fdi        (503) staff       (20)    28924 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    10465 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.228229 yamcs_client-1.9.6/src/yamcs/protobuf/replication/
--rw-r--r--   0 fdi        (503) staff       (20)    13030 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/replication/replication_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.228655 yamcs_client-1.9.6/src/yamcs/protobuf/server/
--rw-r--r--   0 fdi        (503) staff       (20)    70072 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/server/server_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.229846 yamcs_client-1.9.6/src/yamcs/protobuf/services/
--rw-r--r--   0 fdi        (503) staff       (20)     6369 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/services/services_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    11946 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/services/services_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.230343 yamcs_client-1.9.6/src/yamcs/protobuf/table/
--rw-r--r--   0 fdi        (503) staff       (20)    68243 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/table/table_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.240360 yamcs_client-1.9.6/src/yamcs/protobuf/tco/
--rw-r--r--   0 fdi        (503) staff       (20)    32749 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/tco/tco_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.240969 yamcs_client-1.9.6/src/yamcs/protobuf/time/
--rw-r--r--   0 fdi        (503) staff       (20)    12958 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/time/time_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.241481 yamcs_client-1.9.6/src/yamcs/protobuf/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)   125195 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/timeline/timeline_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.242290 yamcs_client-1.9.6/src/yamcs/protobuf/yamcsManagement/
--rw-r--r--   0 fdi        (503) staff       (20)    32409 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    42446 2024-04-17 20:21:54.000000 yamcs_client-1.9.6/src/yamcs/protobuf/yamcs_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.243605 yamcs_client-1.9.6/src/yamcs/storage/
--rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/storage/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     5683 2024-03-05 11:43:25.000000 yamcs_client-1.9.6/src/yamcs/storage/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     6439 2024-04-16 20:50:12.000000 yamcs_client-1.9.6/src/yamcs/storage/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.245104 yamcs_client-1.9.6/src/yamcs/tco/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/tco/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4867 2024-02-24 17:10:21.000000 yamcs_client-1.9.6/src/yamcs/tco/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     3089 2024-02-24 17:11:07.000000 yamcs_client-1.9.6/src/yamcs/tco/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.246175 yamcs_client-1.9.6/src/yamcs/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs_client-1.9.6/src/yamcs/timeline/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7923 2024-03-05 11:01:12.000000 yamcs_client-1.9.6/src/yamcs/timeline/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    16141 2024-03-05 10:37:49.000000 yamcs_client-1.9.6/src/yamcs/timeline/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.247341 yamcs_client-1.9.6/src/yamcs/tmtc/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.6/src/yamcs/tmtc/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    51419 2024-04-17 20:49:20.000000 yamcs_client-1.9.6/src/yamcs/tmtc/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    35330 2024-04-16 20:53:14.000000 yamcs_client-1.9.6/src/yamcs/tmtc/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-18 08:39:38.252208 yamcs_client-1.9.6/src/yamcs_client.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     3504 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)       55 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/requires.txt
--rw-r--r--   0 fdi        (503) staff       (20)        6 2024-04-18 08:39:38.000000 yamcs_client-1.9.6/src/yamcs_client.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.689078 yamcs_client-1.9.7/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs_client-1.9.7/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs_client-1.9.7/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-05-10 14:29:46.688716 yamcs_client-1.9.7/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs_client-1.9.7/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2024-05-10 14:29:46.689148 yamcs_client-1.9.7/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1730 2023-11-03 10:38:04.000000 yamcs_client-1.9.7/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.615717 yamcs_client-1.9.7/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.617446 yamcs_client-1.9.7/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.619476 yamcs_client-1.9.7/src/yamcs/api/
+-rw-r--r--   0 fdi        (503) staff       (20)    13519 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/annotations_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3573 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/exception_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5033 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/httpbody_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13148 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/websocket_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.620478 yamcs_client-1.9.7/src/yamcs/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/archive/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    46715 2024-04-17 19:59:36.000000 yamcs_client-1.9.7/src/yamcs/archive/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8466 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/archive/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.621283 yamcs_client-1.9.7/src/yamcs/client/
+-rw-r--r--   0 fdi        (503) staff       (20)     1495 2024-03-04 11:15:08.000000 yamcs_client-1.9.7/src/yamcs/client/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5326 2024-03-18 13:20:14.000000 yamcs_client-1.9.7/src/yamcs/client/activities.py
+-rw-r--r--   0 fdi        (503) staff       (20)    24601 2024-05-10 10:26:26.000000 yamcs_client-1.9.7/src/yamcs/client/core.py
+-rw-r--r--   0 fdi        (503) staff       (20)       22 2024-05-10 14:25:31.000000 yamcs_client-1.9.7/src/yamcs/clientversion.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.623912 yamcs_client-1.9.7/src/yamcs/core/
+-rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/core/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7290 2024-05-10 10:20:44.000000 yamcs_client-1.9.7/src/yamcs/core/auth.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5597 2024-05-10 10:20:28.000000 yamcs_client-1.9.7/src/yamcs/core/context.py
+-rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/core/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4234 2023-04-16 19:38:09.000000 yamcs_client-1.9.7/src/yamcs/core/futures.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13731 2024-05-10 08:42:48.000000 yamcs_client-1.9.7/src/yamcs/core/helpers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1611 2023-04-16 20:00:45.000000 yamcs_client-1.9.7/src/yamcs/core/pagination.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7817 2024-03-16 08:21:22.000000 yamcs_client-1.9.7/src/yamcs/core/subscriptions.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.624601 yamcs_client-1.9.7/src/yamcs/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/filetransfer/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    11570 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/filetransfer/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15610 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/filetransfer/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.625870 yamcs_client-1.9.7/src/yamcs/link/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/link/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8258 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/link/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1996 2024-02-24 17:03:41.000000 yamcs_client-1.9.7/src/yamcs/link/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.627040 yamcs_client-1.9.7/src/yamcs/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/mdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15401 2024-03-01 15:24:22.000000 yamcs_client-1.9.7/src/yamcs/mdb/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13254 2024-02-24 16:11:30.000000 yamcs_client-1.9.7/src/yamcs/mdb/model.py
+-rw-r--r--   0 fdi        (503) staff       (20)    12970 2024-02-24 16:07:18.000000 yamcs_client-1.9.7/src/yamcs/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.627628 yamcs_client-1.9.7/src/yamcs/protobuf/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.628506 yamcs_client-1.9.7/src/yamcs/protobuf/actions/
+-rw-r--r--   0 fdi        (503) staff       (20)     4545 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/actions/actions_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.630619 yamcs_client-1.9.7/src/yamcs/protobuf/activities/
+-rw-r--r--   0 fdi        (503) staff       (20)    17234 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    38288 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.632805 yamcs_client-1.9.7/src/yamcs/protobuf/alarms/
+-rw-r--r--   0 fdi        (503) staff       (20)    29047 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    40124 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.637153 yamcs_client-1.9.7/src/yamcs/protobuf/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)    33962 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/archive_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    53220 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/index_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    43577 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    19316 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.637886 yamcs_client-1.9.7/src/yamcs/protobuf/audit/
+-rw-r--r--   0 fdi        (503) staff       (20)    11973 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/audit/audit_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.638447 yamcs_client-1.9.7/src/yamcs/protobuf/auth/
+-rw-r--r--   0 fdi        (503) staff       (20)     8446 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/auth/auth_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.639041 yamcs_client-1.9.7/src/yamcs/protobuf/buckets/
+-rw-r--r--   0 fdi        (503) staff       (20)    34808 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/buckets/buckets_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.641223 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/
+-rw-r--r--   0 fdi        (503) staff       (20)    12415 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/clearance_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    41600 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commanding_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    47775 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commands_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    33253 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/queues_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.641586 yamcs_client-1.9.7/src/yamcs/protobuf/config/
+-rw-r--r--   0 fdi        (503) staff       (20)    17412 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/config/config_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.641942 yamcs_client-1.9.7/src/yamcs/protobuf/cop1/
+-rw-r--r--   0 fdi        (503) staff       (20)    34928 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/cop1/cop1_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.642467 yamcs_client-1.9.7/src/yamcs/protobuf/database/
+-rw-r--r--   0 fdi        (503) staff       (20)     8255 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/database/database_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.643358 yamcs_client-1.9.7/src/yamcs/protobuf/events/
+-rw-r--r--   0 fdi        (503) staff       (20)     9301 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/events/events_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    30677 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/events/events_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.643833 yamcs_client-1.9.7/src/yamcs/protobuf/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)    80380 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.644915 yamcs_client-1.9.7/src/yamcs/protobuf/iam/
+-rw-r--r--   0 fdi        (503) staff       (20)    73419 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/iam/iam_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    10014 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/iam/sessions_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.646455 yamcs_client-1.9.7/src/yamcs/protobuf/instances/
+-rw-r--r--   0 fdi        (503) staff       (20)    19968 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    32345 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.646837 yamcs_client-1.9.7/src/yamcs/protobuf/links/
+-rw-r--r--   0 fdi        (503) staff       (20)    31906 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/links/links_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.647475 yamcs_client-1.9.7/src/yamcs/protobuf/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)   280528 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/mdb/mdb_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.649554 yamcs_client-1.9.7/src/yamcs/protobuf/packets/
+-rw-r--r--   0 fdi        (503) staff       (20)     6029 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    46220 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.650507 yamcs_client-1.9.7/src/yamcs/protobuf/plists/
+-rw-r--r--   0 fdi        (503) staff       (20)     4238 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18747 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.652751 yamcs_client-1.9.7/src/yamcs/protobuf/processing/
+-rw-r--r--   0 fdi        (503) staff       (20)    37572 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    86589 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/processing/processing_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.654241 yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/
+-rw-r--r--   0 fdi        (503) staff       (20)    28924 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    10465 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.654797 yamcs_client-1.9.7/src/yamcs/protobuf/replication/
+-rw-r--r--   0 fdi        (503) staff       (20)    13030 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/replication/replication_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.655682 yamcs_client-1.9.7/src/yamcs/protobuf/server/
+-rw-r--r--   0 fdi        (503) staff       (20)    70072 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/server/server_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.658738 yamcs_client-1.9.7/src/yamcs/protobuf/services/
+-rw-r--r--   0 fdi        (503) staff       (20)     6369 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/services/services_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    11946 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/services/services_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.659146 yamcs_client-1.9.7/src/yamcs/protobuf/table/
+-rw-r--r--   0 fdi        (503) staff       (20)    68243 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/table/table_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.660399 yamcs_client-1.9.7/src/yamcs/protobuf/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)    32749 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/tco/tco_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.660868 yamcs_client-1.9.7/src/yamcs/protobuf/time/
+-rw-r--r--   0 fdi        (503) staff       (20)    12958 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/time/time_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.661490 yamcs_client-1.9.7/src/yamcs/protobuf/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)   125195 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/timeline/timeline_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.662444 yamcs_client-1.9.7/src/yamcs/protobuf/yamcsManagement/
+-rw-r--r--   0 fdi        (503) staff       (20)    32409 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    42446 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/yamcs_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.663953 yamcs_client-1.9.7/src/yamcs/storage/
+-rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/storage/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5683 2024-03-05 11:43:25.000000 yamcs_client-1.9.7/src/yamcs/storage/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6439 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/storage/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.664665 yamcs_client-1.9.7/src/yamcs/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/tco/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4867 2024-02-24 17:10:21.000000 yamcs_client-1.9.7/src/yamcs/tco/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3089 2024-02-24 17:11:07.000000 yamcs_client-1.9.7/src/yamcs/tco/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.665380 yamcs_client-1.9.7/src/yamcs/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs_client-1.9.7/src/yamcs/timeline/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7923 2024-03-05 11:01:12.000000 yamcs_client-1.9.7/src/yamcs/timeline/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16141 2024-03-05 10:37:49.000000 yamcs_client-1.9.7/src/yamcs/timeline/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.666715 yamcs_client-1.9.7/src/yamcs/tmtc/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/tmtc/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    51419 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/tmtc/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    35330 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/tmtc/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.688250 yamcs_client-1.9.7/src/yamcs_client.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     3504 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)       55 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/requires.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/top_level.txt
```

### Comparing `yamcs_client-1.9.6/LICENSE` & `yamcs_client-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/PKG-INFO` & `yamcs_client-1.9.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.9.6
+Version: 1.9.7
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs_client-1.9.6/README.md` & `yamcs_client-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/setup.py` & `yamcs_client-1.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/api/annotations_pb2.py` & `yamcs_client-1.9.7/src/yamcs/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/api/exception_pb2.py` & `yamcs_client-1.9.7/src/yamcs/api/exception_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/api/httpbody_pb2.py` & `yamcs_client-1.9.7/src/yamcs/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/api/websocket_pb2.py` & `yamcs_client-1.9.7/src/yamcs/api/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/archive/client.py` & `yamcs_client-1.9.7/src/yamcs/archive/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/archive/model.py` & `yamcs_client-1.9.7/src/yamcs/archive/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/client/__init__.py` & `yamcs_client-1.9.7/src/yamcs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/client/activities.py` & `yamcs_client-1.9.7/src/yamcs/client/activities.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/client/core.py` & `yamcs_client-1.9.7/src/yamcs/client/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         self,
         address: str,
         *,
         tls: bool = False,
         tls_verify: Union[bool, str] = True,
         credentials: Optional[Credentials] = None,
         user_agent: Optional[str] = None,
+        keep_alive: bool = True,
         on_token_update: Optional[Callable[[Credentials], None]] = None,
     ):
         """
         :param address:
             The address of Yamcs in the format 'hostname:port'
         :param tls:
             Whether TLS encryption is expected
@@ -168,14 +169,21 @@
             As an alternative to a boolean value, this option
             may be set to a path containing the appropriate
             TLS CA certificate bundle.
         :param credentials:
             Credentials for when the server is secured
         :param user_agent:
             Optionally override the default user agent
+        :param keep_alive:
+            Automatically renew the client session. If disabled,
+            the session will terminate after about 30 minutes of
+            inactivity.
+
+            This property is only considered when accessing a
+            server that requires authentication.
         """
 
         # Allow server URLs.
         # Currently undocumented, but this is expected to become the
         # default, later on.
         if address.startswith("http://") or address.startswith("https://"):
             components = urlparse(address)
@@ -186,14 +194,15 @@
         self.ctx = Context(
             address=address,
             tls=tls,
             credentials=credentials,
             user_agent=user_agent,
             on_token_update=on_token_update,
             tls_verify=tls_verify,
+            keep_alive=keep_alive,
         )
 
     @staticmethod
     def from_environment():
         """
         Create a :class:`.YamcsClient`, initialized from environment variables.
 
@@ -210,14 +219,20 @@
         credentials = None
         api_key = os.environ.get("YAMCS_API_KEY")
         if api_key:
             credentials = APIKeyCredentials(api_key)
 
         return YamcsClient(url, credentials=credentials)
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+
     def get_time(self, instance) -> Optional[datetime.datetime]:
         """
         Return the current mission time for the specified instance.
         """
         url = f"/instances/{instance}"
         response = self.ctx.get_proto(url)
         message = instances_pb2.YamcsInstance()
@@ -731,7 +746,11 @@
 
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
+
+    def close(self):
+        """Close this client session"""
+        self.ctx.close()
```

### Comparing `yamcs_client-1.9.6/src/yamcs/core/auth.py` & `yamcs_client-1.9.7/src/yamcs/core/auth.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/core/context.py` & `yamcs_client-1.9.7/src/yamcs/core/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+from datetime import datetime, timezone
 from typing import Callable, Optional, Union
 
 import requests
 import urllib3
 from google.protobuf.message import DecodeError
 from yamcs import clientversion
 from yamcs.api import exception_pb2
 from yamcs.core.auth import Credentials
 from yamcs.core.exceptions import NotFound, Unauthorized, YamcsError
-from yamcs.core.helpers import do_request
+from yamcs.core.helpers import FixedDelay, do_request
 
 
 class Context:
-    credentials = None
+    credentials: Optional[Credentials] = None
 
     def __init__(
         self,
         address: str,
         tls: bool = False,
         credentials: Optional[Credentials] = None,
         user_agent: Optional[str] = None,
         on_token_update: Optional[Callable[[Credentials], None]] = None,
         tls_verify: Union[bool, str] = True,
+        keep_alive: bool = True,
     ):
         if address.endswith("/"):
             self.address = address[:-1]
         else:
             self.address = address
 
         if tls:
@@ -47,17 +49,31 @@
                     requests.packages.urllib3.exceptions.InsecureRequestWarning
                 )
             except Exception:
                 # requests >= 2.16.0
                 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
         if credentials:
-            self.credentials = credentials.login(
+            converted_creds = credentials.login(
                 self.session, self.auth_root, on_token_update
             )
+            self.credentials = converted_creds
+
+            # An assigned refresh token lives only for about 30 minutes. We actively
+            # extend it, so that the session survives when idle.
+            if converted_creds.expiry and keep_alive:
+
+                def renew_session():
+                    expiry = converted_creds.expiry
+                    if expiry:
+                        remaining = expiry - datetime.now(tz=timezone.utc)
+                        if 0 < remaining.total_seconds() < 60:
+                            converted_creds.refresh(self.session, self.auth_root)
+
+                self._session_renewer = FixedDelay(renew_session, 10)
 
         if not user_agent:
             user_agent = "python-yamcs-client v" + clientversion.__version__
         self.session.headers.update({"User-Agent": user_agent})
 
     def get_proto(self, path: str, **kwargs) -> requests.Response:
         headers = kwargs.pop("headers", {})
@@ -114,7 +130,15 @@
             msg = getattr(exception_message, "msg")
             raise NotFound(f"404 Client Error: {msg}")
         elif 400 <= response.status_code < 500:
             msg = getattr(exception_message, "msg")
             raise YamcsError(f"{response.status_code} Client Error: {msg}")
         msg = getattr(exception_message, "msg")
         raise YamcsError(f"{response.status_code} Server Error: {msg}")
+
+    def close(self):
+        """Close this context"""
+
+        if self._session_renewer:
+            self._session_renewer.stop()
+
+        self.session.close()
```

### Comparing `yamcs_client-1.9.6/src/yamcs/core/futures.py` & `yamcs_client-1.9.7/src/yamcs/core/futures.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/core/helpers.py` & `yamcs_client-1.9.7/src/yamcs/core/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import binascii
 import collections
 import json
 import logging
 import os
 from datetime import datetime, timezone
-from typing import Any, Iterator, List, Union
+from threading import Timer
+from typing import Any, Callable, Iterator, List, Union
 from urllib.parse import urlparse
 
 import requests
 import urllib3
 from google.protobuf import timestamp_pb2
 from google.protobuf.internal.decoder import _DecodeVarint32
 from google.protobuf.internal.encoder import _VarintBytes
@@ -355,7 +356,38 @@
         repeatable.extend([value._proto for value in __iterable])
 
     def clear(self):
         repeatable = getattr(self.parent_proto, self.items_key)
         copy = list(repeatable)
         for item in copy:
             repeatable.remove(item)
+
+
+class FixedDelay:
+    """
+    Helper class to run a periodic action, with a fixed delay between
+    the termination of one execution, and the commencement of the next.
+    """
+
+    def __init__(self, action: Callable[[], None], period: float):
+        self._timer = None
+        self.action = action
+        self.period = period
+        self.is_running = False
+        self.start()
+
+    def start(self):
+        if not self.is_running:
+            self._timer = Timer(self.period, self._run)
+            self._timer.daemon = True
+            self._timer.start()
+            self.is_running = True
+
+    def stop(self):
+        if self._timer:
+            self._timer.cancel()
+        self.is_running = False
+
+    def _run(self):
+        self.is_running = False
+        self.start()
+        self.action()
```

### Comparing `yamcs_client-1.9.6/src/yamcs/core/pagination.py` & `yamcs_client-1.9.7/src/yamcs/core/pagination.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/core/subscriptions.py` & `yamcs_client-1.9.7/src/yamcs/core/subscriptions.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/filetransfer/client.py` & `yamcs_client-1.9.7/src/yamcs/filetransfer/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/filetransfer/model.py` & `yamcs_client-1.9.7/src/yamcs/filetransfer/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/link/client.py` & `yamcs_client-1.9.7/src/yamcs/link/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/link/model.py` & `yamcs_client-1.9.7/src/yamcs/link/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/mdb/client.py` & `yamcs_client-1.9.7/src/yamcs/mdb/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/mdb/model.py` & `yamcs_client-1.9.7/src/yamcs/mdb/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/model.py` & `yamcs_client-1.9.7/src/yamcs/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/actions/actions_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/actions/actions_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/activities/activities_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/alarms/alarms_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/archive/archive_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/archive/archive_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/archive/index_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/archive/index_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/archive/rocksdb_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/archive/rocksdb_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/audit/audit_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/audit/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/auth/auth_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/buckets/buckets_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/buckets/buckets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/clearance_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/clearance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commanding_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commanding_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/commands_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commands_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/commanding/queues_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/queues_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/config/config_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/config/config_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/cop1/cop1_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/cop1/cop1_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/database/database_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/database/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/events/events_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/events/events_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/events/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/iam/iam_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/iam/iam_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/iam/sessions_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/iam/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/instances/instances_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/links/links_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/links/links_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/mdb/mdb_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/mdb/mdb_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/packets/packets_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/plists/plists_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/processing/mdb_override_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/processing/mdb_override_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/processing/processing_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/processing/processing_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/replication/replication_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/replication/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/server/server_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/server/server_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/services/services_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/services/services_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/services/services_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/services/services_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/table/table_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/table/table_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/tco/tco_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/tco/tco_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/time/time_service_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/time/time_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/timeline/timeline_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/timeline/timeline_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/protobuf/yamcs_pb2.py` & `yamcs_client-1.9.7/src/yamcs/protobuf/yamcs_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/storage/client.py` & `yamcs_client-1.9.7/src/yamcs/storage/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/storage/model.py` & `yamcs_client-1.9.7/src/yamcs/storage/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/tco/client.py` & `yamcs_client-1.9.7/src/yamcs/tco/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/tco/model.py` & `yamcs_client-1.9.7/src/yamcs/tco/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/timeline/client.py` & `yamcs_client-1.9.7/src/yamcs/timeline/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/timeline/model.py` & `yamcs_client-1.9.7/src/yamcs/timeline/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/tmtc/client.py` & `yamcs_client-1.9.7/src/yamcs/tmtc/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs/tmtc/model.py` & `yamcs_client-1.9.7/src/yamcs/tmtc/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.6/src/yamcs_client.egg-info/PKG-INFO` & `yamcs_client-1.9.7/src/yamcs_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.9.6
+Version: 1.9.7
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs_client-1.9.6/src/yamcs_client.egg-info/SOURCES.txt` & `yamcs_client-1.9.7/src/yamcs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

