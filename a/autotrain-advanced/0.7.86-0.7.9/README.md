# Comparing `tmp/autotrain-advanced-0.7.86.tar.gz` & `tmp/autotrain-advanced-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.86.tar", last modified: Fri May 10 12:23:20 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.9.tar", last modified: Sat Mar  9 10:16:49 2024, max compression
```

## Comparing `autotrain-advanced-0.7.86.tar` & `autotrain-advanced-0.7.9.tar`

### file list

```diff
@@ -1,143 +1,111 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.171770 autotrain-advanced-0.7.86/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.86/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    12905 2024-05-10 12:23:20.171770 autotrain-advanced-0.7.86/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2741 2024-05-04 09:15:32.000000 autotrain-advanced-0.7.86/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-10 12:23:20.171770 autotrain-advanced-0.7.86/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.147770 autotrain-advanced-0.7.86/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.147770 autotrain-advanced-0.7.86/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1450 2024-05-10 12:23:15.000000 autotrain-advanced-0.7.86/src/autotrain/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.147770 autotrain-advanced-0.7.86/src/autotrain/app/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10965 2024-05-10 12:20:45.000000 autotrain-advanced-0.7.86/src/autotrain/app/api_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      669 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7379 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/models.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/oauth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17040 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/app/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/static/logo.png
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/app/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49409 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/templates/login.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/training_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16971 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/ui_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/app/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/backends/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.86/src/autotrain/backends/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4872 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.86/src/autotrain/backends/base.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/backends/endpoints.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.86/src/autotrain/backends/local.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.86/src/autotrain/backends/ngc.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/backends/nvcf.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.86/src/autotrain/backends/spaces.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.86/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2854 2024-05-03 11:51:37.000000 autotrain-advanced-0.7.86/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3668 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7706 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9902 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7989 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7933 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_text_regression.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7910 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.86/src/autotrain/cli/run_tools.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13957 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.86/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10860 2024-05-08 17:28:06.000000 autotrain-advanced-0.7.86/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.86/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16270 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.86/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.86/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.86/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6051 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/parser.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.86/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.86/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.86/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7141 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.86/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2520 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.86/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      850 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.86/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/tools/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.86/src/autotrain/tools/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.86/src/autotrain/tools/convert_to_kohya.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.86/src/autotrain/tools/merge_adapter.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.151770 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/train_clm_default.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/train_clm_dpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/train_clm_orpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/train_clm_reward.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/train_clm_sft.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8195 2024-05-06 12:50:40.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/train.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/train_xl.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7242 2024-04-25 05:44:20.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1824 2024-04-25 05:53:27.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8817 2024-04-29 09:01:25.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2424 2024-04-25 05:53:33.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7647 2024-04-25 05:44:56.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1876 2024-04-25 05:53:42.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/text_regression/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_regression/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6928 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_regression/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_regression/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1875 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_regression/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/text_regression/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7428 2024-04-25 05:44:07.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1877 2024-04-25 05:53:47.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1932 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.86/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    12905 2024-05-10 12:23:20.000000 autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4589 2024-05-10 12:23:20.000000 autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-10 12:23:20.000000 autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-10 12:23:20.000000 autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3479 2024-05-10 12:23:20.000000 autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-10 12:23:20.000000 autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:23:20.155770 autotrain-advanced-0.7.86/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.86/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.904001 autotrain-advanced-0.7.9/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.9/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    11924 2024-03-09 10:16:49.904001 autotrain-advanced-0.7.9/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2433 2024-03-08 09:21:33.000000 autotrain-advanced-0.7.9/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-03-09 10:16:49.908001 autotrain-advanced-0.7.9/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-02-29 11:54:14.000000 autotrain-advanced-0.7.9/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      954 2024-03-09 10:16:44.000000 autotrain-advanced-0.7.9/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1774 2024-03-08 08:21:06.000000 autotrain-advanced-0.7.9/src/autotrain/api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17396 2024-03-09 07:47:44.000000 autotrain-advanced-0.7.9/src/autotrain/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5159 2024-02-22 14:54:32.000000 autotrain-advanced-0.7.9/src/autotrain/app_params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5918 2024-02-29 11:39:11.000000 autotrain-advanced-0.7.9/src/autotrain/app_utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    22327 2024-03-09 10:14:16.000000 autotrain-advanced-0.7.9/src/autotrain/backend.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.9/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2110 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1312 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2136 2023-12-15 13:15:05.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13233 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6303 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14393 2024-02-22 15:15:30.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7510 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-09 07:52:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5224 2023-12-05 20:59:47.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5671 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6121 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10880 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9719 2024-02-13 17:29:11.000000 autotrain-advanced-0.7.9/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      309 2023-08-16 09:13:38.000000 autotrain-advanced-0.7.9/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16028 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-02-14 13:51:37.000000 autotrain-advanced-0.7.9/src/autotrain/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-02-21 15:24:07.000000 autotrain-advanced-0.7.9/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1067 2024-02-14 15:04:27.000000 autotrain-advanced-0.7.9/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4323 2024-02-29 14:19:36.000000 autotrain-advanced-0.7.9/src/autotrain/oauth.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3241 2023-12-20 19:37:58.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14997 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7225 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.9/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2449 2024-03-08 08:21:06.000000 autotrain-advanced-0.7.9/src/autotrain/project.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.888002 autotrain-advanced-0.7.9/src/autotrain/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-12-15 11:33:40.000000 autotrain-advanced-0.7.9/src/autotrain/static/logo.png
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2865 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-02-24 10:09:47.000000 autotrain-advanced-0.7.9/src/autotrain/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2023-12-15 11:33:14.000000 autotrain-advanced-0.7.9/src/autotrain/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    36074 2024-03-09 07:52:04.000000 autotrain-advanced-0.7.9/src/autotrain/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2024-02-29 12:52:07.000000 autotrain-advanced-0.7.9/src/autotrain/templates/login.html
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21138 2024-02-23 07:46:34.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3312 2024-02-22 15:16:12.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10791 2024-02-29 12:02:21.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5163 2024-02-19 10:34:58.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13123 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4071 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21920 2023-11-04 11:49:08.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13687 2023-12-20 19:59:04.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      654 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3640 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6699 2024-02-26 12:26:15.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1945 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-08 09:54:18.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8217 2023-12-21 15:04:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2485 2024-02-22 09:28:57.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12525 2023-12-21 18:57:22.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1468 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7253 2024-01-26 09:52:49.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1997 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6999 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1998 2024-02-13 09:53:54.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1696 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6788 2024-02-14 13:51:37.000000 autotrain-advanced-0.7.9/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    11924 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3449 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3129 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-03-09 10:16:49.000000 autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-03-09 10:16:49.892001 autotrain-advanced-0.7.9/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.9/static/logo.png
```

### Comparing `autotrain-advanced-0.7.86/LICENSE` & `autotrain-advanced-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/PKG-INFO` & `autotrain-advanced-0.7.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.86
+Version: 0.7.9
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,212 +16,200 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: albumentations==1.4.4
-Requires-Dist: codecarbon==2.3.5
-Requires-Dist: datasets[vision]~=2.19.0
-Requires-Dist: evaluate==0.4.1
+Requires-Dist: albumentations==1.3.1
+Requires-Dist: codecarbon==2.2.3
+Requires-Dist: datasets[vision]~=2.14.0
+Requires-Dist: evaluate==0.3.0
 Requires-Dist: ipadic==1.0.0
-Requires-Dist: jiwer==3.0.3
-Requires-Dist: joblib==1.4.0
-Requires-Dist: loguru==0.7.2
-Requires-Dist: pandas==2.2.2
+Requires-Dist: jiwer==3.0.2
+Requires-Dist: joblib==1.3.1
+Requires-Dist: loguru==0.7.0
+Requires-Dist: pandas>=1.4
 Requires-Dist: nltk==3.8.1
-Requires-Dist: optuna==3.6.1
-Requires-Dist: Pillow==10.3.0
+Requires-Dist: optuna==3.3.0
+Requires-Dist: Pillow==10.0.0
 Requires-Dist: protobuf==4.23.4
-Requires-Dist: sacremoses==0.1.1
-Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: sentencepiece==0.2.0
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: werkzeug==3.0.2
-Requires-Dist: xgboost==2.0.3
-Requires-Dist: huggingface_hub==0.22.2
+Requires-Dist: sacremoses==0.0.53
+Requires-Dist: scikit-learn==1.3.0
+Requires-Dist: sentencepiece==0.1.99
+Requires-Dist: tqdm==4.65.0
+Requires-Dist: werkzeug==2.3.6
+Requires-Dist: xgboost==1.7.6
+Requires-Dist: huggingface_hub>=0.16.4
 Requires-Dist: requests==2.31.0
-Requires-Dist: einops==0.7.0
+Requires-Dist: einops==0.6.1
 Requires-Dist: invisible-watermark==0.2.0
-Requires-Dist: packaging==24.0
-Requires-Dist: cryptography==42.0.5
-Requires-Dist: nvitop==1.3.2
-Requires-Dist: tensorboard==2.16.2
-Requires-Dist: peft==0.10.0
-Requires-Dist: trl==0.8.6
+Requires-Dist: packaging==23.1
+Requires-Dist: tensorboard
+Requires-Dist: peft==0.9.0
+Requires-Dist: trl==0.7.11
 Requires-Dist: tiktoken==0.6.0
-Requires-Dist: transformers==4.40.1
-Requires-Dist: accelerate==0.29.3
-Requires-Dist: diffusers==0.27.2
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux"
+Requires-Dist: transformers==4.38.2
+Requires-Dist: accelerate==0.27.2
+Requires-Dist: diffusers==0.26.3
+Requires-Dist: bitsandbytes==0.42.0
 Requires-Dist: rouge_score==0.1.2
-Requires-Dist: py7zr==0.21.0
-Requires-Dist: fastapi==0.110.2
-Requires-Dist: uvicorn==0.29.0
-Requires-Dist: python-multipart==0.0.9
-Requires-Dist: pydantic==2.7.1
+Requires-Dist: py7zr==0.20.6
+Requires-Dist: fastapi==0.104.1
+Requires-Dist: uvicorn==0.22.0
+Requires-Dist: python-multipart==0.0.6
+Requires-Dist: gradio==3.41.0
+Requires-Dist: pydantic==2.4.2
 Requires-Dist: hf-transfer
-Requires-Dist: pyngrok==7.1.6
+Requires-Dist: pyngrok==7.0.3
 Requires-Dist: authlib==1.3.0
-Requires-Dist: itsdangerous==2.2.0
+Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: seqeval==1.2.2
-Requires-Dist: httpx==0.27.0
-Requires-Dist: pyyaml==6.0.1
 Provides-Extra: dev
-Requires-Dist: albumentations==1.4.4; extra == "dev"
-Requires-Dist: codecarbon==2.3.5; extra == "dev"
-Requires-Dist: datasets[vision]~=2.19.0; extra == "dev"
-Requires-Dist: evaluate==0.4.1; extra == "dev"
+Requires-Dist: albumentations==1.3.1; extra == "dev"
+Requires-Dist: codecarbon==2.2.3; extra == "dev"
+Requires-Dist: datasets[vision]~=2.14.0; extra == "dev"
+Requires-Dist: evaluate==0.3.0; extra == "dev"
 Requires-Dist: ipadic==1.0.0; extra == "dev"
-Requires-Dist: jiwer==3.0.3; extra == "dev"
-Requires-Dist: joblib==1.4.0; extra == "dev"
-Requires-Dist: loguru==0.7.2; extra == "dev"
-Requires-Dist: pandas==2.2.2; extra == "dev"
+Requires-Dist: jiwer==3.0.2; extra == "dev"
+Requires-Dist: joblib==1.3.1; extra == "dev"
+Requires-Dist: loguru==0.7.0; extra == "dev"
+Requires-Dist: pandas>=1.4; extra == "dev"
 Requires-Dist: nltk==3.8.1; extra == "dev"
-Requires-Dist: optuna==3.6.1; extra == "dev"
-Requires-Dist: Pillow==10.3.0; extra == "dev"
+Requires-Dist: optuna==3.3.0; extra == "dev"
+Requires-Dist: Pillow==10.0.0; extra == "dev"
 Requires-Dist: protobuf==4.23.4; extra == "dev"
-Requires-Dist: sacremoses==0.1.1; extra == "dev"
-Requires-Dist: scikit-learn==1.4.2; extra == "dev"
-Requires-Dist: sentencepiece==0.2.0; extra == "dev"
-Requires-Dist: tqdm==4.66.2; extra == "dev"
-Requires-Dist: werkzeug==3.0.2; extra == "dev"
-Requires-Dist: xgboost==2.0.3; extra == "dev"
-Requires-Dist: huggingface_hub==0.22.2; extra == "dev"
+Requires-Dist: sacremoses==0.0.53; extra == "dev"
+Requires-Dist: scikit-learn==1.3.0; extra == "dev"
+Requires-Dist: sentencepiece==0.1.99; extra == "dev"
+Requires-Dist: tqdm==4.65.0; extra == "dev"
+Requires-Dist: werkzeug==2.3.6; extra == "dev"
+Requires-Dist: xgboost==1.7.6; extra == "dev"
+Requires-Dist: huggingface_hub>=0.16.4; extra == "dev"
 Requires-Dist: requests==2.31.0; extra == "dev"
-Requires-Dist: einops==0.7.0; extra == "dev"
+Requires-Dist: einops==0.6.1; extra == "dev"
 Requires-Dist: invisible-watermark==0.2.0; extra == "dev"
-Requires-Dist: packaging==24.0; extra == "dev"
-Requires-Dist: cryptography==42.0.5; extra == "dev"
-Requires-Dist: nvitop==1.3.2; extra == "dev"
-Requires-Dist: tensorboard==2.16.2; extra == "dev"
-Requires-Dist: peft==0.10.0; extra == "dev"
-Requires-Dist: trl==0.8.6; extra == "dev"
+Requires-Dist: packaging==23.1; extra == "dev"
+Requires-Dist: tensorboard; extra == "dev"
+Requires-Dist: peft==0.9.0; extra == "dev"
+Requires-Dist: trl==0.7.11; extra == "dev"
 Requires-Dist: tiktoken==0.6.0; extra == "dev"
-Requires-Dist: transformers==4.40.1; extra == "dev"
-Requires-Dist: accelerate==0.29.3; extra == "dev"
-Requires-Dist: diffusers==0.27.2; extra == "dev"
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux" and extra == "dev"
+Requires-Dist: transformers==4.38.2; extra == "dev"
+Requires-Dist: accelerate==0.27.2; extra == "dev"
+Requires-Dist: diffusers==0.26.3; extra == "dev"
+Requires-Dist: bitsandbytes==0.42.0; extra == "dev"
 Requires-Dist: rouge_score==0.1.2; extra == "dev"
-Requires-Dist: py7zr==0.21.0; extra == "dev"
-Requires-Dist: fastapi==0.110.2; extra == "dev"
-Requires-Dist: uvicorn==0.29.0; extra == "dev"
-Requires-Dist: python-multipart==0.0.9; extra == "dev"
-Requires-Dist: pydantic==2.7.1; extra == "dev"
+Requires-Dist: py7zr==0.20.6; extra == "dev"
+Requires-Dist: fastapi==0.104.1; extra == "dev"
+Requires-Dist: uvicorn==0.22.0; extra == "dev"
+Requires-Dist: python-multipart==0.0.6; extra == "dev"
+Requires-Dist: gradio==3.41.0; extra == "dev"
+Requires-Dist: pydantic==2.4.2; extra == "dev"
 Requires-Dist: hf-transfer; extra == "dev"
-Requires-Dist: pyngrok==7.1.6; extra == "dev"
+Requires-Dist: pyngrok==7.0.3; extra == "dev"
 Requires-Dist: authlib==1.3.0; extra == "dev"
-Requires-Dist: itsdangerous==2.2.0; extra == "dev"
+Requires-Dist: itsdangerous==2.1.2; extra == "dev"
 Requires-Dist: seqeval==1.2.2; extra == "dev"
-Requires-Dist: httpx==0.27.0; extra == "dev"
-Requires-Dist: pyyaml==6.0.1; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: flake8==3.7.9; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: quality
-Requires-Dist: albumentations==1.4.4; extra == "quality"
-Requires-Dist: codecarbon==2.3.5; extra == "quality"
-Requires-Dist: datasets[vision]~=2.19.0; extra == "quality"
-Requires-Dist: evaluate==0.4.1; extra == "quality"
+Requires-Dist: albumentations==1.3.1; extra == "quality"
+Requires-Dist: codecarbon==2.2.3; extra == "quality"
+Requires-Dist: datasets[vision]~=2.14.0; extra == "quality"
+Requires-Dist: evaluate==0.3.0; extra == "quality"
 Requires-Dist: ipadic==1.0.0; extra == "quality"
-Requires-Dist: jiwer==3.0.3; extra == "quality"
-Requires-Dist: joblib==1.4.0; extra == "quality"
-Requires-Dist: loguru==0.7.2; extra == "quality"
-Requires-Dist: pandas==2.2.2; extra == "quality"
+Requires-Dist: jiwer==3.0.2; extra == "quality"
+Requires-Dist: joblib==1.3.1; extra == "quality"
+Requires-Dist: loguru==0.7.0; extra == "quality"
+Requires-Dist: pandas>=1.4; extra == "quality"
 Requires-Dist: nltk==3.8.1; extra == "quality"
-Requires-Dist: optuna==3.6.1; extra == "quality"
-Requires-Dist: Pillow==10.3.0; extra == "quality"
+Requires-Dist: optuna==3.3.0; extra == "quality"
+Requires-Dist: Pillow==10.0.0; extra == "quality"
 Requires-Dist: protobuf==4.23.4; extra == "quality"
-Requires-Dist: sacremoses==0.1.1; extra == "quality"
-Requires-Dist: scikit-learn==1.4.2; extra == "quality"
-Requires-Dist: sentencepiece==0.2.0; extra == "quality"
-Requires-Dist: tqdm==4.66.2; extra == "quality"
-Requires-Dist: werkzeug==3.0.2; extra == "quality"
-Requires-Dist: xgboost==2.0.3; extra == "quality"
-Requires-Dist: huggingface_hub==0.22.2; extra == "quality"
+Requires-Dist: sacremoses==0.0.53; extra == "quality"
+Requires-Dist: scikit-learn==1.3.0; extra == "quality"
+Requires-Dist: sentencepiece==0.1.99; extra == "quality"
+Requires-Dist: tqdm==4.65.0; extra == "quality"
+Requires-Dist: werkzeug==2.3.6; extra == "quality"
+Requires-Dist: xgboost==1.7.6; extra == "quality"
+Requires-Dist: huggingface_hub>=0.16.4; extra == "quality"
 Requires-Dist: requests==2.31.0; extra == "quality"
-Requires-Dist: einops==0.7.0; extra == "quality"
+Requires-Dist: einops==0.6.1; extra == "quality"
 Requires-Dist: invisible-watermark==0.2.0; extra == "quality"
-Requires-Dist: packaging==24.0; extra == "quality"
-Requires-Dist: cryptography==42.0.5; extra == "quality"
-Requires-Dist: nvitop==1.3.2; extra == "quality"
-Requires-Dist: tensorboard==2.16.2; extra == "quality"
-Requires-Dist: peft==0.10.0; extra == "quality"
-Requires-Dist: trl==0.8.6; extra == "quality"
+Requires-Dist: packaging==23.1; extra == "quality"
+Requires-Dist: tensorboard; extra == "quality"
+Requires-Dist: peft==0.9.0; extra == "quality"
+Requires-Dist: trl==0.7.11; extra == "quality"
 Requires-Dist: tiktoken==0.6.0; extra == "quality"
-Requires-Dist: transformers==4.40.1; extra == "quality"
-Requires-Dist: accelerate==0.29.3; extra == "quality"
-Requires-Dist: diffusers==0.27.2; extra == "quality"
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux" and extra == "quality"
+Requires-Dist: transformers==4.38.2; extra == "quality"
+Requires-Dist: accelerate==0.27.2; extra == "quality"
+Requires-Dist: diffusers==0.26.3; extra == "quality"
+Requires-Dist: bitsandbytes==0.42.0; extra == "quality"
 Requires-Dist: rouge_score==0.1.2; extra == "quality"
-Requires-Dist: py7zr==0.21.0; extra == "quality"
-Requires-Dist: fastapi==0.110.2; extra == "quality"
-Requires-Dist: uvicorn==0.29.0; extra == "quality"
-Requires-Dist: python-multipart==0.0.9; extra == "quality"
-Requires-Dist: pydantic==2.7.1; extra == "quality"
+Requires-Dist: py7zr==0.20.6; extra == "quality"
+Requires-Dist: fastapi==0.104.1; extra == "quality"
+Requires-Dist: uvicorn==0.22.0; extra == "quality"
+Requires-Dist: python-multipart==0.0.6; extra == "quality"
+Requires-Dist: gradio==3.41.0; extra == "quality"
+Requires-Dist: pydantic==2.4.2; extra == "quality"
 Requires-Dist: hf-transfer; extra == "quality"
-Requires-Dist: pyngrok==7.1.6; extra == "quality"
+Requires-Dist: pyngrok==7.0.3; extra == "quality"
 Requires-Dist: authlib==1.3.0; extra == "quality"
-Requires-Dist: itsdangerous==2.2.0; extra == "quality"
+Requires-Dist: itsdangerous==2.1.2; extra == "quality"
 Requires-Dist: seqeval==1.2.2; extra == "quality"
-Requires-Dist: httpx==0.27.0; extra == "quality"
-Requires-Dist: pyyaml==6.0.1; extra == "quality"
 Requires-Dist: black; extra == "quality"
 Requires-Dist: isort; extra == "quality"
 Requires-Dist: flake8==3.7.9; extra == "quality"
 Provides-Extra: docs
-Requires-Dist: albumentations==1.4.4; extra == "docs"
-Requires-Dist: codecarbon==2.3.5; extra == "docs"
-Requires-Dist: datasets[vision]~=2.19.0; extra == "docs"
-Requires-Dist: evaluate==0.4.1; extra == "docs"
+Requires-Dist: albumentations==1.3.1; extra == "docs"
+Requires-Dist: codecarbon==2.2.3; extra == "docs"
+Requires-Dist: datasets[vision]~=2.14.0; extra == "docs"
+Requires-Dist: evaluate==0.3.0; extra == "docs"
 Requires-Dist: ipadic==1.0.0; extra == "docs"
-Requires-Dist: jiwer==3.0.3; extra == "docs"
-Requires-Dist: joblib==1.4.0; extra == "docs"
-Requires-Dist: loguru==0.7.2; extra == "docs"
-Requires-Dist: pandas==2.2.2; extra == "docs"
+Requires-Dist: jiwer==3.0.2; extra == "docs"
+Requires-Dist: joblib==1.3.1; extra == "docs"
+Requires-Dist: loguru==0.7.0; extra == "docs"
+Requires-Dist: pandas>=1.4; extra == "docs"
 Requires-Dist: nltk==3.8.1; extra == "docs"
-Requires-Dist: optuna==3.6.1; extra == "docs"
-Requires-Dist: Pillow==10.3.0; extra == "docs"
+Requires-Dist: optuna==3.3.0; extra == "docs"
+Requires-Dist: Pillow==10.0.0; extra == "docs"
 Requires-Dist: protobuf==4.23.4; extra == "docs"
-Requires-Dist: sacremoses==0.1.1; extra == "docs"
-Requires-Dist: scikit-learn==1.4.2; extra == "docs"
-Requires-Dist: sentencepiece==0.2.0; extra == "docs"
-Requires-Dist: tqdm==4.66.2; extra == "docs"
-Requires-Dist: werkzeug==3.0.2; extra == "docs"
-Requires-Dist: xgboost==2.0.3; extra == "docs"
-Requires-Dist: huggingface_hub==0.22.2; extra == "docs"
+Requires-Dist: sacremoses==0.0.53; extra == "docs"
+Requires-Dist: scikit-learn==1.3.0; extra == "docs"
+Requires-Dist: sentencepiece==0.1.99; extra == "docs"
+Requires-Dist: tqdm==4.65.0; extra == "docs"
+Requires-Dist: werkzeug==2.3.6; extra == "docs"
+Requires-Dist: xgboost==1.7.6; extra == "docs"
+Requires-Dist: huggingface_hub>=0.16.4; extra == "docs"
 Requires-Dist: requests==2.31.0; extra == "docs"
-Requires-Dist: einops==0.7.0; extra == "docs"
+Requires-Dist: einops==0.6.1; extra == "docs"
 Requires-Dist: invisible-watermark==0.2.0; extra == "docs"
-Requires-Dist: packaging==24.0; extra == "docs"
-Requires-Dist: cryptography==42.0.5; extra == "docs"
-Requires-Dist: nvitop==1.3.2; extra == "docs"
-Requires-Dist: tensorboard==2.16.2; extra == "docs"
-Requires-Dist: peft==0.10.0; extra == "docs"
-Requires-Dist: trl==0.8.6; extra == "docs"
+Requires-Dist: packaging==23.1; extra == "docs"
+Requires-Dist: tensorboard; extra == "docs"
+Requires-Dist: peft==0.9.0; extra == "docs"
+Requires-Dist: trl==0.7.11; extra == "docs"
 Requires-Dist: tiktoken==0.6.0; extra == "docs"
-Requires-Dist: transformers==4.40.1; extra == "docs"
-Requires-Dist: accelerate==0.29.3; extra == "docs"
-Requires-Dist: diffusers==0.27.2; extra == "docs"
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux" and extra == "docs"
+Requires-Dist: transformers==4.38.2; extra == "docs"
+Requires-Dist: accelerate==0.27.2; extra == "docs"
+Requires-Dist: diffusers==0.26.3; extra == "docs"
+Requires-Dist: bitsandbytes==0.42.0; extra == "docs"
 Requires-Dist: rouge_score==0.1.2; extra == "docs"
-Requires-Dist: py7zr==0.21.0; extra == "docs"
-Requires-Dist: fastapi==0.110.2; extra == "docs"
-Requires-Dist: uvicorn==0.29.0; extra == "docs"
-Requires-Dist: python-multipart==0.0.9; extra == "docs"
-Requires-Dist: pydantic==2.7.1; extra == "docs"
+Requires-Dist: py7zr==0.20.6; extra == "docs"
+Requires-Dist: fastapi==0.104.1; extra == "docs"
+Requires-Dist: uvicorn==0.22.0; extra == "docs"
+Requires-Dist: python-multipart==0.0.6; extra == "docs"
+Requires-Dist: gradio==3.41.0; extra == "docs"
+Requires-Dist: pydantic==2.4.2; extra == "docs"
 Requires-Dist: hf-transfer; extra == "docs"
-Requires-Dist: pyngrok==7.1.6; extra == "docs"
+Requires-Dist: pyngrok==7.0.3; extra == "docs"
 Requires-Dist: authlib==1.3.0; extra == "docs"
