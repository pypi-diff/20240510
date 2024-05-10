# Comparing `tmp/cesnet_models-0.1.2.tar.gz` & `tmp/cesnet_models-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet_models-0.1.2.tar", last modified: Thu May  2 07:30:41 2024, max compression
+gzip compressed data, was "cesnet_models-0.1.3.tar", last modified: Thu May  9 14:43:02 2024, max compression
```

## Comparing `cesnet_models-0.1.2.tar` & `cesnet_models-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.565347 cesnet_models-0.1.2/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_models-0.1.2/LICENCE
--rw-rw-rw-   0        0        0     3557 2024-05-02 07:30:41.564345 cesnet_models-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2024-04-10 08:36:57.000000 cesnet_models-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.538796 cesnet_models-0.1.2/cesnet_models/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.2/cesnet_models/__init__.py
--rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet_models-0.1.2/cesnet_models/_models_meta.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.562348 cesnet_models-0.1.2/cesnet_models/architectures/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.2/cesnet_models/architectures/__init__.py
--rw-rw-rw-   0        0        0     2131 2024-04-30 13:12:57.000000 cesnet_models-0.1.2/cesnet_models/architectures/cnn_resblock.py
--rw-rw-rw-   0        0        0     8583 2024-04-30 15:07:58.000000 cesnet_models-0.1.2/cesnet_models/architectures/multimodal_cesnet.py
--rw-rw-rw-   0        0        0     9979 2024-04-30 15:51:58.000000 cesnet_models-0.1.2/cesnet_models/architectures/multimodal_cesnet_enhanced.py
--rw-rw-rw-   0        0        0       71 2024-04-29 12:31:20.000000 cesnet_models-0.1.2/cesnet_models/constants.py
--rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet_models-0.1.2/cesnet_models/helpers.py
--rw-rw-rw-   0        0        0    11966 2024-04-30 13:57:45.000000 cesnet_models-0.1.2/cesnet_models/models.py
--rw-rw-rw-   0        0        0    14604 2024-04-30 12:17:48.000000 cesnet_models-0.1.2/cesnet_models/transforms.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.563346 cesnet_models-0.1.2/cesnet_models.egg-info/
--rw-rw-rw-   0        0        0     3557 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1448 2024-05-02 07:30:07.000000 cesnet_models-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 07:30:41.565347 cesnet_models-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 14:43:02.299803 cesnet_models-0.1.3/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_models-0.1.3/LICENCE
+-rw-rw-rw-   0        0        0     3557 2024-05-09 14:43:02.299803 cesnet_models-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2024-04-10 08:36:57.000000 cesnet_models-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 14:43:02.268676 cesnet_models-0.1.3/cesnet_models/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.3/cesnet_models/__init__.py
+-rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet_models-0.1.3/cesnet_models/_models_meta.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:43:02.296531 cesnet_models-0.1.3/cesnet_models/architectures/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.3/cesnet_models/architectures/__init__.py
+-rw-rw-rw-   0        0        0     2149 2024-05-07 21:14:32.000000 cesnet_models-0.1.3/cesnet_models/architectures/cnn_resblock.py
+-rw-rw-rw-   0        0        0     8585 2024-05-09 12:13:33.000000 cesnet_models-0.1.3/cesnet_models/architectures/multimodal_cesnet.py
+-rw-rw-rw-   0        0        0    14668 2024-05-09 13:32:03.000000 cesnet_models-0.1.3/cesnet_models/architectures/multimodal_cesnet_enhanced.py
+-rw-rw-rw-   0        0        0       71 2024-04-29 12:31:20.000000 cesnet_models-0.1.3/cesnet_models/constants.py
+-rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet_models-0.1.3/cesnet_models/helpers.py
+-rw-rw-rw-   0        0        0    11966 2024-05-07 10:23:57.000000 cesnet_models-0.1.3/cesnet_models/models.py
+-rw-rw-rw-   0        0        0    14604 2024-04-30 12:17:48.000000 cesnet_models-0.1.3/cesnet_models/transforms.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:43:02.297640 cesnet_models-0.1.3/cesnet_models.egg-info/
+-rw-rw-rw-   0        0        0     3557 2024-05-09 14:43:02.000000 cesnet_models-0.1.3/cesnet_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-05-09 14:43:02.000000 cesnet_models-0.1.3/cesnet_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:43:02.000000 cesnet_models-0.1.3/cesnet_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2024-05-09 14:43:02.000000 cesnet_models-0.1.3/cesnet_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-09 14:43:02.000000 cesnet_models-0.1.3/cesnet_models.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1448 2024-05-09 14:42:16.000000 cesnet_models-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:43:02.299803 cesnet_models-0.1.3/setup.cfg
```

### Comparing `cesnet_models-0.1.2/LICENCE` & `cesnet_models-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.2/PKG-INFO` & `cesnet_models-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
```

### Comparing `cesnet_models-0.1.2/README.md` & `cesnet_models-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.2/cesnet_models/_models_meta.py` & `cesnet_models-0.1.3/cesnet_models/_models_meta.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.2/cesnet_models/architectures/cnn_resblock.py` & `cesnet_models-0.1.3/cesnet_models/architectures/cnn_resblock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 
-class ResBlock(nn.Module):
+class SimpleResBlock(nn.Module):
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  ):
             super().__init__()
 
             self.cnn = nn.Sequential(
@@ -40,16 +40,16 @@
                  channels1: int = 64,
                  channels2: int = 128,
                  ):
             super().__init__()
 
             self.conv1 = nn.Conv1d(ppi_input_channels, channels1, kernel_size=3, stride=1, padding=1)
             self.bn1 = nn.BatchNorm1d(channels1)
