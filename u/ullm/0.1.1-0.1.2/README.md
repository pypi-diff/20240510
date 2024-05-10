# Comparing `tmp/ullm-0.1.1.tar.gz` & `tmp/ullm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ullm-0.1.1.tar", last modified: Thu May  9 09:30:42 2024, max compression
+gzip compressed data, was "ullm-0.1.2.tar", last modified: Fri May 10 04:12:10 2024, max compression
```

## Comparing `ullm-0.1.1.tar` & `ullm-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.487064 ullm-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-09 09:30:42.487064 ullm-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-09 09:30:37.000000 ullm-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-09 09:30:37.000000 ullm-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:30:42.487064 ullm-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.483064 ullm-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-09 09:30:37.000000 ullm-0.1.1/tests/test_openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.487064 ullm-0.1.1/ullm/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (127)    23335 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/deepseek.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/iflytek.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/minimax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/moonshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/stepfun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/zero_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-09 09:30:37.000000 ullm-0.1.1/ullm/zhipu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:30:42.487064 ullm-0.1.1/ullm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 09:30:42.000000 ullm-0.1.1/ullm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:12:10.481904 ullm-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-10 04:12:10.481904 ullm-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-10 04:12:06.000000 ullm-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-10 04:12:06.000000 ullm-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:12:10.481904 ullm-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:12:10.477904 ullm-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-10 04:12:06.000000 ullm-0.1.2/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:12:10.481904 ullm-0.1.2/ullm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/deepseek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/iflytek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/minimax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/moonshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/stepfun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/zero_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-10 04:12:06.000000 ullm-0.1.2/ullm/zhipu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:12:10.481904 ullm-0.1.2/ullm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-10 04:12:10.000000 ullm-0.1.2/ullm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-10 04:12:10.000000 ullm-0.1.2/ullm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:12:10.000000 ullm-0.1.2/ullm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 04:12:10.000000 ullm-0.1.2/ullm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 04:12:10.000000 ullm-0.1.2/ullm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 04:12:10.000000 ullm-0.1.2/ullm.egg-info/top_level.txt
```

### Comparing `ullm-0.1.1/PKG-INFO` & `ullm-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.1.1 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.1.2 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
```

### Comparing `ullm-0.1.1/README.md` & `ullm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/pyproject.toml` & `ullm-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ullm"
-version = "0.1.1"
+version = "0.1.2"
 description = "A unified interface for local Large Language Model(LLM) models and online LLM providers."
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
     "pydantic",
     "arrow",
```

### Comparing `ullm-0.1.1/tests/test_openai.py` & `ullm-0.1.2/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/__init__.py` & `ullm-0.1.2/ullm/__init__.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/alibaba.py` & `ullm-0.1.2/ullm/alibaba.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/anthropic.py` & `ullm-0.1.2/ullm/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,14 @@
 
         return {"tools": tools}
 
     @validate_call
     def _convert_generation_config(
         self, config: GenerateConfig, system: Optional[str] = None
     ) -> Dict[str, Any]:
-        print(config)
         return {
             "model": self.model,
             "max_tokens": config.max_output_tokens or self.config.max_output_tokens,
             "stop_sequences": config.stop_sequences or self.config.stop_sequences,
             "temperature": config.temperature or self.config.temperature,
             "top_p": config.top_p or self.config.top_p,
             "top_k": config.top_k or self.config.top_k,
```

### Comparing `ullm-0.1.1/ullm/baichuan.py` & `ullm-0.1.2/ullm/baichuan.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/baidu.py` & `ullm-0.1.2/ullm/baidu.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,17 +592,14 @@
         messages: conlist(ChatMessage, min_length=1),
         system: Optional[str] = None,
     ) -> Dict[str, Any]:
         result = {"messages": [self._convert_message(message) for message in messages]}
         if system:
             result["system"] = system
 
-        for msg in result["messages"]:
-            print("        ", msg)
-
         return result
 
     @validate_call
     def _convert_tools(
         self, tools: Optional[List[Tool]] = None, tool_choice: Optional[ToolChoice] = None
     ) -> Dict[str, Any]:
         if not self.is_tool_model or (tool_choice and tool_choice.mode == "none"):
```

### Comparing `ullm-0.1.1/ullm/base.py` & `ullm-0.1.2/ullm/base.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/cli.py` & `ullm-0.1.2/ullm/cli.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/cohere.py` & `ullm-0.1.2/ullm/cohere.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/deepseek.py` & `ullm-0.1.2/ullm/deepseek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/google.py` & `ullm-0.1.2/ullm/google.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/groq.py` & `ullm-0.1.2/ullm/groq.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/iflytek.py` & `ullm-0.1.2/ullm/iflytek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/minimax.py` & `ullm-0.1.2/ullm/minimax.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/moonshot.py` & `ullm-0.1.2/ullm/moonshot.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/ollama.py` & `ullm-0.1.2/ullm/ollama.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/openai.py` & `ullm-0.1.2/ullm/openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/openrouter.py` & `ullm-0.1.2/ullm/openrouter.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/perplexity.py` & `ullm-0.1.2/ullm/perplexity.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/stepfun.py` & `ullm-0.1.2/ullm/stepfun.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/zero_one.py` & `ullm-0.1.2/ullm/zero_one.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm/zhipu.py` & `ullm-0.1.2/ullm/zhipu.py`

 * *Files identical despite different names*

### Comparing `ullm-0.1.1/ullm.egg-info/PKG-INFO` & `ullm-0.1.2/ullm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.1.1 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.1.2 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
```

### Comparing `ullm-0.1.1/ullm.egg-info/SOURCES.txt` & `ullm-0.1.2/ullm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

