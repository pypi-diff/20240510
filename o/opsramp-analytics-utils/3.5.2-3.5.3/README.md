# Comparing `tmp/opsramp-analytics-utils-3.5.2.tar.gz` & `tmp/opsramp-analytics-utils-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.5.2.tar", last modified: Wed May  8 09:02:44 2024, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.5.3.tar", last modified: Fri May 10 07:33:53 2024, max compression
```

## Comparing `opsramp-analytics-utils-3.5.2.tar` & `opsramp-analytics-utils-3.5.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.254931 opsramp-analytics-utils-3.5.2/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/LICENSE
--rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/MANIFEST.in
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-08 09:02:44.254803 opsramp-analytics-utils-3.5.2/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/README.md
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.246716 opsramp-analytics-utils-3.5.2/analytics_sdk/
--rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/__init__.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.248934 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.js
--rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.252507 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.253022 opsramp-analytics-utils-3.5.2/analytics_sdk/api/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17480 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_task.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/thread_process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17467 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/components.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/constants.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-03-08 08:03:00.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/oap_dash.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.253393 opsramp-analytics-utils-3.5.2/analytics_sdk/process/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/process/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/process/process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/process/querybuilder.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.253955 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    35159 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/excel.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17745 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/excel_writer.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/pdf.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    45289 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/utilities.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.254604 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1737 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      148 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/requires.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/top_level.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      162 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/requires-install.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-05-08 09:02:44.254985 opsramp-analytics-utils-3.5.2/setup.cfg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/setup.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.552238 opsramp-analytics-utils-3.5.3/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/LICENSE
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/MANIFEST.in
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-10 07:33:53.552087 opsramp-analytics-utils-3.5.3/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/README.md
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.537131 opsramp-analytics-utils-3.5.3/analytics_sdk/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/__init__.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.540393 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/main.js
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.548495 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.549352 opsramp-analytics-utils-3.5.3/analytics_sdk/api/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/api/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17480 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/api/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/api/api_task.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/api/thread_process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17467 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/components.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/constants.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-05-08 11:52:29.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/oap_dash.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.550001 opsramp-analytics-utils-3.5.3/analytics_sdk/process/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/process/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/process/process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/process/querybuilder.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.551159 opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    35159 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/excel.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17745 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/excel_writer.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/pdf.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    45775 2024-05-10 07:26:49.000000 opsramp-analytics-utils-3.5.3/analytics_sdk/utilities.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:33:53.551864 opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-10 07:33:53.000000 opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1737 2024-05-10 07:33:53.000000 opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-05-10 07:33:53.000000 opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      148 2024-05-10 07:33:53.000000 opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/requires.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-05-10 07:33:53.000000 opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      162 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.3/requires-install.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-05-10 07:33:53.552287 opsramp-analytics-utils-3.5.3/setup.cfg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-05-10 07:30:03.000000 opsramp-analytics-utils-3.5.3/setup.py
```

### Comparing `opsramp-analytics-utils-3.5.2/LICENSE` & `opsramp-analytics-utils-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/PKG-INFO` & `opsramp-analytics-utils-3.5.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.2
+Version: 3.5.3
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.2/README.md` & `opsramp-analytics-utils-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.5.3/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_client.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/api/api_client.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_task.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/api/api_task.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/api/thread_process.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/api/thread_process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/api_client.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/components.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/excel.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/excel_writer.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/excel_writer.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.5.3/analytics_sdk/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from flask.wrappers import Response
 
 import boto3
 import botocore
 from botocore.exceptions import NoCredentialsError
 import flask
 import requests
-
+from flask import request
 from .constants import DATETIME_FORMAT
 logger = logging.getLogger(__name__)
 
 BASE_API_URL = os.getenv('DATA_API_BASE_URL', '')
 API_RETRY = int(os.getenv('API_RETRY', 3))
 API_KEY = os.getenv('API_KEY')
 API_SECRET = os.getenv('API_SECRET')
@@ -474,14 +474,24 @@
     response.headers['Content-Security-Policy'] = "script-src: 'self' 'unsafe-inline' https://www.google.com"
     response.headers['Strict-Transport-Security'] = "max-age=31536000 ; includeSubDomains;preload;"
     response.headers['X-Content-Type-Options'] = 'nosniff'
     response.headers['X-Xss-Protection'] = "1;mode=block"
     return response
 
 
+# Cache Control Mechanism
+def add_cache_control(response):
+    # Check if the requested URL matches the _dash-component-suites route
+    path = request.path
+    if "/opsramp-analytics-utils/" in path or path.endswith("/_dash-layout") or path.endswith("/_dash-dependencies"):
+        # Add Cache-Control header to the response for browser caching
+        response.headers['Cache-Control'] = 'public, max-age=31536000'  # Cache for 365 days
+    return response
+
+
 def update_status_url(analysisRunId, tenantId, genStime, genEtime, status=None):
 
     url = BASE_API_URL + f'/reporting/api/v3/tenants/{tenantId}/runs/{analysisRunId}'
     data={
             "status" : status,
             "runDurStartDate" : genStime,
             "runDurEndDate" : genEtime
```

### Comparing `opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.2
+Version: 3.5.3
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.5.3/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.2/setup.py` & `opsramp-analytics-utils-3.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.5.2",
+    version="3.5.3",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     # url="https://github.com/opsramp/analytics-sdk",
```

