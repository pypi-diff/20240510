# Comparing `tmp/datum-1.8.0.tar.gz` & `tmp/datum-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datum-1.8.0.tar", last modified: Tue Aug 16 15:48:32 2022, max compression
+gzip compressed data, was "datum-1.9.0.tar", last modified: Sun Jan  8 13:40:33 2023, max compression
```

## Comparing `datum-1.8.0.tar` & `datum-1.9.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.580715 datum-1.8.0/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      316 2022-06-02 16:28:04.000000 datum-1.8.0/AUTHORS
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)    11415 2022-06-02 16:28:04.000000 datum-1.8.0/LICENSE
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)       30 2022-06-02 16:28:04.000000 datum-1.8.0/MANIFEST.in
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      676 2022-08-16 15:48:32.580411 datum-1.8.0/PKG-INFO
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     4438 2022-08-03 15:40:36.000000 datum-1.8.0/README.md
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.568679 datum-1.8.0/configs/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2246 2022-06-02 16:28:04.000000 datum-1.8.0/configs/image_clf_configs.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1418 2022-06-02 16:28:04.000000 datum-1.8.0/configs/image_det_configs.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1164 2022-06-02 16:28:04.000000 datum-1.8.0/configs/image_seg_configs.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1182 2022-06-02 16:28:04.000000 datum-1.8.0/configs/text_json_configs.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.569261 datum-1.8.0/datum/
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.571086 datum-1.8.0/datum/cache/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      631 2022-06-02 16:28:04.000000 datum-1.8.0/datum/cache/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     8714 2022-06-02 16:28:04.000000 datum-1.8.0/datum/cache/bucket.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.572196 datum-1.8.0/datum/configs/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      782 2022-08-14 08:43:07.000000 datum-1.8.0/datum/configs/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     5112 2022-08-14 08:43:07.000000 datum-1.8.0/datum/configs/config_base.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2407 2022-06-02 16:28:04.000000 datum-1.8.0/datum/configs/default_configs.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)    11943 2022-08-09 16:44:05.000000 datum-1.8.0/datum/configs/tfr_configs.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2223 2022-06-02 16:28:04.000000 datum-1.8.0/datum/create_tfrecord.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.573012 datum-1.8.0/datum/encoder/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      742 2022-08-14 08:43:06.000000 datum-1.8.0/datum/encoder/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     4509 2022-06-02 16:28:04.000000 datum-1.8.0/datum/encoder/encoder.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2306 2022-06-02 16:28:04.000000 datum-1.8.0/datum/encoder/tokenizer.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.573540 datum-1.8.0/datum/export/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      642 2022-06-02 16:28:04.000000 datum-1.8.0/datum/export/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3956 2022-06-02 16:28:04.000000 datum-1.8.0/datum/export/export.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.574657 datum-1.8.0/datum/generator/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1304 2022-08-14 08:43:06.000000 datum-1.8.0/datum/generator/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1845 2022-08-16 15:47:28.000000 datum-1.8.0/datum/generator/generator.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)    12200 2022-08-09 16:36:01.000000 datum-1.8.0/datum/generator/image.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3366 2022-08-16 15:47:28.000000 datum-1.8.0/datum/generator/text.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.575208 datum-1.8.0/datum/problem/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1253 2022-08-14 08:43:06.000000 datum-1.8.0/datum/problem/problem.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      720 2022-06-02 16:28:04.000000 datum-1.8.0/datum/problem/types.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.576591 datum-1.8.0/datum/reader/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      761 2022-06-02 16:28:04.000000 datum-1.8.0/datum/reader/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)    10875 2022-08-09 16:44:05.000000 datum-1.8.0/datum/reader/dataset.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     5055 2022-06-02 16:28:04.000000 datum-1.8.0/datum/reader/loader.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     4997 2022-06-02 16:28:04.000000 datum-1.8.0/datum/reader/parser.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     8243 2022-06-02 16:28:04.000000 datum-1.8.0/datum/reader/tfrecord_reader.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.577161 datum-1.8.0/datum/serializer/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      647 2022-06-02 16:28:04.000000 datum-1.8.0/datum/serializer/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3891 2022-06-02 16:28:04.000000 datum-1.8.0/datum/serializer/serializer.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.579473 datum-1.8.0/datum/utils/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      590 2022-06-02 16:28:04.000000 datum-1.8.0/datum/utils/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1437 2022-06-02 16:28:04.000000 datum-1.8.0/datum/utils/binary_utils.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)    10309 2022-08-03 15:39:48.000000 datum-1.8.0/datum/utils/common_utils.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3163 2022-06-02 16:28:04.000000 datum-1.8.0/datum/utils/hashing.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     8147 2022-06-02 16:28:04.000000 datum-1.8.0/datum/utils/reader_utils.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     6003 2022-06-02 16:28:04.000000 datum-1.8.0/datum/utils/shard_utils.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3331 2022-06-02 16:28:04.000000 datum-1.8.0/datum/utils/tqdm_utils.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1080 2022-06-02 16:28:04.000000 datum-1.8.0/datum/utils/types_utils.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      613 2022-08-16 15:47:48.000000 datum-1.8.0/datum/version.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.579996 datum-1.8.0/datum/writer/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      647 2022-06-02 16:28:04.000000 datum-1.8.0/datum/writer/__init__.py
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     6052 2022-08-16 15:47:28.000000 datum-1.8.0/datum/writer/tfrecord_writer.py
-drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2022-08-16 15:48:32.570600 datum-1.8.0/datum.egg-info/
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      676 2022-08-16 15:48:32.000000 datum-1.8.0/datum.egg-info/PKG-INFO
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1263 2022-08-16 15:48:32.000000 datum-1.8.0/datum.egg-info/SOURCES.txt
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)        1 2022-08-16 15:48:32.000000 datum-1.8.0/datum.egg-info/dependency_links.txt
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)       66 2022-08-16 15:48:32.000000 datum-1.8.0/datum.egg-info/requires.txt
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)       24 2022-08-16 15:48:32.000000 datum-1.8.0/datum.egg-info/top_level.txt
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)      284 2022-08-03 15:39:48.000000 datum-1.8.0/requirements.txt
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)       38 2022-08-16 15:48:32.580824 datum-1.8.0/setup.cfg
--rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1789 2022-06-02 16:28:04.000000 datum-1.8.0/setup.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.578494 datum-1.9.0/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      316 2022-06-02 16:28:04.000000 datum-1.9.0/AUTHORS
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)    11415 2022-06-02 16:28:04.000000 datum-1.9.0/LICENSE
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)       30 2022-06-02 16:28:04.000000 datum-1.9.0/MANIFEST.in
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      695 2023-01-08 13:40:33.578213 datum-1.9.0/PKG-INFO
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     4438 2022-08-03 15:40:36.000000 datum-1.9.0/README.md
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.565869 datum-1.9.0/configs/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2246 2022-06-02 16:28:04.000000 datum-1.9.0/configs/image_clf_configs.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1418 2022-06-02 16:28:04.000000 datum-1.9.0/configs/image_det_configs.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1164 2022-06-02 16:28:04.000000 datum-1.9.0/configs/image_seg_configs.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1182 2022-06-02 16:28:04.000000 datum-1.9.0/configs/text_json_configs.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.566492 datum-1.9.0/datum/
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.568488 datum-1.9.0/datum/cache/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      631 2022-06-02 16:28:04.000000 datum-1.9.0/datum/cache/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     8714 2022-06-02 16:28:04.000000 datum-1.9.0/datum/cache/bucket.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.569701 datum-1.9.0/datum/configs/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      782 2022-08-14 08:43:07.000000 datum-1.9.0/datum/configs/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     5112 2022-08-14 08:43:07.000000 datum-1.9.0/datum/configs/config_base.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2407 2022-06-02 16:28:04.000000 datum-1.9.0/datum/configs/default_configs.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)    11943 2022-08-09 16:44:05.000000 datum-1.9.0/datum/configs/tfr_configs.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2223 2022-06-02 16:28:04.000000 datum-1.9.0/datum/create_tfrecord.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.570666 datum-1.9.0/datum/encoder/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      742 2022-08-14 08:43:06.000000 datum-1.9.0/datum/encoder/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     4509 2022-06-02 16:28:04.000000 datum-1.9.0/datum/encoder/encoder.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     2306 2022-06-02 16:28:04.000000 datum-1.9.0/datum/encoder/tokenizer.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.571235 datum-1.9.0/datum/export/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      642 2022-06-02 16:28:04.000000 datum-1.9.0/datum/export/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3956 2022-06-02 16:28:04.000000 datum-1.9.0/datum/export/export.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.572293 datum-1.9.0/datum/generator/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1304 2022-08-14 08:43:06.000000 datum-1.9.0/datum/generator/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1845 2022-08-16 15:47:28.000000 datum-1.9.0/datum/generator/generator.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)    12200 2022-08-09 16:36:01.000000 datum-1.9.0/datum/generator/image.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3366 2022-08-16 15:47:28.000000 datum-1.9.0/datum/generator/text.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.572898 datum-1.9.0/datum/problem/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1253 2022-08-14 08:43:06.000000 datum-1.9.0/datum/problem/problem.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      720 2022-06-02 16:28:04.000000 datum-1.9.0/datum/problem/types.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.574454 datum-1.9.0/datum/reader/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      761 2022-06-02 16:28:04.000000 datum-1.9.0/datum/reader/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)    10875 2022-08-09 16:44:05.000000 datum-1.9.0/datum/reader/dataset.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     5055 2022-06-02 16:28:04.000000 datum-1.9.0/datum/reader/loader.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     4997 2022-06-02 16:28:04.000000 datum-1.9.0/datum/reader/parser.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     8243 2022-06-02 16:28:04.000000 datum-1.9.0/datum/reader/tfrecord_reader.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.575054 datum-1.9.0/datum/serializer/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      647 2022-06-02 16:28:04.000000 datum-1.9.0/datum/serializer/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3891 2022-06-02 16:28:04.000000 datum-1.9.0/datum/serializer/serializer.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.577305 datum-1.9.0/datum/utils/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      590 2022-06-02 16:28:04.000000 datum-1.9.0/datum/utils/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1437 2022-06-02 16:28:04.000000 datum-1.9.0/datum/utils/binary_utils.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)    10309 2022-08-03 15:39:48.000000 datum-1.9.0/datum/utils/common_utils.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3163 2022-06-02 16:28:04.000000 datum-1.9.0/datum/utils/hashing.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     8147 2022-06-02 16:28:04.000000 datum-1.9.0/datum/utils/reader_utils.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     6003 2022-06-02 16:28:04.000000 datum-1.9.0/datum/utils/shard_utils.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     3331 2022-06-02 16:28:04.000000 datum-1.9.0/datum/utils/tqdm_utils.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1080 2022-06-02 16:28:04.000000 datum-1.9.0/datum/utils/types_utils.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      613 2023-01-08 13:39:56.000000 datum-1.9.0/datum/version.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.577840 datum-1.9.0/datum/writer/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      647 2022-06-02 16:28:04.000000 datum-1.9.0/datum/writer/__init__.py
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     6052 2022-08-16 15:47:28.000000 datum-1.9.0/datum/writer/tfrecord_writer.py
+drwxr-xr-x   0 mrinalhaloi   (501) staff       (20)        0 2023-01-08 13:40:33.567930 datum-1.9.0/datum.egg-info/
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      695 2023-01-08 13:40:33.000000 datum-1.9.0/datum.egg-info/PKG-INFO
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1263 2023-01-08 13:40:33.000000 datum-1.9.0/datum.egg-info/SOURCES.txt
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)        1 2023-01-08 13:40:33.000000 datum-1.9.0/datum.egg-info/dependency_links.txt
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)       67 2023-01-08 13:40:33.000000 datum-1.9.0/datum.egg-info/requires.txt
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)       24 2023-01-08 13:40:33.000000 datum-1.9.0/datum.egg-info/top_level.txt
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)      285 2023-01-08 13:39:56.000000 datum-1.9.0/requirements.txt
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)       38 2023-01-08 13:40:33.578583 datum-1.9.0/setup.cfg
+-rw-r--r--   0 mrinalhaloi   (501) staff       (20)     1789 2022-06-02 16:28:04.000000 datum-1.9.0/setup.py
```

### Comparing `datum-1.8.0/LICENSE` & `datum-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/PKG-INFO` & `datum-1.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: datum
-Version: 1.8.0
+Version: 1.9.0
 Summary: Datum provides APIs to create tfrecord daatsets and read tfrecord as tf.data.Datasets
 Home-page: https://github.com/openagi/datum
 Download-URL: https://github.com/openagi/datum/tags
 Author: OpenAGI
 Author-email: maintainer@openagi.io
 License: Apache 2.0
 Keywords: datum tensorflow tf.data datasets tfrecord
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS
 
 Datum provides APIs to create tfrecord daatsets and read tfrecord as tf.data.Datasets
