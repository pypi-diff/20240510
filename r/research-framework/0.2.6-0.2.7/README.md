# Comparing `tmp/research_framework-0.2.6.tar.gz` & `tmp/research_framework-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research_framework-0.2.6.tar", last modified: Wed May  8 00:38:00 2024, max compression
+gzip compressed data, was "research_framework-0.2.7.tar", last modified: Fri May 10 17:14:00 2024, max compression
```

## Comparing `research_framework-0.2.6.tar` & `research_framework-0.2.7.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    35149 2023-09-01 08:34:48.000000 research_framework-0.2.6/LICENSE
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       24 2023-09-01 08:34:48.000000 research_framework-0.2.6/MANIFEST.in
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-05-08 00:38:00.187687 research_framework-0.2.6/PKG-INFO
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      393 2024-05-01 13:22:11.000000 research_framework-0.2.6/requirements.txt
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.179686 research_framework-0.2.6/research_framework/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       91 2023-11-07 13:43:38.000000 research_framework-0.2.6/research_framework/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.179686 research_framework-0.2.6/research_framework/base/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/base/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/container/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/base/container/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1990 2023-11-09 16:51:42.000000 research_framework-0.2.6/research_framework/base/container/base_container.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/container/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.6/research_framework/base/container/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      722 2023-09-19 17:54:13.000000 research_framework-0.2.6/research_framework/base/container/model/bind_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/flyweight/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.6/research_framework/base/flyweight/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1074 2023-11-08 13:26:10.000000 research_framework-0.2.6/research_framework/base/flyweight/base_flyweight.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      800 2024-04-25 16:51:06.000000 research_framework-0.2.6/research_framework/base/flyweight/base_flyweight_manager.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/base/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2550 2024-03-02 14:06:30.000000 research_framework-0.2.6/research_framework/base/model/base_dao.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      567 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/base/model/base_utils.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/pipeline/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-06 20:33:03.000000 research_framework-0.2.6/research_framework/base/pipeline/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      227 2023-12-29 14:25:32.000000 research_framework-0.2.6/research_framework/base/pipeline/base_pipeline.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/plugin/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/base/plugin/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1029 2023-10-15 10:47:16.000000 research_framework-0.2.6/research_framework/base/plugin/base_plugin.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      337 2024-04-25 10:02:49.000000 research_framework-0.2.6/research_framework/base/plugin/base_wrapper.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/singleton/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:03:32.000000 research_framework-0.2.6/research_framework/base/singleton/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      262 2024-04-25 16:34:16.000000 research_framework-0.2.6/research_framework/base/singleton/base_singleton.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/storage/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/base/storage/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      545 2024-04-25 16:34:46.000000 research_framework-0.2.6/research_framework/base/storage/base_storage.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/base/utils/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-21 13:26:13.000000 research_framework-0.2.6/research_framework/base/utils/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1503 2024-05-01 17:24:30.000000 research_framework-0.2.6/research_framework/base/utils/grid_seach.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      308 2023-09-19 18:09:27.000000 research_framework-0.2.6/research_framework/base/utils/method_overload.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/container/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.6/research_framework/container/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5265 2024-05-01 16:40:16.000000 research_framework-0.2.6/research_framework/container/container.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/container/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-17 21:22:31.000000 research_framework-0.2.6/research_framework/container/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      505 2024-05-01 12:33:48.000000 research_framework-0.2.6/research_framework/container/model/global_config.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/dataset/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:07:36.000000 research_framework-0.2.6/research_framework/dataset/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      872 2023-09-20 22:03:33.000000 research_framework-0.2.6/research_framework/dataset/basic_dataset.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1071 2023-11-07 10:26:41.000000 research_framework-0.2.6/research_framework/dataset/standard_dataset.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/flyweight/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/flyweight/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8026 2024-04-24 16:58:20.000000 research_framework-0.2.6/research_framework/flyweight/flyweight.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    14387 2024-04-25 17:28:03.000000 research_framework-0.2.6/research_framework/flyweight/flyweight_manager.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3638 2024-05-07 18:36:36.000000 research_framework-0.2.6/research_framework/flyweight/mem_manager.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/flyweight/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/flyweight/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1011 2023-09-06 13:45:32.000000 research_framework-0.2.6/research_framework/flyweight/model/item_dao.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      659 2023-11-08 13:27:58.000000 research_framework-0.2.6/research_framework/flyweight/model/item_model.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      497 2024-04-10 01:30:54.000000 research_framework-0.2.6/research_framework/flyweight/model/item_simple_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/neural_models/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:13:05.000000 research_framework-0.2.6/research_framework/neural_models/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      379 2023-09-13 12:58:06.000000 research_framework-0.2.6/research_framework/neural_models/doomy_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/pipeline/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       48 2023-11-07 13:43:32.000000 research_framework-0.2.6/research_framework/pipeline/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/pipeline/exceptions/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 13:09:29.000000 research_framework-0.2.6/research_framework/pipeline/exceptions/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       54 2024-05-01 13:11:12.000000 research_framework-0.2.6/research_framework/pipeline/exceptions/pipeline_exceptions.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       49 2024-05-01 13:11:19.000000 research_framework-0.2.6/research_framework/pipeline/exceptions/run_exceptions.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      491 2023-09-06 13:45:32.000000 research_framework-0.2.6/research_framework/pipeline/inputs.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.183687 research_framework-0.2.6/research_framework/pipeline/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/research_framework/pipeline/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3293 2024-05-05 09:01:39.000000 research_framework-0.2.6/research_framework/pipeline/model/pipeline_model.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    10055 2024-05-05 08:57:44.000000 research_framework-0.2.6/research_framework/pipeline/pipeline.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2707 2024-05-01 15:18:20.000000 research_framework-0.2.6/research_framework/pipeline/pipeline_manager.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/research_framework/plugins/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      416 2023-09-17 16:58:56.000000 research_framework-0.2.6/research_framework/plugins/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6255 2024-05-05 09:19:43.000000 research_framework-0.2.6/research_framework/plugins/cv_strategies_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1626 2024-04-10 02:28:58.000000 research_framework-0.2.6/research_framework/plugins/data_ingestion_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4391 2023-09-21 10:17:00.000000 research_framework-0.2.6/research_framework/plugins/doomy_predictor.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    11566 2024-05-01 12:28:48.000000 research_framework-0.2.6/research_framework/plugins/grid_search_cross_val.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2968 2024-05-01 12:49:35.000000 research_framework-0.2.6/research_framework/plugins/metrics_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1526 2023-09-20 20:59:39.000000 research_framework-0.2.6/research_framework/plugins/text_mod_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4267 2023-09-20 22:03:53.000000 research_framework-0.2.6/research_framework/plugins/text_rep_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6814 2024-05-07 18:19:04.000000 research_framework-0.2.6/research_framework/plugins/unsupervised_predictor.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1096 2023-09-19 18:12:57.000000 research_framework-0.2.6/research_framework/plugins/vector_red_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3412 2024-05-08 00:36:04.000000 research_framework-0.2.6/research_framework/plugins/wandb_sweep_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5324 2024-05-01 17:06:24.000000 research_framework-0.2.6/research_framework/plugins/wrappers.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/research_framework/storage/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-02 20:07:06.000000 research_framework-0.2.6/research_framework/storage/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4770 2024-04-25 16:30:23.000000 research_framework-0.2.6/research_framework/storage/google_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1732 2024-04-25 16:33:38.000000 research_framework-0.2.6/research_framework/storage/local_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2893 2024-04-25 16:30:12.000000 research_framework-0.2.6/research_framework/storage/s3_storage.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/research_framework.egg-info/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-05-08 00:38:00.000000 research_framework-0.2.6/research_framework.egg-info/PKG-INFO
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3987 2024-05-08 00:38:00.000000 research_framework-0.2.6/research_framework.egg-info/SOURCES.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        1 2024-05-08 00:38:00.000000 research_framework-0.2.6/research_framework.egg-info/dependency_links.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      386 2024-05-08 00:38:00.000000 research_framework-0.2.6/research_framework.egg-info/requires.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       32 2024-05-08 00:38:00.000000 research_framework-0.2.6/research_framework.egg-info/top_level.txt
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/scripts/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.6/scripts/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      507 2023-09-19 19:10:14.000000 research_framework-0.2.6/scripts/clean.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      183 2023-09-06 13:45:32.000000 research_framework-0.2.6/scripts/clean_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       38 2024-05-08 00:38:00.187687 research_framework-0.2.6/setup.cfg
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1059 2024-05-08 00:37:51.000000 research_framework-0.2.6/setup.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/test/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.6/test/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/test/metrics/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:39:11.000000 research_framework-0.2.6/test/metrics/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      757 2024-04-25 18:51:45.000000 research_framework-0.2.6/test/metrics/test_metrics.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-08 00:38:00.187687 research_framework-0.2.6/test/plugins/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.6/test/plugins/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      644 2024-04-25 18:08:47.000000 research_framework-0.2.6/test/plugins/test_mem_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1796 2023-09-20 12:11:32.000000 research_framework-0.2.6/test/plugins/test_plugin.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      956 2023-11-07 13:40:25.000000 research_framework-0.2.6/test/test_container_bindings.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3554 2023-11-07 12:38:53.000000 research_framework-0.2.6/test/test_flyweight_with_google_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2023-11-06 20:17:48.000000 research_framework-0.2.6/test/test_flyweight_with_local_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3555 2024-01-14 01:08:22.000000 research_framework-0.2.6/test/test_flyweight_with_s3_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6278 2024-04-26 12:01:06.000000 research_framework-0.2.6/test/test_mem_module.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     7174 2023-12-29 14:28:04.000000 research_framework-0.2.6/test/test_pipeline.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6881 2023-12-29 14:27:46.000000 research_framework-0.2.6/test/test_pipeline_grid_search.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6934 2024-04-25 16:54:39.000000 research_framework-0.2.6/test/test_simple_pipeline.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6510 2024-04-10 01:52:30.000000 research_framework-0.2.6/test/test_simple_pipeline_manager.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     9090 2024-05-08 00:26:58.000000 research_framework-0.2.6/test/test_simple_pipeline_with_sweep_supervised.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8873 2024-05-08 00:27:12.000000 research_framework-0.2.6/test/test_simple_pipeline_with_sweep_unsupervised.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4580 2023-09-20 12:16:43.000000 research_framework-0.2.6/test/test_wrappers_type_validation.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.753584 research_framework-0.2.7/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    35149 2023-09-01 08:34:48.000000 research_framework-0.2.7/LICENSE
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       24 2023-09-01 08:34:48.000000 research_framework-0.2.7/MANIFEST.in
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-05-10 17:14:00.753584 research_framework-0.2.7/PKG-INFO
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      393 2024-05-01 13:22:11.000000 research_framework-0.2.7/requirements.txt
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.741584 research_framework-0.2.7/research_framework/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       91 2023-11-07 13:43:38.000000 research_framework-0.2.7/research_framework/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.741584 research_framework-0.2.7/research_framework/base/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/base/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.741584 research_framework-0.2.7/research_framework/base/container/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/base/container/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1990 2023-11-09 16:51:42.000000 research_framework-0.2.7/research_framework/base/container/base_container.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.741584 research_framework-0.2.7/research_framework/base/container/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.7/research_framework/base/container/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      722 2023-09-19 17:54:13.000000 research_framework-0.2.7/research_framework/base/container/model/bind_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.741584 research_framework-0.2.7/research_framework/base/flyweight/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.7/research_framework/base/flyweight/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1074 2023-11-08 13:26:10.000000 research_framework-0.2.7/research_framework/base/flyweight/base_flyweight.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      800 2024-04-25 16:51:06.000000 research_framework-0.2.7/research_framework/base/flyweight/base_flyweight_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/base/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/base/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2550 2024-03-02 14:06:30.000000 research_framework-0.2.7/research_framework/base/model/base_dao.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      567 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/base/model/base_utils.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/base/pipeline/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-06 20:33:03.000000 research_framework-0.2.7/research_framework/base/pipeline/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      227 2023-12-29 14:25:32.000000 research_framework-0.2.7/research_framework/base/pipeline/base_pipeline.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/base/plugin/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/base/plugin/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1029 2023-10-15 10:47:16.000000 research_framework-0.2.7/research_framework/base/plugin/base_plugin.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      337 2024-04-25 10:02:49.000000 research_framework-0.2.7/research_framework/base/plugin/base_wrapper.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/base/singleton/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:03:32.000000 research_framework-0.2.7/research_framework/base/singleton/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      262 2024-04-25 16:34:16.000000 research_framework-0.2.7/research_framework/base/singleton/base_singleton.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/base/storage/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/base/storage/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      545 2024-04-25 16:34:46.000000 research_framework-0.2.7/research_framework/base/storage/base_storage.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/base/utils/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-21 13:26:13.000000 research_framework-0.2.7/research_framework/base/utils/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1503 2024-05-01 17:24:30.000000 research_framework-0.2.7/research_framework/base/utils/grid_seach.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      308 2023-09-19 18:09:27.000000 research_framework-0.2.7/research_framework/base/utils/method_overload.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/container/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.7/research_framework/container/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5265 2024-05-01 16:40:16.000000 research_framework-0.2.7/research_framework/container/container.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/container/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-17 21:22:31.000000 research_framework-0.2.7/research_framework/container/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      505 2024-05-01 12:33:48.000000 research_framework-0.2.7/research_framework/container/model/global_config.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/dataset/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:07:36.000000 research_framework-0.2.7/research_framework/dataset/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      872 2023-09-20 22:03:33.000000 research_framework-0.2.7/research_framework/dataset/basic_dataset.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1071 2023-11-07 10:26:41.000000 research_framework-0.2.7/research_framework/dataset/standard_dataset.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/flyweight/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/flyweight/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8026 2024-04-24 16:58:20.000000 research_framework-0.2.7/research_framework/flyweight/flyweight.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    14387 2024-04-25 17:28:03.000000 research_framework-0.2.7/research_framework/flyweight/flyweight_manager.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3638 2024-05-07 18:36:36.000000 research_framework-0.2.7/research_framework/flyweight/mem_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/flyweight/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/flyweight/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1011 2023-09-06 13:45:32.000000 research_framework-0.2.7/research_framework/flyweight/model/item_dao.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      659 2023-11-08 13:27:58.000000 research_framework-0.2.7/research_framework/flyweight/model/item_model.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      497 2024-04-10 01:30:54.000000 research_framework-0.2.7/research_framework/flyweight/model/item_simple_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/neural_models/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:13:05.000000 research_framework-0.2.7/research_framework/neural_models/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      379 2023-09-13 12:58:06.000000 research_framework-0.2.7/research_framework/neural_models/doomy_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/pipeline/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       48 2023-11-07 13:43:32.000000 research_framework-0.2.7/research_framework/pipeline/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.745584 research_framework-0.2.7/research_framework/pipeline/exceptions/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 13:09:29.000000 research_framework-0.2.7/research_framework/pipeline/exceptions/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       54 2024-05-01 13:11:12.000000 research_framework-0.2.7/research_framework/pipeline/exceptions/pipeline_exceptions.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       49 2024-05-01 13:11:19.000000 research_framework-0.2.7/research_framework/pipeline/exceptions/run_exceptions.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      491 2023-09-06 13:45:32.000000 research_framework-0.2.7/research_framework/pipeline/inputs.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.749585 research_framework-0.2.7/research_framework/pipeline/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/research_framework/pipeline/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3293 2024-05-05 09:01:39.000000 research_framework-0.2.7/research_framework/pipeline/model/pipeline_model.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    10055 2024-05-05 08:57:44.000000 research_framework-0.2.7/research_framework/pipeline/pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2707 2024-05-01 15:18:20.000000 research_framework-0.2.7/research_framework/pipeline/pipeline_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.749585 research_framework-0.2.7/research_framework/plugins/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      416 2023-09-17 16:58:56.000000 research_framework-0.2.7/research_framework/plugins/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6255 2024-05-05 09:19:43.000000 research_framework-0.2.7/research_framework/plugins/cv_strategies_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1626 2024-04-10 02:28:58.000000 research_framework-0.2.7/research_framework/plugins/data_ingestion_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4391 2023-09-21 10:17:00.000000 research_framework-0.2.7/research_framework/plugins/doomy_predictor.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    11566 2024-05-01 12:28:48.000000 research_framework-0.2.7/research_framework/plugins/grid_search_cross_val.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2968 2024-05-01 12:49:35.000000 research_framework-0.2.7/research_framework/plugins/metrics_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1526 2023-09-20 20:59:39.000000 research_framework-0.2.7/research_framework/plugins/text_mod_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4267 2023-09-20 22:03:53.000000 research_framework-0.2.7/research_framework/plugins/text_rep_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6814 2024-05-07 18:19:04.000000 research_framework-0.2.7/research_framework/plugins/unsupervised_predictor.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1096 2023-09-19 18:12:57.000000 research_framework-0.2.7/research_framework/plugins/vector_red_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3412 2024-05-08 00:36:04.000000 research_framework-0.2.7/research_framework/plugins/wandb_sweep_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5318 2024-05-10 17:11:55.000000 research_framework-0.2.7/research_framework/plugins/wrappers.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.749585 research_framework-0.2.7/research_framework/storage/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-02 20:07:06.000000 research_framework-0.2.7/research_framework/storage/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4770 2024-04-25 16:30:23.000000 research_framework-0.2.7/research_framework/storage/google_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1732 2024-04-25 16:33:38.000000 research_framework-0.2.7/research_framework/storage/local_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2893 2024-04-25 16:30:12.000000 research_framework-0.2.7/research_framework/storage/s3_storage.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.753584 research_framework-0.2.7/research_framework.egg-info/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-05-10 17:14:00.000000 research_framework-0.2.7/research_framework.egg-info/PKG-INFO
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3987 2024-05-10 17:14:00.000000 research_framework-0.2.7/research_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        1 2024-05-10 17:14:00.000000 research_framework-0.2.7/research_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      386 2024-05-10 17:14:00.000000 research_framework-0.2.7/research_framework.egg-info/requires.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       32 2024-05-10 17:14:00.000000 research_framework-0.2.7/research_framework.egg-info/top_level.txt
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.749585 research_framework-0.2.7/scripts/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.7/scripts/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      507 2023-09-19 19:10:14.000000 research_framework-0.2.7/scripts/clean.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      183 2023-09-06 13:45:32.000000 research_framework-0.2.7/scripts/clean_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       38 2024-05-10 17:14:00.753584 research_framework-0.2.7/setup.cfg
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1059 2024-05-10 17:13:56.000000 research_framework-0.2.7/setup.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.749585 research_framework-0.2.7/test/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.7/test/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.749585 research_framework-0.2.7/test/metrics/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:39:11.000000 research_framework-0.2.7/test/metrics/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      757 2024-04-25 18:51:45.000000 research_framework-0.2.7/test/metrics/test_metrics.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-10 17:14:00.753584 research_framework-0.2.7/test/plugins/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.7/test/plugins/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      644 2024-04-25 18:08:47.000000 research_framework-0.2.7/test/plugins/test_mem_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1796 2023-09-20 12:11:32.000000 research_framework-0.2.7/test/plugins/test_plugin.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      956 2023-11-07 13:40:25.000000 research_framework-0.2.7/test/test_container_bindings.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3554 2023-11-07 12:38:53.000000 research_framework-0.2.7/test/test_flyweight_with_google_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2023-11-06 20:17:48.000000 research_framework-0.2.7/test/test_flyweight_with_local_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3555 2024-01-14 01:08:22.000000 research_framework-0.2.7/test/test_flyweight_with_s3_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6278 2024-04-26 12:01:06.000000 research_framework-0.2.7/test/test_mem_module.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     7174 2023-12-29 14:28:04.000000 research_framework-0.2.7/test/test_pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6881 2023-12-29 14:27:46.000000 research_framework-0.2.7/test/test_pipeline_grid_search.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6934 2024-04-25 16:54:39.000000 research_framework-0.2.7/test/test_simple_pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6510 2024-04-10 01:52:30.000000 research_framework-0.2.7/test/test_simple_pipeline_manager.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     9090 2024-05-08 00:26:58.000000 research_framework-0.2.7/test/test_simple_pipeline_with_sweep_supervised.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8873 2024-05-08 00:27:12.000000 research_framework-0.2.7/test/test_simple_pipeline_with_sweep_unsupervised.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4580 2023-09-20 12:16:43.000000 research_framework-0.2.7/test/test_wrappers_type_validation.py
```

### Comparing `research_framework-0.2.6/LICENSE` & `research_framework-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/PKG-INFO` & `research_framework-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-framework
-Version: 0.2.6
+Version: 0.2.7
 Summary: framework base para investigación
 Home-page: https://github.com/manucouto1/research_framework
 Author: Manuel Couto Pintos
 Author-email: manuel.couto.pintos@usc.es
 License: Apache License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `research_framework-0.2.6/research_framework/base/container/base_container.py` & `research_framework-0.2.7/research_framework/base/container/base_container.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/container/model/bind_model.py` & `research_framework-0.2.7/research_framework/base/container/model/bind_model.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/flyweight/base_flyweight.py` & `research_framework-0.2.7/research_framework/base/flyweight/base_flyweight.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/flyweight/base_flyweight_manager.py` & `research_framework-0.2.7/research_framework/base/flyweight/base_flyweight_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/model/base_dao.py` & `research_framework-0.2.7/research_framework/base/model/base_dao.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/model/base_utils.py` & `research_framework-0.2.7/research_framework/base/model/base_utils.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/plugin/base_plugin.py` & `research_framework-0.2.7/research_framework/base/plugin/base_plugin.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/storage/base_storage.py` & `research_framework-0.2.7/research_framework/base/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/base/utils/grid_seach.py` & `research_framework-0.2.7/research_framework/base/utils/grid_seach.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/container/container.py` & `research_framework-0.2.7/research_framework/container/container.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/dataset/basic_dataset.py` & `research_framework-0.2.7/research_framework/dataset/basic_dataset.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/dataset/standard_dataset.py` & `research_framework-0.2.7/research_framework/dataset/standard_dataset.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/flyweight/flyweight.py` & `research_framework-0.2.7/research_framework/flyweight/flyweight.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/flyweight/flyweight_manager.py` & `research_framework-0.2.7/research_framework/flyweight/flyweight_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/flyweight/mem_manager.py` & `research_framework-0.2.7/research_framework/flyweight/mem_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/flyweight/model/item_dao.py` & `research_framework-0.2.7/research_framework/flyweight/model/item_dao.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/flyweight/model/item_model.py` & `research_framework-0.2.7/research_framework/flyweight/model/item_model.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/pipeline/model/pipeline_model.py` & `research_framework-0.2.7/research_framework/pipeline/model/pipeline_model.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/pipeline/pipeline.py` & `research_framework-0.2.7/research_framework/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/pipeline/pipeline_manager.py` & `research_framework-0.2.7/research_framework/pipeline/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/cv_strategies_plugins.py` & `research_framework-0.2.7/research_framework/plugins/cv_strategies_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/data_ingestion_plugins.py` & `research_framework-0.2.7/research_framework/plugins/data_ingestion_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/doomy_predictor.py` & `research_framework-0.2.7/research_framework/plugins/doomy_predictor.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/grid_search_cross_val.py` & `research_framework-0.2.7/research_framework/plugins/grid_search_cross_val.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/metrics_plugins.py` & `research_framework-0.2.7/research_framework/plugins/metrics_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/text_mod_plugins.py` & `research_framework-0.2.7/research_framework/plugins/text_mod_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/text_rep_plugins.py` & `research_framework-0.2.7/research_framework/plugins/text_rep_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/unsupervised_predictor.py` & `research_framework-0.2.7/research_framework/plugins/unsupervised_predictor.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/vector_red_plugins.py` & `research_framework-0.2.7/research_framework/plugins/vector_red_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/wandb_sweep_plugins.py` & `research_framework-0.2.7/research_framework/plugins/wandb_sweep_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/plugins/wrappers.py` & `research_framework-0.2.7/research_framework/plugins/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     
     @methdispatch
     def predict(self, x):
         raise TypeError(f"Wrong input type {type(x)}")
 
     @fit.register
     def _(self, x:pd.DataFrame) -> BasePlugin:
-        return self.plugin.fit(x, None)
+        return self.plugin.fit(x)
     
     @predict.register
     def _(self, x:pd.DataFrame) -> pd.DataFrame:
         return self.plugin.predict(x)
     
     @fit.register
     def _fit(self, x:StandardDataset):
```

