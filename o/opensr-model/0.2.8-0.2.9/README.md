# Comparing `tmp/opensr_model-0.2.8.tar.gz` & `tmp/opensr_model-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr_model-0.2.8.tar", last modified: Tue Apr 16 13:49:42 2024, max compression
+gzip compressed data, was "opensr_model-0.2.9.tar", last modified: Tue Apr 16 13:59:54 2024, max compression
```

## Comparing `opensr_model-0.2.8.tar` & `opensr_model-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:42.631736 opensr_model-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-16 13:49:28.000000 opensr_model-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 13:49:42.631736 opensr_model-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 13:49:28.000000 opensr_model-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:42.627736 opensr_model-0.2.8/opensr_model/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:42.627736 opensr_model-0.2.8/opensr_model/autoencoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/autoencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/autoencoder/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/autoencoder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:42.631736 opensr_model-0.2.8/opensr_model/denoiser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/denoiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31569 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/denoiser/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40344 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/denoiser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:42.631736 opensr_model-0.2.8/opensr_model/diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37548 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/diffusion/latentdiffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    34445 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/diffusion/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/predict_pl_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    19722 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/srmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-16 13:49:28.000000 opensr_model-0.2.8/opensr_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:49:42.631736 opensr_model-0.2.8/opensr_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 13:49:42.000000 opensr_model-0.2.8/opensr_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-16 13:49:42.000000 opensr_model-0.2.8/opensr_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:49:42.000000 opensr_model-0.2.8/opensr_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 13:49:42.000000 opensr_model-0.2.8/opensr_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 13:49:42.000000 opensr_model-0.2.8/opensr_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:49:42.631736 opensr_model-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-16 13:49:28.000000 opensr_model-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:54.555472 opensr_model-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-16 13:59:41.000000 opensr_model-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 13:59:54.555472 opensr_model-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 13:59:41.000000 opensr_model-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:54.551472 opensr_model-0.2.9/opensr_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:54.551472 opensr_model-0.2.9/opensr_model/autoencoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/autoencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/autoencoder/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/autoencoder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:54.551472 opensr_model-0.2.9/opensr_model/denoiser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/denoiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31569 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/denoiser/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40344 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/denoiser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:54.555472 opensr_model-0.2.9/opensr_model/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37548 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/diffusion/latentdiffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34445 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/diffusion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/predict_pl_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19752 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/srmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-16 13:59:41.000000 opensr_model-0.2.9/opensr_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:54.555472 opensr_model-0.2.9/opensr_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 13:59:54.000000 opensr_model-0.2.9/opensr_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-16 13:59:54.000000 opensr_model-0.2.9/opensr_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:59:54.000000 opensr_model-0.2.9/opensr_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 13:59:54.000000 opensr_model-0.2.9/opensr_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 13:59:54.000000 opensr_model-0.2.9/opensr_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:59:54.555472 opensr_model-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-16 13:59:41.000000 opensr_model-0.2.9/setup.py
```

### Comparing `opensr_model-0.2.8/LICENSE` & `opensr_model-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/PKG-INFO` & `opensr_model-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensr-model
-Version: 0.2.8
+Version: 0.2.9
 Summary: ESA OpenSR Diffusion model package for Super-Resolution of Senintel-2 Imagery
 Home-page: https://isp.uv.es/opensr/
 Author: Simon Donike, Cesar Aybar, Luis Gomez Chova, Freddie Kalaitzis
 Author-email: accounts@donike.net
 License: MIT
 Project-URL: Source Code, https://github.com/ESAopenSR/opensr-model
 Description-Content-Type: text/markdown
```

### Comparing `opensr_model-0.2.8/opensr_model/__init__.py` & `opensr_model-0.2.9/opensr_model/__init__.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/autoencoder/autoencoder.py` & `opensr_model-0.2.9/opensr_model/autoencoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/autoencoder/utils.py` & `opensr_model-0.2.9/opensr_model/autoencoder/utils.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/denoiser/unet.py` & `opensr_model-0.2.9/opensr_model/denoiser/unet.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/denoiser/utils.py` & `opensr_model-0.2.9/opensr_model/denoiser/utils.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/diffusion/latentdiffusion.py` & `opensr_model-0.2.9/opensr_model/diffusion/latentdiffusion.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/diffusion/utils.py` & `opensr_model-0.2.9/opensr_model/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/predict_pl_workflow.py` & `opensr_model-0.2.9/opensr_model/predict_pl_workflow.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model/srmodel.py` & `opensr_model-0.2.9/opensr_model/srmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,15 +429,15 @@
             p = self.xai_step(x, idx)
             return(p)
     
     def xai_step(self, x, idx):
         no_uncertainty = 10 # amount of images to SR
         variations = []
         for i in range(no_uncertainty):
-            sr = self.model.forwardl(x)
+            sr = self.model.forward(x,custom_steps=self.custom_steps)
             sr = sr.squeeze(0)
             variations.append(sr.detach().cpu())
         variations = torch.stack(variations)
         # Get statistics for xAI
         srs_mean = variations.mean(dim=0)
         srs_stdev = variations.std(dim=0)
         lower_bound = srs_mean-srs_stdev
```

### Comparing `opensr_model-0.2.8/opensr_model/utils.py` & `opensr_model-0.2.9/opensr_model/utils.py`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/opensr_model.egg-info/PKG-INFO` & `opensr_model-0.2.9/opensr_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensr-model
-Version: 0.2.8
+Version: 0.2.9
 Summary: ESA OpenSR Diffusion model package for Super-Resolution of Senintel-2 Imagery
 Home-page: https://isp.uv.es/opensr/
 Author: Simon Donike, Cesar Aybar, Luis Gomez Chova, Freddie Kalaitzis
 Author-email: accounts@donike.net
 License: MIT
 Project-URL: Source Code, https://github.com/ESAopenSR/opensr-model
 Description-Content-Type: text/markdown
```

### Comparing `opensr_model-0.2.8/opensr_model.egg-info/SOURCES.txt` & `opensr_model-0.2.9/opensr_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensr_model-0.2.8/setup.py` & `opensr_model-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='opensr-model',
-    version='0.2.8',
+    version='0.2.9',
     author = "Simon Donike, Cesar Aybar, Luis Gomez Chova, Freddie Kalaitzis",
     author_email = "accounts@donike.net",
     description = "ESA OpenSR Diffusion model package for Super-Resolution of Senintel-2 Imagery",
     url = "https://isp.uv.es/opensr/",
     project_urls={'Source Code': 'https://github.com/ESAopenSR/opensr-model'},
     license='MIT',
     packages=find_packages(),
```

