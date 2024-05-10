# Comparing `tmp/bio-image-unet-1.0.0a3.tar.gz` & `tmp/bio-image-unet-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-image-unet-1.0.0a3.tar", max compression
+gzip compressed data, was "bio-image-unet-1.0.0a4.tar", max compression
```

## Comparing `bio-image-unet-1.0.0a3.tar` & `bio-image-unet-1.0.0a4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1072 2022-06-27 10:34:59.772125 bio-image-unet-1.0.0a3/LICENSE
--rw-r--r--   0        0        0      544 2024-05-05 12:32:15.034287 bio-image-unet-1.0.0a3/README.md
--rw-r--r--   0        0        0     6148 2022-11-11 16:07:45.185829 bio-image-unet-1.0.0a3/biu/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-12 12:06:47.828861 bio-image-unet-1.0.0a3/biu/__init__.py
--rw-r--r--   0        0        0       32 2022-06-27 10:34:59.772305 bio-image-unet-1.0.0a3/biu/progress/__init__.py
--rw-r--r--   0        0        0      196 2022-06-27 10:34:59.772393 bio-image-unet-1.0.0a3/biu/progress/note.txt
--rw-r--r--   0        0        0     5969 2022-11-10 16:09:23.098804 bio-image-unet-1.0.0a3/biu/progress/progressnotifier.py
--rw-r--r--   0        0        0     6148 2022-11-11 15:52:42.902284 bio-image-unet-1.0.0a3/biu/siam_unet/.DS_Store
--rw-r--r--   0        0        0      610 2024-04-12 12:06:47.829705 bio-image-unet-1.0.0a3/biu/siam_unet/__init__.py
--rw-r--r--   0        0        0    13741 2024-04-12 12:06:47.829913 bio-image-unet-1.0.0a3/biu/siam_unet/data.py
--rw-r--r--   0        0        0      156 2022-06-27 10:34:59.773322 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/__cpu_count__.py
--rw-r--r--   0        0        0      656 2022-06-27 10:34:59.773399 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/__md5sum__.py
--rw-r--r--   0        0        0     1318 2022-06-27 10:34:59.773503 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/average_tifs.py
--rw-r--r--   0        0        0     1745 2022-06-27 10:34:59.773598 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/create_pixel_value_histogram.py
--rw-r--r--   0        0        0      257 2022-06-27 10:34:59.773681 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/cuda_test.py
--rw-r--r--   0        0        0     1397 2022-06-27 10:34:59.773959 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/extract_frame_of_movie.py
--rw-r--r--   0        0        0     4669 2022-06-27 10:34:59.774141 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/find_frame_of_image.py
--rw-r--r--   0        0        0      699 2022-06-27 10:34:59.774260 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/generate_plain_image.py
--rw-r--r--   0        0        0     5044 2022-09-14 12:28:05.579071 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py
--rw-r--r--   0        0        0     1442 2022-06-27 10:34:59.774530 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/low_mem_tif_utils.py
--rw-r--r--   0        0        0     1280 2022-06-27 10:34:59.774638 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/threshold_images.py
--rw-r--r--   0        0        0     3196 2022-06-27 10:34:59.774817 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/tif_to_mp4.py
--rw-r--r--   0        0        0     3914 2022-06-27 10:34:59.774949 bio-image-unet-1.0.0a3/biu/siam_unet/helpers/util.py
--rw-r--r--   0        0        0     3533 2024-05-05 12:32:15.034957 bio-image-unet-1.0.0a3/biu/siam_unet/losses.py
--rw-r--r--   0        0        0    11123 2024-05-05 12:32:15.035182 bio-image-unet-1.0.0a3/biu/siam_unet/predict.py
--rw-r--r--   0        0        0     5422 2024-05-05 12:32:15.035770 bio-image-unet-1.0.0a3/biu/siam_unet/siam_unet.py
--rw-r--r--   0        0        0     7891 2024-05-05 12:32:15.036066 bio-image-unet-1.0.0a3/biu/siam_unet/train.py
--rw-r--r--   0        0        0      329 2024-04-12 12:06:47.830762 bio-image-unet-1.0.0a3/biu/unet/__init__.py
--rw-r--r--   0        0        0     7148 2024-05-05 12:32:15.036490 bio-image-unet-1.0.0a3/biu/unet/attention_unet.py
--rw-r--r--   0        0        0     3456 2022-09-14 12:28:05.579805 bio-image-unet-1.0.0a3/biu/unet/baby_unet.py
--rw-r--r--   0        0        0    12210 2024-05-06 09:15:26.910839 bio-image-unet-1.0.0a3/biu/unet/data.py
--rw-r--r--   0        0        0     2868 2024-04-12 12:06:47.831488 bio-image-unet-1.0.0a3/biu/unet/losses.py
--rw-r--r--   0        0        0    10262 2024-05-06 09:15:26.911043 bio-image-unet-1.0.0a3/biu/unet/predict.py
--rw-r--r--   0        0        0     9004 2024-05-06 09:15:26.911479 bio-image-unet-1.0.0a3/biu/unet/train.py
--rw-r--r--   0        0        0     4298 2024-04-12 12:06:47.831999 bio-image-unet-1.0.0a3/biu/unet/unet.py
--rw-r--r--   0        0        0     4052 2024-05-06 09:15:26.911589 bio-image-unet-1.0.0a3/biu/unet/unet_v0.py
--rw-r--r--   0        0        0      291 2024-05-05 12:32:15.037423 bio-image-unet-1.0.0a3/biu/unet3d/__init__.py
--rw-r--r--   0        0        0    11989 2024-05-05 12:32:15.037643 bio-image-unet-1.0.0a3/biu/unet3d/data.py
--rw-r--r--   0        0        0     2868 2024-05-05 12:32:15.037758 bio-image-unet-1.0.0a3/biu/unet3d/losses.py
--rw-r--r--   0        0        0     8327 2024-05-06 09:15:26.912046 bio-image-unet-1.0.0a3/biu/unet3d/predict.py
--rw-r--r--   0        0        0     9323 2024-05-05 12:32:15.038232 bio-image-unet-1.0.0a3/biu/unet3d/train.py
--rw-r--r--   0        0        0     3369 2024-05-05 12:32:15.038361 bio-image-unet-1.0.0a3/biu/unet3d/unet3d.py
--rw-r--r--   0        0        0       21 2024-04-12 12:06:47.832254 bio-image-unet-1.0.0a3/biu/utils/__init__.py
--rw-r--r--   0        0        0     3742 2024-04-12 12:06:47.832351 bio-image-unet-1.0.0a3/biu/utils/test.py
--rw-r--r--   0        0        0     2264 2024-04-12 12:06:47.832460 bio-image-unet-1.0.0a3/biu/utils/utils.py
--rw-r--r--   0        0        0      636 2024-05-06 09:18:35.466461 bio-image-unet-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     1481 2024-05-06 09:18:41.729412 bio-image-unet-1.0.0a3/setup.py
--rw-r--r--   0        0        0     1414 2024-05-06 09:18:41.729575 bio-image-unet-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-27 10:34:59.772125 bio-image-unet-1.0.0a4/LICENSE
+-rw-r--r--   0        0        0      544 2024-05-05 12:32:15.034287 bio-image-unet-1.0.0a4/README.md
+-rw-r--r--   0        0        0     6148 2022-11-11 16:07:45.185829 bio-image-unet-1.0.0a4/biu/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-12 12:06:47.828861 bio-image-unet-1.0.0a4/biu/__init__.py
+-rw-r--r--   0        0        0       32 2022-06-27 10:34:59.772305 bio-image-unet-1.0.0a4/biu/progress/__init__.py
+-rw-r--r--   0        0        0      196 2022-06-27 10:34:59.772393 bio-image-unet-1.0.0a4/biu/progress/note.txt
+-rw-r--r--   0        0        0     5969 2022-11-10 16:09:23.098804 bio-image-unet-1.0.0a4/biu/progress/progressnotifier.py
+-rw-r--r--   0        0        0     6148 2022-11-11 15:52:42.902284 bio-image-unet-1.0.0a4/biu/siam_unet/.DS_Store
+-rw-r--r--   0        0        0      610 2024-04-12 12:06:47.829705 bio-image-unet-1.0.0a4/biu/siam_unet/__init__.py
+-rw-r--r--   0        0        0    13741 2024-04-12 12:06:47.829913 bio-image-unet-1.0.0a4/biu/siam_unet/data.py
+-rw-r--r--   0        0        0      156 2022-06-27 10:34:59.773322 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/__cpu_count__.py
+-rw-r--r--   0        0        0      656 2022-06-27 10:34:59.773399 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/__md5sum__.py
+-rw-r--r--   0        0        0     1318 2022-06-27 10:34:59.773503 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/average_tifs.py
+-rw-r--r--   0        0        0     1745 2022-06-27 10:34:59.773598 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/create_pixel_value_histogram.py
+-rw-r--r--   0        0        0      257 2022-06-27 10:34:59.773681 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/cuda_test.py
+-rw-r--r--   0        0        0     1397 2022-06-27 10:34:59.773959 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/extract_frame_of_movie.py
+-rw-r--r--   0        0        0     4669 2022-06-27 10:34:59.774141 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/find_frame_of_image.py
+-rw-r--r--   0        0        0      699 2022-06-27 10:34:59.774260 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_plain_image.py
+-rw-r--r--   0        0        0     5044 2022-09-14 12:28:05.579071 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py
+-rw-r--r--   0        0        0     1442 2022-06-27 10:34:59.774530 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/low_mem_tif_utils.py
+-rw-r--r--   0        0        0     1280 2022-06-27 10:34:59.774638 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/threshold_images.py
+-rw-r--r--   0        0        0     3196 2022-06-27 10:34:59.774817 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/tif_to_mp4.py
+-rw-r--r--   0        0        0     3914 2022-06-27 10:34:59.774949 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/util.py
+-rw-r--r--   0        0        0     3539 2024-05-10 17:20:33.893986 bio-image-unet-1.0.0a4/biu/siam_unet/losses.py
+-rw-r--r--   0        0        0    11386 2024-05-10 17:20:33.894445 bio-image-unet-1.0.0a4/biu/siam_unet/predict.py
+-rw-r--r--   0        0        0     5422 2024-05-05 12:32:15.035770 bio-image-unet-1.0.0a4/biu/siam_unet/siam_unet.py
+-rw-r--r--   0        0        0     8216 2024-05-10 17:20:33.894666 bio-image-unet-1.0.0a4/biu/siam_unet/train.py
+-rw-r--r--   0        0        0      329 2024-04-12 12:06:47.830762 bio-image-unet-1.0.0a4/biu/unet/__init__.py
+-rw-r--r--   0        0        0     7148 2024-05-05 12:32:15.036490 bio-image-unet-1.0.0a4/biu/unet/attention_unet.py
+-rw-r--r--   0        0        0     3456 2022-09-14 12:28:05.579805 bio-image-unet-1.0.0a4/biu/unet/baby_unet.py
+-rw-r--r--   0        0        0    12210 2024-05-06 09:15:26.910839 bio-image-unet-1.0.0a4/biu/unet/data.py
+-rw-r--r--   0        0        0     2868 2024-04-12 12:06:47.831488 bio-image-unet-1.0.0a4/biu/unet/losses.py
+-rw-r--r--   0        0        0    10592 2024-05-10 17:20:33.894890 bio-image-unet-1.0.0a4/biu/unet/predict.py
+-rw-r--r--   0        0        0     9362 2024-05-10 17:20:33.895131 bio-image-unet-1.0.0a4/biu/unet/train.py
+-rw-r--r--   0        0        0     4298 2024-04-12 12:06:47.831999 bio-image-unet-1.0.0a4/biu/unet/unet.py
+-rw-r--r--   0        0        0     4052 2024-05-06 09:15:26.911589 bio-image-unet-1.0.0a4/biu/unet/unet_v0.py
+-rw-r--r--   0        0        0      291 2024-05-05 12:32:15.037423 bio-image-unet-1.0.0a4/biu/unet3d/__init__.py
+-rw-r--r--   0        0        0    11989 2024-05-05 12:32:15.037643 bio-image-unet-1.0.0a4/biu/unet3d/data.py
+-rw-r--r--   0        0        0     2868 2024-05-05 12:32:15.037758 bio-image-unet-1.0.0a4/biu/unet3d/losses.py
+-rw-r--r--   0        0        0     8761 2024-05-10 17:20:33.895336 bio-image-unet-1.0.0a4/biu/unet3d/predict.py
+-rw-r--r--   0        0        0     9874 2024-05-10 17:20:33.895529 bio-image-unet-1.0.0a4/biu/unet3d/train.py
+-rw-r--r--   0        0        0     3956 2024-05-10 17:20:33.895730 bio-image-unet-1.0.0a4/biu/unet3d/unet3d.py
+-rw-r--r--   0        0        0       21 2024-04-12 12:06:47.832254 bio-image-unet-1.0.0a4/biu/utils/__init__.py
+-rw-r--r--   0        0        0     5039 2024-05-10 17:20:33.896485 bio-image-unet-1.0.0a4/biu/utils/test.py
+-rw-r--r--   0        0        0     2264 2024-04-12 12:06:47.832460 bio-image-unet-1.0.0a4/biu/utils/utils.py
+-rw-r--r--   0        0        0      636 2024-05-10 17:20:49.957960 bio-image-unet-1.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     1481 2024-05-10 17:20:55.743171 bio-image-unet-1.0.0a4/setup.py
+-rw-r--r--   0        0        0     1414 2024-05-10 17:20:55.743409 bio-image-unet-1.0.0a4/PKG-INFO
```

### Comparing `bio-image-unet-1.0.0a3/LICENSE` & `bio-image-unet-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/README.md` & `bio-image-unet-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/.DS_Store` & `bio-image-unet-1.0.0a4/biu/.DS_Store`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/progress/progressnotifier.py` & `bio-image-unet-1.0.0a4/biu/progress/progressnotifier.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/.DS_Store` & `bio-image-unet-1.0.0a4/biu/siam_unet/.DS_Store`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/__init__.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/__init__.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/data.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/data.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/__md5sum__.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/__md5sum__.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/average_tifs.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/average_tifs.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/create_pixel_value_histogram.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/create_pixel_value_histogram.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/extract_frame_of_movie.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/extract_frame_of_movie.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/find_frame_of_image.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/find_frame_of_image.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/generate_plain_image.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_plain_image.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/low_mem_tif_utils.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/low_mem_tif_utils.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/threshold_images.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/threshold_images.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/tif_to_mp4.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/tif_to_mp4.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/helpers/util.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/util.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/losses.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/losses.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
     def forward(self, logits, targets):
         x = self.dice(logits, targets)
         return torch.log((torch.exp(x) + torch.exp(-x)) / 2)
 
 
 class BCELoss2d(nn.Module):
