# Comparing `tmp/geocif-0.1.21.tar.gz` & `tmp/geocif-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.1.21.tar", last modified: Fri May 10 00:53:54 2024, max compression
+gzip compressed data, was "geocif-0.1.22.tar", last modified: Fri May 10 00:58:51 2024, max compression
```

## Comparing `geocif-0.1.21.tar` & `geocif-0.1.22.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.186391 geocif-0.1.21/
--rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.21/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.21/MANIFEST.in
--rw-rw-rw-   0        0        0     2566 2024-05-10 00:53:54.185383 geocif-0.1.21/PKG-INFO
--rw-rw-rw-   0        0        0      589 2024-05-10 00:49:32.000000 geocif-0.1.21/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.030583 geocif-0.1.21/geocif/
--rw-rw-rw-   0        0        0      148 2024-05-09 17:33:59.000000 geocif-0.1.21/geocif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.110484 geocif-0.1.21/geocif/agmet/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.21/geocif/agmet/__init__.py
--rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.21/geocif/agmet/geoagmet.py
--rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.21/geocif/agmet/plot.py
--rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.21/geocif/agmet/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.130966 geocif-0.1.21/geocif/backup/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.21/geocif/backup/__init__.py
--rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.21/geocif/backup/constants.py
--rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.21/geocif/backup/features.py
--rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.21/geocif/backup/geo.py
--rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.21/geocif/backup/geocif.py
--rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.21/geocif/backup/metadata.py
--rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.21/geocif/backup/models.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.139982 geocif-0.1.21/geocif/cei/
--rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.21/geocif/cei/__init__.py
--rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.21/geocif/cei/definitions.py
--rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.21/geocif/cei/indices.py
--rw-rw-rw-   0        0        0    40731 2024-05-10 00:53:39.000000 geocif-0.1.21/geocif/geocif.py
--rw-rw-rw-   0        0        0     6426 2024-05-09 19:50:03.000000 geocif-0.1.21/geocif/indices_runner.py
--rw-rw-rw-   0        0        0     1846 2024-05-10 00:43:12.000000 geocif-0.1.21/geocif/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.179278 geocif-0.1.21/geocif/ml/
--rw-rw-rw-   0        0        0        0 2024-05-09 17:32:51.000000 geocif-0.1.21/geocif/ml/__init__.py
--rw-rw-rw-   0        0        0    31393 2024-05-09 15:38:37.000000 geocif-0.1.21/geocif/ml/analysis.py
--rw-rw-rw-   0        0        0    12251 2024-05-09 21:07:36.000000 geocif-0.1.21/geocif/ml/correlations.py
--rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.21/geocif/ml/embedding.py
--rw-rw-rw-   0        0        0    12505 2024-05-09 22:33:28.000000 geocif-0.1.21/geocif/ml/feature_engineering.py
--rw-rw-rw-   0        0        0     6562 2024-05-09 20:18:20.000000 geocif-0.1.21/geocif/ml/feature_selection.py
--rw-rw-rw-   0        0        0    12461 2024-05-09 15:38:37.000000 geocif-0.1.21/geocif/ml/misc.py
--rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.21/geocif/ml/outliers.py
--rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.21/geocif/ml/outlook.py
--rw-rw-rw-   0        0        0     3542 2024-05-09 19:16:41.000000 geocif-0.1.21/geocif/ml/output.py
--rw-rw-rw-   0        0        0     8044 2024-05-09 19:16:41.000000 geocif-0.1.21/geocif/ml/stages.py
--rw-rw-rw-   0        0        0     4961 2024-05-09 19:26:37.000000 geocif-0.1.21/geocif/ml/stats.py
--rw-rw-rw-   0        0        0     9718 2024-05-09 21:02:58.000000 geocif-0.1.21/geocif/ml/trainers.py
--rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.21/geocif/ml/trend.py
--rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.21/geocif/ml/xai.py
--rw-rw-rw-   0        0        0    18972 2024-05-09 19:38:53.000000 geocif-0.1.21/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.100017 geocif-0.1.21/geocif.egg-info/
--rw-rw-rw-   0        0        0     2566 2024-05-10 00:53:53.000000 geocif-0.1.21/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2024-05-10 00:53:53.000000 geocif-0.1.21/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      657 2024-05-10 00:53:53.000000 geocif-0.1.21/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.21/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      656 2024-05-10 00:53:53.000000 geocif-0.1.21/geocif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 00:53:53.000000 geocif-0.1.21/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      656 2024-05-10 00:50:26.000000 geocif-0.1.21/requirements.txt
--rw-rw-rw-   0        0        0      414 2024-05-10 00:53:54.195451 geocif-0.1.21/setup.cfg
--rw-rw-rw-   0        0        0     1620 2024-05-10 00:53:39.000000 geocif-0.1.21/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:53:54.181181 geocif-0.1.21/tests/
--rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.21/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.450466 geocif-0.1.22/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.22/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.22/MANIFEST.in
+-rw-rw-rw-   0        0        0     2566 2024-05-10 00:58:51.449440 geocif-0.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2024-05-10 00:49:32.000000 geocif-0.1.22/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.276234 geocif-0.1.22/geocif/
+-rw-rw-rw-   0        0        0      148 2024-05-09 17:33:59.000000 geocif-0.1.22/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.359741 geocif-0.1.22/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.22/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.22/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.22/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.22/geocif/agmet/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.382483 geocif-0.1.22/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.22/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.22/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.22/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.22/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.22/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.22/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.22/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.392634 geocif-0.1.22/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.22/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.22/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.22/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    40731 2024-05-10 00:53:39.000000 geocif-0.1.22/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6426 2024-05-09 19:50:03.000000 geocif-0.1.22/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     2267 2024-05-10 00:58:39.000000 geocif-0.1.22/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.441425 geocif-0.1.22/geocif/ml/
+-rw-rw-rw-   0        0        0        0 2024-05-09 17:32:51.000000 geocif-0.1.22/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    31393 2024-05-09 15:38:37.000000 geocif-0.1.22/geocif/ml/analysis.py
+-rw-rw-rw-   0        0        0    12251 2024-05-09 21:07:36.000000 geocif-0.1.22/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.22/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    12505 2024-05-09 22:33:28.000000 geocif-0.1.22/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     6562 2024-05-09 20:18:20.000000 geocif-0.1.22/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0    12461 2024-05-09 15:38:37.000000 geocif-0.1.22/geocif/ml/misc.py
+-rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.22/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.22/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3542 2024-05-09 19:16:41.000000 geocif-0.1.22/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     8044 2024-05-09 19:16:41.000000 geocif-0.1.22/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     4961 2024-05-09 19:26:37.000000 geocif-0.1.22/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0     9718 2024-05-09 21:02:58.000000 geocif-0.1.22/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.22/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.22/geocif/ml/xai.py
+-rw-rw-rw-   0        0        0    18531 2024-05-10 00:58:39.000000 geocif-0.1.22/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.346509 geocif-0.1.22/geocif.egg-info/
+-rw-rw-rw-   0        0        0     2566 2024-05-10 00:58:50.000000 geocif-0.1.22/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2024-05-10 00:58:51.000000 geocif-0.1.22/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      657 2024-05-10 00:58:50.000000 geocif-0.1.22/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.22/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      656 2024-05-10 00:58:50.000000 geocif-0.1.22/geocif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 00:58:50.000000 geocif-0.1.22/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      656 2024-05-10 00:50:26.000000 geocif-0.1.22/requirements.txt
+-rw-rw-rw-   0        0        0      414 2024-05-10 00:58:51.458591 geocif-0.1.22/setup.cfg
+-rw-rw-rw-   0        0        0     1620 2024-05-10 00:58:39.000000 geocif-0.1.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:58:51.445425 geocif-0.1.22/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.22/tests/test_geocif.py
```

### Comparing `geocif-0.1.21/LICENSE` & `geocif-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/PKG-INFO` & `geocif-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.21
+Version: 0.1.22
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.21/README.md` & `geocif-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/agmet/geoagmet.py` & `geocif-0.1.22/geocif/agmet/geoagmet.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/agmet/plot.py` & `geocif-0.1.22/geocif/agmet/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/agmet/utils.py` & `geocif-0.1.22/geocif/agmet/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/backup/features.py` & `geocif-0.1.22/geocif/backup/features.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/backup/geo.py` & `geocif-0.1.22/geocif/backup/geo.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/backup/geocif.py` & `geocif-0.1.22/geocif/backup/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/backup/metadata.py` & `geocif-0.1.22/geocif/backup/metadata.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/cei/definitions.py` & `geocif-0.1.22/geocif/cei/definitions.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/cei/indices.py` & `geocif-0.1.22/geocif/cei/indices.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/geocif.py` & `geocif-0.1.22/geocif/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/indices_runner.py` & `geocif-0.1.22/geocif/indices_runner.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/logger.py` & `geocif-0.1.22/geocif/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,36 @@
 import logging
 import os
 from pathlib import Path
 
 import arrow as ar
 import logzero
 
