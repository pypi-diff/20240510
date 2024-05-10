# Comparing `tmp/wxhook-0.0.8.tar.gz` & `tmp/wxhook-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhook-0.0.8.tar", last modified: Tue May  7 03:15:48 2024, max compression
+gzip compressed data, was "wxhook-0.0.9.tar", last modified: Fri May 10 05:58:23 2024, max compression
```

## Comparing `wxhook-0.0.8.tar` & `wxhook-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:15:48.532832 wxhook-0.0.8/
--rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       51 2024-05-06 09:07:02.000000 wxhook-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3397 2024-05-07 03:15:48.531825 wxhook-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2653 2024-05-06 10:56:59.000000 wxhook-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 03:15:48.532832 wxhook-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3928 2024-05-07 03:03:15.000000 wxhook-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:15:48.500647 wxhook-0.0.8/wxhook/
--rw-rw-rw-   0        0        0       44 2024-05-07 03:03:15.000000 wxhook-0.0.8/wxhook/__init__.py
--rw-rw-rw-   0        0        0    16377 2024-05-07 03:09:45.000000 wxhook-0.0.8/wxhook/core.py
--rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.8/wxhook/events.py
--rw-rw-rw-   0        0        0      310 2024-05-06 08:37:49.000000 wxhook-0.0.8/wxhook/logger.py
--rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.8/wxhook/model.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:15:48.530751 wxhook-0.0.8/wxhook/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.8/wxhook/tools/faker.exe
--rwxrwxrwx   0        0        0   911872 2024-05-07 02:06:33.000000 wxhook-0.0.8/wxhook/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.8/wxhook/tools/wxhook.dll
--rw-rw-rw-   0        0        0     3785 2024-05-06 12:02:21.000000 wxhook-0.0.8/wxhook/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:15:48.524962 wxhook-0.0.8/wxhook.egg-info/
--rw-rw-rw-   0        0        0     3397 2024-05-07 03:15:48.000000 wxhook-0.0.8/wxhook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-05-07 03:15:48.000000 wxhook-0.0.8/wxhook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:15:48.000000 wxhook-0.0.8/wxhook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-07 03:15:48.000000 wxhook-0.0.8/wxhook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 03:15:48.000000 wxhook-0.0.8/wxhook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 05:58:23.503262 wxhook-0.0.9/
+-rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-05-06 09:07:02.000000 wxhook-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3397 2024-05-10 05:58:23.502264 wxhook-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2653 2024-05-06 10:56:59.000000 wxhook-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 05:58:23.504263 wxhook-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3928 2024-05-10 05:57:43.000000 wxhook-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:58:23.489196 wxhook-0.0.9/wxhook/
+-rw-rw-rw-   0        0        0       44 2024-05-10 05:57:43.000000 wxhook-0.0.9/wxhook/__init__.py
+-rw-rw-rw-   0        0        0    16588 2024-05-10 05:39:43.000000 wxhook-0.0.9/wxhook/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.9/wxhook/events.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 08:37:49.000000 wxhook-0.0.9/wxhook/logger.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.9/wxhook/model.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:58:23.501261 wxhook-0.0.9/wxhook/tools/
+-rw-rw-rw-   0        0        0       22 2024-05-10 03:57:34.000000 wxhook-0.0.9/wxhook/tools/config.ini
+-rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.9/wxhook/tools/faker.exe
+-rwxrwxrwx   0        0        0   911872 2024-05-07 02:06:33.000000 wxhook-0.0.9/wxhook/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.9/wxhook/tools/wxhook.dll
+-rw-rw-rw-   0        0        0      102 2024-05-10 03:57:35.000000 wxhook-0.0.9/wxhook/tools/wxhook.json
+-rw-rw-rw-   0        0        0     3785 2024-05-06 12:02:21.000000 wxhook-0.0.9/wxhook/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:58:23.495266 wxhook-0.0.9/wxhook.egg-info/
+-rw-rw-rw-   0        0        0     3397 2024-05-10 05:58:23.000000 wxhook-0.0.9/wxhook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-10 05:58:23.000000 wxhook-0.0.9/wxhook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 05:58:23.000000 wxhook-0.0.9/wxhook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-10 05:58:23.000000 wxhook-0.0.9/wxhook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 05:58:23.000000 wxhook-0.0.9/wxhook.egg-info/top_level.txt
```

### Comparing `wxhook-0.0.8/LICENSE` & `wxhook-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/PKG-INFO` & `wxhook-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.8
+Version: 0.0.9
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wxhook-0.0.8/README.md` & `wxhook-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/setup.py` & `wxhook-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'wxhook'
 DESCRIPTION = 'wechat robot framework.'
 URL = 'https://github.com/miloira/wxhook'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhook-0.0.8/wxhook/core.py` & `wxhook-0.0.9/wxhook/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,19 @@
             self.request.close()
 
 
 class Bot:
 
     def __init__(
         self,
-        on_login: typing.Callable = None,
-        on_before_message: typing.Callable = None,
-        on_after_message: typing.Callable = None,
-        on_start: typing.Callable = None,
-        on_stop: typing.Callable = None,
+        on_login: typing.Optional[typing.Callable[["Bot", Event], typing.Any]] = None,
+        on_before_message: typing.Optional[typing.Callable[["Bot", Event], typing.Any]] = None,
+        on_after_message: typing.Optional[typing.Callable[["Bot", Event], typing.Any]] = None,
+        on_start: typing.Optional[typing.Callable[["Bot"], typing.Any]] = None,
+        on_stop: typing.Optional[typing.Callable[["Bot"], typing.Any]] = None,
         faked_version: typing.Optional[str] = None
     ):
         self.version = "3.9.5.81"
         self.server_host = "127.0.0.1"
         self.remote_host = "127.0.0.1"
         self.on_start = on_start
         self.on_login = on_login
```

### Comparing `wxhook-0.0.8/wxhook/events.py` & `wxhook-0.0.9/wxhook/events.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/wxhook/model.py` & `wxhook-0.0.9/wxhook/model.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/wxhook/tools/faker.exe` & `wxhook-0.0.9/wxhook/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/wxhook/tools/start-wechat.exe` & `wxhook-0.0.9/wxhook/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/wxhook/tools/wxhook.dll` & `wxhook-0.0.9/wxhook/tools/wxhook.dll`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/wxhook/utils.py` & `wxhook-0.0.9/wxhook/utils.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.8/wxhook.egg-info/PKG-INFO` & `wxhook-0.0.9/wxhook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.8
+Version: 0.0.9
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

