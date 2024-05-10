# Comparing `tmp/eventstoredb-0.8.1.tar.gz` & `tmp/eventstoredb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventstoredb-0.8.1.tar", last modified: Tue Jan 30 17:08:42 2024, max compression
+gzip compressed data, was "eventstoredb-0.9.0.tar", last modified: Fri May 10 19:15:38 2024, max compression
```

## Comparing `eventstoredb-0.8.1.tar` & `eventstoredb-0.9.0.tar`

### file list

```diff
@@ -1,108 +1,113 @@
--rw-r--r--   0        0        0    11357 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/LICENSE
--rw-r--r--   0        0        0     1684 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/README.md
--rw-r--r--   0        0        0       75 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/__init__.py
--rw-r--r--   0        0        0       22 2024-01-30 17:08:42.894197 eventstoredb-0.8.1/eventstoredb/__version__.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/append_to_stream/__init__.py
--rw-r--r--   0        0        0     1116 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/append_to_stream/exceptions.py
--rw-r--r--   0        0        0     4595 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/append_to_stream/grpc.py
--rw-r--r--   0        0        0     1473 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/append_to_stream/mixin.py
--rw-r--r--   0        0        0      586 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/append_to_stream/types.py
--rw-r--r--   0        0        0     2495 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/client.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_all/__init__.py
--rw-r--r--   0        0        0     3239 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_all/grpc.py
--rw-r--r--   0        0        0     1354 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_all/mixin.py
--rw-r--r--   0        0        0      835 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_all/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/__init__.py
--rw-r--r--   0        0        0      463 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/exceptions.py
--rw-r--r--   0        0        0     4528 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/grpc.py
--rw-r--r--   0        0        0     1362 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/mixin.py
--rw-r--r--   0        0        0     1019 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_all/__init__.py
--rw-r--r--   0        0        0      726 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_all/grpc.py
--rw-r--r--   0        0        0     1354 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_all/mixin.py
--rw-r--r--   0        0        0      135 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_all/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_stream/__init__.py
--rw-r--r--   0        0        0      816 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_stream/grpc.py
--rw-r--r--   0        0        0     1444 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_stream/mixin.py
--rw-r--r--   0        0        0      142 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_stream/types.py
--rw-r--r--   0        0        0     1027 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/exceptions.py
--rw-r--r--   0        0        0      223 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/protocol.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_all/__init__.py
--rw-r--r--   0        0        0     2903 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_all/grpc.py
--rw-r--r--   0        0        0     1060 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_all/mixin.py
--rw-r--r--   0        0        0      654 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_all/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_stream/__init__.py
--rw-r--r--   0        0        0     4171 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_stream/grpc.py
--rw-r--r--   0        0        0     1124 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_stream/mixin.py
--rw-r--r--   0        0        0      391 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/read_stream/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_all/__init__.py
--rw-r--r--   0        0        0     3788 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_all/grpc.py
--rw-r--r--   0        0        0     1308 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_all/mixin.py
--rw-r--r--   0        0        0      669 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_all/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_all/__init__.py
--rw-r--r--   0        0        0      856 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_all/grpc.py
--rw-r--r--   0        0        0     1058 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_all/mixin.py
--rw-r--r--   0        0        0      341 2024-01-30 17:08:15.082449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_all/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/exceptions.py
--rw-r--r--   0        0        0     5019 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/grpc.py
--rw-r--r--   0        0        0     3367 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/mixin.py
--rw-r--r--   0        0        0      380 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_stream/__init__.py
--rw-r--r--   0        0        0     2243 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_stream/grpc.py
--rw-r--r--   0        0        0     1470 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_stream/mixin.py
--rw-r--r--   0        0        0      341 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/subscribe_to_stream/types.py
--rw-r--r--   0        0        0     1208 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_all/__init__.py
--rw-r--r--   0        0        0     1757 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_all/grpc.py
--rw-r--r--   0        0        0     1354 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_all/mixin.py
--rw-r--r--   0        0        0      268 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_all/types.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_stream/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_stream/exceptions.py
--rw-r--r--   0        0        0     1710 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_stream/grpc.py
--rw-r--r--   0        0        0     1444 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_stream/mixin.py
--rw-r--r--   0        0        0      280 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_stream/types.py
--rw-r--r--   0        0        0     1423 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/events.py
--rw-r--r--   0        0        0     1118 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/exceptions.py
--rw-r--r--   0        0        0      323 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/filters.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/__init__.py
--rw-r--r--   0        0        0     2722 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/__init__.py
--rw-r--r--   0        0        0     2817 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/gossip/__init__.py
--rw-r--r--   0        0        0     2224 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/monitoring/__init__.py
--rw-r--r--   0        0        0    10616 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/operations/__init__.py
--rw-r--r--   0        0        0    26972 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/persistent_subscriptions/__init__.py
--rw-r--r--   0        0        0    18443 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/projections/__init__.py
--rw-r--r--   0        0        0     4951 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/redaction/__init__.py
--rw-r--r--   0        0        0     2408 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/server_features/__init__.py
--rw-r--r--   0        0        0    22069 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/streams/__init__.py
--rw-r--r--   0        0        0    13872 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/client/users/__init__.py
--rw-r--r--   0        0        0    22153 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/event_store/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/google/__init__.py
--rw-r--r--   0        0        0     7745 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/generated/google/rpc/__init__.py
--rw-r--r--   0        0        0     2409 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/options.py
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/py.typed
--rw-r--r--   0        0        0      253 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/subscriptions.py
--rw-r--r--   0        0        0      358 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/eventstoredb/types.py
--rw-r--r--   0        0        0     5194 2024-01-30 17:08:42.910197 eventstoredb-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0     2290 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0      738 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/docker-compose.yml
--rw-r--r--   0        0        0     9527 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_append_to_stream.py
--rw-r--r--   0        0        0     1126 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_client_options.py
--rw-r--r--   0        0        0     5447 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_create_persistent_subscription_to_all.py
--rw-r--r--   0        0        0     4728 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_create_persistent_subscription_to_stream.py
--rw-r--r--   0        0        0     1312 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_delete_persistent_subscription_to_all.py
--rw-r--r--   0        0        0     1426 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_delete_persistent_subscription_to_stream.py
--rw-r--r--   0        0        0       73 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_import.py
--rw-r--r--   0        0        0    13548 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_read_all.py
--rw-r--r--   0        0        0     6084 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_read_stream.py
--rw-r--r--   0        0        0    10686 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_subscribe_to_all.py
--rw-r--r--   0        0        0    14046 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_subscribe_to_persistent_subscription_to_all.py
--rw-r--r--   0        0        0     3786 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_subscribe_to_persistent_subscription_to_stream.py
--rw-r--r--   0        0        0     3601 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_subscribe_to_stream.py
--rw-r--r--   0        0        0     1752 2024-01-30 17:08:15.086449 eventstoredb-0.8.1/tests/test_update_persistent_subscription_to_all.py
--rw-r--r--   0        0        0     1865 2024-01-30 17:08:15.090448 eventstoredb-0.8.1/tests/test_update_persistent_subscription_to_stream.py
--rw-r--r--   0        0        0     3119 2024-01-30 17:08:15.090448 eventstoredb-0.8.1/tests/utils.py
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 eventstoredb-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1684 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/README.md
+-rw-r--r--   0        0        0       75 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-10 19:15:38.143659 eventstoredb-0.9.0/eventstoredb/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/append_to_stream/__init__.py
+-rw-r--r--   0        0        0     1116 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/append_to_stream/exceptions.py
+-rw-r--r--   0        0        0     4595 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/append_to_stream/grpc.py
+-rw-r--r--   0        0        0     1473 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/append_to_stream/mixin.py
+-rw-r--r--   0        0        0      586 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/append_to_stream/types.py
+-rw-r--r--   0        0        0     2659 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/client.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_all/__init__.py
+-rw-r--r--   0        0        0     3239 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_all/grpc.py
+-rw-r--r--   0        0        0     1354 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_all/mixin.py
+-rw-r--r--   0        0        0      835 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_all/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/__init__.py
+-rw-r--r--   0        0        0      463 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/exceptions.py
+-rw-r--r--   0        0        0     4528 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/grpc.py
+-rw-r--r--   0        0        0     1362 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/mixin.py
+-rw-r--r--   0        0        0     1019 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_all/__init__.py
+-rw-r--r--   0        0        0      726 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_all/grpc.py
+-rw-r--r--   0        0        0     1354 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_all/mixin.py
+-rw-r--r--   0        0        0      135 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_all/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.839752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_stream/__init__.py
+-rw-r--r--   0        0        0      816 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_stream/grpc.py
+-rw-r--r--   0        0        0     1444 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_stream/mixin.py
+-rw-r--r--   0        0        0      138 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_stream/types.py
+-rw-r--r--   0        0        0     1027 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/get_persistent_subscription_details/__init__.py
+-rw-r--r--   0        0        0     1610 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/get_persistent_subscription_details/grpc.py
+-rw-r--r--   0        0        0     1595 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/get_persistent_subscription_details/mixin.py
+-rw-r--r--   0        0        0      399 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/get_persistent_subscription_details/types.py
+-rw-r--r--   0        0        0      223 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/protocol.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_all/__init__.py
+-rw-r--r--   0        0        0     2903 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_all/grpc.py
+-rw-r--r--   0        0        0     1060 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_all/mixin.py
+-rw-r--r--   0        0        0      654 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_all/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_stream/__init__.py
+-rw-r--r--   0        0        0     4171 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_stream/grpc.py
+-rw-r--r--   0        0        0     1124 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_stream/mixin.py
+-rw-r--r--   0        0        0      391 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/read_stream/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_all/__init__.py
+-rw-r--r--   0        0        0     3788 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_all/grpc.py
+-rw-r--r--   0        0        0     1308 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_all/mixin.py
+-rw-r--r--   0        0        0      669 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_all/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_all/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_all/grpc.py
+-rw-r--r--   0        0        0     1058 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_all/mixin.py
+-rw-r--r--   0        0        0      341 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_all/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/exceptions.py
+-rw-r--r--   0        0        0     5019 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/grpc.py
+-rw-r--r--   0        0        0     3367 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/mixin.py
+-rw-r--r--   0        0        0      380 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_stream/__init__.py
+-rw-r--r--   0        0        0     2243 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_stream/grpc.py
+-rw-r--r--   0        0        0     1470 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_stream/mixin.py
+-rw-r--r--   0        0        0      341 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/subscribe_to_stream/types.py
+-rw-r--r--   0        0        0     1208 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_all/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_all/grpc.py
+-rw-r--r--   0        0        0     1354 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_all/mixin.py
+-rw-r--r--   0        0        0      268 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_all/types.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_stream/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_stream/exceptions.py
+-rw-r--r--   0        0        0     1710 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_stream/grpc.py
+-rw-r--r--   0        0        0     1444 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_stream/mixin.py
+-rw-r--r--   0        0        0      280 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_stream/types.py
+-rw-r--r--   0        0        0     1423 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/events.py
+-rw-r--r--   0        0        0     1118 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/exceptions.py
+-rw-r--r--   0        0        0      323 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/filters.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/gossip/__init__.py
+-rw-r--r--   0        0        0     2224 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/monitoring/__init__.py
+-rw-r--r--   0        0        0    10616 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/operations/__init__.py
+-rw-r--r--   0        0        0    26972 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/persistent_subscriptions/__init__.py
+-rw-r--r--   0        0        0    18443 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/projections/__init__.py
+-rw-r--r--   0        0        0     4951 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/redaction/__init__.py
+-rw-r--r--   0        0        0     2408 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/server_features/__init__.py
+-rw-r--r--   0        0        0    22069 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/streams/__init__.py
+-rw-r--r--   0        0        0    13872 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/client/users/__init__.py
+-rw-r--r--   0        0        0    22153 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/event_store/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/google/__init__.py
+-rw-r--r--   0        0        0     7745 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/generated/google/rpc/__init__.py
+-rw-r--r--   0        0        0     2409 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/options.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/py.typed
+-rw-r--r--   0        0        0      253 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/subscriptions.py
+-rw-r--r--   0        0        0      358 2024-05-10 19:15:14.843752 eventstoredb-0.9.0/eventstoredb/types.py
+-rw-r--r--   0        0        0     5194 2024-05-10 19:15:38.151659 eventstoredb-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2290 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      738 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/docker-compose.yml
+-rw-r--r--   0        0        0     9527 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_append_to_stream.py
+-rw-r--r--   0        0        0     1126 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_client_options.py
+-rw-r--r--   0        0        0     5447 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_create_persistent_subscription_to_all.py
+-rw-r--r--   0        0        0     4728 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_create_persistent_subscription_to_stream.py
+-rw-r--r--   0        0        0     1312 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_delete_persistent_subscription_to_all.py
+-rw-r--r--   0        0        0     1426 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_delete_persistent_subscription_to_stream.py
+-rw-r--r--   0        0        0     1853 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_get_persistent_subscription_details.py
+-rw-r--r--   0        0        0       73 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_import.py
+-rw-r--r--   0        0        0    13548 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_read_all.py
+-rw-r--r--   0        0        0     6084 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_read_stream.py
+-rw-r--r--   0        0        0    10686 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_subscribe_to_all.py
+-rw-r--r--   0        0        0    14046 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_subscribe_to_persistent_subscription_to_all.py
+-rw-r--r--   0        0        0     3786 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_subscribe_to_persistent_subscription_to_stream.py
+-rw-r--r--   0        0        0     3601 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_subscribe_to_stream.py
+-rw-r--r--   0        0        0     1752 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_update_persistent_subscription_to_all.py
+-rw-r--r--   0        0        0     1865 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/test_update_persistent_subscription_to_stream.py
+-rw-r--r--   0        0        0     3119 2024-05-10 19:15:14.847752 eventstoredb-0.9.0/tests/utils.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 eventstoredb-0.9.0/PKG-INFO
```

### Comparing `eventstoredb-0.8.1/LICENSE` & `eventstoredb-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/README.md` & `eventstoredb-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/append_to_stream/exceptions.py` & `eventstoredb-0.9.0/eventstoredb/client/append_to_stream/exceptions.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/append_to_stream/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/append_to_stream/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/append_to_stream/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/append_to_stream/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/append_to_stream/types.py` & `eventstoredb-0.9.0/eventstoredb/client/append_to_stream/types.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/client.py` & `eventstoredb-0.9.0/eventstoredb/client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 )
 from eventstoredb.client.delete_persistent_subscription_to_all.mixin import (
     DeletePersistentSubscriptionToAllMixin,
 )
 from eventstoredb.client.delete_persistent_subscription_to_stream.mixin import (
     DeletePersistentSubscriptionToStreamMixin,
 )
