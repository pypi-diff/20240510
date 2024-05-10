# Comparing `tmp/duwi_smart_sdk-0.2.1.tar.gz` & `tmp/duwi_smart_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.2.1.tar", last modified: Thu May  9 05:15:48 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.2.2.tar", last modified: Thu May  9 07:52:58 2024, max compression
```

## Comparing `duwi_smart_sdk-0.2.1.tar` & `duwi_smart_sdk-0.2.2.tar`

### file list

```diff
@@ -1,55 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.935298 duwi_smart_sdk-0.2.1/
--rw-rw-rw-   0        0        0      885 2024-05-09 05:15:48.935298 duwi_smart_sdk-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-05-09 02:50:27.000000 duwi_smart_sdk-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.879988 duwi_smart_sdk-0.2.1/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.898480 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2098 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4514 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2686 2024-05-07 09:08:05.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2156 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4788 2024-05-07 07:31:40.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.902895 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.905404 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.907363 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.913222 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.918801 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.888945 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      885 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 05:15:48.936400 duwi_smart_sdk-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      937 2024-05-09 05:15:42.000000 duwi_smart_sdk-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.920760 duwi_smart_sdk-0.2.1/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.927711 duwi_smart_sdk-0.2.1/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.1/test/api/__init__.py
--rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.1/test/api/test_control.py
--rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.1/test/api/test_discover.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.1/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.1/test/api/test_login.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.1/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.930667 duwi_smart_sdk-0.2.1/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.1/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.158641 duwi_smart_sdk-0.2.2/
+-rw-rw-rw-   0        0        0      885 2024-05-09 07:52:58.158641 duwi_smart_sdk-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-05-09 02:50:27.000000 duwi_smart_sdk-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.102805 duwi_smart_sdk-0.2.2/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.121001 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2098 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4514 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2658 2024-05-09 07:48:49.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/floor.py
+-rw-rw-rw-   0        0        0     2686 2024-05-07 09:08:05.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2156 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2787 2024-05-09 07:30:47.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/room.py
+-rw-rw-rw-   0        0        0     4788 2024-05-07 07:31:40.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.125440 duwi_smart_sdk-0.2.2/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.127393 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.129346 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.139112 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0      626 2024-05-09 07:51:45.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/floor.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/room.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.143017 duwi_smart_sdk-0.2.2/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.109640 duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      885 2024-05-09 07:52:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1396 2024-05-09 07:52:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:52:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-09 07:52:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-09 07:52:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 07:52:58.000000 duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:52:58.159617 duwi_smart_sdk-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-09 07:52:55.000000 duwi_smart_sdk-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.143993 duwi_smart_sdk-0.2.2/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.153757 duwi_smart_sdk-0.2.2/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.2/test/api/__init__.py
+-rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.2/test/api/test_control.py
+-rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.2/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.2.2/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.2/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.2/test/api/test_login.py
+-rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.2.2/test/api/test_room.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.2/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:52:58.156688 duwi_smart_sdk-0.2.2/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.2/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.2/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.2.1/PKG-INFO` & `duwi_smart_sdk-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.2.2/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,35 +7,41 @@
 duwi_smart_sdk.egg-info/entry_points.txt
 duwi_smart_sdk.egg-info/requires.txt
 duwi_smart_sdk.egg-info/top_level.txt
 duwi_smart_sdk/api/__init__.py
 duwi_smart_sdk/api/account.py
 duwi_smart_sdk/api/control.py
 duwi_smart_sdk/api/discover.py
+duwi_smart_sdk/api/floor.py
 duwi_smart_sdk/api/house.py
 duwi_smart_sdk/api/refresh_token.py
+duwi_smart_sdk/api/room.py
 duwi_smart_sdk/api/ws.py
 duwi_smart_sdk/const/__init__.py
 duwi_smart_sdk/const/const.py
 duwi_smart_sdk/const/status.py
 duwi_smart_sdk/const/type_map.py
 duwi_smart_sdk/model/__init__.py
 duwi_smart_sdk/model/req/__init__.py
 duwi_smart_sdk/model/req/device_control.py
 duwi_smart_sdk/model/resp/__init__.py
 duwi_smart_sdk/model/resp/auth.py
 duwi_smart_sdk/model/resp/control.py
 duwi_smart_sdk/model/resp/device.py
+duwi_smart_sdk/model/resp/floor.py
 duwi_smart_sdk/model/resp/house.py
+duwi_smart_sdk/model/resp/room.py
 duwi_smart_sdk/util/__init__.py
 duwi_smart_sdk/util/http.py
 duwi_smart_sdk/util/sign.py
 duwi_smart_sdk/util/timestamp.py
 test/__init__.py
 test/api/__init__.py
 test/api/test_control.py
 test/api/test_discover.py
+test/api/test_floor.py
 test/api/test_house.py
 test/api/test_login.py
+test/api/test_room.py
 test/api/test_ws.py
 test/util/__init__.py
 test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.2.1/setup.py` & `duwi_smart_sdk-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.01'
+VERSION = '0.2.2'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.2.1/test/api/test_control.py` & `duwi_smart_sdk-0.2.2/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/test/api/test_discover.py` & `duwi_smart_sdk-0.2.2/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/test/api/test_house.py` & `duwi_smart_sdk-0.2.2/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/test/api/test_login.py` & `duwi_smart_sdk-0.2.2/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/test/api/test_ws.py` & `duwi_smart_sdk-0.2.2/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.1/test/util/test_http.py` & `duwi_smart_sdk-0.2.2/test/util/test_http.py`

 * *Files identical despite different names*