-Requires-Dist: itsdangerous==2.2.0; extra == "docs"
+Requires-Dist: itsdangerous==2.1.2; extra == "docs"
 Requires-Dist: seqeval==1.2.2; extra == "docs"
-Requires-Dist: httpx==0.27.0; extra == "docs"
-Requires-Dist: pyyaml==6.0.1; extra == "docs"
 Requires-Dist: recommonmark; extra == "docs"
 Requires-Dist: sphinx==3.1.2; extra == "docs"
 Requires-Dist: sphinx-markdown-tables; extra == "docs"
 Requires-Dist: sphinx-rtd-theme==0.4.3; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 
 # 🤗 AutoTrain Advanced
@@ -253,23 +241,14 @@
     conda install -c "nvidia/label/cuda-12.1.0" cuda-nvcc
 
 Once done, you can start the application using:
 
     autotrain app --port 8080 --host 127.0.0.1
 
 
-If you are not fond of UI, you can use AutoTrain Configs to train using command line or simply AutoTrain CLI.
-
-To use config file for training, you can use the following command:
-
-    autotrain --config <path_to_config_file>
-
-
-You can find sample config files in the `configs` directory of this repository.
-
 ## Colabs
 
 | Task | Colab Link |
 | --- | --- |
 | LLM Fine Tuning | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_LLM.ipynb) |
 | DreamBooth Training | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_Dreambooth.ipynb) |
```

### Comparing `autotrain-advanced-0.7.86/README.md` & `autotrain-advanced-0.7.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,14 @@
     conda install -c "nvidia/label/cuda-12.1.0" cuda-nvcc
 
 Once done, you can start the application using:
 
     autotrain app --port 8080 --host 127.0.0.1
 
 
-If you are not fond of UI, you can use AutoTrain Configs to train using command line or simply AutoTrain CLI.
-
-To use config file for training, you can use the following command:
-
-    autotrain --config <path_to_config_file>
-
-
-You can find sample config files in the `configs` directory of this repository.
-
 ## Colabs
 
 | Task | Colab Link |
 | --- | --- |
 | LLM Fine Tuning | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_LLM.ipynb) |
 | DreamBooth Training | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_Dreambooth.ipynb) |