### Comparing `research_framework-0.2.6/research_framework/storage/google_storage.py` & `research_framework-0.2.7/research_framework/storage/google_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/storage/local_storage.py` & `research_framework-0.2.7/research_framework/storage/local_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework/storage/s3_storage.py` & `research_framework-0.2.7/research_framework/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/research_framework.egg-info/PKG-INFO` & `research_framework-0.2.7/research_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-framework
-Version: 0.2.6
+Version: 0.2.7
 Summary: framework base para investigación
 Home-page: https://github.com/manucouto1/research_framework
 Author: Manuel Couto Pintos
 Author-email: manuel.couto.pintos@usc.es
 License: Apache License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `research_framework-0.2.6/research_framework.egg-info/SOURCES.txt` & `research_framework-0.2.7/research_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/setup.py` & `research_framework-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         str(requirement)
         for requirement
         in parse_requirements(requirements_txt)
     ]
 
 setup(
     name="research-framework",
-    version='0.2.6',
+    version='0.2.7',
     description="framework base para investigación",
     url="https://github.com/manucouto1/research_framework",
     author="Manuel Couto Pintos",
     author_email="manuel.couto.pintos@usc.es",
     license="Apache License",
     packages=find_packages(),
     install_requires=install_requires,
```

### Comparing `research_framework-0.2.6/test/metrics/test_metrics.py` & `research_framework-0.2.7/test/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/plugins/test_mem_plugins.py` & `research_framework-0.2.7/test/plugins/test_mem_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/plugins/test_plugin.py` & `research_framework-0.2.7/test/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_container_bindings.py` & `research_framework-0.2.7/test/test_container_bindings.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_flyweight_with_google_storage.py` & `research_framework-0.2.7/test/test_flyweight_with_google_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_flyweight_with_local_storage.py` & `research_framework-0.2.7/test/test_flyweight_with_local_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_flyweight_with_s3_storage.py` & `research_framework-0.2.7/test/test_flyweight_with_s3_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_mem_module.py` & `research_framework-0.2.7/test/test_mem_module.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_pipeline.py` & `research_framework-0.2.7/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_pipeline_grid_search.py` & `research_framework-0.2.7/test/test_pipeline_grid_search.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_simple_pipeline.py` & `research_framework-0.2.7/test/test_simple_pipeline.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_simple_pipeline_manager.py` & `research_framework-0.2.7/test/test_simple_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_simple_pipeline_with_sweep_supervised.py` & `research_framework-0.2.7/test/test_simple_pipeline_with_sweep_supervised.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_simple_pipeline_with_sweep_unsupervised.py` & `research_framework-0.2.7/test/test_simple_pipeline_with_sweep_unsupervised.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.6/test/test_wrappers_type_validation.py` & `research_framework-0.2.7/test/test_wrappers_type_validation.py`

 * *Files identical despite different names*

