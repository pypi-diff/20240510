# Comparing `tmp/blues_lib-1.0.4.tar.gz` & `tmp/blues_lib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.0.4.tar", last modified: Fri May 10 13:24:32 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.0.5.tar", last modified: Fri May 10 13:31:57 2024, max compression
```

## Comparing `blues_lib-1.0.4.tar` & `blues_lib-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.509160 blues_lib-1.0.4/
--rw-rw-rw-   0        0        0     1065 2024-05-10 13:24:32.509160 blues_lib-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.464784 blues_lib-1.0.4/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.472520 blues_lib-1.0.4/blues_sele/
--rw-rw-rw-   0        0        0      435 2024-05-09 18:41:09.000000 blues_lib-1.0.4/blues_sele/BluesBrowser.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.4/blues_sele/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.481752 blues_lib-1.0.4/blues_sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.4/blues_sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.4/blues_sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.4/blues_sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.4/blues_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.508156 blues_lib-1.0.4/blues_util/
--rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.4/blues_util/BluesConsole.py
--rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.4/blues_util/BluesDateTime.py
--rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.4/blues_util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.4/blues_util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.4/blues_util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.4/blues_util/BluesMailer.py
--rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.4/blues_util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.4/blues_util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.4/blues_util/__init__.py
--rw-rw-rw-   0        0        0       86 2024-05-10 13:24:32.511621 blues_lib-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-05-10 13:23:04.000000 blues_lib-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.449257 blues_lib-1.0.5/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 13:31:57.450257 blues_lib-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.116966 blues_lib-1.0.5/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 13:31:56.000000 blues_lib-1.0.5/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1265 2024-05-10 13:31:57.000000 blues_lib-1.0.5/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:31:56.000000 blues_lib-1.0.5/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-10 13:31:56.000000 blues_lib-1.0.5/blues_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.123529 blues_lib-1.0.5/blues_sele/
+-rw-rw-rw-   0        0        0      435 2024-05-09 18:41:09.000000 blues_lib-1.0.5/blues_sele/BluesBrowser.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.5/blues_sele/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.128063 blues_lib-1.0.5/blues_sele/action/
+-rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.0.5/blues_sele/action/BluesDriverAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.5/blues_sele/action/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.181632 blues_lib-1.0.5/blues_sele/action/parts/
+-rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesAlertAction.py
+-rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesCookieAction.py
+-rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesDocumentAction.py
+-rw-rw-rw-   0        0        0     4408 2024-05-08 16:59:14.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesElementAction.py
+-rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesEventAction.py
+-rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesFormAction.py
+-rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesFrameAction.py
+-rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesJavaScriptAction.py
+-rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesMoverAction.py
+-rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesSelectAction.py
+-rw-rw-rw-   0        0        0     3388 2024-05-09 12:48:42.000000 blues_lib-1.0.5/blues_sele/action/parts/BluesWindowAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.5/blues_sele/action/parts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.235888 blues_lib-1.0.5/blues_sele/browser/
+-rw-rw-rw-   0        0        0     3137 2024-05-09 16:42:46.000000 blues_lib-1.0.5/blues_sele/browser/BluesChrome.py
+-rw-rw-rw-   0        0        0     3024 2024-05-09 16:46:32.000000 blues_lib-1.0.5/blues_sele/browser/BluesDebugChrome.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.5/blues_sele/browser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.251542 blues_lib-1.0.5/blues_sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.5/blues_sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.5/blues_sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.5/blues_sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.5/blues_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:31:57.448256 blues_lib-1.0.5/blues_util/
+-rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.5/blues_util/BluesConsole.py
+-rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.5/blues_util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.5/blues_util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.5/blues_util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.5/blues_util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.5/blues_util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.5/blues_util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.5/blues_util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.5/blues_util/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-05-10 13:31:57.452256 blues_lib-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-05-10 13:31:51.000000 blues_lib-1.0.5/setup.py
```

### Comparing `blues_lib-1.0.4/PKG-INFO` & `blues_lib-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues_lib
-Version: 1.0.4
+Version: 1.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.0.4/README.md` & `blues_lib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_lib.egg-info/PKG-INFO` & `blues_lib-1.0.5/blues_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues-lib
-Version: 1.0.4
+Version: 1.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.0.4/blues_sql/BluesMySQLExecutor.py` & `blues_lib-1.0.5/blues_sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_sql/BluesSQLConvertor.py` & `blues_lib-1.0.5/blues_sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_sql/BluesSQLExecutor.py` & `blues_lib-1.0.5/blues_sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_util/BluesConsole.py` & `blues_lib-1.0.5/blues_util/BluesConsole.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_util/BluesDateTime.py` & `blues_lib-1.0.5/blues_util/BluesDateTime.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_util/BluesFiler.py` & `blues_lib-1.0.5/blues_util/BluesFiler.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_util/BluesImager.py` & `blues_lib-1.0.5/blues_util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_util/BluesLogger.py` & `blues_lib-1.0.5/blues_util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_util/BluesMailer.py` & `blues_lib-1.0.5/blues_util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/blues_util/BluesPowerShell.py` & `blues_lib-1.0.5/blues_util/BluesPowerShell.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.4/setup.py` & `blues_lib-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 class CleanCommandExtension():
   def run(self):
     print('--->test')
 
 setup(
   name="blues_lib", # package name
-  version="1.0.4", # package version
+  version="1.0.5", # package version
   cmdclass = {
     'clean':CleanCommandExtension, # clear the dist dir auto
   },
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
   packages=find_packages(), # package module
   # add from requirement.txt,本地测试注释所有包，不能从镜像立即安装
```

