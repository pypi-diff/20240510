# Comparing `tmp/celitech_sdk-1.1.56.tar.gz` & `tmp/celitech_sdk-1.1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech_sdk-1.1.56.tar", last modified: Tue May  7 17:37:31 2024, max compression
+gzip compressed data, was "celitech_sdk-1.1.57.tar", last modified: Fri May 10 09:37:46 2024, max compression
```

## Comparing `celitech_sdk-1.1.56.tar` & `celitech_sdk-1.1.57.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.207803 celitech_sdk-1.1.56/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14758 2024-05-07 17:37:31.207803 celitech_sdk-1.1.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:37:31.207803 celitech_sdk-1.1.56/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.191803 celitech_sdk-1.1.56/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.191803 celitech_sdk-1.1.56/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.191803 celitech_sdk-1.1.56/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.195803 celitech_sdk-1.1.56/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.199803 celitech_sdk-1.1.56/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.199803 celitech_sdk-1.1.56/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.199803 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-07 17:37:19.000000 celitech_sdk-1.1.56/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:31.203803 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14758 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 17:37:31.000000 celitech_sdk-1.1.56/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.328387 celitech_sdk-1.1.57/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.332387 celitech_sdk-1.1.57/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.332387 celitech_sdk-1.1.57/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.332387 celitech_sdk-1.1.57/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech_sdk-1.1.56/LICENSE` & `celitech_sdk-1.1.57/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/PKG-INFO` & `celitech_sdk-1.1.57/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: celitech-sdk
-Version: 1.1.56
-Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Celitech Python SDK 1.1.56
+# Celitech Python SDK 1.1.57
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.56
+- SDK version: 1.1.57
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -191,30 +181,38 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases`
 
 **Parameters**
 
 | Name         | Type                  | Required | Description       |
 | :----------- | :-------------------- | :------: | :---------------- |
-| request_body | CreatePurchaseRequest |    ❌    | The request body. |
+| request_body | CreatePurchaseRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import CreatePurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.create_purchase()
+request_body = CreatePurchaseRequest(
+    destination="FRA",
+    data_limit_in_gb=1,
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
 #### **top_up_esim**
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
@@ -222,30 +220,38 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases/topup`
 
 **Parameters**
 
 | Name         | Type             | Required | Description       |
 | :----------- | :--------------- | :------: | :---------------- |