-            self.block1 = ResBlock(channels1, channels1)
-            self.block2 = ResBlock(channels1, channels2)
+            self.block1 = SimpleResBlock(channels1, channels1)
+            self.block2 = SimpleResBlock(channels1, channels2)
             self.classifier = nn.Linear(channels2, num_classes)
 
     def _forward_impl(self, ppi):
         out = self.conv1(ppi)
         out = self.bn1(out)
         out = self.block1(out)
         out = self.block2(out)
```

### Comparing `cesnet_models-0.1.2/cesnet_models/architectures/multimodal_cesnet.py` & `cesnet_models-0.1.3/cesnet_models/architectures/multimodal_cesnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,33 +10,33 @@
     BATCH_NORM = "batch-norm"
     GROUP_NORM = "group-norm"
     LAYER_NORM = "layer-norm"
     INSTANCE_NORM = "instance-norm"
     NO_NORM = "no-norm"
     def __str__(self): return self.value
 
-def conv_norm_from_enum(size: int, norm_enum: NormalizationEnum, group_norm_groups: int = 8):
+def conv_norm_from_enum(size: int, norm_enum: NormalizationEnum, group_norm_groups: int = 16):
     if norm_enum == NormalizationEnum.BATCH_NORM:
-        return [nn.BatchNorm1d(size)]
+        return nn.BatchNorm1d(size)
     elif norm_enum == NormalizationEnum.GROUP_NORM:
-        return [nn.GroupNorm(num_groups=group_norm_groups, num_channels=size)]
+        return nn.GroupNorm(num_channels=size, num_groups=group_norm_groups)
     elif norm_enum == NormalizationEnum.INSTANCE_NORM:
-        return [nn.InstanceNorm1d(size)]
+        return nn.InstanceNorm1d(size)
     elif norm_enum == NormalizationEnum.NO_NORM:
-        return []
+        return nn.Identity()
     else:
         raise ValueError(f"Bad normalization for nn.Conv1d: {str(norm_enum)}")
 
 def linear_norm_from_enum(size: int, norm_enum: NormalizationEnum):
     if norm_enum == NormalizationEnum.BATCH_NORM:
-        return [nn.BatchNorm1d(size)]
+        return nn.BatchNorm1d(size)
     if norm_enum == NormalizationEnum.LAYER_NORM:
-        return [nn.LayerNorm(size)]
+        return nn.LayerNorm(size)
     elif norm_enum == NormalizationEnum.NO_NORM:
-        return []
+        return nn.Identity()
     else:
         raise ValueError(f"Bad normalization for nn.Linear: {str(norm_enum)}")
 
 class GeM(nn.Module):
     """
     https://www.kaggle.com/code/scaomath/g2net-1d-cnn-gem-pool-pytorch-train-inference
     """
@@ -95,74 +95,74 @@
             mlp_shared_input_size += cnn_ppi_channels3 * CNN_PPI_OUTPUT_LEN
 
         self.cnn_ppi = nn.Sequential(
             # [(W−K+2P)/S]+1
             # Input: 30 * 3
             nn.Conv1d(self.ppi_input_channels, cnn_ppi_channels1, kernel_size=7, stride=1, groups=conv1d_groups, padding=3),
             nn.ReLU(inplace=False),
-            *conv_norm(cnn_ppi_channels1),
+            conv_norm(cnn_ppi_channels1),
 
             # 30 x channels1
             *(nn.Sequential(
                 nn.Conv1d(cnn_ppi_channels1, cnn_ppi_channels1, kernel_size=5, stride=1, groups=conv1d_groups, padding=2),
                 nn.ReLU(inplace=False),
-                *conv_norm(cnn_ppi_channels1),) for _ in range(cnn_ppi_num_blocks)),
+                conv_norm(cnn_ppi_channels1),) for _ in range(cnn_ppi_num_blocks)),
 
             # 30 x channels1
             nn.Conv1d(cnn_ppi_channels1, cnn_ppi_channels2, kernel_size=5, stride=1),
             nn.ReLU(inplace=False),
