# Comparing `tmp/llama_index_llms_huggingface-0.1.5.tar.gz` & `tmp/llama_index_llms_huggingface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_huggingface-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_llms_huggingface-0.2.0.tar", max compression
```

## Comparing `llama_index_llms_huggingface-0.1.5.tar` & `llama_index_llms_huggingface-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/README.md
--rw-r--r--   0        0        0      212 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    39711 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/base.py
--rw-r--r--   0        0        0     2082 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/utils.py
--rw-r--r--   0        0        0     1636 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       43 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/README.md
+-rw-r--r--   0        0        0      212 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    39711 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/base.py
+-rw-r--r--   0        0        0     2082 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/utils.py
+-rw-r--r--   0        0        0     1636 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.2.0/PKG-INFO
```

### Comparing `llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/base.py` & `llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/utils.py` & `llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_huggingface-0.1.5/pyproject.toml` & `llama_index_llms_huggingface-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms huggingface integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-huggingface"
 readme = "README.md"
-version = "0.1.5"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-huggingface-hub = "^0.20.3"
+huggingface-hub = "^0.23.0"
 torch = "^2.1.2"
 text-generation = "^0.7.0"
 
 [tool.poetry.dependencies.transformers]
 extras = ["torch"]
 version = "^4.37.0"
```

### Comparing `llama_index_llms_huggingface-0.1.5/PKG-INFO` & `llama_index_llms_huggingface-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-huggingface
-Version: 0.1.5
+Version: 0.2.0
 Summary: llama-index llms huggingface integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: huggingface-hub (>=0.20.3,<0.21.0)
+Requires-Dist: huggingface-hub (>=0.23.0,<0.24.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: text-generation (>=0.7.0,<0.8.0)
 Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: transformers[torch] (>=4.37.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Huggingface
```

