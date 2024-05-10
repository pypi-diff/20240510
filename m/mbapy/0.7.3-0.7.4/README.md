# Comparing `tmp/mbapy-0.7.3.tar.gz` & `tmp/mbapy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.7.3.tar", last modified: Thu Apr 25 15:18:07 2024, max compression
+gzip compressed data, was "mbapy-0.7.4.tar", last modified: Fri May 10 13:06:23 2024, max compression
```

## Comparing `mbapy-0.7.3.tar` & `mbapy-0.7.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.150521 mbapy-0.7.3/
--rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.3/LICENSE
--rw-rw-rw-   0        0        0      214 2024-04-21 10:41:48.000000 mbapy-0.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7500 2024-04-25 15:18:07.149519 mbapy-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     5549 2024-04-04 11:37:22.000000 mbapy-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:06.993658 mbapy-0.7.3/mbapy/
--rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.3/mbapy/__init__.py
--rw-rw-rw-   0        0        0      402 2024-04-25 15:17:56.000000 mbapy-0.7.3/mbapy/__version__.py
--rw-rw-rw-   0        0        0    27309 2024-04-25 14:59:13.000000 mbapy-0.7.3/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.031911 mbapy-0.7.3/mbapy/bio/
--rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.3/mbapy/bio/__init__.py
--rw-rw-rw-   0        0        0    21232 2024-03-12 14:00:39.000000 mbapy-0.7.3/mbapy/bio/peptide.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.044903 mbapy-0.7.3/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.045902 mbapy-0.7.3/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.049999 mbapy-0.7.3/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.055026 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.3/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.3/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.057996 mbapy-0.7.3/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.3/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0    22088 2024-04-21 10:54:51.000000 mbapy-0.7.3/mbapy/file.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.062168 mbapy-0.7.3/mbapy/file_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.3/mbapy/file_utils/__init__.py
--rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.3/mbapy/file_utils/image.py
--rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.3/mbapy/file_utils/video.py
--rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/game.py
--rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.3/mbapy/paper.py
--rw-rw-rw-   0        0        0    11093 2024-04-23 13:37:47.000000 mbapy-0.7.3/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.074159 mbapy-0.7.3/mbapy/plot_utils/
--rw-rw-rw-   0        0        0        0 2024-04-21 13:25:30.000000 mbapy-0.7.3/mbapy/plot_utils/__init__.py
--rw-rw-rw-   0        0        0    15028 2024-04-24 01:25:33.000000 mbapy-0.7.3/mbapy/plot_utils/bar_utils.py
--rw-rw-rw-   0        0        0        0 2024-04-21 13:26:21.000000 mbapy-0.7.3/mbapy/plot_utils/line_utils.py
--rw-rw-rw-   0        0        0    11533 2024-04-23 03:04:53.000000 mbapy-0.7.3/mbapy/plot_utils/scatter_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.081195 mbapy-0.7.3/mbapy/sci_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.3/mbapy/sci_utils/__init__.py
--rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.3/mbapy/sci_utils/paper_download.py
--rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.3/mbapy/sci_utils/paper_parse.py
--rw-rw-rw-   0        0        0    16559 2024-04-25 15:14:19.000000 mbapy-0.7.3/mbapy/sci_utils/paper_search.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.116393 mbapy-0.7.3/mbapy/scripts/
--rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/__init__.py
--rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/__main__.py
--rw-rw-rw-   0        0        0     2821 2024-04-21 10:45:32.000000 mbapy-0.7.3/mbapy/scripts/_main_.py
--rw-rw-rw-   0        0        0      522 2024-04-10 06:02:44.000000 mbapy-0.7.3/mbapy/scripts/_script_utils_.py
--rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/avif.py
--rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.3/mbapy/scripts/cluster.py
--rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/cnipa.py
--rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/cp.py
--rw-rw-rw-   0        0        0     4806 2024-04-24 02:05:38.000000 mbapy-0.7.3/mbapy/scripts/duitang.py
--rw-rw-rw-   0        0        0     2651 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/extract-dir.py
--rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/extract_paper.py
--rw-rw-rw-   0        0        0     3781 2024-04-15 15:02:22.000000 mbapy-0.7.3/mbapy/scripts/file-size.py
--rw-rw-rw-   0        0        0     9141 2024-04-23 02:49:34.000000 mbapy-0.7.3/mbapy/scripts/hplc.py
--rw-rw-rw-   0        0        0    14775 2024-04-23 02:48:49.000000 mbapy-0.7.3/mbapy/scripts/mass.py
--rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/mv.py
--rw-rw-rw-   0        0        0    26028 2024-04-10 09:30:41.000000 mbapy-0.7.3/mbapy/scripts/peptide.py
--rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.3/mbapy/scripts/reviz.py
--rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/rm.py
--rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/scihub.py
--rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/scihub_selenium.py
--rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/splash_img.py
--rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.7.3/mbapy/scripts/video.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.125388 mbapy-0.7.3/mbapy/stats/
--rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.3/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.3/mbapy/stats/cluster.py
--rw-rw-rw-   0        0        0    15779 2024-04-09 06:03:49.000000 mbapy-0.7.3/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     4009 2024-04-23 02:29:03.000000 mbapy-0.7.3/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    16955 2024-04-05 10:19:56.000000 mbapy-0.7.3/mbapy/stats/test.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.134394 mbapy-0.7.3/mbapy/storage/
--rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libsci.dll
--rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libsci.so
--rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libstats.dll
--rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libstats.so
--rw-rw-rw-   0        0        0     3546 2024-04-21 10:41:06.000000 mbapy-0.7.3/mbapy/storage/mbapy-cli-scripts-list.json
--rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.3/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.143379 mbapy-0.7.3/mbapy/web_utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.3/mbapy/web_utils/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.3/mbapy/web_utils/parse.py
--rw-rw-rw-   0        0        0    35800 2024-04-25 03:11:33.000000 mbapy-0.7.3/mbapy/web_utils/request.py
--rw-rw-rw-   0        0        0    31544 2024-04-25 01:49:36.000000 mbapy-0.7.3/mbapy/web_utils/spider.py
--rw-rw-rw-   0        0        0    16389 2024-04-25 13:20:01.000000 mbapy-0.7.3/mbapy/web_utils/task.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.028787 mbapy-0.7.3/mbapy.egg-info/
--rw-rw-rw-   0        0        0     7500 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2231 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      961 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      899 2024-04-09 04:33:27.000000 mbapy-0.7.3/requirements.json
--rw-rw-rw-   0        0        0       42 2024-04-25 15:18:07.150521 mbapy-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     3400 2024-04-25 15:18:02.000000 mbapy-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.148385 mbapy-0.7.3/test/
--rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.3/test/test_base.py
--rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.3/test/test_game.py
--rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.3/test/test_web.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.646023 mbapy-0.7.4/
+-rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0      214 2024-04-21 10:41:48.000000 mbapy-0.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    10206 2024-05-10 13:06:23.644024 mbapy-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8039 2024-04-30 02:19:58.000000 mbapy-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.461975 mbapy-0.7.4/mbapy/
+-rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.4/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      402 2024-05-10 13:06:01.000000 mbapy-0.7.4/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    27309 2024-04-25 14:59:13.000000 mbapy-0.7.4/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.523398 mbapy-0.7.4/mbapy/bio/
+-rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.4/mbapy/bio/__init__.py
+-rw-rw-rw-   0        0        0    21230 2024-04-29 08:59:11.000000 mbapy-0.7.4/mbapy/bio/peptide.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.537643 mbapy-0.7.4/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.541641 mbapy-0.7.4/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.547202 mbapy-0.7.4/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.552198 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.4/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.4/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.553255 mbapy-0.7.4/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.4/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    22088 2024-04-21 10:54:51.000000 mbapy-0.7.4/mbapy/file.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.557255 mbapy-0.7.4/mbapy/file_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.4/mbapy/file_utils/__init__.py
+-rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.4/mbapy/file_utils/image.py
+-rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.4/mbapy/file_utils/video.py
+-rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/game.py
+-rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.4/mbapy/paper.py
+-rw-rw-rw-   0        0        0    11217 2024-05-04 10:36:23.000000 mbapy-0.7.4/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.564867 mbapy-0.7.4/mbapy/plot_utils/
+-rw-rw-rw-   0        0        0        0 2024-04-21 13:25:30.000000 mbapy-0.7.4/mbapy/plot_utils/__init__.py
+-rw-rw-rw-   0        0        0    15028 2024-04-24 01:25:33.000000 mbapy-0.7.4/mbapy/plot_utils/bar_utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-21 13:26:21.000000 mbapy-0.7.4/mbapy/plot_utils/line_utils.py
+-rw-rw-rw-   0        0        0    11533 2024-04-23 03:04:53.000000 mbapy-0.7.4/mbapy/plot_utils/scatter_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.569496 mbapy-0.7.4/mbapy/sci_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.4/mbapy/sci_utils/__init__.py
+-rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.4/mbapy/sci_utils/paper_download.py
+-rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.4/mbapy/sci_utils/paper_parse.py
+-rw-rw-rw-   0        0        0    16559 2024-04-25 15:14:19.000000 mbapy-0.7.4/mbapy/sci_utils/paper_search.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.606990 mbapy-0.7.4/mbapy/scripts/
+-rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/__main__.py
+-rw-rw-rw-   0        0        0     2821 2024-04-21 10:45:32.000000 mbapy-0.7.4/mbapy/scripts/_main_.py
+-rw-rw-rw-   0        0        0     1628 2024-05-02 13:29:19.000000 mbapy-0.7.4/mbapy/scripts/_script_utils_.py
+-rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/avif.py
+-rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.4/mbapy/scripts/cluster.py
+-rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/cnipa.py
+-rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/cp.py
+-rw-rw-rw-   0        0        0     4806 2024-04-24 02:05:38.000000 mbapy-0.7.4/mbapy/scripts/duitang.py
+-rw-rw-rw-   0        0        0     3175 2024-05-03 09:21:25.000000 mbapy-0.7.4/mbapy/scripts/extract-dir.py
+-rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/extract_paper.py
+-rw-rw-rw-   0        0        0     3781 2024-04-15 15:02:22.000000 mbapy-0.7.4/mbapy/scripts/file-size.py
+-rw-rw-rw-   0        0        0    28801 2024-05-06 09:11:10.000000 mbapy-0.7.4/mbapy/scripts/hplc.py
+-rw-rw-rw-   0        0        0    26861 2024-05-10 09:08:25.000000 mbapy-0.7.4/mbapy/scripts/mass.py
+-rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/mv.py
+-rw-rw-rw-   0        0        0    29037 2024-05-10 08:37:48.000000 mbapy-0.7.4/mbapy/scripts/peptide.py
+-rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.4/mbapy/scripts/reviz.py
+-rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/rm.py
+-rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/scihub.py
+-rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/scihub_selenium.py
+-rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/splash_img.py
+-rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.7.4/mbapy/scripts/video.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.618525 mbapy-0.7.4/mbapy/stats/
+-rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.4/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.4/mbapy/stats/cluster.py
+-rw-rw-rw-   0        0        0    15779 2024-04-09 06:03:49.000000 mbapy-0.7.4/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     4009 2024-04-23 02:29:03.000000 mbapy-0.7.4/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    16955 2024-04-05 10:19:56.000000 mbapy-0.7.4/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.629536 mbapy-0.7.4/mbapy/storage/
+-rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libsci.dll
+-rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libsci.so
+-rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libstats.dll
+-rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libstats.so
+-rw-rw-rw-   0        0        0     7557 2024-04-26 14:00:52.000000 mbapy-0.7.4/mbapy/storage/mbapy-cli-scripts-list.json
+-rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.4/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.637075 mbapy-0.7.4/mbapy/web_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.4/mbapy/web_utils/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.4/mbapy/web_utils/parse.py
+-rw-rw-rw-   0        0        0    35800 2024-04-25 03:11:33.000000 mbapy-0.7.4/mbapy/web_utils/request.py
+-rw-rw-rw-   0        0        0    31544 2024-04-25 01:49:36.000000 mbapy-0.7.4/mbapy/web_utils/spider.py
+-rw-rw-rw-   0        0        0    20128 2024-05-01 10:43:48.000000 mbapy-0.7.4/mbapy/web_utils/task.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.520358 mbapy-0.7.4/mbapy.egg-info/
+-rw-rw-rw-   0        0        0    10206 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2231 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      990 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      976 2024-05-03 13:01:37.000000 mbapy-0.7.4/requirements.json
+-rw-rw-rw-   0        0        0       42 2024-05-10 13:06:23.646023 mbapy-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     3400 2024-05-10 13:06:15.000000 mbapy-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.642026 mbapy-0.7.4/test/
+-rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.4/test/test_base.py
+-rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.4/test/test_game.py
+-rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.4/test/test_web.py
```

### Comparing `mbapy-0.7.3/LICENSE` & `mbapy-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/__init__.py` & `mbapy-0.7.4/mbapy/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/base.py` & `mbapy-0.7.4/mbapy/base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/bio/peptide.py` & `mbapy-0.7.4/mbapy/bio/peptide.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,31 +305,31 @@
                         C_pg = parts[-1] + '-'
                         repr = repr.replace(C_pg,'')
                 parts = re.findall(pattern, repr)
                 parts[0] = N_pg + parts[0]
                 parts[-1] = parts[-1] + C_pg
             # generate AAs
             self.AAs = [AnimoAcid(part, aa_repr_w) for part in parts]
