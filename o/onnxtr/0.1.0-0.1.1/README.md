# Comparing `tmp/onnxtr-0.1.0.tar.gz` & `tmp/onnxtr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxtr-0.1.0.tar", last modified: Fri May 10 08:45:03 2024, max compression
+gzip compressed data, was "onnxtr-0.1.1.tar", last modified: Fri May 10 09:20:49 2024, max compression
```

## Comparing `onnxtr-0.1.0.tar` & `onnxtr-0.1.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.946223 onnxtr-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 08:44:50.000000 onnxtr-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24626 2024-05-10 08:45:03.946223 onnxtr-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-10 08:44:50.000000 onnxtr-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.930223 onnxtr-0.1.0/onnxtr/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.930223 onnxtr-0.1.0/onnxtr/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/contrib/artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/contrib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.930223 onnxtr-0.1.0/onnxtr/io/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/io/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/io/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/io/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/io/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/io/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/classification/models/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/classification/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/classification/models/mobilenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/classification/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/classification/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/classification/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/classification/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/detection/models/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/models/differentiable_binarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/models/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/models/linknet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/detection/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/postprocessor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.934223 onnxtr-0.1.0/onnxtr/models/detection/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/detection/zoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.938223 onnxtr-0.1.0/onnxtr/models/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.938223 onnxtr-0.1.0/onnxtr/models/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/preprocessor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.938223 onnxtr-0.1.0/onnxtr/models/recognition/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.938223 onnxtr-0.1.0/onnxtr/models/recognition/models/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/models/crnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/models/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/models/parseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/models/sar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/models/vitstr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.938223 onnxtr-0.1.0/onnxtr/models/recognition/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/predictor/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/recognition/zoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.938223 onnxtr-0.1.0/onnxtr/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/transforms/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.942223 onnxtr-0.1.0/onnxtr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/common_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17002 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/multithreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/reconstitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 08:44:50.000000 onnxtr-0.1.0/onnxtr/utils/vocabs.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 08:45:03.000000 onnxtr-0.1.0/onnxtr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:03.942223 onnxtr-0.1.0/onnxtr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24626 2024-05-10 08:45:03.000000 onnxtr-0.1.0/onnxtr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-10 08:45:03.000000 onnxtr-0.1.0/onnxtr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:45:03.000000 onnxtr-0.1.0/onnxtr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 08:45:03.000000 onnxtr-0.1.0/onnxtr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 08:45:03.000000 onnxtr-0.1.0/onnxtr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:45:03.000000 onnxtr-0.1.0/onnxtr.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-10 08:44:50.000000 onnxtr-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:45:03.946223 onnxtr-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-10 08:44:50.000000 onnxtr-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.885275 onnxtr-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 09:20:39.000000 onnxtr-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-10 09:20:49.885275 onnxtr-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-10 09:20:39.000000 onnxtr-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.865275 onnxtr-0.1.1/onnxtr/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.865275 onnxtr-0.1.1/onnxtr/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/contrib/artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/contrib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.869275 onnxtr-0.1.1/onnxtr/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/io/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/io/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/io/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/io/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.869275 onnxtr-0.1.1/onnxtr/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.869275 onnxtr-0.1.1/onnxtr/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.869275 onnxtr-0.1.1/onnxtr/models/classification/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/classification/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/classification/models/mobilenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.869275 onnxtr-0.1.1/onnxtr/models/classification/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/classification/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/classification/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/classification/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.869275 onnxtr-0.1.1/onnxtr/models/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.873275 onnxtr-0.1.1/onnxtr/models/detection/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/models/differentiable_binarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/models/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/models/linknet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.873275 onnxtr-0.1.1/onnxtr/models/detection/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/postprocessor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.873275 onnxtr-0.1.1/onnxtr/models/detection/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/detection/zoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.873275 onnxtr-0.1.1/onnxtr/models/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.873275 onnxtr-0.1.1/onnxtr/models/preprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/preprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/preprocessor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.873275 onnxtr-0.1.1/onnxtr/models/recognition/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.877275 onnxtr-0.1.1/onnxtr/models/recognition/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/models/crnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/models/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/models/parseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/models/sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/models/vitstr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.877275 onnxtr-0.1.1/onnxtr/models/recognition/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/predictor/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/recognition/zoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.877275 onnxtr-0.1.1/onnxtr/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/transforms/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.881275 onnxtr-0.1.1/onnxtr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17002 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/multithreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/reconstitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 09:20:39.000000 onnxtr-0.1.1/onnxtr/utils/vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 09:20:49.000000 onnxtr-0.1.1/onnxtr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:20:49.881275 onnxtr-0.1.1/onnxtr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-10 09:20:49.000000 onnxtr-0.1.1/onnxtr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-10 09:20:49.000000 onnxtr-0.1.1/onnxtr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:20:49.000000 onnxtr-0.1.1/onnxtr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 09:20:49.000000 onnxtr-0.1.1/onnxtr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 09:20:49.000000 onnxtr-0.1.1/onnxtr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:20:49.000000 onnxtr-0.1.1/onnxtr.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-10 09:20:39.000000 onnxtr-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:20:49.885275 onnxtr-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-10 09:20:39.000000 onnxtr-0.1.1/setup.py
```

### Comparing `onnxtr-0.1.0/LICENSE` & `onnxtr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/PKG-INFO` & `onnxtr-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxtr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Onnx Text Recognition (OnnxTR): docTR Onnx-Wrapper for high-performance OCR on documents.
 Author-email: Felix Dittrich <felixdittrich92@gmail.com>
 Maintainer: Felix Dittrich
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,25 +224,26 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: <4,>=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2.0.0,>=1.16.0
 Requires-Dist: scipy<2.0.0,>=1.4.0
 Requires-Dist: onnx<2.0.0,>=1.12.0