+from eventstoredb.client.get_persistent_subscription_details.mixin import (
+    GetPersistentSubscriptionDetailsMixin,
+)
 from eventstoredb.client.read_all.mixin import ReadAllMixin
 from eventstoredb.client.read_stream.mixin import ReadStreamMixin
 from eventstoredb.client.subscribe_to_all.mixin import SubscribeToAllMixin
 from eventstoredb.client.subscribe_to_persistent_subscription_to_all.mixin import (
     SubscribeToPersistentSubscriptionToAllMixin,
 )
 from eventstoredb.client.subscribe_to_persistent_subscription_to_stream.mixin import (
@@ -43,14 +46,15 @@
     CreatePersistentSubscriptionToStreamMixin,
     UpdatePersistentSubscriptionToStreamMixin,
     DeletePersistentSubscriptionToStreamMixin,
     SubscribeToPersistentSubscriptionToStreamMixin,
     CreatePersistentSubscriptionToAllMixin,
     UpdatePersistentSubscriptionToAllMixin,
     DeletePersistentSubscriptionToAllMixin,
+    GetPersistentSubscriptionDetailsMixin,
     SubscribeToPersistentSubscriptionToAllMixin,
 ):
     def __init__(self, options: ClientOptions | str) -> None:
         if isinstance(options, str):
             self._options = ClientOptions.from_connection_string(options)
         else:
             self._options = options