+        else:
+            self.AAs = []
         
     def flatten(self, inplace: bool = False):
         """
         Params:
             - inplace: bool(False), if True, make inplace change and return self, else return changed seq only
         """
         seq = []
         for aa in self.AAs:
             if isinstance(aa, list):
                 seq.extend(aa)
             else:
                 seq.append(aa)
         if inplace:
             self.AAs = seq
-            return self
-        else:
-            return seq
+        return seq
         
     def repr(self, repr_w: int = 3, include_pg: bool = True,
              include_dash: bool = True):
         """
         NOTE: if do not include dash and include pg, the N and C ternimal pg will STILL get a dash.
         """
         assert repr_w in [1, 3], "repr_w must be 1 or 3"
```

### Comparing `mbapy-0.7.3/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.7.4/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.7.4/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/bb.py` & `mbapy-0.7.4/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/data.py` & `mbapy-0.7.4/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/hyper_search.py` & `mbapy-0.7.4/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/loss.py` & `mbapy-0.7.4/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/m.py` & `mbapy-0.7.4/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/optim.py` & `mbapy-0.7.4/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/paper/bb.py` & `mbapy-0.7.4/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/dl_torch/utils.py` & `mbapy-0.7.4/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/file.py` & `mbapy-0.7.4/mbapy/file.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/file_utils/image.py` & `mbapy-0.7.4/mbapy/file_utils/image.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/file_utils/video.py` & `mbapy-0.7.4/mbapy/file_utils/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/game.py` & `mbapy-0.7.4/mbapy/game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/paper.py` & `mbapy-0.7.4/mbapy/paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/plot.py` & `mbapy-0.7.4/mbapy/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,28 +53,30 @@
     Parameters
     ----------
     n: how many colors required
     mode: kind of colors
         - hls : [default] sns.color_palette('hls', n)
         - green : sum 5 grenns
         - pair : plt.get_cmap('tab20')
