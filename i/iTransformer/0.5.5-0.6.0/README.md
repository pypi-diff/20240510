# Comparing `tmp/iTransformer-0.5.5.tar.gz` & `tmp/itransformer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iTransformer-0.5.5.tar", last modified: Tue Jan 30 16:37:57 2024, max compression
+gzip compressed data, was "itransformer-0.6.0.tar", last modified: Fri May 10 14:33:17 2024, max compression
```

## Comparing `iTransformer-0.5.5.tar` & `itransformer-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 16:37:57.064415 iTransformer-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-30 16:37:49.000000 iTransformer-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-30 16:37:57.064415 iTransformer-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-01-30 16:37:49.000000 iTransformer-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 16:37:57.064415 iTransformer-0.5.5/iTransformer/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-30 16:37:49.000000 iTransformer-0.5.5/iTransformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-01-30 16:37:49.000000 iTransformer-0.5.5/iTransformer/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-01-30 16:37:49.000000 iTransformer-0.5.5/iTransformer/iTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-01-30 16:37:49.000000 iTransformer-0.5.5/iTransformer/iTransformer2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-01-30 16:37:49.000000 iTransformer-0.5.5/iTransformer/iTransformerFFT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-01-30 16:37:49.000000 iTransformer-0.5.5/iTransformer/revin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 16:37:57.064415 iTransformer-0.5.5/iTransformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-30 16:37:57.000000 iTransformer-0.5.5/iTransformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-01-30 16:37:57.000000 iTransformer-0.5.5/iTransformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 16:37:57.000000 iTransformer-0.5.5/iTransformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-30 16:37:57.000000 iTransformer-0.5.5/iTransformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-30 16:37:57.000000 iTransformer-0.5.5/iTransformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 16:37:57.064415 iTransformer-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-30 16:37:49.000000 iTransformer-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:17.967950 itransformer-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 14:33:14.000000 itransformer-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 14:33:17.967950 itransformer-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-05-10 14:33:14.000000 itransformer-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:17.963950 itransformer-0.6.0/iTransformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 14:33:14.000000 itransformer-0.6.0/iTransformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-10 14:33:14.000000 itransformer-0.6.0/iTransformer/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-10 14:33:14.000000 itransformer-0.6.0/iTransformer/iTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-10 14:33:14.000000 itransformer-0.6.0/iTransformer/iTransformer2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-10 14:33:14.000000 itransformer-0.6.0/iTransformer/iTransformerFFT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-10 14:33:14.000000 itransformer-0.6.0/iTransformer/revin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:17.967950 itransformer-0.6.0/iTransformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 14:33:17.000000 itransformer-0.6.0/iTransformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-10 14:33:17.000000 itransformer-0.6.0/iTransformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:33:17.000000 itransformer-0.6.0/iTransformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 14:33:17.000000 itransformer-0.6.0/iTransformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 14:33:17.000000 itransformer-0.6.0/iTransformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:33:17.967950 itransformer-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-10 14:33:14.000000 itransformer-0.6.0/setup.py
```

### Comparing `iTransformer-0.5.5/LICENSE` & `itransformer-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iTransformer-0.5.5/PKG-INFO` & `itransformer-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iTransformer
-Version: 0.5.5
+Version: 0.6.0
 Summary: iTransformer - Inverted Transformer Are Effective for Time Series Forecasting
 Home-page: https://github.com/lucidrains/iTransformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,time series forecasting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iTransformer-0.5.5/README.md` & `itransformer-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `iTransformer-0.5.5/iTransformer/attend.py` & `itransformer-0.6.0/iTransformer/attend.py`

 * *Files identical despite different names*

### Comparing `iTransformer-0.5.5/iTransformer/iTransformer.py` & `itransformer-0.6.0/iTransformer/iTransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
         self.to_qkv = nn.Sequential(
             nn.Linear(dim, dim_inner * 3, bias = False),
             Rearrange('b n (qkv h d) -> qkv b h n d', qkv = 3, h = heads)
         )
 
         self.to_v_gates = nn.Sequential(
-            nn.Linear(dim, dim_inner, bias = False),
-            nn.SiLU(),
-            Rearrange('b n (h d) -> b h n d', h = heads)
+            nn.Linear(dim, heads, bias = False),
+            nn.Sigmoid(),
+            Rearrange('b n h -> b h n 1', h = heads)
         )
 
         self.attend = Attend(flash = flash, dropout = dropout)
 
         self.to_out = nn.Sequential(
             Rearrange('b h n d -> b n (h d)'),
             nn.Linear(dim_inner, dim, bias = False),
```

### Comparing `iTransformer-0.5.5/iTransformer/iTransformer2D.py` & `itransformer-0.6.0/iTransformer/iTransformer2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 
         self.to_qkv = nn.Sequential(
             nn.Linear(dim, dim_inner * 3, bias = False),
             Rearrange('b n (qkv h d) -> qkv b h n d', qkv = 3, h = heads)
         )
 
         self.to_v_gates = nn.Sequential(
-            nn.Linear(dim, dim_inner, bias = False),
-            nn.SiLU(),
-            Rearrange('b n (h d) -> b h n d', h = heads)
+            nn.Linear(dim, heads, bias = False),
+            nn.Sigmoid(),
+            Rearrange('b n h -> b h n 1', h = heads)
         )
 
         self.attend = Attend(flash = flash, dropout = dropout, causal = causal)
 
         self.to_out = nn.Sequential(
             Rearrange('b h n d -> b n (h d)'),
             nn.Linear(dim_inner, dim, bias = False),
```

### Comparing `iTransformer-0.5.5/iTransformer/iTransformerFFT.py` & `itransformer-0.6.0/iTransformer/iTransformerFFT.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 
         self.to_qkv = nn.Sequential(
             nn.Linear(dim, dim_inner * 3, bias = False),
             Rearrange('b n (qkv h d) -> qkv b h n d', qkv = 3, h = heads)
         )
 
         self.to_v_gates = nn.Sequential(
-            nn.Linear(dim, dim_inner, bias = False),
-            nn.SiLU(),
-            Rearrange('b n (h d) -> b h n d', h = heads)
+            nn.Linear(dim, heads, bias = False),
+            nn.Sigmoid(),
+            Rearrange('b n h -> b h n 1', h = heads)
         )
 
         self.attend = Attend(flash = flash, dropout = dropout)
 
         self.to_out = nn.Sequential(
             Rearrange('b h n d -> b n (h d)'),
             nn.Linear(dim_inner, dim, bias = False),
```

### Comparing `iTransformer-0.5.5/iTransformer/revin.py` & `itransformer-0.6.0/iTransformer/revin.py`

 * *Files identical despite different names*

### Comparing `iTransformer-0.5.5/iTransformer.egg-info/PKG-INFO` & `itransformer-0.6.0/iTransformer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iTransformer
-Version: 0.5.5
+Version: 0.6.0
 Summary: iTransformer - Inverted Transformer Are Effective for Time Series Forecasting
 Home-page: https://github.com/lucidrains/iTransformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,time series forecasting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iTransformer-0.5.5/setup.py` & `itransformer-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'iTransformer',
   packages = find_packages(exclude=[]),
-  version = '0.5.5',
+  version = '0.6.0',
   license='MIT',
   description = 'iTransformer - Inverted Transformer Are Effective for Time Series Forecasting',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/iTransformer',
   keywords = [
```