-    def __init__(self, weight=None, size_average=True, **kwargs):
+    def __init__(self, weight=None, reduction='mean', **kwargs):
         super(BCELoss2d, self).__init__()
-        self.bce_loss = nn.BCELoss(weight, size_average)
+        self.bce_loss = nn.BCELoss(weight, reduction=reduction)
 
     def forward(self, logits, targets):
         probs = torch.sigmoid(logits)
         probs_flat = probs.view(-1)
         targets_flat = targets.view(-1)
         return self.bce_loss(probs_flat, targets_flat)
```

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/predict.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import os
+from typing import Union
 
 import numpy as np
 import tifffile
 import torch
 from tifffile.tifffile import TiffFile
 from tqdm import tqdm as tqdm
 from biu.progress import ProgressNotifier
 
 from .siam_unet import Siam_UNet
 from ..utils import get_device
 
-# select device
-device = get_device()
-
 
 class Predict:
     """
     Class for prediction of tif-movies.
     1) Loading file and preprocess (normalization)
     2) Resizing of images into patches with resize_dim
     3) Prediction with U-Net
     4) Stitching of predicted patches and averaging of overlapping regions
     """
 
     def __init__(self, tif_file, result_name, model_params, resize_dim=(512, 512), invert=False,
                  normalization_mode='single', clip_threshold=(0.0, 99.98), add_tile=0, normalize_result=False,
-                 show_progress=True, progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
+                 show_progress=True, device: Union[torch.device, str] = 'auto',
+                 progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
         """
         Predicts a tif movie
 
         Parameters
         ----------
         tif_file : str
             Path to input tif stack
@@ -47,31 +46,36 @@
             'all': based on histogram of full stack, 'first': based on histogram of first image in stack)
         clip_threshold : Tuple[float, float]
             Clip threshold for image intensity before prediction
         add_tile : int, optional
             Add additional tiles for splitting large images to increase overlap
         normalize_result : bool
             If True, results are normalized to [0, 255]
-        show_progress : bool
-            Whether to show progress bar and resize shape.
+        device : torch.device or str, optional
+            Device to run the pytorch model on, defaults to 'auto', which selects CUDA or MPS if available.
         progress_notifier:
             Wrapper to show tqdm progress notifier in gui
         """
+        if device == 'auto':
+            self.device = get_device()
+        else:
+            self.device = torch.device(device)
+
         self.tif_file = tif_file
         self.add_tile = add_tile
         self.invert = invert
         self.normalization_mode = normalization_mode
         self.clip_threshold = clip_threshold
         self.result_name = result_name
         self.normalize_result = normalize_result  # todo to be implemented for Siam-U-Net?
         self.show_progress = show_progress
 
         # load model
-        self.model_params = torch.load(model_params, map_location=device)
-        self.model = Siam_UNet(n_filter=self.model_params['n_filter'], mode=self.model_params['mode']).to(device)
+        self.model_params = torch.load(model_params, map_location=self.device)
+        self.model = Siam_UNet(n_filter=self.model_params['n_filter'], mode=self.model_params['mode']).to(self.device)
         self.model.load_state_dict(self.model_params['state_dict'])
         self.model.eval()
 
         # split data into groups of two images
         tif_key = TiffFile(self.tif_file)
         self.tif_len = len(tif_key.pages)
         self.imgs_shape = [self.tif_len, tif_key.pages[0].shape[0], tif_key.pages[0].shape[1]]
@@ -195,17 +199,17 @@
     def __predict(self, patches):
         result_patches = np.zeros((patches.shape[0], 1, patches.shape[2], patches.shape[3]), dtype='uint8')
         with torch.no_grad():
             for i, patch_i in enumerate(patches):
                 image_patch_i = patch_i[0, :, :]
                 prev_image_patch_i = patch_i[1, :, :]
 
-                image_patch_i = torch.from_numpy(image_patch_i.astype('float32') / 255).to(device).view(
+                image_patch_i = torch.from_numpy(image_patch_i.astype('float32') / 255).to(self.device).view(
                     (1, 1, self.resize_dim[0], self.resize_dim[1]))
-                prev_image_patch_i = torch.from_numpy(prev_image_patch_i.astype('float32') / 255).to(device).view(
+                prev_image_patch_i = torch.from_numpy(prev_image_patch_i.astype('float32') / 255).to(self.device).view(
                     (1, 1, self.resize_dim[0], self.resize_dim[1]))
 
                 res_i = self.model(image_patch_i, prev_image_patch_i)[0].view(
                     (1, self.resize_dim[0], self.resize_dim[1])).cpu().numpy() * 255
                 result_patches[i] = res_i.astype('uint8')
                 del patch_i, res_i
         return result_patches
```

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/siam_unet.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/siam_unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/siam_unet/train.py` & `bio-image-unet-1.0.0a4/biu/siam_unet/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import glob
 import os