-        - None : plt.get_cmap('Set1') for n<=9 or plt.get_cmap('Set3') for n<= 12
+        - others : plt.get_cmap(mode)
     """
     assert n >= 1, 'n < 1'
     ret = None
     if mode == 'hls':
         ret = rgbs2hexs(sns.color_palette('hls', n))
     elif n <= 5 and mode == 'green':
         ret = ['#80ab1c', '#405535', '#99b69b', '#92e4ce', '#72cb87'][0:n]
     elif n <= 9:
         ret = rgbs2hexs(plt.get_cmap('Set1').colors)
     elif n <= 12:
         ret = rgbs2hexs(plt.get_cmap('Set3').colors)
     elif n <= 20 and mode == 'pair':
         ret = rgbs2hexs(plt.get_cmap('tab20').colors)
+    else:
+        ret = rgbs2hexs(plt.get_cmap(mode).colors)
     if return_n and ret is not None:
         ret = ret[:n]
     return ret
     
 
 def calcu_swarm_pos(x: float, y: np.ndarray, width: float, d: Optional[float] = None):
     """
@@ -137,29 +139,28 @@
         if 'tick_size' in kwargs:
             axs[-1].tick_params(labelsize = kwargs['tick_size'])
         if 'label_size' in kwargs:
             axs[-1].set_xlabel('Theoretical Quantiles', fontsize = kwargs['label_size'])
             axs[-1].set_ylabel('Sample Quantiles', fontsize = kwargs['label_size'])
     return axs
             
-def save_show(path:str, dpi = 300, bbox_inches = 'tight'):
+def save_show(path:str, dpi = 300, bbox_inches = 'tight', show: bool = True):
     """
     Saves the current matplotlib figure to a file at the specified path and displays the figure.
 
     Parameters:
-        path (str): The path where the figure will be saved.
-        dpi (int, optional): The resolution of the saved figure in dots per inch. Default is 300.
-        bbox_inches (str or Bbox, optional): The portion of the figure to save. Default is 'tight'.
-
-    Returns:
-        None
+        - path (str): The path where the figure will be saved.
+        - dpi (int, optional): The resolution of the saved figure in dots per inch. Default is 300.
+        - bbox_inches (str or Bbox, optional): The portion of the figure to save. Default is 'tight'.
+        - show (bool, optional): Whether to show the figure after saving. Default is True.
     """
     plt.tight_layout()
     plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches)
