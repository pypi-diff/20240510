# Comparing `tmp/iudex-0.4.3.tar.gz` & `tmp/iudex-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.3.tar", max compression
+gzip compressed data, was "iudex-0.4.4.tar", max compression
```

## Comparing `iudex-0.4.3.tar` & `iudex-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.3/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.3/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.3/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.3/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.3/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.3/iudex/functions.py
--rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.3/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.3/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2816 2024-05-10 11:08:48.595109 iudex-0.4.3/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1622 2024-05-10 08:08:22.984691 iudex-0.4.3/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.3/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1165 2024-05-10 08:08:22.984691 iudex-0.4.3/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.3/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.3/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.3/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-10 10:59:40.087371 iudex-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.4/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.4/README.md
+-rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.4/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.4/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.4/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.4/iudex/functions.py
+-rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.4/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.4/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 17:33:40.765835 iudex-0.4.4/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1622 2024-05-10 08:08:22.984691 iudex-0.4.4/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.4/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1165 2024-05-10 08:08:22.984691 iudex-0.4.4/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.4/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.4/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.4/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-10 17:33:52.285815 iudex-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.4/PKG-INFO
```

### Comparing `iudex-0.4.3/LICENSE` & `iudex-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/README.md` & `iudex-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/chat.py` & `iudex-0.4.4/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/client.py` & `iudex-0.4.4/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/functions.py` & `iudex-0.4.4/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/instrumentation/README.md` & `iudex-0.4.4/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/instrumentation/attributes.py` & `iudex-0.4.4/iudex/instrumentation/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     attributes[SpanAttributes.CODE_LINENO] = record.lineno
 
     if record.exc_info:
         exctype, value, tb = record.exc_info
         if exctype is not None:
             attributes[SpanAttributes.EXCEPTION_TYPE] = exctype.__name__
         if value is not None and value.args:
-            attributes[SpanAttributes.EXCEPTION_MESSAGE] = value.args[0]
+            attributes[SpanAttributes.EXCEPTION_MESSAGE] = str(value.args[0])
         if tb is not None:
             # https://github.com/open-telemetry/opentelemetry-specification/blob/9fa7c656b26647b27e485a6af7e38dc716eba98a/specification/trace/semantic_conventions/exceptions.md#stacktrace-representation
             attributes[SpanAttributes.EXCEPTION_STACKTRACE] = "".join(
                 traceback.format_exception(*record.exc_info)
             )
     return attributes
```

### Comparing `iudex-0.4.3/iudex/instrumentation/fastapi.py` & `iudex-0.4.4/iudex/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/instrumentation/instrumentation.py` & `iudex-0.4.4/iudex/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/instrumentation/lambda.py` & `iudex-0.4.4/iudex/instrumentation/lambda.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/iudex/types/function.py` & `iudex-0.4.4/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.3/pyproject.toml` & `iudex-0.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
```

### Comparing `iudex-0.4.3/PKG-INFO` & `iudex-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

