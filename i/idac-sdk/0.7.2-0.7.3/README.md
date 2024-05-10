# Comparing `tmp/idac_sdk-0.7.2.tar.gz` & `tmp/idac_sdk-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idac_sdk-0.7.2.tar", last modified: Fri Jul 14 10:01:57 2023, max compression
+gzip compressed data, was "idac_sdk-0.7.3.tar", last modified: Fri May 10 09:16:01 2024, max compression
```

## Comparing `idac_sdk-0.7.2.tar` & `idac_sdk-0.7.3.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.364268 idac_sdk-0.7.2/
--rw-r--r--   0 duferrei   (501) staff       (20)      847 2023-07-14 10:01:57.363959 idac_sdk-0.7.2/PKG-INFO
--rw-r--r--   0 duferrei   (501) staff       (20)      126 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/README.md
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.343703 idac_sdk-0.7.2/idac_sdk/
--rw-r--r--   0 duferrei   (501) staff       (20)      513 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)       22 2023-07-14 10:01:52.000000 idac_sdk-0.7.2/idac_sdk/_version.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.349039 idac_sdk-0.7.2/idac_sdk/asynced/
--rw-r--r--   0 duferrei   (501) staff       (20)       39 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/asynced/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)     3191 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/asynced/controller.py
--rw-r--r--   0 duferrei   (501) staff       (20)    13215 2023-07-13 17:03:00.000000 idac_sdk-0.7.2/idac_sdk/asynced/request.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.350138 idac_sdk-0.7.2/idac_sdk/base/
--rw-r--r--   0 duferrei   (501) staff       (20)      775 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/base/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)    10216 2023-07-13 17:01:39.000000 idac_sdk-0.7.2/idac_sdk/base/controller.py
--rw-r--r--   0 duferrei   (501) staff       (20)     6462 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/base/request.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.351024 idac_sdk-0.7.2/idac_sdk/cli/
--rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/__init__.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.354174 idac_sdk-0.7.2/idac_sdk/cli/commands/
--rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)      971 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/cleanup.py
--rw-r--r--   0 duferrei   (501) staff       (20)     4674 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/config.py
--rw-r--r--   0 duferrei   (501) staff       (20)     5164 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/create.py
--rw-r--r--   0 duferrei   (501) staff       (20)      854 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/extend.py
--rw-r--r--   0 duferrei   (501) staff       (20)      754 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/restart.py
--rw-r--r--   0 duferrei   (501) staff       (20)     1685 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/status.py
--rw-r--r--   0 duferrei   (501) staff       (20)      941 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/idac.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.355968 idac_sdk-0.7.2/idac_sdk/cli/lib/
--rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)     2100 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/_controller_options.py
--rw-r--r--   0 duferrei   (501) staff       (20)     2512 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/_helpers.py
--rw-r--r--   0 duferrei   (501) staff       (20)     2563 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/_vpn_options.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.356491 idac_sdk-0.7.2/idac_sdk/config/
--rw-r--r--   0 duferrei   (501) staff       (20)     2219 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/config/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)      832 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/errors.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.357455 idac_sdk-0.7.2/idac_sdk/lib/
--rw-r--r--   0 duferrei   (501) staff       (20)        0 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/lib/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)      646 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/lib/_helpers.py
--rw-r--r--   0 duferrei   (501) staff       (20)      703 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/log.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.361503 idac_sdk-0.7.2/idac_sdk/models/
--rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/models/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)      123 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/auth.py
--rw-r--r--   0 duferrei   (501) staff       (20)      435 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/config.py
--rw-r--r--   0 duferrei   (501) staff       (20)      460 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/models/new_request.py
--rw-r--r--   0 duferrei   (501) staff       (20)     3344 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/request_state.py
--rw-r--r--   0 duferrei   (501) staff       (20)      758 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/vpn_config.py
--rw-r--r--   0 duferrei   (501) staff       (20)     6204 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/session_data.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.363368 idac_sdk-0.7.2/idac_sdk/synced/
--rw-r--r--   0 duferrei   (501) staff       (20)       38 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/synced/__init__.py
--rw-r--r--   0 duferrei   (501) staff       (20)     3302 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/synced/controller.py
--rw-r--r--   0 duferrei   (501) staff       (20)    13039 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/synced/request.py
--rw-r--r--   0 duferrei   (501) staff       (20)      734 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/types.py
-drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.347521 idac_sdk-0.7.2/idac_sdk.egg-info/
--rw-r--r--   0 duferrei   (501) staff       (20)      847 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/PKG-INFO
--rw-r--r--   0 duferrei   (501) staff       (20)     1239 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 duferrei   (501) staff       (20)        1 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 duferrei   (501) staff       (20)       49 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/entry_points.txt
--rw-r--r--   0 duferrei   (501) staff       (20)      125 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/requires.txt
--rw-r--r--   0 duferrei   (501) staff       (20)        9 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/top_level.txt
--rw-r--r--   0 duferrei   (501) staff       (20)       38 2023-07-14 10:01:57.364395 idac_sdk-0.7.2/setup.cfg
--rw-r--r--   0 duferrei   (501) staff       (20)     1695 2023-07-14 10:00:40.000000 idac_sdk-0.7.2/setup.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.320686 idac_sdk-0.7.3/
+-rw-r--r--   0 duferrei   (501) staff       (20)     1062 2024-05-10 09:16:01.319706 idac_sdk-0.7.3/PKG-INFO
+-rw-r--r--   0 duferrei   (501) staff       (20)      126 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/README.md
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.266927 idac_sdk-0.7.3/idac_sdk/
+-rw-r--r--   0 duferrei   (501) staff       (20)      513 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)       22 2024-05-10 09:15:52.000000 idac_sdk-0.7.3/idac_sdk/_version.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.280164 idac_sdk-0.7.3/idac_sdk/asynced/
+-rw-r--r--   0 duferrei   (501) staff       (20)       39 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/asynced/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     3191 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/asynced/controller.py
+-rw-r--r--   0 duferrei   (501) staff       (20)    13215 2023-07-13 17:03:00.000000 idac_sdk-0.7.3/idac_sdk/asynced/request.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.285209 idac_sdk-0.7.3/idac_sdk/base/
+-rw-r--r--   0 duferrei   (501) staff       (20)      775 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/base/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)    10216 2023-07-13 17:01:39.000000 idac_sdk-0.7.3/idac_sdk/base/controller.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     6462 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/base/request.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.287330 idac_sdk-0.7.3/idac_sdk/cli/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/cli/__init__.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.297074 idac_sdk-0.7.3/idac_sdk/cli/commands/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/cli/commands/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      971 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/cli/commands/cleanup.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     4674 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/cli/commands/config.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     5164 2023-07-13 12:57:28.000000 idac_sdk-0.7.3/idac_sdk/cli/commands/create.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      854 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/cli/commands/extend.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      754 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/cli/commands/restart.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     1685 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/cli/commands/status.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      941 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/cli/idac.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.300818 idac_sdk-0.7.3/idac_sdk/cli/lib/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/cli/lib/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     2100 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/cli/lib/_controller_options.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     2512 2023-07-13 12:57:28.000000 idac_sdk-0.7.3/idac_sdk/cli/lib/_helpers.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     2563 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/cli/lib/_vpn_options.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.301772 idac_sdk-0.7.3/idac_sdk/config/
+-rw-r--r--   0 duferrei   (501) staff       (20)     2219 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/config/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      832 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/errors.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.303474 idac_sdk-0.7.3/idac_sdk/lib/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/lib/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      646 2023-07-13 12:57:28.000000 idac_sdk-0.7.3/idac_sdk/lib/_helpers.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      703 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/log.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.310094 idac_sdk-0.7.3/idac_sdk/models/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/models/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      123 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/models/auth.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      435 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/models/config.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      460 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/models/new_request.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     3344 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/models/request_state.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      758 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/models/vpn_config.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     6204 2023-07-13 12:57:28.000000 idac_sdk-0.7.3/idac_sdk/session_data.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.312984 idac_sdk-0.7.3/idac_sdk/synced/
+-rw-r--r--   0 duferrei   (501) staff       (20)       38 2022-03-16 10:33:13.000000 idac_sdk-0.7.3/idac_sdk/synced/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     3302 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/synced/controller.py
+-rw-r--r--   0 duferrei   (501) staff       (20)    13196 2024-05-10 08:54:10.000000 idac_sdk-0.7.3/idac_sdk/synced/request.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      734 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/idac_sdk/types.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.318158 idac_sdk-0.7.3/idac_sdk.egg-info/
+-rw-r--r--   0 duferrei   (501) staff       (20)     1062 2024-05-10 09:16:01.000000 idac_sdk-0.7.3/idac_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 duferrei   (501) staff       (20)     1278 2024-05-10 09:16:01.000000 idac_sdk-0.7.3/idac_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)        1 2024-05-10 09:16:01.000000 idac_sdk-0.7.3/idac_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)       48 2024-05-10 09:16:01.000000 idac_sdk-0.7.3/idac_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)      125 2024-05-10 09:16:01.000000 idac_sdk-0.7.3/idac_sdk.egg-info/requires.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)        9 2024-05-10 09:16:01.000000 idac_sdk-0.7.3/idac_sdk.egg-info/top_level.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)       38 2024-05-10 09:16:01.320966 idac_sdk-0.7.3/setup.cfg
+-rw-r--r--   0 duferrei   (501) staff       (20)     1699 2024-05-10 08:54:37.000000 idac_sdk-0.7.3/setup.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2024-05-10 09:16:01.316297 idac_sdk-0.7.3/tests/
+-rw-r--r--   0 duferrei   (501) staff       (20)     5788 2023-07-13 17:03:05.000000 idac_sdk-0.7.3/tests/test_async.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     7111 2023-01-16 09:47:06.000000 idac_sdk-0.7.3/tests/test_sync.py
```

### Comparing `idac_sdk-0.7.2/PKG-INFO` & `idac_sdk-0.7.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: idac_sdk
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python 3 SDK for iDAC
 Home-page: https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python
 Author: Cisco GDE CAT
 Author-email: cat-dev-support@cisco.com
 License: MIT
 Keywords: idac sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Requires-Dist: asyncclick>=8.0.3.2