-| request_body | TopUpEsimRequest |    ❌    | The request body. |
+| request_body | TopUpEsimRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import TopUpEsimRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.top_up_esim()
+request_body = TopUpEsimRequest(
+    iccid="1111222233334444555",
+    data_limit_in_gb=1,
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
 #### **edit_purchase**
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
@@ -253,30 +259,37 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases/edit`
 
 **Parameters**
 
 | Name         | Type                | Required | Description       |
 | :----------- | :------------------ | :------: | :---------------- |
-| request_body | EditPurchaseRequest |    ❌    | The request body. |
+| request_body | EditPurchaseRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import EditPurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.edit_purchase()
+request_body = EditPurchaseRequest(
+    purchase_id="ae471106-c8b4-42cf-b83a-b061291f2922",
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_purchase_consumption**
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
```

### Comparing `celitech_sdk-1.1.56/README.md` & `celitech_sdk-1.1.57/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# Celitech Python SDK 1.1.56
+Metadata-Version: 2.1
+Name: celitech-sdk
+Version: 1.1.57
+Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Celitech Python SDK 1.1.57
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.56
+- SDK version: 1.1.57
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -181,30 +191,38 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases`
 
 **Parameters**
 
 | Name         | Type                  | Required | Description       |
 | :----------- | :-------------------- | :------: | :---------------- |
-| request_body | CreatePurchaseRequest |    ❌    | The request body. |
+| request_body | CreatePurchaseRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import CreatePurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.create_purchase()
+request_body = CreatePurchaseRequest(
+    destination="FRA",
+    data_limit_in_gb=1,
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
 #### **top_up_esim**
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
@@ -212,30 +230,38 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases/topup`
 
 **Parameters**
 
 | Name         | Type             | Required | Description       |
 | :----------- | :--------------- | :------: | :---------------- |
-| request_body | TopUpEsimRequest |    ❌    | The request body. |
+| request_body | TopUpEsimRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import TopUpEsimRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.top_up_esim()
+request_body = TopUpEsimRequest(
+    iccid="1111222233334444555",
+    data_limit_in_gb=1,
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
 #### **edit_purchase**
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
@@ -243,30 +269,37 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases/edit`
 
 **Parameters**
 
 | Name         | Type                | Required | Description       |
 | :----------- | :------------------ | :------: | :---------------- |
-| request_body | EditPurchaseRequest |    ❌    | The request body. |
+| request_body | EditPurchaseRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import EditPurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.edit_purchase()
+request_body = EditPurchaseRequest(
+    purchase_id="ae471106-c8b4-42cf-b83a-b061291f2922",
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_purchase_consumption**
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
```

### Comparing `celitech_sdk-1.1.56/src/celitech/hooks/hook.py` & `celitech_sdk-1.1.57/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/__init__.py` & `celitech_sdk-1.1.57/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/base.py` & `celitech_sdk-1.1.57/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/create_purchase_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/create_purchase_request.py` & `celitech_sdk-1.1.57/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/edit_purchase_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/edit_purchase_request.py` & `celitech_sdk-1.1.57/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/get_esim_device_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/get_esim_history_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/get_esim_mac_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/get_esim_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/list_destinations_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/list_packages_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/list_purchases_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/top_up_esim_ok_response.py` & `celitech_sdk-1.1.57/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/top_up_esim_request.py` & `celitech_sdk-1.1.57/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/utils/cast_models.py` & `celitech_sdk-1.1.57/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/models/utils/json_map.py` & `celitech_sdk-1.1.57/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/request_chain/request_chain.py` & `celitech_sdk-1.1.57/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/transport/request.py` & `celitech_sdk-1.1.57/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/transport/request_error.py` & `celitech_sdk-1.1.57/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/transport/response.py` & `celitech_sdk-1.1.57/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/transport/serializer.py` & `celitech_sdk-1.1.57/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/net/transport/utils.py` & `celitech_sdk-1.1.57/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/sdk.py` & `celitech_sdk-1.1.57/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/services/destinations.py` & `celitech_sdk-1.1.57/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/services/e_sim.py` & `celitech_sdk-1.1.57/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/services/packages.py` & `celitech_sdk-1.1.57/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/services/purchases.py` & `celitech_sdk-1.1.57/src/celitech/services/purchases.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,82 +73,82 @@
 
         response = self.send_request(serialized_request)
 
         return ListPurchasesOkResponse._unmap(response)
 
     @cast_models
     def create_purchase(
-        self, request_body: CreatePurchaseRequest = None
+        self, request_body: CreatePurchaseRequest
     ) -> CreatePurchaseOkResponse:
         """This endpoint is used to purchase a new eSIM by providing the package details.
 
-        :param request_body: The request body., defaults to None
-        :type request_body: CreatePurchaseRequest, optional
+        :param request_body: The request body.
+        :type request_body: CreatePurchaseRequest
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: CreatePurchaseOkResponse
         """
 
-        Validator(CreatePurchaseRequest).is_optional().validate(request_body)
+        Validator(CreatePurchaseRequest).validate(request_body)
 
         serialized_request = (
             Serializer(f"{self.base_url}/purchases", self.get_default_headers())
             .serialize()
             .set_method("POST")
             .set_body(request_body)
         )
 
         response = self.send_request(serialized_request)
 
         return CreatePurchaseOkResponse._unmap(response)
 
     @cast_models
-    def top_up_esim(self, request_body: TopUpEsimRequest = None) -> TopUpEsimOkResponse:
+    def top_up_esim(self, request_body: TopUpEsimRequest) -> TopUpEsimOkResponse:
         """This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
 
-        :param request_body: The request body., defaults to None
-        :type request_body: TopUpEsimRequest, optional
+        :param request_body: The request body.
+        :type request_body: TopUpEsimRequest
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: TopUpEsimOkResponse
         """
 
-        Validator(TopUpEsimRequest).is_optional().validate(request_body)
+        Validator(TopUpEsimRequest).validate(request_body)
 
         serialized_request = (
             Serializer(f"{self.base_url}/purchases/topup", self.get_default_headers())
             .serialize()
             .set_method("POST")
             .set_body(request_body)
         )
 
         response = self.send_request(serialized_request)
 
         return TopUpEsimOkResponse._unmap(response)
 
     @cast_models
     def edit_purchase(
-        self, request_body: EditPurchaseRequest = None
+        self, request_body: EditPurchaseRequest
     ) -> EditPurchaseOkResponse:
         """This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
 
-        :param request_body: The request body., defaults to None
-        :type request_body: EditPurchaseRequest, optional
+        :param request_body: The request body.
+        :type request_body: EditPurchaseRequest
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: EditPurchaseOkResponse
         """
 
-        Validator(EditPurchaseRequest).is_optional().validate(request_body)
+        Validator(EditPurchaseRequest).validate(request_body)
 
         serialized_request = (
             Serializer(f"{self.base_url}/purchases/edit", self.get_default_headers())
             .serialize()
             .set_method("POST")
             .set_body(request_body)
         )
```

### Comparing `celitech_sdk-1.1.56/src/celitech/services/utils/base_service.py` & `celitech_sdk-1.1.57/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/services/utils/default_headers.py` & `celitech_sdk-1.1.57/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech/services/utils/validator.py` & `celitech_sdk-1.1.57/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.56/src/celitech_sdk.egg-info/PKG-INFO` & `celitech_sdk-1.1.57/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.56
+Version: 1.1.57
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.56
+# Celitech Python SDK 1.1.57
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.56
+- SDK version: 1.1.57
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -191,30 +191,38 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases`
 
 **Parameters**
 
 | Name         | Type                  | Required | Description       |
 | :----------- | :-------------------- | :------: | :---------------- |
-| request_body | CreatePurchaseRequest |    ❌    | The request body. |
+| request_body | CreatePurchaseRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import CreatePurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.create_purchase()
+request_body = CreatePurchaseRequest(
+    destination="FRA",
+    data_limit_in_gb=1,
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
 #### **top_up_esim**
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
@@ -222,30 +230,38 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases/topup`
 
 **Parameters**
 
 | Name         | Type             | Required | Description       |
 | :----------- | :--------------- | :------: | :---------------- |
-| request_body | TopUpEsimRequest |    ❌    | The request body. |
+| request_body | TopUpEsimRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import TopUpEsimRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.top_up_esim()
+request_body = TopUpEsimRequest(
+    iccid="1111222233334444555",
+    data_limit_in_gb=1,
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
 #### **edit_purchase**
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
@@ -253,30 +269,37 @@
 - HTTP Method: `POST`
 - Endpoint: `/purchases/edit`
 
 **Parameters**
 
 | Name         | Type                | Required | Description       |
 | :----------- | :------------------ | :------: | :---------------- |
-| request_body | EditPurchaseRequest |    ❌    | The request body. |
+| request_body | EditPurchaseRequest |    ✅    | The request body. |
 
 **Return Type**
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
+from celitech.models import EditPurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.edit_purchase()
+request_body = EditPurchaseRequest(
+    purchase_id="ae471106-c8b4-42cf-b83a-b061291f2922",
+    start_date="2023-11-01",
+    end_date="2023-11-20"
+)
+
+result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_purchase_consumption**
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
```

### Comparing `celitech_sdk-1.1.56/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech_sdk-1.1.57/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

