# Comparing `tmp/libem-0.0.4.tar.gz` & `tmp/libem-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libem-0.0.4.tar", last modified: Tue May  7 17:34:10 2024, max compression
+gzip compressed data, was "libem-0.0.5.tar", last modified: Thu May  9 21:12:49 2024, max compression
```

## Comparing `libem-0.0.4.tar` & `libem-0.0.5.tar`

### file list

```diff
@@ -1,83 +1,80 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.918170 libem-0.0.4/
--rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.4/LICENSE
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-07 17:34:10.918032 libem-0.0.4/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      550 2024-05-07 02:02:55.000000 libem-0.0.4/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.906209 libem-0.0.4/cli/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.4/cli/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      509 2024-05-06 01:35:06.000000 libem-0.0.4/cli/libem
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.908133 libem-0.0.4/libem/
--rw-r--r--   0 silv       (501) staff       (20)      144 2024-05-07 06:32:51.000000 libem-0.0.4/libem/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.909707 libem-0.0.4/libem/browse/
--rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.4/libem/browse/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1542 2024-05-03 17:04:24.000000 libem-0.0.4/libem/browse/function.py
--rw-r--r--   0 silv       (501) staff       (20)       85 2024-05-05 01:29:22.000000 libem-0.0.4/libem/browse/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.4/libem/browse/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.910261 libem-0.0.4/libem/calibrate/
--rw-r--r--   0 silv       (501) staff       (20)       98 2024-05-07 16:02:23.000000 libem-0.0.4/libem/calibrate/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      711 2024-05-07 17:18:26.000000 libem-0.0.4/libem/calibrate/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/calibrate/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/calibrate/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      422 2024-05-05 16:22:40.000000 libem-0.0.4/libem/constant.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.910958 libem-0.0.4/libem/core/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.4/libem/core/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      651 2024-05-06 01:38:58.000000 libem-0.0.4/libem/core/eval.py
--rw-r--r--   0 silv       (501) staff       (20)     2991 2024-05-07 17:07:28.000000 libem-0.0.4/libem/core/model.py
--rw-r--r--   0 silv       (501) staff       (20)     1097 2024-05-06 01:44:20.000000 libem-0.0.4/libem/core/struct.py
--rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.4/libem/function.py
--rw-r--r--   0 silv       (501) staff       (20)      836 2024-05-07 17:32:21.000000 libem-0.0.4/libem/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.911889 libem-0.0.4/libem/match/
--rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.4/libem/match/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1126 2024-05-07 16:02:52.000000 libem-0.0.4/libem/match/function.py
--rw-r--r--   0 silv       (501) staff       (20)      197 2024-05-07 17:01:12.000000 libem-0.0.4/libem/match/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      429 2024-05-07 16:31:34.000000 libem-0.0.4/libem/match/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      216 2024-05-07 06:42:34.000000 libem-0.0.4/libem/parameter.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.912794 libem-0.0.4/libem/prepare/
--rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.4/libem/prepare/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.914408 libem-0.0.4/libem/prepare/datasets/
--rw-r--r--   0 silv       (501) staff       (20)      197 2024-05-05 06:12:44.000000 libem-0.0.4/libem/prepare/datasets/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2842 2024-05-07 02:22:18.000000 libem-0.0.4/libem/prepare/datasets/abt_buy.py
--rw-r--r--   0 silv       (501) staff       (20)     2465 2024-05-07 02:18:30.000000 libem-0.0.4/libem/prepare/datasets/amazon_google.py
--rw-r--r--   0 silv       (501) staff       (20)     2637 2024-05-07 02:20:12.000000 libem-0.0.4/libem/prepare/datasets/dblp_acm.py
--rw-r--r--   0 silv       (501) staff       (20)     2618 2024-05-07 02:20:21.000000 libem-0.0.4/libem/prepare/datasets/dblp_scholar.py
--rw-r--r--   0 silv       (501) staff       (20)     2646 2024-05-07 02:20:28.000000 libem-0.0.4/libem/prepare/datasets/walmart_amazon.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-06 01:50:49.000000 libem-0.0.4/libem/prepare/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.4/libem/prepare/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.4/libem/prepare/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.4/libem/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.915185 libem-0.0.4/libem/tune/
--rw-r--r--   0 silv       (501) staff       (20)       88 2024-05-07 06:19:35.000000 libem-0.0.4/libem/tune/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.4/libem/tune/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.915793 libem-0.0.4/libem/tune/learn/
--rw-r--r--   0 silv       (501) staff       (20)       95 2024-05-07 06:21:06.000000 libem-0.0.4/libem/tune/learn/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.4/libem/tune/learn/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/learn/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/learn/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.916402 libem-0.0.4/libem/tune/load/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.4/libem/tune/load/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.4/libem/tune/load/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/load/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/load/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.916946 libem-0.0.4/libem/tune/save/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.4/libem/tune/save/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.4/libem/tune/save/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/save/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/save/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.917523 libem-0.0.4/libem/tune/search/
--rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.4/libem/tune/search/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.4/libem/tune/search/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/search/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/search/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:26:56.000000 libem-0.0.4/libem/tune/storage.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.908861 libem-0.0.4/libem.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     1619 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)      133 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/top_level.txt
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.917727 libem-0.0.4/serve/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.4/serve/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.4/serve/run.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-07 17:34:10.918205 libem-0.0.4/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-07 17:34:06.000000 libem-0.0.4/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.796092 libem-0.0.5/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.5/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-09 21:12:49.795978 libem-0.0.5/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1343 2024-05-09 21:01:57.000000 libem-0.0.5/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.784318 libem-0.0.5/cli/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.5/cli/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1367 2024-05-09 01:15:34.000000 libem-0.0.5/cli/libem
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.785729 libem-0.0.5/libem/
+-rw-r--r--   0 silv       (501) staff       (20)      347 2024-05-09 16:04:48.000000 libem-0.0.5/libem/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.787053 libem-0.0.5/libem/browse/
+-rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.5/libem/browse/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1623 2024-05-09 00:19:21.000000 libem-0.0.5/libem/browse/function.py
+-rw-r--r--   0 silv       (501) staff       (20)       85 2024-05-05 01:29:22.000000 libem-0.0.5/libem/browse/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      292 2024-05-09 03:38:00.000000 libem-0.0.5/libem/browse/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.787675 libem-0.0.5/libem/calibrate/
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-09 20:29:02.000000 libem-0.0.5/libem/calibrate/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      729 2024-05-08 19:28:44.000000 libem-0.0.5/libem/calibrate/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      365 2024-05-09 21:07:53.000000 libem-0.0.5/libem/calibrate/interface.py
+-rw-r--r--   0 silv       (501) staff       (20)      751 2024-05-09 16:23:53.000000 libem-0.0.5/libem/constant.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.789359 libem-0.0.5/libem/core/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.5/libem/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3823 2024-05-08 06:37:24.000000 libem-0.0.5/libem/core/eval.py
+-rw-r--r--   0 silv       (501) staff       (20)     3784 2024-05-09 16:55:50.000000 libem-0.0.5/libem/core/log.py
+-rw-r--r--   0 silv       (501) staff       (20)     3216 2024-05-09 03:20:14.000000 libem-0.0.5/libem/core/model.py
+-rw-r--r--   0 silv       (501) staff       (20)     4145 2024-05-09 19:57:45.000000 libem-0.0.5/libem/core/struct.py
+-rw-r--r--   0 silv       (501) staff       (20)      907 2024-05-09 16:10:45.000000 libem-0.0.5/libem/core/telemetry.py
+-rw-r--r--   0 silv       (501) staff       (20)     1098 2024-05-08 21:50:28.000000 libem-0.0.5/libem/core/trace.py
+-rw-r--r--   0 silv       (501) staff       (20)     1020 2024-05-09 21:08:05.000000 libem-0.0.5/libem/core/util.py
+-rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.5/libem/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      936 2024-05-08 00:39:19.000000 libem-0.0.5/libem/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.790208 libem-0.0.5/libem/match/
+-rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.5/libem/match/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1473 2024-05-09 18:24:22.000000 libem-0.0.5/libem/match/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      197 2024-05-07 17:01:12.000000 libem-0.0.5/libem/match/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      597 2024-05-09 19:46:03.000000 libem-0.0.5/libem/match/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      216 2024-05-07 06:42:34.000000 libem-0.0.5/libem/parameter.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.791044 libem-0.0.5/libem/prepare/
+-rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.5/libem/prepare/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.792312 libem-0.0.5/libem/prepare/datasets/
+-rw-r--r--   0 silv       (501) staff       (20)      134 2024-05-09 00:08:47.000000 libem-0.0.5/libem/prepare/datasets/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2954 2024-05-09 00:05:08.000000 libem-0.0.5/libem/prepare/datasets/abt_buy.py
+-rw-r--r--   0 silv       (501) staff       (20)     2698 2024-05-09 00:06:05.000000 libem-0.0.5/libem/prepare/datasets/amazon_google.py
+-rw-r--r--   0 silv       (501) staff       (20)     2763 2024-05-09 00:08:08.000000 libem-0.0.5/libem/prepare/datasets/dblp_acm.py
+-rw-r--r--   0 silv       (501) staff       (20)     2760 2024-05-09 00:08:21.000000 libem-0.0.5/libem/prepare/datasets/dblp_scholar.py
+-rw-r--r--   0 silv       (501) staff       (20)     2792 2024-05-09 00:08:37.000000 libem-0.0.5/libem/prepare/datasets/walmart_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)       72 2024-05-08 23:56:27.000000 libem-0.0.5/libem/prepare/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.5/libem/prepare/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.5/libem/prepare/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.5/libem/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.793273 libem-0.0.5/libem/tune/
+-rw-r--r--   0 silv       (501) staff       (20)      129 2024-05-08 00:48:47.000000 libem-0.0.5/libem/tune/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.5/libem/tune/function.py
+-rw-r--r--   0 silv       (501) staff       (20)     3251 2024-05-09 19:15:32.000000 libem-0.0.5/libem/tune/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.794020 libem-0.0.5/libem/tune/learn/
+-rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-07 23:38:41.000000 libem-0.0.5/libem/tune/learn/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2932 2024-05-09 19:54:37.000000 libem-0.0.5/libem/tune/learn/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-08 23:52:04.000000 libem-0.0.5/libem/tune/learn/interface.py
+-rw-r--r--   0 silv       (501) staff       (20)      131 2024-05-09 06:30:44.000000 libem-0.0.5/libem/tune/learn/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      688 2024-05-09 19:07:02.000000 libem-0.0.5/libem/tune/learn/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.794454 libem-0.0.5/libem/tune/load/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.5/libem/tune/load/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.5/libem/tune/load/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.794918 libem-0.0.5/libem/tune/save/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.5/libem/tune/save/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.5/libem/tune/save/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.795381 libem-0.0.5/libem/tune/search/
+-rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.5/libem/tune/search/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.5/libem/tune/search/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:26:56.000000 libem-0.0.5/libem/tune/storage.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.786296 libem-0.0.5/libem.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-09 21:12:49.000000 libem-0.0.5/libem.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1514 2024-05-09 21:12:49.000000 libem-0.0.5/libem.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-09 21:12:49.000000 libem-0.0.5/libem.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)      133 2024-05-09 21:12:49.000000 libem-0.0.5/libem.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-09 21:12:49.000000 libem-0.0.5/libem.egg-info/top_level.txt
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-09 21:12:49.795661 libem-0.0.5/serve/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.5/serve/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.5/serve/run.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-09 21:12:49.796125 libem-0.0.5/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-09 21:12:48.000000 libem-0.0.5/setup.py
```

### Comparing `libem-0.0.4/LICENSE` & `libem-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libem-0.0.4/libem/browse/function.py` & `libem-0.0.5/libem/browse/function.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import os
 import json
 
 from langchain_google_community import GoogleSearchAPIWrapper
 from langchain_core.tools import Tool
 
 import libem
