# Comparing `tmp/serviceboot-2.1.8.tar.gz` & `tmp/serviceboot-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serviceboot-2.1.8.tar", last modified: Tue May 16 06:42:34 2023, max compression
+gzip compressed data, was "dist/serviceboot-2.1.9.tar", last modified: Fri Feb  2 02:59:23 2024, max compression
```

## Comparing `serviceboot-2.1.8.tar` & `serviceboot-2.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 06:42:34.000000 serviceboot-2.1.8/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 06:42:34.000000 serviceboot-2.1.8/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.8/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3283 2023-05-15 02:27:33.000000 serviceboot-2.1.8/serviceboot/build_docker.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4542 2023-05-15 02:27:33.000000 serviceboot-2.1.8/serviceboot/build_zip.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/command.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/compile_python.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/config_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/consul_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/oauth_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/onboarding.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/request_info.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    24784 2023-05-16 06:42:31.000000 serviceboot-2.1.8/serviceboot/serviceboot.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.8/serviceboot/token_service.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-16 06:42:34.000000 serviceboot-2.1.8/serviceboot.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-16 06:42:34.000000 serviceboot-2.1.8/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-16 06:42:31.000000 serviceboot-2.1.8/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-02-02 02:59:23.000000 serviceboot-2.1.9/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2024-02-02 02:59:23.000000 serviceboot-2.1.9/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.9/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3283 2023-05-15 02:27:33.000000 serviceboot-2.1.9/serviceboot/build_docker.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4542 2023-05-15 02:27:33.000000 serviceboot-2.1.9/serviceboot/build_zip.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/command.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/compile_python.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/config_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/consul_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/oauth_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/onboarding.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/request_info.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    24784 2023-05-16 06:45:42.000000 serviceboot-2.1.9/serviceboot/serviceboot.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.9/serviceboot/token_service.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      556 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       83 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       93 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       12 2024-02-02 02:59:23.000000 serviceboot-2.1.9/serviceboot.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2024-02-02 02:59:23.000000 serviceboot-2.1.9/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2024-02-02 02:59:17.000000 serviceboot-2.1.9/setup.py
```

### Comparing `serviceboot-2.1.8/PKG-INFO` & `serviceboot-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.8
+Version: 2.1.9
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.8/README.md` & `serviceboot-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/build_docker.py` & `serviceboot-2.1.9/serviceboot/build_docker.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/build_zip.py` & `serviceboot-2.1.9/serviceboot/build_zip.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/command.py` & `serviceboot-2.1.9/serviceboot/command.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/compile_python.py` & `serviceboot-2.1.9/serviceboot/compile_python.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/consul_client.py` & `serviceboot-2.1.9/serviceboot/consul_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/oauth_client.py` & `serviceboot-2.1.9/serviceboot/oauth_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/onboarding.py` & `serviceboot-2.1.9/serviceboot/onboarding.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/serviceboot.py` & `serviceboot-2.1.9/serviceboot/serviceboot.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot/token_service.py` & `serviceboot-2.1.9/serviceboot/token_service.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/serviceboot.egg-info/PKG-INFO` & `serviceboot-2.1.9/serviceboot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.8
+Version: 2.1.9
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.8/serviceboot.egg-info/SOURCES.txt` & `serviceboot-2.1.9/serviceboot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.8/setup.py` & `serviceboot-2.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='serviceboot',
-    version='2.1.8',
+    version='2.1.9',
     author='cubeai',
     author_email='cubeai@163.com',
     description='ServiceBoot云原生微服务引擎',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
     install_requires=[
         'cython==0.29.21',
         'requests',
-        'tornado==6.0.4',
-        'pyyaml==5.3.1',
+        'tornado>=6.0.4',
+        'pyyaml>=5.3.1',
         'python_jwt==3.2.6',
         'python-consul==1.1.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
```