-import utils
+
+def read_config(path_config_file):
+    """
+
+    Args:
+        path_config_file ():
+
+    Returns:
+
+    """
+    from configparser import ConfigParser, ExtendedInterpolation
+
+    parser = ConfigParser(
+        inline_comment_prefixes=(";",), interpolation=ExtendedInterpolation()
+    )
+
+    try:
+        parser.read(path_config_file)
+    except Exception as e:
+        raise IOError(f"Cannot read {path_config_file}: {e}")
+
+    return parser
 
 
 class Logger:
     # adapted from https://gist.github.com/empr/2036153
     # Level	    Numeric value
     # CRITICAL	      50
     # ERROR	          40
@@ -58,15 +79,15 @@
         name_project:
         name_file:
         level:
 
     Returns:
 
     """
-    parser = utils.read_config(path_config_file)
+    parser = read_config(path_config_file)
     dir_log = parser.get("PATHS", "dir_log")
 
     logger = Logger(
         dir_log=dir_log,
         project=name_project,
         file=name_file,
         level=level,
```

### Comparing `geocif-0.1.21/geocif/ml/analysis.py` & `geocif-0.1.22/geocif/ml/analysis.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/correlations.py` & `geocif-0.1.22/geocif/ml/correlations.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/embedding.py` & `geocif-0.1.22/geocif/ml/embedding.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/feature_engineering.py` & `geocif-0.1.22/geocif/ml/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/feature_selection.py` & `geocif-0.1.22/geocif/ml/feature_selection.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/misc.py` & `geocif-0.1.22/geocif/ml/misc.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/outliers.py` & `geocif-0.1.22/geocif/ml/outliers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/outlook.py` & `geocif-0.1.22/geocif/ml/outlook.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/output.py` & `geocif-0.1.22/geocif/ml/output.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/stages.py` & `geocif-0.1.22/geocif/ml/stages.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/stats.py` & `geocif-0.1.22/geocif/ml/stats.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/trainers.py` & `geocif-0.1.22/geocif/ml/trainers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/trend.py` & `geocif-0.1.22/geocif/ml/trend.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/ml/xai.py` & `geocif-0.1.22/geocif/ml/xai.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif/utils.py` & `geocif-0.1.22/geocif/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,37 +96,14 @@
     # Set styles for axes
     plt.rcParams["axes.edgecolor"] = "#333F4B"
     plt.rcParams["axes.linewidth"] = 0.8
     plt.rcParams["xtick.color"] = "#333F4B"
     plt.rcParams["ytick.color"] = "#333F4B"
 
 
-def read_config(path_config_file):
-    """
-
-    Args:
-        path_config_file ():
-
-    Returns:
-
-    """
-    from configparser import ConfigParser, ExtendedInterpolation
-
-    parser = ConfigParser(
-        inline_comment_prefixes=(";",), interpolation=ExtendedInterpolation()
-    )
-
-    try:
-        parser.read(path_config_file)
-    except Exception as e:
-        raise IOError(f"Cannot read {path_config_file}: {e}")
-
-    return parser
-
-
 def delete_empty_dirs(_dir):
     """
     Cleanup by deleting folders which have no files in them. Delete folders which only have empty subdirs
     Args:
         _dir:
 
     Returns:
```

### Comparing `geocif-0.1.21/geocif.egg-info/PKG-INFO` & `geocif-0.1.22/geocif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.21
+Version: 0.1.22
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.21/geocif.egg-info/SOURCES.txt` & `geocif-0.1.22/geocif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif.egg-info/dependency_links.txt` & `geocif-0.1.22/geocif.egg-info/dependency_links.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/geocif.egg-info/requires.txt` & `geocif-0.1.22/geocif.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/requirements.txt` & `geocif-0.1.22/requirements.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.21/setup.py` & `geocif-0.1.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords='geocif',
     name='geocif',
     packages=find_packages(include=['geocif', 'geocif.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://ritviksahajpal.github.io/yield_forecasting/',
-    version='0.1.21',
+    version='0.1.22',
     zip_safe=False,
 )
```

