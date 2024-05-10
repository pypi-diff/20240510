# Comparing `tmp/towbintools-0.1.5.tar.gz` & `tmp/towbintools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towbintools-0.1.5.tar", last modified: Wed Apr 17 14:30:26 2024, max compression
+gzip compressed data, was "towbintools-0.1.6.tar", last modified: Fri May 10 08:02:29 2024, max compression
```

## Comparing `towbintools-0.1.5.tar` & `towbintools-0.1.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.114070 towbintools-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-17 14:30:21.000000 towbintools-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-17 14:30:26.114070 towbintools-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-17 14:30:21.000000 towbintools-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-17 14:30:21.000000 towbintools-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:30:26.114070 towbintools-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/classification/classification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/data_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/data_analysis/growth_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/deep_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/deep_learning/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/architectures/archs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/architectures/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/deep_learning_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/deep_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/foundation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/binary_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/detect_molts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/image_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/image_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/worm_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/zstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/legacy_straightening/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/legacy_straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/legacy_straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/quantification/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/quantification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/quantification/quantification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/segmentation/segmentation_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/straightening/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-10 08:02:24.000000 towbintools-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-10 08:02:29.254521 towbintools-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-10 08:02:24.000000 towbintools-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 08:02:24.000000 towbintools-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:02:29.254521 towbintools-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.246521 towbintools-0.1.6/towbintools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/classification/classification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/data_analysis/growth_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/deep_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/deep_learning/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/architectures/archs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/architectures/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/deep_learning_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/deep_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/foundation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/binary_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/detect_molts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/image_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/image_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/worm_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/zstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/legacy_straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/legacy_straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/legacy_straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/quantification/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/quantification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/quantification/quantification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/segmentation/segmentation_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/top_level.txt
```

### Comparing `towbintools-0.1.5/LICENSE` & `towbintools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/PKG-INFO` & `towbintools-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.5
+Version: 0.1.6
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.5/README.md` & `towbintools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/pyproject.toml` & `towbintools-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "towbintools"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Sacha Psalmon", email="sacha.psalmon@unibe.ch" },
   {name="Boris Gusev", email="boris.gusev@unibe.ch" }
 ]
 maintainers = [
     {name = "Sacha Psalmon", email="sacha.psalmon@unibe.ch"},
 ]
```

### Comparing `towbintools-0.1.5/towbintools/classification/classification_tools.py` & `towbintools-0.1.6/towbintools/classification/classification_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/data_analysis/growth_rate.py` & `towbintools-0.1.6/towbintools/data_analysis/growth_rate.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/deep_learning/architectures/archs.py` & `towbintools-0.1.6/towbintools/deep_learning/architectures/archs.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/deep_learning/architectures/models.py` & `towbintools-0.1.6/towbintools/deep_learning/architectures/models.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/deep_learning/deep_learning_tools.py` & `towbintools-0.1.6/towbintools/deep_learning/deep_learning_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/deep_learning/utils/augmentation.py` & `towbintools-0.1.6/towbintools/deep_learning/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/deep_learning/utils/dataset.py` & `towbintools-0.1.6/towbintools/deep_learning/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/deep_learning/utils/loss.py` & `towbintools-0.1.6/towbintools/deep_learning/utils/loss.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/backbone.py` & `towbintools-0.1.6/towbintools/foundation/backbone.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/binary_image.py` & `towbintools-0.1.6/towbintools/foundation/binary_image.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/detect_molts.py` & `towbintools-0.1.6/towbintools/foundation/detect_molts.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/file_handling.py` & `towbintools-0.1.6/towbintools/foundation/file_handling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-
+import numpy as np
 import pandas as pd
 
 
 def get_all_timepoints_from_dir(
     dir_path: str,
 ) -> list:
     """
@@ -24,25 +24,24 @@
     # Get a sorted list of image paths in the directory.
     images_path = [
         os.path.join(dir_path, x) for x in os.listdir(dir_path) if ~(os.path.isdir(x))
     ]
 
     # Iterate through each image path.
     for image_path in images_path:
-        if image_path.endswith(".tiff"):
-            # Search for the time and point in the image path using the pattern.
-            match = pattern.search(image_path)
-            if match:
-                # Extract the time and point as integers from the matched groups.
-                time = int(match.group(1))
-                point = int(match.group(2))
-                # Add the time, point, and image path to the list as a dictionary.
-                timepoint_list.append(
-                    {"Time": time, "Point": point, "ImagePath": image_path}
-                )
+        # Search for the time and point in the image path using the pattern.
+        match = pattern.search(image_path)
+        if match:
+            # Extract the time and point as integers from the matched groups.
+            time = int(match.group(1))
+            point = int(match.group(2))
+            # Add the time, point, and image path to the list as a dictionary.
+            timepoint_list.append(
+                {"Time": time, "Point": point, "ImagePath": image_path}
+            )
 
     return timepoint_list
 
 
 def fill_empty_timepoints(
     filemap: pd.DataFrame,
 ) -> pd.DataFrame:
@@ -144,11 +143,18 @@
                 )
                 experiment_filemap = experiment_filemap.merge(
                     filemap, on=["Time", "Point"], how="outer"
                 )
     experiment_filemap = experiment_filemap.fillna("")
     return experiment_filemap
 
-
-# def get_directory_filemap(
-#     dir_path: str,
-# ) -> pd.DataFrame:
+def add_dir_to_experiment_filemap(experiment_filemap, dir_path, subdir_name):
+    subdir_filemap = get_dir_filemap(dir_path)
+    subdir_filemap.rename(columns={"ImagePath": subdir_name}, inplace=True)
+    # check if column already exists
+    if subdir_name in experiment_filemap.columns:
+        experiment_filemap.drop(columns=[subdir_name], inplace=True)
+    experiment_filemap = experiment_filemap.merge(
+        subdir_filemap, on=["Time", "Point"], how="left"
+    )
+    experiment_filemap = experiment_filemap.replace(np.nan, "", regex=True)
+    return experiment_filemap
```

### Comparing `towbintools-0.1.5/towbintools/foundation/image_handling.py` & `towbintools-0.1.6/towbintools/foundation/image_handling.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/image_quality.py` & `towbintools-0.1.6/towbintools/foundation/image_quality.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/utils.py` & `towbintools-0.1.6/towbintools/foundation/utils.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/worm_features.py` & `towbintools-0.1.6/towbintools/foundation/worm_features.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/foundation/zstack.py` & `towbintools-0.1.6/towbintools/foundation/zstack.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/legacy_straightening/straightening_tools.py` & `towbintools-0.1.6/towbintools/legacy_straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/quantification/quantification_tools.py` & `towbintools-0.1.6/towbintools/quantification/quantification_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/segmentation/segmentation_tools.py` & `towbintools-0.1.6/towbintools/segmentation/segmentation_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools/straightening/straightening_tools.py` & `towbintools-0.1.6/towbintools/straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.5/towbintools.egg-info/PKG-INFO` & `towbintools-0.1.6/towbintools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.5
+Version: 0.1.6
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.5/towbintools.egg-info/SOURCES.txt` & `towbintools-0.1.6/towbintools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

