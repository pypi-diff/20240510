# Comparing `tmp/edgegap_scheduling-1.7.1.tar.gz` & `tmp/edgegap_scheduling-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-1.7.1.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.8.0.tar", max compression
```

## Comparing `edgegap_scheduling-1.7.1.tar` & `edgegap_scheduling-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1993 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/LICENSE
--rw-r--r--   0        0        0     2164 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/README.md
--rw-r--r--   0        0        0      447 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0      124 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_model.py
--rw-r--r--   0        0        0     4642 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     5724 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1285 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1468 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      550 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     4381 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0      133 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      691 2024-05-09 20:08:28.274661 edgegap_scheduling-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2164 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/README.md
+-rw-r--r--   0        0        0      467 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0      124 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_model.py
+-rw-r--r--   0        0        0     4642 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     5724 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1305 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1468 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      550 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     4381 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0      133 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-10 18:41:29.584479 edgegap_scheduling-1.8.0/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      691 2024-05-10 18:41:50.396418 edgegap_scheduling-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.8.0/PKG-INFO
```

### Comparing `edgegap_scheduling-1.7.1/LICENSE` & `edgegap_scheduling-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.1/README.md` & `edgegap_scheduling-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.1/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.8.0/edgegap_scheduling/_runner.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.1/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.8.0/edgegap_scheduling/_scheduler.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.1/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.8.0/edgegap_scheduling/_signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import logging
 from types import AsyncGeneratorType, GeneratorType
 from typing import Any, Callable
 
 from pydantic import BaseModel
 
-from ._depends import Depends
+from ._depends import SchedulingDepends
 
 
 class TaskSignature:
     def __init__(self, identifier: str, name: str, func: Callable):
         self.__identifier = identifier
         self.__name = name
         self.__func = func
@@ -20,15 +20,15 @@
     ) -> tuple[dict[str, Any], dict[str, Any]]:
         specs = {}
         generators = {}
         signature = inspect.signature(self.__func)
 
         for name, param in signature.parameters.items():
             match param.default:
-                case Depends():
+                case SchedulingDepends():
                     value = param.default.dependency()
 
                     if isinstance(value, (GeneratorType, AsyncGeneratorType)):
                         generators[name] = value
                     else:
                         specs[name] = value
```

### Comparing `edgegap_scheduling-1.7.1/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.8.0/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.1/edgegap_scheduling/_state.py` & `edgegap_scheduling-1.8.0/edgegap_scheduling/_state.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.1/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.8.0/edgegap_scheduling/_task.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.1/pyproject.toml` & `edgegap_scheduling-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-scheduling"
-version = "1.7.1"
+version = "1.8.0"
 description = "The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.7.1"
```

### Comparing `edgegap_scheduling-1.7.1/PKG-INFO` & `edgegap_scheduling-1.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 1.7.1
+Version: 1.8.0
 Summary: The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