```

### Comparing `eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_all/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_all/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_all/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_all/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_all/types.py` & `eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_all/types.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/create_persistent_subscription_to_stream/types.py` & `eventstoredb-0.9.0/eventstoredb/client/create_persistent_subscription_to_stream/types.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_all/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_all/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_all/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_all/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_stream/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_stream/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/delete_persistent_subscription_to_stream/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/delete_persistent_subscription_to_stream/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/exceptions.py` & `eventstoredb-0.9.0/eventstoredb/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/read_all/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/read_all/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/read_all/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/read_all/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/read_all/types.py` & `eventstoredb-0.9.0/eventstoredb/client/read_all/types.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/read_stream/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/read_stream/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/read_stream/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/read_stream/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_all/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_all/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_all/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_all/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_all/types.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_all/types.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_all/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_all/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_all/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_all/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_persistent_subscription_to_stream/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_stream/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_stream/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/subscribe_to_stream/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/subscribe_to_stream/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/types.py` & `eventstoredb-0.9.0/eventstoredb/client/types.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_all/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_all/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_all/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_all/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_stream/grpc.py` & `eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_stream/grpc.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/client/update_persistent_subscription_to_stream/mixin.py` & `eventstoredb-0.9.0/eventstoredb/client/update_persistent_subscription_to_stream/mixin.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/events.py` & `eventstoredb-0.9.0/eventstoredb/events.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/exceptions.py` & `eventstoredb-0.9.0/eventstoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/gossip/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/gossip/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/monitoring/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/operations/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/persistent_subscriptions/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/persistent_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/projections/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/redaction/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/redaction/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/server_features/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/server_features/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/streams/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/client/users/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/client/users/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/event_store/cluster/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/event_store/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/generated/google/rpc/__init__.py` & `eventstoredb-0.9.0/eventstoredb/generated/google/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/eventstoredb/options.py` & `eventstoredb-0.9.0/eventstoredb/options.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/pyproject.toml` & `eventstoredb-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Typing :: Typed",
 ]
 dynamic = []
 dependencies = [
     "betterproto==2.0.0b5",
     "yarl>=1.9.4",
 ]