```

### Comparing `autotrain-advanced-0.7.86/setup.py` & `autotrain-advanced-0.7.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,24 +10,16 @@
 DOCLINES = __doc__.split("\n")
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 # get INSTALL_REQUIRES from requirements.txt
-INSTALL_REQUIRES = []
-requirements_path = os.path.join(this_directory, "requirements.txt")
-with open(requirements_path, encoding="utf-8") as f:
-    for line in f:
-        # Exclude 'bitsandbytes' if installing on macOS
-        if "bitsandbytes" in line:
-            line = line.strip() + " ; sys_platform == 'linux'"
-            INSTALL_REQUIRES.append(line.strip())
-        else:
-            INSTALL_REQUIRES.append(line.strip())
+with open(os.path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
+    INSTALL_REQUIRES = f.read().splitlines()
 
 QUALITY_REQUIRE = [
     "black",
     "isort",
     "flake8==3.7.9",
 ]
 
@@ -73,20 +65,20 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords="automl autonlp autotrain huggingface",
     data_files=[
-        ("static", ["src/autotrain/app/static/logo.png"]),
+        ("static", ["src/autotrain/static/logo.png"]),
         (
             "templates",
             [
-                "src/autotrain/app/templates/index.html",
-                "src/autotrain/app/templates/error.html",
-                "src/autotrain/app/templates/duplicate.html",
-                "src/autotrain/app/templates/login.html",
+                "src/autotrain/templates/index.html",
+                "src/autotrain/templates/error.html",
+                "src/autotrain/templates/duplicate.html",
+                "src/autotrain/templates/login.html",
             ],
         ),
     ],
     include_package_data=True,
 )
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/app/db.py` & `autotrain-advanced-0.7.9/src/autotrain/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/app/oauth.py` & `autotrain-advanced-0.7.9/src/autotrain/oauth.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 Taken from: https://github.com/gradio-app/gradio/blob/main/gradio/oauth.py
 """
 
 from __future__ import annotations
 
 import hashlib
 import os
+import random
+import string
 import urllib.parse
 
 import fastapi
-from authlib.integrations.base_client.errors import MismatchingStateError
 from authlib.integrations.starlette_client import OAuth
 from fastapi.responses import RedirectResponse
 from starlette.middleware.sessions import SessionMiddleware
 
 
 OAUTH_CLIENT_ID = os.environ.get("OAUTH_CLIENT_ID")
 OAUTH_CLIENT_SECRET = os.environ.get("OAUTH_CLIENT_SECRET")
 OAUTH_SCOPES = os.environ.get("OAUTH_SCOPES")
 OPENID_PROVIDER_URL = os.environ.get("OPENID_PROVIDER_URL")
+RANDOM_STRING = "".join(random.choices(string.ascii_letters + string.digits, k=20))
 
 
 def attach_oauth(app: fastapi.FastAPI):
     _add_oauth_routes(app)
     # Session Middleware requires a secret key to sign the cookies. Let's use a hash
     # of the OAuth secret key to make it unique to the Space + updated in case OAuth
     # config gets updated.
-    session_secret = OAUTH_CLIENT_SECRET + "-autotrain-v1"
+    session_secret = OAUTH_CLIENT_SECRET + RANDOM_STRING
     # ^ if we change the session cookie format in the future, we can bump the version of the session secret to make
     #   sure cookies are invalidated. Otherwise some users with an old cookie format might get a HTTP 500 error.
     app.add_middleware(
         SessionMiddleware,
         secret_key=hashlib.sha256(session_secret.encode()).hexdigest(),
         https_only=True,
         same_site="none",
@@ -72,33 +74,15 @@
         if redirect_uri.netloc.endswith(".hf.space"):
             redirect_uri_as_str = redirect_uri_as_str.replace("http://", "https://")
         return await oauth.huggingface.authorize_redirect(request, redirect_uri_as_str)  # type: ignore
 
     @app.get("/auth")
     async def auth(request: fastapi.Request) -> RedirectResponse:
         """Endpoint that handles the OAuth callback."""
-        try:
-            oauth_info = await oauth.huggingface.authorize_access_token(request)  # type: ignore
-        except MismatchingStateError:
-            # If the state mismatch, it is very likely that the cookie is corrupted.
-            # There is a bug reported in authlib that causes the token to grow indefinitely if the user tries to login
-            # repeatedly. Since cookies cannot get bigger than 4kb, the token will be truncated at some point - hence
-            # losing the state. A workaround is to delete the cookie and redirect the user to the login page again.
-            # See https://github.com/lepture/authlib/issues/622 for more details.
-            login_uri = "/login/huggingface"
-            if "_target_url" in request.query_params:
-                login_uri += "?" + urllib.parse.urlencode(  # Keep same _target_url as before
-                    {"_target_url": request.query_params["_target_url"]}
-                )
-            for key in list(request.session.keys()):
-                # Delete all keys that are related to the OAuth state
-                if key.startswith("_state_huggingface"):
-                    request.session.pop(key)
-            return RedirectResponse(login_uri)
-
+        oauth_info = await oauth.huggingface.authorize_access_token(request)  # type: ignore
         request.session["oauth_info"] = oauth_info
         return _redirect_to_target(request)
 
 
 def _generate_redirect_uri(request: fastapi.Request) -> str:
     if "_target_url" in request.query_params:
         # if `_target_url` already in query params => respect it
@@ -112,10 +96,10 @@
     if redirect_uri.netloc.endswith(".hf.space"):
         # In Space, FastAPI redirect as http but we want https
         redirect_uri_as_str = redirect_uri_as_str.replace("http://", "https://")
     return redirect_uri_as_str
 
 
 def _redirect_to_target(request: fastapi.Request, default_target: str = "/") -> RedirectResponse:
-    target = request.query_params.get("_target_url", default_target)
-    # target = "https://huggingface.co/spaces/" + os.environ.get("SPACE_ID")
+    # target = request.query_params.get("_target_url", default_target)
+    target = "https://huggingface.co/spaces/" + os.environ.get("SPACE_ID")
     return RedirectResponse(target)
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/app/static/logo.png` & `autotrain-advanced-0.7.9/src/autotrain/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/app/templates/duplicate.html` & `autotrain-advanced-0.7.9/src/autotrain/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/app/templates/error.html` & `autotrain-advanced-0.7.9/src/autotrain/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/app/templates/index.html` & `autotrain-advanced-0.7.9/src/autotrain/templates/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -3,39 +3,35 @@
 
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <script src="https://cdn.tailwindcss.com"></script>
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
   <script>
-    var autotrain_local_value = {{ enable_local }};
-  </script>
-  <script>
     document.addEventListener('DOMContentLoaded', function () {
       document.getElementById('json-error-message').textContent = '';
+      // Function to fetch data and update the textarea
       function fetchDataAndUpdateTextarea() {
         const taskValue = document.getElementById('task').value;
-        const basicParamsRadio = document.getElementById('basic-params-radio');
-
         document.getElementById('params').value = 'Loading...';
-        fetch(`/ui/params/${taskValue}/${basicParamsRadio.checked ? 'basic' : 'full'}`)
+        fetch(`/params/${taskValue}`)
           .then(response => response.json())
           .then(data => {
             document.getElementById('params').value = JSON.stringify(data, null, 2);
           })
           .catch(error => console.error('Error:', error));
       }
       function fetchDataAndUpdateModels() {
         const taskValue = document.getElementById('task').value;
         const baseModelSelect = document.getElementById('base_model');
         const queryParams = new URLSearchParams(window.location.search);
         const customModelsValue = queryParams.get('custom_models');
         console.log(customModelsValue);
 
-        let fetchURL = `/ui/model_choices/${taskValue}`;
+        let fetchURL = `/model_choices/${taskValue}`;
         if (customModelsValue) {
           fetchURL += `?custom_models=${customModelsValue}`;
         }
         baseModelSelect.innerHTML = 'Fetching models...';
         fetch(fetchURL)
           .then(response => response.json())
           .then(data => {
@@ -46,176 +42,103 @@
               option.value = model.id; // Assuming each model has an 'id'
               option.textContent = model.name; // Assuming each model has a 'name'
               baseModelSelect.appendChild(option);
             });
           })
           .catch(error => console.error('Error:', error));
       }
+
+
       // Function to validate JSON in the textarea
       function validateJSON() {
         try {
           JSON.parse(document.getElementById('params').value);
           document.getElementById('error-message').textContent = '';
         } catch (e) {
           document.getElementById('error-message').textContent = 'Invalid parameters: ' + e.message;
         }
       }
       function pollAccelerators() {
-        if (autotrain_local_value === 0) {
-          let statusParagraph = document.getElementById('num_accelerators');
-          statusParagraph.innerText = '';
-          return;
-        }
         // Send a request to the /accelerators endpoint
-        fetch('/ui/accelerators')
+        fetch('/accelerators')
           .then(response => response.json()) // Assuming the response is in JSON format
           .then(data => {
             // Update the paragraph with the number of accelerators
             document.getElementById('num_accelerators').innerText = `Accelerators: ${data.accelerators}`;
           })
           .catch(error => {
             console.error('Error:', error);
             // Update the paragraph to show an error message
             document.getElementById('num_accelerators').innerText = 'Accelerators: Error fetching data';
           });
       }
       function pollModelTrainingStatus() {
         // Send a request to the /is_model_training endpoint
-
-        if (autotrain_local_value === 0) {
-          let statusParagraph = document.getElementById('is_model_training');
-          statusParagraph.innerText = '';
-          return;
-        }
-        fetch('/ui/is_model_training')
+        fetch('/is_model_training')
           .then(response => response.json()) // Assuming the response is in JSON format
           .then(data => {
             // Construct the message to display
-            let message = data.model_training ? 'Running job PID(s): ' + data.pids.join(', ') : 'No running jobs';
+            let message = data.model_training ? 'Running jobs: ' + data.pids.join(', ') : 'No running jobs';
 
             // Update the paragraph with the status of model training
             let statusParagraph = document.getElementById('is_model_training');
             statusParagraph.innerText = message;
-            let stopTrainingButton = document.getElementById('stop-training-button');
-            let startTrainingButton = document.getElementById('start-training-button');
 
             // Change the text color based on the model training status
             if (data.model_training) {
               // Set text color to red if jobs are running
               statusParagraph.style.color = 'red';
-              stopTrainingButton.style.display = 'block';
-              startTrainingButton.style.display = 'none';
             } else {
               // Set text color to green if no jobs are running
               statusParagraph.style.color = 'green';
-              stopTrainingButton.style.display = 'none';
-              startTrainingButton.style.display = 'block';
             }
           })
           .catch(error => {
             console.error('Error:', error);
             // Update the paragraph to show an error message
             let statusParagraph = document.getElementById('is_model_training');
             statusParagraph.innerText = 'Error fetching training status';
             statusParagraph.style.color = 'red'; // Set error message color to red
           });
       }
 
+
       setInterval(pollAccelerators, 10000);
       setInterval(pollModelTrainingStatus, 5000);
 
       // Event listener for dropdown changes
       document.getElementById('task').addEventListener('change', fetchDataAndUpdateTextarea);
       document.getElementById('task').addEventListener('change', fetchDataAndUpdateModels);
-      document.getElementById("basic-params-radio").addEventListener("click", fetchDataAndUpdateTextarea);
-      document.getElementById("full-params-radio").addEventListener("click", fetchDataAndUpdateTextarea);
 
       // Event listener for textarea changes
       document.getElementById('params').addEventListener('blur', validateJSON);
 
       // Initial call to populate the textarea when the page loads
       fetchDataAndUpdateTextarea();
       fetchDataAndUpdateModels();
       pollAccelerators();
       pollModelTrainingStatus();
     });
   </script>
-  <script>
-    document.addEventListener('DOMContentLoaded', function () {
-      var fetchLogsInterval;
-
-      // Function to check the modal's display property and fetch logs if visible
-      function fetchAndDisplayLogs() {
-        var modal = document.getElementById('logs-modal');
-        var displayStyle = window.getComputedStyle(modal).display;
-
-        // Check if the modal display property is 'flex'
-        if (displayStyle === 'flex') {
-          fetchLogs(); // Initial fetch when the modal is opened
-
-          // Clear any existing interval to avoid duplicates
-          clearInterval(fetchLogsInterval);
-
-          // Set up the interval to fetch logs every 5 seconds
-          fetchLogsInterval = setInterval(fetchLogs, 5000);
-        } else {
-          // Clear the interval when the modal is not displayed as 'flex'
-          clearInterval(fetchLogsInterval);
-        }
-      }
-
-      // Function to fetch logs from the server
-      function fetchLogs() {
-        fetch('/ui/logs')
-          .then(response => response.json())
-          .then(data => {
-            var logContainer = document.getElementById('logContent');
-            logContainer.innerHTML = ''; // Clear previous logs
-
-            // Handling the case when logs are only available in local mode or no logs available
-            if (typeof data.logs === 'string') {
-              logContainer.textContent = data.logs;
-            } else {
-              // Assuming data.logs is an array of log entries
-              data.logs.forEach(log => {
-                if (log.trim().length > 0) {
-                  var p = document.createElement('p');
-                  p.textContent = log;
-                  logContainer.appendChild(p); // Appends logs in order received
-                }
-              });
-            }
-          })
-          .catch(error => console.error('Error fetching logs:', error));
-      }
-
-      // Set up an observer to detect when the modal becomes visible or hidden
-      var observer = new MutationObserver(function (mutations) {
-        mutations.forEach(function (mutation) {
-          if (mutation.attributeName === 'class') {
-            fetchAndDisplayLogs();
-          }
-        });
-      });
-
-      var modal = document.getElementById('logs-modal');
-      observer.observe(modal, {
-        attributes: true //configure it to listen to attribute changes
-      });
-    });
-  </script>
 </head>
 
 <body>
-  <header class="bg-white-800 text-white p-2">
+  <header class="bg-white-800 text-white p-4">
     <div class="container mx-auto flex justify-between items-center">
       <img src="/static/logo.png" alt="AutoTrain" , class="w-32">
     </div>
   </header>
-  <div class="form-container max-w-5xl mx-auto p-6 shadow-2xl">
+  <div class="form-container max-w-5xl mx-auto mt-3 p-6 shadow-2xl">
+    <div class="block text-sm font-normal text-gray-700">AutoTrain Advanced is a no-code solution that
+      allows you to train machine learning models in just a few clicks. Please note that you must upload data in correct
+      format for project to be created.
+      For help regarding proper data format and pricing, click <a href="https://hf.co/docs/autotrain" target="_blank"
+        class="text-blue-700">here</a>.
+    </div>
+    <hr class="h-px my-4 bg-gray-200 border-b-2 dark:bg-gray-700">
     <form action="#" method="post" class="grid grid-cols-2 gap-2" enctype="multipart/form-data">
       <div>
         <div class="columns-2 mb-2">
           <div class="form-group">
             <label for="autotrain_user" class="text-sm font-medium text-gray-700">Hugging Face User
               <button type="button" id="autotrain_user_info" class="text-gray-500 hover:text-gray-700">
                 <i class="fas fa-info-circle"></i>
@@ -243,73 +166,65 @@
               <button type="button" id="hardware_info" class="text-gray-500 hover:text-gray-700">
                 <i class="fas fa-info-circle"></i>
               </button>
             </label>
             <select id="hardware" name="hardware"
               class="mt-1 block w-full border border-gray-300 px-3 py-2 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
               {% if enable_local == 1 %}
-              <option value="local-ui">Local/Space</option>
-              {% endif %}
-              {% if enable_local == 0 and enable_ngc == 0 and enable_nvcf == 0 %}
+              <option value="Local">Local/Space</option>
+              {% else %}
               <optgroup label="Hugging Face Spaces">
-                <option value="spaces-a10g-large">1xA10G Large</option>
-                <option value="spaces-a10g-largex2">2xA10G Large</option>
-                <option value="spaces-a10g-largex4">4xA10G Large</option>
-                <option value="spaces-a100-large">A100 Large</option>
-                <option value="spaces-a10g-small">A10G Small</option>
-                <option value="spaces-t4-medium">T4 Medium</option>
-                <option value="spaces-t4-small">T4 Small</option>
-                <option value="spaces-cpu-upgrade">CPU Upgrade</option>
-                <option value="spaces-cpu-basic">CPU (Free)</option>
+                <option value="A10G Large">A10G Large</option>
+                <option value="A100 Large">A100 Large</option>
+                <option value="A10G Small">A10G Small</option>
+                <option value="T4 Medium">T4 Medium</option>
+                <option value="T4 Small">T4 Small</option>
+                <option value="CPU Upgrade">CPU Upgrade</option>
+                <option value="CPU (Free)">CPU (Free)</option>
               </optgroup>
               <optgroup label="Hugging Face Endpoints">
-                <option value="ep-aws-useast1-m">1xA10G</option>
-                <option value="ep-aws-useast1-xl">1xA100</option>
-                <option value="ep-aws-useast1-2xl">2xA100</option>
-                <option value="ep-aws-useast1-4xl">4xA100</option>
-                <option value="ep-aws-useast1-8xl">8xA100</option>
+                <option value="EP US-East-1 1xA10g">1xA10G</option>
+                <option value="EP US-East-1 1xA100">1xA100</option>
+                <option value="EP US-East-1 2xA100">2xA100</option>
+                <option value="EP US-East-1 4xA100">4xA100</option>
+                <option value="EP US-East-1 8xA100">8xA100</option>
               </optgroup>
-              {% endif %}
               {% if enable_ngc == 1 %}
               <optgroup label="NVIDIA DGX Cloud">
-                <option value="dgx-a100">1xA100 DGX</option>
-                <option value="dgx-2a100">2xA100 DGX</option>
-                <option value="dgx-4a100">4xA100 DGX</option>
-                <option value="dgx-8a100">8xA100 DGX</option>
+                <option value="DGX 1xA100">1xA100 DGX</option>
+                <option value="DGX 2xA100">2xA100 DGX</option>
+                <option value="DGX 4xA100">4xA100 DGX</option>
+                <option value="DGX 8xA100">8xA100 DGX</option>
               </optgroup>
               {% endif %}
               {% if enable_nvcf == 1 %}
               <optgroup label="NVIDIA Cloud Functions">
-                <option value="nvcf-l40sx1">1xL40S</option>
-                <option value="nvcf-h100x1">1xH100</option>
-                <option value="nvcf-h100x2">2xH100</option>
-                <option value="nvcf-h100x4">4xH100</option>
-                <option value="nvcf-h100x8">8xH100</option>
+                <option value="NVCF 1xL40">1xL40</option>
+                <option value="NVCF 1xH100">1xH100</option>
               </optgroup>
               {% endif %}
+              {% endif %}
             </select>
           </div>
           <div class="form-group">
             <label for="task" class="text-sm font-medium text-gray-700">Task
               <button type="button" id="task_info" class="text-gray-500 hover:text-gray-700">
                 <i class="fas fa-info-circle"></i>
               </button>
             </label>
             <select id="task" name="task"
               class="mt-1 block w-full border border-gray-300 px-3 py-2 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
               <optgroup label="LLM Finetuning">
                 <option value="llm:sft">LLM SFT</option>
-                <option value="llm:orpo">LLM ORPO</option>
                 <option value="llm:generic">LLM Generic</option>
                 <option value="llm:dpo">LLM DPO</option>
                 <option value="llm:reward">LLM Reward</option>
               </optgroup>
               <optgroup label="Other Text Tasks">
                 <option value="text-classification">Text Classification</option>
-                <option value="text-regression">Text Regression</option>
                 <option value="seq2seq">Sequence To Sequence</option>
                 <option value="token-classification">Token Classification</option>
               </optgroup>
               <optgroup label="Image Tasks">
                 <option value="dreambooth">DreamBooth LoRA</option>
                 <option value="image-classification">Image Classification</option>
               </optgroup>
@@ -326,99 +241,60 @@
               <i class="fas fa-info-circle"></i>
             </button>
           </label>
           <select name="base_model" id="base_model"
             class="mt-1 block w-full border border-gray-300 px-3 py-2 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
           </select>
         </div>
-        <div class="mb-2">
-          <label class="text-sm font-medium text-gray-700">Dataset
-            <button type="button" id="dataset_info" class="text-gray-500 hover:text-gray-700">
-              <i class="fas fa-info-circle"></i>
-            </button>
-          </label>
-          <div class="flex items-center ps-4 border border-gray-300 rounded">
-            <input checked id="upload-dataset-radio" type="radio" value="" name="dataset-radio"
-              class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2">
-            <label for="upload-dataset-radio" class="w-full py-4 ms-2 text-sm font-medium text-gray-900">Upload
-              Dataset</label>
-            <input id="hub-dataset-radio" type="radio" value="" name="dataset-radio"
-              class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2">
-            <label for="hub-dataset-radio" class="w-full py-4 ms-2 text-sm font-medium text-gray-900">Hub
-              Dataset</label>
-          </div>
-        </div>
-        <div id="form-group">
-          <div id="hub-data-tab-content">
-            <div class="form-group">
-              <label for="hub_dataset" class="text-sm font-medium text-gray-700">Hub Dataset
-              </label>
-              <input type="text" name="hub_dataset" id="hub_dataset"
-                class="mt-1 block w-full border border-gray-300 px-3 py-2.5 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
-            </div>
-            <div class="columns-2 mb-2 mt-2">
-              <div class="form-group">
-                <label for="train_split" class="text-sm font-medium text-gray-700">Train split
-                </label>
-                <input type="text" name="train_split" id="train_split"
-                  class="mt-1 block w-full border border-gray-300 px-3 py-2 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
-                <label for="valid_split" class="text-sm font-medium text-gray-700">Valid split (optional)
-                </label>
-                <input type="text" name="valid_split" id="valid_split"
-                  class="mt-1 block w-full border border-gray-300 px-3 py-2 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
-              </div>
-            </div>
+        <div class="form-group mb-2">
+          <div class="mb-4">
+            <ul class="flex flex-wrap -mb-px text-sm font-medium text-center" id="default-tab"
+              data-tabs-toggle="#default-tab-content" role="tablist">
+              <li class="me-2" role="presentation">
+                <button class="inline-block p-4 border-b-2 rounded-t-lg" id="training-data-tab"
+                  data-tabs-target="#training-data" type="button" role="tab" aria-controls="training-data"
+                  aria-selected="false">Training Data</button>
+              </li>
+              <li class="me-2" role="presentation">
+                <button class="inline-block p-4 border-b-2 rounded-t-lg" id="valid-data-tab"
+                  data-tabs-target="#valid-data" type="button" role="tab" aria-controls="valid-data"
+                  aria-selected="false">Validation Data
+                  (optional)</button>
+              </li>
+            </ul>
           </div>
-        </div>
-        <div id="upload-data-tabs">
-          <ul class="flex flex-wrap -mb-px text-sm font-medium text-center" id="upload-data-tab"
-            data-tabs-toggle="#upload-data-tab-content" role="tablist">
-            <li class="me-2" role="presentation">
-              <button class="p-4 hover:text-gray-600 hover:bg-gray-50" id="training-data-tab"
-                data-tabs-target="#training-data" type="button" role="tab" aria-controls="training-data"
-                aria-selected="false">Training Data</button>
-            </li>
-            <li class="me-2" role="presentation">
-              <button class="p-4 hover:text-gray-600 hover:bg-gray-50" id="valid-data-tab"
-                data-tabs-target="#valid-data" type="button" role="tab" aria-controls="valid-data"
-                aria-selected="false">Validation Data
-                (optional)</button>
-            </li>
-          </ul>
-        </div>
-        <div id="form-group">
-          <div id="upload-data-tab-content">
-            <div class="hidden p-4" id="training-data" role="tabpanel" aria-labelledby="training-data-tab">
+          <div id="default-tab-content">
+            <div class="hidden p-4 rounded-lg" id="training-data" role="tabpanel" aria-labelledby="training-data-tab">
               <div class="flex items-center justify-center w-full h-20">
                 <label for="data_files_training"
-                  class="flex flex-col items-center justify-center w-full h-40 cursor-pointer">
+                  class="flex flex-col items-center justify-center w-full h-40cursor-pointer">
                   <div class="flex flex-col items-center justify-center pt-5 pb-6">
                     <svg class="w-8 h-8 mb-4 text-gray-700" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                       fill="none" viewBox="0 0 20 16">
                       <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                         d="M13 13h3a3 3 0 0 0 0-6h-.025A5.56 5.56 0 0 0 16 6.5 5.5 5.5 0 0 0 5.207 5.021C5.137 5.017 5.071 5 5 5a4 4 0 0 0 0 8h2.167M10 15V6m0 0L8 8m2-2 2 2" />
                     </svg>
-                    <p class="text-sm text-gray-700"><span class="font-semibold">Upload Training File(s)
+                    <p class="mb-2 text-sm text-gray-700"><span class="font-semibold">Upload Training File(s)
                         <p class="text-xs text-gray-700" id="file-container-training"></p>
                   </div>
                   <input id="data_files_training" name="data_files_training" type="file" multiple class="hidden" />
                 </label>
               </div>
             </div>
-            <div class="hidden p-4" id="valid-data" role="tabpanel" aria-labelledby="valid-data-tab">
+            <div class="hidden p-4 rounded-lg" id="valid-data" role="tabpanel" aria-labelledby="valid-data-tab">
               <div class="flex items-center justify-center w-full h-20">
                 <label for="data_files_valid"
                   class="flex flex-col items-center justify-center w-full h-40 cursor-pointer">
                   <div class="flex flex-col items-center justify-center pt-5 pb-6">
                     <svg class="w-8 h-8 mb-4 text-gray-700" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                       fill="none" viewBox="0 0 20 16">
                       <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                         d="M13 13h3a3 3 0 0 0 0-6h-.025A5.56 5.56 0 0 0 16 6.5 5.5 5.5 0 0 0 5.207 5.021C5.137 5.017 5.071 5 5 5a4 4 0 0 0 0 8h2.167M10 15V6m0 0L8 8m2-2 2 2" />
                     </svg>
-                    <p class="text-sm text-gray-700"><span class="font-semibold">Upload Validation File(s)
+                    <p class="mb-2 text-sm text-gray-700"><span class="font-semibold">Upload Validation File(s)
                         <p class="text-xs text-gray-700" id="file-container-valid"></p>
                   </div>
                   <input id="data_files_valid" name="data_files_valid" type="file" multiple class="hidden" />
                 </label>
               </div>
             </div>
           </div>
@@ -426,64 +302,38 @@
         <div class="columns-1" id="text_label">
           <label for="column_mapping" class="text-sm font-medium text-gray-700">Column mapping
             <button type="button" id="column_mapping_info" class="text-gray-500 hover:text-gray-700">
               <i class="fas fa-info-circle"></i>
             </button>
           </label>
           <input type="text" name="column_mapping" id="column_mapping"
-            class="mt-2 mb-4 block w-full border border-gray-300 px-3 py-2 rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
+            class="mt-1 block w-full border border-gray-300 px-3 py-2 rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500">
+        </div>
+        <div class="form-actions mt-6">
+          <button type="submit"
+            class="w-full px-4 py-2 text-white bg-blue-600 rounded-md hover:bg-blue-700 focus:outline-none focus:bg-blue-700">Start
+            Training</button>
+        </div>
+        <div class="mt-5">
+          <p class="mb-2 text-sm text-gray-700" id="num_accelerators">Accelerators: Fetching...</p>
         </div>
-
       </div>
       <div>
         <div class="form-group">
-          <div class="text-sm font-normal text-right mb-2">
-            <button type="button" id="button_logs"
-              class="text-gray-900 bg-gray-100 hover:bg-gray-200 font-medium rounded-lg text-xs px-3 py-1.5 text-center inline-flex items-center">
-              <svg class="w-3 h-3 me-1 -ms-1 text-[#626890]" aria-hidden="true" focusable="false" data-prefix="fas"
-                data-icon="terminal" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">
-                <path fill="currentColor"
-                  d="M624 64H304a48 48 0 0 0-48 48v352a48 48 0 0 0 48 48h320a48 48 0 0 0 48-48V112a48 48 0 0 0-48-48zM328 120h72a8 8 0 0 1 0 16h-72a8 8 0 0 1 0-16zm144 0h72a8 8 0 0 1 0 16h-72a8 8 0 0 1 0-16zm-72 48h72a8 8 0 0 1 0 16h-72a8 8 0 0 1 0-16zm-72 0h-72a8 8 0 0 1 0-16h72a8 8 0 0 1 0 16zm0 48h72a8 8 0 0 1 0 16h-72a8 8 0 0 1 0-16zm72 48h72a8 8 0 0 1 0 16h-72a8 8 0 0 1 0-16zm-72 0h-72a8 8 0 0 1 0-16h72a8 8 0 0 1 0 16zm-72 48h320a8 8 0 0 1 8 8v16a8 8 0 0 1-8 8H304a8 8 0 0 1-8-8v-16a8 8 0 0 1 8-8zm0 112v-48h320v48zm-8-128h336v96H312z">
-                </path>
-              </svg>
-              Logs
-            </button>
-          </div>
-          <hr>
           <label for="params" class="text-sm font-medium text-gray-700">Training Parameters (find params to
             copy-paste <a class="text-sm font-medium text-blue-700" href="#">here</a>)
             <button type="button" id="params_info" class="text-gray-500 hover:text-gray-700">
               <i class="fas fa-info-circle"></i>
             </button>
           </label>
-          <div class="flex items-center ps-20">
-            <input checked id="basic-params-radio" type="radio" value="" name="params-radio"
-              class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2">
-            <label for="basic-params-radio" class="w-full py-4 ms-2 text-sm font-medium text-gray-900">Basic</label>
-            <input id="full-params-radio" type="radio" value="" name="params-radio"
-              class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2">
-            <label for="full-params-radio" class="w-full py-4 ms-2 text-sm font-medium text-gray-900">Full</label>
-          </div>
-          <textarea id="params" name="params" rows="20" class="p-2.5 w-full text-sm text-gray-900"
+          <textarea id="params" name="params" rows="25" class="p-2.5 w-full text-sm text-gray-900"
             placeholder="Loading..."></textarea>
         </div>
-      </div>
-      <div class="col-span-2">
-        <button type="submit" id="start-training-button"
-          class="w-full px-4 py-2 text-white bg-blue-600 rounded-md hover:bg-blue-700 focus:outline-none focus:bg-blue-700">Start
-          Training
-        </button>
-        <button type="button" id="stop-training-button"
-          class="hidden w-full px-4 py-2 text-white bg-red-600 rounded-md hover:bg-red-700 focus:outline-none focus:bg-red-700">Stop
-          Training
-        </button>
-        <div class="columns-2 mb-2 mt-2">
-          <p class="text-sm text-gray-700" id="num_accelerators">Accelerators: Fetching...</p>
-          <p class="text-sm text-gray-700 font-bold text-right" id="is_model_training">Fetching training
-            status...
+        <div class="mt-5">
+          <p class="mb-2 text-sm text-gray-700 text-right font-bold" id="is_model_training">Fetching training status...
           </p>
         </div>
       </div>
     </form>
     <div id="json-error-message" style="color: red;"></div>
     <div id="error-message" style="color: red;"></div>
     <div id="success-message" style="color: green;"></div>
@@ -510,36 +360,14 @@
             <button data-modal-hide="confirmation-modal" type="button"
               class="cancel text-white bg-red-600 hover:bg-red-100 focus:ring-4 focus:outline-none focus:ring-red-200 rounded-lg border border-red-200 text-sm font-medium px-5 py-2.5 hover:text-red-900 focus:z-10">No,
               cancel</button>
           </div>
         </div>
       </div>
     </div>
-    <div id="logs-modal" tabindex="-1"
-      class="hidden overflow-y-auto overflow-x-hidden fixed top-0 right-0 left-0 z-50 justify-center items-center w-full md:inset-0 h-[calc(100%-1rem)] max-h-full">
-      <div class="relative p-4 w-full max-w-5xl max-h-full">
-        <div class="relative bg-white rounded-lg shadow-2xl">
-          <button type="button"
-            class="absolute top-3 end-2.5 text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 ms-auto inline-flex justify-center items-center dark:hover:bg-gray-600 dark:hover:text-white"
-            data-modal-hide="logs-modal">
-            <svg class="w-3 h-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 14">
-              <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
-                d="m1 1 6 6m0 0 6 6M7 7l6-6M7 7l-6 6" />
-            </svg>
-            <span class="sr-only">Close</span>
-          </button>
-          <div class="p-4 md:p-5 text-center">
-            <h3 class="mb-5 text-sm font-normal text-gray-800"></h3>
-            <div id="logContent" class="text-xs font-normal text-left overflow-y-auto max-h-[calc(100vh-400px)]">
-              <!-- Logs will be appended here -->
-            </div>
-          </div>
-        </div>
-      </div>
-    </div>
     <div id="final-modal" tabindex="-1"
       class="hidden overflow-y-auto overflow-x-hidden fixed top-0 right-0 left-0 z-50 justify-center items-center w-full md:inset-0 h-[calc(100%-1rem)] max-h-full">
       <div class="relative p-4 w-full max-w-md max-h-full">
         <div class="relative bg-white rounded-lg shadow-2xl">
           <button type="button"
             class="absolute top-3 end-2.5 text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 ms-auto inline-flex justify-center items-center dark:hover:bg-gray-600 dark:hover:text-white"
             data-modal-hide="final-modal">
@@ -551,14 +379,15 @@
           </button>
           <div class="p-4 md:p-5 text-center">
             <h3 class="mb-5 text-sm font-normal text-gray-800"></h3>
           </div>
         </div>
       </div>
     </div>
+
     <div id="help-modal" tabindex="-1"
       class="hidden overflow-y-auto overflow-x-hidden fixed top-0 right-0 left-0 z-50 justify-center items-center w-full md:inset-0 h-[calc(100%-1rem)] max-h-full">
       <div class="relative p-4 w-full max-w-md max-h-full">
         <div class="relative bg-white rounded-lg shadow-2xl">
           <br>
           <button type="button"
             class="absolute top-3 end-2.5 text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 ms-auto inline-flex justify-center items-center dark:hover:bg-gray-600 dark:hover:text-white"
@@ -571,96 +400,33 @@
           </button>
           <div class="p-4 md:p-5 text-center">
             <h3 class="mb-5 text-sm font-normal text-gray-800"></h3>
           </div>
         </div>
       </div>
     </div>
-    <hr class="h-px my-1 bg-gray-200 border-b-2 dark:bg-gray-700">
-    <div class="block text-sm font-normal text-gray-700 text-center"><a href="https://hf.co/autotrain" target="_blank"
-        class="text-gray-700">Powered by 🤗 Hugging Face</a>.
-    </div>
-    <div class="block text-sm font-normal text-gray-700 text-center"><a href="https://hf.co/docs/autotrain"
-        target="_blank" class="text-blue-600">Docs</a> | <a href="https://github.com/huggingface/autotrain-advanced"
-        target="_blank" class="text-blue-600">GitHub</a>
-    </div>
-    <div class="block text-xs font-normal text-gray-400 text-center">{{version}}
-    </div>
   </div>
   </div>
 </body>
-<script>
-  window.addEventListener("load", function () {
-    // Get references to the radio buttons and the tab content elements
-    const hubDatasetRadio = document.getElementById("hub-dataset-radio");
-    const uploadDatasetRadio = document.getElementById("upload-dataset-radio");
-    const uploadDataTabContent = document.getElementById("upload-data-tab-content");
-    const hubDataTabContent = document.getElementById("hub-data-tab-content");
-    const uploadDataTabs = document.getElementById("upload-data-tabs");
-
-    // Function to handle radio button click events
-    function handleRadioButtonClick() {
-      if (hubDatasetRadio.checked) {
-        uploadDataTabContent.style.display = "none";
-        uploadDataTabs.style.display = "none";
-        hubDataTabContent.style.display = "block";
-      } else if (uploadDatasetRadio.checked) {
-        uploadDataTabContent.style.display = "block";
-        uploadDataTabs.style.display = "block";
-        hubDataTabContent.style.display = "none";
-      }
-    }
 
-    // Attach event listeners to radio buttons
-    hubDatasetRadio.addEventListener("click", handleRadioButtonClick);
-    uploadDatasetRadio.addEventListener("click", handleRadioButtonClick);
-
-    // Trigger initial click event to ensure correct display on page load
-    uploadDatasetRadio.click();
-  });
-</script>
-<script>
-  window.addEventListener('load', function () {
-    const stopTrainingButton = document.getElementById('stop-training-button');
-    const loadingSpinner = document.getElementById('loadingSpinner');
-
-    stopTrainingButton.addEventListener('click', function () {
-      loadingSpinner.classList.remove('hidden');
-
-      fetch('/ui/stop_training', {
-        method: 'GET'
-      })
-        .then(response => response.text())
-        .then(data => {
-          console.log(data);
-          loadingSpinner.classList.add('hidden');
-        })
-        .catch(error => {
-          console.error('Error:', error);
-          loadingSpinner.classList.add('hidden');
-        });
-    });
-  });
-</script>
 <script>
   async function openHelpModal(contentId) {
     const modal = document.getElementById('help-modal');
     var helpModalContent = document.querySelector('#help-modal .text-center');
 
     try {
-      const response = await fetch(`/ui/help/${contentId}`);
+      const response = await fetch(`/help/${contentId}`);
       if (!response.ok) {
         throw new Error('Network response was not ok');
       }
       const data = await response.json();
 
       helpModalContent.innerHTML = data.message;
 
       modal.classList.remove('hidden');
-      modal.classList.add('flex');
     } catch (error) {
       console.error('There has been a problem with your fetch operation:', error);
     }
   }
 
   document.getElementById('autotrain_user_info').addEventListener('click', function () {
     openHelpModal('autotrain_user_info');
@@ -692,92 +458,61 @@
 
   // Close modal functionality
   document.querySelector('[data-modal-hide="help-modal"]').addEventListener('click', function () {
     document.getElementById('help-modal').classList.add('hidden');
   });
 
 </script>
+
 <script>
   document.addEventListener('DOMContentLoaded', function () {
     var taskSelect = document.getElementById('task');
     var columnMappingInput = document.getElementById('column_mapping');
 
     // Function to update the placeholder based on the selected task
     function updateColumnMapping() {
       var selectedTask = taskSelect.value;
       var placeholderText = '';
       var isDisabled = false;
 
       switch (selectedTask) {
         case 'llm:sft':
           placeholderText = '{"text": "text"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = true;
           break;
         case 'llm:generic':
           placeholderText = '{"text": "text"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = true;
           break;
         case 'llm:dpo':
           placeholderText = '{"prompt": "prompt", "text": "text", "rejected_text": "rejected_text"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = true;
           break;
         case 'llm:reward':
           placeholderText = '{"text": "text", "rejected_text": "rejected_text"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = true;
-          break;
-        case 'llm:orpo':
-          placeholderText = '{"prompt": "prompt", "text": "text", "rejected_text": "rejected_text"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = true;
           break;
         case 'text-classification':
           placeholderText = '{"text": "text", "label": "target"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = false;
-          break;
-        case 'text-regression':
-          placeholderText = '{"text": "text", "label": "target"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = false;
           break;
         case 'token-classification':
           placeholderText = '{"text": "tokens", "label": "tags"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = false;
           break;
         case 'seq2seq':
           placeholderText = '{"text": "text", "label": "target"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = false;
           break;
         case 'dreambooth':
           placeholderText = '{"image": "image"}';
           isDisabled = true;
-          document.getElementById("upload-dataset-radio").checked = true;
-          document.getElementById("hub-dataset-radio").disabled = true;
-          document.getElementById("upload-dataset-radio").click();
           break;
         case 'image-classification':
           placeholderText = '{"image": "image", "label": "label"}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = false;
+          isDisabled = true;
           break;
         case 'tabular:classification':
           placeholderText = '{"id": "id", "label": ["target"]}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = false;
           break;
         case 'tabular:regression':
           placeholderText = '{"id": "id", "label": ["target"]}';
-          document.getElementById("hub-dataset-radio").disabled = false;
-          document.getElementById("valid_split").disabled = false;
           break;
         default:
           placeholderText = 'Enter column mapping...';
       }
 
       columnMappingInput.value = placeholderText;
       columnMappingInput.disabled = isDisabled;
@@ -786,14 +521,15 @@
     taskSelect.addEventListener('change', function () {
       updateColumnMapping();
     });
     updateColumnMapping();
   });
 
 </script>
+
 <script>
   document.addEventListener('DOMContentLoaded', function () {
     const taskSelect = document.getElementById('task');
     const validDataTab = document.getElementById('valid-data-tab');
 
     function toggleValidationTab() {
       const task = taskSelect.value;
@@ -809,25 +545,26 @@
     toggleValidationTab();
 
     // Add event listener for changes in the task dropdown
     taskSelect.addEventListener('change', toggleValidationTab);
   });
 
 </script>
+
 <script>
   // Function to hide all tab contents
   function hideAllTabContents() {
-    document.querySelectorAll('#upload-data-tab-content > div').forEach(function (tabContent) {
+    document.querySelectorAll('#default-tab-content > div').forEach(function (tabContent) {
       tabContent.classList.add('hidden');
     });
   }
 
   // Function to deactivate all tabs
   function deactivateAllTabs() {
-    document.querySelectorAll('#upload-data-tab > li > button').forEach(function (tabButton) {
+    document.querySelectorAll('#default-tab > li > button').forEach(function (tabButton) {
       tabButton.classList.remove('border-b-2', 'rounded-t-lg');
       tabButton.setAttribute('aria-selected', 'false');
     });
   }
 
   // Function to activate a tab
   function activateTab(tabButton, tabContent) {
@@ -850,14 +587,15 @@
     activateTab(this, document.querySelector('#valid-data'));
   });
 
   // Initialize by showing the first tab
   activateTab(document.querySelector('#training-data-tab'), document.querySelector('#training-data'));
 
 </script>
+
 <script type="module">
   import { uploadFiles, createRepo } from 'https://cdn.jsdelivr.net/npm/@huggingface/hub@0.12.1/+esm'
   document.addEventListener("DOMContentLoaded", function () {
     document.getElementById('success-message').textContent = '';
     document.getElementById('error-message').textContent = '';
     // Select the form element
     const form = document.querySelector('form');
@@ -881,26 +619,14 @@
     // Function to show the modal
     function showModal() {
       const modal = document.getElementById('confirmation-modal');
       modal.classList.add('flex');
       modal.classList.remove('hidden');
     }
 
-    function showLogsModal() {
-      const modal = document.getElementById('logs-modal');
-      modal.classList.add('flex');
-      modal.classList.remove('hidden');
-    }
-
-    function hideLogsModal() {
-      const modal = document.getElementById('logs-modal');
-      modal.classList.remove('flex');
-      modal.classList.add('hidden');
-    }
-
     // Function to hide the modal
     function hideModal() {
       const modal = document.getElementById('confirmation-modal');
       modal.classList.remove('flex');
       modal.classList.add('hidden');
     }
 
@@ -923,35 +649,69 @@
 
       // Show the loading spinner
       loadingSpinner.classList.remove('hidden');
 
       // Get form data
       const formData = new FormData(form);
 
+      // Extract necessary data for Hugging Face
+      const token = formData.get('token');
+      const username = formData.get('username');
+      const project_name = formData.get('project_name');
+      const train_files = formData.getAll('data_files_training');
+      const valid_files = formData.getAll('data_files_valid');
+
+      // Prepare credentials and repo information for Hugging Face
+      const credentials = { accessToken: token };
+      const repo = { type: 'model', name: `${username}/autotrain-data-${project_name}` };
+
+      // Upload files to Hugging Face Hub
+      // MODIFY for training and valid files both
+      // try {
+      //     await createRepo({
+      //       repo: repo,
+      //       credentials: credentials,
+      //       private: true,
+      //     });
+      //     for (let file of files) {
+      //         await uploadFiles({
+      //             repo,
+      //             credentials,
+      //             files: [{
+      //                 path: file.name,
+      //                 content: file
+      //             }],
+      //         });
+      //     }
+      //     console.log('Files uploaded to Hugging Face Hub successfully');
+      //     document.getElementById('success-message').textContent = 'Uploaded files to Hugging Face Hub successfully';
+      // } catch (error) {
+      //     console.error('Error uploading files to Hugging Face Hub:', error);
+      //     // Hide the loading spinner and return to stop further processing
+      //     document.getElementById('error-message').textContent = 'Error uploading files to Hugging Face Hub: ' + error.message;
+      //     loadingSpinner.classList.add('hidden');
+      //     return;
+      // }
+
       // Send request to internal API
       const xhr = new XMLHttpRequest();
-      xhr.open('POST', '/ui/create_project', true);
+      xhr.open('POST', '/create_project', true); // Replace '/create_project' with your FastAPI endpoint URL
 
       // Handle the response
       xhr.onload = function () {
         // Hide the loading spinner
         loadingSpinner.classList.add('hidden');
         var finalModalContent = document.querySelector('#final-modal .text-center');
 
         if (xhr.status === 200) {
           console.log('Response:', xhr.responseText);
           var responseObj = JSON.parse(xhr.responseText);
           var monitorURL = responseObj.monitor_url;
-          if (monitorURL.startsWith('http')) {
-            finalModalContent.innerHTML = '<p>Success!</p>' +
-              '<p>You can check the progress of your training here: <a href="' + monitorURL + '" target="_blank">' + monitorURL + '</a></p>';
-          } else {
-            finalModalContent.innerHTML = '<p>Success!</p>' +
-              '<p>' + monitorURL + '</p>';
-          }
+          finalModalContent.innerHTML = '<p>Success!</p>' +
+            '<p>You can check the progress of your training here: <a href="' + monitorURL + '" target="_blank">' + monitorURL + '</a></p>';
 
           showFinalModal();
         } else {
           // Error logic here
           finalModalContent.innerHTML = '<p>Error: ' + xhr.status + ' ' + xhr.statusText + '</p>' + '<p> Please check the logs for more information.</p>';
           console.error('Error:', xhr.status, xhr.statusText);
           showFinalModal();
@@ -963,22 +723,17 @@
     });
     document.querySelector('#confirmation-modal .cancel').addEventListener('click', function () {
       hideModal();
     });
     document.querySelector('#final-modal button').addEventListener('click', function () {
       hideFinalModal();
     });
-    document.querySelector('#button_logs').addEventListener('click', function () {
-      showLogsModal();
-    });
-    document.querySelector('[data-modal-hide="logs-modal"]').addEventListener('click', function () {
-      hideLogsModal();
-    });
   });
 </script>
+
 <script>
   document.getElementById('data_files_training').addEventListener('change', function () {
     var fileContainer = document.getElementById('file-container-training');
     var files = this.files;
     var fileText = '';
 
     for (var i = 0; i < files.length; i++) {
@@ -1024,8 +779,8 @@
     document.getElementById('project_name').value = randomName;
   }
 
   // Call the function on page load
   window.onload = setRandomProjectName;
 </script>
 
-</html>
+</html>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,71 +1,58 @@
 class="w-32">
+AutoTrain Advanced is a no-code solution that allows you to train machine
+learning models in just a few clicks. Please note that you must upload data in
+correct format for project to be created. For help regarding proper data format
+and pricing, click _h_e_r_e.
+===============================================================================
 Hugging Face User
 id="autotrain_user" class="mt-1 block w-full border border-gray-300 px-3 py-
 2 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:
 border-indigo-500"> {% for user in valid_users %}
 {{ user }}
 {% endfor %}
 Project name[project_name        ]
 {% if enable_local == 1 %}
 Local/Space
-{% endif %} {% if enable_local == 0 and enable_ngc == 0 and enable_nvcf == 0 %}
-1xA10G Large
-2xA10G Large
-4xA10G Large
+{% else %}
+A10G Large
 A100 Large
 A10G Small
 T4 Medium
 T4 Small
 CPU Upgrade
 CPU (Free)
 1xA10G
 1xA100
 2xA100
 4xA100
 8xA100
-{% endif %} {% if enable_ngc == 1 %}
+{% if enable_ngc == 1 %}
 1xA100 DGX
 2xA100 DGX
 4xA100 DGX
 8xA100 DGX
 {% endif %} {% if enable_nvcf == 1 %}
-1xL40S
+1xL40
 1xH100
-2xH100
-4xH100
-8xH100
-{% endif %}
-Task[One of: LLM SFT/LLM ORPO/LLM Generic/LLM DPO/LLM Reward/Text
-Classification/Text Regression/Sequence To Sequence/Token Classification/
-DreamBooth LoRA/Image Classification/Tabular Classification/Tabular Regression]
-Dataset
-#Upload Dataset oHub Dataset
-Hub Dataset[hub_dataset         ]
-Train split [train_split         ]Valid split (optional)[valid_split         ]
+{% endif %} {% endif %}
+Task[One of: LLM SFT/LLM Generic/LLM DPO/LLM Reward/Text Classification/
+Sequence To Sequence/Token Classification/DreamBooth LoRA/Image Classification/
+Tabular Classification/Tabular Regression]
     * Training Data
     * Validation Data (optional)
 Upload Training File(s)
 [File]
 Upload Validation File(s)
 [File]
 Column mapping[column_mapping      ]
-Logs
-===============================================================================
-Training Parameters (find params to copy-paste _h_e_r_e)
-#Basic oFull
-Start Training Stop Training
+Start Training
 Accelerators: Fetching...
 Fetching training status...
 Loading...
 ******** AAuuttooTTrraaiinn iiss aa ppaaiidd ooffffeerriinngg aanndd yyoouu wwiillll bbee cchhaarrggeedd ffoorr tthhiiss aaccttiioonn.. YYoouu
 ccaann iiggnnoorree tthhiiss mmeessssaaggee iiff yyoouu aarree rruunnnniinngg AAuuttooTTrraaiinn oonn aa llooccaall hhaarrddwwaarree.. AArree
 yyoouu ssuurree yyoouu wwaanntt ttoo ccoonnttiinnuuee?? ********
 Yes, I'm sure No, cancel
 Close
-Close
 
 Close
-===============================================================================
-_P_o_w_e_r_e_d_ _b_y_ _🤗_ _H_u_g_g_i_n_g_ _F_a_c_e.
-_D_o_c_s | _G_i_t_H_u_b
-{{version}}
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/app/training_api.py` & `autotrain-advanced-0.7.9/src/autotrain/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import asyncio
 import os
+import signal
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
 
 from autotrain import logger
-from autotrain.app.db import AutoTrainDB
-from autotrain.app.utils import get_running_jobs, kill_process_by_pid
-from autotrain.utils import run_training
+from autotrain.app_utils import get_running_jobs, run_training
+from autotrain.db import AutoTrainDB
 
 
+log_file_path = "/tmp/app.log"
+
 HF_TOKEN = os.environ.get("HF_TOKEN")
 AUTOTRAIN_USERNAME = os.environ.get("AUTOTRAIN_USERNAME")
 PROJECT_NAME = os.environ.get("PROJECT_NAME")
 TASK_ID = int(os.environ.get("TASK_ID"))
 PARAMS = os.environ.get("PARAMS")
 DATA_PATH = os.environ.get("DATA_PATH")
 MODEL = os.environ.get("MODEL")
+OUTPUT_MODEL_REPO = os.environ.get("OUTPUT_MODEL_REPO")
 DB = AutoTrainDB("autotrain.db")
 
 
 class BackgroundRunner:
     async def run_main(self):
         while True:
             running_jobs = get_running_jobs(DB)
             if not running_jobs:
                 logger.info("No running jobs found. Shutting down the server.")
-                kill_process_by_pid(os.getpid())
+                os.kill(os.getpid(), signal.SIGINT)
+            else:
+                logger.info("No running jobs found.")
             await asyncio.sleep(30)
 
 
 runner = BackgroundRunner()
 
 
 @asynccontextmanager
@@ -44,14 +49,15 @@
 
 api = FastAPI(lifespan=lifespan)
 logger.info(f"AUTOTRAIN_USERNAME: {AUTOTRAIN_USERNAME}")
 logger.info(f"PROJECT_NAME: {PROJECT_NAME}")
 logger.info(f"TASK_ID: {TASK_ID}")
 logger.info(f"DATA_PATH: {DATA_PATH}")
 logger.info(f"MODEL: {MODEL}")
+logger.info(f"OUTPUT_MODEL_REPO: {OUTPUT_MODEL_REPO}")
 
 
 @api.get("/")
 async def root():
     return "Your model is being trained..."
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,10 +44,10 @@
         self.port = port
         self.host = host
         self.task = task
 
     def run(self):
         import uvicorn
 
-        from autotrain.app.training_api import api
+        from autotrain.api import api
 
         uvicorn.run(api, host=self.host, port=self.port)
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_dreambooth.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,19 +265,24 @@
             {
                 "arg": "--xl",
                 "help": "XL",
                 "required": False,
                 "action": "store_true",
             },
             {
-                "arg": "--mixed-precision",
-                "help": "mixed precision, fp16, bf16, none",
+                "arg": "--fp16",
+                "help": "FP16",
                 "required": False,
-                "type": str,
-                "default": "none",
+                "action": "store_true",
+            },
+            {
+                "arg": "--bf16",
+                "help": "BF16",
+                "required": False,
+                "action": "store_true",
             },
             {
                 "arg": "--validation-prompt",
                 "help": "Validation prompt",
                 "required": False,
                 "type": str,
             },
@@ -311,15 +316,15 @@
                 "arg": "--logging",
                 "help": "Logging using tensorboard",
                 "required": False,
                 "action": "store_true",
             },
         ]
 
-        arg_list = common_args() + arg_list
+        arg_list.extend(common_args())
         run_dreambooth_parser = parser.add_parser("dreambooth", description="✨ Run AutoTrain DreamBooth Training")
         for arg in arg_list:
             if "action" in arg:
                 run_dreambooth_parser.add_argument(
                     arg["arg"],
                     help=arg["help"],
                     required=arg.get("required", False),
@@ -329,65 +334,69 @@
             else:
                 run_dreambooth_parser.add_argument(
                     arg["arg"],
                     help=arg["help"],
                     required=arg.get("required", False),
                     type=arg.get("type"),
                     default=arg.get("default"),
-                    choices=arg.get("choices"),
                 )
         run_dreambooth_parser.set_defaults(func=run_dreambooth_command_factory)
 
     def __init__(self, args):
         self.args = args
+        logger.info(self.args)
 
         store_true_arg_names = [
             "center_crop",
             "train_text_encoder",
             "disable_gradient_checkpointing",
             "scale_lr",
             "use_8bit_adam",
             "allow_tf32",
             "xformers",
             "pre_compute_text_embeddings",
             "text_encoder_use_attention_mask",
             "xl",
+            "fp16",
+            "bf16",
             "push_to_hub",
             "logging",
             "prior_preservation",
         ]
 
         for arg_name in store_true_arg_names:
             if getattr(self.args, arg_name) is None:
                 setattr(self.args, arg_name, False)
 
+        if self.args.fp16 and self.args.bf16:
+            raise ValueError("❌ Please choose either FP16 or BF16")
+
         # check if self.args.image_path is a directory with images
         if not os.path.isdir(self.args.image_path):
             raise ValueError("❌ Please specify a valid image directory")
 
         # count the number of images in the directory. valid images are .jpg, .jpeg, .png
         num_images = count_images(self.args.image_path)
         if num_images == 0:
             raise ValueError("❌ Please specify a valid image directory")
 
         if self.args.push_to_hub:
-            if self.args.username is None:
-                raise ValueError("❌ Please specify a username to push to hub")
+            if self.args.repo_id is None and self.args.username is None:
+                raise ValueError("❌ Please specify a username or repo id to push to hub")
 
         if self.args.model in XL_MODELS:
             self.args.xl = True
 
         if self.args.backend.startswith("spaces") or self.args.backend.startswith("ep-"):
             if not self.args.push_to_hub:
                 raise ValueError("Push to hub must be specified for spaces backend")
-            if self.args.username is None:
-                raise ValueError("Username must be specified for spaces backend")
+            if self.args.username is None and self.args.repo_id is None:
+                raise ValueError("Repo id or username must be specified for spaces backend")
             if self.args.token is None:
                 raise ValueError("Token must be specified for spaces backend")
 
     def run(self):
         logger.info("Running DreamBooth Training")
         params = DreamBoothTrainingParams(**vars(self.args))
         params = dreambooth_munge_data(params, local=self.args.backend.startswith("local"))
         project = AutoTrainProject(params=params, backend=self.args.backend)
-        job_id = project.create()
-        logger.info(f"Job ID: {job_id}")
+        _ = project.create()
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_image_classification.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,85 +28,91 @@
                 "help": "Target column to use",
                 "required": False,
                 "type": str,
                 "default": "target",
             },
             {
                 "arg": "--warmup-ratio",
-                "help": "Define the proportion of training to be dedicated to a linear warmup where learning rate gradually increases. This can help in stabilizing the training process early on. Default ratio is 0.1.",
+                "help": "Warmup proportion to use",
                 "required": False,
                 "type": float,
                 "default": 0.1,
             },
             {
                 "arg": "--optimizer",
-                "help": "Choose the optimizer algorithm for training the model. Different optimizers can affect the training speed and model performance. 'adamw_torch' is used by default.",
+                "help": "Optimizer to use",
                 "required": False,
                 "type": str,
                 "default": "adamw_torch",
             },
             {
                 "arg": "--scheduler",
-                "help": "Select the learning rate scheduler to adjust the learning rate based on the number of epochs. 'linear' decreases the learning rate linearly from the initial lr set. Default is 'linear'. Try 'cosine' for a cosine annealing schedule.",
+                "help": "Scheduler to use",
                 "required": False,
                 "type": str,
                 "default": "linear",
             },
             {
                 "arg": "--weight-decay",
-                "help": "Set the weight decay rate to apply for regularization. Helps in preventing the model from overfitting by penalizing large weights. Default is 0.0, meaning no weight decay is applied.",
+                "help": "Weight decay to use",
                 "required": False,
                 "type": float,
                 "default": 0.0,
             },
             {
                 "arg": "--max-grad-norm",
-                "help": "Specify the maximum norm of the gradients for gradient clipping. Gradient clipping is used to prevent the exploding gradient problem in deep neural networks. Default is 1.0.",
+                "help": "Max gradient norm to use",
                 "required": False,
                 "type": float,
                 "default": 1.0,
             },
             {
                 "arg": "--logging-steps",
-                "help": "Determine how often to log training progress. Set this to the number of steps between each log output. -1 determines logging steps automatically. Default is -1.",
+                "help": "Logging steps to use",
                 "required": False,
                 "type": int,
                 "default": -1,
             },
             {
                 "arg": "--evaluation-strategy",
-                "help": "Specify how often to evaluate the model performance. Options include 'no', 'steps', 'epoch'. 'epoch' evaluates at the end of each training epoch by default.",
+                "help": "Evaluation strategy to use",
                 "required": False,
                 "type": str,
                 "default": "epoch",
-                "choices": ["steps", "epoch", "no"],
             },
             {
                 "arg": "--save-total-limit",
-                "help": "Limit the total number of model checkpoints to save. Helps manage disk space by retaining only the most recent checkpoints. Default is to save only the latest one.",
+                "help": "Save total limit to use",
                 "required": False,
                 "type": int,
                 "default": 1,
             },
             {
+                "arg": "--save-strategy",
+                "help": "Save strategy to use",
+                "required": False,
+                "type": str,
+                "default": "epoch",
+            },
+            {
                 "arg": "--auto-find-batch-size",
-                "help": "Enable automatic batch size determination based on your hardware capabilities. When set, it tries to find the largest batch size that fits in memory.",
+                "help": "Auto find batch size True/False",
                 "required": False,
                 "action": "store_true",
             },
             {
                 "arg": "--mixed-precision",
-                "help": "Choose the precision mode for training to optimize performance and memory usage. Options are 'fp16', 'bf16', or None for default precision. Default is None.",
+                "help": "fp16, bf16, or None",
                 "required": False,
                 "type": str,
                 "default": None,
                 "choices": ["fp16", "bf16", None],
             },
         ]
-        arg_list = common_args() + arg_list
+        arg_list.extend(common_args())
         run_text_classification_parser = parser.add_parser(
             "image-classification", description="✨ Run AutoTrain Image Classification"
         )
         for arg in arg_list:
             if "action" in arg:
                 run_text_classification_parser.add_argument(
                     arg["arg"],
@@ -118,15 +124,14 @@
             else:
                 run_text_classification_parser.add_argument(
                     arg["arg"],
                     help=arg["help"],
                     required=arg.get("required", False),
                     type=arg.get("type"),
                     default=arg.get("default"),
-                    choices=arg.get("choices"),
                 )
         run_text_classification_parser.set_defaults(func=run_image_classification_command_factory)
 
     def __init__(self, args):
         self.args = args
 
         store_true_arg_names = [
@@ -144,28 +149,27 @@
             if self.args.project_name is None:
                 raise ValueError("Project name must be specified")
             if self.args.data_path is None:
                 raise ValueError("Data path must be specified")
             if self.args.model is None:
                 raise ValueError("Model must be specified")
             if self.args.push_to_hub:
-                if self.args.username is None:
-                    raise ValueError("Username must be specified for push to hub")
+                if self.args.repo_id is None:
+                    raise ValueError("Repo id must be specified for push to hub")
         else:
             raise ValueError("Must specify --train, --deploy or --inference")
 
         if self.args.backend.startswith("spaces") or self.args.backend.startswith("ep-"):
             if not self.args.push_to_hub:
                 raise ValueError("Push to hub must be specified for spaces backend")
-            if self.args.username is None:
-                raise ValueError("Username must be specified for spaces backend")
+            if self.args.username is None and self.args.repo_id is None:
+                raise ValueError("Repo id or username must be specified for spaces backend")
             if self.args.token is None:
                 raise ValueError("Token must be specified for spaces backend")
 
     def run(self):
         logger.info("Running Text Classification")
         if self.args.train:
             params = ImageClassificationParams(**vars(self.args))
             params = img_clf_munge_data(params, local=self.args.backend.startswith("local"))
             project = AutoTrainProject(params=params, backend=self.args.backend)
-            job_id = project.create()
-            logger.info(f"Job ID: {job_id}")
+            _ = project.create()
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_llm.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,215 +14,202 @@
 
 class RunAutoTrainLLMCommand(BaseAutoTrainCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         arg_list = [
             {
                 "arg": "--text_column",
-                "help": "Specify the dataset column to use for text data. This parameter is essential for models processing textual information. Default is 'text'.",
+                "help": "Text column to use",
                 "required": False,
                 "type": str,
                 "default": "text",
                 "alias": ["--text-column"],
             },
             {
                 "arg": "--rejected_text_column",
-                "help": "Define the column to use for storing rejected text entries, which are typically entries that do not meet certain criteria for processing. Default is 'rejected'. Used only for orpo, dpo and reward trainerss",
+                "help": "Rejected text column to use",
                 "required": False,
                 "type": str,
                 "default": "rejected",
                 "alias": ["--rejected-text-column"],
             },
             {
-                "arg": "--prompt_text_column",
-                "help": "Identify the column that contains prompt text for tasks requiring contextual inputs, such as conversation or completion generation. Default is 'prompt'. Used only for dpo trainer",
+                "arg": "--prompt-text-column",
+                "help": "Prompt text column to use",
                 "required": False,
                 "type": str,
                 "default": "prompt",
                 "alias": ["--prompt-text-column"],
             },
             {
                 "arg": "--model-ref",
                 "help": "Reference model to use for DPO when not using PEFT",
                 "required": False,
                 "type": str,
-                "alias": ["--model-ref"],
             },
             {
                 "arg": "--warmup_ratio",
-                "help": "Set the proportion of training allocated to warming up the learning rate, which can enhance model stability and performance at the start of training. Default is 0.1",
+                "help": "Warmup proportion to use",
                 "required": False,
                 "type": float,
                 "default": 0.1,
                 "alias": ["--warmup-ratio"],
             },
             {
                 "arg": "--optimizer",
-                "help": "Choose the optimizer algorithm for training the model. Different optimizers can affect the training speed and model performance. 'adamw_torch' is used by default.",
+                "help": "Optimizer to use",
                 "required": False,
                 "type": str,
                 "default": "adamw_torch",
             },
             {
                 "arg": "--scheduler",
-                "help": "Select the learning rate scheduler to adjust the learning rate based on the number of epochs. 'linear' decreases the learning rate linearly from the initial lr set. Default is 'linear'. Try 'cosine' for a cosine annealing schedule.",
+                "help": "Scheduler to use",
                 "required": False,
                 "type": str,
                 "default": "linear",
             },
             {
                 "arg": "--weight_decay",
-                "help": "Define the weight decay rate for regularization, which helps prevent overfitting by penalizing larger weights. Default is 0.0",
+                "help": "Weight decay to use",
                 "required": False,
                 "type": float,
                 "default": 0.0,
                 "alias": ["--weight-decay"],
             },
             {
                 "arg": "--max_grad_norm",
-                "help": "Set the maximum norm for gradient clipping, which is critical for preventing gradients from exploding during backpropagation. Default is 1.0.",
+                "help": "Max gradient norm to use",
                 "required": False,
                 "type": float,
                 "default": 1.0,
                 "alias": ["--max-grad-norm"],
             },
             {
                 "arg": "--add_eos_token",
-                "help": "Toggle whether to automatically add an End Of Sentence (EOS) token at the end of texts, which can be critical for certain types of models like language models. Only used for `default` trainer",
+                "help": "Add EOS token to use",
                 "required": False,
                 "action": "store_true",
                 "alias": ["--add-eos-token"],
             },
             {
                 "arg": "--block_size",
-                "help": "Specify the block size for processing sequences. This is maximum sequence length or length of one block of text. Setting to -1 determines block size automatically. Default is -1.",
+                "help": "Block size to use",
                 "required": False,
                 "type": str,
                 "default": "-1",
                 "alias": ["--block-size"],
             },
             {
                 "arg": "--peft",
-                "help": "Enable LoRA-PEFT",
+                "help": "Use PEFT",
                 "required": False,
                 "action": "store_true",
                 "alias": ["--use-peft"],
             },
             {
                 "arg": "--lora_r",
-                "help": "Set the 'r' parameter for Low-Rank Adaptation (LoRA). Default is 16.",
+                "help": "Lora r to use",
                 "required": False,
                 "type": int,
                 "default": 16,
                 "alias": ["--lora-r"],
             },
             {
                 "arg": "--lora_alpha",
-                "help": "Specify the 'alpha' parameter for LoRA. Default is 32.",
+                "help": "Lora alpha to use",
                 "required": False,
                 "type": int,
                 "default": 32,
                 "alias": ["--lora-alpha"],
             },
             {
                 "arg": "--lora_dropout",
-                "help": "Set the dropout rate within the LoRA layers to help prevent overfitting during adaptation. Default is 0.05.",
+                "help": "Lora dropout to use",
                 "required": False,
                 "type": float,
                 "default": 0.05,
                 "alias": ["--lora-dropout"],
             },
             {
                 "arg": "--logging_steps",
-                "help": "Determine how often to log training progress in terms of steps. Setting it to '-1' determines logging steps automatically.",
+                "help": "Logging steps to use",
                 "required": False,
                 "type": int,
                 "default": -1,
                 "alias": ["--logging-steps"],
             },
             {
                 "arg": "--evaluation_strategy",
-                "help": "Choose how frequently to evaluate the model's performance, with 'epoch' as the default, meaning at the end of each training epoch",
+                "help": "Evaluation strategy to use",
                 "required": False,
                 "type": str,
                 "default": "epoch",
                 "alias": ["--evaluation-strategy"],
-                "choices": ["epoch", "steps", "no"],
             },
             {
                 "arg": "--save_total_limit",
-                "help": "Limit the total number of saved model checkpoints to manage disk usage effectively. Default is to save only the latest checkpoint",
+                "help": "Save total limit to use",
                 "required": False,
                 "type": int,
                 "default": 1,
                 "alias": ["--save-total-limit"],
             },
             {
+                "arg": "--save_strategy",
+                "help": "Save strategy to use",
+                "required": False,
+                "type": str,
+                "default": "epoch",
+                "alias": ["--save-strategy"],
+            },
+            {
                 "arg": "--auto_find_batch_size",
-                "help": "Automatically determine the optimal batch size based on system capabilities to maximize efficiency.",
+                "help": "Auto find batch size True/False",
                 "required": False,
                 "action": "store_true",
                 "alias": ["--auto-find-batch-size"],
             },
             {
-                "arg": "--mixed_precision",
-                "help": "Choose the precision mode for training to optimize performance and memory usage. Options are 'fp16', 'bf16', or None for default precision. Default is None.",
+                "arg": "--mixed-precision",
+                "help": "fp16, bf16, or None",
                 "required": False,
                 "type": str,
                 "default": None,
-                "choices": ["fp16", "bf16", None],
-                "alias": ["--mixed-precision"],
+                "alias": ["--mixed-precision", "--mp"],
             },
             {
                 "arg": "--quantization",
-                "help": "Choose the quantization level to reduce model size and potentially increase inference speed. Options include 'int4', 'int8', or None. Enabling requires --peft",
+                "help": "int4, int8, or None",
                 "required": False,
                 "type": str,
                 "default": None,
                 "alias": ["--quantization"],
-                "choices": ["int4", "int8", None],
             },
             {
                 "arg": "--model_max_length",
-                "help": "Set the maximum length for the model to process in a single batch, which can affect both performance and memory usage. Default is 1024",
+                "help": "Model max length to use",
                 "required": False,
                 "type": int,
                 "default": 1024,
-                "alias": ["--model-max-length"],
-            },
-            {
-                "arg": "--max_prompt_length",
-                "help": "Specify the maximum length for prompts used in training, particularly relevant for tasks requiring initial contextual input. Used only for `orpo` trainer.",
-                "required": False,
-                "type": int,
-                "default": 128,
-                "alias": ["--max-prompt-length"],
-            },
-            {
-                "arg": "--max_completion_length",
-                "help": "Completion length to use, for orpo: encoder-decoder models only",
-                "required": False,
-                "type": int,
-                "default": None,
-                "alias": ["--max-completion-length"],
+                "alias": ["--max-len", "--max-length"],
             },
             {
                 "arg": "--trainer",
                 "help": "Trainer type to use",
                 "required": False,
                 "type": str,
                 "default": "default",
-                "choices": ["default", "dpo", "sft", "orpo", "reward"],
             },
             {
                 "arg": "--target_modules",
-                "help": "Identify specific modules within the model architecture to target with adaptations or optimizations, such as LoRA. Comma separated list of module names. Default is 'all-linear'.",
+                "help": "Target modules to use",
                 "required": False,
                 "type": str,
-                "default": "all-linear",
+                "default": None,
                 "alias": ["--target-modules"],
             },
             {
                 "arg": "--merge_adapter",
                 "help": "Use this flag to merge PEFT adapter with the model",
                 "required": False,
                 "action": "store_true",
@@ -241,31 +228,30 @@
                 "required": False,
                 "type": float,
                 "default": 0.1,
                 "alias": ["--dpo-beta"],
             },
             {
                 "arg": "--chat_template",
-                "help": "Apply a specific template for chat-based interactions, with options including 'tokenizer', 'chatml', 'zephyr', or None. This setting can shape the model's conversational behavior. ",
+                "help": "Apply chat template",
                 "required": False,
                 "default": None,
                 "alias": ["--chat-template"],
-                "choices": ["tokenizer", "chatml", "zephyr", None],
+                "choices": ["tokenizer", "chatml", "zephyr"],
             },
             {
                 "arg": "--padding",
-                "help": "Specify the padding direction for sequences, critical for models sensitive to input alignment. Options include 'left', 'right', or None",
+                "help": "Padding side",
                 "required": False,
                 "type": str,
                 "default": None,
                 "alias": ["--padding"],
-                "choices": ["left", "right", None],
             },
         ]
-        arg_list = common_args() + arg_list
+        arg_list.extend(common_args())
         run_llm_parser = parser.add_parser("llm", description="✨ Run AutoTrain LLM")
         for arg in arg_list:
             names = [arg["arg"]] + arg.get("alias", [])
             if "action" in arg:
                 run_llm_parser.add_argument(
                     *names,
                     dest=arg["arg"].replace("--", "").replace("-", "_"),
@@ -278,15 +264,14 @@
                 run_llm_parser.add_argument(
                     *names,
                     dest=arg["arg"].replace("--", "").replace("-", "_"),
                     help=arg["help"],
                     required=arg.get("required", False),
                     type=arg.get("type"),
                     default=arg.get("default"),
-                    choices=arg.get("choices"),
                 )
         run_llm_parser.set_defaults(func=run_llm_command_factory)
 
     def __init__(self, args):
         self.args = args
 
         store_true_arg_names = [
@@ -317,34 +302,82 @@
             if self.args.project_name is None:
                 raise ValueError("Project name must be specified")
             if self.args.data_path is None:
                 raise ValueError("Data path must be specified")
             if self.args.model is None:
                 raise ValueError("Model must be specified")
             if self.args.push_to_hub:
-                # must have project_name, username and token OR project_name, token
-                if self.args.username is None:
-                    raise ValueError("Usernamemust be specified for push to hub")
+                # must have project_name, username and token OR project_name, repo_id, token
+                if self.args.username is None and self.args.repo_id is None:
+                    raise ValueError("Username or repo id must be specified for push to hub")
                 if self.args.token is None:
                     raise ValueError("Token must be specified for push to hub")
 
             if self.args.backend.startswith("spaces") or self.args.backend.startswith("ep-"):
                 if not self.args.push_to_hub:
                     raise ValueError("Push to hub must be specified for spaces backend")
-                if self.args.username is None:
-                    raise ValueError("Username must be specified for spaces backend")
+                if self.args.username is None and self.args.repo_id is None:
+                    raise ValueError("Repo id or username must be specified for spaces backend")
                 if self.args.token is None:
                     raise ValueError("Token must be specified for spaces backend")
 
         if self.args.deploy:
             raise NotImplementedError("Deploy is not implemented yet")
         if self.args.inference:
             raise NotImplementedError("Inference is not implemented yet")
 
     def run(self):
         logger.info("Running LLM")
+        logger.info(f"Params: {self.args}")
         if self.args.train:
-            params = LLMTrainingParams(**vars(self.args))
+            params = LLMTrainingParams(
+                model=self.args.model,
+                data_path=self.args.data_path,
+                train_split=self.args.train_split,
+                valid_split=self.args.valid_split,
+                text_column=self.args.text_column,
+                lr=self.args.lr,
+                epochs=self.args.epochs,
+                batch_size=self.args.batch_size,
+                warmup_ratio=self.args.warmup_ratio,
+                gradient_accumulation=self.args.gradient_accumulation,
+                optimizer=self.args.optimizer,
+                scheduler=self.args.scheduler,
+                weight_decay=self.args.weight_decay,
+                max_grad_norm=self.args.max_grad_norm,
+                seed=self.args.seed,
+                add_eos_token=self.args.add_eos_token,
+                block_size=self.args.block_size,
+                peft=self.args.peft,
+                lora_r=self.args.lora_r,
+                lora_alpha=self.args.lora_alpha,
+                lora_dropout=self.args.lora_dropout,
+                logging_steps=self.args.logging_steps,
+                project_name=self.args.project_name,
+                evaluation_strategy=self.args.evaluation_strategy,
+                save_total_limit=self.args.save_total_limit,
+                save_strategy=self.args.save_strategy,
+                auto_find_batch_size=self.args.auto_find_batch_size,
+                mixed_precision=self.args.mixed_precision,
+                push_to_hub=self.args.push_to_hub,
+                model_max_length=self.args.model_max_length,
+                repo_id=self.args.repo_id,
+                quantization=self.args.quantization,
+                trainer=self.args.trainer,
+                target_modules=self.args.target_modules,
+                token=self.args.token,
+                merge_adapter=self.args.merge_adapter,
+                username=self.args.username,
+                use_flash_attention_2=self.args.use_flash_attention_2,
+                log=self.args.log,
+                rejected_text_column=self.args.rejected_text_column,
+                disable_gradient_checkpointing=self.args.disable_gradient_checkpointing,
+                model_ref=self.args.model_ref,
+                dpo_beta=self.args.dpo_beta,
+                prompt_text_column=self.args.prompt_text_column,
+                chat_template=self.args.chat_template,
+                padding=self.args.padding,
+            )
+
             params = llm_munge_data(params, local=self.args.backend.startswith("local"))
             project = AutoTrainProject(params=params, backend=self.args.backend)
-            job_id = project.create()
-            logger.info(f"Job ID: {job_id}")
+            _ = project.create()
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/run_spacerunner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from argparse import ArgumentParser
 
-from autotrain import logger
-from autotrain.backends.base import AVAILABLE_HARDWARE
-from autotrain.backends.spaces import SpaceRunner
+from autotrain.backend import SpaceRunner
 from autotrain.trainers.generic.params import GenericParams
 from autotrain.trainers.generic.utils import create_dataset_repo
 
 from . import BaseAutoTrainCommand
 
 
-BACKEND_CHOICES = list(AVAILABLE_HARDWARE.keys())
-BACKEND_CHOICES = [b for b in BACKEND_CHOICES if b.startswith("spaces-")]
+BACKEND_CHOICES = [
+    "spaces-a10gl",
+    "spaces-a10gs",
+    "spaces-a100",
+    "spaces-t4m",
+    "spaces-t4s",
+    "spaces-cpu",
+    "spaces-cpuf",
+]
 
 
 def run_spacerunner_command_factory(args):
     return RunAutoTrainSpaceRunnerCommand(args)
 
 
 class RunAutoTrainSpaceRunnerCommand(BaseAutoTrainCommand):
@@ -130,14 +135,15 @@
             token=self.args.token,
         )
         params = GenericParams(
             project_name=self.args.project_name,
             data_path=dataset_id,
             username=self.args.username,
             token=self.args.token,
+            backend=self.args.backend,
             script_path=self.args.script_path,
             env=self.args.env,
             args=self.args.args,
+            repo_id=f"{self.args.username}/{self.args.project_name}",
         )
-        project = SpaceRunner(params=params, backend=self.args.backend)
-        job_id = project.create()
-        logger.info(f"Job ID: {job_id}")
+        sr = SpaceRunner(params=params, backend=self.args.backend)
+        sr.prepare()
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/cli/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,78 @@
 import os
 
-from autotrain.backends.base import AVAILABLE_HARDWARE
 from autotrain.dataset import AutoTrainDataset, AutoTrainDreamboothDataset
 
 
 def common_args():
     args = [
         {
             "arg": "--train",
-            "help": "Command to train the model",
+            "help": "Train the model",
             "required": False,
             "action": "store_true",
         },
         {
             "arg": "--deploy",
-            "help": "Command to deploy the model (limited availability)",
+            "help": "Deploy the model",
             "required": False,
             "action": "store_true",
         },
         {
             "arg": "--inference",
-            "help": "Command to run inference (limited availability)",
+            "help": "Run inference",
             "required": False,
             "action": "store_true",
         },
         {
             "arg": "--username",
             "help": "Hugging Face Hub Username",
             "required": False,
             "type": str,
         },
         {
             "arg": "--backend",
-            "help": "Backend to use: default or spaces. Spaces backend requires push_to_hub & username. Advanced users only.",
+            "help": "Backend to use: default or spaces. Spaces backend requires push_to_hub and repo_id",
             "required": False,
             "type": str,
-            "default": "local",
-            "choices": AVAILABLE_HARDWARE.keys(),
+            "default": "local-cli",
         },
         {
             "arg": "--token",
-            "help": "Your Hugging Face API token. Token must have write access to the model hub.",
+            "help": "Hub token",
+            "required": False,
+            "type": str,
+        },
+        {
+            "arg": "--repo-id",
+            "help": "Hub repo id",
             "required": False,
             "type": str,
         },
         {
             "arg": "--push-to-hub",
-            "help": "Push to hub after training will push the trained model to the Hugging Face model hub.",
+            "help": "Push to hub",
             "required": False,
             "action": "store_true",
         },
         {
             "arg": "--model",
-            "help": "Base model to use for training",
+            "help": "Model to use for training",
             "required": True,
             "type": str,
         },
         {
             "arg": "--project-name",
-            "help": "Output directory / repo id for trained model (must be unique on hub)",
+            "help": "Output directory or repo id",
             "required": True,
             "type": str,
         },
         {
-            "arg": "--data-path",
-            "help": "Train dataset to use. When using cli, this should be a directory path containing training and validation data in appropriate formats",
-            "required": False,
-            "type": str,
-        },
-        {
-            "arg": "--train-split",
-            "help": "Train dataset split to use",
-            "required": False,
-            "type": str,
-            "default": "train",
-        },
-        {
-            "arg": "--valid-split",
-            "help": "Validation dataset split to use",
-            "required": False,
-            "type": str,
-            "default": None,
-        },
-        {
-            "arg": "--batch-size",
-            "help": "Training batch size to use",
-            "required": False,
-            "type": int,
-            "default": 2,
-            "alias": ["--train-batch-size"],
-        },
-        {
             "arg": "--seed",
-            "help": "Random seed for reproducibility",
+            "help": "Seed",
             "required": False,
             "default": 42,
             "type": int,
         },
         {
             "arg": "--epochs",
             "help": "Number of training epochs",
@@ -106,18 +82,17 @@
         },
         {
             "arg": "--gradient-accumulation",
             "help": "Gradient accumulation steps",
             "required": False,
             "default": 1,
             "type": int,
-            "alias": ["--gradient-accumulation"],
         },
         {
-            "arg": "--disable-gradient-checkpointing",
+            "arg": "--disable_gradient_checkpointing",
             "help": "Disable gradient checkpointing",
             "required": False,
             "action": "store_true",
             "alias": ["--disable-gradient-checkpointing", "--disable-gc"],
         },
         {
             "arg": "--lr",
@@ -128,15 +103,42 @@
         },
         {
             "arg": "--log",
             "help": "Use experiment tracking",
             "required": False,
             "type": str,
             "default": "none",
-            "choices": ["none", "wandb", "tensorboard"],
+        },
+        {
+            "arg": "--data-path",
+            "help": "Train dataset to use",
+            "required": False,
+            "type": str,
+        },
+        {
+            "arg": "--train-split",
+            "help": "Test dataset split to use",
+            "required": False,
+            "type": str,
+            "default": "train",
+        },
+        {
+            "arg": "--valid-split",
+            "help": "Validation dataset split to use",
+            "required": False,
+            "type": str,
+            "default": None,
+        },
+        {
+            "arg": "--batch-size",
+            "help": "Training batch size to use",
+            "required": False,
+            "type": int,
+            "default": 2,
+            "alias": ["--train-batch-size"],
         },
     ]
     return args
 
 
 def tabular_munge_data(params, local):
     if isinstance(params.target_columns, str):
@@ -151,62 +153,45 @@
     elif task == "regression" and len(col_map_label) > 1:
         task = "tabular_multi_column_regression"
     elif task == "regression" and len(col_map_label) == 1:
         task = "tabular_single_column_regression"
     else:
         raise Exception("Please select a valid task.")
 
-    exts = ["csv", "jsonl"]
-    ext_to_use = None
-    for ext in exts:
-        path = f"{params.data_path}/{params.train_split}.{ext}"
-        if os.path.exists(path):
-            ext_to_use = ext
-            break
-
-    train_data_path = f"{params.data_path}/{params.train_split}.{ext_to_use}"
+    train_data_path = f"{params.data_path}/{params.train_split}.csv"
     if params.valid_split is not None:
-        valid_data_path = f"{params.data_path}/{params.valid_split}.{ext_to_use}"
+        valid_data_path = f"{params.data_path}/{params.valid_split}.csv"
     else:
         valid_data_path = None
     if os.path.exists(train_data_path):
         dset = AutoTrainDataset(
             train_data=[train_data_path],
             task=task,
             token=params.token,
             project_name=params.project_name,
             username=params.username,
             column_mapping={"id": params.id_column, "label": col_map_label},
             valid_data=[valid_data_path] if valid_data_path is not None else None,
             percent_valid=None,  # TODO: add to UI
             local=local,
-            ext=ext_to_use,
         )
         params.data_path = dset.prepare()
         params.valid_split = "validation"
         params.id_column = "autotrain_id"
         if len(col_map_label) == 1:
             params.target_columns = ["autotrain_label"]
         else:
             params.target_columns = [f"autotrain_label_{i}" for i in range(len(col_map_label))]
     return params
 
 
 def llm_munge_data(params, local):
-    exts = ["csv", "jsonl"]
-    ext_to_use = None
-    for ext in exts:
-        path = f"{params.data_path}/{params.train_split}.{ext}"
-        if os.path.exists(path):
-            ext_to_use = ext
-            break
-
-    train_data_path = f"{params.data_path}/{params.train_split}.{ext_to_use}"
+    train_data_path = f"{params.data_path}/{params.train_split}.csv"
     if params.valid_split is not None:
-        valid_data_path = f"{params.data_path}/{params.valid_split}.{ext_to_use}"
+        valid_data_path = f"{params.data_path}/{params.valid_split}.csv"
     else:
         valid_data_path = None
     if os.path.exists(train_data_path):
         col_map = {"text": params.text_column}
         if params.rejected_text_column is not None:
             col_map["rejected_text"] = params.rejected_text_column
         if params.prompt_text_column is not None:
@@ -217,170 +202,107 @@
             token=params.token,
             project_name=params.project_name,
             username=params.username,
             column_mapping=col_map,
             valid_data=[valid_data_path] if valid_data_path is not None else None,
             percent_valid=None,  # TODO: add to UI
             local=local,
-            ext=ext_to_use,
         )
         params.data_path = dset.prepare()
         params.valid_split = None
         params.text_column = "autotrain_text"
         params.rejected_text_column = "autotrain_rejected_text"
         params.prompt_text_column = "autotrain_prompt"
     return params
 
 
 def seq2seq_munge_data(params, local):
-    exts = ["csv", "jsonl"]
-    ext_to_use = None
-    for ext in exts:
-        path = f"{params.data_path}/{params.train_split}.{ext}"
-        if os.path.exists(path):
-            ext_to_use = ext
-            break
-
-    train_data_path = f"{params.data_path}/{params.train_split}.{ext_to_use}"
+    train_data_path = f"{params.data_path}/{params.train_split}.csv"
     if params.valid_split is not None:
-        valid_data_path = f"{params.data_path}/{params.valid_split}.{ext_to_use}"
+        valid_data_path = f"{params.data_path}/{params.valid_split}.csv"
     else:
         valid_data_path = None
     if os.path.exists(train_data_path):
         dset = AutoTrainDataset(
             train_data=[train_data_path],
             task="seq2seq",
             token=params.token,
             project_name=params.project_name,
             username=params.username,
             column_mapping={"text": params.text_column, "label": params.target_column},
             valid_data=[valid_data_path] if valid_data_path is not None else None,
             percent_valid=None,  # TODO: add to UI
             local=local,
-            ext=ext_to_use,
         )
         params.data_path = dset.prepare()
         params.valid_split = "validation"
         params.text_column = "autotrain_text"
         params.target_column = "autotrain_label"
     return params
 
 
 def text_clf_munge_data(params, local):
-    exts = ["csv", "jsonl"]
-    ext_to_use = None
-    for ext in exts:
-        path = f"{params.data_path}/{params.train_split}.{ext}"
-        if os.path.exists(path):
-            ext_to_use = ext
-            break
-
-    train_data_path = f"{params.data_path}/{params.train_split}.{ext_to_use}"
+    train_data_path = f"{params.data_path}/{params.train_split}.csv"
     if params.valid_split is not None:
-        valid_data_path = f"{params.data_path}/{params.valid_split}.{ext_to_use}"
+        valid_data_path = f"{params.data_path}/{params.valid_split}.csv"
     else:
         valid_data_path = None
     if os.path.exists(train_data_path):
         dset = AutoTrainDataset(
             train_data=[train_data_path],
             valid_data=[valid_data_path] if valid_data_path is not None else None,
             task="text_multi_class_classification",
             token=params.token,
             project_name=params.project_name,
             username=params.username,
             column_mapping={"text": params.text_column, "label": params.target_column},
             percent_valid=None,  # TODO: add to UI
             local=local,
             convert_to_class_label=True,
-            ext=ext_to_use,
-        )
-        params.data_path = dset.prepare()
-        params.valid_split = "validation"
-        params.text_column = "autotrain_text"
-        params.target_column = "autotrain_label"
-    return params
-
-
-def text_reg_munge_data(params, local):
-    exts = ["csv", "jsonl"]
-    ext_to_use = None
-    for ext in exts:
-        path = f"{params.data_path}/{params.train_split}.{ext}"
-        if os.path.exists(path):
-            ext_to_use = ext
-            break
-
-    train_data_path = f"{params.data_path}/{params.train_split}.{ext_to_use}"
-    if params.valid_split is not None:
-        valid_data_path = f"{params.data_path}/{params.valid_split}.{ext_to_use}"
-    else:
-        valid_data_path = None
-    if os.path.exists(train_data_path):
-        dset = AutoTrainDataset(
-            train_data=[train_data_path],
-            valid_data=[valid_data_path] if valid_data_path is not None else None,
-            task="text_single_column_regression",
-            token=params.token,
-            project_name=params.project_name,
-            username=params.username,
-            column_mapping={"text": params.text_column, "label": params.target_column},
-            percent_valid=None,  # TODO: add to UI
-            local=local,
-            convert_to_class_label=False,
-            ext=ext_to_use,
         )
         params.data_path = dset.prepare()
         params.valid_split = "validation"
         params.text_column = "autotrain_text"
         params.target_column = "autotrain_label"
     return params
 
 
 def token_clf_munge_data(params, local):
-    exts = ["csv", "jsonl"]
-    ext_to_use = None
-    for ext in exts:
-        path = f"{params.data_path}/{params.train_split}.{ext}"
-        if os.path.exists(path):
-            ext_to_use = ext
-            break
-
-    train_data_path = f"{params.data_path}/{params.train_split}.{ext_to_use}"
+    train_data_path = f"{params.data_path}/{params.train_split}.csv"
     if params.valid_split is not None:
-        valid_data_path = f"{params.data_path}/{params.valid_split}.{ext_to_use}"
+        valid_data_path = f"{params.data_path}/{params.valid_split}.csv"
     else:
         valid_data_path = None
     if os.path.exists(train_data_path):
         dset = AutoTrainDataset(
             train_data=[train_data_path],
             valid_data=[valid_data_path] if valid_data_path is not None else None,
             task="text_token_classification",
             token=params.token,
             project_name=params.project_name,
             username=params.username,
             column_mapping={"text": params.tokens_column, "label": params.tags_column},
             percent_valid=None,  # TODO: add to UI
             local=local,
             convert_to_class_label=True,
-            ext=ext_to_use,
         )
         params.data_path = dset.prepare()
         params.valid_split = "validation"
         params.text_column = "autotrain_text"
         params.target_column = "autotrain_label"
     return params
 
 
 def img_clf_munge_data(params, local):
     train_data_path = f"{params.data_path}/{params.train_split}"
-    # if params.valid_split is not None:
-    #     valid_data_path = f"{params.data_path}/{params.valid_split}"
-    # else:
-    #     valid_data_path = None
-    if os.path.isdir(train_data_path):
+    if params.valid_split is not None:
+        valid_data_path = f"{params.data_path}/{params.valid_split}"
+    else:
+        valid_data_path = None
+    if os.path.isdir(train_data_path) or os.path.isdir(valid_data_path):
         raise Exception("Image classification is not yet supported for local datasets using the CLI. Please use UI.")
     return params
 
 
 def dreambooth_munge_data(params, local):
     # check if params.image_path is a directory
     if os.path.isdir(params.image_path):
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/commands.py` & `autotrain-advanced-0.7.9/src/autotrain/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from autotrain.trainers.clm.params import LLMTrainingParams
 from autotrain.trainers.dreambooth.params import DreamBoothTrainingParams
 from autotrain.trainers.generic.params import GenericParams
 from autotrain.trainers.image_classification.params import ImageClassificationParams
 from autotrain.trainers.seq2seq.params import Seq2SeqParams
 from autotrain.trainers.tabular.params import TabularParams
 from autotrain.trainers.text_classification.params import TextClassificationParams
-from autotrain.trainers.text_regression.params import TextRegressionParams
 from autotrain.trainers.token_classification.params import TokenClassificationParams
 
 
 def launch_command(params):
     params.project_name = shlex.split(params.project_name)[0]
     cuda_available = torch.cuda.is_available()
     mps_available = torch.backends.mps.is_available()
@@ -49,15 +48,15 @@
                 "--multi_gpu",
                 "--num_machines",
                 "1",
                 "--num_processes",
                 "2",
             ]
         else:
-            if params.quantization in ("int8", "int4") and params.peft and params.mixed_precision == "bf16":
+            if params.quantization in ("int8", "int4") and params.peft:
                 cmd = [
                     "accelerate",
                     "launch",
                     "--multi_gpu",
                     "--num_machines",
                     "1",
                     "--num_processes",
@@ -72,20 +71,14 @@
                     "3",
                     "--offload_optimizer_device",
                     "none",
                     "--offload_param_device",
                     "none",
                     "--zero3_save_16bit_model",
                     "true",
-                    "--zero3_init_flag",
-                    "true",
-                    "--deepspeed_multinode_launcher",
-                    "standard",
-                    "--gradient_accumulation_steps",
-                    str(params.gradient_accumulation),
                 ]
 
         if num_gpus > 0:
             cmd.append("--mixed_precision")
             if params.mixed_precision == "fp16":
                 cmd.append("fp16")
             elif params.mixed_precision == "bf16":
@@ -121,15 +114,15 @@
         cmd = [
             "python",
             "-m",
             "autotrain.trainers.tabular",
             "--training_config",
             os.path.join(params.project_name, "training_params.json"),
         ]
-    elif isinstance(params, TextClassificationParams) or isinstance(params, TextRegressionParams):
+    elif isinstance(params, TextClassificationParams):
         if num_gpus == 0:
             cmd = [
                 "accelerate",
                 "launch",
                 "--cpu",
             ]
         elif num_gpus == 1:
@@ -157,32 +150,22 @@
             if params.mixed_precision == "fp16":
                 cmd.append("fp16")
             elif params.mixed_precision == "bf16":
                 cmd.append("bf16")
             else:
                 cmd.append("no")
 
-        if isinstance(params, TextRegressionParams):
-            cmd.extend(
-                [
-                    "-m",
-                    "autotrain.trainers.text_regression",
-                    "--training_config",
-                    os.path.join(params.project_name, "training_params.json"),
-                ]
-            )
-        else:
-            cmd.extend(
-                [
-                    "-m",
-                    "autotrain.trainers.text_classification",
-                    "--training_config",
-                    os.path.join(params.project_name, "training_params.json"),
-                ]
-            )
+        cmd.extend(
+            [
+                "-m",
+                "autotrain.trainers.text_classification",
+                "--training_config",
+                os.path.join(params.project_name, "training_params.json"),
+            ]
+        )
     elif isinstance(params, TokenClassificationParams):
         if num_gpus == 0:
             cmd = [
                 "accelerate",
                 "launch",
                 "--cpu",
             ]
@@ -291,15 +274,15 @@
                 "--multi_gpu",
                 "--num_machines",
                 "1",
                 "--num_processes",
                 "2",
             ]
         else:
-            if params.quantization in ("int8", "int4") and params.peft and params.mixed_precision == "bf16":
+            if params.quantization in ("int8", "int4") and params.peft:
                 cmd = [
                     "accelerate",
                     "launch",
                     "--multi_gpu",
                     "--num_machines",
                     "1",
                     "--num_processes",
@@ -314,20 +297,14 @@
                     "3",
                     "--offload_optimizer_device",
                     "none",
                     "--offload_param_device",
                     "none",
                     "--zero3_save_16bit_model",
                     "true",
-                    "--zero3_init_flag",
-                    "true",
-                    "--deepspeed_multinode_launcher",
-                    "standard",
-                    "--gradient_accumulation_steps",
-                    str(params.gradient_accumulation),
                 ]
         if num_gpus > 0:
             cmd.append("--mixed_precision")
             if params.mixed_precision == "fp16":
                 cmd.append("fp16")
             elif params.mixed_precision == "bf16":
                 cmd.append("bf16")
@@ -342,10 +319,8 @@
                 os.path.join(params.project_name, "training_params.json"),
             ]
         )
 
     else:
         raise ValueError("Unsupported params type")
 
-    logger.info(cmd)
-    logger.info(params)
     return cmd
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import uuid
 import zipfile
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
 
+from autotrain import logger
 from autotrain.preprocessor.dreambooth import DreamboothPreprocessor
 from autotrain.preprocessor.tabular import (
     TabularBinaryClassificationPreprocessor,
     TabularMultiClassClassificationPreprocessor,
     TabularMultiColumnRegressionPreprocessor,
     TabularMultiLabelClassificationPreprocessor,
     TabularSingleColumnRegressionPreprocessor,
@@ -58,14 +59,15 @@
 
     def __str__(self) -> str:
         info = f"Dataset: {self.project_name} ({self.task})\n"
         return info
 
     def __post_init__(self):
         self.task = "dreambooth"
+        logger.info(self.__str__())
 
     @property
     def num_samples(self):
         return len(self.concept_images)
 
     def prepare(self):
         preprocessor = DreamboothPreprocessor(
@@ -99,14 +101,15 @@
         self.task = "image_multi_class_classification"
         if not self.valid_data and self.percent_valid is None:
             self.percent_valid = 0.2
         elif self.valid_data and self.percent_valid is not None:
             raise ValueError("You can only specify one of valid_data or percent_valid")
         elif self.valid_data:
             self.percent_valid = 0.0
+        logger.info(self.__str__())
 
         self.num_files = self._count_files()
 
     @property
     def num_samples(self):
         return self.num_files
 
@@ -176,15 +179,14 @@
     project_name: str
     username: Optional[str] = None
     column_mapping: Optional[Dict[str, str]] = None
     valid_data: Optional[List[str]] = None
     percent_valid: Optional[float] = None
     convert_to_class_label: Optional[bool] = False
     local: bool = False
-    ext: Optional[str] = "csv"
 
     def __str__(self) -> str:
         info = f"Dataset: {self.project_name} ({self.task})\n"
         info += f"Train data: {self.train_data}\n"
         info += f"Valid data: {self.valid_data}\n"
         info += f"Column mapping: {self.column_mapping}\n"
         return info
@@ -196,41 +198,36 @@
             self.percent_valid = 0.2
         elif self.valid_data and self.percent_valid is not None:
             raise ValueError("You can only specify one of valid_data or percent_valid")
         elif self.valid_data:
             self.percent_valid = 0.0
 
         self.train_df, self.valid_df = self._preprocess_data()
+        logger.info(self.__str__())
 
     def _preprocess_data(self):
         train_df = []
         for file in self.train_data:
             if isinstance(file, pd.DataFrame):
                 train_df.append(file)
             else:
-                if self.ext == "jsonl":
-                    train_df.append(pd.read_json(file, lines=True))
-                else:
-                    train_df.append(pd.read_csv(file))
+                train_df.append(pd.read_csv(file))
         if len(train_df) > 1:
             train_df = pd.concat(train_df)
         else:
             train_df = train_df[0]
 
         valid_df = None
         if len(self.valid_data) > 0:
             valid_df = []
             for file in self.valid_data:
                 if isinstance(file, pd.DataFrame):
                     valid_df.append(file)
                 else:
-                    if self.ext == "jsonl":
-                        valid_df.append(pd.read_json(file, lines=True))
-                    else:
-                        valid_df.append(pd.read_csv(file))
+                    valid_df.append(pd.read_csv(file))
             if len(valid_df) > 1:
                 valid_df = pd.concat(valid_df)
             else:
                 valid_df = valid_df[0]
         return train_df, valid_df
 
     @property
@@ -284,15 +281,14 @@
                 username=self.username,
                 project_name=self.project_name,
                 valid_data=self.valid_df,
                 test_size=self.percent_valid,
                 token=self.token,
                 seed=42,
                 local=self.local,
-                convert_to_class_label=self.convert_to_class_label,
             )
             return preprocessor.prepare()
 
         elif self.task == "text_single_column_regression":
             text_column = self.column_mapping["text"]
             label_column = self.column_mapping["label"]
             preprocessor = TextSingleColumnRegressionPreprocessor(
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/help.py` & `autotrain-advanced-0.7.9/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/dreambooth.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,17 @@
                 )
             except Exception:
                 logger.error("Error creating repo")
                 raise ValueError("Error creating repo")
 
     def _upload_concept_images(self, file, api):
         logger.info(f"Uploading {file} to concept1")
-        if isinstance(file, str):
-            path_in_repo = f"concept1/{file.split('/')[-1]}"
-        else:
-            path_in_repo = f"concept1/{file.filename.split('/')[-1]}"
-
         api.upload_file(
-            path_or_fileobj=file if isinstance(file, str) else file.file.read(),
-            path_in_repo=path_in_repo,
+            path_or_fileobj=file.file.read(),
+            path_in_repo=f"concept1/{file.filename.split('/')[-1]}",
             repo_id=self.repo_name,
             repo_type="dataset",
             token=self.token,
         )
 
     def _upload_concept_prompts(self, api):
         _prompts = {}
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import pandas as pd
 from datasets import ClassLabel, Dataset, DatasetDict, Sequence
 from sklearn.model_selection import train_test_split
 
-from autotrain import logger
-
 
 RESERVED_COLUMNS = ["autotrain_text", "autotrain_label"]
 LLM_RESERVED_COLUMNS = [
     "autotrain_prompt",
     "autotrain_context",
     "autotrain_rejected_text",
     "autotrain_prompt_start",
@@ -78,17 +76,14 @@
         valid_df = valid_df.drop(columns=[self.text_column, self.label_column])
         return train_df, valid_df
 
     def prepare(self):
         train_df, valid_df = self.split()
         train_df, valid_df = self.prepare_columns(train_df, valid_df)
 
-        train_df.loc[:, "autotrain_label"] = train_df["autotrain_label"].astype(str)
-        valid_df.loc[:, "autotrain_label"] = valid_df["autotrain_label"].astype(str)
-
         label_names = sorted(set(train_df["autotrain_label"].unique().tolist()))
 
         train_df = Dataset.from_pandas(train_df)
         valid_df = Dataset.from_pandas(valid_df)
 
         if self.convert_to_class_label:
             train_df = train_df.cast_column("autotrain_label", ClassLabel(names=label_names))
@@ -135,47 +130,14 @@
                 test_size=self.test_size,
                 random_state=self.seed,
             )
             train_df = train_df.reset_index(drop=True)
             valid_df = valid_df.reset_index(drop=True)
             return train_df, valid_df
 
-    def prepare(self):
-        train_df, valid_df = self.split()
-        train_df, valid_df = self.prepare_columns(train_df, valid_df)
-
-        train_df = Dataset.from_pandas(train_df)
-        valid_df = Dataset.from_pandas(valid_df)
-
-        if self.local:
-            dataset = DatasetDict(
-                {
-                    "train": train_df,
-                    "validation": valid_df,
-                }
-            )
-            dataset.save_to_disk(f"{self.project_name}/autotrain-data")
-        else:
-            train_df.push_to_hub(
-                f"{self.username}/autotrain-data-{self.project_name}",
-                split="train",
-                private=True,
-                token=self.token,
-            )
-            valid_df.push_to_hub(
-                f"{self.username}/autotrain-data-{self.project_name}",
-                split="validation",
-                private=True,
-                token=self.token,
-            )
-
-        if self.local:
-            return f"{self.project_name}/autotrain-data"
-        return f"{self.username}/autotrain-data-{self.project_name}"
-
 
 class TextTokenClassificationPreprocessor(TextBinaryClassificationPreprocessor):
     def split(self):
         if self.valid_data is not None:
             return self.train_data, self.valid_data
         else:
             train_df, valid_df = train_test_split(
@@ -186,26 +148,16 @@
             train_df = train_df.reset_index(drop=True)
             valid_df = valid_df.reset_index(drop=True)
             return train_df, valid_df
 
     def prepare(self):
         train_df, valid_df = self.split()
         train_df, valid_df = self.prepare_columns(train_df, valid_df)
-        try:
-            train_df.loc[:, "autotrain_text"] = train_df["autotrain_text"].apply(lambda x: ast.literal_eval(x))
-            valid_df.loc[:, "autotrain_text"] = valid_df["autotrain_text"].apply(lambda x: ast.literal_eval(x))
-        except ValueError:
-            logger.warning("Unable to do ast.literal_eval on train_df['autotrain_text']")
-            logger.warning("assuming autotrain_text is already a list")
-        try:
-            train_df.loc[:, "autotrain_label"] = train_df["autotrain_label"].apply(lambda x: ast.literal_eval(x))
-            valid_df.loc[:, "autotrain_label"] = valid_df["autotrain_label"].apply(lambda x: ast.literal_eval(x))
-        except ValueError:
-            logger.warning("Unable to do ast.literal_eval on train_df['autotrain_label']")
-            logger.warning("assuming autotrain_label is already a list")
+        train_df.loc[:, "autotrain_text"] = train_df["autotrain_label"].apply(lambda x: ast.literal_eval(x))
+        valid_df.loc[:, "autotrain_text"] = valid_df["autotrain_label"].apply(lambda x: ast.literal_eval(x))
 
         label_names_train = sorted(set(train_df["autotrain_label"].explode().unique().tolist()))
         label_names_valid = sorted(set(valid_df["autotrain_label"].explode().unique().tolist()))
         label_names = sorted(set(label_names_train + label_names_valid))
 
         train_df = Dataset.from_pandas(train_df)
         valid_df = Dataset.from_pandas(valid_df)
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.9/src/autotrain/preprocessor/vision.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import pandas as pd
 from datasets import load_dataset
 from sklearn.model_selection import train_test_split
 
+from autotrain import logger
+
 
 ALLOWED_EXTENSIONS = ("jpeg", "png", "jpg", "JPG", "JPEG", "PNG")
 
 
 @dataclass
 class ImageClassificationPreprocessor:
     train_data: str
@@ -27,14 +29,15 @@
         # Check if train data path exists
         if not os.path.exists(self.train_data):
             raise ValueError(f"{self.train_data} does not exist.")
 
         # Check if train data path contains at least 2 folders
         subfolders = [f.path for f in os.scandir(self.train_data) if f.is_dir()]
         # list subfolders
+        logger.info(f"🚀 Subfolders: {subfolders}")
         if len(subfolders) < 2:
             raise ValueError(f"{self.train_data} should contain at least 2 subfolders.")
 
         # Check if each subfolder contains at least 5 image files in jpeg, png or jpg format only
         for subfolder in subfolders:
             image_files = [f for f in os.listdir(subfolder) if f.endswith(ALLOWED_EXTENSIONS)]
             if len(image_files) < 5:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/clm/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,57 +12,55 @@
     # data params
     data_path: str = Field("data", title="Data path")
     train_split: str = Field("train", title="Train data config")
     valid_split: Optional[str] = Field(None, title="Validation data config")
     add_eos_token: bool = Field(True, title="Add EOS token")
     block_size: Union[int, List[int]] = Field(-1, title="Block size")
     model_max_length: int = Field(2048, title="Model max length")
-    padding: Optional[str] = Field("right", title="Padding side")
+    padding: Optional[str] = Field(None, title="Padding side")
 
     # trainer params
     trainer: str = Field("default", title="Trainer type")
     use_flash_attention_2: bool = Field(False, title="Use flash attention 2")
     log: str = Field("none", title="Logging using experiment tracking")
     disable_gradient_checkpointing: bool = Field(False, title="Gradient checkpointing")
     logging_steps: int = Field(-1, title="Logging steps")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     save_total_limit: int = Field(1, title="Save total limit")
+    save_strategy: str = Field("epoch", title="Save strategy")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     lr: float = Field(3e-5, title="Learning rate")
     epochs: int = Field(1, title="Number of training epochs")
     batch_size: int = Field(2, title="Training batch size")
     warmup_ratio: float = Field(0.1, title="Warmup proportion")
-    gradient_accumulation: int = Field(4, title="Gradient accumulation steps")
+    gradient_accumulation: int = Field(1, title="Gradient accumulation steps")
     optimizer: str = Field("adamw_torch", title="Optimizer")
     scheduler: str = Field("linear", title="Scheduler")
     weight_decay: float = Field(0.0, title="Weight decay")
     max_grad_norm: float = Field(1.0, title="Max gradient norm")
     seed: int = Field(42, title="Seed")
     chat_template: Optional[str] = Field(None, title="Chat template, one of: None, zephyr, chatml or tokenizer")
 
     # peft
-    quantization: Optional[str] = Field("int4", title="int4, int8, or None")
+    quantization: Optional[str] = Field(None, title="int4, int8, or None")
     target_modules: Optional[str] = Field("all-linear", title="Target modules")
     merge_adapter: bool = Field(False, title="Merge adapter")
     peft: bool = Field(False, title="Use PEFT")
     lora_r: int = Field(16, title="Lora r")
     lora_alpha: int = Field(32, title="Lora alpha")
     lora_dropout: float = Field(0.05, title="Lora dropout")
 
     # dpo
     model_ref: Optional[str] = Field(None, title="Reference, for DPO trainer")
     dpo_beta: float = Field(0.1, title="Beta for DPO trainer")
 
-    # orpo + dpo
-    max_prompt_length: int = Field(128, title="Prompt length")
-    max_completion_length: Optional[int] = Field(None, title="Completion length")
-
     # column mappings
     prompt_text_column: Optional[str] = Field(None, title="Prompt text column")
     text_column: str = Field("text", title="Text column")
     rejected_text_column: Optional[str] = Field(None, title="Rejected text column")
 
     # push to hub
     push_to_hub: bool = Field(False, title="Push to hub")
+    repo_id: Optional[str] = Field(None, title="Repo id")
     username: Optional[str] = Field(None, title="Hugging Face Username")
     token: Optional[str] = Field(None, title="Huggingface token")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/clm/train_clm_default.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,202 @@
-from functools import partial
+import argparse
+import json
 
-import torch
-from datasets import Dataset
-from peft import LoraConfig, get_peft_model, prepare_model_for_kbit_training
-from peft.tuners.lora import LoraLayer
+from accelerate.state import PartialState
+from datasets import load_dataset, load_from_disk
+from huggingface_hub import HfApi
 from transformers import (
     AutoConfig,
-    AutoModelForCausalLM,
-    BitsAndBytesConfig,
+    AutoModelForSequenceClassification,
+    AutoTokenizer,
+    EarlyStoppingCallback,
     Trainer,
     TrainingArguments,
-    default_data_collator,
 )
-from transformers.trainer_callback import PrinterCallback
 
 from autotrain import logger
-from autotrain.trainers.clm import utils
-from autotrain.trainers.clm.params import LLMTrainingParams
-from autotrain.trainers.common import ALLOW_REMOTE_CODE
+from autotrain.trainers.common import monitor, pause_space, remove_autotrain_data, save_training_params
+from autotrain.trainers.text_classification import utils
+from autotrain.trainers.text_classification.dataset import TextClassificationDataset
+from autotrain.trainers.text_classification.params import TextClassificationParams
 
 
-def process_data(data, tokenizer, config):
-    data = data.to_pandas()
-    data = data.fillna("")
-
-    data = data[[config.text_column]]
-    if config.add_eos_token:
-        data[config.text_column] = data[config.text_column] + tokenizer.eos_token
-    data = Dataset.from_pandas(data)
-    return data
+def parse_args():
+    # get training_config.json from the end user
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--training_config", type=str, required=True)
+    return parser.parse_args()
 
 
+@monitor
 def train(config):
-    logger.info("Starting default/generic CLM training...")
     if isinstance(config, dict):
-        config = LLMTrainingParams(**config)
-    train_data, valid_data = utils.process_input_data(config)
-    tokenizer = utils.get_tokenizer(config)
-    train_data, valid_data = utils.process_data_with_chat_template(config, tokenizer, train_data, valid_data)
-
-    train_data = process_data(
-        data=train_data,
-        tokenizer=tokenizer,
-        config=config,
-    )
+        config = TextClassificationParams(**config)
+
+    if config.repo_id is None and config.username is not None:
+        config.repo_id = f"{config.username}/{config.project_name}"
+
+    if PartialState().process_index == 0:
+        logger.info("Starting training...")
+        logger.info(f"Training config: {config}")
+
+    train_data = None
+    valid_data = None
+    # check if config.train_split.csv exists in config.data_path
+    if config.train_split is not None:
+        if config.data_path == f"{config.project_name}/autotrain-data":
+            logger.info("loading dataset from disk")
+            train_data = load_from_disk(config.data_path)[config.train_split]
+        else:
+            train_data = load_dataset(
+                config.data_path,
+                split=config.train_split,
+                token=config.token,
+            )
+
     if config.valid_split is not None:
-        valid_data = process_data(
-            data=valid_data,
-            tokenizer=tokenizer,
-            config=config,
-        )
+        if config.data_path == f"{config.project_name}/autotrain-data":
+            logger.info("loading dataset from disk")
+            valid_data = load_from_disk(config.data_path)[config.valid_split]
+        else:
+            valid_data = load_dataset(
+                config.data_path,
+                split=config.valid_split,
+                token=config.token,
+            )
 
-    logging_steps = utils.configure_logging_steps(config, train_data, valid_data)
-    training_args = utils.configure_training_args(config, logging_steps)
-    config = utils.configure_block_size(config, tokenizer)
-    args = TrainingArguments(**training_args)
+    classes = train_data.features[config.target_column].names
+    label2id = {c: i for i, c in enumerate(classes)}
+    num_classes = len(classes)
 
-    logger.info("loading model config...")
-    model_config = AutoConfig.from_pretrained(
-        config.model,
-        token=config.token,
-        trust_remote_code=ALLOW_REMOTE_CODE,
-        use_cache=config.disable_gradient_checkpointing,
-    )
+    if num_classes < 2:
+        raise ValueError("Invalid number of classes. Must be greater than 1.")
 
-    logger.info("loading model...")
-    if config.peft:
-        if config.quantization == "int4":
-            bnb_config = BitsAndBytesConfig(
-                load_in_4bit=True,
-                bnb_4bit_quant_type="nf4",
-                bnb_4bit_compute_dtype=torch.float16,
-                bnb_4bit_use_double_quant=False,
+    if config.valid_split is not None:
+        num_classes_valid = len(valid_data.unique(config.target_column))
+        if num_classes_valid != num_classes:
+            raise ValueError(
+                f"Number of classes in train and valid are not the same. Training has {num_classes} and valid has {num_classes_valid}"
             )
-        elif config.quantization == "int8":
-            bnb_config = BitsAndBytesConfig(load_in_8bit=True)
-        else:
-            bnb_config = None
 
-        model = AutoModelForCausalLM.from_pretrained(
+    model_config = AutoConfig.from_pretrained(config.model, num_labels=num_classes)
+    model_config._num_labels = len(label2id)
+    model_config.label2id = label2id
+    model_config.id2label = {v: k for k, v in label2id.items()}
+
+    try:
+        model = AutoModelForSequenceClassification.from_pretrained(
             config.model,
             config=model_config,
+            trust_remote_code=True,
             token=config.token,
-            quantization_config=bnb_config,
-            trust_remote_code=ALLOW_REMOTE_CODE,
-            use_flash_attention_2=config.use_flash_attention_2,
+            ignore_mismatched_sizes=True,
         )
-    else:
-        model = AutoModelForCausalLM.from_pretrained(
+    except OSError:
+        model = AutoModelForSequenceClassification.from_pretrained(
             config.model,
             config=model_config,
+            from_tf=True,
+            trust_remote_code=True,
             token=config.token,
-            trust_remote_code=ALLOW_REMOTE_CODE,
-            use_flash_attention_2=config.use_flash_attention_2,
+            ignore_mismatched_sizes=True,
         )
 
-    logger.info(f"model dtype: {model.dtype}")
-    model.resize_token_embeddings(len(tokenizer))
-    if config.peft:
-        logger.info("preparing peft model...")
-        if config.quantization is not None:
-            gradient_checkpointing_kwargs = {}
-            if not config.disable_gradient_checkpointing:
-                if config.quantization in ("int4", "int8"):
-                    gradient_checkpointing_kwargs = {"use_reentrant": True}
-                else:
-                    gradient_checkpointing_kwargs = {"use_reentrant": False}
-            model = prepare_model_for_kbit_training(
-                model,
-                use_gradient_checkpointing=not config.disable_gradient_checkpointing,
-                gradient_checkpointing_kwargs=gradient_checkpointing_kwargs,
-            )
-        else:
-            model.enable_input_require_grads()
-
-        peft_config = LoraConfig(
-            r=config.lora_r,
-            lora_alpha=config.lora_alpha,
-            lora_dropout=config.lora_dropout,
-            bias="none",
-            task_type="CAUSAL_LM",
-            target_modules=utils.get_target_modules(config),
-        )
-        model = get_peft_model(model, peft_config)
-
-    tokenize_fn = partial(utils.tokenize, tokenizer=tokenizer, config=config)
-    group_texts_fn = partial(utils.group_texts, config=config)
+    tokenizer = AutoTokenizer.from_pretrained(config.model, token=config.token, trust_remote_code=True)
+    train_data = TextClassificationDataset(data=train_data, tokenizer=tokenizer, config=config)
+    if config.valid_split is not None:
+        valid_data = TextClassificationDataset(data=valid_data, tokenizer=tokenizer, config=config)
 
-    train_data = train_data.map(
-        tokenize_fn,
-        batched=True,
-        num_proc=1,
-        remove_columns=list(train_data.features),
-        desc="Running tokenizer on train dataset",
-    )
+    if config.logging_steps == -1:
+        if config.valid_split is not None:
+            logging_steps = int(0.2 * len(valid_data) / config.batch_size)
+        else:
+            logging_steps = int(0.2 * len(train_data) / config.batch_size)
+        if logging_steps == 0:
+            logging_steps = 1
 
-    if config.valid_split is not None:
-        valid_data = valid_data.map(
-            tokenize_fn,
-            batched=True,
-            num_proc=1,
-            remove_columns=list(valid_data.features),
-            desc="Running tokenizer on validation dataset",
-        )
+    else:
+        logging_steps = config.logging_steps
 
-    train_data = train_data.map(
-        group_texts_fn,
-        batched=True,
-        num_proc=4,
-        desc=f"Grouping texts in chunks of {config.block_size}",
-    )
+    training_args = dict(
+        output_dir=config.project_name,
+        per_device_train_batch_size=config.batch_size,
+        per_device_eval_batch_size=2 * config.batch_size,
+        learning_rate=config.lr,
+        num_train_epochs=config.epochs,
+        evaluation_strategy=config.evaluation_strategy if config.valid_split is not None else "no",
+        logging_steps=logging_steps,
+        save_total_limit=config.save_total_limit,
+        save_strategy=config.save_strategy,
+        gradient_accumulation_steps=config.gradient_accumulation,
+        report_to=config.log,
+        auto_find_batch_size=config.auto_find_batch_size,
+        lr_scheduler_type=config.scheduler,
+        optim=config.optimizer,
+        warmup_ratio=config.warmup_ratio,
+        weight_decay=config.weight_decay,
+        max_grad_norm=config.max_grad_norm,
+        push_to_hub=False,
+        load_best_model_at_end=True if config.valid_split is not None else False,
+        ddp_find_unused_parameters=False,
+    )
+
+    if config.mixed_precision == "fp16":
+        training_args["fp16"] = True
+    if config.mixed_precision == "bf16":
+        training_args["bf16"] = True
 
     if config.valid_split is not None:
-        valid_data = valid_data.map(
-            group_texts_fn,
-            batched=True,
-            num_proc=4,
-            desc=f"Grouping texts in chunks of {config.block_size}",
-        )
+        early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
+        callbacks_to_use = [early_stop]
+    else:
+        callbacks_to_use = []
 
-    logger.info("creating trainer")
-    callbacks = utils.get_callbacks(config)
+    args = TrainingArguments(**training_args)
     trainer_args = dict(
         args=args,
         model=model,
-        callbacks=callbacks,
+        callbacks=callbacks_to_use,
+        compute_metrics=(
+            utils._binary_classification_metrics if num_classes == 2 else utils._multi_class_classification_metrics
+        ),
     )
+
     trainer = Trainer(
         **trainer_args,
         train_dataset=train_data,
-        eval_dataset=valid_data if config.valid_split is not None else None,
-        tokenizer=tokenizer,
-        data_collator=default_data_collator,
+        eval_dataset=valid_data,
     )
-    for name, module in trainer.model.named_modules():
-        if isinstance(module, LoraLayer):
-            if config.mixed_precision == "bf16":
-                module = module.to(torch.bfloat16)
-        if "norm" in name:
-            module = module.to(torch.float32)
-        if any(x in name for x in ["lm_head", "embed_tokens", "wte", "wpe"]):
-            if hasattr(module, "weight"):
-                if config.mixed_precision == "bf16" and module.weight.dtype == torch.float32:
-                    module = module.to(torch.bfloat16)
-
-    trainer.remove_callback(PrinterCallback)
     trainer.train()
-    utils.post_training_steps(config, trainer)
+
+    logger.info("Finished training, saving model...")
+    trainer.save_model(config.project_name)
+    tokenizer.save_pretrained(config.project_name)
+
+    model_card = utils.create_model_card(config, trainer, num_classes)
+
+    # save model card to output directory as README.md
+    with open(f"{config.project_name}/README.md", "w") as f:
+        f.write(model_card)
+
+    if config.push_to_hub:
+        if PartialState().process_index == 0:
+            remove_autotrain_data(config)
+            save_training_params(config)
+            logger.info("Pushing model to hub...")
+            api = HfApi(token=config.token)
+            api.create_repo(repo_id=config.repo_id, repo_type="model", private=True)
+            api.upload_folder(
+                folder_path=config.project_name,
+                repo_id=config.repo_id,
+                repo_type="model",
+            )
+
+    if PartialState().process_index == 0:
+        pause_space(config)
+
+
+if __name__ == "__main__":
+    args = parse_args()
+    training_config = json.load(open(args.training_config))
+    config = TextClassificationParams(**training_config)
+    train(config)
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pydantic import Field
 
 from autotrain.trainers.common import AutoTrainParams
 
 
 class DreamBoothTrainingParams(AutoTrainParams):
     model: str = Field(None, title="Model name")
-    vae_model: Optional[str] = Field(None, title="VAE model name")
     revision: Optional[str] = Field(None, title="Revision")
     tokenizer: Optional[str] = Field(None, title="Tokenizer, if different from model")
     image_path: str = Field(None, title="Image path")
     class_image_path: Optional[str] = Field(None, title="Class image path")
     prompt: str = Field(None, title="Instance prompt")
     class_prompt: Optional[str] = Field(None, title="Class prompt")
     num_class_images: int = Field(100, title="Number of class images")
@@ -31,15 +30,15 @@
     num_steps: int = Field(None, title="Max train steps")
     checkpointing_steps: int = Field(500, title="Checkpointing steps")
     resume_from_checkpoint: Optional[str] = Field(None, title="Resume from checkpoint")
 
     gradient_accumulation: int = Field(1, title="Gradient accumulation steps")
     disable_gradient_checkpointing: bool = Field(False, title="Gradient checkpointing")
 
-    lr: float = Field(1e-4, title="Learning rate")
+    lr: float = Field(5e-4, title="Learning rate")
     scale_lr: bool = Field(False, title="Scale learning rate")
     scheduler: str = Field("constant", title="Learning rate scheduler")
     warmup_steps: int = Field(0, title="Learning rate warmup steps")
     num_cycles: int = Field(1, title="Learning rate num cycles")
     lr_power: float = Field(1.0, title="Learning rate power")
 
     dataloader_num_workers: int = Field(0, title="Dataloader num workers")
@@ -57,17 +56,19 @@
     pre_compute_text_embeddings: bool = Field(False, title="Pre compute text embeddings")
     tokenizer_max_length: Optional[int] = Field(None, title="Tokenizer max length")
     text_encoder_use_attention_mask: bool = Field(False, title="Text encoder use attention mask")
 
     rank: int = Field(4, title="Rank")
     xl: bool = Field(False, title="XL")
 
-    mixed_precision: Optional[str] = Field(None, title="Mixed precision")
+    fp16: bool = Field(False, title="FP16")
+    bf16: bool = Field(False, title="BF16")
 
     token: Optional[str] = Field(None, title="Hub token")
+    repo_id: Optional[str] = Field(None, title="Hub model id")
     push_to_hub: bool = Field(False, title="Push to hub")
     username: Optional[str] = Field(None, title="Hub username")
 
     # disabled:
     validation_prompt: Optional[str] = Field(None, title="Validation prompt")
     num_validation_images: int = Field(4, title="Number of validation images")
     validation_epochs: int = Field(50, title="Validation epochs")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
                     text_encoder_lora_layers=text_encoder_lora_layers_1,
                     safe_serialization=True,
                 )
         self.accelerator.end_training()
 
     def push_to_hub(self):
         repo_id = create_repo(
-            repo_id=f"{self.config.username}/{self.config.project_name}",
+            repo_id=self.config.repo_id,
             exist_ok=True,
             private=True,
             token=self.config.token,
         ).repo_id
 
         utils.create_model_card(
             repo_id,
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/generic/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 
 class GenericParams(AutoTrainParams):
     username: str = Field(None, title="Hugging Face Username")
     project_name: str = Field("project-name", title="path to script.py")
     data_path: str = Field(None, title="Data path")
     token: str = Field(None, title="Hub Token")
     script_path: str = Field(None, title="Script path")
+    repo_id: Optional[str] = Field(None, title="Repo ID")
     env: Optional[Dict[str, str]] = Field(None, title="Environment Variables")
     args: Optional[Dict[str, str]] = Field(None, title="Arguments")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/generic/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import subprocess
 
 import requests
 from huggingface_hub import HfApi, snapshot_download
-
-from autotrain import logger
+from loguru import logger
 
 
 def create_dataset_repo(username, project_name, script_path, token):
     logger.info("Creating dataset repo...")
     api = HfApi(token=token)
     repo_id = f"{username}/autotrain-{project_name}"
     api.create_repo(
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,17 @@
     AutoConfig,
     AutoImageProcessor,
     AutoModelForImageClassification,
     EarlyStoppingCallback,
     Trainer,
     TrainingArguments,
 )
-from transformers.trainer_callback import PrinterCallback
 
 from autotrain import logger
-from autotrain.trainers.common import (
-    ALLOW_REMOTE_CODE,
-    LossLoggingCallback,
-    TrainStartCallback,
-    UploadLogs,
-    monitor,
-    pause_space,
-    remove_autotrain_data,
-    save_training_params,
-)
+from autotrain.trainers.common import monitor, pause_space, remove_autotrain_data, save_training_params
 from autotrain.trainers.image_classification import utils
 from autotrain.trainers.image_classification.params import ImageClassificationParams
 
 
 def parse_args():
     # get training_config.json from the end user
     parser = argparse.ArgumentParser()
@@ -37,14 +27,18 @@
 
 
 @monitor
 def train(config):
     if isinstance(config, dict):
         config = ImageClassificationParams(**config)
 
+    if PartialState().process_index == 0:
+        logger.info("Starting training...")
+        logger.info(f"Training config: {config}")
+
     valid_data = None
     if config.data_path == f"{config.project_name}/autotrain-data":
         train_data = load_from_disk(config.data_path)[config.train_split]
     else:
         train_data = load_dataset(
             config.data_path,
             split=config.train_split,
@@ -84,56 +78,52 @@
     model_config.label2id = label2id
     model_config.id2label = {v: k for k, v in label2id.items()}
 
     try:
         model = AutoModelForImageClassification.from_pretrained(
             config.model,
             config=model_config,
-            trust_remote_code=ALLOW_REMOTE_CODE,
+            trust_remote_code=True,
             token=config.token,
             ignore_mismatched_sizes=True,
         )
     except OSError:
         model = AutoModelForImageClassification.from_pretrained(
             config.model,
             config=model_config,
             from_tf=True,
-            trust_remote_code=ALLOW_REMOTE_CODE,
+            trust_remote_code=True,
             token=config.token,
             ignore_mismatched_sizes=True,
         )
 
     image_processor = AutoImageProcessor.from_pretrained(config.model, token=config.token)
     train_data, valid_data = utils.process_data(train_data, valid_data, image_processor, config)
 
     if config.logging_steps == -1:
         if config.valid_split is not None:
             logging_steps = int(0.2 * len(valid_data) / config.batch_size)
         else:
             logging_steps = int(0.2 * len(train_data) / config.batch_size)
         if logging_steps == 0:
             logging_steps = 1
-        if logging_steps > 25:
-            logging_steps = 25
-        config.logging_steps = logging_steps
+
     else:
         logging_steps = config.logging_steps
 
-    logger.info(f"Logging steps: {logging_steps}")
-
     training_args = dict(
         output_dir=config.project_name,
         per_device_train_batch_size=config.batch_size,
         per_device_eval_batch_size=2 * config.batch_size,
         learning_rate=config.lr,
         num_train_epochs=config.epochs,
         evaluation_strategy=config.evaluation_strategy if config.valid_split is not None else "no",
         logging_steps=logging_steps,
         save_total_limit=config.save_total_limit,
-        save_strategy=config.evaluation_strategy if config.valid_split is not None else "no",
+        save_strategy=config.save_strategy,
         gradient_accumulation_steps=config.gradient_accumulation,
         report_to=config.log,
         auto_find_batch_size=config.auto_find_batch_size,
         lr_scheduler_type=config.scheduler,
         optim=config.optimizer,
         warmup_ratio=config.warmup_ratio,
         weight_decay=config.weight_decay,
@@ -150,16 +140,14 @@
 
     if config.valid_split is not None:
         early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
-    callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
-
     args = TrainingArguments(**training_args)
     trainer_args = dict(
         args=args,
         model=model,
         callbacks=callbacks_to_use,
         compute_metrics=(
             utils._binary_classification_metrics if num_classes == 2 else utils._multi_class_classification_metrics
@@ -167,15 +155,14 @@
     )
 
     trainer = Trainer(
         **trainer_args,
         train_dataset=train_data,
         eval_dataset=valid_data,
     )
-    trainer.remove_callback(PrinterCallback)
     trainer.train()
 
     logger.info("Finished training, saving model...")
     trainer.save_model(config.project_name)
     image_processor.save_pretrained(config.project_name)
 
     model_card = utils.create_model_card(config, trainer, num_classes)
@@ -186,20 +173,16 @@
 
     if config.push_to_hub:
         if PartialState().process_index == 0:
             remove_autotrain_data(config)
             save_training_params(config)
             logger.info("Pushing model to hub...")
             api = HfApi(token=config.token)
-            api.create_repo(
-                repo_id=f"{config.username}/{config.project_name}", repo_type="model", private=True, exist_ok=True
-            )
-            api.upload_folder(
-                folder_path=config.project_name, repo_id=f"{config.username}/{config.project_name}", repo_type="model"
-            )
+            api.create_repo(repo_id=config.repo_id, repo_type="model", private=True)
+            api.upload_folder(folder_path=config.project_name, repo_id=config.repo_id, repo_type="model")
 
     if PartialState().process_index == 0:
         pause_space(config)
 
 
 if __name__ == "__main__":
     _args = parse_args()
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,13 +22,15 @@
     train_split: str = Field("train", title="Train split")
     valid_split: Optional[str] = Field(None, title="Validation split")
     logging_steps: int = Field(-1, title="Logging steps")
     project_name: str = Field("project-name", title="Output directory")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
+    save_strategy: str = Field("epoch", title="Save strategy")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
+    repo_id: Optional[str] = Field(None, title="Repo id")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     image_column: str = Field("image", title="Image column")
     target_column: str = Field("target", title="Target column")
     log: str = Field("none", title="Logging using experiment tracking")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/image_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import json
+import sys
 from functools import partial
 
 import torch
 from accelerate.state import PartialState
 from datasets import load_dataset, load_from_disk
 from huggingface_hub import HfApi
 from peft import LoraConfig, TaskType, get_peft_model, prepare_model_for_kbit_training
@@ -13,27 +14,17 @@
     AutoTokenizer,
     BitsAndBytesConfig,
     DataCollatorForSeq2Seq,
     EarlyStoppingCallback,
     Seq2SeqTrainer,
     Seq2SeqTrainingArguments,
 )
-from transformers.trainer_callback import PrinterCallback
 
 from autotrain import logger
-from autotrain.trainers.common import (
-    ALLOW_REMOTE_CODE,
-    LossLoggingCallback,
-    TrainStartCallback,
-    UploadLogs,
-    monitor,
-    pause_space,
-    remove_autotrain_data,
-    save_training_params,
-)
+from autotrain.trainers.common import monitor, pause_space, remove_autotrain_data, save_training_params
 from autotrain.trainers.seq2seq import utils
 from autotrain.trainers.seq2seq.dataset import Seq2SeqDataset
 from autotrain.trainers.seq2seq.params import Seq2SeqParams
 
 
 def parse_args():
     # get training_config.json from the end user
@@ -43,14 +34,21 @@
 
 
 @monitor
 def train(config):
     if isinstance(config, dict):
         config = Seq2SeqParams(**config)
 
+    if config.repo_id is None and config.username is not None:
+        config.repo_id = f"{config.username}/{config.project_name}"
+
+    if PartialState().process_index == 0:
+        logger.info("Starting training...")
+        logger.info(f"Training config: {config}")
+
     train_data = None
     valid_data = None
     # check if config.train_split.csv exists in config.data_path
     if config.train_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
             train_data = load_from_disk(config.data_path)[config.train_split]
@@ -68,47 +66,94 @@
         else:
             valid_data = load_dataset(
                 config.data_path,
                 split=config.valid_split,
                 token=config.token,
             )
 
-    tokenizer = AutoTokenizer.from_pretrained(config.model, token=config.token, trust_remote_code=ALLOW_REMOTE_CODE)
+    model_config = AutoConfig.from_pretrained(config.model, token=config.token, trust_remote_code=True)
+
+    if config.peft:
+        if config.quantization == "int4":
+            raise NotImplementedError("int4 quantization is not supported")
+        # if config.use_int4:
+        #     bnb_config = BitsAndBytesConfig(
+        #         load_in_4bit=config.use_int4,
+        #         bnb_4bit_quant_type="nf4",
+        #         bnb_4bit_compute_dtype=torch.float16,
+        #         bnb_4bit_use_double_quant=False,
+        #     )
+        #     config.fp16 = True
+        if config.quantization == "int8":
+            bnb_config = BitsAndBytesConfig(load_in_8bit=True)
+        else:
+            bnb_config = None
+
+        model = AutoModelForSeq2SeqLM.from_pretrained(
+            config.model,
+            config=model_config,
+            token=config.token,
+            quantization_config=bnb_config,
+            trust_remote_code=True,
+        )
+    else:
+        model = AutoModelForSeq2SeqLM.from_pretrained(
+            config.model,
+            config=model_config,
+            token=config.token,
+            trust_remote_code=True,
+        )
+
+    tokenizer = AutoTokenizer.from_pretrained(config.model, token=config.token, trust_remote_code=True)
+
+    embedding_size = model.get_input_embeddings().weight.shape[0]
+    if len(tokenizer) > embedding_size:
+        model.resize_token_embeddings(len(tokenizer))
+
+    if config.peft:
+        lora_config = LoraConfig(
+            r=config.lora_r,
+            lora_alpha=config.lora_alpha,
+            target_modules=None if len(config.target_modules) == 0 else config.target_modules,
+            lora_dropout=config.lora_dropout,
+            bias="none",
+            task_type=TaskType.SEQ_2_SEQ_LM,
+        )
+        if config.quantization is not None:
+            model = prepare_model_for_kbit_training(model)
+
+        model = get_peft_model(model, lora_config)
 
     train_data = Seq2SeqDataset(data=train_data, tokenizer=tokenizer, config=config)
     if config.valid_split is not None:
         valid_data = Seq2SeqDataset(data=valid_data, tokenizer=tokenizer, config=config)
 
     if config.logging_steps == -1:
         if config.valid_split is not None:
             logging_steps = int(0.2 * len(valid_data) / config.batch_size)
         else:
             logging_steps = int(0.2 * len(train_data) / config.batch_size)
         if logging_steps == 0:
             logging_steps = 1
-        if logging_steps > 25:
-            logging_steps = 25
-        config.logging_steps = logging_steps
+
     else:
         logging_steps = config.logging_steps
 
-    logger.info(f"Logging steps: {logging_steps}")
-
     training_args = dict(
         output_dir=config.project_name,
         per_device_train_batch_size=config.batch_size,
         per_device_eval_batch_size=2 * config.batch_size,
         learning_rate=config.lr,
         num_train_epochs=config.epochs,
         evaluation_strategy=config.evaluation_strategy if config.valid_split is not None else "no",
         logging_steps=logging_steps,
         save_total_limit=config.save_total_limit,
-        save_strategy=config.evaluation_strategy if config.valid_split is not None else "no",
+        save_strategy=config.save_strategy,
         gradient_accumulation_steps=config.gradient_accumulation,
-        report_to=config.log,
+        report_to="tensorboard",
         auto_find_batch_size=config.auto_find_batch_size,
         lr_scheduler_type=config.scheduler,
         optim=config.optimizer,
         warmup_ratio=config.warmup_ratio,
         weight_decay=config.weight_decay,
         max_grad_norm=config.max_grad_norm,
         push_to_hub=False,
@@ -125,81 +170,16 @@
 
     if config.valid_split is not None:
         early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
-    callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
-
     args = Seq2SeqTrainingArguments(**training_args)
-
-    model_config = AutoConfig.from_pretrained(
-        config.model,
-        token=config.token,
-        trust_remote_code=ALLOW_REMOTE_CODE,
-        use_cache=False,
-    )
-
-    if config.peft:
-        if config.quantization == "int4":
-            raise NotImplementedError("int4 quantization is not supported")
-        # if config.use_int4:
-        #     bnb_config = BitsAndBytesConfig(
-        #         load_in_4bit=config.use_int4,
-        #         bnb_4bit_quant_type="nf4",
-        #         bnb_4bit_compute_dtype=torch.float16,
-        #         bnb_4bit_use_double_quant=False,
-        #     )
-        #     config.fp16 = True
-        if config.quantization == "int8":
-            bnb_config = BitsAndBytesConfig(load_in_8bit=True)
-        else:
-            bnb_config = None
-
-        model = AutoModelForSeq2SeqLM.from_pretrained(
-            config.model,
-            config=model_config,
-            token=config.token,
-            quantization_config=bnb_config,
-            trust_remote_code=ALLOW_REMOTE_CODE,
-        )
-    else:
-        model = AutoModelForSeq2SeqLM.from_pretrained(
-            config.model,
-            config=model_config,
-            token=config.token,
-            trust_remote_code=ALLOW_REMOTE_CODE,
-        )
-
-    embedding_size = model.get_input_embeddings().weight.shape[0]
-    if len(tokenizer) > embedding_size:
-        model.resize_token_embeddings(len(tokenizer))
-
-    if config.peft:
-        target_modules = config.target_modules.split(",") if config.target_modules is not None else None
-        if target_modules:
-            target_modules = [module.strip() for module in target_modules]
-        if len(target_modules) == 1 and target_modules[0] == "all-linear":
-            target_modules = "all-linear"
-        lora_config = LoraConfig(
-            r=config.lora_r,
-            lora_alpha=config.lora_alpha,
-            target_modules=target_modules,
-            lora_dropout=config.lora_dropout,
-            bias="none",
-            task_type=TaskType.SEQ_2_SEQ_LM,
-        )
-        if config.quantization is not None:
-            model = prepare_model_for_kbit_training(model)
-
-        model = get_peft_model(model, lora_config)
-
     _s2s_metrics = partial(utils._seq2seq_metrics, tokenizer=tokenizer)
-
     trainer_args = dict(
         args=args,
         model=model,
         callbacks=callbacks_to_use,
         compute_metrics=_s2s_metrics,
     )
     data_collator = DataCollatorForSeq2Seq(tokenizer, model=model)
@@ -207,48 +187,49 @@
         **trainer_args,
         train_dataset=train_data,
         eval_dataset=valid_data,
         data_collator=data_collator,
         tokenizer=tokenizer,
     )
 
+    model.config.use_cache = False
+
+    if torch.__version__ >= "2" and sys.platform != "win32":
+        model = torch.compile(model)
+
     for name, module in trainer.model.named_modules():
         if "norm" in name:
             module = module.to(torch.float32)
-
-    trainer.remove_callback(PrinterCallback)
     trainer.train()
 
     logger.info("Finished training, saving model...")
-    trainer.model.config.use_cache = True
     trainer.save_model(config.project_name)
+    tokenizer.save_pretrained(config.project_name)
 
     model_card = utils.create_model_card(config, trainer)
 
     # save model card to output directory as README.md
-    with open(f"{config.project_name}/README.md", "w", encoding="utf-8") as f:
+    with open(f"{config.project_name}/README.md", "w") as f:
         f.write(model_card)
 
     if config.push_to_hub:
         if PartialState().process_index == 0:
             remove_autotrain_data(config)
             save_training_params(config)
             logger.info("Pushing model to hub...")
             api = HfApi(token=config.token)
-            api.create_repo(
-                repo_id=f"{config.username}/{config.project_name}", repo_type="model", private=True, exist_ok=True
-            )
+            api.create_repo(repo_id=config.repo_id, repo_type="model", private=True)
             api.upload_folder(
                 folder_path=config.project_name,
-                repo_id=f"{config.username}/{config.project_name}",
+                repo_id=config.repo_id,
                 repo_type="model",
             )
 
     if PartialState().process_index == 0:
         pause_space(config)
 
 
 if __name__ == "__main__":
-    _args = parse_args()
-    training_config = json.load(open(_args.training_config))
+    args = parse_args()
+    training_config = json.load(open(args.training_config))
     config = Seq2SeqParams(**training_config)
     train(config)
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import List, Optional
 
 from pydantic import Field
 
 from autotrain.trainers.common import AutoTrainParams
 
 
 class Seq2SeqParams(AutoTrainParams):
@@ -13,32 +13,33 @@
     train_split: str = Field("train", title="Train split")
     valid_split: Optional[str] = Field(None, title="Validation split")
     project_name: str = Field("project-name", title="Output directory")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
     text_column: str = Field("text", title="Text column")
     target_column: str = Field("target", title="Target text column")
+    repo_id: Optional[str] = Field(None, title="Repo ID")
     lr: float = Field(5e-5, title="Learning rate")
     epochs: int = Field(3, title="Number of training epochs")
     max_seq_length: int = Field(128, title="Max sequence length")
     max_target_length: int = Field(128, title="Max target sequence length")
-    batch_size: int = Field(2, title="Training batch size")
+    batch_size: int = Field(8, title="Training batch size")
     warmup_ratio: float = Field(0.1, title="Warmup proportion")
     gradient_accumulation: int = Field(1, title="Gradient accumulation steps")
     optimizer: str = Field("adamw_torch", title="Optimizer")
     scheduler: str = Field("linear", title="Scheduler")
     weight_decay: float = Field(0.0, title="Weight decay")
     max_grad_norm: float = Field(1.0, title="Max gradient norm")
     logging_steps: int = Field(-1, title="Logging steps")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
+    save_strategy: str = Field("epoch", title="Save strategy")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
     peft: bool = Field(False, title="Use PEFT")
-    quantization: Optional[str] = Field("int4", title="int4, int8, or None")
+    quantization: Optional[str] = Field(None, title="int4, int8, or None")
     lora_r: int = Field(16, title="LoRA-R")
     lora_alpha: int = Field(32, title="LoRA-Alpha")
     lora_dropout: float = Field(0.05, title="LoRA-Dropout")
-    target_modules: str = Field("all-linear", title="Target modules for PEFT")
-    log: str = Field("none", title="Logging using experiment tracking")
+    target_modules: List[str] = Field(["all-linear"], title="Target modules for PEFT")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/seq2seq/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,17 @@
 
 
 @monitor
 def train(config):
     if isinstance(config, dict):
         config = TabularParams(**config)
 
+    if config.repo_id is None and config.username is not None:
+        config.repo_id = f"{config.username}/{config.project_name}"
+
     logger.info("Starting training...")
     logger.info(f"Training config: {config}")
 
     train_data = None
     valid_data = None
     if config.data_path == f"{config.project_name}/autotrain-data":
         logger.info("loading dataset from disk")
@@ -321,18 +324,16 @@
         f.write(model_card)
 
     if config.push_to_hub:
         remove_autotrain_data(config)
         save_training_params(config)
         logger.info("Pushing model to hub...")
         api = HfApi(token=config.token)
-        api.create_repo(repo_id=f"{config.username}/{config.project_name}", repo_type="model", private=True)
-        api.upload_folder(
-            folder_path=config.project_name, repo_id=f"{config.username}/{config.project_name}", repo_type="model"
-        )
+        api.create_repo(repo_id=config.repo_id, repo_type="model", private=True)
+        api.upload_folder(folder_path=config.project_name, repo_id=config.repo_id, repo_type="model")
 
     pause_space(config)
 
 
 if __name__ == "__main__":
     args = parse_args()
     training_config = json.load(open(args.training_config))
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     train_split: str = Field("train", title="Train split")
     valid_split: Optional[str] = Field(None, title="Validation split")
     project_name: str = Field("project-name", title="Output directory")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
     id_column: str = Field("id", title="ID column")
     target_columns: Union[List[str], str] = Field(["target"], title="Target column(s)")
+    repo_id: Optional[str] = Field(None, title="Repo ID")
     categorical_columns: Optional[List[str]] = Field(None, title="Categorical columns")
     numerical_columns: Optional[List[str]] = Field(None, title="Numerical columns")
     task: str = Field("classification", title="Task")
     num_trials: int = Field(10, title="Number of trials")
     time_limit: int = Field(600, title="Time limit")
     categorical_imputer: Optional[str] = Field(None, title="Categorical imputer")
     numerical_imputer: Optional[str] = Field(None, title="Numerical imputer")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 import argparse
 import json
+from functools import partial
 
 from accelerate.state import PartialState
 from datasets import load_dataset, load_from_disk
 from huggingface_hub import HfApi
 from transformers import (
     AutoConfig,
-    AutoModelForSequenceClassification,
+    AutoModelForTokenClassification,
     AutoTokenizer,
     EarlyStoppingCallback,
     Trainer,
     TrainingArguments,
 )
-from transformers.trainer_callback import PrinterCallback
 
 from autotrain import logger
-from autotrain.trainers.common import (
-    ALLOW_REMOTE_CODE,
-    LossLoggingCallback,
-    TrainStartCallback,
-    UploadLogs,
-    monitor,
-    pause_space,
-    remove_autotrain_data,
-    save_training_params,
-)
-from autotrain.trainers.text_classification import utils
-from autotrain.trainers.text_classification.dataset import TextClassificationDataset
-from autotrain.trainers.text_classification.params import TextClassificationParams
+from autotrain.trainers.common import monitor, pause_space, remove_autotrain_data, save_training_params
+from autotrain.trainers.token_classification import utils
+from autotrain.trainers.token_classification.dataset import TokenClassificationDataset
+from autotrain.trainers.token_classification.params import TokenClassificationParams
 
 
 def parse_args():
     # get training_config.json from the end user
     parser = argparse.ArgumentParser()
     parser.add_argument("--training_config", type=str, required=True)
     return parser.parse_args()
 
 
 @monitor
 def train(config):
     if isinstance(config, dict):
-        config = TextClassificationParams(**config)
+        config = TokenClassificationParams(**config)
+
+    if config.repo_id is None and config.username is not None:
+        config.repo_id = f"{config.username}/{config.project_name}"
+
+    if PartialState().process_index == 0:
+        logger.info("Starting training...")
+        logger.info(f"Training config: {config}")
 
     train_data = None
     valid_data = None
     # check if config.train_split.csv exists in config.data_path
     if config.train_split is not None:
         if config.data_path == f"{config.project_name}/autotrain-data":
             logger.info("loading dataset from disk")
@@ -63,81 +61,72 @@
         else:
             valid_data = load_dataset(
                 config.data_path,
                 split=config.valid_split,
                 token=config.token,
             )
 
-    classes = train_data.features[config.target_column].names
-    label2id = {c: i for i, c in enumerate(classes)}
-    num_classes = len(classes)
-
-    if num_classes < 2:
-        raise ValueError("Invalid number of classes. Must be greater than 1.")
-
-    if config.valid_split is not None:
-        num_classes_valid = len(valid_data.unique(config.target_column))
-        if num_classes_valid != num_classes:
-            raise ValueError(
-                f"Number of classes in train and valid are not the same. Training has {num_classes} and valid has {num_classes_valid}"
-            )
+    label_list = train_data.features[config.tags_column].feature.names
+    num_classes = len(label_list)
 
     model_config = AutoConfig.from_pretrained(config.model, num_labels=num_classes)
-    model_config._num_labels = len(label2id)
-    model_config.label2id = label2id
-    model_config.id2label = {v: k for k, v in label2id.items()}
+    model_config._num_labels = num_classes
+    model_config.label2id = {l: i for i, l in enumerate(label_list)}
+    model_config.id2label = dict(enumerate(label_list))
 
     try:
-        model = AutoModelForSequenceClassification.from_pretrained(
+        model = AutoModelForTokenClassification.from_pretrained(
             config.model,
             config=model_config,
-            trust_remote_code=ALLOW_REMOTE_CODE,
+            trust_remote_code=True,
             token=config.token,
             ignore_mismatched_sizes=True,
         )
     except OSError:
-        model = AutoModelForSequenceClassification.from_pretrained(
+        model = AutoModelForTokenClassification.from_pretrained(
             config.model,
             config=model_config,
             from_tf=True,
-            trust_remote_code=ALLOW_REMOTE_CODE,
+            trust_remote_code=True,
             token=config.token,
             ignore_mismatched_sizes=True,
         )
 
-    tokenizer = AutoTokenizer.from_pretrained(config.model, token=config.token, trust_remote_code=ALLOW_REMOTE_CODE)
-    train_data = TextClassificationDataset(data=train_data, tokenizer=tokenizer, config=config)
+    if model_config.model_type in {"bloom", "gpt2", "roberta"}:
+        tokenizer = AutoTokenizer.from_pretrained(
+            config.model, token=config.token, trust_remote_code=True, add_prefix_space=True
+        )
+    else:
+        tokenizer = AutoTokenizer.from_pretrained(config.model, token=config.token, trust_remote_code=True)
+
+    train_data = TokenClassificationDataset(data=train_data, tokenizer=tokenizer, config=config)
     if config.valid_split is not None:
-        valid_data = TextClassificationDataset(data=valid_data, tokenizer=tokenizer, config=config)
+        valid_data = TokenClassificationDataset(data=valid_data, tokenizer=tokenizer, config=config)
 
     if config.logging_steps == -1:
         if config.valid_split is not None:
             logging_steps = int(0.2 * len(valid_data) / config.batch_size)
         else:
             logging_steps = int(0.2 * len(train_data) / config.batch_size)
         if logging_steps == 0:
             logging_steps = 1
-        if logging_steps > 25:
-            logging_steps = 25
-        config.logging_steps = logging_steps
+
     else:
         logging_steps = config.logging_steps
 
-    logger.info(f"Logging steps: {logging_steps}")
-
     training_args = dict(
         output_dir=config.project_name,
         per_device_train_batch_size=config.batch_size,
         per_device_eval_batch_size=2 * config.batch_size,
         learning_rate=config.lr,
         num_train_epochs=config.epochs,
         evaluation_strategy=config.evaluation_strategy if config.valid_split is not None else "no",
         logging_steps=logging_steps,
         save_total_limit=config.save_total_limit,
-        save_strategy=config.evaluation_strategy if config.valid_split is not None else "no",
+        save_strategy=config.save_strategy,
         gradient_accumulation_steps=config.gradient_accumulation,
         report_to=config.log,
         auto_find_batch_size=config.auto_find_batch_size,
         lr_scheduler_type=config.scheduler,
         optim=config.optimizer,
         warmup_ratio=config.warmup_ratio,
         weight_decay=config.weight_decay,
@@ -154,61 +143,54 @@
 
     if config.valid_split is not None:
         early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
-    callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
-
     args = TrainingArguments(**training_args)
     trainer_args = dict(
         args=args,
         model=model,
         callbacks=callbacks_to_use,
-        compute_metrics=(
-            utils._binary_classification_metrics if num_classes == 2 else utils._multi_class_classification_metrics
-        ),
+        compute_metrics=partial(utils.token_classification_metrics, label_list=label_list),
     )
 
     trainer = Trainer(
         **trainer_args,
         train_dataset=train_data,
         eval_dataset=valid_data,
     )
-    trainer.remove_callback(PrinterCallback)
     trainer.train()
 
     logger.info("Finished training, saving model...")
     trainer.save_model(config.project_name)
     tokenizer.save_pretrained(config.project_name)
 
-    model_card = utils.create_model_card(config, trainer, num_classes)
+    model_card = utils.create_model_card(config, trainer)
 
     # save model card to output directory as README.md
-    with open(f"{config.project_name}/README.md", "w") as f:
+    with open(f"{config.project_name}/README.md", "w", encoding="utf-8") as f:
         f.write(model_card)
 
     if config.push_to_hub:
         if PartialState().process_index == 0:
             remove_autotrain_data(config)
             save_training_params(config)
             logger.info("Pushing model to hub...")
             api = HfApi(token=config.token)
-            api.create_repo(
-                repo_id=f"{config.username}/{config.project_name}", repo_type="model", private=True, exist_ok=True
-            )
+            api.create_repo(repo_id=config.repo_id, repo_type="model", private=True)
             api.upload_folder(
                 folder_path=config.project_name,
-                repo_id=f"{config.username}/{config.project_name}",
+                repo_id=config.repo_id,
                 repo_type="model",
             )
 
     if PartialState().process_index == 0:
         pause_space(config)
 
 
 if __name__ == "__main__":
     args = parse_args()
     training_config = json.load(open(args.training_config))
-    config = TextClassificationParams(**training_config)
+    config = TokenClassificationParams(**training_config)
     train(config)
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from pydantic import Field
 
 from autotrain.trainers.common import AutoTrainParams
 
 
-class TextClassificationParams(AutoTrainParams):
+class TokenClassificationParams(AutoTrainParams):
     data_path: str = Field(None, title="Data path")
     model: str = Field("bert-base-uncased", title="Model name")
     lr: float = Field(5e-5, title="Learning rate")
     epochs: int = Field(3, title="Number of training epochs")
     max_seq_length: int = Field(128, title="Max sequence length")
     batch_size: int = Field(8, title="Training batch size")
     warmup_ratio: float = Field(0.1, title="Warmup proportion")
@@ -17,19 +17,21 @@
     optimizer: str = Field("adamw_torch", title="Optimizer")
     scheduler: str = Field("linear", title="Scheduler")
     weight_decay: float = Field(0.0, title="Weight decay")
     max_grad_norm: float = Field(1.0, title="Max gradient norm")
     seed: int = Field(42, title="Seed")
     train_split: str = Field("train", title="Train split")
     valid_split: Optional[str] = Field(None, title="Validation split")
-    text_column: str = Field("text", title="Text column")
-    target_column: str = Field("target", title="Target column")
+    tokens_column: str = Field("tokens", title="Tokens column")
+    tags_column: str = Field("tags", title="Tags column")
     logging_steps: int = Field(-1, title="Logging steps")
     project_name: str = Field("project-name", title="Output directory")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
+    save_strategy: str = Field("epoch", title="Save strategy")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
+    repo_id: Optional[str] = Field(None, title="Repo id")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     username: Optional[str] = Field(None, title="Hugging Face Username")
     log: str = Field("none", title="Logging using experiment tracking")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/text_regression/params.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/text_classification/params.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from pydantic import Field
 
 from autotrain.trainers.common import AutoTrainParams
 
 
-class TextRegressionParams(AutoTrainParams):
+class TextClassificationParams(AutoTrainParams):
     data_path: str = Field(None, title="Data path")
     model: str = Field("bert-base-uncased", title="Model name")
     lr: float = Field(5e-5, title="Learning rate")
     epochs: int = Field(3, title="Number of training epochs")
     max_seq_length: int = Field(128, title="Max sequence length")
     batch_size: int = Field(8, title="Training batch size")
     warmup_ratio: float = Field(0.1, title="Warmup proportion")
@@ -18,18 +18,20 @@
     scheduler: str = Field("linear", title="Scheduler")
     weight_decay: float = Field(0.0, title="Weight decay")
     max_grad_norm: float = Field(1.0, title="Max gradient norm")
     seed: int = Field(42, title="Seed")
     train_split: str = Field("train", title="Train split")
     valid_split: Optional[str] = Field(None, title="Validation split")
     text_column: str = Field("text", title="Text column")
-    target_column: str = Field("target", title="Target column(s)")
+    target_column: str = Field("target", title="Target column")
     logging_steps: int = Field(-1, title="Logging steps")
     project_name: str = Field("project-name", title="Output directory")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
+    save_strategy: str = Field("epoch", title="Save strategy")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
+    repo_id: Optional[str] = Field(None, title="Repo id")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     username: Optional[str] = Field(None, title="Hugging Face Username")
     log: str = Field("none", title="Logging using experiment tracking")
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.86/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.9/src/autotrain/trainers/token_classification/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
-from seqeval import metrics
+from datasets import load_metric
 
 
+_METRICS = load_metric("seqeval")
+
 MODEL_CARD = """
 ---
 tags:
 - autotrain
 - token-classification
 widget:
 - text: "I love AutoTrain"
