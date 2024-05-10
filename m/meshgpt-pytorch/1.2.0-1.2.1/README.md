# Comparing `tmp/meshgpt_pytorch-1.2.0.tar.gz` & `tmp/meshgpt_pytorch-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt_pytorch-1.2.0.tar", last modified: Fri May 10 17:54:10 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.1.tar", last modified: Fri May 10 17:58:44 2024, max compression
```

## Comparing `meshgpt_pytorch-1.2.0.tar` & `meshgpt_pytorch-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    50365 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50407 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/setup.py
```

### Comparing `meshgpt_pytorch-1.2.0/LICENSE` & `meshgpt_pytorch-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.0/PKG-INFO` & `meshgpt_pytorch-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
@@ -25,9 +25,9 @@
 Requires-Dist: numpy
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: taylor-series-linear-attention>=0.1.6
 Requires-Dist: torch>=2.1
 Requires-Dist: torch_geometric
 Requires-Dist: torchtyping
 Requires-Dist: tqdm
-Requires-Dist: vector-quantize-pytorch>=1.12.8
+Requires-Dist: vector-quantize-pytorch>=1.14.22
 Requires-Dist: x-transformers>=1.26.0
```

### Comparing `meshgpt_pytorch-1.2.0/README.md` & `meshgpt_pytorch-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.0/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.1/meshgpt_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.0/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.1/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,16 @@
             quantize_dropout_multiple_of = 1,
         ),
         rvq_kwargs: dict = dict(
             kmeans_init = True,
             threshold_ema_dead_code = 2,
         ),
         rlfq_kwargs: dict = dict(
-            frac_per_sample_entropy = 1.
+            frac_per_sample_entropy = 1.,
+            soft_clamp_input_value = 10.
         ),
         rvq_stochastic_sample_codes = True,
         sageconv_kwargs: dict = dict(
             normalize = True,
             project = True
         ),
         commit_loss_weight = 0.1,
```

### Comparing `meshgpt_pytorch-1.2.0/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.1/meshgpt_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
@@ -25,9 +25,9 @@
 Requires-Dist: numpy
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: taylor-series-linear-attention>=0.1.6
 Requires-Dist: torch>=2.1
 Requires-Dist: torch_geometric
 Requires-Dist: torchtyping
 Requires-Dist: tqdm
-Requires-Dist: vector-quantize-pytorch>=1.12.8
+Requires-Dist: vector-quantize-pytorch>=1.14.22
 Requires-Dist: x-transformers>=1.26.0
```

### Comparing `meshgpt_pytorch-1.2.0/setup.py` & `meshgpt_pytorch-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     'numpy',
     'pytorch-custom-utils>=0.0.9',
     'taylor-series-linear-attention>=0.1.6',
     'torch>=2.1',
     'torch_geometric',
     'torchtyping',
     'tqdm',
-    'vector-quantize-pytorch>=1.12.8',
+    'vector-quantize-pytorch>=1.14.22',
     'x-transformers>=1.26.0',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
```