-    plt.show()
+    if show:
+        plt.show()
     
 def plot_stats_star(x1: float, x2: float, h: float, endpoint: float, p_value: float,
                     ax = plt, p2star: Callable[[float], str] = p_value_to_stars):
     """
     Params
         - x1: The x-coordinate of the left endpoint.
         - x2: The x-coordinate of the right endpoint.
```

### Comparing `mbapy-0.7.3/mbapy/plot_utils/bar_utils.py` & `mbapy-0.7.4/mbapy/plot_utils/bar_utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/plot_utils/scatter_utils.py` & `mbapy-0.7.4/mbapy/plot_utils/scatter_utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/sci_utils/paper_download.py` & `mbapy-0.7.4/mbapy/sci_utils/paper_download.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/sci_utils/paper_parse.py` & `mbapy-0.7.4/mbapy/sci_utils/paper_parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/sci_utils/paper_search.py` & `mbapy-0.7.4/mbapy/sci_utils/paper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/_main_.py` & `mbapy-0.7.4/mbapy/scripts/_main_.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/avif.py` & `mbapy-0.7.4/mbapy/scripts/avif.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/cluster.py` & `mbapy-0.7.4/mbapy/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/cnipa.py` & `mbapy-0.7.4/mbapy/scripts/cnipa.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/cp.py` & `mbapy-0.7.4/mbapy/scripts/cp.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/duitang.py` & `mbapy-0.7.4/mbapy/scripts/duitang.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/extract-dir.py` & `mbapy-0.7.4/mbapy/scripts/rm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,58 @@
 '''
 Date: 2024-02-05 15:12:32
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-02-20 10:12:23
+LastEditTime: 2024-02-20 10:01:09
 Description: 
 '''
 
 import argparse
 import os
-import shutil
 from typing import Dict, List
 
 from tqdm import tqdm
+from mbapy.base import put_err
+from mbapy.file import get_paths_with_extension
 
 if __name__ == '__main__':
-    from mbapy.base import put_err
-    from mbapy.file import get_paths_with_extension
     from mbapy.scripts._script_utils_ import clean_path, show_args
 else:
-    from ..base import put_err
-    from ..file import get_paths_with_extension
     from ._script_utils_ import clean_path, show_args
     
 
 def main(sys_args: List[str] = None):
-    # set and parse args
-    args_paser = argparse.ArgumentParser(description = 'move files with specific suffix or sub-string in name to root dir')
+    args_paser = argparse.ArgumentParser(description = 'delete files with specific suffix or sub-string in name')
     args_paser.add_argument('-t', '--type', type = str, default='',
                             help='format of files to remove, splited by ",". Default is %(default)s')
     args_paser.add_argument('-n', '--name', type = str, default='',
                             help='sub-string of name of files to remove. Default is %(default)s')
-    args_paser.add_argument('-i', '--input', type=str, default='.',
-                            help='files path or dir path. Default is %(default)s.')
+    args_paser.add_argument('-i', '--input', type=str,
+                            help='files path or dir path.')
     args_paser.add_argument('-r', '--recursive', action='store_true', default=False,
                             help='FLAG, recursive search. Default is %(default)s.')
-    args_paser.add_argument('-j', '--join-str', type=str, default=' ',
-                            help='join string of file name. Default is %(default)s.')
     args = args_paser.parse_args(sys_args)
-    # process args
+    
     args.type = args.type.split(',')
     args.input = clean_path(args.input)
-    show_args(args, ['type', 'input', 'name', 'recursive', 'join_str'])
+    show_args(args, ['type', 'input', 'name', 'recursive'])
     
     paths = get_paths_with_extension(args.input, args.type,
                                      args.recursive, args.name)
     print(f'files to remove: {len(paths)}')
     # manual confirm
     inputs = input('Are you sure to delete these files? (y/n) ')
     if inputs.lower() != 'y':
         print('cancel delete files')
         return []
-    # move files
-    root = str(args.input)
+    # delete files
     for path in tqdm(paths):
         try:
-            path = str(clean_path(path))
-            dist = path.replace(root, '').replace(os.path.sep, ' ')
-            dist = os.path.join(root, dist)
-            shutil.move(path, dist)
+            os.remove(path)
         except Exception as e:
-            put_err(f'Error: {e}. Can not move {path}, skip')
+            put_err(f'Error: {e}. Can not delete {path}, skip')
     return paths
     
     
 
 # dev code
 # main(['-i', r'E:\\', '-t', 'JPG'])
```

### Comparing `mbapy-0.7.3/mbapy/scripts/extract_paper.py` & `mbapy-0.7.4/mbapy/scripts/extract_paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/file-size.py` & `mbapy-0.7.4/mbapy/scripts/file-size.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/mv.py` & `mbapy-0.7.4/mbapy/scripts/mv.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/peptide.py` & `mbapy-0.7.4/mbapy/scripts/peptide.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import argparse
+import itertools
 import os
+import math
 import sys
 from copy import deepcopy
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, List
 
 import numpy as np
+from tqdm import tqdm
 
 os.environ['MBAPY_AUTO_IMPORT_TORCH'] = 'False'
 os.environ['MBAPY_FAST_LOAD'] = 'True'
-from mbapy import base, file
-from mbapy.bio.peptide import AnimoAcid, Peptide
 
-if __name__ == '__main__':
-    from mbapy.scripts._script_utils_ import clean_path, show_args
-else:
-    from ._script_utils_ import clean_path, show_args
+# if __name__ == '__main__':
+from mbapy.base import put_err, split_list
+from mbapy.bio.peptide import AnimoAcid, Peptide
+from mbapy.file import opts_file, get_valid_file_path
+from mbapy.web import TaskPool
+from mbapy.scripts._script_utils_ import clean_path, Command, excute_command, show_args
+# else:
+#     from ..base import put_err
+#     from ..file import opts_file, get_valid_file_path
+#     from ._script_utils_ import clean_path, show_args
+#     from ..bio.peptide import AnimoAcid, Peptide
 
 
 def calcu_substitution_value(args: argparse.Namespace):
     """
     Calculates the substitution value and plots a scatter plot with a linear 
     regression model. The function first processes the input arguments to 
     convert the strings to float values and stores them in arrays. It then 
@@ -39,14 +47,15 @@
     import matplotlib.pyplot as plt
     import seaborn as sns
     from sklearn.linear_model import LinearRegression
     
     a = np.array([float(i) for i in args.absorbance.split(',') if len(i)])
     m = np.array([float(i) for i in args.weight.split(',') if len(i)])
     mean_subval = np.mean(args.coff*a/m)
+    print(f'\nSubstitution Value: {args.coff*a/m}')
     print(f'\nAvg Substitution Value: {mean_subval}')
     
     fig, ax = plt.subplots(figsize=(8, 6))
     ax.set_xlim(0, max(20, m.max()*1.2))
     ax.set_ylim(0, max(0.4, a.max()*1.2))
 
     regressor = LinearRegression()
@@ -176,16 +185,15 @@
                 aa.C_protect = 'OH'
         # change mutate branch 's pos 's sum_repeat to tree.opts.repeat_AA + 1
         tree.mutate.pos[2] = tree.opts.AA_repeat + 1
         # trun off the repeat AA opts in mutate branches
         tree.mutate.opts = MutationOpts(AA_repeat=0)
         # decrease the repeat AA opts in remain branches
         tree.remain.opts.AA_repeat -= 1
-        return tree
-        
+        return tree        
 
     def delete_NCR(self, tree: 'MutationTree', NCR: str):
         """
         perform delete_NCR mutation in tree.mutate branch, trun off the tree.branches.opt.X_protect_deletion
         Params:
             - tree: MutationTree, tree to opt.
             - NCR: str, N or C or R.
@@ -215,15 +223,15 @@
                 - trun off opts in two branches
                 - move pos ONLY in mutate branch.
                 - DO NOT CHECK IF MEETS END in both this dot and two branches.
                 - return the tree.
         """
         able = tree.opts.check_empty(tree.pos, tree.seq, args)
         if able:
-            # generate two branch
+            # generate two branch and set seq to None to free memory
             tree.generate_two_branch()
             # perform mutation
             if 'AA_deletion' in able:
                 tree = self.delete_AA(tree, args.max_repeat)
             elif 'AA_repeat' in able:
                 tree = self.repeat_AA(tree)
             elif 'N_protect_deletion' in able:
@@ -266,25 +274,30 @@
             cp.mutate = deepcopy(self.mutate)
         else:
             cp.father = father
             cp.remain = remain
             cp.mutate = mutate
         return cp
     
-    def extract_mutations(self):
+    def extract_mutations(self, flatten: bool = True):
         """
         extract all terminal dots from mutations(Tree)
-            - will CHANGE it's peptide.AAs
+            - flatten==True:  will CHANGE it's peptide.AAs, return the flattened peptide.
+            - flatten==False: will simply return all leaves of MutationTree.
         """
         if self.mutate is None and self.remain is None:
-            return [self.seq.flatten(inplace=True)]
+            if flatten:
+                self.seq.flatten(inplace=True)
+                return [self.seq]
+            else:
+                return [self]
         else:
             final_seq = []
-            final_seq.extend(self.remain.extract_mutations())
-            final_seq.extend(self.mutate.extract_mutations())
+            final_seq.extend(self.remain.extract_mutations(flatten))
+            final_seq.extend(self.mutate.extract_mutations(flatten))
             return final_seq
     
     def check_is_end_pos(self):
         """check if current AA is the last AA whether in repeat or mother peptide"""
         if self.pos[0] >= len(self.peptide.AAs) - 1 and self.pos[1] >= self.pos[2] - 1:
             return True
         return False
