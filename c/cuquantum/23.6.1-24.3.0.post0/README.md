# Comparing `tmp/cuquantum-23.6.1.tar.gz` & `tmp/cuquantum-24.3.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuquantum-23.6.1.tar", last modified: Thu Jul 20 16:49:26 2023, max compression
+gzip compressed data, from Unix
```

## Comparing `cuquantum-23.6.1.tar` & `cuquantum-24.3.0.post0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:49:26.202466 cuquantum-23.6.1/
--rw-r--r--   0 root         (0) root         (0)    11004 2023-07-20 16:47:10.000000 cuquantum-23.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2853 2023-07-20 16:49:26.202466 cuquantum-23.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2052 2023-07-20 16:47:10.000000 cuquantum-23.6.1/README.rst
--rw-r--r--   0 root         (0) root         (0)     8953 2023-07-20 16:47:10.000000 cuquantum-23.6.1/cuda_autodetect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:49:26.202466 cuquantum-23.6.1/cuquantum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2853 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      210 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:49:26.202466 cuquantum-23.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2525 2023-07-20 16:47:10.000000 cuquantum-23.6.1/setup.py
+drwxr-xr-x   0 majones   (1000) majones   (1000)        0 2024-05-07 20:40:27.000000 cuquantum-24.3.0.post0/
+-rw-r--r--   0 majones   (1000) majones   (1000)     2052 2024-05-07 20:37:13.000000 cuquantum-24.3.0.post0/README.rst
+-rw-r--r--   0 majones   (1000) majones   (1000)     8953 2024-05-07 20:37:13.000000 cuquantum-24.3.0.post0/cuda_autodetect.py
+-rw-r--r--   0 majones   (1000) majones   (1000)    11004 2024-05-07 20:37:13.000000 cuquantum-24.3.0.post0/LICENSE
+-rw-r--r--   0 majones   (1000) majones   (1000)       38 2024-05-07 20:40:27.000000 cuquantum-24.3.0.post0/setup.cfg
+-rw-r--r--   0 majones   (1000) majones   (1000)     2531 2024-05-09 21:17:58.000000 cuquantum-24.3.0.post0/setup.py
+-rw-r--r--   0 majones   (1000) majones   (1000)     2859 2024-05-09 21:16:16.000000 cuquantum-24.3.0.post0/PKG-INFO
+drwxr-xr-x   0 majones   (1000) majones   (1000)        0 2024-05-07 20:40:27.000000 cuquantum-24.3.0.post0/cuquantum.egg-info/
+-rw-r--r--   0 majones   (1000) majones   (1000)        1 2024-05-07 20:40:27.000000 cuquantum-24.3.0.post0/cuquantum.egg-info/not-zip-safe
+-rw-r--r--   0 majones   (1000) majones   (1000)        1 2024-05-07 20:40:27.000000 cuquantum-24.3.0.post0/cuquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 majones   (1000) majones   (1000)      210 2024-05-07 20:40:27.000000 cuquantum-24.3.0.post0/cuquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 majones   (1000) majones   (1000)       16 2024-05-07 20:40:27.000000 cuquantum-24.3.0.post0/cuquantum.egg-info/top_level.txt
+-rw-r--r--   0 majones   (1000) majones   (1000)     2859 2024-05-09 21:16:57.000000 cuquantum-24.3.0.post0/cuquantum.egg-info/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cuquantum-23.6.1/LICENSE` & `cuquantum-24.3.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuquantum-23.6.1/PKG-INFO` & `cuquantum-24.3.0.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum
-Version: 23.6.1
+Version: 24.3.0.post0
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
```

### Comparing `cuquantum-23.6.1/README.rst` & `cuquantum-24.3.0.post0/README.rst`

 * *Files identical despite different names*

### Comparing `cuquantum-23.6.1/cuda_autodetect.py` & `cuquantum-24.3.0.post0/cuda_autodetect.py`

 * *Files identical despite different names*

### Comparing `cuquantum-23.6.1/cuquantum.egg-info/PKG-INFO` & `cuquantum-24.3.0.post0/cuquantum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum
-Version: 23.6.1
+Version: 24.3.0.post0
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
```

### Comparing `cuquantum-23.6.1/setup.py` & `cuquantum-24.3.0.post0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# Copyright (c) 2021-2024, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
 #
 # SPDX-License-Identifier: LicenseRef-NvidiaProprietary
 
 import glob
 import os
 import shutil
 import site
@@ -11,15 +11,15 @@
 
 from setuptools import setup
 
 from cuda_autodetect import infer_best_package, bdist_wheel
 
 
 # Update this for every release
-package_ver = '23.06.1'
+package_ver = '24.03.0.post0'
 package_name = "cuquantum"
 
 
 # get project long description
 with open("README.rst") as f:
     long_description = f.read()
```

