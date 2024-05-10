# Comparing `tmp/InternEvo-0.4.8.tar.gz` & `tmp/InternEvo-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternEvo-0.4.8.tar", last modified: Thu May  9 03:26:09 2024, max compression
+gzip compressed data, was "InternEvo-0.4.9.tar", last modified: Thu May  9 12:03:02 2024, max compression
```

## Comparing `InternEvo-0.4.8.tar` & `InternEvo-0.4.9.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:11.413163 InternEvo-0.4.8/
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.576333 InternEvo-0.4.8/InternEvo.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-09 03:26:05.000000 InternEvo-0.4.8/InternEvo.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4662 2024-05-09 03:26:06.000000 InternEvo-0.4.8/InternEvo.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-09 03:26:05.000000 InternEvo-0.4.8/InternEvo.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       20 2024-05-09 03:26:05.000000 InternEvo-0.4.8/InternEvo.egg-info/requires.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-09 03:26:05.000000 InternEvo-0.4.8/InternEvo.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.4.8/LICENSE
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-09 03:26:09.612060 InternEvo-0.4.8/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.4.8/README.md
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.581862 InternEvo-0.4.8/internlm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.4.8/internlm/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.615431 InternEvo-0.4.8/internlm/accelerator/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/accelerator/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/accelerator/abstract_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/accelerator/cuda_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/accelerator/dipu_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/accelerator/npu_accelerator.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.629724 InternEvo-0.4.8/internlm/apis/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.8/internlm/apis/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.4.8/internlm/apis/inference.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.667440 InternEvo-0.4.8/internlm/checkpoint/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/checkpoint/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.4.8/internlm/checkpoint/checkpoint_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.4.8/internlm/checkpoint/components.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14174 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/checkpoint/load_funcs.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.4.8/internlm/checkpoint/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.700915 InternEvo-0.4.8/internlm/core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.4.8/internlm/core/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.730519 InternEvo-0.4.8/internlm/core/communication/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/core/communication/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23944 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/core/communication/isp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/core/communication/p2p.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10118 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/core/communication/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.759922 InternEvo-0.4.8/internlm/core/context/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.4.8/internlm/core/context/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/core/context/parallel_context.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.4.8/internlm/core/context/process_group_initializer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/core/context/random.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/core/engine.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/core/gradient_handler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8195 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/core/naive_amp.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.786398 InternEvo-0.4.8/internlm/core/scheduler/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.4.8/internlm/core/scheduler/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.4.8/internlm/core/scheduler/base_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9071 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/core/scheduler/no_pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    64105 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/core/scheduler/pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:42.000000 InternEvo-0.4.8/internlm/core/trainer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:09.812464 InternEvo-0.4.8/internlm/data/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/data/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:14:24.000000 InternEvo-0.4.8/internlm/data/build_dataloader.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.542977 InternEvo-0.4.8/internlm/data/tokenized/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.4.8/internlm/data/tokenized/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/data/tokenized/batch_sampler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.4.8/internlm/data/tokenized/collaters.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/data/tokenized/dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/data/tokenized/dummy_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.4.8/internlm/data/tokenized/dummy_dataset_multimodal.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.4.8/internlm/data/tokenized/packed_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/data/tokenized/single_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/data/train_state.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1919 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/data/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.560161 InternEvo-0.4.8/internlm/eval/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/eval/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.4.8/internlm/eval/evaluation.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.587671 InternEvo-0.4.8/internlm/initialize/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.4.8/internlm/initialize/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.4.8/internlm/initialize/initialize_tensor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5922 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/initialize/initialize_trainer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27458 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/initialize/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.600665 InternEvo-0.4.8/internlm/initialize/legacy/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.8/internlm/initialize/legacy/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/initialize/legacy/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.651299 InternEvo-0.4.8/internlm/model/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1124 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.677678 InternEvo-0.4.8/internlm/model/llava_modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-03 18:56:44.000000 InternEvo-0.4.8/internlm/model/llava_modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/llava_modules/clip_builder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/llava_modules/clip_encoder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/llava_modules/projector_builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.696737 InternEvo-0.4.8/internlm/model/losses/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.4.8/internlm/model/losses/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1786 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/losses/ce_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16344 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/metrics.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23422 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modeling_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54060 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modeling_internlm2.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    51790 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modeling_llama.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20872 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modeling_llava.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25417 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modeling_moe.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.725123 InternEvo-0.4.8/internlm/model/modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.8/internlm/model/modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20370 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modules/embedding.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10093 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modules/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    40600 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/modules/multi_head_attention.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.761768 InternEvo-0.4.8/internlm/model/moe/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      678 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/moe/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/model/moe/base_layer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.4.8/internlm/model/moe/experts.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20490 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/moe/gshard_layer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.794374 InternEvo-0.4.8/internlm/model/moe/megablock/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.4.8/internlm/model/moe/megablock/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8705 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/moe/megablock/megablock_dmoe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13643 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/moe/megablock/megablock_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2555 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/moe/megablock/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11986 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/moe/megablock/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4494 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/moe/moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.4.8/internlm/model/moe/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.819604 InternEvo-0.4.8/internlm/model/ops/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.8/internlm/model/ops/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6316 2024-05-06 07:30:03.000000 InternEvo-0.4.8/internlm/model/ops/fusion_ops_import_helper.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16010 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/ops/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/model/ops/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24931 2024-05-06 07:30:03.000000 InternEvo-0.4.8/internlm/model/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.846349 InternEvo-0.4.8/internlm/monitor/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/monitor/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/monitor/alert.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/monitor/monitor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/monitor/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.877966 InternEvo-0.4.8/internlm/solver/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.4.8/internlm/solver/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/solver/activation_checkpoint.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.918987 InternEvo-0.4.8/internlm/solver/optimizer/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.4.8/internlm/solver/optimizer/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.4.8/internlm/solver/optimizer/base_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.4.8/internlm/solver/optimizer/fsdp_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42555 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/solver/optimizer/hybrid_zero_optim.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.4.8/internlm/solver/optimizer/store.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.4.8/internlm/solver/optimizer/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/solver/pipeline_utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:10.938845 InternEvo-0.4.8/internlm/solver/schedulers/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.4.8/internlm/solver/schedulers/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.4.8/internlm/solver/schedulers/beta2_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.4.8/internlm/solver/schedulers/lr_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:11.220356 InternEvo-0.4.8/internlm/train/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      591 2024-05-06 07:30:03.000000 InternEvo-0.4.8/internlm/train/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22392 2024-05-06 07:30:03.000000 InternEvo-0.4.8/internlm/train/pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3567 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/train/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:11.302454 InternEvo-0.4.8/internlm/utils/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.8/internlm/utils/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9244 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/utils/common.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/utils/gputest.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.4.8/internlm/utils/logger.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/utils/megatron_timers.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4061 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/utils/parallel.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/utils/registry.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.4.8/internlm/utils/simple_memory_profiler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/utils/storage_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.4.8/internlm/utils/timeout.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-05-03 18:58:40.000000 InternEvo-0.4.8/internlm/utils/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.4.8/internlm/utils/writer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-09 03:26:09.615525 InternEvo-0.4.8/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1186 2024-05-09 02:41:29.000000 InternEvo-0.4.8/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:11.313301 InternEvo-0.4.8/tests/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.8/tests/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4536 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/common_fixture.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:11.333586 InternEvo-0.4.8/tests/test_core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.8/tests/test_core/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-24 06:39:45.000000 InternEvo-0.4.8/tests/test_core/test_pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6978 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_core/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 03:24:11.403393 InternEvo-0.4.8/tests/test_training/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.4.8/tests/test_training/7B_check_acc.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.4.8/tests/test_training/7B_check_init.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.4.8/tests/test_training/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7882 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_training/test_forward_output_no_fa.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11700 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_training/test_load_ckpt_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14416 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_training/test_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3845 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_training/test_no_fa_train_temp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6763 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_training/test_norm_weight.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12557 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_training/test_swap_nb_loss_and_gradnorm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14000 2024-05-03 18:58:40.000000 InternEvo-0.4.8/tests/test_training/train_CI.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.444968 InternEvo-0.4.9/
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.355947 InternEvo-0.4.9/InternEvo.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-09 12:03:00.000000 InternEvo-0.4.9/InternEvo.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4662 2024-05-09 12:03:01.000000 InternEvo-0.4.9/InternEvo.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-09 12:03:00.000000 InternEvo-0.4.9/InternEvo.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       20 2024-05-09 12:03:00.000000 InternEvo-0.4.9/InternEvo.egg-info/requires.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-09 12:03:00.000000 InternEvo-0.4.9/InternEvo.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.4.9/LICENSE
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-09 12:03:02.808904 InternEvo-0.4.9/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.4.9/README.md
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.362618 InternEvo-0.4.9/internlm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.4.9/internlm/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.409072 InternEvo-0.4.9/internlm/accelerator/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/accelerator/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/accelerator/abstract_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/accelerator/cuda_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/accelerator/dipu_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/accelerator/npu_accelerator.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.429494 InternEvo-0.4.9/internlm/apis/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.9/internlm/apis/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.4.9/internlm/apis/inference.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.478808 InternEvo-0.4.9/internlm/checkpoint/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/checkpoint/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.4.9/internlm/checkpoint/checkpoint_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.4.9/internlm/checkpoint/components.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14174 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/checkpoint/load_funcs.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.4.9/internlm/checkpoint/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.524816 InternEvo-0.4.9/internlm/core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.4.9/internlm/core/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.568193 InternEvo-0.4.9/internlm/core/communication/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/core/communication/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23944 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/core/communication/isp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/core/communication/p2p.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10118 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/core/communication/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.605727 InternEvo-0.4.9/internlm/core/context/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.4.9/internlm/core/context/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/core/context/parallel_context.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.4.9/internlm/core/context/process_group_initializer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/core/context/random.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/core/engine.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/core/gradient_handler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8195 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/core/naive_amp.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.646858 InternEvo-0.4.9/internlm/core/scheduler/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.4.9/internlm/core/scheduler/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.4.9/internlm/core/scheduler/base_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9071 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/core/scheduler/no_pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    64105 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/core/scheduler/pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:42.000000 InternEvo-0.4.9/internlm/core/trainer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.679771 InternEvo-0.4.9/internlm/data/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/data/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:14:24.000000 InternEvo-0.4.9/internlm/data/build_dataloader.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.745284 InternEvo-0.4.9/internlm/data/tokenized/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.4.9/internlm/data/tokenized/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/data/tokenized/batch_sampler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.4.9/internlm/data/tokenized/collaters.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/data/tokenized/dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/data/tokenized/dummy_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.4.9/internlm/data/tokenized/dummy_dataset_multimodal.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.4.9/internlm/data/tokenized/packed_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/data/tokenized/single_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/data/train_state.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1919 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/data/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.764907 InternEvo-0.4.9/internlm/eval/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/eval/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.4.9/internlm/eval/evaluation.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.800949 InternEvo-0.4.9/internlm/initialize/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.4.9/internlm/initialize/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.4.9/internlm/initialize/initialize_tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5922 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/initialize/initialize_trainer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27458 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/initialize/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.816923 InternEvo-0.4.9/internlm/initialize/legacy/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.9/internlm/initialize/legacy/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/initialize/legacy/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.877118 InternEvo-0.4.9/internlm/model/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1124 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.905351 InternEvo-0.4.9/internlm/model/llava_modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-03 18:56:44.000000 InternEvo-0.4.9/internlm/model/llava_modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/llava_modules/clip_builder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/llava_modules/clip_encoder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/llava_modules/projector_builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.922374 InternEvo-0.4.9/internlm/model/losses/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.4.9/internlm/model/losses/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1786 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/losses/ce_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16344 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/metrics.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23422 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modeling_internlm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54060 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modeling_internlm2.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    51790 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modeling_llama.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20872 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modeling_llava.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25417 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modeling_moe.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:03.953428 InternEvo-0.4.9/internlm/model/modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.9/internlm/model/modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20370 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modules/embedding.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10093 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modules/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    40600 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/modules/multi_head_attention.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.000619 InternEvo-0.4.9/internlm/model/moe/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      678 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/moe/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/model/moe/base_layer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.4.9/internlm/model/moe/experts.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20490 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/moe/gshard_layer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.042899 InternEvo-0.4.9/internlm/model/moe/megablock/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.4.9/internlm/model/moe/megablock/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8705 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/moe/megablock/megablock_dmoe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13643 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/moe/megablock/megablock_moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2555 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/moe/megablock/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11986 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/moe/megablock/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4494 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/moe/moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.4.9/internlm/model/moe/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.077510 InternEvo-0.4.9/internlm/model/ops/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.9/internlm/model/ops/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6316 2024-05-06 07:30:03.000000 InternEvo-0.4.9/internlm/model/ops/fusion_ops_import_helper.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16010 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/ops/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/model/ops/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24931 2024-05-06 07:30:03.000000 InternEvo-0.4.9/internlm/model/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.109845 InternEvo-0.4.9/internlm/monitor/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/monitor/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/monitor/alert.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/monitor/monitor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/monitor/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.132033 InternEvo-0.4.9/internlm/solver/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.4.9/internlm/solver/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/solver/activation_checkpoint.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.181855 InternEvo-0.4.9/internlm/solver/optimizer/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.4.9/internlm/solver/optimizer/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.4.9/internlm/solver/optimizer/base_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.4.9/internlm/solver/optimizer/fsdp_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42555 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/solver/optimizer/hybrid_zero_optim.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.4.9/internlm/solver/optimizer/store.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.4.9/internlm/solver/optimizer/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/solver/pipeline_utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.206338 InternEvo-0.4.9/internlm/solver/schedulers/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.4.9/internlm/solver/schedulers/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.4.9/internlm/solver/schedulers/beta2_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.4.9/internlm/solver/schedulers/lr_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.230471 InternEvo-0.4.9/internlm/train/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      591 2024-05-06 07:30:03.000000 InternEvo-0.4.9/internlm/train/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22392 2024-05-06 07:30:03.000000 InternEvo-0.4.9/internlm/train/pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3567 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/train/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.326968 InternEvo-0.4.9/internlm/utils/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.9/internlm/utils/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9244 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/utils/common.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/utils/gputest.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.4.9/internlm/utils/logger.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/utils/megatron_timers.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4061 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/utils/parallel.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/utils/registry.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.4.9/internlm/utils/simple_memory_profiler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/utils/storage_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.4.9/internlm/utils/timeout.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-05-03 18:58:40.000000 InternEvo-0.4.9/internlm/utils/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.4.9/internlm/utils/writer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-09 12:03:02.812327 InternEvo-0.4.9/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1157 2024-05-09 04:27:32.000000 InternEvo-0.4.9/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.339535 InternEvo-0.4.9/tests/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.9/tests/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4536 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/common_fixture.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.360859 InternEvo-0.4.9/tests/test_core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.9/tests/test_core/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-24 06:39:45.000000 InternEvo-0.4.9/tests/test_core/test_pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6978 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_core/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-09 12:01:04.435241 InternEvo-0.4.9/tests/test_training/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.4.9/tests/test_training/7B_check_acc.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.4.9/tests/test_training/7B_check_init.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.4.9/tests/test_training/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7882 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_training/test_forward_output_no_fa.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11700 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_training/test_load_ckpt_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14416 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_training/test_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3845 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_training/test_no_fa_train_temp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6763 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_training/test_norm_weight.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12557 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_training/test_swap_nb_loss_and_gradnorm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14000 2024-05-03 18:58:40.000000 InternEvo-0.4.9/tests/test_training/train_CI.py
```

### Comparing `InternEvo-0.4.8/InternEvo.egg-info/PKG-INFO` & `InternEvo-0.4.9/InternEvo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.4.8
+Version: 0.4.9
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.4.8 Summary: an open-sourced
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.9 Summary: an open-sourced
 lightweight training framework aims to support model pre-training without the
 need for extensive dependencies Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Description-
 Content-Type: text/markdown License-File: LICENSE # InternEvo
