# Comparing `tmp/martian_adapters-5.0.0.tar.gz` & `tmp/martian_adapters-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-5.0.0.tar", max compression
+gzip compressed data, was "martian_adapters-5.0.1.tar", max compression
```

## Comparing `martian_adapters-5.0.0.tar` & `martian_adapters-5.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/LICENSE
--rw-r--r--   0        0        0     3553 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/README.md
--rw-r--r--   0        0        0      725 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     2125 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2486 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0      523 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5893 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     6778 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3416 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0     1017 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9231 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4102 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2412 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2587 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1836 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2985 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4444 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2450 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2602 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    11047 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/rate_limiter.py
--rw-r--r--   0        0        0      335 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/requirements.txt
--rw-r--r--   0        0        0     6903 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/types.py
--rw-r--r--   0        0        0        0 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-05-07 19:56:20.868040 martian_adapters-5.0.0/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-05-07 19:56:20.872040 martian_adapters-5.0.0/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1170 2024-05-07 19:56:20.872040 martian_adapters-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     4901 1970-01-01 00:00:00.000000 martian_adapters-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/LICENSE
+-rw-r--r--   0        0        0     3553 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/README.md
+-rw-r--r--   0        0        0      725 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     2125 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2486 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0      523 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5893 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     6778 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3416 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0     1017 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9231 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4102 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2412 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2587 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1836 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2985 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1757 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1331 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4444 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2450 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2602 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    11047 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      316 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/requirements.txt
+-rw-r--r--   0        0        0     6903 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-09 16:46:37.261694 martian_adapters-5.0.1/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-09 16:46:37.265694 martian_adapters-5.0.1/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-09 16:46:37.265694 martian_adapters-5.0.1/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1147 2024-05-09 16:46:37.265694 martian_adapters-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 martian_adapters-5.0.1/PKG-INFO
```

### Comparing `martian_adapters-5.0.0/LICENSE` & `martian_adapters-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/README.md` & `martian_adapters-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/__init__.py` & `martian_adapters-5.0.1/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-5.0.1/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-5.0.1/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-5.0.1/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-5.0.1/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-5.0.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-5.0.1/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-5.0.1/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/adapter_factory.py` & `martian_adapters-5.0.1/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-5.0.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/__init__.py` & `martian_adapters-5.0.1/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-5.0.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/rate_limiter.py` & `martian_adapters-5.0.1/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/types.py` & `martian_adapters-5.0.1/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/utils/general_utils.py` & `martian_adapters-5.0.1/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/utils/network_utils.py` & `martian_adapters-5.0.1/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/adapters/utils/openai_client_factory.py` & `martian_adapters-5.0.1/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.0.0/pyproject.toml` & `martian_adapters-5.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "5.0.0"
+version = "5.0.1"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.9.4"
 aiolimiter = "^1.1.0"
 aiosignal = "^1.3.1"
 anthropic = "0.16.0"
 async-timeout = "^4.0.3"
 attrs = "^23.1.0"
-certifi = "^2023.7.22"
 charset-normalizer = "^3.2.0"
 frozenlist = "^1.4.0"
 idna = "^3.7"
 isort = "^5.12.0"
 multidict = "^6.0.4"
 regex = "^2023.8.8"
 requests = "^2.31.0"
```

### Comparing `martian_adapters-5.0.0/PKG-INFO` & `martian_adapters-5.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 5.0.0
+Version: 5.0.1
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: aiosignal (>=1.3.1,<2.0.0)
 Requires-Dist: anthropic (==0.16.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: charset-normalizer (>=3.2.0,<4.0.0)
 Requires-Dist: frozenlist (>=1.4.0,<2.0.0)
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
 Requires-Dist: idna (>=3.7,<4.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: multidict (>=6.0.4,<7.0.0)
 Requires-Dist: openai (==1.23.6)
```

