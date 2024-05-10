# Comparing `tmp/sqlman-0.1.tar.gz` & `tmp/sqlman-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlman-0.1.tar", last modified: Tue May  7 14:03:12 2024, max compression
+gzip compressed data, was "sqlman-0.2.tar", last modified: Thu May  9 16:00:25 2024, max compression
```

## Comparing `sqlman-0.1.tar` & `sqlman-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 14:03:12.966293 sqlman-0.1/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3902 2024-05-07 14:03:12.966084 sqlman-0.1/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     3616 2024-04-21 13:36:08.000000 sqlman-0.1/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-07 14:03:12.966329 sqlman-0.1/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      623 2024-05-07 14:02:56.000000 sqlman-0.1/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 14:03:12.965056 sqlman-0.1/sqlman/
--rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.1/sqlman/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     6478 2024-04-21 14:22:23.000000 sqlman-0.1/sqlman/handler.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     9430 2024-04-21 14:32:46.000000 sqlman-0.1/sqlman/table_controller.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.1/sqlman/tools.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 14:03:12.965931 sqlman-0.1/sqlman.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3902 2024-05-07 14:03:12.000000 sqlman-0.1/sqlman.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      276 2024-05-07 14:03:12.000000 sqlman-0.1/sqlman.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 14:03:12.000000 sqlman-0.1/sqlman.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 14:03:12.000000 sqlman-0.1/sqlman.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-07 14:03:12.000000 sqlman-0.1/sqlman.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-07 14:03:12.000000 sqlman-0.1/sqlman.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-09 16:00:25.380459 sqlman-0.2/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3802 2024-05-09 16:00:25.380278 sqlman-0.2/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3516 2024-05-09 16:00:14.000000 sqlman-0.2/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-09 16:00:25.380496 sqlman-0.2/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      643 2024-05-09 16:00:14.000000 sqlman-0.2/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-09 16:00:25.379314 sqlman-0.2/sqlman/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.2/sqlman/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     6478 2024-04-21 14:22:23.000000 sqlman-0.2/sqlman/handler.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     9430 2024-04-21 14:32:46.000000 sqlman-0.2/sqlman/table_controller.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.2/sqlman/tools.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-09 16:00:25.380117 sqlman-0.2/sqlman.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3802 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      276 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/top_level.txt
```

### Comparing `sqlman-0.1/PKG-INFO` & `sqlman-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.1
+Version: 0.2
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
 
-# 说明
-
-- 持续更新中...
-- 从此告别SQL语句，直接调用方法就完事
-- python3.10+
-
 # 如何吸引你？
 
 ### 如此简易的连接方式
 
 一个字典参数即可
 
 ### 插入数据如此的贴心
```

### Comparing `sqlman-0.1/README.md` & `sqlman-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-# 说明
-
-- 持续更新中...
-- 从此告别SQL语句，直接调用方法就完事
-- python3.10+
-
 # 如何吸引你？
 
 ### 如此简易的连接方式
 
 一个字典参数即可
 
 ### 插入数据如此的贴心
```

### Comparing `sqlman-0.1/setup.py` & `sqlman-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='sqlman',
-    version='0.1',
+    version='0.2',
     description='告别SQL语句，python操作mysql的贴心助手',
     url='https://github.com/markadc/sqlman',
     author='WangTuo',
     author_email='markadc@126.com',
-    packages=['sqlman'],
+    packages=find_packages(),
     license='MIT',
     zip_safe=False,
     install_requires=['DBUtils', 'PyMySQL', 'Faker', 'loguru'],
     keywords=['Python', 'MySQL', 'Database'],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `sqlman-0.1/sqlman/handler.py` & `sqlman-0.2/sqlman/handler.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.1/sqlman/table_controller.py` & `sqlman-0.2/sqlman/table_controller.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.1/sqlman/tools.py` & `sqlman-0.2/sqlman/tools.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.1/sqlman.egg-info/PKG-INFO` & `sqlman-0.2/sqlman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.1
+Version: 0.2
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
 
-# 说明
-
-- 持续更新中...
-- 从此告别SQL语句，直接调用方法就完事
-- python3.10+
-
 # 如何吸引你？
 
 ### 如此简易的连接方式
 
 一个字典参数即可
 
 ### 插入数据如此的贴心
```