-Requires-Dist: onnxruntime>=1.11.0
 Requires-Dist: opencv-python<5.0.0,>=4.5.0
 Requires-Dist: pypdfium2<5.0.0,>=4.0.0
 Requires-Dist: pyclipper<2.0.0,>=1.2.0
 Requires-Dist: shapely<3.0.0,>=1.6.0
 Requires-Dist: rapidfuzz<4.0.0,>=3.0.0
 Requires-Dist: langdetect<2.0.0,>=1.0.9
 Requires-Dist: Pillow>=9.2.0
 Requires-Dist: defusedxml>=0.7.0
 Requires-Dist: anyascii>=0.3.2
 Requires-Dist: tqdm>=4.30.0
+Provides-Extra: cpu
+Requires-Dist: onnxruntime>=1.11.0; extra == "cpu"
 Provides-Extra: gpu
 Requires-Dist: onnxruntime-gpu>=1.11.0; extra == "gpu"
 Provides-Extra: html
 Requires-Dist: weasyprint>=55.0; extra == "html"
 Provides-Extra: viz
 Requires-Dist: matplotlib>=3.1.0; extra == "viz"
 Requires-Dist: mplcursors>=0.3; extra == "viz"
@@ -251,14 +252,15 @@
 Requires-Dist: coverage[toml]>=4.5.4; extra == "testing"
 Requires-Dist: requests>=2.20.0; extra == "testing"
 Provides-Extra: quality
 Requires-Dist: ruff>=0.1.5; extra == "quality"
 Requires-Dist: mypy>=0.812; extra == "quality"
 Requires-Dist: pre-commit>=2.17.0; extra == "quality"
 Provides-Extra: dev
+Requires-Dist: onnxruntime>=1.11.0; extra == "dev"
 Requires-Dist: weasyprint>=55.0; extra == "dev"
 Requires-Dist: matplotlib>=3.1.0; extra == "dev"
 Requires-Dist: mplcursors>=0.3; extra == "dev"
 Requires-Dist: pytest>=5.3.2; extra == "dev"
 Requires-Dist: coverage[toml]>=4.5.4; extra == "dev"
 Requires-Dist: requests>=2.20.0; extra == "dev"
 Requires-Dist: ruff>=0.1.5; extra == "dev"