```

### Comparing `InternEvo-0.4.8/InternEvo.egg-info/SOURCES.txt` & `InternEvo-0.4.9/InternEvo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/LICENSE` & `InternEvo-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/PKG-INFO` & `InternEvo-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.4.8
+Version: 0.4.9
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.4.8 Summary: an open-sourced
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.9 Summary: an open-sourced
 lightweight training framework aims to support model pre-training without the
 need for extensive dependencies Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Description-
 Content-Type: text/markdown License-File: LICENSE # InternEvo
```

### Comparing `InternEvo-0.4.8/README.md` & `InternEvo-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/accelerator/abstract_accelerator.py` & `InternEvo-0.4.9/internlm/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/accelerator/cuda_accelerator.py` & `InternEvo-0.4.9/internlm/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/accelerator/dipu_accelerator.py` & `InternEvo-0.4.9/internlm/accelerator/dipu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/accelerator/npu_accelerator.py` & `InternEvo-0.4.9/internlm/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/apis/inference.py` & `InternEvo-0.4.9/internlm/apis/inference.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/checkpoint/checkpoint_manager.py` & `InternEvo-0.4.9/internlm/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/checkpoint/components.py` & `InternEvo-0.4.9/internlm/checkpoint/components.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/checkpoint/load_funcs.py` & `InternEvo-0.4.9/internlm/checkpoint/load_funcs.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/checkpoint/utils.py` & `InternEvo-0.4.9/internlm/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/communication/__init__.py` & `InternEvo-0.4.9/internlm/core/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/communication/isp.py` & `InternEvo-0.4.9/internlm/core/communication/isp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/communication/p2p.py` & `InternEvo-0.4.9/internlm/core/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/communication/utils.py` & `InternEvo-0.4.9/internlm/core/communication/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/context/__init__.py` & `InternEvo-0.4.9/internlm/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/context/parallel_context.py` & `InternEvo-0.4.9/internlm/core/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/context/process_group_initializer.py` & `InternEvo-0.4.9/internlm/core/context/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/context/random.py` & `InternEvo-0.4.9/internlm/core/context/random.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/engine.py` & `InternEvo-0.4.9/internlm/core/engine.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/gradient_handler.py` & `InternEvo-0.4.9/internlm/core/gradient_handler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/naive_amp.py` & `InternEvo-0.4.9/internlm/core/naive_amp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/scheduler/base_scheduler.py` & `InternEvo-0.4.9/internlm/core/scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/scheduler/no_pipeline_scheduler.py` & `InternEvo-0.4.9/internlm/core/scheduler/no_pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/scheduler/pipeline_scheduler.py` & `InternEvo-0.4.9/internlm/core/scheduler/pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/core/trainer.py` & `InternEvo-0.4.9/internlm/core/trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/build_dataloader.py` & `InternEvo-0.4.9/internlm/data/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/tokenized/batch_sampler.py` & `InternEvo-0.4.9/internlm/data/tokenized/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/tokenized/collaters.py` & `InternEvo-0.4.9/internlm/data/tokenized/collaters.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/tokenized/dataset.py` & `InternEvo-0.4.9/internlm/data/tokenized/dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/tokenized/dummy_dataset.py` & `InternEvo-0.4.9/internlm/data/tokenized/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/tokenized/dummy_dataset_multimodal.py` & `InternEvo-0.4.9/internlm/data/tokenized/dummy_dataset_multimodal.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/tokenized/packed_dataset.py` & `InternEvo-0.4.9/internlm/data/tokenized/packed_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/tokenized/single_dataset.py` & `InternEvo-0.4.9/internlm/data/tokenized/single_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/data/utils.py` & `InternEvo-0.4.9/internlm/data/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/eval/evaluation.py` & `InternEvo-0.4.9/internlm/eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/initialize/initialize_tensor.py` & `InternEvo-0.4.9/internlm/initialize/initialize_tensor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/initialize/initialize_trainer.py` & `InternEvo-0.4.9/internlm/initialize/initialize_trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/initialize/launch.py` & `InternEvo-0.4.9/internlm/initialize/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/initialize/legacy/launch.py` & `InternEvo-0.4.9/internlm/initialize/legacy/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/__init__.py` & `InternEvo-0.4.9/internlm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/llava_modules/clip_encoder.py` & `InternEvo-0.4.9/internlm/model/llava_modules/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/llava_modules/projector_builder.py` & `InternEvo-0.4.9/internlm/model/llava_modules/projector_builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/losses/ce_loss.py` & `InternEvo-0.4.9/internlm/model/losses/ce_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/metrics.py` & `InternEvo-0.4.9/internlm/model/metrics.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modeling_internlm.py` & `InternEvo-0.4.9/internlm/model/modeling_internlm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modeling_internlm2.py` & `InternEvo-0.4.9/internlm/model/modeling_internlm2.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modeling_llama.py` & `InternEvo-0.4.9/internlm/model/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modeling_llava.py` & `InternEvo-0.4.9/internlm/model/modeling_llava.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modeling_moe.py` & `InternEvo-0.4.9/internlm/model/modeling_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modules/embedding.py` & `InternEvo-0.4.9/internlm/model/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modules/mlp.py` & `InternEvo-0.4.9/internlm/model/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/modules/multi_head_attention.py` & `InternEvo-0.4.9/internlm/model/modules/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/__init__.py` & `InternEvo-0.4.9/internlm/model/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/base_layer.py` & `InternEvo-0.4.9/internlm/model/moe/base_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/experts.py` & `InternEvo-0.4.9/internlm/model/moe/experts.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/gshard_layer.py` & `InternEvo-0.4.9/internlm/model/moe/gshard_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/megablock/megablock_dmoe.py` & `InternEvo-0.4.9/internlm/model/moe/megablock/megablock_dmoe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/megablock/megablock_moe.py` & `InternEvo-0.4.9/internlm/model/moe/megablock/megablock_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/megablock/mlp.py` & `InternEvo-0.4.9/internlm/model/moe/megablock/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/megablock/utils.py` & `InternEvo-0.4.9/internlm/model/moe/megablock/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/moe.py` & `InternEvo-0.4.9/internlm/model/moe/moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/moe/utils.py` & `InternEvo-0.4.9/internlm/model/moe/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/ops/fusion_ops_import_helper.py` & `InternEvo-0.4.9/internlm/model/ops/fusion_ops_import_helper.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/ops/linear.py` & `InternEvo-0.4.9/internlm/model/ops/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/ops/norm.py` & `InternEvo-0.4.9/internlm/model/ops/norm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/model/utils.py` & `InternEvo-0.4.9/internlm/model/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/monitor/alert.py` & `InternEvo-0.4.9/internlm/monitor/alert.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/monitor/monitor.py` & `InternEvo-0.4.9/internlm/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/monitor/utils.py` & `InternEvo-0.4.9/internlm/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/activation_checkpoint.py` & `InternEvo-0.4.9/internlm/solver/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/optimizer/base_optimizer.py` & `InternEvo-0.4.9/internlm/solver/optimizer/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/optimizer/fsdp_optimizer.py` & `InternEvo-0.4.9/internlm/solver/optimizer/fsdp_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/optimizer/hybrid_zero_optim.py` & `InternEvo-0.4.9/internlm/solver/optimizer/hybrid_zero_optim.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/optimizer/store.py` & `InternEvo-0.4.9/internlm/solver/optimizer/store.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/optimizer/utils.py` & `InternEvo-0.4.9/internlm/solver/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/pipeline_utils.py` & `InternEvo-0.4.9/internlm/solver/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/schedulers/beta2_scheduler.py` & `InternEvo-0.4.9/internlm/solver/schedulers/beta2_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/solver/schedulers/lr_scheduler.py` & `InternEvo-0.4.9/internlm/solver/schedulers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/train/__init__.py` & `InternEvo-0.4.9/internlm/train/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/train/pipeline.py` & `InternEvo-0.4.9/internlm/train/pipeline.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/train/utils.py` & `InternEvo-0.4.9/internlm/train/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/common.py` & `InternEvo-0.4.9/internlm/utils/common.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/gputest.py` & `InternEvo-0.4.9/internlm/utils/gputest.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/logger.py` & `InternEvo-0.4.9/internlm/utils/logger.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/megatron_timers.py` & `InternEvo-0.4.9/internlm/utils/megatron_timers.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/parallel.py` & `InternEvo-0.4.9/internlm/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/registry.py` & `InternEvo-0.4.9/internlm/utils/registry.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/simple_memory_profiler.py` & `InternEvo-0.4.9/internlm/utils/simple_memory_profiler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/storage_manager.py` & `InternEvo-0.4.9/internlm/utils/storage_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/timeout.py` & `InternEvo-0.4.9/internlm/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/utils.py` & `InternEvo-0.4.9/internlm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/internlm/utils/writer.py` & `InternEvo-0.4.9/internlm/utils/writer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/setup.py` & `InternEvo-0.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,17 @@
     return content
 
 def get_version():
     with open(os.path.join(pwd, 'version.txt'), 'r') as f:
         content = f.read()
     return content
 
