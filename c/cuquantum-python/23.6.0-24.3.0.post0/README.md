# Comparing `tmp/cuquantum-python-23.6.0.tar.gz` & `tmp/cuquantum_python-24.3.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuquantum-python-23.6.0.tar", last modified: Tue Jul 11 03:51:23 2023, max compression
+gzip compressed data, from Unix
```

## Comparing `cuquantum-python-23.6.0.tar` & `cuquantum_python-24.3.0.post0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2148 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1283 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     8953 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/cuda_autodetect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/cuquantum_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2148 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3233 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/setup.py
+drwxr-xr-x   0 majones   (1000) majones   (1000)        0 2024-05-07 21:02:40.000000 cuquantum_python-24.3.0.post0/
+-rw-r--r--   0 majones   (1000) majones   (1000)     1283 2024-05-07 20:37:13.000000 cuquantum_python-24.3.0.post0/README.rst
+-rw-r--r--   0 majones   (1000) majones   (1000)     8953 2024-05-07 20:37:13.000000 cuquantum_python-24.3.0.post0/cuda_autodetect.py
+-rw-r--r--   0 majones   (1000) majones   (1000)     1516 2024-05-07 20:37:13.000000 cuquantum_python-24.3.0.post0/LICENSE
+-rw-r--r--   0 majones   (1000) majones   (1000)       38 2024-05-07 21:02:40.000000 cuquantum_python-24.3.0.post0/setup.cfg
+drwxr-xr-x   0 majones   (1000) majones   (1000)        0 2024-05-07 21:02:40.000000 cuquantum_python-24.3.0.post0/cuquantum_python.egg-info/
+-rw-r--r--   0 majones   (1000) majones   (1000)        1 2024-05-07 21:02:40.000000 cuquantum_python-24.3.0.post0/cuquantum_python.egg-info/not-zip-safe
+-rw-r--r--   0 majones   (1000) majones   (1000)        1 2024-05-07 21:02:40.000000 cuquantum_python-24.3.0.post0/cuquantum_python.egg-info/dependency_links.txt
+-rw-r--r--   0 majones   (1000) majones   (1000)      245 2024-05-07 21:02:40.000000 cuquantum_python-24.3.0.post0/cuquantum_python.egg-info/SOURCES.txt
+-rw-r--r--   0 majones   (1000) majones   (1000)       16 2024-05-07 21:02:40.000000 cuquantum_python-24.3.0.post0/cuquantum_python.egg-info/top_level.txt
+-rw-r--r--   0 majones   (1000) majones   (1000)     2154 2024-05-09 21:18:53.000000 cuquantum_python-24.3.0.post0/cuquantum_python.egg-info/PKG-INFO
+-rw-r--r--   0 majones   (1000) majones   (1000)     3211 2024-05-09 21:19:21.000000 cuquantum_python-24.3.0.post0/setup.py
+-rw-r--r--   0 majones   (1000) majones   (1000)     2154 2024-05-09 21:18:46.000000 cuquantum_python-24.3.0.post0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cuquantum-python-23.6.0/LICENSE` & `cuquantum_python-24.3.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuquantum-python-23.6.0/PKG-INFO` & `cuquantum_python-24.3.0.post0/cuquantum_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum-python
-Version: 23.6.0
+Version: 24.3.0.post0
 Summary: NVIDIA cuQuantum Python
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
```

### Comparing `cuquantum-python-23.6.0/README.rst` & `cuquantum_python-24.3.0.post0/README.rst`

 * *Files identical despite different names*

### Comparing `cuquantum-python-23.6.0/cuda_autodetect.py` & `cuquantum_python-24.3.0.post0/cuda_autodetect.py`

 * *Files identical despite different names*

### Comparing `cuquantum-python-23.6.0/cuquantum_python.egg-info/PKG-INFO` & `cuquantum_python-24.3.0.post0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum-python
-Version: 23.6.0
+Version: 24.3.0.post0
 Summary: NVIDIA cuQuantum Python
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
```

### Comparing `cuquantum-python-23.6.0/setup.py` & `cuquantum_python-24.3.0.post0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021-2023, NVIDIA CORPORATION & AFFILIATES.
+# Copyright (c) 2021-2024, NVIDIA CORPORATION & AFFILIATES.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import glob
 import os
 import shutil
 import site
@@ -13,15 +13,15 @@
 
 import cuda_autodetect
 from cuda_autodetect import infer_best_package, bdist_wheel
 
 
 # Update this for every release
 # Must pin to the cuquantum-python-cuXX version
-package_ver = "23.06.0"
+package_ver = "24.03.0.post0"
 package_name = "cuquantum-python"
 
 
 # get project long description
 with open("README.rst") as f:
     long_description = f.read()
 
@@ -35,20 +35,19 @@
     # Case 1: generate sdist
     install_requires = []
     data_files = [('', ['cuda_autodetect.py',])]  # extra files to be copied into sdist
     cmdclass = {}
 else:
     # Case 2: install sdist
     install_requires = [f"{infer_best_package(package_name)}=={package_ver}",]
-    if 11000 <= cuda_autodetect.CUDA_RESOLUTION < 11010:
-        install_requires.append('cupy-cuda110')
-    elif 11010 <= cuda_autodetect.CUDA_RESOLUTION < 11020:
-        install_requires.append('cupy-cuda111')
-    elif 11020 <= cuda_autodetect.CUDA_RESOLUTION < 12000:
-        install_requires.append('cupy-cuda11x')
+    # For cuQuantum 24.03+, we need cuTENSOR 2.0+, meaning we can't use CuPy older than
+    # v13.0.0, and CuPy v13+ supports CUDA 11.2+ 
+    if 11020 <= cuda_autodetect.CUDA_RESOLUTION < 12000:
+        # no ambiguity for CUDA 11, cuquantum-python-cu11 would do the right thing
+        pass
     elif 12000 <= cuda_autodetect.CUDA_RESOLUTION < 13000:
         # no ambiguity for CUDA 12, cuquantum-python-cu12 would do the right thing
         pass
     else:
         # most likely we failed to detect the CUDA version, assume CUDA 11.2+
         install_requires.append('cupy-cuda11x')
     data_files = []
```

