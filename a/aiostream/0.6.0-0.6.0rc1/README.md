# Comparing `tmp/aiostream-0.6.0.tar.gz` & `tmp/aiostream-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiostream-0.6.0.tar", last modified: Fri May 10 10:43:40 2024, max compression
+gzip compressed data, was "aiostream-0.6.0rc1.tar", last modified: Fri May 10 10:30:26 2024, max compression
```

## Comparing `aiostream-0.6.0.tar` & `aiostream-0.6.0rc1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:43:40.305966 aiostream-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-10 10:43:36.000000 aiostream-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    50733 2024-05-10 10:43:40.305966 aiostream-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-10 10:43:36.000000 aiostream-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:43:40.301966 aiostream-0.6.0/aiostream/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/aiter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24871 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:43:40.301966 aiostream-0.6.0/aiostream/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/stream/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-10 10:43:36.000000 aiostream-0.6.0/aiostream/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:43:40.305966 aiostream-0.6.0/aiostream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50733 2024-05-10 10:43:40.000000 aiostream-0.6.0/aiostream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 10:43:40.000000 aiostream-0.6.0/aiostream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:43:40.000000 aiostream-0.6.0/aiostream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 10:43:40.000000 aiostream-0.6.0/aiostream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 10:43:40.000000 aiostream-0.6.0/aiostream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-10 10:43:36.000000 aiostream-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:43:40.305966 aiostream-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:43:40.305966 aiostream-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_aiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_task_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-10 10:43:36.000000 aiostream-0.6.0/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.068953 aiostream-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50736 2024-05-10 10:30:26.068953 aiostream-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.060953 aiostream-0.6.0rc1/aiostream/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/aiter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24871 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.064953 aiostream-0.6.0rc1/aiostream/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.064953 aiostream-0.6.0rc1/aiostream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50736 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:30:26.068953 aiostream-0.6.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.064953 aiostream-0.6.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_aiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_task_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_transform.py
```

### Comparing `aiostream-0.6.0/LICENSE` & `aiostream-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/PKG-INFO` & `aiostream-0.6.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostream
-Version: 0.6.0
+Version: 0.6.0rc1
 Summary: Generator-based operators for asynchronous iteration
 Author-email: Vincent Michel <vxgmichel@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `aiostream-0.6.0/README.rst` & `aiostream-0.6.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/__init__.py` & `aiostream-0.6.0rc1/aiostream/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - test_utils: utilities for testing stream operators (require pytest)
 """
 
 from . import stream, pipe
 from .aiter_utils import async_, await_
 from .core import StreamEmpty, operator, pipable_operator, streamcontext
 
-__version__ = "0.6.0"
+__version__ = "0.6.0rc1"
 
 __all__ = [
     "stream",
     "pipe",
     "async_",
     "await_",
     "operator",
```

### Comparing `aiostream-0.6.0/aiostream/aiter_utils.py` & `aiostream-0.6.0rc1/aiostream/aiter_utils.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/core.py` & `aiostream-0.6.0rc1/aiostream/core.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/manager.py` & `aiostream-0.6.0rc1/aiostream/manager.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/pipe.py` & `aiostream-0.6.0rc1/aiostream/pipe.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/advanced.py` & `aiostream-0.6.0rc1/aiostream/stream/advanced.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/aggregate.py` & `aiostream-0.6.0rc1/aiostream/stream/aggregate.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/combine.py` & `aiostream-0.6.0rc1/aiostream/stream/combine.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/create.py` & `aiostream-0.6.0rc1/aiostream/stream/create.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/misc.py` & `aiostream-0.6.0rc1/aiostream/stream/misc.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/select.py` & `aiostream-0.6.0rc1/aiostream/stream/select.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/time.py` & `aiostream-0.6.0rc1/aiostream/stream/time.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/stream/transform.py` & `aiostream-0.6.0rc1/aiostream/stream/transform.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream/test_utils.py` & `aiostream-0.6.0rc1/aiostream/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/aiostream.egg-info/PKG-INFO` & `aiostream-0.6.0rc1/aiostream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostream
-Version: 0.6.0
+Version: 0.6.0rc1
 Summary: Generator-based operators for asynchronous iteration
 Author-email: Vincent Michel <vxgmichel@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `aiostream-0.6.0/aiostream.egg-info/SOURCES.txt` & `aiostream-0.6.0rc1/aiostream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/pyproject.toml` & `aiostream-0.6.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_advanced.py` & `aiostream-0.6.0rc1/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_aggregate.py` & `aiostream-0.6.0rc1/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_aiter.py` & `aiostream-0.6.0rc1/tests/test_aiter.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_combine.py` & `aiostream-0.6.0rc1/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_core.py` & `aiostream-0.6.0rc1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_create.py` & `aiostream-0.6.0rc1/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_misc.py` & `aiostream-0.6.0rc1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_select.py` & `aiostream-0.6.0rc1/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_task_group.py` & `aiostream-0.6.0rc1/tests/test_task_group.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.6.0/tests/test_transform.py` & `aiostream-0.6.0rc1/tests/test_transform.py`

 * *Files identical despite different names*

