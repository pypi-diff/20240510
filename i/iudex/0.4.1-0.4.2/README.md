# Comparing `tmp/iudex-0.4.1.tar.gz` & `tmp/iudex-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.1.tar", max compression
+gzip compressed data, was "iudex-0.4.2.tar", max compression
```

## Comparing `iudex-0.4.1.tar` & `iudex-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.1/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.1/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.1/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.1/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.1/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.1/iudex/functions.py
--rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.1/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-10 07:57:57.940028 iudex-0.4.1/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     1622 2024-05-10 07:59:11.073154 iudex-0.4.1/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     4873 2024-05-10 08:03:58.388134 iudex-0.4.1/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1165 2024-05-10 07:59:15.173146 iudex-0.4.1/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.1/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.1/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.1/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-10 08:05:53.190659 iudex-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.2/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.2/README.md
+-rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.2/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.2/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.2/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.2/iudex/functions.py
+-rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.2/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.2/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2080 2024-05-10 09:52:04.727928 iudex-0.4.2/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1622 2024-05-10 08:08:22.984691 iudex-0.4.2/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.2/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1165 2024-05-10 08:08:22.984691 iudex-0.4.2/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.2/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.2/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.2/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-10 09:53:12.899857 iudex-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.2/PKG-INFO
```

### Comparing `iudex-0.4.1/LICENSE` & `iudex-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/README.md` & `iudex-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/iudex/chat.py` & `iudex-0.4.2/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/iudex/client.py` & `iudex-0.4.2/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/iudex/functions.py` & `iudex-0.4.2/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/iudex/instrumentation/README.md` & `iudex-0.4.2/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/iudex/instrumentation/fastapi.py` & `iudex-0.4.2/iudex/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/iudex/instrumentation/instrumentation.py` & `iudex-0.4.2/iudex/instrumentation/instrumentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     OTEL_SERVICE_NAME,
 )
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.trace import set_tracer_provider
 
+from .attributes import get_attributes
+
 _logger = logging.getLogger(__name__)
 
 DEFAULT_SERVICE_NAME = "unknown_service:python"
 DEFAULT_IUDEX_LOGS_ENDPOINT = "https://api.iudex.ai/resource_logs"
 DEFAULT_IUDEX_TRACES_ENDPOINT = "https://api.iudex.ai/traces"
 LOG_LEVEL_ATOI = {
     "DEBUG": logging.DEBUG,
@@ -128,10 +130,12 @@
     """
     if isinstance(log_level, str):
         log_level = LOG_LEVEL_ATOI.get(log_level.upper())
     log_level = log_level or logging.NOTSET
 
     logger = logging.getLogger(logger_name)
     logger.setLevel(log_level)
-    logger.addHandler(LoggingHandler(level=log_level))
+    logger_handler = LoggingHandler(level=log_level)
+    logger_handler._get_attributes = get_attributes
+    logger.addHandler(logger_handler)
 
     return logger
```

### Comparing `iudex-0.4.1/iudex/instrumentation/lambda.py` & `iudex-0.4.2/iudex/instrumentation/lambda.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/iudex/types/function.py` & `iudex-0.4.2/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.1/pyproject.toml` & `iudex-0.4.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
```

### Comparing `iudex-0.4.1/PKG-INFO` & `iudex-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

