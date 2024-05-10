# Comparing `tmp/fast_params-0.1.0.tar.gz` & `tmp/fast_params-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_params-0.1.0.tar", max compression
+gzip compressed data, was "fast_params-0.1.1.tar", max compression
```

## Comparing `fast_params-0.1.0.tar` & `fast_params-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      857 2024-05-08 12:44:21.631568 fast_params-0.1.0/README.md
--rw-r--r--   0        0        0     3844 2024-05-08 12:46:24.564509 fast_params-0.1.0/fast_params/__init__.py
--rw-r--r--   0        0        0      452 2024-05-08 12:46:44.372793 fast_params-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1229 1970-01-01 00:00:00.000000 fast_params-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-10 02:41:02.339435 fast_params-0.1.1/README.md
+-rw-r--r--   0        0        0     3902 2024-05-10 02:39:18.233045 fast_params-0.1.1/fast_params/__init__.py
+-rw-r--r--   0        0        0      452 2024-05-10 02:38:51.429360 fast_params-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 fast_params-0.1.1/PKG-INFO
```

### Comparing `fast_params-0.1.0/fast_params/__init__.py` & `fast_params-0.1.1/fast_params/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import re
-from typing import Any, Dict
-from starlette.datastructures import ImmutableMultiDict
+from typing import Any, Dict, Protocol, runtime_checkable
 
 
 class ParamsTooDeepError(Exception): ...
 
 
 class ParameterTypeError(Exception): ...
 
 
 PAT = re.compile(r"\[\]")
 PAT2 = re.compile(r"[\[\]]+")
 
 
+@runtime_checkable
+class MultiDict(Protocol):
+    def multi_items(self) -> list[tuple[str, Any]]: ...
+
+
 class ParamParser:
     def __init__(self, param_depth_limit: int = 32) -> None:
         self._param_depth_limit = param_depth_limit
 
-    def __call__(self, form: ImmutableMultiDict[str, Any]) -> Dict[str, Any]:
+    def __call__(self, form: MultiDict) -> Dict[str, Any]:
         js = self._make_params()
         for k, v in form.multi_items():
             self._normalize_params(js, k, v)
         return js
 
     def _normalize_params(
         self, params: Dict[str, Any], name: str, v: Any, depth: int = 0
```

### Comparing `fast_params-0.1.0/PKG-INFO` & `fast_params-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: fast-params
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Chongchen Chen
 Author-email: chenkovsky@qq.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: starlette (>=0.37.0)
 Description-Content-Type: text/markdown
 
 # Fast Params
 
-Support Rails style QueryParams and FormData for Starlette and FastAPI
+Support Rails style QueryParams and FormData for Starlette and FastAPI.
+
+you can also used it in other frameworks, if your params or forms follow this protocol.
+
+```
+@runtime_checkable
+class MultiDict(Protocol):
+    def multi_items(self) -> list[tuple[str, Any]]: ...
+
+```
 
 ## Install
 
 ```bash
 pip install fast-params
 ```
```