+Requires-Dist: httpx>=0.22.0
+Requires-Dist: xmltodict>=0.12.0
+Requires-Dist: pydantic<2.0.0,>=1.9.0
+Requires-Dist: deepmerge>=1.0.1
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: jsonpath-ng>=1.5.3
 
 # Python3 SDK for iDAC
 
 Docs are available [here](https://www-github.cisco.com/pages/GDE-Content-Engineering/idac-sdk-python/)
-
```

### Comparing `idac_sdk-0.7.2/idac_sdk/__init__.py` & `idac_sdk-0.7.3/idac_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/asynced/controller.py` & `idac_sdk-0.7.3/idac_sdk/asynced/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/asynced/request.py` & `idac_sdk-0.7.3/idac_sdk/asynced/request.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/base/__init__.py` & `idac_sdk-0.7.3/idac_sdk/base/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/base/controller.py` & `idac_sdk-0.7.3/idac_sdk/base/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/base/request.py` & `idac_sdk-0.7.3/idac_sdk/base/request.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/commands/cleanup.py` & `idac_sdk-0.7.3/idac_sdk/cli/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/commands/config.py` & `idac_sdk-0.7.3/idac_sdk/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/commands/create.py` & `idac_sdk-0.7.3/idac_sdk/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/commands/extend.py` & `idac_sdk-0.7.3/idac_sdk/cli/commands/extend.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/commands/restart.py` & `idac_sdk-0.7.3/idac_sdk/cli/commands/restart.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/commands/status.py` & `idac_sdk-0.7.3/idac_sdk/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/idac.py` & `idac_sdk-0.7.3/idac_sdk/cli/idac.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/lib/_controller_options.py` & `idac_sdk-0.7.3/idac_sdk/cli/lib/_controller_options.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/lib/_helpers.py` & `idac_sdk-0.7.3/idac_sdk/cli/lib/_helpers.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/cli/lib/_vpn_options.py` & `idac_sdk-0.7.3/idac_sdk/cli/lib/_vpn_options.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/config/__init__.py` & `idac_sdk-0.7.3/idac_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/errors.py` & `idac_sdk-0.7.3/idac_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/lib/_helpers.py` & `idac_sdk-0.7.3/idac_sdk/lib/_helpers.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/log.py` & `idac_sdk-0.7.3/idac_sdk/log.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/models/request_state.py` & `idac_sdk-0.7.3/idac_sdk/models/request_state.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/models/vpn_config.py` & `idac_sdk-0.7.3/idac_sdk/models/vpn_config.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/session_data.py` & `idac_sdk-0.7.3/idac_sdk/session_data.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/synced/controller.py` & `idac_sdk-0.7.3/idac_sdk/synced/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk/synced/request.py` & `idac_sdk-0.7.3/idac_sdk/synced/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from httpx import Client, Request
+from httpx import Client, Request, ReadTimeout
 import json
 from typing import Dict, List, Optional, Tuple, Union
 
 from idac_sdk.base import (
     DEFAULT_MAX_TRIES,
     DEFAULT_WAIT_INTERVAL,
     REQUEST_ERROR_STATES,
@@ -321,18 +321,21 @@
             raise NoIdError("No ID/UUID provided for Wait For Status")
 
         wanted_state = self.sanitize_states(wanted_state)
 
         def try_infinite() -> RequestState:
             for attempt in range(1, max_attempts + 1):
                 logger.debug(f"Attempt #{attempt} of {max_attempts}")
-                st = self.get_state()
-                status = IDACRequestStatus(st.status)
-                if status in wanted_state:
-                    return st
-                if stop_on_error and status in REQUEST_ERROR_STATES:
-                    raise IDACRequestStateError(f"Request landed in error state: {status.value}")
-                logger.debug(f"Going to sleep for {interval} seconds")
+                try:
+                    st = self.get_state()
+                    status = IDACRequestStatus(st.status)
+                    if status in wanted_state:
+                        return st
+                    if stop_on_error and status in REQUEST_ERROR_STATES:
+                        raise IDACRequestStateError(f"Request landed in error state: {status.value}")
+                    logger.debug(f"Going to sleep for {interval} seconds")
+                except ReadTimeout as e:
+                    logger.debug(f"Got timeout: {e}")
                 time.sleep(interval)
             raise TimeoutError("Max amount of attempts reached")
 
         return try_infinite()
```

### Comparing `idac_sdk-0.7.2/idac_sdk/types.py` & `idac_sdk-0.7.3/idac_sdk/types.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.2/idac_sdk.egg-info/PKG-INFO` & `idac_sdk-0.7.3/idac_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
-Name: idac-sdk
-Version: 0.7.2
+Name: idac_sdk
+Version: 0.7.3
 Summary: Python 3 SDK for iDAC
 Home-page: https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python
 Author: Cisco GDE CAT
 Author-email: cat-dev-support@cisco.com
 License: MIT
 Keywords: idac sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Requires-Dist: asyncclick>=8.0.3.2
+Requires-Dist: httpx>=0.22.0
+Requires-Dist: xmltodict>=0.12.0
+Requires-Dist: pydantic<2.0.0,>=1.9.0
+Requires-Dist: deepmerge>=1.0.1
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: jsonpath-ng>=1.5.3
 
 # Python3 SDK for iDAC
 
 Docs are available [here](https://www-github.cisco.com/pages/GDE-Content-Engineering/idac-sdk-python/)
-
```

### Comparing `idac_sdk-0.7.2/idac_sdk.egg-info/SOURCES.txt` & `idac_sdk-0.7.3/idac_sdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -38,8 +38,10 @@
 idac_sdk/models/auth.py
 idac_sdk/models/config.py
 idac_sdk/models/new_request.py
 idac_sdk/models/request_state.py
 idac_sdk/models/vpn_config.py
 idac_sdk/synced/__init__.py
 idac_sdk/synced/controller.py
-idac_sdk/synced/request.py
+idac_sdk/synced/request.py
+tests/test_async.py
+tests/test_sync.py
```

### Comparing `idac_sdk-0.7.2/setup.py` & `idac_sdk-0.7.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         "httpx>=0.22.0",
         "xmltodict>=0.12.0",
         "pydantic>=1.9.0,<2.0.0",
         "deepmerge>=1.0.1",
         "PyYAML>=5.4.1",
         "jsonpath-ng>=1.5.3",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.10",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     entry_points={"console_scripts": ["idac = idac_sdk.cli.idac:main"]},
 )
```