@@ -31,19 +33,20 @@
         for prediction, label in zip(predictions, labels)
     ]
     true_labels = [
         [label_list[lbl] for (predi, lbl) in zip(prediction, label) if lbl != -100]
         for prediction, label in zip(predictions, labels)
     ]
 
+    results = _METRICS.compute(predictions=true_predictions, references=true_labels)
     results = {
-        "precision": metrics.precision_score(true_labels, true_predictions),
-        "recall": metrics.recall_score(true_labels, true_predictions),
-        "f1": metrics.f1_score(true_labels, true_predictions),
-        "accuracy": metrics.accuracy_score(true_labels, true_predictions),
+        "precision": results["overall_precision"],
+        "recall": results["overall_recall"],
+        "f1": results["overall_f1"],
+        "accuracy": results["overall_accuracy"],
     }
     return results
 
 
 def create_model_card(config, trainer):
     if config.valid_split is not None:
         eval_scores = trainer.evaluate()
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.86
+Version: 0.7.9
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,212 +16,200 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: albumentations==1.4.4
-Requires-Dist: codecarbon==2.3.5
-Requires-Dist: datasets[vision]~=2.19.0
-Requires-Dist: evaluate==0.4.1
+Requires-Dist: albumentations==1.3.1
+Requires-Dist: codecarbon==2.2.3
+Requires-Dist: datasets[vision]~=2.14.0
+Requires-Dist: evaluate==0.3.0
 Requires-Dist: ipadic==1.0.0
