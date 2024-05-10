# Comparing `tmp/pms_encoder-0.0.3.tar.gz` & `tmp/pms_encoder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pms_encoder-0.0.3.tar", max compression
+gzip compressed data, was "pms_encoder-0.0.4.tar", max compression
```

## Comparing `pms_encoder-0.0.3.tar` & `pms_encoder-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       14 2024-05-09 05:03:07.501861 pms_encoder-0.0.3/README.md
--rw-r--r--   0        0        0       21 2024-05-09 06:24:23.493636 pms_encoder-0.0.3/pms_encoder/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 08:06:38.018830 pms_encoder-0.0.3/pms_encoder/common/__init__.py
--rw-r--r--   0        0        0     1132 2024-04-26 08:17:07.818517 pms_encoder-0.0.3/pms_encoder/common/_mysql_client.py
--rw-r--r--   0        0        0      430 2024-04-22 04:28:43.595684 pms_encoder-0.0.3/pms_encoder/common/_redis_client.py
--rw-r--r--   0        0        0      264 2024-04-19 06:20:36.942200 pms_encoder-0.0.3/pms_encoder/common/data_struct.py
--rw-r--r--   0        0        0       83 2024-04-22 05:41:52.374096 pms_encoder-0.0.3/pms_encoder/encoder/__init__.py
--rw-r--r--   0        0        0      328 2024-04-19 02:13:11.495941 pms_encoder-0.0.3/pms_encoder/encoder/_image_encoder.py
--rw-r--r--   0        0        0     3984 2024-04-26 05:59:21.734942 pms_encoder-0.0.3/pms_encoder/encoder/_video_encoder.py
--rw-r--r--   0        0        0        0 2024-04-19 08:51:59.078657 pms_encoder-0.0.3/pms_encoder/encoder/processor/__init__.py
--rw-r--r--   0        0        0     7390 2024-04-26 09:46:26.871534 pms_encoder-0.0.3/pms_encoder/encoder/processor/_video_processor.py
--rw-r--r--   0        0        0        0 2024-04-26 07:08:26.644245 pms_encoder-0.0.3/pms_encoder/encoder/redis/__init__.py
--rw-r--r--   0        0        0      266 2024-04-22 04:34:34.408615 pms_encoder-0.0.3/pms_encoder/encoder/redis/_progress.py
--rw-r--r--   0        0        0        0 2024-04-24 01:37:21.991083 pms_encoder-0.0.3/pms_encoder/encoder/repository/__init__.py
--rw-r--r--   0        0        0     1108 2024-04-26 08:14:42.976527 pms_encoder-0.0.3/pms_encoder/encoder/repository/_file_status_repo.py
--rw-r--r--   0        0        0     1638 2024-04-26 08:23:39.472819 pms_encoder-0.0.3/pms_encoder/encoder/repository/_video_meta_repo.py
--rw-r--r--   0        0        0        0 2024-04-19 02:29:29.646151 pms_encoder-0.0.3/pms_encoder/encoder/utils/__init__.py
--rw-r--r--   0        0        0      446 2024-04-22 07:14:07.738949 pms_encoder-0.0.3/pms_encoder/encoder/utils/_calculate_progress.py
--rw-r--r--   0        0        0      950 2024-04-26 03:39:29.023184 pms_encoder-0.0.3/pms_encoder/encoder/utils/_delete_file_util.py
--rw-r--r--   0        0        0     4571 2024-04-22 07:32:04.298739 pms_encoder-0.0.3/pms_encoder/encoder/utils/_queue_object_generator.py
--rw-r--r--   0        0        0      531 2024-04-26 08:25:54.330799 pms_encoder-0.0.3/pms_encoder/encoder/utils/_sub_output_util.py
--rw-r--r--   0        0        0    10615 2024-04-26 03:11:48.449690 pms_encoder-0.0.3/pms_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py
--rw-r--r--   0        0        0     2739 2024-05-09 06:29:09.269065 pms_encoder-0.0.3/pms_encoder/encoder_factory.py
--rw-r--r--   0        0        0      399 2024-05-09 06:29:22.852848 pms_encoder-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 pms_encoder-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       14 2024-05-09 05:03:07.501861 pms_encoder-0.0.4/README.md
+-rw-r--r--   0        0        0       21 2024-05-09 06:24:23.493636 pms_encoder-0.0.4/pms_encoder/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:06:38.018830 pms_encoder-0.0.4/pms_encoder/common/__init__.py
+-rw-r--r--   0        0        0     1132 2024-04-26 08:17:07.818517 pms_encoder-0.0.4/pms_encoder/common/_mysql_client.py
+-rw-r--r--   0        0        0      430 2024-04-22 04:28:43.595684 pms_encoder-0.0.4/pms_encoder/common/_redis_client.py
+-rw-r--r--   0        0        0      264 2024-04-19 06:20:36.942200 pms_encoder-0.0.4/pms_encoder/common/data_struct.py
+-rw-r--r--   0        0        0       83 2024-04-22 05:41:52.374096 pms_encoder-0.0.4/pms_encoder/encoder/__init__.py
+-rw-r--r--   0        0        0      328 2024-04-19 02:13:11.495941 pms_encoder-0.0.4/pms_encoder/encoder/_image_encoder.py
+-rw-r--r--   0        0        0     4013 2024-05-09 06:37:58.372644 pms_encoder-0.0.4/pms_encoder/encoder/_video_encoder.py
+-rw-r--r--   0        0        0        0 2024-04-19 08:51:59.078657 pms_encoder-0.0.4/pms_encoder/encoder/processor/__init__.py
+-rw-r--r--   0        0        0     7390 2024-04-26 09:46:26.871534 pms_encoder-0.0.4/pms_encoder/encoder/processor/_video_processor.py
+-rw-r--r--   0        0        0        0 2024-04-26 07:08:26.644245 pms_encoder-0.0.4/pms_encoder/encoder/redis/__init__.py
+-rw-r--r--   0        0        0      266 2024-04-22 04:34:34.408615 pms_encoder-0.0.4/pms_encoder/encoder/redis/_progress.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:37:21.991083 pms_encoder-0.0.4/pms_encoder/encoder/repository/__init__.py
+-rw-r--r--   0        0        0     1108 2024-04-26 08:14:42.976527 pms_encoder-0.0.4/pms_encoder/encoder/repository/_file_status_repo.py
+-rw-r--r--   0        0        0     1638 2024-04-26 08:23:39.472819 pms_encoder-0.0.4/pms_encoder/encoder/repository/_video_meta_repo.py
+-rw-r--r--   0        0        0        0 2024-04-19 02:29:29.646151 pms_encoder-0.0.4/pms_encoder/encoder/utils/__init__.py
+-rw-r--r--   0        0        0      446 2024-04-22 07:14:07.738949 pms_encoder-0.0.4/pms_encoder/encoder/utils/_calculate_progress.py
+-rw-r--r--   0        0        0      950 2024-04-26 03:39:29.023184 pms_encoder-0.0.4/pms_encoder/encoder/utils/_delete_file_util.py
+-rw-r--r--   0        0        0     4571 2024-04-22 07:32:04.298739 pms_encoder-0.0.4/pms_encoder/encoder/utils/_queue_object_generator.py
+-rw-r--r--   0        0        0      531 2024-04-26 08:25:54.330799 pms_encoder-0.0.4/pms_encoder/encoder/utils/_sub_output_util.py
+-rw-r--r--   0        0        0    10615 2024-04-26 03:11:48.449690 pms_encoder-0.0.4/pms_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py
+-rw-r--r--   0        0        0     2739 2024-05-09 06:29:09.269065 pms_encoder-0.0.4/pms_encoder/encoder_factory.py
+-rw-r--r--   0        0        0      399 2024-05-09 06:38:04.100553 pms_encoder-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 pms_encoder-0.0.4/PKG-INFO
```

### Comparing `pms_encoder-0.0.3/pms_encoder/common/_mysql_client.py` & `pms_encoder-0.0.4/pms_encoder/common/_mysql_client.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/_video_encoder.py` & `pms_encoder-0.0.4/pms_encoder/encoder/_video_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import asyncio
 import ffmpeg
 import pms_inference_engine as E
