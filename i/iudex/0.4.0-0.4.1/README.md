# Comparing `tmp/iudex-0.4.0.tar.gz` & `tmp/iudex-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.0.tar", max compression
+gzip compressed data, was "iudex-0.4.1.tar", max compression
```

## Comparing `iudex-0.4.0.tar` & `iudex-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.0/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.0/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.0/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.0/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.0/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.0/iudex/functions.py
--rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.0/iudex/instrumentation/README.md
--rw-r--r--   0        0        0        0 2024-05-10 00:08:55.250836 iudex-0.4.0/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     1840 2024-05-10 07:41:42.254253 iudex-0.4.0/iudex/instrumentation/fastapi_instrumentation.py
--rw-r--r--   0        0        0     4772 2024-05-10 07:40:26.701919 iudex-0.4.0/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1383 2024-05-10 07:42:04.844179 iudex-0.4.0/iudex/instrumentation/lambda_instrumentation.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.0/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.0/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.0/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-10 07:42:07.714902 iudex-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.1/README.md
+-rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.1/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.1/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.1/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.1/iudex/functions.py
+-rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.1/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-10 07:57:57.940028 iudex-0.4.1/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1622 2024-05-10 07:59:11.073154 iudex-0.4.1/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     4873 2024-05-10 08:03:58.388134 iudex-0.4.1/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1165 2024-05-10 07:59:15.173146 iudex-0.4.1/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.1/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.1/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.1/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-10 08:05:53.190659 iudex-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.1/PKG-INFO
```

### Comparing `iudex-0.4.0/LICENSE` & `iudex-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.0/README.md` & `iudex-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.0/iudex/chat.py` & `iudex-0.4.1/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.0/iudex/client.py` & `iudex-0.4.1/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.0/iudex/functions.py` & `iudex-0.4.1/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.0/iudex/instrumentation/README.md` & `iudex-0.4.1/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.0/iudex/instrumentation/fastapi_instrumentation.py` & `iudex-0.4.1/iudex/instrumentation/fastapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,21 +20,14 @@
     If you use Gunicorn, invoke it within a post_fork hook:
     ```python
     def post_fork(server, worker):
         instrument(...)
     ```
     Per https://opentelemetry-python.readthedocs.io/en/latest/examples/fork-process-model/README.html.
 
-    If you use named loggers, instrument them using the returned config object:
-    ```python
-    my_logger = logging.getLogger("my_logger")
-    config = instrument(...)
-    config.configure_logger(my_logger)
-    ```
-
     Args:
         app: FastAPI app to instrument.
         service_name: Name of the service, e.g. "billing_service", __name__.
             If not supplied, env var OTEL_SERVICE_NAME will be used.
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
```

### Comparing `iudex-0.4.0/iudex/instrumentation/instrumentation.py` & `iudex-0.4.1/iudex/instrumentation/instrumentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,31 +102,36 @@
         # configure logger
         logger_provider = LoggerProvider(resource=resource)
         log_exporter = OTLPLogExporter(endpoint=self.logs_endpoint, headers=headers)
         logger_provider.add_log_record_processor(BatchLogRecordProcessor(log_exporter))
         set_logger_provider(logger_provider)
         logging.basicConfig(level=self.log_level)
         # add handler to root logger
-        self.configure_logger(log_level=self.log_level)
+        configure_logger(log_level=self.log_level)
 
         # configure tracer
         trace_provider = TracerProvider(resource=resource)
         span_exporter = OTLPSpanExporter(endpoint=self.traces_endpoint, headers=headers)
         trace_provider.add_span_processor(BatchSpanProcessor(span_exporter))
         set_tracer_provider(trace_provider)
 
         IUDEX_CONFIGURED = True
 
-    def configure_logger(
-        self,
-        logger_name: Optional[str] = None,
-        log_level: Optional[Union[str, int]] = logging.NOTSET,
-    ):
-        if isinstance(log_level, str):
-            log_level = LOG_LEVEL_ATOI.get(log_level.upper())
-        log_level = log_level or self.log_level or logging.NOTSET
-
-        logger = logging.getLogger(logger_name)
-        logger.setLevel(log_level)
-        logger.addHandler(LoggingHandler(level=log_level))
 
-        return logger
+def configure_logger(
+    logger_name: Optional[str] = None,
+    log_level: Optional[Union[str, int]] = logging.NOTSET,
+):
+    """Instruments a named logger.
+
+    Useful for non-root loggers with propagate=False.
+    This way, the logger still has the instrumented handler to send logs to Iudex.
+    """
+    if isinstance(log_level, str):
+        log_level = LOG_LEVEL_ATOI.get(log_level.upper())
+    log_level = log_level or logging.NOTSET
+
+    logger = logging.getLogger(logger_name)
+    logger.setLevel(log_level)
+    logger.addHandler(LoggingHandler(level=log_level))
+
+    return logger
```

### Comparing `iudex-0.4.0/iudex/instrumentation/lambda_instrumentation.py` & `iudex-0.4.1/iudex/instrumentation/lambda.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,14 @@
     iudex_api_key: Optional[str] = None,
     config: Optional[IudexConfig] = None,
 ):
     """Auto-instruments app to send OTel signals to Iudex.
 
     Invoke this function in your Lambda entrypoint.
 
-    If you use named loggers, instrument them using the returned config object:
-    ```python
-    my_logger = logging.getLogger("my_logger")
-    config = instrument(...)
-    config.configure_logger(my_logger)
-    ```
-
     Args:
         service_name: Name of the service, e.g. "billing_service", __name__.
             If not supplied, env var OTEL_SERVICE_NAME will be used.
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
         config: IudexConfig object with more granular options.
```

### Comparing `iudex-0.4.0/iudex/types/function.py` & `iudex-0.4.1/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.0/pyproject.toml` & `iudex-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
```

### Comparing `iudex-0.4.0/PKG-INFO` & `iudex-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