-Requires-Dist: jiwer==3.0.3
-Requires-Dist: joblib==1.4.0
-Requires-Dist: loguru==0.7.2
-Requires-Dist: pandas==2.2.2
+Requires-Dist: jiwer==3.0.2
+Requires-Dist: joblib==1.3.1
+Requires-Dist: loguru==0.7.0
+Requires-Dist: pandas>=1.4
 Requires-Dist: nltk==3.8.1
-Requires-Dist: optuna==3.6.1
-Requires-Dist: Pillow==10.3.0
+Requires-Dist: optuna==3.3.0
+Requires-Dist: Pillow==10.0.0
 Requires-Dist: protobuf==4.23.4
-Requires-Dist: sacremoses==0.1.1
-Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: sentencepiece==0.2.0
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: werkzeug==3.0.2
-Requires-Dist: xgboost==2.0.3
-Requires-Dist: huggingface_hub==0.22.2
+Requires-Dist: sacremoses==0.0.53
+Requires-Dist: scikit-learn==1.3.0
+Requires-Dist: sentencepiece==0.1.99
+Requires-Dist: tqdm==4.65.0
+Requires-Dist: werkzeug==2.3.6
+Requires-Dist: xgboost==1.7.6
+Requires-Dist: huggingface_hub>=0.16.4
 Requires-Dist: requests==2.31.0
