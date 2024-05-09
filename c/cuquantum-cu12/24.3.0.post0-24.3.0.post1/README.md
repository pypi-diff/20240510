# Comparing `tmp/cuquantum_cu12-24.3.0.post0-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/cuquantum_cu12-24.3.0.post1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7528 bytes, number of entries: 6
-drwxr-xr-x  3.0 unx        0 bx stor 24-May-09 20:51 cuquantum_cu12-24.3.0.post0.dist-info/
--rw-r--r--  3.0 unx    11004 tx defN 24-May-08 02:35 cuquantum_cu12-24.3.0.post0.dist-info/LICENSE
--rw-r--r--  3.0 unx        1 tx stor 24-May-08 02:35 cuquantum_cu12-24.3.0.post0.dist-info/top_level.txt
--rw-r--r--  3.0 unx      109 tx defN 24-May-08 02:35 cuquantum_cu12-24.3.0.post0.dist-info/WHEEL
--rw-rw-r--  3.0 unx      427 tx defN 24-May-09 20:51 cuquantum_cu12-24.3.0.post0.dist-info/RECORD
--rw-r--r--  3.0 unx     2680 tx defN 24-May-09 20:06 cuquantum_cu12-24.3.0.post0.dist-info/METADATA
-6 files, 14221 bytes uncompressed, 6204 bytes compressed:  56.4%
+Zip file size: 7534 bytes, number of entries: 6
+drwxr-xr-x  3.0 unx        0 bx stor 24-May-09 22:21 cuquantum_cu12-24.3.0.post1.dist-info/
+-rw-r--r--  3.0 unx    11004 tx defN 24-May-09 22:21 cuquantum_cu12-24.3.0.post1.dist-info/LICENSE
+-rw-r--r--  3.0 unx        1 tx stor 24-May-09 22:21 cuquantum_cu12-24.3.0.post1.dist-info/top_level.txt
+-rw-r--r--  3.0 unx      109 tx defN 24-May-09 22:21 cuquantum_cu12-24.3.0.post1.dist-info/WHEEL
+-rw-rw-r--  3.0 unx      457 tx defN 24-May-09 22:21 cuquantum_cu12-24.3.0.post1.dist-info/RECORD
+-rw-r--r--  3.0 unx     2692 tx defN 24-May-09 22:21 cuquantum_cu12-24.3.0.post1.dist-info/METADATA
+6 files, 14263 bytes uncompressed, 6210 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cuquantum_cu12-24.3.0.post0.dist-info/
+Filename: cuquantum_cu12-24.3.0.post1.dist-info/
 Comment: 
 
-Filename: cuquantum_cu12-24.3.0.post0.dist-info/LICENSE
+Filename: cuquantum_cu12-24.3.0.post1.dist-info/LICENSE
 Comment: 
 
-Filename: cuquantum_cu12-24.3.0.post0.dist-info/top_level.txt
+Filename: cuquantum_cu12-24.3.0.post1.dist-info/top_level.txt
 Comment: 
 
-Filename: cuquantum_cu12-24.3.0.post0.dist-info/WHEEL
+Filename: cuquantum_cu12-24.3.0.post1.dist-info/WHEEL
 Comment: 
 
-Filename: cuquantum_cu12-24.3.0.post0.dist-info/RECORD
+Filename: cuquantum_cu12-24.3.0.post1.dist-info/RECORD
 Comment: 
 
-Filename: cuquantum_cu12-24.3.0.post0.dist-info/METADATA
+Filename: cuquantum_cu12-24.3.0.post1.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## Comparing `cuquantum_cu12-24.3.0.post0.dist-info/LICENSE` & `cuquantum_cu12-24.3.0.post1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cuquantum_cu12-24.3.0.post0.dist-info/METADATA` & `cuquantum_cu12-24.3.0.post1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cuquantum-cu12
-Version: 24.3.0.post0
+Version: 24.3.0.post1
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
 Project-URL: Documentation, https://docs.nvidia.com/cuda/cuquantum/
 Keywords: cuda,nvidia,state vector,tensor network,high-performance computing,quantum computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: custatevec-cu12 ==1.6.0
-Requires-Dist: cutensornet-cu12 ==2.4.0
+Requires-Dist: custatevec-cu12 ==1.6.0.post1
+Requires-Dist: cutensornet-cu12 ==2.4.0.post1
 
 **************************************************************************************
 cuQuantum SDK: A High-Performance Library for Accelerating Quantum Information Science
 **************************************************************************************
 
 `NVIDIA cuQuantum SDK <https://developer.nvidia.com/cuquantum-sdk>`_ is a high-performance library for quantum information science and beyond.
 Currently its primary target is *quantum circuit simulations* and it consists of two major components:
```

