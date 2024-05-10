# Comparing `tmp/Deep-KAN-0.0.1.tar.gz` & `tmp/Deep-KAN-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Deep-KAN-0.0.1.tar", last modified: Mon May  6 09:26:19 2024, max compression
+gzip compressed data, was "Deep-KAN-0.0.2.tar", last modified: Thu May  9 17:16:15 2024, max compression
```

## Comparing `Deep-KAN-0.0.1.tar` & `Deep-KAN-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:26:19.195472 Deep-KAN-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:26:19.195472 Deep-KAN-0.0.1/Deep_KAN.egg-info/
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-06 09:26:19.000000 Deep-KAN-0.0.1/Deep_KAN.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-06 09:26:19.000000 Deep-KAN-0.0.1/Deep_KAN.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:26:19.000000 Deep-KAN-0.0.1/Deep_KAN.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-06 09:26:19.000000 Deep-KAN-0.0.1/Deep_KAN.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-06 09:26:19.000000 Deep-KAN-0.0.1/Deep_KAN.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-06 09:26:19.195472 Deep-KAN-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 09:25:36.000000 Deep-KAN-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:26:19.195472 Deep-KAN-0.0.1/deepkan/
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-06 09:25:06.000000 Deep-KAN-0.0.1/deepkan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7125 2024-05-06 09:24:14.000000 Deep-KAN-0.0.1/deepkan/deepkan.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 09:26:19.195472 Deep-KAN-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      768 2024-05-06 09:22:37.000000 Deep-KAN-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/Deep_KAN.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3774 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3774 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3423 2024-05-09 17:14:52.000000 Deep-KAN-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/deepkan/
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-09 16:55:46.000000 Deep-KAN-0.0.2/deepkan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8122 2024-05-09 16:54:53.000000 Deep-KAN-0.0.2/deepkan/deepkan.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      768 2024-05-09 16:56:07.000000 Deep-KAN-0.0.2/setup.py
```

### Comparing `Deep-KAN-0.0.1/deepkan/deepkan.py` & `Deep-KAN-0.0.2/deepkan/deepkan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import torch
 import torch.nn.functional as F
 import torch.optim as optim
+import torch.nn as nn
+import numpy as np
 
 class SplineLinearLayer(torch.nn.Module):
     def __init__(self, input_dim, output_dim, num_knots=5, spline_order=3,
                  noise_scale=0.1, base_scale=1.0, spline_scale=1.0,
                  activation=torch.nn.SiLU, grid_epsilon=0.02, grid_range=[-1, 1],
                  standalone_spline_scaling=True):
         super(SplineLinearLayer, self).__init__()
@@ -145,8 +147,33 @@
         Args:
             regularize_activation (float): Regularization strength for activation.
             regularize_entropy (float): Regularization strength for entropy.
 
         Returns:
             torch.Tensor: Regularization loss.
         """
-        return sum(layer._regularization_loss(regularize_activation, regularize_entropy) for layer in self.layers)
+        return sum(layer._regularization_loss(regularize_activation, regularize_entropy) for layer in self.layers)
+
+
+
+
+class ChebyshevKANLayer(nn.Module):
+    def __init__(self, input_dim, output_dim, degree):
+        super(ChebyshevKANLayer, self).__init__()
+        self.inputdim = input_dim
+        self.outdim = output_dim
+        self.degree = degree
+
+        self.cheby_coeffs = nn.Parameter(torch.empty(input_dim, output_dim, degree + 1))
+        nn.init.xavier_uniform_(self.cheby_coeffs, gain=nn.init.calculate_gain('relu'))
+
+    def forward(self, x):
+        x = torch.reshape(x, (-1, self.inputdim))  
+        x = torch.tanh(x)
+        cheby = torch.ones(x.shape[0], self.inputdim, self.degree + 1, device=x.device)
+        if self.degree > 0:
+            cheby[:, :, 1] = x
+        for i in range(2, self.degree + 1):
+            cheby[:, :, i] = 2 * x * cheby[:, :, i - 1].clone() - cheby[:, :, i - 2].clone()
+        y = torch.einsum('bid,iod->bo', cheby, self.cheby_coeffs)  
+        y = y.view(-1, self.outdim)
+        return y
```

### Comparing `Deep-KAN-0.0.1/setup.py` & `Deep-KAN-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Deep-KAN',
-    version='0.0.1',
+    version='0.0.2',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Implimentation of Kolmogorov–Arnold Networks(KAN)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

