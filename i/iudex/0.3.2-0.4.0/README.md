# Comparing `tmp/iudex-0.3.2.tar.gz` & `tmp/iudex-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.3.2.tar", max compression
+gzip compressed data, was "iudex-0.4.0.tar", max compression
```

## Comparing `iudex-0.3.2.tar` & `iudex-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.3.2/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.3.2/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.3.2/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.3.2/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.3.2/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.3.2/iudex/functions.py
--rw-r--r--   0        0        0     1429 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/README.md
--rw-r--r--   0        0        0        0 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     1605 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/fastapi_instrumentation.py
--rw-r--r--   0        0        0     1532 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/lambda_instrumentation.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.3.2/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.3.2/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.3.2/iudex/utils.py
--rw-r--r--   0        0        0      607 2024-05-09 16:32:47.053890 iudex-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9119 1970-01-01 00:00:00.000000 iudex-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.0/README.md
+-rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.0/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.0/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.0/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.0/iudex/functions.py
+-rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.0/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 00:08:55.250836 iudex-0.4.0/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-10 07:41:42.254253 iudex-0.4.0/iudex/instrumentation/fastapi_instrumentation.py
+-rw-r--r--   0        0        0     4772 2024-05-10 07:40:26.701919 iudex-0.4.0/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1383 2024-05-10 07:42:04.844179 iudex-0.4.0/iudex/instrumentation/lambda_instrumentation.py
+-rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.0/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.0/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.0/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-10 07:42:07.714902 iudex-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.0/PKG-INFO
```

### Comparing `iudex-0.3.2/LICENSE` & `iudex-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.3.2/README.md` & `iudex-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.3.2/iudex/chat.py` & `iudex-0.4.0/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.2/iudex/client.py` & `iudex-0.4.0/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.2/iudex/functions.py` & `iudex-0.4.0/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.2/iudex/instrumentation/README.md` & `iudex-0.4.0/iudex/instrumentation/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,19 @@
 
 # Lambda / Serverless
 
 1. Pip install dependencies
 ```bash
 pip install iudex
 ```
-2. Import `instrument_app` where you defined FastAPI (usually `main.py`) from `iudex`
+2. Import `instrument_app` from `iudex` and invoke it in your entrypoint (usually `main.py`)
 ```python
 # Add this in your lambda function file (likely lambda_function.py)
 from iudex.instrumentation.lambda_instrumentation import instrument_app
-instrument_app(api_key=os.getenv("IUDEX_API_KEY"), service_name=__main__)
+instrument_app(
+  api_key=os.getenv("IUDEX_API_KEY"),
+  service_name=__name__, # or any string describing your service
+)
 ```
 3. Make sure the app has access to the environment variable `IUDEX_API_KEY`
 4. You should be all set! Go to [https://app.iudex.ai/](https://app.iudex.ai/) and enter your API key
 5. Go to [https://app.iudex.ai/logs](https://app.iudex.ai/logs) and press `Search` to view your logs
```

### Comparing `iudex-0.3.2/iudex/types/function.py` & `iudex-0.4.0/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.2/pyproject.toml` & `iudex-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "iudex"
-version = "0.3.2"
+version = "0.4.0"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
 httpx = "^0.26.0"
 pydantic = "^2.7.1"
 opentelemetry-distro = "^0.45b0"
 opentelemetry-instrumentation-fastapi = "^0.45b0"
 opentelemetry-exporter-otlp-proto-http = "^1.24.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.2.0"
 python-dotenv = "^1.0.1"
 
+[tool.poetry.group.test.dependencies]
+pytest = "^8.2.0"
+fastapi = "^0.111.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [virtualenvs]
 in-project = true
```

### Comparing `iudex-0.3.2/PKG-INFO` & `iudex-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: opentelemetry-distro (>=0.45b0,<0.46)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.24.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.45b0,<0.46)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
```