-Requires-Dist: einops==0.7.0
+Requires-Dist: einops==0.6.1
 Requires-Dist: invisible-watermark==0.2.0
-Requires-Dist: packaging==24.0
-Requires-Dist: cryptography==42.0.5
-Requires-Dist: nvitop==1.3.2
-Requires-Dist: tensorboard==2.16.2
-Requires-Dist: peft==0.10.0
-Requires-Dist: trl==0.8.6
+Requires-Dist: packaging==23.1
+Requires-Dist: tensorboard
+Requires-Dist: peft==0.9.0
+Requires-Dist: trl==0.7.11
 Requires-Dist: tiktoken==0.6.0
-Requires-Dist: transformers==4.40.1
-Requires-Dist: accelerate==0.29.3
-Requires-Dist: diffusers==0.27.2
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux"
+Requires-Dist: transformers==4.38.2
+Requires-Dist: accelerate==0.27.2
+Requires-Dist: diffusers==0.26.3
+Requires-Dist: bitsandbytes==0.42.0
 Requires-Dist: rouge_score==0.1.2
-Requires-Dist: py7zr==0.21.0
-Requires-Dist: fastapi==0.110.2
-Requires-Dist: uvicorn==0.29.0
-Requires-Dist: python-multipart==0.0.9
-Requires-Dist: pydantic==2.7.1
+Requires-Dist: py7zr==0.20.6
+Requires-Dist: fastapi==0.104.1
+Requires-Dist: uvicorn==0.22.0
+Requires-Dist: python-multipart==0.0.6
+Requires-Dist: gradio==3.41.0
+Requires-Dist: pydantic==2.4.2
 Requires-Dist: hf-transfer