@@ -331,14 +344,36 @@
             # it is the end, return tree
             return tree
     else: # go on with two branches
         mutate_peptide(tree.mutate, args)
         mutate_peptide(tree.remain, args)
     return tree
 
+def calcu_mutations_mw(seqs: List[Peptide], mass: bool = False, verbose: bool = True):
+    peps, mw2pep = {}, {}
+    for pep in tqdm(seqs,
+                    desc='Gathering mutations and Calculating molecular weight',
+                    disable=not verbose):
+        full_pep = Peptide(None)
+        full_pep.AAs.extend(aa.AAs for aa in pep)
+        full_pep.flatten(inplace = True)
+        if len(full_pep.AAs):
+            pep_repr = str(full_pep)
+            if pep_repr not in peps:
+                peps[pep_repr] = len(peps)
+                if mass:
+                    mw = full_pep.calcu_mass()
+                else:
+                    mw = full_pep.calcu_mw()
+                if mw in mw2pep:
+                    mw2pep[mw].append(full_pep)
+                else:
+                    mw2pep[mw] = [full_pep]
+    return peps, mw2pep
+
 def calcu_mw_of_mutations(args: argparse.Namespace):
     """
     Calculates the molecular weight of mutations based on the given arguments.
 
     Args:
         args (object): An object that contains the following attributes:
             - seq (str): The input sequence.
@@ -361,77 +396,90 @@
     It iterates over each individual mutation and calculates its molecular weight.
     If the molecular weight is already present in `mw2pep`, the mutation is appended to the list of peptides with the same molecular weight.
     Otherwise, a new entry is created in `mw2pep` with the molecular weight as the key and the mutation as the value.
     Finally, the function prints the number of mutations found and the details of each mutation, along with their respective indices.
     If an output file was specified, it is closed at the end.
     """
     # set _print
-    def _print(content: str, f):
+    def _print(content: str, f, verbose = True):
         if f is not None:
             f.write(content+'\n')
-        print(content)
+        if verbose:
+            print(content)
     if args.out is not None:
         args.out = clean_path(args.out)
         if os.path.isdir(args.out):
-            file_name = file.get_valid_file_path(" ".join(sys.argv[1:]))+'.txt'
+            file_name = get_valid_file_path(" ".join(sys.argv[1:]))+'.txt'
             args.out = os.path.join(args.out, file_name)
         f = open(args.out, 'w')
     else:
         f = None
     # show args
-    show_args(args, ['seq', 'weight','max_repeat', 'disable_aa_deletion', 'out','mass'],
+    verbose = not args.disable_verbose
+    show_args(args, ['seq', 'weight', 'max_repeat', 'disable_aa_deletion',
+                     'out', 'mass', 'disable_verbose', 'multi_process'],
               printf = lambda x : _print(x, f))
     # show mother peptide info
     peptide, expand_mw_dict = calcu_mw(args, _print = lambda x : _print(x, f))
     # calcu mutations
-    all_mutations = MutationTree(peptide=peptide, seq=peptide.copy(),
-                                 opts=MutationOpts(AA_repeat=args.max_repeat),
-                                 pos=[0, 0, 1])
-    all_mutations = mutate_peptide(all_mutations, args)
-    all_mutations = all_mutations.extract_mutations()
-    mw2pep, peps = {}, {}
-    for pep in all_mutations:
-        if len(pep.AAs):
-            pep_repr = str(pep)
-            if pep_repr not in peps:
-                peps[pep_repr] = len(peps)
-                if args.mass:
-                    mw = pep.calcu_mass()
-                else:
-                    mw = pep.calcu_mw()
-                if mw in mw2pep:
-                    mw2pep[mw].append(pep)
+    seq, mw2pep, peps = [], {}, {}
+    for aa in tqdm(peptide.AAs, desc='Mutating peptide'):
+        pep = Peptide(None)
+        pep.AAs = [aa.copy()]
+        aa_mutations = MutationTree(peptide=pep, seq=pep.copy(),
+                                    opts=MutationOpts(AA_repeat=args.max_repeat),
+                                    pos=[0, 0, 1])
+        aa_mutations = mutate_peptide(aa_mutations, args)
+        seq.append(aa_mutations.extract_mutations())
+    # gather mutations, calcu mw and store in dict
+    seqs = list(itertools.product(*seq))
+    if args.multi_process == 1:
+        peps, mw2pep = calcu_mutations_mw(seqs, mass=args.mass, verbose=True)
+    else:
+        print('Gathering mutations and Calculating molecular weight...')
+        peps, mw2pep = {}, {}
+        pool = TaskPool('process', args.multi_process)
+        for i, batch in enumerate(split_list(seqs, args.process_batch)):
+            pool.add_task(f'{i}', calcu_mutations_mw, batch, args.mass, False)
+        pool.run()
+        pool.wait_till(lambda : pool.count_done_tasks() == len(pool.tasks), verbose=True)
+        for (_, (peps_i, mw2pep_i), _) in pool.tasks.values():
+            peps.update(peps_i)
+            for i in mw2pep_i:
+                if i in mw2pep:
+                    mw2pep[i].extend(mw2pep_i[i])
                 else:
-                    mw2pep[mw] = [pep]
+                    mw2pep[i] = mw2pep_i[i]
     # output info
     _print(f'\n{len(peps)-1} mutations found, followings include one original peptide seqeunce:\n', f)
-    idx, weigth_type = 0, 'Exact Mass' if args.mass else 'MW'
-    for i, mw in enumerate(sorted(mw2pep)):
-        _print(f'\n{weigth_type}: {mw:10.5f}', f)
-        for j, pep in enumerate(mw2pep[mw]):
-            mf = f'({pep.get_molecular_formula()})' if args.mass else ''
-            _print(f'    pep-{i:>4}-{j:<4}({idx:8d})({len(pep.AAs)} AA){mf}: {pep}', f)
-            idx += 1
+    if verbose:
+        idx, weigth_type = 0, 'Exact Mass' if args.mass else 'MW'
+        for i, mw in enumerate(sorted(mw2pep)):
+            _print(f'\n{weigth_type}: {mw:10.5f}', f, verbose)
+            for j, pep in enumerate(mw2pep[mw]):
+                mf = f'({pep.get_molecular_formula()})' if args.mass else ''
+                _print(f'    pep-{i:>4}-{j:<4}({idx:8d})({len(pep.AAs)} AA){mf}: {pep}', f, verbose)
+                idx += 1
     # handle f-print
     if f is not None:
         f.close()
+        # save mw2pep and peps
+        opts_file(str(args.out)+'.pkl', 'wb', data = {'mw2pep':mw2pep, 'peps':peps}, way = 'pkl')
+        
+
+class cycmmw(Command):
+    def __init__(self, args: argparse.Namespace, printf=...) -> None:
+        super().__init__(args, printf)
+
         
 def transfer_letters(args):
     # show args
-    print(f'get arg: seqeunce: {args.seq}')
-    print(f'get arg: source repr width: {args.src}')
-    print(f'get arg: target repr width: {args.trg}')
-    print(f'get arg: disable protect groups: {args.dpg}')
-    print(f'get arg: disable dash line: {args.ddash}')
-    print(f'get arg: input: {args.input}')
-    print(f'get arg: out: {args.out}')
+    show_args(args, ['seq', 'src', 'trg', 'dpg', 'ddash', 'input', 'out'])
     # get input
     if args.input is not None:
-        from mbapy.base import put_err
-        from mbapy.file import opts_file
         path = clean_path(args.input)
         peps = []
         for line in opts_file(path, way='lines'):
             try:
                 peps.append(Peptide(line, args.src))
             except:
                 put_err(f'error when parsing: {line}, skip')
@@ -455,27 +503,22 @@
     'molecularweight': calcu_mw,
     'molecular-weight': calcu_mw,
     
     'mmw': calcu_mw_of_mutations,
     'mutationweight': calcu_mw_of_mutations,
     'mutation-weight': calcu_mw_of_mutations,
     
+    'cycmmw': None,
+    'cyclicmutationweight': None,
+    
     'letters': transfer_letters,
     'transfer-letters': transfer_letters,
 }
 
 