+from typing import Union
 
 import torch
-import torch.nn as nn
 import torch.optim as optim
+from torch.utils.data import DataLoader, random_split
 from tqdm import tqdm
 
 from biu.siam_unet import BCEDiceLoss
-from torch.utils.data import DataLoader, random_split
-
 from . import logcoshTverskyLoss, TverskyLoss, weightedBCELoss
 from .predict import Predict
 from .siam_unet import Siam_UNet
 from ..utils import get_device
 
-# select device
-device = get_device()
-
 
 class Trainer:
     def __init__(self, dataset, num_epochs, batch_size=4, lr=1e-3, n_filter=32, mode='max', val_split=0.2,
                  save_dir='./', save_name='model.pth', save_iter=False, loss_function='BCEDice',
-                 loss_params=(1, 1), load_weights=None):
+                 loss_params=(1, 1), load_weights=None, device: Union[torch.device, str] = 'auto'):
         """
         Class for training of neural network. Creates trainer object, training is started with .start().
 
         Parameters
         ----------
         dataset
             Training data, object of PyTorch Dataset class
@@ -49,17 +45,23 @@
             If True, network state is save after each epoch
         load_weights : str, optional
             If not None, network state is loaded before training
         loss_function : str
             Loss function ('BCEDice', 'Tversky' or 'logcoshTversky')
         loss_params : Tuple[float, float]
             Parameter of loss function, depends on chosen loss function
+        device : torch.device or str, optional
+            Device to run the pytorch model on, defaults to 'auto', which selects CUDA or MPS if available.
         """
