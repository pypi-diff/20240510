# Comparing `tmp/orq_ai_sdk-2.3.5.tar.gz` & `tmp/orq_ai_sdk-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orq_ai_sdk-2.3.5.tar", max compression
+gzip compressed data, was "orq_ai_sdk-2.3.6.tar", max compression
```

## Comparing `orq_ai_sdk-2.3.5.tar` & `orq_ai_sdk-2.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2024-03-15 09:27:20.060670 orq_ai_sdk-2.3.5/LICENSE
--rw-r--r--   0        0        0     7382 2024-03-21 12:42:41.520384 orq_ai_sdk-2.3.5/README.md
--rw-r--r--   0        0        0       38 2024-03-15 09:27:20.061191 orq_ai_sdk-2.3.5/orq_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:27:20.061230 orq_ai_sdk-2.3.5/orq_ai_sdk/api_resources/__init__.py
--rw-r--r--   0        0        0    14123 2024-03-26 00:32:08.214534 orq_ai_sdk-2.3.5/orq_ai_sdk/api_resources/async_deployments.py
--rw-r--r--   0        0        0    14144 2024-03-26 00:32:08.257393 orq_ai_sdk-2.3.5/orq_ai_sdk/api_resources/deployments.py
--rw-r--r--   0        0        0     2739 2024-03-15 09:27:20.061820 orq_ai_sdk-2.3.5/orq_ai_sdk/client.py
--rw-r--r--   0        0        0     1653 2024-03-15 09:27:20.061947 orq_ai_sdk-2.3.5/orq_ai_sdk/exceptions.py
--rw-r--r--   0        0        0     2218 2024-04-18 09:01:59.667059 orq_ai_sdk-2.3.5/orq_ai_sdk/http_client.py
--rw-r--r--   0        0        0      136 2024-03-15 09:27:20.062170 orq_ai_sdk-2.3.5/orq_ai_sdk/models.py
--rw-r--r--   0        0        0     1399 2024-03-21 12:24:03.900585 orq_ai_sdk-2.3.5/orq_ai_sdk/util.py
--rw-r--r--   0        0        0       18 2024-04-18 09:02:38.594963 orq_ai_sdk-2.3.5/orq_ai_sdk/version.py
--rw-r--r--   0        0        0     1306 2024-04-18 09:02:39.416601 orq_ai_sdk-2.3.5/pyproject.toml
--rw-r--r--   0        0        0     8474 1970-01-01 00:00:00.000000 orq_ai_sdk-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-03-15 09:27:20.060670 orq_ai_sdk-2.3.6/LICENSE
+-rw-r--r--   0        0        0     7382 2024-03-21 12:42:41.520384 orq_ai_sdk-2.3.6/README.md
+-rw-r--r--   0        0        0       38 2024-03-15 09:27:20.061191 orq_ai_sdk-2.3.6/orq_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:27:20.061230 orq_ai_sdk-2.3.6/orq_ai_sdk/api_resources/__init__.py
+-rw-r--r--   0        0        0    14123 2024-03-26 00:32:08.214534 orq_ai_sdk-2.3.6/orq_ai_sdk/api_resources/async_deployments.py
+-rw-r--r--   0        0        0    14144 2024-03-26 00:32:08.257393 orq_ai_sdk-2.3.6/orq_ai_sdk/api_resources/deployments.py
+-rw-r--r--   0        0        0     2739 2024-03-15 09:27:20.061820 orq_ai_sdk-2.3.6/orq_ai_sdk/client.py
+-rw-r--r--   0        0        0     1653 2024-03-15 09:27:20.061947 orq_ai_sdk-2.3.6/orq_ai_sdk/exceptions.py
+-rw-r--r--   0        0        0     2268 2024-05-10 08:04:24.038457 orq_ai_sdk-2.3.6/orq_ai_sdk/http_client.py
+-rw-r--r--   0        0        0      136 2024-03-15 09:27:20.062170 orq_ai_sdk-2.3.6/orq_ai_sdk/models.py
+-rw-r--r--   0        0        0     1399 2024-03-21 12:24:03.900585 orq_ai_sdk-2.3.6/orq_ai_sdk/util.py
+-rw-r--r--   0        0        0       18 2024-05-10 08:06:13.934540 orq_ai_sdk-2.3.6/orq_ai_sdk/version.py
+-rw-r--r--   0        0        0     1306 2024-05-10 08:16:01.830255 orq_ai_sdk-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0     8474 1970-01-01 00:00:00.000000 orq_ai_sdk-2.3.6/PKG-INFO
```

### Comparing `orq_ai_sdk-2.3.5/LICENSE` & `orq_ai_sdk-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.5/README.md` & `orq_ai_sdk-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.5/orq_ai_sdk/api_resources/async_deployments.py` & `orq_ai_sdk-2.3.6/orq_ai_sdk/api_resources/async_deployments.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.5/orq_ai_sdk/api_resources/deployments.py` & `orq_ai_sdk-2.3.6/orq_ai_sdk/api_resources/deployments.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.5/orq_ai_sdk/client.py` & `orq_ai_sdk-2.3.6/orq_ai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.5/orq_ai_sdk/exceptions.py` & `orq_ai_sdk-2.3.6/orq_ai_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.5/orq_ai_sdk/http_client.py` & `orq_ai_sdk-2.3.6/orq_ai_sdk/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     }
 
 
 def build_body(environment, body):
     if environment:
         if body.get("context", None) is None:
             body["context"] = {"environments": [environment]}
-        else:
+        elif body["context"].get("environments", None) is None:
             body["context"]["environments"] = [environment]
     return body
 
 
 def post(url: str, api_key: str, body: dict, environment=None):
     headers = build_headers(api_key)
     body = build_body(environment, body)
```

### Comparing `orq_ai_sdk-2.3.5/orq_ai_sdk/util.py` & `orq_ai_sdk-2.3.6/orq_ai_sdk/util.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.5/pyproject.toml` & `orq_ai_sdk-2.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orq_ai_sdk"
-version = '2.3.5'
+version = '2.3.6'
 description = "Integrate and operate your products with the power of Large Language Models from a single collaboration platform. Conduct prompt engineering, experimentation, operations and monitoring across models, with full transparency on quality and costs."
 authors = ["orq.ai <support@orq.ai>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `orq_ai_sdk-2.3.5/PKG-INFO` & `orq_ai_sdk-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orq_ai_sdk
-Version: 2.3.5
+Version: 2.3.6
 Summary: Integrate and operate your products with the power of Large Language Models from a single collaboration platform. Conduct prompt engineering, experimentation, operations and monitoring across models, with full transparency on quality and costs.
 Author: orq.ai
 Author-email: support@orq.ai
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: orq_ai_sdk Version: 2.3.5 Summary: Integrate and
+Metadata-Version: 2.1 Name: orq_ai_sdk Version: 2.3.6 Summary: Integrate and
 operate your products with the power of Large Language Models from a single
 collaboration platform. Conduct prompt engineering, experimentation, operations
 and monitoring across models, with full transparency on quality and costs.
 Author: orq.ai Author-email: support@orq.ai Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
```