-# if __name__ == '__main__':
-#     # dev code
-#     from mbapy.game import BaseInfo
-#     calcu_mw_of_mutations(BaseInfo(seq = 'Fmoc-Cys(Acm)-Val-Asn(Trt)', out = '.',
-#                                    max_repeat = 1, weight = '', mass = False))
-#     calcu_mw_of_mutations(BaseInfo(seq = 'Fmoc-Cys(Acm)-Val-Asn(Trt)', out = '.',
-#                                    max_repeat = 1, weight = '', mass = True))
-
 def main(sys_args: List[str] = None):
     args_paser = argparse.ArgumentParser()
     subparsers = args_paser.add_subparsers(title='subcommands', dest='sub_command')
     
     sub_val_args = subparsers.add_parser('subval', aliases = ['sb'], description='calcu SPPS substitution value for a release test of resin.')
     sub_val_args.add_argument('-a', '-A', '--absorbance', '--Absorbance', type = str,
                               help='Absorbance (OD value), input as 0.503,0.533')
@@ -501,14 +544,20 @@
                                 help='max times for repeat a AA in sequence')
     mutationweight.add_argument('--disable-aa-deletion', action='store_true', default=False,
                                 help='disable AA deletion in mutations.')
     mutationweight.add_argument('-o', '--out', type = str, default = None,
                                 help='save results to output file/dir. Defaults None, do not save.')
     mutationweight.add_argument('-m', '--mass', action='store_true', default=False,
                                 help='calcu Exact Mass instead of Molecular Weight.')