+        if device == 'auto':
+            self.device = get_device()
+        else:
+            self.device = torch.device(device)
 
-        self.model = Siam_UNet(n_filter=n_filter, mode=mode).to(device)
+        self.model = Siam_UNet(n_filter=n_filter, mode=mode).to(self.device)
 
         self.data = dataset
         self.num_epochs = num_epochs
         self.batch_size = batch_size
         self.lr = lr
         self.n_filter = n_filter
         self.mode = mode
@@ -94,34 +96,34 @@
             self.state = torch.load(load_weights)
             self.model.load_state_dict(self.state['state_dict'])
 
     def iterate(self, epoch, mode):
         if mode == 'train':
             print('\nStarting training epoch %s ...' % epoch)
             for i, batch_i in tqdm(enumerate(self.train_loader), total=len(self.train_loader), unit='batch'):
-                x_i = batch_i['image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                prev_x_i = batch_i['prev_image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                y_i = batch_i['mask'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
+                x_i = batch_i['image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(self.device)
+                prev_x_i = batch_i['prev_image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(self.device)
+                y_i = batch_i['mask'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(self.device)
                 # Forward pass: Compute predicted y by passing x to the model
                 y_pred, y_logits = self.model(x_i, prev_x_i)
                 # Compute loss
                 loss = self.criterion(y_logits, y_i)
                 # Zero gradients, perform a backward pass, and update the weights.
                 self.optimizer.zero_grad()
                 loss.backward()
                 self.optimizer.step()
 
         elif mode == 'val':
             loss_list = []
             print('\nStarting validation epoch %s ...' % epoch)
             with torch.no_grad():
                 for i, batch_i in tqdm(enumerate(self.val_loader), total=len(self.val_loader), unit='batch'):
-                    x_i = batch_i['image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                    prev_x_i = batch_i['prev_image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                    y_i = batch_i['mask'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
+                    x_i = batch_i['image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(self.device)
+                    prev_x_i = batch_i['prev_image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(self.device)
+                    y_i = batch_i['mask'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(self.device)
                     # Forward pass: Compute predicted y by passing x to the model
                     y_pred, y_logits = self.model(x_i, prev_x_i)
                     # Compute loss
                     loss = self.criterion(y_logits, y_i)
                     loss_list.append(loss.detach())
             val_loss = torch.stack(loss_list).mean()
             return val_loss
```

### Comparing `bio-image-unet-1.0.0a3/biu/unet/attention_unet.py` & `bio-image-unet-1.0.0a4/biu/unet/attention_unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet/baby_unet.py` & `bio-image-unet-1.0.0a4/biu/unet/baby_unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet/data.py` & `bio-image-unet-1.0.0a4/biu/unet/data.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet/losses.py` & `bio-image-unet-1.0.0a4/biu/unet/losses.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet/predict.py` & `bio-image-unet-1.0.0a4/biu/unet/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
+from typing import Union
+
 import numpy as np
 import tifffile
 import torch
 
 from ..progress import ProgressNotifier
 from .unet import Unet
 from .unet_v0 import Unet_v0
 from .attention_unet import AttentionUnet
 from ..utils import save_as_tif, get_device
 
-# select device
-device = get_device()
-
 
 class Predict:
     """Class for prediction of movies and images with U-Net"""
 
     def __init__(self, imgs, result_name, model_params, network='Unet', resize_dim=(512, 512),
                  invert=False, normalization_mode='single', clip_threshold=(0., 99.8), add_tile=0,
-                 normalize_result=False, show_progress=True,
+                 normalize_result=False, show_progress=True, device: Union[torch.device, str] = 'auto',
                  progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
         """
         Prediction of tif files with standard 2D U-Net
 
         1) Loading file and preprocess (normalization)
         2) Resizing of images into patches with resize_dim
         3) Prediction with U-Net
@@ -48,17 +47,24 @@
             Clip threshold for image intensity before prediction
         add_tile : int, optional
             Add additional tiles for splitting large images to increase overlap
         normalize_result : bool
             If true, results are normalized to [0, 255]
         show_progress : bool
             Whether to show progress bar.
+        device : torch.device or str, optional
+            Device to run the pytorch model on, defaults to 'auto', which selects CUDA or MPS if available.
         progress_notifier:
             Wrapper to show tqdm progress notifier in gui
         """
+        if device == 'auto':
+            self.device = get_device()
+        else:
+            self.device = torch.device(device)
+
         if isinstance(imgs, str):
             imgs = tifffile.imread(imgs)
 
         self.resize_dim = resize_dim
         self.add_tile = add_tile
         self.normalize_result = normalize_result
         self.invert = invert
@@ -70,15 +76,15 @@
         # read, preprocess and split data
         imgs = self.__reshape_data(imgs)
         imgs = self.__preprocess(imgs)
         patches = self.__split(imgs)
         del imgs
 
         # load model and predict data
-        self.model_params = torch.load(model_params, map_location=device)
+        self.model_params = torch.load(model_params, map_location=self.device)
         if network is None:
             if 'network' in self.model_params.keys():
                 network = self.model_params['network']
             else:
                 raise ValueError('network is not defined')
         if network == 'Unet':
             network = Unet
@@ -86,15 +92,15 @@
             network = AttentionUnet
         elif network == 'Unet_v0':
             network = Unet_v0
             if 'in_channels' not in self.model_params.keys():
                 self.model_params['in_channels'] = 1
                 self.model_params['out_channels'] = 1
         self.model = network(n_filter=self.model_params['n_filter'], in_channels=self.model_params['in_channels'],
-                             out_channels=self.model_params['out_channels']).to(device)
+                             out_channels=self.model_params['out_channels']).to(self.device)
         self.model.load_state_dict(self.model_params['state_dict'])
         self.model.eval()
         result_patches = self.__predict(patches, progress_notifier)
         del patches, self.model
 
         # stitch patches (mean of overlapped regions)
         imgs_result = self.__stitch(result_patches)
@@ -179,15 +185,15 @@
         result_patches = np.zeros((patches.shape[0], self.model_params['out_channels'], *patches.shape[2:]),
                                   dtype='uint8')
         print('Predicting data ...') if self.show_progress else None
         with torch.no_grad():
             _progress_notifier = enumerate(progress_notifier.iterator(patches)) if self.show_progress else enumerate(
                 patches)
             for i, patch_i in _progress_notifier:
-                patch_i = torch.from_numpy(patch_i.astype('float32') / 255).to(device).view((1,
+                patch_i = torch.from_numpy(patch_i.astype('float32') / 255).to(self.device).view((1,
                                                                                              self.model_params[
                                                                                                  'in_channels'],
                                                                                              self.resize_dim[0],
                                                                                              self.resize_dim[1]))
                 res_i, logits_i = self.model(patch_i)
                 res_i = res_i.view(
                     (self.model_params['out_channels'], self.resize_dim[0], self.resize_dim[1])).cpu().numpy()
```

### Comparing `bio-image-unet-1.0.0a3/biu/unet/train.py` & `bio-image-unet-1.0.0a4/biu/unet/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import glob
 import os
+from typing import Union
 
 import tifffile
 import torch.optim as optim
 from torch.utils.data import DataLoader, random_split
 from tqdm import tqdm
 
 from .losses import *
 from .predict import Predict
 from .unet import Unet
 from .attention_unet import AttentionUnet
 from ..utils import init_weights, get_device
 
-# get device
-device = get_device()
-
 
 class Trainer:
     def __init__(self, dataset, num_epochs, network=Unet, batch_size=4, lr=1e-3, in_channels=1, out_channels=1,
                  channel_weights=None, n_filter=64, dilation=1, val_split=0.2, save_dir='./', save_name='model.pth',
-                 save_iter=False, load_weights=False, loss_function='BCEDice', loss_params=(0.5, 0.5)):
+                 save_iter=False, load_weights=False, loss_function='BCEDice', loss_params=(0.5, 0.5),
+                 device: Union[torch.device, str] = 'auto'):
         """
         Class for training of neural network. Creates trainer object, training is started with .start().
 
         Parameters
         ----------
         dataset
             Training data, object of PyTorch Dataset class
@@ -53,18 +52,24 @@
             If True, network state is save after each epoch
         load_weights : str, optional
             If not None, network state is loaded before training
         loss_function : str
             Loss function ('BCEDice', 'Tversky' or 'logcoshTversky')
         loss_params : Tuple[float, float]
             Parameter of loss function, depends on chosen loss function
+        device : torch.device or str, optional
+            Device to run the pytorch model on, defaults to 'auto', which selects CUDA or MPS if available.
         """
+        if device == 'auto':
+            self.device = get_device()
+        else:
+            self.device = torch.device(device)
         self.network = network
         self.model = network(n_filter=n_filter, in_channels=in_channels, out_channels=out_channels,
-                             dilation=dilation).to(device)
+                             dilation=dilation).to(self.device)
         self.model.apply(init_weights)
         self.data = dataset
         self.num_epochs = num_epochs
         self.batch_size = batch_size
         self.lr = lr
         self.best_loss = torch.tensor(float('inf'))
         self.save_iter = save_iter
@@ -114,16 +119,16 @@
             self.state = torch.load(self.save_dir + '/' + self.save_name)
             self.model.load_state_dict(self.state['state_dict'])
 
     def __iterate(self, epoch, mode):
         if mode == 'train':
             print('\nStarting training epoch %s ...' % epoch)
             for i, batch_i in tqdm(enumerate(self.train_loader), total=len(self.train_loader), unit='batch'):
-                x_i = batch_i['image'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1]).to(device)
-                y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[0]).to(device)
+                x_i = batch_i['image'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1]).to(self.device)
+                y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[0]).to(self.device)
                 # Forward pass: Compute predicted y by passing x to the model
                 y_pred, y_logits = self.model(x_i)
 
                 # Compute loss
                 loss = sum([self.criterion(y_logits[ch], y_i[ch]) * self.channel_weights[j] for j, ch in
                             enumerate(range(self.out_channels))]) / sum(self.channel_weights)
 
@@ -133,16 +138,16 @@
                 self.optimizer.step()
 
         elif mode == 'val':
             loss_list = []
             print('\nStarting validation epoch %s ...' % epoch)
             with torch.no_grad():
                 for i, batch_i in tqdm(enumerate(self.val_loader), total=len(self.val_loader), unit='batch'):
-                    x_i = batch_i['image'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1]).to(device)
-                    y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[1]).to(device)
+                    x_i = batch_i['image'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1]).to(self.device)
+                    y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[1]).to(self.device)
                     # Forward pass: Compute predicted y by passing x to the model
                     y_pred, y_logits = self.model(x_i)
                     # Compute loss
                     loss = sum([self.criterion(y_logits[ch], y_i[ch]) * self.channel_weights[j] for j, ch in
                                 enumerate(range(self.out_channels))]) / sum(self.channel_weights)
                 loss_list.append(loss.detach())
             val_loss = torch.stack(loss_list).mean()
```

### Comparing `bio-image-unet-1.0.0a3/biu/unet/unet.py` & `bio-image-unet-1.0.0a4/biu/unet/unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet/unet_v0.py` & `bio-image-unet-1.0.0a4/biu/unet/unet_v0.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet3d/data.py` & `bio-image-unet-1.0.0a4/biu/unet3d/data.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet3d/losses.py` & `bio-image-unet-1.0.0a4/biu/unet3d/losses.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/biu/unet3d/predict.py` & `bio-image-unet-1.0.0a4/biu/unet3d/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+from typing import Union
+
 import numpy as np
 import tifffile
 import torch
 
 from .unet3d import UNet3D
 from ..progress import ProgressNotifier
 from ..utils import save_as_tif, get_device
 
-# select device
-device = get_device()
-
 
 class Predict:
     """Class for prediction of movies and images with U-Net"""
 
     def __init__(self, vol, result_name, model_params, network=UNet3D, resize_dim=(512, 512),
                  invert=False, normalization_mode='single', clip_threshold=(0., 99.8), add_patch=0,
-                 normalize_result=False, progress_bar=True,
+                 normalize_result=False, progress_bar=True, device: Union[torch.device, str] = 'auto',
                  progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
         """
         Prediction of tif files with standard 2D U-Net
 
         1) Loading file and preprocess (normalization)
         2) Resizing of images into patches with resize_dim
         3) Prediction with U-Net
@@ -44,20 +43,29 @@
             'all': based on histogram of full stack, 'first': based on histogram of first image in stack)
         clip_threshold : Tuple[float, float]
             Clip threshold for image intensity before prediction
         add_patch : int, optional
             Add additional patches for splitting large images to increase overlap
         normalize_result : bool
             If true, results are normalized to [0, 255]
+        progress_bar : bool, optional
+            Whether to display progress bar during prediction.
+        device : torch.device, optional
+            Device to run pytorch model on. Default is 'auto', which selects CUDA or MPS if available.
         progress_notifier:
             Wrapper to show tqdm progress notifier in gui
         """
         if isinstance(vol, str):
             vol = tifffile.imread(vol)
 
+        if device == 'auto':
+            self.device = get_device()
+        else:
+            self.device = torch.device(device)
+
         self.resize_dim = resize_dim
         self.add_patch = add_patch
         self.normalize_result = normalize_result
         self.invert = invert
         self.normalization_mode = normalization_mode
         self.clip_threshold = clip_threshold
         self.result_name = result_name
@@ -66,17 +74,17 @@
         # read, preprocess and split data
         vol = self.__reshape_data(vol)
         vol = self.__preprocess(vol)
         patches = self.__split(vol)
         del vol
 
         # load model and predict data
-        self.model_params = torch.load(model_params, map_location=device)
+        self.model_params = torch.load(model_params, map_location=self.device)
         self.model = network(n_filter=self.model_params['n_filter'], in_channels=self.model_params['in_channels'],
-                             out_channels=self.model_params['out_channels']).to(device)
+                             out_channels=self.model_params['out_channels']).to(self.device)
         self.model.load_state_dict(self.model_params['state_dict'])
         self.model.eval()
         result_patches = self.__predict(patches, progress_notifier)
         del patches, self.model
 
         # stitch patches (mean of overlapped regions)
         vol_result = self.__stitch(result_patches)
@@ -144,18 +152,18 @@
     def __predict(self, patches, progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
         result_patches = np.zeros_like(patches, dtype='uint8')
         print('Predicting data ...') if self.progress_bar else None
         with torch.no_grad():
             _progress_notifier = enumerate(progress_notifier.iterator(patches)) if self.progress_bar else enumerate(
                 patches)
             for i, patch_i in _progress_notifier:
-                patch_i = torch.from_numpy(patch_i.astype('float32') / 255).to(device).view((1, 1,
-                                                                                             self.resize_dim[0],
-                                                                                             self.resize_dim[1],
-                                                                                             self.resize_dim[2]))
+                patch_i = torch.from_numpy(patch_i.astype('float32') / 255).to(self.device).view((1, 1,
+                                                                                                  self.resize_dim[0],
+                                                                                                  self.resize_dim[1],
+                                                                                                  self.resize_dim[2]))
                 res_i, logits_i = self.model(patch_i)
                 res_i = res_i.view(
                     (self.resize_dim[0], self.resize_dim[1], self.resize_dim[2])).cpu().numpy()
                 result_patches[i] = (res_i * 255).astype('uint8')
                 del patch_i, res_i
         return result_patches
```

### Comparing `bio-image-unet-1.0.0a3/biu/unet3d/train.py` & `bio-image-unet-1.0.0a4/biu/unet3d/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import glob
 import os
+from typing import Union
 
 import tifffile
 import torch.optim as optim
 from torch.utils.data import DataLoader, random_split
 from tqdm import tqdm
 
 from .unet3d import UNet3D
 from .losses import *
 from .predict import Predict
 from ..utils import init_weights, get_device
 
-# get device
-device = get_device()
-
 
 class Trainer:
-    def __init__(self, dataset, num_epochs, network=UNet3D, batch_size=4, lr=1e-3, in_channels=1, out_channels=1,
-                 channel_weights=None, n_filter=64, dilation=1, val_split=0.2, save_dir='./', save_name='model.pth',
-                 save_iter=False, load_weights=False, loss_function='BCEDice', loss_params=(0.5, 0.5),
-                 time_loss_weight=0.1):
+    def __init__(self, dataset, num_epochs, network=UNet3D, use_interpolation=False, batch_size=4, lr=1e-3,
+                 in_channels=1, out_channels=1, channel_weights=None, n_filter=64, dilation=1, val_split=0.2,
+                 save_dir='./', save_name='model.pth', save_iter=False, load_weights=False, loss_function='BCEDice',
+                 loss_params=(0.5, 0.5), time_loss_weight=0.1, device: Union[torch.device, str] = 'auto'):
         """
         Class for training of neural network. Creates trainer object, training is started with .start().
 
         Parameters
         ----------
         dataset
             Training data, object of PyTorch Dataset class
         num_epochs : int
             Number of training epochs
         network
             Network class (Default Unet)
+        use_interpolation : bool
+            Whether to use interpolation in decoder instead of transpose convolution.
         batch_size : int
             Batch size for training
         lr : float
             Learning rate
         in_channels : int
             Number of input channels
         out_channels : int
@@ -53,17 +53,24 @@
             If True, network state is save after each epoch
         load_weights : str, optional
             If not None, network state is loaded before training
         loss_function : str
             Loss function ('BCEDice', 'Tversky' or 'logcoshTversky')
         loss_params : Tuple[float, float]
             Parameter of loss function, depends on chosen loss function
+        device : torch.device or str, optional
+            Device to run the pytorch model on, defaults to 'auto', which selects CUDA or MPS if available.
         """
+        if device == 'auto':
+            self.device = get_device()
+        else:
+            self.device = torch.device(device)
         self.network = network
-        self.model = network(n_filter=n_filter, in_channels=in_channels, out_channels=out_channels).to(device)
+        self.model = network(n_filter=n_filter, in_channels=in_channels, out_channels=out_channels,
+                             use_interpolation=use_interpolation).to(self.device)
         self.model.apply(init_weights)
         self.data = dataset
         self.num_epochs = num_epochs
         self.batch_size = batch_size
         self.lr = lr
         self.best_loss = torch.tensor(float('inf'))
         self.save_iter = save_iter
@@ -116,16 +123,16 @@
             self.state = torch.load(self.save_dir + '/' + self.save_name)
             self.model.load_state_dict(self.state['state_dict'])
 
     def __iterate(self, epoch, mode):
         if mode == 'train':
             print('\nStarting training epoch %s ...' % epoch)
             for i, batch_i in tqdm(enumerate(self.train_loader), total=len(self.train_loader), unit='batch'):
-                x_i = batch_i['volume'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1], self.dim[2]).to(device)
-                y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[1], self.dim[2]).to(device)
+                x_i = batch_i['volume'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1], self.dim[2]).to(self.device)
+                y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[1], self.dim[2]).to(self.device)
 
                 # Forward pass: Compute predicted y by passing x to the model
                 y_pred, y_logits = self.model(x_i)
 
                 # Compute segmentation loss
                 loss_seg = self.criterion(y_logits, y_i)
 
