# Comparing `tmp/blues_lib-1.0.2.tar.gz` & `tmp/blues_lib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.0.2.tar", last modified: Fri May 10 12:21:00 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.0.3.tar", last modified: Fri May 10 12:55:23 2024, max compression
```

## Comparing `blues_lib-1.0.2.tar` & `blues_lib-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.844857 blues_lib-1.0.2/
--rw-rw-rw-   0        0        0     1065 2024-05-10 12:21:00.845889 blues_lib-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.804804 blues_lib-1.0.2/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.817705 blues_lib-1.0.2/blues_sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.2/blues_sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.2/blues_sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.2/blues_sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.2/blues_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.843350 blues_lib-1.0.2/blues_util/
--rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.2/blues_util/BluesConsole.py
--rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.2/blues_util/BluesDateTime.py
--rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.2/blues_util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.2/blues_util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.2/blues_util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.2/blues_util/BluesMailer.py
--rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.2/blues_util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.2/blues_util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.2/blues_util/__init__.py
--rw-rw-rw-   0        0        0       86 2024-05-10 12:21:00.847888 blues_lib-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-05-10 12:20:16.000000 blues_lib-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.088528 blues_lib-1.0.3/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 12:55:23.088528 blues_lib-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.069709 blues_lib-1.0.3/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-05-10 12:55:23.000000 blues_lib-1.0.3/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.072258 blues_lib-1.0.3/blues_sele/
+-rw-rw-rw-   0        0        0      435 2024-05-09 18:41:09.000000 blues_lib-1.0.3/blues_sele/BluesBrowser.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.3/blues_sele/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.076317 blues_lib-1.0.3/blues_sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.3/blues_sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.3/blues_sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.3/blues_sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.3/blues_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.087062 blues_lib-1.0.3/blues_util/
+-rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.3/blues_util/BluesConsole.py
+-rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.3/blues_util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.3/blues_util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.3/blues_util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.3/blues_util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.3/blues_util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.3/blues_util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.3/blues_util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.3/blues_util/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-05-10 12:55:23.090033 blues_lib-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      670 2024-05-10 12:43:03.000000 blues_lib-1.0.3/setup.py
```

### Comparing `blues_lib-1.0.2/PKG-INFO` & `blues_lib-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues_lib
-Version: 1.0.2
+Version: 1.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.0.2/README.md` & `blues_lib-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_lib.egg-info/PKG-INFO` & `blues_lib-1.0.3/blues_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues-lib
-Version: 1.0.2
+Version: 1.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.0.2/blues_lib.egg-info/SOURCES.txt` & `blues_lib-1.0.3/blues_lib.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 setup.cfg
 setup.py
 blues_lib.egg-info/PKG-INFO
 blues_lib.egg-info/SOURCES.txt
 blues_lib.egg-info/dependency_links.txt
 blues_lib.egg-info/requires.txt
 blues_lib.egg-info/top_level.txt
+blues_sele/BluesBrowser.py
+blues_sele/__init__.py
 blues_sql/BluesMySQLExecutor.py
 blues_sql/BluesSQLConvertor.py
 blues_sql/BluesSQLExecutor.py
 blues_sql/__init__.py
 blues_util/BluesConsole.py
 blues_util/BluesDateTime.py
 blues_util/BluesFiler.py
```

### Comparing `blues_lib-1.0.2/blues_sql/BluesMySQLExecutor.py` & `blues_lib-1.0.3/blues_sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_sql/BluesSQLConvertor.py` & `blues_lib-1.0.3/blues_sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_sql/BluesSQLExecutor.py` & `blues_lib-1.0.3/blues_sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_util/BluesConsole.py` & `blues_lib-1.0.3/blues_util/BluesConsole.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_util/BluesDateTime.py` & `blues_lib-1.0.3/blues_util/BluesDateTime.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_util/BluesFiler.py` & `blues_lib-1.0.3/blues_util/BluesFiler.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_util/BluesImager.py` & `blues_lib-1.0.3/blues_util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_util/BluesLogger.py` & `blues_lib-1.0.3/blues_util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_util/BluesMailer.py` & `blues_lib-1.0.3/blues_util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.2/blues_util/BluesPowerShell.py` & `blues_lib-1.0.3/blues_util/BluesPowerShell.py`

 * *Files identical despite different names*

