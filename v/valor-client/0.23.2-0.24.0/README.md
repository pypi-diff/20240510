# Comparing `tmp/valor_client-0.23.2.tar.gz` & `tmp/valor_client-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.23.2.tar", last modified: Wed May  8 20:34:21 2024, max compression
+gzip compressed data, was "valor_client-0.24.0.tar", last modified: Thu May  9 22:43:42 2024, max compression
```

## Comparing `valor_client-0.23.2.tar` & `valor_client-0.24.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-08 20:34:17.000000 valor_client-0.23.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-08 20:34:21.736180 valor_client-0.23.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 20:34:17.000000 valor_client-0.23.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:34:21.736180 valor_client-0.23.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-08 20:34:17.000000 valor_client-0.23.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29488 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54922 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.013657 valor_client-0.24.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 22:43:37.000000 valor_client-0.24.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-09 22:43:42.013657 valor_client-0.24.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 22:43:37.000000 valor_client-0.24.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:43:42.013657 valor_client-0.24.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-09 22:43:37.000000 valor_client-0.24.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29488 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54922 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.013657 valor_client-0.24.0/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-09 22:43:42.000000 valor_client-0.24.0/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.23.2/LICENSE` & `valor_client-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/PKG-INFO` & `valor_client-0.24.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.23.2
+Version: 0.24.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.23.2/pyproject.toml` & `valor_client-0.24.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/conftest.py` & `valor_client-0.24.0/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/coretypes/test_core.py` & `valor_client-0.24.0/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.24.0/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/coretypes/test_filtering.py` & `valor_client-0.24.0/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/schemas/test_filters.py` & `valor_client-0.24.0/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/schemas/test_geojson.py` & `valor_client-0.24.0/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/schemas/test_label.py` & `valor_client-0.24.0/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.24.0/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.24.0/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.24.0/unit-tests/symbolic/collections/test_structures.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/symbolic/test_operators.py` & `valor_client-0.24.0/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.24.0/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.24.0/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/test_client.py` & `valor_client-0.24.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/unit-tests/test_viz.py` & `valor_client-0.24.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/__init__.py` & `valor_client-0.24.0/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/client.py` & `valor_client-0.24.0/valor/client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/coretypes.py` & `valor_client-0.24.0/valor/coretypes.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/enums.py` & `valor_client-0.24.0/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/exceptions.py` & `valor_client-0.24.0/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/metatypes.py` & `valor_client-0.24.0/valor/metatypes.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/schemas/__init__.py` & `valor_client-0.24.0/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/schemas/evaluation.py` & `valor_client-0.24.0/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/schemas/filters.py` & `valor_client-0.24.0/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/schemas/symbolic/collections.py` & `valor_client-0.24.0/valor/schemas/symbolic/collections.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/schemas/symbolic/operators.py` & `valor_client-0.24.0/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/schemas/symbolic/types.py` & `valor_client-0.24.0/valor/schemas/symbolic/types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/type_checks.py` & `valor_client-0.24.0/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor/viz.py` & `valor_client-0.24.0/valor/viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.2/valor_client.egg-info/PKG-INFO` & `valor_client-0.24.0/valor_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.23.2
+Version: 0.24.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.23.2/valor_client.egg-info/SOURCES.txt` & `valor_client-0.24.0/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