@@ -140,16 +147,16 @@
                 self.optimizer.step()
 
         elif mode == 'val':
             loss_list = []
             print('\nStarting validation epoch %s ...' % epoch)
             with torch.no_grad():
                 for i, batch_i in tqdm(enumerate(self.val_loader), total=len(self.val_loader), unit='batch'):
-                    x_i = batch_i['volume'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1], self.dim[2]).to(device)
-                    y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[1], self.dim[2]).to(device)
+                    x_i = batch_i['volume'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1], self.dim[2]).to(self.device)
+                    y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[1], self.dim[2]).to(self.device)
 
                     # Forward pass: Compute predicted y by passing x to the model
                     y_pred, y_logits = self.model(x_i)
 
                     # Compute loss
                     loss_seg = self.criterion(y_logits, y_i)
```

### Comparing `bio-image-unet-1.0.0a3/biu/unet3d/unet3d.py` & `bio-image-unet-1.0.0a4/biu/unet3d/unet3d.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import torch
 from torch import nn
+import torch.nn.functional as F
 
 
 class UNet3D(nn.Module):
-    def __init__(self, in_channels=1, out_channels=1, n_filter=16):
+    def __init__(self, in_channels=1, out_channels=1, n_filter=16, use_interpolation=False):
         """
         Neural network for time-consistent segmentation or volume segmentation,
         adapted from Li, X. et al. Real-time denoising enables high-sensitivity fluorescence time-lapse imaging
         beyond the shot-noise limit. Nat Biotechnol 41, 282–292 (2023).
 
 
         Parameters
         ----------
         n_filter : int
             Number of convolutional filters (commonly 16, 32, or 64)
         """
         super().__init__()