-version = "0.8.1"
+version = "0.9.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://github.com/betaboon/EventStoreDB-Client-Python"
 Documentation = "https://betaboon.github.io/EventStoreDB-Client-Python"
```

### Comparing `eventstoredb-0.8.1/tests/conftest.py` & `eventstoredb-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/docker-compose.yml` & `eventstoredb-0.9.0/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_append_to_stream.py` & `eventstoredb-0.9.0/tests/test_append_to_stream.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_client_options.py` & `eventstoredb-0.9.0/tests/test_client_options.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_create_persistent_subscription_to_all.py` & `eventstoredb-0.9.0/tests/test_create_persistent_subscription_to_all.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_create_persistent_subscription_to_stream.py` & `eventstoredb-0.9.0/tests/test_create_persistent_subscription_to_stream.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_delete_persistent_subscription_to_all.py` & `eventstoredb-0.9.0/tests/test_delete_persistent_subscription_to_all.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_delete_persistent_subscription_to_stream.py` & `eventstoredb-0.9.0/tests/test_delete_persistent_subscription_to_stream.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_read_all.py` & `eventstoredb-0.9.0/tests/test_read_all.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_read_stream.py` & `eventstoredb-0.9.0/tests/test_read_stream.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_subscribe_to_all.py` & `eventstoredb-0.9.0/tests/test_subscribe_to_all.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_subscribe_to_persistent_subscription_to_all.py` & `eventstoredb-0.9.0/tests/test_subscribe_to_persistent_subscription_to_all.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_subscribe_to_persistent_subscription_to_stream.py` & `eventstoredb-0.9.0/tests/test_subscribe_to_persistent_subscription_to_stream.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_subscribe_to_stream.py` & `eventstoredb-0.9.0/tests/test_subscribe_to_stream.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_update_persistent_subscription_to_all.py` & `eventstoredb-0.9.0/tests/test_update_persistent_subscription_to_all.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/test_update_persistent_subscription_to_stream.py` & `eventstoredb-0.9.0/tests/test_update_persistent_subscription_to_stream.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/tests/utils.py` & `eventstoredb-0.9.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `eventstoredb-0.8.1/PKG-INFO` & `eventstoredb-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: eventstoredb
-Version: 0.8.1
+Version: 0.9.0
 Summary: A EventstoreDB gRPC client written in python .
-Keywords: eventstore eventstoredb
+Keywords: eventstore,eventstoredb
 Author-Email: betaboon <betaboon@0x80.ninja>
 Maintainer-Email: betaboon <betaboon@0x80.ninja>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