@@ -297,23 +299,23 @@
 ### Latest release
 
 You can then install the latest release of the package using [pypi](https://pypi.org/project/OnnxTR/) as follows:
 
 **NOTE:** For GPU support please take a look at: [ONNX Runtime](https://onnxruntime.ai/getting-started). Currently supported execution providers by default are: CPU, CUDA
 
 ```shell
-pip install OnnxTR
+pip install onnxtr[cpu]
 # with gpu support
-pip install "OnnxTR[gpu]"
+pip install "onnxtr[gpu]"
 # with HTML support
-pip install "OnnxTR[html]"
+pip install "onnxtr[html]"
 # with support for visualization
-pip install "OnnxTR[viz]"
+pip install "onnxtr[viz]"
 # with support for all dependencies
-pip install "OnnxTR[html, gpu, viz]"
+pip install "onnxtr[html, gpu, viz]"
 ```
 
 ### Reading files
 
 Documents can be interpreted from PDF / Images / Webpages / Multiple page images using the following code snippet:
 
 ```python
```

### Comparing `onnxtr-0.1.0/README.md` & `onnxtr-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 ### Latest release
 
 You can then install the latest release of the package using [pypi](https://pypi.org/project/OnnxTR/) as follows:
 
 **NOTE:** For GPU support please take a look at: [ONNX Runtime](https://onnxruntime.ai/getting-started). Currently supported execution providers by default are: CPU, CUDA
 
 ```shell
-pip install OnnxTR
+pip install onnxtr[cpu]
 # with gpu support
-pip install "OnnxTR[gpu]"
+pip install "onnxtr[gpu]"
 # with HTML support
-pip install "OnnxTR[html]"
+pip install "onnxtr[html]"
 # with support for visualization
-pip install "OnnxTR[viz]"
+pip install "onnxtr[viz]"
 # with support for all dependencies
-pip install "OnnxTR[html, gpu, viz]"
+pip install "onnxtr[html, gpu, viz]"
 ```
 
 ### Reading files
 
 Documents can be interpreted from PDF / Images / Webpages / Multiple page images using the following code snippet:
 
 ```python
```

### Comparing `onnxtr-0.1.0/onnxtr/contrib/artefacts.py` & `onnxtr-0.1.1/onnxtr/contrib/artefacts.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/contrib/base.py` & `onnxtr-0.1.1/onnxtr/contrib/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/file_utils.py` & `onnxtr-0.1.1/onnxtr/file_utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/io/elements.py` & `onnxtr-0.1.1/onnxtr/io/elements.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/io/html.py` & `onnxtr-0.1.1/onnxtr/io/html.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/io/image.py` & `onnxtr-0.1.1/onnxtr/io/image.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/io/pdf.py` & `onnxtr-0.1.1/onnxtr/io/pdf.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/io/reader.py` & `onnxtr-0.1.1/onnxtr/io/reader.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/_utils.py` & `onnxtr-0.1.1/onnxtr/models/_utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/builder.py` & `onnxtr-0.1.1/onnxtr/models/builder.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/classification/models/mobilenet.py` & `onnxtr-0.1.1/onnxtr/models/classification/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/classification/predictor/base.py` & `onnxtr-0.1.1/onnxtr/models/classification/predictor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/classification/zoo.py` & `onnxtr-0.1.1/onnxtr/models/classification/zoo.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/detection/core.py` & `onnxtr-0.1.1/onnxtr/models/detection/core.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/detection/models/differentiable_binarization.py` & `onnxtr-0.1.1/onnxtr/models/detection/models/differentiable_binarization.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/detection/models/fast.py` & `onnxtr-0.1.1/onnxtr/models/detection/models/fast.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/detection/models/linknet.py` & `onnxtr-0.1.1/onnxtr/models/detection/models/linknet.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/detection/postprocessor/base.py` & `onnxtr-0.1.1/onnxtr/models/detection/postprocessor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/detection/predictor/base.py` & `onnxtr-0.1.1/onnxtr/models/detection/predictor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/detection/zoo.py` & `onnxtr-0.1.1/onnxtr/models/detection/zoo.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/engine.py` & `onnxtr-0.1.1/onnxtr/models/engine.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/predictor/base.py` & `onnxtr-0.1.1/onnxtr/models/predictor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/predictor/predictor.py` & `onnxtr-0.1.1/onnxtr/models/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/preprocessor/base.py` & `onnxtr-0.1.1/onnxtr/models/preprocessor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/core.py` & `onnxtr-0.1.1/onnxtr/models/recognition/core.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/models/crnn.py` & `onnxtr-0.1.1/onnxtr/models/recognition/models/crnn.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/models/master.py` & `onnxtr-0.1.1/onnxtr/models/recognition/models/master.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/models/parseq.py` & `onnxtr-0.1.1/onnxtr/models/recognition/models/parseq.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/models/sar.py` & `onnxtr-0.1.1/onnxtr/models/recognition/models/sar.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/models/vitstr.py` & `onnxtr-0.1.1/onnxtr/models/recognition/models/vitstr.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/predictor/_utils.py` & `onnxtr-0.1.1/onnxtr/models/recognition/predictor/_utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/predictor/base.py` & `onnxtr-0.1.1/onnxtr/models/recognition/predictor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/utils.py` & `onnxtr-0.1.1/onnxtr/models/recognition/utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/recognition/zoo.py` & `onnxtr-0.1.1/onnxtr/models/recognition/zoo.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/models/zoo.py` & `onnxtr-0.1.1/onnxtr/models/zoo.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/transforms/base.py` & `onnxtr-0.1.1/onnxtr/transforms/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/common_types.py` & `onnxtr-0.1.1/onnxtr/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/data.py` & `onnxtr-0.1.1/onnxtr/utils/data.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/fonts.py` & `onnxtr-0.1.1/onnxtr/utils/fonts.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/geometry.py` & `onnxtr-0.1.1/onnxtr/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/multithreading.py` & `onnxtr-0.1.1/onnxtr/utils/multithreading.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/reconstitution.py` & `onnxtr-0.1.1/onnxtr/utils/reconstitution.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/repr.py` & `onnxtr-0.1.1/onnxtr/utils/repr.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/visualization.py` & `onnxtr-0.1.1/onnxtr/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr/utils/vocabs.py` & `onnxtr-0.1.1/onnxtr/utils/vocabs.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr.egg-info/PKG-INFO` & `onnxtr-0.1.1/onnxtr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxtr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Onnx Text Recognition (OnnxTR): docTR Onnx-Wrapper for high-performance OCR on documents.
 Author-email: Felix Dittrich <felixdittrich92@gmail.com>
 Maintainer: Felix Dittrich
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,25 +224,26 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: <4,>=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2.0.0,>=1.16.0
 Requires-Dist: scipy<2.0.0,>=1.4.0
 Requires-Dist: onnx<2.0.0,>=1.12.0
-Requires-Dist: onnxruntime>=1.11.0
 Requires-Dist: opencv-python<5.0.0,>=4.5.0
 Requires-Dist: pypdfium2<5.0.0,>=4.0.0
 Requires-Dist: pyclipper<2.0.0,>=1.2.0
 Requires-Dist: shapely<3.0.0,>=1.6.0
 Requires-Dist: rapidfuzz<4.0.0,>=3.0.0
 Requires-Dist: langdetect<2.0.0,>=1.0.9
 Requires-Dist: Pillow>=9.2.0
 Requires-Dist: defusedxml>=0.7.0
 Requires-Dist: anyascii>=0.3.2
 Requires-Dist: tqdm>=4.30.0
+Provides-Extra: cpu
+Requires-Dist: onnxruntime>=1.11.0; extra == "cpu"
 Provides-Extra: gpu
 Requires-Dist: onnxruntime-gpu>=1.11.0; extra == "gpu"
 Provides-Extra: html
 Requires-Dist: weasyprint>=55.0; extra == "html"
 Provides-Extra: viz
 Requires-Dist: matplotlib>=3.1.0; extra == "viz"
 Requires-Dist: mplcursors>=0.3; extra == "viz"
@@ -251,14 +252,15 @@
 Requires-Dist: coverage[toml]>=4.5.4; extra == "testing"
 Requires-Dist: requests>=2.20.0; extra == "testing"
 Provides-Extra: quality
 Requires-Dist: ruff>=0.1.5; extra == "quality"
 Requires-Dist: mypy>=0.812; extra == "quality"
 Requires-Dist: pre-commit>=2.17.0; extra == "quality"
 Provides-Extra: dev
+Requires-Dist: onnxruntime>=1.11.0; extra == "dev"
 Requires-Dist: weasyprint>=55.0; extra == "dev"
 Requires-Dist: matplotlib>=3.1.0; extra == "dev"
 Requires-Dist: mplcursors>=0.3; extra == "dev"
 Requires-Dist: pytest>=5.3.2; extra == "dev"
 Requires-Dist: coverage[toml]>=4.5.4; extra == "dev"
 Requires-Dist: requests>=2.20.0; extra == "dev"
 Requires-Dist: ruff>=0.1.5; extra == "dev"
@@ -297,23 +299,23 @@
 ### Latest release
 
 You can then install the latest release of the package using [pypi](https://pypi.org/project/OnnxTR/) as follows:
 
 **NOTE:** For GPU support please take a look at: [ONNX Runtime](https://onnxruntime.ai/getting-started). Currently supported execution providers by default are: CPU, CUDA
 
 ```shell
-pip install OnnxTR
+pip install onnxtr[cpu]
 # with gpu support
-pip install "OnnxTR[gpu]"
+pip install "onnxtr[gpu]"
 # with HTML support
-pip install "OnnxTR[html]"
+pip install "onnxtr[html]"
 # with support for visualization
-pip install "OnnxTR[viz]"
+pip install "onnxtr[viz]"
 # with support for all dependencies
-pip install "OnnxTR[html, gpu, viz]"
+pip install "onnxtr[html, gpu, viz]"
 ```
 
 ### Reading files
 
 Documents can be interpreted from PDF / Images / Webpages / Multiple page images using the following code snippet:
 
 ```python
```

### Comparing `onnxtr-0.1.0/onnxtr.egg-info/SOURCES.txt` & `onnxtr-0.1.1/onnxtr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.0/onnxtr.egg-info/requires.txt` & `onnxtr-0.1.1/onnxtr.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 numpy<2.0.0,>=1.16.0
 scipy<2.0.0,>=1.4.0
 onnx<2.0.0,>=1.12.0
-onnxruntime>=1.11.0
 opencv-python<5.0.0,>=4.5.0
 pypdfium2<5.0.0,>=4.0.0
 pyclipper<2.0.0,>=1.2.0
 shapely<3.0.0,>=1.6.0
 rapidfuzz<4.0.0,>=3.0.0
 langdetect<2.0.0,>=1.0.9
 Pillow>=9.2.0
 defusedxml>=0.7.0
 anyascii>=0.3.2
 tqdm>=4.30.0
 
+[cpu]
+onnxruntime>=1.11.0
+
 [dev]
+onnxruntime>=1.11.0
 weasyprint>=55.0
 matplotlib>=3.1.0
 mplcursors>=0.3
 pytest>=5.3.2
 coverage[toml]>=4.5.4
 requests>=2.20.0
 ruff>=0.1.5
```

### Comparing `onnxtr-0.1.0/pyproject.toml` & `onnxtr-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,30 @@
 dynamic = ["version"]
 dependencies = [
     # For proper typing, mypy needs numpy>=1.20.0 (cf. https://github.com/numpy/numpy/pull/16515)
     # Additional typing support is brought by numpy>=1.22.4, but core build sticks to >=1.16.0
     "numpy>=1.16.0,<2.0.0",
     "scipy>=1.4.0,<2.0.0",
     "onnx>=1.12.0,<2.0.0",
-    "onnxruntime>=1.11.0",
     "opencv-python>=4.5.0,<5.0.0",
     "pypdfium2>=4.0.0,<5.0.0",
     "pyclipper>=1.2.0,<2.0.0",
     "shapely>=1.6.0,<3.0.0",
     "rapidfuzz>=3.0.0,<4.0.0",
     "langdetect>=1.0.9,<2.0.0",
     "Pillow>=9.2.0",
     "defusedxml>=0.7.0",
     "anyascii>=0.3.2",
     "tqdm>=4.30.0",
 ]
 
 [project.optional-dependencies]
+cpu = [
+    "onnxruntime>=1.11.0",
+]
 gpu = [
     "onnxruntime-gpu>=1.11.0",
 ]
 html = [
     "weasyprint>=55.0",
 ]
 viz = [
@@ -65,14 +67,16 @@
 ]
 quality = [
     "ruff>=0.1.5",
     "mypy>=0.812",
     "pre-commit>=2.17.0",
 ]
 dev = [
+    # Runtime
+    "onnxruntime>=1.11.0",
     # HTML
     "weasyprint>=55.0",
     # Visualization
     "matplotlib>=3.1.0",
     "mplcursors>=0.3",
     # Testing
     "pytest>=5.3.2",
```

### Comparing `onnxtr-0.1.0/setup.py` & `onnxtr-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 from pathlib import Path
 
 from setuptools import setup
 
 PKG_NAME = "onnxtr"
-VERSION = os.getenv("BUILD_VERSION", "0.1.0a0")
+VERSION = os.getenv("BUILD_VERSION", "0.1.1a0")
 
 
 if __name__ == "__main__":
     print(f"Building wheel {PKG_NAME}-{VERSION}")
 
     # Dynamically set the __version__ attribute
     cwd = Path(__file__).parent.absolute()
```

