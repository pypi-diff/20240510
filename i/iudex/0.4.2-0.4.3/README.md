# Comparing `tmp/iudex-0.4.2.tar.gz` & `tmp/iudex-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.2.tar", max compression
+gzip compressed data, was "iudex-0.4.3.tar", max compression
```

## Comparing `iudex-0.4.2.tar` & `iudex-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.2/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.2/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.2/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.2/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.2/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.2/iudex/functions.py
--rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.2/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.2/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2080 2024-05-10 09:52:04.727928 iudex-0.4.2/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1622 2024-05-10 08:08:22.984691 iudex-0.4.2/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.2/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1165 2024-05-10 08:08:22.984691 iudex-0.4.2/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.2/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.2/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.2/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-10 09:53:12.899857 iudex-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.3/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.3/README.md
+-rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.3/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.3/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.3/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.3/iudex/functions.py
+-rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.3/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.3/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2816 2024-05-10 11:08:48.595109 iudex-0.4.3/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1622 2024-05-10 08:08:22.984691 iudex-0.4.3/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.3/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1165 2024-05-10 08:08:22.984691 iudex-0.4.3/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.3/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.3/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.3/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-10 10:59:40.087371 iudex-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.3/PKG-INFO
```

### Comparing `iudex-0.4.2/LICENSE` & `iudex-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/README.md` & `iudex-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/chat.py` & `iudex-0.4.3/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/client.py` & `iudex-0.4.3/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/functions.py` & `iudex-0.4.3/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/instrumentation/README.md` & `iudex-0.4.3/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/instrumentation/attributes.py` & `iudex-0.4.3/iudex/instrumentation/attributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,17 +36,15 @@
 
 
 def get_attributes(record: LogRecord):
     """Monkeypatch for non-primitive (e.g. dict) attribute values defined in LogRecord.extra.
 
     See https://github.com/open-telemetry/opentelemetry-python/blob/c06e6f4b8616618907d70fa023eb2baab7a6ca61/opentelemetry-sdk/src/opentelemetry/sdk/_logs/_internal/__init__.py#L460
     """
-    attributes: Dict = {
-        k: str(v) for k, v in vars(record).items() if k not in _RESERVED_ATTRS
-    }
+    attributes = flatten_attributes(record)
 
     # Add standard code attributes for logs.
     attributes[SpanAttributes.CODE_FILEPATH] = record.pathname
     attributes[SpanAttributes.CODE_FUNCTION] = record.funcName
     attributes[SpanAttributes.CODE_LINENO] = record.lineno
 
     if record.exc_info:
@@ -57,7 +55,33 @@
             attributes[SpanAttributes.EXCEPTION_MESSAGE] = value.args[0]
         if tb is not None:
             # https://github.com/open-telemetry/opentelemetry-specification/blob/9fa7c656b26647b27e485a6af7e38dc716eba98a/specification/trace/semantic_conventions/exceptions.md#stacktrace-representation
             attributes[SpanAttributes.EXCEPTION_STACKTRACE] = "".join(
                 traceback.format_exception(*record.exc_info)
             )
     return attributes
+
+
+def flatten_attributes(record: LogRecord):
+    """Convert LogRecord to flattened attribute dict.
+
+    For instance {"a": {"b": 1}} will be converted to {"a.b": 1}.
+    """
+    seen = set()
+    attrs = {}
+    def flatten_helper(item, prefix=""):
+        if prefix in _RESERVED_ATTRS:
+            return
+        if not isinstance(item, dict):
+            attrs[prefix] = str(item)
+            return
+        for key, value in item.items():
+            full_key = f"{prefix}.{key}" if prefix else key
+            if id(value) in seen:
+                # circular reference
+                attrs[full_key] = str(value)
+                continue
+            seen.add(id(value))
+            flatten_helper(value, full_key)
+            seen.remove(id(value))
+    flatten_helper(vars(record))
+    return attrs
```

### Comparing `iudex-0.4.2/iudex/instrumentation/fastapi.py` & `iudex-0.4.3/iudex/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/instrumentation/instrumentation.py` & `iudex-0.4.3/iudex/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/instrumentation/lambda.py` & `iudex-0.4.3/iudex/instrumentation/lambda.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/iudex/types/function.py` & `iudex-0.4.3/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.2/pyproject.toml` & `iudex-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
```

### Comparing `iudex-0.4.2/PKG-INFO` & `iudex-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