-            *conv_norm(cnn_ppi_channels2),
+            conv_norm(cnn_ppi_channels2),
             # 26 * channels2
             nn.Conv1d(cnn_ppi_channels2, cnn_ppi_channels2, kernel_size=5, stride=1),
             nn.ReLU(inplace=False),
-            *conv_norm(cnn_ppi_channels2),
+            conv_norm(cnn_ppi_channels2),
             # 22 * channels2
             nn.Conv1d(cnn_ppi_channels2, cnn_ppi_channels3, kernel_size=4, stride=2),
             nn.ReLU(inplace=False),
             # 10 * channels3
             # CNN_PPI_OUTPUT_LEN = 10
         )
         if cnn_ppi_use_pooling:
             self.cnn_global_pooling = nn.Sequential(
                 GeM(kernel_size=CNN_PPI_OUTPUT_LEN),
                 nn.Flatten(),
-                *linear_norm(cnn_ppi_channels3),
+                linear_norm(cnn_ppi_channels3),
                 nn.Dropout(cnn_ppi_dropout_rate),
             )
         else:
             self.cnn_flatten_without_pooling = nn.Sequential(
                 nn.Flatten(),
-                *linear_norm(cnn_ppi_channels3 * CNN_PPI_OUTPUT_LEN),
+                linear_norm(cnn_ppi_channels3 * CNN_PPI_OUTPUT_LEN),
                 nn.Dropout(cnn_ppi_dropout_rate),
             )
         self.mlp_flowstats = nn.Sequential(
             nn.Linear(mlp_flowstats_input_size, mlp_flowstats_size1),
             nn.ReLU(inplace=False),
-            *linear_norm(mlp_flowstats_size1),
+            linear_norm(mlp_flowstats_size1),
 
             *(nn.Sequential(
                 nn.Linear(mlp_flowstats_size1, mlp_flowstats_size1),
                 nn.ReLU(inplace=False),
-                *linear_norm(mlp_flowstats_size1)) for _ in range(mlp_flowstats_num_hidden)),
+                linear_norm(mlp_flowstats_size1)) for _ in range(mlp_flowstats_num_hidden)),
 
             nn.Linear(mlp_flowstats_size1, mlp_flowstats_size2),
             nn.ReLU(inplace=False),
-            *linear_norm(mlp_flowstats_size2),
+            linear_norm(mlp_flowstats_size2),
             nn.Dropout(mlp_flowstats_dropout_rate),
         )
         self.mlp_shared = nn.Sequential(
             nn.Linear(mlp_shared_input_size, mlp_shared_size),
             nn.ReLU(inplace=False),
-            *linear_norm(mlp_shared_size),
+            linear_norm(mlp_shared_size),
             nn.Dropout(mlp_shared_dropout_rate),
 
             *(nn.Sequential(
                 nn.Linear(mlp_shared_size, mlp_shared_size),
                 nn.ReLU(inplace=False),
-                *linear_norm(mlp_shared_size),
+                linear_norm(mlp_shared_size),
                 nn.Dropout(mlp_shared_dropout_rate)) for _ in range(mlp_shared_num_hidden)),
         )
         self.classifier = nn.Linear(mlp_shared_size, num_classes)
 
     def _forward_impl(self, ppi, flowstats):
         out = self.cnn_ppi(ppi)
         if self.cnn_ppi_use_pooling:
```

### Comparing `cesnet_models-0.1.2/cesnet_models/helpers.py` & `cesnet_models-0.1.3/cesnet_models/helpers.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.2/cesnet_models/models.py` & `cesnet_models-0.1.3/cesnet_models/models.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.2/cesnet_models/transforms.py` & `cesnet_models-0.1.3/cesnet_models/transforms.py`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.2/cesnet_models.egg-info/PKG-INFO` & `cesnet_models-0.1.3/cesnet_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
```

### Comparing `cesnet_models-0.1.2/cesnet_models.egg-info/SOURCES.txt` & `cesnet_models-0.1.3/cesnet_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesnet_models-0.1.2/pyproject.toml` & `cesnet_models-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-models"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