+
```

### Comparing `datum-1.8.0/README.md` & `datum-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/configs/image_clf_configs.py` & `datum-1.9.0/configs/image_clf_configs.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/configs/image_det_configs.py` & `datum-1.9.0/configs/image_det_configs.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/configs/image_seg_configs.py` & `datum-1.9.0/configs/image_seg_configs.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/configs/text_json_configs.py` & `datum-1.9.0/configs/text_json_configs.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/cache/__init__.py` & `datum-1.9.0/datum/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/cache/bucket.py` & `datum-1.9.0/datum/cache/bucket.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/configs/__init__.py` & `datum-1.9.0/datum/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/configs/config_base.py` & `datum-1.9.0/datum/configs/config_base.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/configs/default_configs.py` & `datum-1.9.0/datum/configs/default_configs.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/configs/tfr_configs.py` & `datum-1.9.0/datum/configs/tfr_configs.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/create_tfrecord.py` & `datum-1.9.0/datum/create_tfrecord.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/encoder/__init__.py` & `datum-1.9.0/datum/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/encoder/encoder.py` & `datum-1.9.0/datum/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/encoder/tokenizer.py` & `datum-1.9.0/datum/encoder/tokenizer.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/export/__init__.py` & `datum-1.9.0/datum/export/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/export/export.py` & `datum-1.9.0/datum/export/export.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/generator/__init__.py` & `datum-1.9.0/datum/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/generator/generator.py` & `datum-1.9.0/datum/generator/generator.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/generator/image.py` & `datum-1.9.0/datum/generator/image.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/generator/text.py` & `datum-1.9.0/datum/generator/text.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/problem/problem.py` & `datum-1.9.0/datum/problem/problem.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/problem/types.py` & `datum-1.9.0/datum/problem/types.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/reader/__init__.py` & `datum-1.9.0/datum/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/reader/dataset.py` & `datum-1.9.0/datum/reader/dataset.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/reader/loader.py` & `datum-1.9.0/datum/reader/loader.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/reader/parser.py` & `datum-1.9.0/datum/reader/parser.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/reader/tfrecord_reader.py` & `datum-1.9.0/datum/reader/tfrecord_reader.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/serializer/__init__.py` & `datum-1.9.0/datum/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/serializer/serializer.py` & `datum-1.9.0/datum/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/__init__.py` & `datum-1.9.0/datum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/binary_utils.py` & `datum-1.9.0/datum/utils/binary_utils.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/common_utils.py` & `datum-1.9.0/datum/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/hashing.py` & `datum-1.9.0/datum/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/reader_utils.py` & `datum-1.9.0/datum/utils/reader_utils.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/shard_utils.py` & `datum-1.9.0/datum/utils/shard_utils.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/tqdm_utils.py` & `datum-1.9.0/datum/utils/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/utils/types_utils.py` & `datum-1.9.0/datum/utils/types_utils.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/version.py` & `datum-1.9.0/datum/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.8.0'
+__version__ = '1.9.0'
```

### Comparing `datum-1.8.0/datum/writer/__init__.py` & `datum-1.9.0/datum/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum/writer/tfrecord_writer.py` & `datum-1.9.0/datum/writer/tfrecord_writer.py`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/datum.egg-info/PKG-INFO` & `datum-1.9.0/datum.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: datum
-Version: 1.8.0
+Version: 1.9.0
 Summary: Datum provides APIs to create tfrecord daatsets and read tfrecord as tf.data.Datasets
 Home-page: https://github.com/openagi/datum
 Download-URL: https://github.com/openagi/datum/tags
 Author: OpenAGI
 Author-email: maintainer@openagi.io
 License: Apache 2.0
 Keywords: datum tensorflow tf.data datasets tfrecord
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS
 
 Datum provides APIs to create tfrecord daatsets and read tfrecord as tf.data.Datasets
+
```

### Comparing `datum-1.8.0/datum.egg-info/SOURCES.txt` & `datum-1.9.0/datum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datum-1.8.0/setup.py` & `datum-1.9.0/setup.py`

 * *Files identical despite different names*

