# Comparing `tmp/middleware-help-python-0.0.8.tar.gz` & `tmp/middleware-help-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.0.8.tar", last modified: Fri May 10 10:36:05 2024, max compression
+gzip compressed data, was "middleware-help-python-0.0.9.tar", last modified: Fri May 10 10:40:02 2024, max compression
```

## Comparing `middleware-help-python-0.0.8.tar` & `middleware-help-python-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 10:36:05.471533 middleware-help-python-0.0.8/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      543 2024-05-10 10:36:05.469564 middleware-help-python-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 10:36:05.468564 middleware-help-python-0.0.8/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      543 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 10:36:05.465572 middleware-help-python-0.0.8/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.8/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0      530 2024-05-10 10:22:25.000000 middleware-help-python-0.0.8/middleware_helper/libs.py
--rw-rw-rw-   0        0        0     5026 2024-05-10 10:35:38.000000 middleware-help-python-0.0.8/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.8/middleware_helper/network.py
--rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.8/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-05-10 10:36:05.472554 middleware-help-python-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-05-10 10:35:53.000000 middleware-help-python-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:40:02.000271 middleware-help-python-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      543 2024-05-10 10:40:01.999246 middleware-help-python-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:40:01.997251 middleware-help-python-0.0.9/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-05-10 10:40:01.000000 middleware-help-python-0.0.9/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-10 10:40:01.000000 middleware-help-python-0.0.9/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:40:01.000000 middleware-help-python-0.0.9/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-10 10:40:01.000000 middleware-help-python-0.0.9/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 10:40:01.000000 middleware-help-python-0.0.9/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 10:40:01.995256 middleware-help-python-0.0.9/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.9/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0      530 2024-05-10 10:22:25.000000 middleware-help-python-0.0.9/middleware_helper/libs.py
+-rw-rw-rw-   0        0        0     5049 2024-05-10 10:39:48.000000 middleware-help-python-0.0.9/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.9/middleware_helper/network.py
+-rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.9/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:40:02.000271 middleware-help-python-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-05-10 10:39:56.000000 middleware-help-python-0.0.9/setup.py
```

### Comparing `middleware-help-python-0.0.8/LICENSE` & `middleware-help-python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.8/PKG-INFO` & `middleware-help-python-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.8/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.0.9/middleware_help_python.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.8/middleware_helper/libs.py` & `middleware-help-python-0.0.9/middleware_helper/libs.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.8/middleware_helper/mysql.py` & `middleware-help-python-0.0.9/middleware_helper/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
     def retry_connection(self) -> connect:
         conn = self.__connect_to_mysql()
         i = 0
         while conn is None or not conn.is_connected():
             if i > 9:
                 logger.warning("尝试连接数据库10次以上，最终未能成功")
+                break
             else:
                 if i > 0:
                     logger.warning("尝试重连数据库...")
                 conn = self.__connect_to_mysql()
             i = i + 1
         return conn
```

### Comparing `middleware-help-python-0.0.8/middleware_helper/network.py` & `middleware-help-python-0.0.9/middleware_helper/network.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.8/middleware_helper/redis.py` & `middleware-help-python-0.0.9/middleware_helper/redis.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.8/setup.py` & `middleware-help-python-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.0.8',
+    version='0.0.9',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

