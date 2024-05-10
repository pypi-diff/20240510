# Comparing `tmp/qlv-client-0.2.3.tar.gz` & `tmp/qlv-client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.2.3.tar", last modified: Fri May 10 03:54:29 2024, max compression
+gzip compressed data, was "qlv-client-0.2.4.tar", last modified: Fri May 10 05:14:29 2024, max compression
```

## Comparing `qlv-client-0.2.3.tar` & `qlv-client-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:54:29.925753 qlv-client-0.2.3/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      456 2024-05-10 03:54:29.925257 qlv-client-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 03:54:29.922773 qlv-client-0.2.3/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.3/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.3/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.2.3/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.3/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.3/qlv_client/http_client.py
--rw-rw-rw-   0        0        0    10291 2024-05-10 03:54:21.000000 qlv-client-0.2.3/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.3/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.3/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.3/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:54:29.924761 qlv-client-0.2.3/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 03:54:29.925753 qlv-client-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-10 03:54:25.000000 qlv-client-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:14:29.372692 qlv-client-0.2.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-05-10 05:14:29.372692 qlv-client-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 05:14:29.370209 qlv-client-0.2.4/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.4/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.4/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1850 2024-05-10 05:14:14.000000 qlv-client-0.2.4/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.4/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.4/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0    10291 2024-05-10 03:54:21.000000 qlv-client-0.2.4/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.4/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.4/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.4/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:14:29.372196 qlv-client-0.2.4/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 05:14:29.372692 qlv-client-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-10 05:14:21.000000 qlv-client-0.2.4/setup.py
```

### Comparing `qlv-client-0.2.3/LICENSE` & `qlv-client-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.3/qlv_client/api.py` & `qlv-client-0.2.4/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.3/qlv_client/converter.py` & `qlv-client-0.2.4/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.3/qlv_client/http_client.py` & `qlv-client-0.2.4/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.3/qlv_client/proxy.py` & `qlv-client-0.2.4/qlv_client/proxy.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.3/qlv_client/repository.py` & `qlv-client-0.2.4/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.3/qlv_client/test.py` & `qlv-client-0.2.4/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.3/qlv_client/utils.py` & `qlv-client-0.2.4/qlv_client/utils.py`

 * *Files identical despite different names*

