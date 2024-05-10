# Comparing `tmp/iscasmodel-0.8.tar.gz` & `tmp/iscasmodel-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscasmodel-0.8.tar", last modified: Mon Dec 25 05:38:13 2023, max compression
+gzip compressed data, was "iscasmodel-0.9.tar", last modified: Tue Dec 26 07:19:02 2023, max compression
```

## Comparing `iscasmodel-0.8.tar` & `iscasmodel-0.9.tar`

### file list

```diff
@@ -1,14 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-12-25 05:38:13.948212 iscasmodel-0.8/
--rw-rw-rw-   0        0        0      241 2023-12-25 05:38:13.947212 iscasmodel-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-25 05:38:13.931208 iscasmodel-0.8/iscasmodel/
--rw-rw-rw-   0        0        0        0 2023-08-28 02:51:49.000000 iscasmodel-0.8/iscasmodel/__init__.py
--rw-rw-rw-   0        0        0     4208 2023-12-25 03:17:24.000000 iscasmodel-0.8/iscasmodel/core.py
--rw-rw-rw-   0        0        0     1308 2023-11-27 03:04:18.000000 iscasmodel-0.8/iscasmodel/feng.py
-drwxrwxrwx   0        0        0        0 2023-12-25 05:38:13.944213 iscasmodel-0.8/iscasmodel.egg-info/
--rw-rw-rw-   0        0        0      241 2023-12-25 05:38:13.000000 iscasmodel-0.8/iscasmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-12-25 05:38:13.000000 iscasmodel-0.8/iscasmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-25 05:38:13.000000 iscasmodel-0.8/iscasmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-12-25 05:38:13.000000 iscasmodel-0.8/iscasmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-12-25 05:38:13.000000 iscasmodel-0.8/iscasmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-25 05:38:13.948212 iscasmodel-0.8/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-12-25 05:37:16.000000 iscasmodel-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.297364 iscasmodel-0.9/
+-rw-rw-rw-   0        0        0      241 2023-12-26 07:19:02.296366 iscasmodel-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.104368 iscasmodel-0.9/iscasmodel/
+-rw-rw-rw-   0        0        0        0 2023-08-28 02:51:49.000000 iscasmodel-0.9/iscasmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.153365 iscasmodel-0.9/iscasmodel/accelerate/
+-rw-rw-rw-   0        0        0      789 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/__init__.py
+-rw-rw-rw-   0        0        0   139296 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/accelerator.py
+-rw-rw-rw-   0        0        0    26145 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/big_modeling.py
+-rw-rw-rw-   0        0        0    11372 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/checkpointing.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.171364 iscasmodel-0.9/iscasmodel/accelerate/commands/
+-rw-rw-rw-   0        0        0        0 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/accelerate_cli.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.191367 iscasmodel-0.9/iscasmodel/accelerate/commands/config/
+-rw-rw-rw-   0        0        0     1645 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/__init__.py
+-rw-rw-rw-   0        0        0    28020 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/cluster.py
+-rw-rw-rw-   0        0        0     3035 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/config.py
+-rw-rw-rw-   0        0        0     9633 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/config_args.py
+-rw-rw-rw-   0        0        0     2913 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/config_utils.py
+-rw-rw-rw-   0        0        0     5044 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/default.py
+-rw-rw-rw-   0        0        0    10341 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/sagemaker.py
+-rw-rw-rw-   0        0        0     2395 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/config/update.py
+-rw-rw-rw-   0        0        0     3056 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/env.py
+-rw-rw-rw-   0        0        0    10429 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/estimate.py
+-rw-rw-rw-   0        0        0    39729 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/launch.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.205367 iscasmodel-0.9/iscasmodel/accelerate/commands/menu/
+-rw-rw-rw-   0        0        0       39 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/menu/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/menu/cursor.py
+-rw-rw-rw-   0        0        0     1483 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/menu/helpers.py
+-rw-rw-rw-   0        0        0     2581 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/menu/input.py
+-rw-rw-rw-   0        0        0     4087 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/menu/keymap.py
+-rw-rw-rw-   0        0        0     4920 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/menu/selection_menu.py
+-rw-rw-rw-   0        0        0     2179 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/test.py
+-rw-rw-rw-   0        0        0     5553 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/commands/tpu.py
+-rw-rw-rw-   0        0        0    45754 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/data_loader.py
+-rw-rw-rw-   0        0        0    25320 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/hooks.py
+-rw-rw-rw-   0        0        0    11331 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/launchers.py
+-rw-rw-rw-   0        0        0     3924 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/local_sgd.py
+-rw-rw-rw-   0        0        0     4897 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/logging.py
+-rw-rw-rw-   0        0        0      862 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/memory_utils.py
+-rw-rw-rw-   0        0        0     7205 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/optimizer.py
+-rw-rw-rw-   0        0        0     4238 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/scheduler.py
+-rw-rw-rw-   0        0        0    46592 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/state.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.214366 iscasmodel-0.9/iscasmodel/accelerate/test_utils/
+-rw-rw-rw-   0        0        0      641 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/__init__.py
+-rw-rw-rw-   0        0        0     7301 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/examples.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.230365 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/
+-rw-rw-rw-   0        0        0        0 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.243368 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/external_deps/
+-rw-rw-rw-   0        0        0        0 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/external_deps/__init__.py
+-rw-rw-rw-   0        0        0    10686 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/external_deps/test_checkpointing.py
+-rw-rw-rw-   0        0        0    10981 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/external_deps/test_metrics.py
+-rw-rw-rw-   0        0        0    10725 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/external_deps/test_peak_memory_usage.py
+-rw-rw-rw-   0        0        0     9093 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/external_deps/test_performance.py
+-rw-rw-rw-   0        0        0      227 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/test_cli.py
+-rw-rw-rw-   0        0        0     8236 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/test_distributed_data_loop.py
+-rw-rw-rw-   0        0        0     1016 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/test_notebook.py
+-rw-rw-rw-   0        0        0     5263 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/test_ops.py
+-rw-rw-rw-   0        0        0    26246 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/test_script.py
+-rw-rw-rw-   0        0        0    17147 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/scripts/test_sync.py
+-rw-rw-rw-   0        0        0    17472 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/testing.py
+-rw-rw-rw-   0        0        0     4019 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/test_utils/training.py
+-rw-rw-rw-   0        0        0    39526 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/tracking.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.294370 iscasmodel-0.9/iscasmodel/accelerate/utils/
+-rw-rw-rw-   0        0        0     5094 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/__init__.py
+-rw-rw-rw-   0        0        0    20570 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/bnb.py
+-rw-rw-rw-   0        0        0     2553 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/constants.py
+-rw-rw-rw-   0        0        0    68604 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/dataclasses.py
+-rw-rw-rw-   0        0        0    10208 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/deepspeed.py
+-rw-rw-rw-   0        0        0     4062 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/environment.py
+-rw-rw-rw-   0        0        0     9825 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/fsdp_utils.py
+-rw-rw-rw-   0        0        0     9841 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/imports.py
+-rw-rw-rw-   0        0        0    25032 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/launch.py
+-rw-rw-rw-   0        0        0    57263 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/megatron_lm.py
+-rw-rw-rw-   0        0        0     4880 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/memory.py
+-rw-rw-rw-   0        0        0    71095 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/modeling.py
+-rw-rw-rw-   0        0        0     7842 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/offload.py
+-rw-rw-rw-   0        0        0    25298 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/operations.py
+-rw-rw-rw-   0        0        0    10403 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/other.py
+-rw-rw-rw-   0        0        0     4292 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/random.py
+-rw-rw-rw-   0        0        0      847 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/rich.py
+-rw-rw-rw-   0        0        0     1908 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/torch_xla.py
+-rw-rw-rw-   0        0        0     1344 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/tqdm.py
+-rw-rw-rw-   0        0        0     3561 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/transformer_engine.py
+-rw-rw-rw-   0        0        0     2149 2023-12-22 19:10:22.000000 iscasmodel-0.9/iscasmodel/accelerate/utils/versions.py
+-rw-rw-rw-   0        0        0     4193 2023-12-26 07:16:45.000000 iscasmodel-0.9/iscasmodel/core.py
+-rw-rw-rw-   0        0        0     1308 2023-11-27 03:04:18.000000 iscasmodel-0.9/iscasmodel/feng.py
+drwxrwxrwx   0        0        0        0 2023-12-26 07:19:02.116368 iscasmodel-0.9/iscasmodel.egg-info/
+-rw-rw-rw-   0        0        0      241 2023-12-26 07:19:01.000000 iscasmodel-0.9/iscasmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3499 2023-12-26 07:19:01.000000 iscasmodel-0.9/iscasmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-26 07:19:01.000000 iscasmodel-0.9/iscasmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-12-26 07:19:01.000000 iscasmodel-0.9/iscasmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-12-26 07:19:01.000000 iscasmodel-0.9/iscasmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-26 07:19:02.297364 iscasmodel-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-12-26 07:18:55.000000 iscasmodel-0.9/setup.py
```

### Comparing `iscasmodel-0.8/iscasmodel/core.py` & `iscasmodel-0.9/iscasmodel/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 import urllib.request
 import urllib.parse
 import zipfile
-from accelerate.utils import calculate_maximum_sizes, convert_bytes
+from accelerate.utils import calculate_maximum_sizes
 
 
 class ModelUtils:
 
     def __init__(self):
         self.svc_ip = os.getenv("svc_ip")
         self.model_id = os.getenv("model_id")
```

### Comparing `iscasmodel-0.8/iscasmodel/feng.py` & `iscasmodel-0.9/iscasmodel/feng.py`

 * *Files identical despite different names*

