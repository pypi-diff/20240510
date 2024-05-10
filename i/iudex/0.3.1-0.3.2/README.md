# Comparing `tmp/iudex-0.3.1.tar.gz` & `tmp/iudex-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.3.1.tar", max compression
+gzip compressed data, was "iudex-0.3.2.tar", max compression
```

## Comparing `iudex-0.3.1.tar` & `iudex-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-03-05 02:32:42.683184 iudex-0.3.1/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-07 17:48:23.958486 iudex-0.3.1/README.md
--rw-r--r--   0        0        0       54 2024-03-05 02:32:42.685374 iudex-0.3.1/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-22 23:11:09.655241 iudex-0.3.1/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-22 23:11:09.655456 iudex-0.3.1/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-22 23:11:09.655988 iudex-0.3.1/iudex/functions.py
--rw-r--r--   0        0        0     1429 2024-05-07 19:47:37.568338 iudex-0.3.1/iudex/instrumentation/README.md
--rw-r--r--   0        0        0        0 2024-05-07 18:53:14.946672 iudex-0.3.1/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     1605 2024-05-07 18:50:00.465742 iudex-0.3.1/iudex/instrumentation/fastapi_instrumentation.py
--rw-r--r--   0        0        0     1532 2024-05-07 19:47:37.568588 iudex-0.3.1/iudex/instrumentation/lambda_instrumentation.py
--rw-r--r--   0        0        0      236 2024-03-05 02:32:42.686766 iudex-0.3.1/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-22 23:11:09.656442 iudex-0.3.1/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-06 19:49:41.321305 iudex-0.3.1/iudex/utils.py
--rw-r--r--   0        0        0      607 2024-05-07 19:49:06.998438 iudex-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.3.2/README.md
+-rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.3.2/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.3.2/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.3.2/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.3.2/iudex/functions.py
+-rw-r--r--   0        0        0     1429 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1605 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/fastapi_instrumentation.py
+-rw-r--r--   0        0        0     1532 2024-05-07 19:47:45.464330 iudex-0.3.2/iudex/instrumentation/lambda_instrumentation.py
+-rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.3.2/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.3.2/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.3.2/iudex/utils.py
+-rw-r--r--   0        0        0      607 2024-05-09 16:32:47.053890 iudex-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9119 1970-01-01 00:00:00.000000 iudex-0.3.2/PKG-INFO
```

### Comparing `iudex-0.3.1/LICENSE` & `iudex-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/README.md` & `iudex-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/iudex/chat.py` & `iudex-0.3.2/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/iudex/client.py` & `iudex-0.3.2/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/iudex/functions.py` & `iudex-0.3.2/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/iudex/instrumentation/README.md` & `iudex-0.3.2/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/iudex/instrumentation/fastapi_instrumentation.py` & `iudex-0.3.2/iudex/instrumentation/fastapi_instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/iudex/instrumentation/lambda_instrumentation.py` & `iudex-0.3.2/iudex/instrumentation/lambda_instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/iudex/types/function.py` & `iudex-0.3.2/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.3.1/pyproject.toml` & `iudex-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "iudex"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
 httpx = "^0.26.0"
-pydantic = "^1.0.0"
+pydantic = "^2.7.1"
 opentelemetry-distro = "^0.45b0"
 opentelemetry-instrumentation-fastapi = "^0.45b0"
 opentelemetry-exporter-otlp-proto-http = "^1.24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 python-dotenv = "^1.0.1"
```

### Comparing `iudex-0.3.1/PKG-INFO` & `iudex-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: opentelemetry-distro (>=0.45b0,<0.46)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.24.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.45b0,<0.46)
-Requires-Dist: pydantic (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Iudex Python Client
 
 **✨ Build 🛠 With Next Gen LLM Function Calling ✨**
 
 [Iudex](https://iudex.ai) is an agent accessible via API that provides more accurate, secure, and scalable LLM function calling.
```