+import pms_furiosa_processor
 # import processor._video_processor as v_processor
 from loguru import logger
 from queue import Queue
 from .processor import _video_processor as v_processor
 from .repository._file_status_repo import *
 from .repository._video_meta_repo import insert_inferenced_file_meta
 from .utils import _delete_file_util as dfu
```

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/processor/_video_processor.py` & `pms_encoder-0.0.4/pms_encoder/encoder/processor/_video_processor.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/repository/_file_status_repo.py` & `pms_encoder-0.0.4/pms_encoder/encoder/repository/_file_status_repo.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/repository/_video_meta_repo.py` & `pms_encoder-0.0.4/pms_encoder/encoder/repository/_video_meta_repo.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/utils/_delete_file_util.py` & `pms_encoder-0.0.4/pms_encoder/encoder/utils/_delete_file_util.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/utils/_queue_object_generator.py` & `pms_encoder-0.0.4/pms_encoder/encoder/utils/_queue_object_generator.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/utils/_sub_output_util.py` & `pms_encoder-0.0.4/pms_encoder/encoder/utils/_sub_output_util.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py` & `pms_encoder-0.0.4/pms_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/pms_encoder/encoder_factory.py` & `pms_encoder-0.0.4/pms_encoder/encoder_factory.py`

 * *Files identical despite different names*

### Comparing `pms_encoder-0.0.3/PKG-INFO` & `pms_encoder-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pms-encoder
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: heeyong.kwon
 Author-email: heeyong.kwon@4by4inc.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