+    mutationweight.add_argument('--disable-verbose', action='store_true', default=False,
+                                help='disable verbose output to console.')
+    mutationweight.add_argument('--multi-process', type = int, default = 1,
+                                help='number of multi-process to use. Defaults 1, no multi-process.')
+    mutationweight.add_argument('--process-batch', type = int, default = 500000,
+                                help='number of peptides to process in each batch. Defaults %(default)% in a batch.')
     
     letters = subparsers.add_parser('letters', aliases = ['transfer-letters'], description='transfer AnimoAcid repr letters width.')
     letters.add_argument('-s', '--seq', '--seqeunce', '--pep', '--peptide', type = str, default='',
                                 help='peptide seqeunce, input as Fmoc-Cys(Acm)-Leu-OH or ABC(Trt)DE')
     letters.add_argument('--src', '--source-width', type = int, choices=[1, 3], default = 3,
                                 help='source repr width of AnimoAcid, only accept 1 and 3.')
     letters.add_argument('--trg', '--target-width', type = int, choices=[1, 3], default = 1,
@@ -524,11 +573,21 @@
     
     args = args_paser.parse_args(sys_args)
     
     if args.sub_command in _str2func:
         print(f'excuting command: {args.sub_command}')
         _str2func[args.sub_command](args)
     else:
-        base.put_err(f'no such sub commmand: {args.sub_command}')
+        put_err(f'no such sub commmand: {args.sub_command}')
 
 if __name__ == "__main__":
+    # dev code. MUST BE COMMENTED OUT WHEN PUBLISHING
+    # from mbapy.base import TimeCosts
+    # @TimeCosts(5)
+    # def func(idx, mp):
+    # main(f'mmw -s Fmoc-Cys(Acm)-Val-Asn(Trt)-Cys(Acm)-Val-Asn(Trt) -m --multi-process 2 --process-batch 1000'.split())
+    # # func(mp = 1) # func used     33.542s in total,      6.708s by mean (release run)
+    # # func(mp = 3) # func used     74.241s in total,     14.848s by mean (release run)
+    # # func(mp = 4) # func used     73.012s in total,     14.602s by mean (release run)
+    
+    # release code
     main()
```

### Comparing `mbapy-0.7.3/mbapy/scripts/reviz.py` & `mbapy-0.7.4/mbapy/scripts/reviz.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/scihub.py` & `mbapy-0.7.4/mbapy/scripts/scihub.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/scihub_selenium.py` & `mbapy-0.7.4/mbapy/scripts/scihub_selenium.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/splash_img.py` & `mbapy-0.7.4/mbapy/scripts/splash_img.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/scripts/video.py` & `mbapy-0.7.4/mbapy/scripts/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/stats/__init__.py` & `mbapy-0.7.4/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/stats/cluster.py` & `mbapy-0.7.4/mbapy/stats/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/stats/df.py` & `mbapy-0.7.4/mbapy/stats/df.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/stats/geography.py` & `mbapy-0.7.4/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/stats/reg.py` & `mbapy-0.7.4/mbapy/stats/reg.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/stats/test.py` & `mbapy-0.7.4/mbapy/stats/test.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/storage/libsci.dll` & `mbapy-0.7.4/mbapy/storage/libsci.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/storage/libsci.so` & `mbapy-0.7.4/mbapy/storage/libsci.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/storage/libstats.dll` & `mbapy-0.7.4/mbapy/storage/libstats.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/storage/libstats.so` & `mbapy-0.7.4/mbapy/storage/libstats.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/web.py` & `mbapy-0.7.4/mbapy/web.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/web_utils/parse.py` & `mbapy-0.7.4/mbapy/web_utils/parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/web_utils/request.py` & `mbapy-0.7.4/mbapy/web_utils/request.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/web_utils/spider.py` & `mbapy-0.7.4/mbapy/web_utils/spider.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy/web_utils/task.py` & `mbapy-0.7.4/mbapy/web_utils/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import _thread
 import asyncio
 import os
 import re
 import time
 import threading
+import multiprocessing
 from collections import namedtuple
 from enum import Enum
+from functools import partial
 from queue import Queue
 from typing import Any, Callable, Dict, List, Tuple, Union
+from uuid import uuid4
+
+from tqdm import tqdm
 
 if __name__ == '__main__':
     # dev mode
     from mbapy.base import put_err, put_log, parameter_checker
 else:
     from ..base import put_err, put_log, parameter_checker
 
@@ -237,22 +242,27 @@
         - tasks (Dict[str, asyncio.Future]): task name to future.
         - TASK_NOT_FOUND (TaskStatus): signal FLAG, task not found.
         - TASK_NOT_FINISHED (TaskStatus): signal FLAG, task not finished.
         - TASK_NOT_SUCCEEDED (TaskStatus): signal FLAG, task not succeeded.
         
     Methods:
     """
-    @parameter_checker(mode = lambda mode: mode in ['async', 'thread', 'threads'])
-    def __init__(self, mode: str = 'async', n_worker: int = None):
+    @parameter_checker(mode = lambda mode: mode in ['async', 'thread',
+                                                    'threads', 'process'])
+    def __init__(self, mode: str = 'async', n_worker: int = None,
+                 sleep_while_empty: float = 0.1):
         """
         Parameters:
             - mode (str, default='async'): 'async' or 'thread', use asyncio or threading to run a pool.
                 - If it's IO heavy and has suitable coroutine function, use 'async'
                 - If it's IO heavy and only has normal function, and wants run ONE task at ONCE, use 'thread'. Use Queue to cache tasks and run ONE task at ONCE.
                 - If it's IO heavy and only has normal function, and wants run MULTI tasks at ONCE, use 'threads'. Use Queue to cache tasks and run MULTI tasks at ONCE.
+                - If it's CPU heavy and wants run MULTI tasks at ONCE, use 'process'. Use multiprocessing.Pool to run MULTI tasks at ONCE.
+            - n_worker (int, default=None): number of worker threads or processes.
+            - sleep_while_empty (float, default=0.1): sleep time in a loop while task queue is empty.
         """
         if mode in ['async', 'thread'] and n_worker is not None:
             put_err(f'n_worker should be None when mode is {mode}, skip')
         self.MODE = mode
         self.N_WORKER = n_worker
         self._async_loop: asyncio.AbstractEventLoop = None
         self._thread_task_queue: Queue = Queue()
@@ -274,109 +284,166 @@
                 task_name, task_func, task_args, task_kwargs = self._thread_task_queue.get()
                 try:
                     result = task_func(*task_args, **task_kwargs)
                     self._thread_result_queue.put((task_name, result, TaskStatus.SUCCEED))
                 except Exception as e:
                     self._thread_result_queue.put((task_name, e, TaskStatus.NOT_SUCCEEDED))
             time.sleep(0.1)
+            
+    def _run_process_loop(self):
+        pool, tasks_cache = multiprocessing.Pool(self.N_WORKER), {}
+        while not self._thread_quit_event.is_set():
+            # put async result into cache
+            if not self._thread_task_queue.empty():
+                task_name, task_func, task_args, task_kwargs = self._thread_task_queue.get()
+                tasks_cache[task_name] = pool.apply_async(task_func, task_args, task_kwargs)
+            # get finished tasks from cache
+            for task_name, task_result in list(tasks_cache.items()):
+                if task_result.ready(): # 无论任务是否因异常结束，ready()都返回True
+                    try:
+                        self._thread_result_queue.put((task_name, task_result.get(),
+                                                       TaskStatus.SUCCEED))
+                    except Exception as e:
+                        self._thread_result_queue.put((task_name, e, TaskStatus.NOT_SUCCEEDED))
+                    del tasks_cache[task_name]
+            time.sleep(0.1)
+        pool.close()
 
     def _add_task_async(self, name: str, coro_func, *args, **kwargs):
         future = asyncio.run_coroutine_threadsafe(coro_func(*args, **kwargs), self._async_loop)
-        self.tasks[name] = future
+        future.add_done_callback(partial(self._query_async_task_callback, task_name=name))
+        self.tasks[name] = TaskStatus.NOT_RETURNED
         return name
     
     def _add_task_thread(self, name: str, func, *args, **kwargs):
         self._thread_task_queue.put((name, func, args, kwargs))
         self.tasks[name] = TaskStatus.NOT_RETURNED
         return name
     
-    def _add_task_threads(self, name: str, func, *args, **kwargs):
-        return self._add_task_thread(name, func, *args, **kwargs)
-    
     def add_task(self, name: str, coro_func, *args, **kwargs):
+        # check name
         if name == '' or name is None:
-            name = f'{coro_func.__name__}-{time.time():.2f}'
+            name = f'{coro_func.__name__}-{uuid4()}'
         if name in self.tasks:
             put_err(f'Task {name} already exists, replace it with the new one')
-        return getattr(self, f'_add_task_{self.MODE}')(name, coro_func, *args, **kwargs)
-
-    def _query_async_task(self, name, block: bool = True, timeout: int = 3):
-        if name in self.tasks:
-            future = self.tasks[name]
-            if future.done():
-                try:
-                    result = future.result()
-                    del self.tasks[name]
-                    return result
-                except Exception as e:
-                    del self.tasks[name]
-                    return self.TASK_NOT_SUCCEEDED, e
-            else:
-                return self.TASK_NOT_FINISHED
-        else:
-            return self.TASK_NOT_FOUND
+        # map mode to function
+        mode = 'async' if self.MODE == 'async' else 'thread'
+        return getattr(self, f'_add_task_{mode}')(name, coro_func, *args, **kwargs)
+
+    def _query_async_task_callback(self, future: asyncio.Future, task_name: str):
+        try:
+            self._thread_result_queue.put((task_name, future.result(),
+                                           TaskStatus.SUCCEED))
+        except Exception as e:
+            self._thread_result_queue.put((task_name, e, TaskStatus.NOT_SUCCEEDED))
+            
+    def _query_task_queue(self, block: bool = True, timeout: int = 3):
+        while not self._thread_result_queue.empty():
+            try:
+                _name, result, statue = self._thread_result_queue.get(block, timeout)
+                self.tasks[_name] = (_name, result, statue)
+            except Exception as e:
+                put_err(f'error {e} when get result from queue')        
         
-    def _query_thread_task(self, name, block: bool = True, timeout: int = 3):
+    def query_task(self, name, block: bool = False, timeout: int = 3):
         # short-cut for not found
         if name not in self.tasks:
             return self.TASK_NOT_FOUND
         # retrive finished results
-        while not self._thread_result_queue.empty():
-            try:
-                _name, result, statue = self._thread_result_queue.get(block, timeout)
-                self.tasks[_name] = (_name, result, statue)
-            except:
-                pass
+        self._query_task_queue(block=block, timeout=timeout)
         # check if not return, succeed, or not succeed
         if self.tasks[name] == TaskStatus.NOT_RETURNED:
             return self.TASK_NOT_FINISHED
         else:
             _name, result, statue = self.tasks[name]
             del self.tasks[name]
             if statue == TaskStatus.NOT_SUCCEEDED:
                 put_err(f'Task {name} failed with {result}, return {result}')
             return result
+    
+    def count_waiting_tasks(self):
+        """
+        - for async mode, return the number of unfinished tasks.
+        - for thread, threads, and process mode, return the number of the un-begined tasks.
+        """
+        if self.MODE == 'async':
+            return len([None for task in self.tasks.values() if not task.done()])
+        elif self.MODE in ['thread', 'threads', 'process']:
+            return self._thread_task_queue.qsize()
         
-    def _query_threads_task(self, name, block: bool = True, timeout: int = 3):
-        return self._query_thread_task(name, block, timeout)
-        
-    def query_task(self, name: str, block: bool = False):
-        return getattr(self, f'_query_{self.MODE}_task')(name, block)
+    def count_done_tasks(self):
+        """INCLUDE succeed and failed tasks."""
+        self._query_task_queue(block=False)
+        in_que = self._thread_result_queue.qsize()
+        in_dict = len([None for task in self.tasks.values() if task != TaskStatus.NOT_RETURNED])
+        return in_que + in_dict
 
     def run(self):
+        """launch the thread and event loop"""
         if self.MODE == 'async':
             self._async_loop = asyncio.new_event_loop()
         if self.MODE == 'threads':
             self.thread = []
             for _ in range(self.N_WORKER):
                 self.thread.append(threading.Thread(target=self._run_thread_loop, daemon=True))
                 self.thread[-1].start()
-        else:
+        else: # async, thread and process only need one thread
             self.thread = threading.Thread(target=getattr(self, f'_run_{self.MODE}_loop'), daemon=True)
             self.thread.start()
         return self
     
     def check_empty(self):
+        """check tasks (undo and done) is empty"""
         if self.MODE == 'async':
             for task in self.tasks.values():
                 if not task.done():
                     return False
             return True
-        elif self.MODE in ['thread', 'threads']:
+        elif self.MODE in ['thread', 'threads', 'process']:
             return self._thread_task_queue.empty()
+        
+    def wait_till(self, condition_func, wait_each_loop: float = 0.5,
+                  timeout: float = None, verbose: bool = False, *args, **kwargs):
+        """
+        wait till condition_func return True, or timeout.
+        
+        Parameters:
+            - condition_func (Callable): a function that return True or False.
+            - wait_each_loop (float, default=0.1): sleep time in a loop while waiting.
+            - timeout (float, default=None): timeout in seconds.
+            - *args, **kwargs: other args for condition_func.
+        
+        Returns:
+            - pool(TaskPool): retrun self for chaining.
+            - False: means timeout.
+        """
+        st = time.time()
+        if verbose:
+            bar =tqdm(desc='waiting', total=len(self.tasks), initial=self.count_done_tasks())
+        while not condition_func(*args, **kwargs):
+            if timeout is not None and time.time() - st > timeout:
+                return False
+            if verbose:
+                done = self.count_done_tasks()
+                bar.set_description(f'done/sum: {done}/{len(self.tasks)}')
+                bar.update(self.count_done_tasks() - bar.n)
+            time.sleep(wait_each_loop)
+        return self
     
     def close(self):
+        """close the thread and event loop, join the thread"""
+        # close async pool
         if self.MODE == 'async':
+            self._async_loop.call_soon_threadsafe(self._async_loop.stop)
             self._async_loop.close()
-            self.thread.join()
-        elif self.MODE == 'thread':
-            self._thread_quit_event.set()
+        # close thread and join it
+        self._thread_quit_event.set()
+        if self.MODE in ['async', 'thread', 'process']:
             self.thread.join()
         elif self.MODE == 'threads':
-            self._thread_quit_event.set()
             [t.join() for t in self.thread]
 
 
 __all__ = [
     'Key2Action',
     'statuesQue',
     '_wait_for_quit',
```

### Comparing `mbapy-0.7.3/mbapy.egg-info/SOURCES.txt` & `mbapy-0.7.4/mbapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/mbapy.egg-info/requires.txt` & `mbapy-0.7.4/mbapy.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 PyPDF2
 rispy
 lxml
 crossref_commons
 wget
 pdfplumber
 pyteomics
+pygame
+nicegui
 
 [full]
 aiohttp
 beautifulsoup4
 chardet
 matplotlib
 numpy
@@ -62,25 +64,27 @@
 scikit_posthocs
 pdfminer
 PyPDF2
 rispy
 lxml
 crossref_commons
 cn2an
+ujson
 yaml
 pdfplumber
 Markdown
 imageio
 pillow_heif
 wget
 pyteomics
 opencv-python
 moviepy
 pygame
 easyocr
+nicegui
 
 [game]
 aiohttp
 beautifulsoup4
 chardet
 matplotlib
 numpy
```

### Comparing `mbapy-0.7.3/requirements.json` & `mbapy-0.7.4/requirements.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9321428571428572%*

 * *Differences: {"'bio'": "{insert: [(3, 'pygame'), (4, 'nicegui')]}",*

 * * "'full'": "{insert: [(1, 'ujson'), (13, 'nicegui')]}"}*

```diff
@@ -1,26 +1,30 @@
 {
     "bio": [
         "wget",
         "pdfplumber",
-        "pyteomics"
+        "pyteomics",
+        "pygame",
+        "nicegui"
     ],
     "full": [
         "cn2an",
+        "ujson",
         "yaml",
         "pdfplumber",
         "Markdown",
         "imageio",
         "pillow_heif",
         "wget",
         "pyteomics",
         "opencv-python",
         "moviepy",
         "pygame",
-        "easyocr"
+        "easyocr",
+        "nicegui"
     ],
     "game": [
         "pygame",
         "opencv-python"
     ],
     "std": [
         "aiohttp",
```

### Comparing `mbapy-0.7.3/setup.py` & `mbapy-0.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-04-25 23:18:02
+LastEditTime: 2024-05-10 21:06:14
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 thanks to https://github.com/gaogaotiantian/viztracer/blob/master/setup.py
 """
@@ -104,8 +104,8 @@
         'full': requirements['std'] + requirements['full'],
         },
 )
 
 # pip install .
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.7.3.tar.gz
+# twine upload dist/mbapy-0.7.4.tar.gz
```

### Comparing `mbapy-0.7.3/test/test_base.py` & `mbapy-0.7.4/test/test_base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/test/test_game.py` & `mbapy-0.7.4/test/test_game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.3/test/test_web.py` & `mbapy-0.7.4/test/test_web.py`

 * *Files identical despite different names*