-Requires-Dist: pyngrok==7.1.6
+Requires-Dist: pyngrok==7.0.3
 Requires-Dist: authlib==1.3.0
-Requires-Dist: itsdangerous==2.2.0
+Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: seqeval==1.2.2
-Requires-Dist: httpx==0.27.0
-Requires-Dist: pyyaml==6.0.1
 Provides-Extra: dev
-Requires-Dist: albumentations==1.4.4; extra == "dev"
-Requires-Dist: codecarbon==2.3.5; extra == "dev"
-Requires-Dist: datasets[vision]~=2.19.0; extra == "dev"
-Requires-Dist: evaluate==0.4.1; extra == "dev"
+Requires-Dist: albumentations==1.3.1; extra == "dev"
+Requires-Dist: codecarbon==2.2.3; extra == "dev"
+Requires-Dist: datasets[vision]~=2.14.0; extra == "dev"
+Requires-Dist: evaluate==0.3.0; extra == "dev"
 Requires-Dist: ipadic==1.0.0; extra == "dev"
-Requires-Dist: jiwer==3.0.3; extra == "dev"
-Requires-Dist: joblib==1.4.0; extra == "dev"
-Requires-Dist: loguru==0.7.2; extra == "dev"
-Requires-Dist: pandas==2.2.2; extra == "dev"
+Requires-Dist: jiwer==3.0.2; extra == "dev"
+Requires-Dist: joblib==1.3.1; extra == "dev"
+Requires-Dist: loguru==0.7.0; extra == "dev"
+Requires-Dist: pandas>=1.4; extra == "dev"
 Requires-Dist: nltk==3.8.1; extra == "dev"
