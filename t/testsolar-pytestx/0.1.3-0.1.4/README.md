# Comparing `tmp/testsolar-pytestx-0.1.3.tar.gz` & `tmp/testsolar-pytestx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-pytestx-0.1.3.tar", last modified: Mon Apr 29 08:40:23 2024, max compression
+gzip compressed data, was "testsolar-pytestx-0.1.4.tar", last modified: Fri May 10 02:06:31 2024, max compression
```

## Comparing `testsolar-pytestx-0.1.3.tar` & `testsolar-pytestx-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:23.036992 testsolar-pytestx-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 08:40:23.036992 testsolar-pytestx-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:40:23.036992 testsolar-pytestx-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:23.032992 testsolar-pytestx-0.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:23.032992 testsolar-pytestx-0.1.3/src/testsolar_pytestx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/case_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:23.032992 testsolar-pytestx-0.1.3/src/testsolar_pytestx/extend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/extend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/extend/allure_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:23.032992 testsolar-pytestx-0.1.3/src/testsolar_pytestx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 08:40:23.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-29 08:40:23.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:40:23.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 08:40:23.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 08:40:23.000000 testsolar-pytestx-0.1.3/src/testsolar_pytestx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:40:23.032992 testsolar-pytestx-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-29 08:40:03.000000 testsolar-pytestx-0.1.3/tests/test_run_allure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:31.768115 testsolar-pytestx-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-10 02:06:31.768115 testsolar-pytestx-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:06:31.768115 testsolar-pytestx-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:31.764115 testsolar-pytestx-0.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:31.764115 testsolar-pytestx-0.1.4/src/testsolar_pytestx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/case_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:31.764115 testsolar-pytestx-0.1.4/src/testsolar_pytestx/extend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/extend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/extend/allure_extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:31.764115 testsolar-pytestx-0.1.4/src/testsolar_pytestx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-10 02:06:31.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 02:06:31.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:06:31.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 02:06:31.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 02:06:31.000000 testsolar-pytestx-0.1.4/src/testsolar_pytestx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:06:31.768115 testsolar-pytestx-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-10 02:06:12.000000 testsolar-pytestx-0.1.4/tests/test_run_allure.py
```

### Comparing `testsolar-pytestx-0.1.3/src/load.py` & `testsolar-pytestx-0.1.4/src/load.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/run.py` & `testsolar-pytestx-0.1.4/src/run.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx/case_log.py` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx/case_log.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx/collector.py` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx/collector.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx/converter.py` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx/converter.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx/executor.py` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx/executor.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx/extend/allure_extend.py` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx/extend/allure_extend.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx/filter.py` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx/filter.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx/parser.py` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx/parser.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/src/testsolar_pytestx.egg-info/SOURCES.txt` & `testsolar-pytestx-0.1.4/src/testsolar_pytestx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/tests/test_collector.py` & `testsolar-pytestx-0.1.4/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/tests/test_converter.py` & `testsolar-pytestx-0.1.4/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/tests/test_executor.py` & `testsolar-pytestx-0.1.4/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/tests/test_load.py` & `testsolar-pytestx-0.1.4/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/tests/test_run.py` & `testsolar-pytestx-0.1.4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `testsolar-pytestx-0.1.3/tests/test_run_allure.py` & `testsolar-pytestx-0.1.4/tests/test_run_allure.py`

 * *Files identical despite different names*

