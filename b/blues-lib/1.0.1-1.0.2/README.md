# Comparing `tmp/blues_lib-1.0.1.tar.gz` & `tmp/blues_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.0.1.tar", last modified: Thu May  9 18:10:12 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.0.2.tar", last modified: Fri May 10 12:21:00 2024, max compression
```

## Comparing `blues_lib-1.0.1.tar` & `blues_lib-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.885818 blues_lib-1.0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-09 18:10:12.886844 blues_lib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      622 2024-05-07 10:02:36.000000 blues_lib-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.855414 blues_lib-1.0.1/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.864993 blues_lib-1.0.1/blues_sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.1/blues_sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.1/blues_sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.1/blues_sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.1/blues_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.883654 blues_lib-1.0.1/blues_util/
--rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.1/blues_util/BluesConsole.py
--rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.1/blues_util/BluesDateTime.py
--rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.1/blues_util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.1/blues_util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.1/blues_util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.1/blues_util/BluesMailer.py
--rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.1/blues_util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.1/blues_util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.1/blues_util/__init__.py
--rw-rw-rw-   0        0        0       86 2024-05-09 18:10:12.887846 blues_lib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-05-09 18:09:22.000000 blues_lib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.844857 blues_lib-1.0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 12:21:00.845889 blues_lib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.804804 blues_lib-1.0.2/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-10 12:21:00.000000 blues_lib-1.0.2/blues_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.817705 blues_lib-1.0.2/blues_sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.2/blues_sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.2/blues_sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.2/blues_sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.2/blues_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:21:00.843350 blues_lib-1.0.2/blues_util/
+-rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.2/blues_util/BluesConsole.py
+-rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.2/blues_util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.2/blues_util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.2/blues_util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.2/blues_util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.2/blues_util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.2/blues_util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.2/blues_util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.2/blues_util/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-05-10 12:21:00.847888 blues_lib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-05-10 12:20:16.000000 blues_lib-1.0.2/setup.py
```

### Comparing `blues_lib-1.0.1/PKG-INFO` & `blues_lib-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: blues_lib
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
         ```
-        pip install blues-lib==1.0.0
+        pip install blues-lib==1.0.1
         ```
         
         ### blues_sele
         #### BluesDebugChrome
         
         ##### reliant env variables
         1. `$env:CHROME_EXE` : the chrome's .exe file path - * required
```

### Comparing `blues_lib-1.0.1/README.md` & `blues_lib-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## Description
 Python library writed by Blues Liu.
 
 ### Install
 ```
-pip install blues-lib==1.0.0
+pip install blues-lib==1.0.1
 ```
 
 ### blues_sele
 #### BluesDebugChrome
 
 ##### reliant env variables
 1. `$env:CHROME_EXE` : the chrome's .exe file path - * required
```

### Comparing `blues_lib-1.0.1/blues_lib.egg-info/PKG-INFO` & `blues_lib-1.0.2/blues_lib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: blues-lib
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
         ```
-        pip install blues-lib==1.0.0
+        pip install blues-lib==1.0.1
         ```
         
         ### blues_sele
         #### BluesDebugChrome
         
         ##### reliant env variables
         1. `$env:CHROME_EXE` : the chrome's .exe file path - * required
```

### Comparing `blues_lib-1.0.1/blues_lib.egg-info/SOURCES.txt` & `blues_lib-1.0.2/blues_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_sql/BluesMySQLExecutor.py` & `blues_lib-1.0.2/blues_sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_sql/BluesSQLConvertor.py` & `blues_lib-1.0.2/blues_sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_sql/BluesSQLExecutor.py` & `blues_lib-1.0.2/blues_sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_util/BluesConsole.py` & `blues_lib-1.0.2/blues_util/BluesConsole.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_util/BluesDateTime.py` & `blues_lib-1.0.2/blues_util/BluesDateTime.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_util/BluesFiler.py` & `blues_lib-1.0.2/blues_util/BluesFiler.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_util/BluesImager.py` & `blues_lib-1.0.2/blues_util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_util/BluesLogger.py` & `blues_lib-1.0.2/blues_util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_util/BluesMailer.py` & `blues_lib-1.0.2/blues_util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.1/blues_util/BluesPowerShell.py` & `blues_lib-1.0.2/blues_util/BluesPowerShell.py`

 * *Files identical despite different names*

