# Comparing `tmp/irisml_tasks_yolov9-0.0.3.tar.gz` & `tmp/irisml_tasks_yolov9-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml_tasks_yolov9-0.0.3.tar", last modified: Wed May  8 17:17:53 2024, max compression
+gzip compressed data, was "irisml_tasks_yolov9-0.0.4.tar", last modified: Thu May  9 18:47:58 2024, max compression
```

## Comparing `irisml_tasks_yolov9-0.0.3.tar` & `irisml_tasks_yolov9-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:17:53.461750 irisml_tasks_yolov9-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 17:15:37.000000 irisml_tasks_yolov9-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-08 17:17:53.461750 irisml_tasks_yolov9-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-08 17:15:37.000000 irisml_tasks_yolov9-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:17:53.457750 irisml_tasks_yolov9-0.0.3/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:17:53.457750 irisml_tasks_yolov9-0.0.3/irisml/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:17:53.457750 irisml_tasks_yolov9-0.0.3/irisml/tasks/create_yolov9_detection_model/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 17:15:37.000000 irisml_tasks_yolov9-0.0.3/irisml/tasks/create_yolov9_detection_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-08 17:15:37.000000 irisml_tasks_yolov9-0.0.3/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:17:53.461750 irisml_tasks_yolov9-0.0.3/irisml_tasks_yolov9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-08 17:17:53.000000 irisml_tasks_yolov9-0.0.3/irisml_tasks_yolov9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-08 17:17:53.000000 irisml_tasks_yolov9-0.0.3/irisml_tasks_yolov9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:17:53.000000 irisml_tasks_yolov9-0.0.3/irisml_tasks_yolov9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 17:17:53.000000 irisml_tasks_yolov9-0.0.3/irisml_tasks_yolov9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 17:17:53.000000 irisml_tasks_yolov9-0.0.3/irisml_tasks_yolov9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 17:15:37.000000 irisml_tasks_yolov9-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:17:53.461750 irisml_tasks_yolov9-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:17:53.461750 irisml_tasks_yolov9-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-08 17:15:37.000000 irisml_tasks_yolov9-0.0.3/test/test_create_yolov9_detection_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:58.545874 irisml_tasks_yolov9-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-09 18:47:58.545874 irisml_tasks_yolov9-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:58.537874 irisml_tasks_yolov9-0.0.4/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:58.537874 irisml_tasks_yolov9-0.0.4/irisml/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:58.537874 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:58.541874 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/resources/gelan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/resources/gelanc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/resources/gelane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/resources/yolov9.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/resources/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/resources/yolov9e.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/irisml/tasks/load_yolov9_prediction_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:58.541874 irisml_tasks_yolov9-0.0.4/irisml_tasks_yolov9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-09 18:47:58.000000 irisml_tasks_yolov9-0.0.4/irisml_tasks_yolov9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 18:47:58.000000 irisml_tasks_yolov9-0.0.4/irisml_tasks_yolov9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:47:58.000000 irisml_tasks_yolov9-0.0.4/irisml_tasks_yolov9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 18:47:58.000000 irisml_tasks_yolov9-0.0.4/irisml_tasks_yolov9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 18:47:58.000000 irisml_tasks_yolov9-0.0.4/irisml_tasks_yolov9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:47:58.545874 irisml_tasks_yolov9-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:58.541874 irisml_tasks_yolov9-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/test/test_create_yolov9_detection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-09 18:45:52.000000 irisml_tasks_yolov9-0.0.4/test/test_load_yolov9_prediction_results.py
```

### Comparing `irisml_tasks_yolov9-0.0.3/LICENSE` & `irisml_tasks_yolov9-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.3/PKG-INFO` & `irisml_tasks_yolov9-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-yolov9
-Version: 0.0.3
+Version: 0.0.4
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: irisml
 Requires-Dist: pyyolov9<1
 
 # irisml-tasks-yolov9
```

### Comparing `irisml_tasks_yolov9-0.0.3/README.md` & `irisml_tasks_yolov9-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.3/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py` & `irisml_tasks_yolov9-0.0.4/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.3/irisml_tasks_yolov9.egg-info/PKG-INFO` & `irisml_tasks_yolov9-0.0.4/irisml_tasks_yolov9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-yolov9
-Version: 0.0.3
+Version: 0.0.4
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: irisml
 Requires-Dist: pyyolov9<1
 
 # irisml-tasks-yolov9
```

### Comparing `irisml_tasks_yolov9-0.0.3/test/test_create_yolov9_detection_model.py` & `irisml_tasks_yolov9-0.0.4/test/test_create_yolov9_detection_model.py`

 * *Files identical despite different names*