-proj_version = get_version()
-
 setup(
     name='InternEvo',
-    version=proj_version,
+    version=get_version(),
     description='an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'rotary_emb',
         'xentropy',
```

### Comparing `InternEvo-0.4.8/tests/common_fixture.py` & `InternEvo-0.4.9/tests/common_fixture.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_core/test_pipeline.py` & `InternEvo-0.4.9/tests/test_core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_core/utils.py` & `InternEvo-0.4.9/tests/test_core/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/7B_check_acc.py` & `InternEvo-0.4.9/tests/test_training/7B_check_acc.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/7B_check_init.py` & `InternEvo-0.4.9/tests/test_training/7B_check_init.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/test_forward_output_no_fa.py` & `InternEvo-0.4.9/tests/test_training/test_forward_output_no_fa.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/test_load_ckpt_loss.py` & `InternEvo-0.4.9/tests/test_training/test_load_ckpt_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/test_loss.py` & `InternEvo-0.4.9/tests/test_training/test_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/test_no_fa_train_temp.py` & `InternEvo-0.4.9/tests/test_training/test_no_fa_train_temp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/test_norm_weight.py` & `InternEvo-0.4.9/tests/test_training/test_norm_weight.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/test_swap_nb_loss_and_gradnorm.py` & `InternEvo-0.4.9/tests/test_training/test_swap_nb_loss_and_gradnorm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.8/tests/test_training/train_CI.py` & `InternEvo-0.4.9/tests/test_training/train_CI.py`

 * *Files identical despite different names*

