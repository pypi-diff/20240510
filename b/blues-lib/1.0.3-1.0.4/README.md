# Comparing `tmp/blues_lib-1.0.3.tar.gz` & `tmp/blues_lib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.0.3.tar", last modified: Fri May 10 12:55:23 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.0.4.tar", last modified: Fri May 10 13:24:32 2024, max compression
```

## Comparing `blues_lib-1.0.3.tar` & `blues_lib-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.088528 blues_lib-1.0.3/
--rw-rw-rw-   0        0        0     1065 2024-05-10 12:55:23.088528 blues_lib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.069709 blues_lib-1.0.3/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-05-10 12:55:23.000000 blues_lib-1.0.3/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2024-05-10 12:55:22.000000 blues_lib-1.0.3/blues_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.072258 blues_lib-1.0.3/blues_sele/
--rw-rw-rw-   0        0        0      435 2024-05-09 18:41:09.000000 blues_lib-1.0.3/blues_sele/BluesBrowser.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.3/blues_sele/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.076317 blues_lib-1.0.3/blues_sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.3/blues_sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.3/blues_sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.3/blues_sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.3/blues_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:55:23.087062 blues_lib-1.0.3/blues_util/
--rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.3/blues_util/BluesConsole.py
--rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.3/blues_util/BluesDateTime.py
--rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.3/blues_util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.3/blues_util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.3/blues_util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.3/blues_util/BluesMailer.py
--rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.3/blues_util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.3/blues_util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.3/blues_util/__init__.py
--rw-rw-rw-   0        0        0       86 2024-05-10 12:55:23.090033 blues_lib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      670 2024-05-10 12:43:03.000000 blues_lib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.509160 blues_lib-1.0.4/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 13:24:32.509160 blues_lib-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.464784 blues_lib-1.0.4/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-10 13:24:32.000000 blues_lib-1.0.4/blues_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.472520 blues_lib-1.0.4/blues_sele/
+-rw-rw-rw-   0        0        0      435 2024-05-09 18:41:09.000000 blues_lib-1.0.4/blues_sele/BluesBrowser.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.4/blues_sele/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.481752 blues_lib-1.0.4/blues_sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.4/blues_sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.4/blues_sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.4/blues_sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.4/blues_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:32.508156 blues_lib-1.0.4/blues_util/
+-rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.4/blues_util/BluesConsole.py
+-rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.4/blues_util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.4/blues_util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.4/blues_util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.4/blues_util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.4/blues_util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.4/blues_util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.4/blues_util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.4/blues_util/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-05-10 13:24:32.511621 blues_lib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-05-10 13:23:04.000000 blues_lib-1.0.4/setup.py
```

### Comparing `blues_lib-1.0.3/PKG-INFO` & `blues_lib-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues_lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.0.3/README.md` & `blues_lib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_lib.egg-info/PKG-INFO` & `blues_lib-1.0.4/blues_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blues-lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
```

### Comparing `blues_lib-1.0.3/blues_lib.egg-info/SOURCES.txt` & `blues_lib-1.0.4/blues_lib.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 setup.cfg
 setup.py
 blues_lib.egg-info/PKG-INFO
 blues_lib.egg-info/SOURCES.txt
 blues_lib.egg-info/dependency_links.txt
-blues_lib.egg-info/requires.txt
 blues_lib.egg-info/top_level.txt
 blues_sele/BluesBrowser.py
 blues_sele/__init__.py
 blues_sql/BluesMySQLExecutor.py
 blues_sql/BluesSQLConvertor.py
 blues_sql/BluesSQLExecutor.py
 blues_sql/__init__.py
```

### Comparing `blues_lib-1.0.3/blues_sql/BluesMySQLExecutor.py` & `blues_lib-1.0.4/blues_sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_sql/BluesSQLConvertor.py` & `blues_lib-1.0.4/blues_sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_sql/BluesSQLExecutor.py` & `blues_lib-1.0.4/blues_sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_util/BluesConsole.py` & `blues_lib-1.0.4/blues_util/BluesConsole.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_util/BluesDateTime.py` & `blues_lib-1.0.4/blues_util/BluesDateTime.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_util/BluesFiler.py` & `blues_lib-1.0.4/blues_util/BluesFiler.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_util/BluesImager.py` & `blues_lib-1.0.4/blues_util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_util/BluesLogger.py` & `blues_lib-1.0.4/blues_util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_util/BluesMailer.py` & `blues_lib-1.0.4/blues_util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/blues_util/BluesPowerShell.py` & `blues_lib-1.0.4/blues_util/BluesPowerShell.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.0.3/setup.py` & `blues_lib-1.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 class CleanCommandExtension():
   def run(self):
     print('--->test')
 
 setup(
   name="blues_lib", # package name
-  version="1.0.3", # package version
+  version="1.0.4", # package version
   cmdclass = {
     'clean':CleanCommandExtension, # clear the dist dir auto
   },
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
   packages=find_packages(), # package module
-  # add from requirement.txt
+  # add from requirement.txt,本地测试注释所有包，不能从镜像立即安装
   install_requires=[
-    'Pillow>=10.3.0',
-    'Requests>=2.31.0',
-    'selenium>=4.20.0',
-    'selenium_wire>=5.1.0',
-    'setuptools>=47.1.0',
-    'webdriver_manager>=4.0.0',
+    #'Pillow>=10.3.0',
+    #'Requests>=2.31.0',
+    #'selenium>=4.20.0',
+    #'selenium_wire>=5.1.0',
+    #'setuptools>=47.1.0',
+    #'webdriver_manager>=4.0.0',
   ] # package dependency
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