+from libem.browse import prompt
+from libem.core.struct import Prompt
 
 schema = {
     "type": "function",
     "function": {
         "name": "browse",
-        "description": "Browse the web to find descriptions for the given entity",
+        "description": Prompt.join(
+            prompt.description(), prompt.rule()
+        ),
         "parameters": {
             "type": "object",
             "properties": {
                 "entity": {
                     "type": "string",
                     "description": "Entity description",
                 },
```

### Comparing `libem-0.0.4/libem/core/model.py` & `libem-0.0.5/libem/core/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,34 +64,41 @@
     num_model_call = 1
     while tool_calls and num_model_call < max_model_call:
         messages.append(response_message)
         for tool_call in tool_calls:
             function_name = tool_call.function.name
             function_to_call = available_functions[function_name]
             function_args = json.loads(tool_call.function.arguments)
-            print(f"Tool: {function_name} - running ..")
+
+            libem.info(f"Tool: {function_name} - running ..")
             function_response = function_to_call(**function_args)
             messages.append(
                 {
                     "tool_call_id": tool_call.id,
                     "role": "tool",
                     "name": function_name,
                     "content": function_response,
                 }
             )
-            print(f"Tool: {function_name} - {function_response}")
+            libem.trace.add({
+                function_name: {
+                    "id": tool_call.id,
+                    "arguments": function_args,
+                    "response": function_response}
+            })
+            libem.info(f"Tool: {function_name} - {function_response}")
 
         # Call the model again with the tool outcomes
         response = client.chat.completions.create(
             model=model,
             messages=messages,
             tools=tools,
             tool_choice="auto",
             temperature=temperature,
         )
         response_message = response.choices[0].message
         tool_calls = response_message.tool_calls
         num_model_call += 1
 
     if num_model_call == max_model_call:
-        raise Warning(f"Max call reached: {messages}\n{response_message}")
+        libem.warn(f"Max call reached: {messages}\n{response_message}")
     return response_message.content
```

### Comparing `libem-0.0.4/libem/interface.py` & `libem-0.0.5/libem/interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import random
 
 import libem.core.model as model
 from libem.core.struct import Prompt
-
 from libem import prompt, parameter
 
-"""Chat interface"""
+"""Chat access"""
 
 
 def chat(message):
     return model.call(
         prompt=Prompt.join(prompt.role(), message, sep="\n"),
         tools=["libem.match"],
         model=parameter.model(),
         temperature=parameter.temperature(),
     )
 
 
-"""Programming interface"""
+"""Programmatic access"""
 from libem.match import func as match_func
+from libem.calibrate import func as calibrate_func
+from libem.tune import func as tune_func
 
 
 def match(left, right,
           always=None,
           guess=False,
           seed=42) -> str:
     if always is not None:
@@ -31,12 +32,13 @@
     if guess:
         random.seed(seed)
         return random.choice(["yes", "no"])
 
     return match_func(left, right)
 
 
-from libem.calibrate import func as calibrate_func
-
-
 def calibrate(*args, **kwargs):
     return calibrate_func(*args, **kwargs)
+
+
+def tune(*args, **kwargs):
+    return tune_func(*args, **kwargs)
```

### Comparing `libem-0.0.4/libem/match/function.py` & `libem-0.0.5/libem/match/function.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import libem
 from libem.match import prompt, parameter
 from libem.core.struct import Prompt
-import libem.core.model as model
+from libem.core import model
 
 schema = {
     "type": "function",
     "function": {
         "name": "match",
         "description": "Perform entity matching given two entity description.",
         "parameters": {
@@ -22,21 +23,31 @@
             "required": ["left", "right"],
         },
     }
 }
 
 
 def func(left, right):
-    return model.call(
-        prompt=Prompt.join(
-            prompt.query(
-                left=left,
-                right=right
-            ),
-            prompt.output(),
-            prompt.rule(),
-            prompt.experience()
+    match_prompt = Prompt.join(
+        prompt.query(
+            left=left,
+            right=right
         ),
+        prompt.rule(),
+        prompt.experience(),
+        prompt.output(),
+    )
+    pred = parse_output(model.call(
+        prompt=match_prompt,
         tools=parameter.tools(),
         model=parameter.model(),
         temperature=parameter.temperature(),
-    )
+    ))
+    libem.trace.add({"match": {"left": left, "right": right, "pred": pred,
+                               "prompt": match_prompt}})
+    return pred
+
+
+def parse_output(output: str) -> str:
+    libem.debug("Match raw output:", output)
+    output = output.split("\n")[-1].lower()
+    return "yes" if "yes" in output else "no"
```

### Comparing `libem-0.0.4/libem/prepare/datasets/abt_buy.py` & `libem-0.0.5/libem/prepare/datasets/abt_buy.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import libem.prepare.datasets as datasets
 
 path = os.path.join(datasets.LIBEM_SAMPLE_DATA_PATH, "abt-buy")
 test_file = os.path.join(path, "test.ndjson")
 train_file = os.path.join(path, "train.ndjson")
 valid_file = os.path.join(path, "valid.ndjson")
-
+description = "The Abt-Buy dataset for entity resolution derives from the online retailers Abt.com and Buy.com."
 
 # sample data:
 # {"id_left":"abt_942","name_left":"sony bravia theater black micro system davis50b","description_left":"sony bravia theater black micro system davis50b 5.1-channel surround sound golf ball-sized speakers compact design s-air digital wireless capability hdmi connectivity bravia sync digital cinema sound ( dcs ) technology s-master digital amplifier portable audio enhancer black finish","price_left":null,"cluster_id_left":813,
 # "id_right":"buy_949","name_right":"sony bravia dav-is50 \/ b home theater system","description_right":"dvd player , 5.1 speakers 1 disc ( s ) progressive scan 450w rms dolby digital ex , dolby pro logic , dolby pro logic ii","price_right":null,"cluster_id_right":813,
 # "label":1,"pair_id":"abt_942#buy_949"}
 def read(file, schema=True):
     with open(file) as f:
```

### Comparing `libem-0.0.4/libem/prepare/datasets/amazon_google.py` & `libem-0.0.5/libem/prepare/datasets/walmart_amazon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import json
 
 import libem.prepare.datasets as datasets
 
-path = os.path.join(datasets.LIBEM_SAMPLE_DATA_PATH, "amazon-google")
+path = os.path.join(datasets.LIBEM_SAMPLE_DATA_PATH, "walmart-amazon")
 test_file = os.path.join(path, "test.ndjson")
 train_file = os.path.join(path, "train.ndjson")
 valid_file = os.path.join(path, "valid.ndjson")
+description = "The Walmart-Amazon dataset for entity resolution derives " \
+              "from the online retailers Walmart.com and Amazon.com."
 
 
 # sample data:
-# {"id_left":"amazon_1191","title_left":"sims 2 glamour life stuff pack","manufacturer_left":"aspyr media","price_left":24.99,"cluster_id_left":810,
-#  "id_right":"google_567","title_right":"aspyr media inc sims 2 glamour life stuff pack","manufacturer_right":null,"price_right":23.44,"cluster_id_right":810,
-#  "label":1,"pair_id":"amazon_1191#google_567"}
+# {"id_left":"walmart_88","title_left":"balt wheasel easel adjustable melamine dry erase board white","category_left":"stationery & office machinery","brand_left":"balt","modelno_left":"33250","price_left":239.88,"cluster_id_left":463,
+# "id_right":"amazon_3269","title_right":"balt inc. wheasel easel adjustable melamine dry erase board 28 3 4 x 59 1 2 white","category_right":"laminating supplies","brand_right":"mayline","modelno_right":null,"price_right":134.45,"cluster_id_right":463,
+# "label":1,"pair_id":"walmart_88#amazon_3269"}
 def read(file, schema=True):
     with open(file) as f:
         for line in f:
             data = json.loads(line.strip())
             parsed_data = {'left': {}, 'right': {}, 'label': data.get('label', None)}
 
             # clean the data
```

### Comparing `libem-0.0.4/libem/prepare/datasets/dblp_acm.py` & `libem-0.0.5/libem/prepare/datasets/dblp_acm.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import libem.prepare.datasets as datasets
 
 path = os.path.join(datasets.LIBEM_SAMPLE_DATA_PATH, "dblp-acm")
 test_file = os.path.join(path, "test.ndjson")
 train_file = os.path.join(path, "train.ndjson")
 valid_file = os.path.join(path, "valid.ndjson")
-
+description = "The DBLP-ACM dataset for entity resolution derives " \
+              "from the DBLP and ACM digital libraries."
 
 # sample data:
 # {"id_left":"dblp_1835","title_left":"wavelet-based histograms for selectivity estimation","authors_left":"jeffrey scott vitter , yossi matias , min wang","venue_left":"sigmod conference","year_left":1998,"cluster_id_left":2110,
 # "id_right":"acm_184","title_right":"wavelet-based histograms for selectivity estimation","authors_right":"yossi matias , jeffrey scott vitter , min wang","venue_right":"international conference on management of data","year_right":1998,"cluster_id_right":2110,
 # "label":1,"pair_id":"dblp_1835#acm_184"}
 def read(file, schema=True):
     with open(file) as f:
```

### Comparing `libem-0.0.4/libem/prepare/datasets/dblp_scholar.py` & `libem-0.0.5/libem/prepare/datasets/dblp_scholar.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import libem.prepare.datasets as datasets
 
 path = os.path.join(datasets.LIBEM_SAMPLE_DATA_PATH, "dblp-scholar")
 test_file = os.path.join(path, "test.ndjson")
 train_file = os.path.join(path, "train.ndjson")
 valid_file = os.path.join(path, "valid.ndjson")
+description = "The DBLP-Scholar dataset for entity resolution derives " \
+              "from the DBLP and Google Scholar digital libraries."
 
 
 # sample data:
 # {"id_left":"dblp_1853","title_left":"further improvements on integrity constraint checking for stratifiable deductive databases","authors_left":"s lee , t ling","venue_left":"vldb","year_left":1996,"cluster_id_left":2290,
 # "id_right":"scholar_17524","title_right":"further improvements on integrity constraint checking for stratifiable deductive databases","authors_right":"sy lee , tw ling","venue_right":"vldb ,","year_right":1996.0,"cluster_id_right":2290,
 # "label":1,"pair_id":"dblp_1853#scholar_17524"}
 def read(file, schema=True):
```

### Comparing `libem-0.0.4/libem.egg-info/SOURCES.txt` & `libem-0.0.5/libem.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,20 +16,23 @@
 libem.egg-info/top_level.txt
 libem/browse/__init__.py
 libem/browse/function.py
 libem/browse/parameter.py
 libem/browse/prompt.py
 libem/calibrate/__init__.py
 libem/calibrate/function.py
-libem/calibrate/parameter.py
-libem/calibrate/prompt.py
+libem/calibrate/interface.py
 libem/core/__init__.py
 libem/core/eval.py
+libem/core/log.py
 libem/core/model.py
 libem/core/struct.py
+libem/core/telemetry.py
+libem/core/trace.py
+libem/core/util.py
 libem/match/__init__.py
 libem/match/function.py
 libem/match/parameter.py
 libem/match/prompt.py
 libem/prepare/__init__.py
 libem/prepare/function.py
 libem/prepare/parameter.py
@@ -38,28 +41,22 @@
 libem/prepare/datasets/abt_buy.py
 libem/prepare/datasets/amazon_google.py
 libem/prepare/datasets/dblp_acm.py
 libem/prepare/datasets/dblp_scholar.py
 libem/prepare/datasets/walmart_amazon.py
 libem/tune/__init__.py
 libem/tune/function.py
-libem/tune/parameter.py
-libem/tune/prompt.py
+libem/tune/interface.py
 libem/tune/storage.py
 libem/tune/learn/__init__.py
 libem/tune/learn/function.py
+libem/tune/learn/interface.py
 libem/tune/learn/parameter.py
 libem/tune/learn/prompt.py
 libem/tune/load/__init__.py
 libem/tune/load/function.py
-libem/tune/load/parameter.py
-libem/tune/load/prompt.py
 libem/tune/save/__init__.py
 libem/tune/save/function.py
-libem/tune/save/parameter.py
-libem/tune/save/prompt.py
 libem/tune/search/__init__.py
 libem/tune/search/function.py
-libem/tune/search/parameter.py
-libem/tune/search/prompt.py
 serve/__init__.py
 serve/run.py
```

### Comparing `libem-0.0.4/serve/run.py` & `libem-0.0.5/serve/run.py`

 * *Files identical despite different names*

