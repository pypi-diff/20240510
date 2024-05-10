# Comparing `tmp/autoboot-data-0.1.2.tar.gz` & `tmp/autoboot-data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoboot-data-0.1.2.tar", last modified: Mon Nov 27 02:13:45 2023, max compression
+gzip compressed data, was "autoboot-data-0.2.0.tar", last modified: Thu Nov 30 02:25:12 2023, max compression
```

## Comparing `autoboot-data-0.1.2.tar` & `autoboot-data-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-27 02:13:45.212246 autoboot-data-0.1.2/
--rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot-data-0.1.2/LICENSE.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-15 07:56:55.000000 autoboot-data-0.1.2/MANIFEST.in
--rw-r--r--   0 yizzuide   (501) staff       (20)      640 2023-11-27 02:13:45.212363 autoboot-data-0.1.2/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)       69 2023-11-22 06:07:07.000000 autoboot-data-0.1.2/README.md
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-27 02:13:45.208277 autoboot-data-0.1.2/autoboot_data/
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-22 06:17:25.000000 autoboot-data-0.1.2/autoboot_data/__init__.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-27 02:13:45.212013 autoboot-data-0.1.2/autoboot_data/redis/
--rw-r--r--   0 yizzuide   (501) staff       (20)      127 2023-11-24 07:07:32.000000 autoboot-data-0.1.2/autoboot_data/redis/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1661 2023-11-27 02:13:32.000000 autoboot-data-0.1.2/autoboot_data/redis/redis_config.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1560 2023-11-22 08:22:58.000000 autoboot-data-0.1.2/autoboot_data/redis/redis_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-27 02:13:45.210398 autoboot-data-0.1.2/autoboot_data.egg-info/
--rw-r--r--   0 yizzuide   (501) staff       (20)      640 2023-11-27 02:13:45.000000 autoboot-data-0.1.2/autoboot_data.egg-info/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)      385 2023-11-27 02:13:45.000000 autoboot-data-0.1.2/autoboot_data.egg-info/SOURCES.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-11-27 02:13:45.000000 autoboot-data-0.1.2/autoboot_data.egg-info/dependency_links.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       22 2023-11-27 02:13:45.000000 autoboot-data-0.1.2/autoboot_data.egg-info/requires.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       14 2023-11-27 02:13:45.000000 autoboot-data-0.1.2/autoboot_data.egg-info/top_level.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)     1313 2023-11-15 07:41:11.000000 autoboot-data-0.1.2/pyproject.toml
--rw-r--r--   0 yizzuide   (501) staff       (20)      106 2023-11-27 02:13:45.212813 autoboot-data-0.1.2/setup.cfg
--rw-r--r--   0 yizzuide   (501) staff       (20)     1036 2023-11-27 02:13:32.000000 autoboot-data-0.1.2/setup.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:25:12.742203 autoboot-data-0.2.0/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot-data-0.2.0/LICENSE.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-15 07:56:55.000000 autoboot-data-0.2.0/MANIFEST.in
+-rw-r--r--   0 yizzuide   (501) staff       (20)      640 2023-11-30 02:25:12.742318 autoboot-data-0.2.0/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)       69 2023-11-22 06:07:07.000000 autoboot-data-0.2.0/README.md
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:25:12.738623 autoboot-data-0.2.0/autoboot_data/
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-22 06:17:25.000000 autoboot-data-0.2.0/autoboot_data/__init__.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:25:12.741883 autoboot-data-0.2.0/autoboot_data/redis/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      127 2023-11-24 07:07:32.000000 autoboot-data-0.2.0/autoboot_data/redis/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1661 2023-11-27 02:13:32.000000 autoboot-data-0.2.0/autoboot_data/redis/redis_config.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1560 2023-11-22 08:22:58.000000 autoboot-data-0.2.0/autoboot_data/redis/redis_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:25:12.740493 autoboot-data-0.2.0/autoboot_data.egg-info/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      640 2023-11-30 02:25:12.000000 autoboot-data-0.2.0/autoboot_data.egg-info/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)      385 2023-11-30 02:25:12.000000 autoboot-data-0.2.0/autoboot_data.egg-info/SOURCES.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-11-30 02:25:12.000000 autoboot-data-0.2.0/autoboot_data.egg-info/dependency_links.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       22 2023-11-30 02:25:12.000000 autoboot-data-0.2.0/autoboot_data.egg-info/requires.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       14 2023-11-30 02:25:12.000000 autoboot-data-0.2.0/autoboot_data.egg-info/top_level.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1313 2023-11-15 07:41:11.000000 autoboot-data-0.2.0/pyproject.toml
+-rw-r--r--   0 yizzuide   (501) staff       (20)      106 2023-11-30 02:25:12.742831 autoboot-data-0.2.0/setup.cfg
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1036 2023-11-30 02:24:52.000000 autoboot-data-0.2.0/setup.py
```

### Comparing `autoboot-data-0.1.2/LICENSE.txt` & `autoboot-data-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoboot-data-0.1.2/PKG-INFO` & `autoboot-data-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoboot-data
-Version: 0.1.2
+Version: 0.2.0
 Summary: Data access build with autoboot
 Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide
 Author-email: fu837014586@163.com
 Keywords: autoboot,data,redis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `autoboot-data-0.1.2/autoboot_data/redis/redis_config.py` & `autoboot-data-0.2.0/autoboot_data/redis/redis_config.py`

 * *Files identical despite different names*

### Comparing `autoboot-data-0.1.2/autoboot_data/redis/redis_properties.py` & `autoboot-data-0.2.0/autoboot_data/redis/redis_properties.py`

 * *Files identical despite different names*

### Comparing `autoboot-data-0.1.2/autoboot_data.egg-info/PKG-INFO` & `autoboot-data-0.2.0/autoboot_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoboot-data
-Version: 0.1.2
+Version: 0.2.0
 Summary: Data access build with autoboot
 Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide
 Author-email: fu837014586@163.com
 Keywords: autoboot,data,redis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `autoboot-data-0.1.2/pyproject.toml` & `autoboot-data-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoboot-data-0.1.2/setup.py` & `autoboot-data-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.1.2'
+VERSION = '0.2.0'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='autoboot-data',
     version=VERSION,
@@ -14,15 +14,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/yizzuide/autoboot_data',
     keywords=['autoboot', 'data', 'redis'],
     packages=find_packages(exclude=['tests*']),
     include_package_data=True,
     install_requires=[
-        'autoboot>=0.5.1',
+        'autoboot>=0.6.0',
         'redis'
     ],
     tests_require=[
         'pytest>=6.2.0',
         'pytest-cov>=2.10.0'
     ],
     python_requires='>=3.8',
```