-Requires-Dist: optuna==3.6.1; extra == "dev"
-Requires-Dist: Pillow==10.3.0; extra == "dev"
+Requires-Dist: optuna==3.3.0; extra == "dev"
+Requires-Dist: Pillow==10.0.0; extra == "dev"
 Requires-Dist: protobuf==4.23.4; extra == "dev"
-Requires-Dist: sacremoses==0.1.1; extra == "dev"
-Requires-Dist: scikit-learn==1.4.2; extra == "dev"
-Requires-Dist: sentencepiece==0.2.0; extra == "dev"
-Requires-Dist: tqdm==4.66.2; extra == "dev"
-Requires-Dist: werkzeug==3.0.2; extra == "dev"
-Requires-Dist: xgboost==2.0.3; extra == "dev"
-Requires-Dist: huggingface_hub==0.22.2; extra == "dev"
+Requires-Dist: sacremoses==0.0.53; extra == "dev"
+Requires-Dist: scikit-learn==1.3.0; extra == "dev"
+Requires-Dist: sentencepiece==0.1.99; extra == "dev"
+Requires-Dist: tqdm==4.65.0; extra == "dev"
+Requires-Dist: werkzeug==2.3.6; extra == "dev"
+Requires-Dist: xgboost==1.7.6; extra == "dev"
+Requires-Dist: huggingface_hub>=0.16.4; extra == "dev"
 Requires-Dist: requests==2.31.0; extra == "dev"
-Requires-Dist: einops==0.7.0; extra == "dev"
+Requires-Dist: einops==0.6.1; extra == "dev"
 Requires-Dist: invisible-watermark==0.2.0; extra == "dev"
-Requires-Dist: packaging==24.0; extra == "dev"
-Requires-Dist: cryptography==42.0.5; extra == "dev"
-Requires-Dist: nvitop==1.3.2; extra == "dev"
-Requires-Dist: tensorboard==2.16.2; extra == "dev"
-Requires-Dist: peft==0.10.0; extra == "dev"
-Requires-Dist: trl==0.8.6; extra == "dev"
+Requires-Dist: packaging==23.1; extra == "dev"
+Requires-Dist: tensorboard; extra == "dev"
+Requires-Dist: peft==0.9.0; extra == "dev"
+Requires-Dist: trl==0.7.11; extra == "dev"
 Requires-Dist: tiktoken==0.6.0; extra == "dev"
-Requires-Dist: transformers==4.40.1; extra == "dev"
-Requires-Dist: accelerate==0.29.3; extra == "dev"
-Requires-Dist: diffusers==0.27.2; extra == "dev"
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux" and extra == "dev"
+Requires-Dist: transformers==4.38.2; extra == "dev"
+Requires-Dist: accelerate==0.27.2; extra == "dev"
+Requires-Dist: diffusers==0.26.3; extra == "dev"
+Requires-Dist: bitsandbytes==0.42.0; extra == "dev"
 Requires-Dist: rouge_score==0.1.2; extra == "dev"
-Requires-Dist: py7zr==0.21.0; extra == "dev"
-Requires-Dist: fastapi==0.110.2; extra == "dev"
-Requires-Dist: uvicorn==0.29.0; extra == "dev"
-Requires-Dist: python-multipart==0.0.9; extra == "dev"
-Requires-Dist: pydantic==2.7.1; extra == "dev"
+Requires-Dist: py7zr==0.20.6; extra == "dev"
+Requires-Dist: fastapi==0.104.1; extra == "dev"
+Requires-Dist: uvicorn==0.22.0; extra == "dev"
+Requires-Dist: python-multipart==0.0.6; extra == "dev"
+Requires-Dist: gradio==3.41.0; extra == "dev"
+Requires-Dist: pydantic==2.4.2; extra == "dev"
 Requires-Dist: hf-transfer; extra == "dev"
-Requires-Dist: pyngrok==7.1.6; extra == "dev"
+Requires-Dist: pyngrok==7.0.3; extra == "dev"
 Requires-Dist: authlib==1.3.0; extra == "dev"
-Requires-Dist: itsdangerous==2.2.0; extra == "dev"
+Requires-Dist: itsdangerous==2.1.2; extra == "dev"
 Requires-Dist: seqeval==1.2.2; extra == "dev"
-Requires-Dist: httpx==0.27.0; extra == "dev"
-Requires-Dist: pyyaml==6.0.1; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: flake8==3.7.9; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: quality
-Requires-Dist: albumentations==1.4.4; extra == "quality"
-Requires-Dist: codecarbon==2.3.5; extra == "quality"
-Requires-Dist: datasets[vision]~=2.19.0; extra == "quality"
-Requires-Dist: evaluate==0.4.1; extra == "quality"
+Requires-Dist: albumentations==1.3.1; extra == "quality"
+Requires-Dist: codecarbon==2.2.3; extra == "quality"
+Requires-Dist: datasets[vision]~=2.14.0; extra == "quality"
+Requires-Dist: evaluate==0.3.0; extra == "quality"
 Requires-Dist: ipadic==1.0.0; extra == "quality"
-Requires-Dist: jiwer==3.0.3; extra == "quality"
-Requires-Dist: joblib==1.4.0; extra == "quality"
-Requires-Dist: loguru==0.7.2; extra == "quality"
-Requires-Dist: pandas==2.2.2; extra == "quality"
+Requires-Dist: jiwer==3.0.2; extra == "quality"
+Requires-Dist: joblib==1.3.1; extra == "quality"
+Requires-Dist: loguru==0.7.0; extra == "quality"
+Requires-Dist: pandas>=1.4; extra == "quality"
 Requires-Dist: nltk==3.8.1; extra == "quality"
-Requires-Dist: optuna==3.6.1; extra == "quality"
-Requires-Dist: Pillow==10.3.0; extra == "quality"
+Requires-Dist: optuna==3.3.0; extra == "quality"
+Requires-Dist: Pillow==10.0.0; extra == "quality"
 Requires-Dist: protobuf==4.23.4; extra == "quality"
-Requires-Dist: sacremoses==0.1.1; extra == "quality"
-Requires-Dist: scikit-learn==1.4.2; extra == "quality"
-Requires-Dist: sentencepiece==0.2.0; extra == "quality"
-Requires-Dist: tqdm==4.66.2; extra == "quality"
-Requires-Dist: werkzeug==3.0.2; extra == "quality"
-Requires-Dist: xgboost==2.0.3; extra == "quality"
-Requires-Dist: huggingface_hub==0.22.2; extra == "quality"
+Requires-Dist: sacremoses==0.0.53; extra == "quality"
+Requires-Dist: scikit-learn==1.3.0; extra == "quality"
+Requires-Dist: sentencepiece==0.1.99; extra == "quality"
+Requires-Dist: tqdm==4.65.0; extra == "quality"
+Requires-Dist: werkzeug==2.3.6; extra == "quality"
+Requires-Dist: xgboost==1.7.6; extra == "quality"
+Requires-Dist: huggingface_hub>=0.16.4; extra == "quality"
 Requires-Dist: requests==2.31.0; extra == "quality"
-Requires-Dist: einops==0.7.0; extra == "quality"
+Requires-Dist: einops==0.6.1; extra == "quality"
 Requires-Dist: invisible-watermark==0.2.0; extra == "quality"
-Requires-Dist: packaging==24.0; extra == "quality"
-Requires-Dist: cryptography==42.0.5; extra == "quality"
-Requires-Dist: nvitop==1.3.2; extra == "quality"
-Requires-Dist: tensorboard==2.16.2; extra == "quality"
-Requires-Dist: peft==0.10.0; extra == "quality"
-Requires-Dist: trl==0.8.6; extra == "quality"
+Requires-Dist: packaging==23.1; extra == "quality"
+Requires-Dist: tensorboard; extra == "quality"
+Requires-Dist: peft==0.9.0; extra == "quality"
+Requires-Dist: trl==0.7.11; extra == "quality"
 Requires-Dist: tiktoken==0.6.0; extra == "quality"
-Requires-Dist: transformers==4.40.1; extra == "quality"
-Requires-Dist: accelerate==0.29.3; extra == "quality"
-Requires-Dist: diffusers==0.27.2; extra == "quality"
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux" and extra == "quality"
+Requires-Dist: transformers==4.38.2; extra == "quality"
+Requires-Dist: accelerate==0.27.2; extra == "quality"
+Requires-Dist: diffusers==0.26.3; extra == "quality"
+Requires-Dist: bitsandbytes==0.42.0; extra == "quality"
 Requires-Dist: rouge_score==0.1.2; extra == "quality"
-Requires-Dist: py7zr==0.21.0; extra == "quality"
-Requires-Dist: fastapi==0.110.2; extra == "quality"
-Requires-Dist: uvicorn==0.29.0; extra == "quality"
-Requires-Dist: python-multipart==0.0.9; extra == "quality"
-Requires-Dist: pydantic==2.7.1; extra == "quality"
+Requires-Dist: py7zr==0.20.6; extra == "quality"
+Requires-Dist: fastapi==0.104.1; extra == "quality"
+Requires-Dist: uvicorn==0.22.0; extra == "quality"
+Requires-Dist: python-multipart==0.0.6; extra == "quality"
+Requires-Dist: gradio==3.41.0; extra == "quality"
+Requires-Dist: pydantic==2.4.2; extra == "quality"
 Requires-Dist: hf-transfer; extra == "quality"
-Requires-Dist: pyngrok==7.1.6; extra == "quality"
+Requires-Dist: pyngrok==7.0.3; extra == "quality"
 Requires-Dist: authlib==1.3.0; extra == "quality"
-Requires-Dist: itsdangerous==2.2.0; extra == "quality"
+Requires-Dist: itsdangerous==2.1.2; extra == "quality"
 Requires-Dist: seqeval==1.2.2; extra == "quality"
-Requires-Dist: httpx==0.27.0; extra == "quality"
-Requires-Dist: pyyaml==6.0.1; extra == "quality"
 Requires-Dist: black; extra == "quality"
 Requires-Dist: isort; extra == "quality"
 Requires-Dist: flake8==3.7.9; extra == "quality"
 Provides-Extra: docs
-Requires-Dist: albumentations==1.4.4; extra == "docs"
-Requires-Dist: codecarbon==2.3.5; extra == "docs"
-Requires-Dist: datasets[vision]~=2.19.0; extra == "docs"
-Requires-Dist: evaluate==0.4.1; extra == "docs"
+Requires-Dist: albumentations==1.3.1; extra == "docs"
+Requires-Dist: codecarbon==2.2.3; extra == "docs"
+Requires-Dist: datasets[vision]~=2.14.0; extra == "docs"
+Requires-Dist: evaluate==0.3.0; extra == "docs"
 Requires-Dist: ipadic==1.0.0; extra == "docs"
-Requires-Dist: jiwer==3.0.3; extra == "docs"
-Requires-Dist: joblib==1.4.0; extra == "docs"
-Requires-Dist: loguru==0.7.2; extra == "docs"
-Requires-Dist: pandas==2.2.2; extra == "docs"
+Requires-Dist: jiwer==3.0.2; extra == "docs"
+Requires-Dist: joblib==1.3.1; extra == "docs"
+Requires-Dist: loguru==0.7.0; extra == "docs"
+Requires-Dist: pandas>=1.4; extra == "docs"
 Requires-Dist: nltk==3.8.1; extra == "docs"
-Requires-Dist: optuna==3.6.1; extra == "docs"
-Requires-Dist: Pillow==10.3.0; extra == "docs"
+Requires-Dist: optuna==3.3.0; extra == "docs"
+Requires-Dist: Pillow==10.0.0; extra == "docs"
 Requires-Dist: protobuf==4.23.4; extra == "docs"
-Requires-Dist: sacremoses==0.1.1; extra == "docs"
-Requires-Dist: scikit-learn==1.4.2; extra == "docs"
-Requires-Dist: sentencepiece==0.2.0; extra == "docs"
-Requires-Dist: tqdm==4.66.2; extra == "docs"
-Requires-Dist: werkzeug==3.0.2; extra == "docs"
-Requires-Dist: xgboost==2.0.3; extra == "docs"
-Requires-Dist: huggingface_hub==0.22.2; extra == "docs"
+Requires-Dist: sacremoses==0.0.53; extra == "docs"
+Requires-Dist: scikit-learn==1.3.0; extra == "docs"
+Requires-Dist: sentencepiece==0.1.99; extra == "docs"
+Requires-Dist: tqdm==4.65.0; extra == "docs"
+Requires-Dist: werkzeug==2.3.6; extra == "docs"
+Requires-Dist: xgboost==1.7.6; extra == "docs"
+Requires-Dist: huggingface_hub>=0.16.4; extra == "docs"
 Requires-Dist: requests==2.31.0; extra == "docs"
-Requires-Dist: einops==0.7.0; extra == "docs"
+Requires-Dist: einops==0.6.1; extra == "docs"
 Requires-Dist: invisible-watermark==0.2.0; extra == "docs"
-Requires-Dist: packaging==24.0; extra == "docs"
-Requires-Dist: cryptography==42.0.5; extra == "docs"
-Requires-Dist: nvitop==1.3.2; extra == "docs"
-Requires-Dist: tensorboard==2.16.2; extra == "docs"
-Requires-Dist: peft==0.10.0; extra == "docs"
-Requires-Dist: trl==0.8.6; extra == "docs"
+Requires-Dist: packaging==23.1; extra == "docs"
+Requires-Dist: tensorboard; extra == "docs"
+Requires-Dist: peft==0.9.0; extra == "docs"
+Requires-Dist: trl==0.7.11; extra == "docs"
 Requires-Dist: tiktoken==0.6.0; extra == "docs"
-Requires-Dist: transformers==4.40.1; extra == "docs"
-Requires-Dist: accelerate==0.29.3; extra == "docs"
-Requires-Dist: diffusers==0.27.2; extra == "docs"
-Requires-Dist: bitsandbytes==0.43.1; sys_platform == "linux" and extra == "docs"
+Requires-Dist: transformers==4.38.2; extra == "docs"
+Requires-Dist: accelerate==0.27.2; extra == "docs"
+Requires-Dist: diffusers==0.26.3; extra == "docs"
+Requires-Dist: bitsandbytes==0.42.0; extra == "docs"
 Requires-Dist: rouge_score==0.1.2; extra == "docs"
-Requires-Dist: py7zr==0.21.0; extra == "docs"
-Requires-Dist: fastapi==0.110.2; extra == "docs"
-Requires-Dist: uvicorn==0.29.0; extra == "docs"
-Requires-Dist: python-multipart==0.0.9; extra == "docs"
-Requires-Dist: pydantic==2.7.1; extra == "docs"
+Requires-Dist: py7zr==0.20.6; extra == "docs"
+Requires-Dist: fastapi==0.104.1; extra == "docs"
+Requires-Dist: uvicorn==0.22.0; extra == "docs"
+Requires-Dist: python-multipart==0.0.6; extra == "docs"
+Requires-Dist: gradio==3.41.0; extra == "docs"
+Requires-Dist: pydantic==2.4.2; extra == "docs"
 Requires-Dist: hf-transfer; extra == "docs"
-Requires-Dist: pyngrok==7.1.6; extra == "docs"
+Requires-Dist: pyngrok==7.0.3; extra == "docs"
 Requires-Dist: authlib==1.3.0; extra == "docs"
-Requires-Dist: itsdangerous==2.2.0; extra == "docs"
+Requires-Dist: itsdangerous==2.1.2; extra == "docs"
 Requires-Dist: seqeval==1.2.2; extra == "docs"
-Requires-Dist: httpx==0.27.0; extra == "docs"
-Requires-Dist: pyyaml==6.0.1; extra == "docs"
 Requires-Dist: recommonmark; extra == "docs"
 Requires-Dist: sphinx==3.1.2; extra == "docs"
 Requires-Dist: sphinx-markdown-tables; extra == "docs"
 Requires-Dist: sphinx-rtd-theme==0.4.3; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 
 # 🤗 AutoTrain Advanced
@@ -253,23 +241,14 @@
     conda install -c "nvidia/label/cuda-12.1.0" cuda-nvcc
 
 Once done, you can start the application using:
 
     autotrain app --port 8080 --host 127.0.0.1
 
 
-If you are not fond of UI, you can use AutoTrain Configs to train using command line or simply AutoTrain CLI.
-
-To use config file for training, you can use the following command:
-
-    autotrain --config <path_to_config_file>
-
-
-You can find sample config files in the `configs` directory of this repository.
-
 ## Colabs
 
 | Task | Colab Link |
 | --- | --- |
 | LLM Fine Tuning | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_LLM.ipynb) |
 | DreamBooth Training | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_Dreambooth.ipynb) |
```

### Comparing `autotrain-advanced-0.7.86/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.9/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,62 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/autotrain/__init__.py
+src/autotrain/api.py
+src/autotrain/app.py
+src/autotrain/app_params.py
+src/autotrain/app_utils.py
+src/autotrain/backend.py
 src/autotrain/commands.py
 src/autotrain/config.py
 src/autotrain/dataset.py
+src/autotrain/db.py
 src/autotrain/help.py
 src/autotrain/logging.py
-src/autotrain/parser.py
+src/autotrain/oauth.py
 src/autotrain/project.py
 src/autotrain/tasks.py
 src/autotrain/utils.py
-src/autotrain/app/__init__.py
-src/autotrain/app/api_routes.py
-src/autotrain/app/app.py
-src/autotrain/app/db.py
-src/autotrain/app/models.py
-src/autotrain/app/oauth.py
-src/autotrain/app/params.py
-src/autotrain/app/training_api.py
-src/autotrain/app/ui_routes.py
-src/autotrain/app/utils.py
-src/autotrain/app/static/logo.png
-src/autotrain/app/templates/duplicate.html
-src/autotrain/app/templates/error.html
-src/autotrain/app/templates/index.html
-src/autotrain/app/templates/login.html
-src/autotrain/backends/__init__.py
-src/autotrain/backends/base.py
-src/autotrain/backends/endpoints.py
-src/autotrain/backends/local.py
-src/autotrain/backends/ngc.py
-src/autotrain/backends/nvcf.py
-src/autotrain/backends/spaces.py
 src/autotrain/cli/__init__.py
 src/autotrain/cli/autotrain.py
 src/autotrain/cli/run_api.py
 src/autotrain/cli/run_app.py
 src/autotrain/cli/run_dreambooth.py
 src/autotrain/cli/run_image_classification.py
 src/autotrain/cli/run_llm.py
 src/autotrain/cli/run_seq2seq.py
 src/autotrain/cli/run_setup.py
 src/autotrain/cli/run_spacerunner.py
 src/autotrain/cli/run_tabular.py
 src/autotrain/cli/run_text_classification.py
-src/autotrain/cli/run_text_regression.py
 src/autotrain/cli/run_token_classification.py
-src/autotrain/cli/run_tools.py
 src/autotrain/cli/utils.py
 src/autotrain/preprocessor/__init__.py
 src/autotrain/preprocessor/dreambooth.py
 src/autotrain/preprocessor/tabular.py
 src/autotrain/preprocessor/text.py
 src/autotrain/preprocessor/vision.py
-src/autotrain/tools/__init__.py
-src/autotrain/tools/convert_to_kohya.py
-src/autotrain/tools/merge_adapter.py
+src/autotrain/static/logo.png
+src/autotrain/templates/duplicate.html
+src/autotrain/templates/error.html
+src/autotrain/templates/index.html
+src/autotrain/templates/login.html
 src/autotrain/trainers/__init__.py
 src/autotrain/trainers/common.py
 src/autotrain/trainers/clm/__init__.py
 src/autotrain/trainers/clm/__main__.py
 src/autotrain/trainers/clm/callbacks.py
 src/autotrain/trainers/clm/params.py
-src/autotrain/trainers/clm/train_clm_default.py
-src/autotrain/trainers/clm/train_clm_dpo.py
-src/autotrain/trainers/clm/train_clm_orpo.py
-src/autotrain/trainers/clm/train_clm_reward.py
-src/autotrain/trainers/clm/train_clm_sft.py
 src/autotrain/trainers/clm/utils.py
 src/autotrain/trainers/dreambooth/__init__.py
 src/autotrain/trainers/dreambooth/__main__.py
 src/autotrain/trainers/dreambooth/datasets.py
 src/autotrain/trainers/dreambooth/params.py
-src/autotrain/trainers/dreambooth/train.py
-src/autotrain/trainers/dreambooth/train_xl.py
 src/autotrain/trainers/dreambooth/trainer.py
 src/autotrain/trainers/dreambooth/utils.py
 src/autotrain/trainers/generic/__init__.py
 src/autotrain/trainers/generic/__main__.py
 src/autotrain/trainers/generic/params.py
 src/autotrain/trainers/generic/utils.py
 src/autotrain/trainers/image_classification/__init__.py
@@ -97,19 +74,14 @@
 src/autotrain/trainers/tabular/params.py
 src/autotrain/trainers/tabular/utils.py
 src/autotrain/trainers/text_classification/__init__.py
 src/autotrain/trainers/text_classification/__main__.py
 src/autotrain/trainers/text_classification/dataset.py
 src/autotrain/trainers/text_classification/params.py
 src/autotrain/trainers/text_classification/utils.py
-src/autotrain/trainers/text_regression/__init__.py
-src/autotrain/trainers/text_regression/__main__.py
-src/autotrain/trainers/text_regression/dataset.py
-src/autotrain/trainers/text_regression/params.py
-src/autotrain/trainers/text_regression/utils.py
 src/autotrain/trainers/token_classification/__init__.py
 src/autotrain/trainers/token_classification/__main__.py
 src/autotrain/trainers/token_classification/dataset.py
 src/autotrain/trainers/token_classification/params.py
 src/autotrain/trainers/token_classification/utils.py
 src/autotrain_advanced.egg-info/PKG-INFO
 src/autotrain_advanced.egg-info/SOURCES.txt
```

### Comparing `autotrain-advanced-0.7.86/static/logo.png` & `autotrain-advanced-0.7.9/static/logo.png`

 * *Files identical despite different names*