+        self.use_interpolation = use_interpolation
+
         # encode
         self.encode1 = self.conv3D(in_channels=in_channels, out_channels=n_filter // 2)
         self.encode2 = self.conv3D(n_filter // 2, n_filter)
         self.maxpool1 = nn.MaxPool3d(kernel_size=2, stride=2)
         self.encode3 = self.conv3D(n_filter, n_filter)
         self.encode4 = self.conv3D(n_filter, 2 * n_filter)
         self.maxpool2 = nn.MaxPool3d(kernel_size=2, stride=2)
@@ -28,21 +31,23 @@
         self.maxpool3 = nn.MaxPool3d(kernel_size=2, stride=2)
 
         # middle
         self.middle_conv1 = self.conv3D(4 * n_filter, 4 * n_filter)
         self.middle_conv2 = self.conv3D(4 * n_filter, 8 * n_filter)
 
         # decode
-        self.up1 = nn.ConvTranspose3d(8 * n_filter, 8 * n_filter, kernel_size=2, stride=2)
+        if not use_interpolation:
+            self.up1 = nn.ConvTranspose3d(8 * n_filter, 8 * n_filter, kernel_size=2, stride=2)
+            self.up2 = nn.ConvTranspose3d(4 * n_filter, 4 * n_filter, kernel_size=2, stride=2)
+            self.up3 = nn.ConvTranspose3d(2 * n_filter, 2 * n_filter, kernel_size=2, stride=2)
+
         self.decode1 = self.conv3D(12 * n_filter, 4 * n_filter)
         self.decode2 = self.conv3D(4 * n_filter, 4 * n_filter)
-        self.up2 = nn.ConvTranspose3d(4 * n_filter, 4 * n_filter, kernel_size=2, stride=2)
         self.decode3 = self.conv3D(6 * n_filter, 2 * n_filter)
         self.decode4 = self.conv3D(2 * n_filter, 2 * n_filter)
-        self.up3 = nn.ConvTranspose3d(2 * n_filter, 2 * n_filter, kernel_size=2, stride=2)
         self.decode5 = self.conv3D(3 * n_filter, n_filter)
         self.decode6 = self.conv3D(n_filter, n_filter // 2)
         self.final = nn.Conv3d(n_filter // 2, out_channels=out_channels, kernel_size=1, padding=0)
 
     def conv3D(self, in_channels, out_channels, kernel_size=3, dropout=0., dilation=1):
         layers = [
             nn.Conv3d(in_channels, out_channels, kernel_size, padding=dilation, dilation=dilation),
@@ -64,21 +69,30 @@
         e5 = self.encode5(m2)
         e6 = self.encode6(e5)
         m3 = self.maxpool3(e6)
 
         mid1 = self.middle_conv1(m3)
         mid2 = self.middle_conv2(mid1)
 
-        u1 = self.up1(mid2)
+        if self.use_interpolation:
+            u1 = F.interpolate(mid2, scale_factor=2, mode='trilinear', align_corners=False)
+        else:
+            u1 = self.up1(mid2)
         c1 = self.concat(u1, e6)
         d1 = self.decode1(c1)
         d2 = self.decode2(d1)
-        u2 = self.up2(d2)
+        if self.use_interpolation:
+            u2 = F.interpolate(d2, scale_factor=2, mode='trilinear', align_corners=False)
+        else:
+            u2 = self.up2(d2)
         c2 = self.concat(u2, e4)
         d3 = self.decode3(c2)
         d4 = self.decode4(d3)
-        u3 = self.up3(d4)
+        if self.use_interpolation:
+            u3 = F.interpolate(d4, scale_factor=2, mode='trilinear', align_corners=False)
+        else:
+            u3 = self.up3(d4)
         c3 = self.concat(u3, e2)
         d5 = self.decode5(c3)
         d6 = self.decode6(d5)
         logits = self.final(d6)
         return torch.sigmoid(logits), logits
```

### Comparing `bio-image-unet-1.0.0a3/biu/utils/test.py` & `bio-image-unet-1.0.0a4/biu/utils/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import gc
 
 import numpy as np
 import tifffile
 
 import biu.siam_unet as siam
 import biu.unet as unet
+from biu import unet3d
 # create test folder with random training and test data
 from biu.progress import ProgressNotifier
 
 folder = './temp_test/'
 
 
 def test_unet():
@@ -75,14 +76,44 @@
     train_siam.start()
 
     # predict movie
     siam.Predict(folder + 'movie.tif', result_name=folder_results + 'movie.tif',
                  model_params=folder + 'models_siam/model.pth', resize_dim=(64, 64),
                  progress_notifier=ProgressNotifier())
 
+def test_unet3d():
+    folder_image = folder + 'training_data_3d/image/'
+    folder_mask = folder + 'training_data_3d/mask/'
+    folder_results = folder + 'results/'
+    os.makedirs(folder_image, exist_ok=True)
+    os.makedirs(folder_mask, exist_ok=True)
+    os.makedirs(folder_results, exist_ok=True)
+
+    for i in range(5):
+        # regular unet
+        random_image = np.random.randint(0, 255, (32, 128, 128))
+        random_mask = np.random.randint(0, 255, (32, 128, 128))
+        tifffile.imwrite(folder_image + f'{i}.tif', random_image)
+        tifffile.imwrite(folder_mask + f'{i}.tif', random_mask)
+
+    random_movie = np.random.randint(0, 255, (32, 128, 128))
+    tifffile.imwrite(folder + 'movie.tif', random_movie)
+
+    # create training data set
+    data = unet3d.DataProcess(source_dir=(folder_image, folder_mask), dim_out=(32, 64, 64), data_path=folder + 'data/')
+
+    # train
+    train = unet3d.Trainer(data, num_epochs=4, n_filter=8, save_dir=folder + 'models_unet3d/')
+    train.start()
+
+    # predict movie
+    unet3d.Predict(folder + 'movie.tif', result_name=folder_results + 'movie.tif',
+                 model_params=folder + 'models_unet3d/model.pth', resize_dim=(16, 64, 64),
+                 progress_notifier=ProgressNotifier())
+
 
 def delete_folder_with_retry(folder, max_attempts=5, wait_seconds=2):
     for attempt in range(max_attempts):
         try:
             gc.collect()  # Force garbage collection
             shutil.rmtree(folder)
             print(f"Successfully deleted {folder}")
@@ -96,10 +127,11 @@
     else:
         print(f"Failed to delete {folder} after {max_attempts} attempts.")
 
 
 if __name__ == "__main__":
     test_unet()
     test_siam_unet()
+    test_unet3d()
     # delete test folder
     delete_folder_with_retry(folder)
     print("*" * 20 + " \nTests completed successfully")
```

### Comparing `bio-image-unet-1.0.0a3/biu/utils/utils.py` & `bio-image-unet-1.0.0a4/biu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a3/pyproject.toml` & `bio-image-unet-1.0.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "bio-image-unet"
 packages = [
     { include = "biu" }
 ]
-version = "1.0.0-alpha.3"
+version = "1.0.0-alpha.4"
 description = "Implementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation"
 authors = ["Daniel Haertter", "Yuxi Long"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/danihae/bio-image-unet"
 
 [tool.poetry.dependencies]
```

### Comparing `bio-image-unet-1.0.0a3/setup.py` & `bio-image-unet-1.0.0a4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-image>0.18,<1.0',
  'tifffile',
  'torch>=2.0.0,<3.0.0',
  'tqdm>=4.61,<5.0']
 
 setup_kwargs = {
     'name': 'bio-image-unet',
-    'version': '1.0.0a3',
+    'version': '1.0.0a4',
     'description': 'Implementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation',
     'long_description': '# Bio Image U-Net\n\nImplementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation\n\n\n## Installation\n### PyPI\n``pip install bio-image-unet``\n### GitHub\n``pip install git+https://github.com/danihae/bio-image-unet``\n\n## Usage example\nImport package with ``import biu``\n\n[iPython Notebook for getting started with U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_unet.ipynb) \\\n[iPython Notebook for getting started with Siam U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_siam_unet.ipynb)\n',
     'author': 'Daniel Haertter',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/danihae/bio-image-unet',
```

### Comparing `bio-image-unet-1.0.0a3/PKG-INFO` & `bio-image-unet-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-image-unet
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Implementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation
 Home-page: https://github.com/danihae/bio-image-unet
 License: MIT
 Author: Daniel Haertter
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

