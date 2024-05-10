# Comparing `tmp/llama_tools-0.1.3.tar.gz` & `tmp/llama_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_tools-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llama_tools-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llama_tools-0.1.3.tar` & `llama_tools-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.3/.gitignore
--rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.3/README.md
--rw-r--r--   0        0        0      314 2024-05-09 22:16:44.058649 llama_tools-0.1.3/llama_tools/__init__.py
--rw-r--r--   0        0        0     1626 2024-05-09 22:16:03.483726 llama_tools-0.1.3/llama_tools/postprocess.py
--rw-r--r--   0        0        0    11029 2024-05-09 01:00:53.061092 llama_tools-0.1.3/llama_tools/preprocess.py
--rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.4/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.4/README.md
+-rw-r--r--   0        0        0      314 2024-05-10 00:33:36.280975 llama_tools-0.1.4/llama_tools/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-10 00:22:41.202663 llama_tools-0.1.4/llama_tools/postprocess.py
+-rw-r--r--   0        0        0    11024 2024-05-10 00:27:14.907468 llama_tools-0.1.4/llama_tools/preprocess.py
+-rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.4/PKG-INFO
```

### Comparing `llama_tools-0.1.3/llama_tools/postprocess.py` & `llama_tools-0.1.4/llama_tools/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
         return []
     str_to_parse = output_str.split("<functions>")[1]
     list_of_str_to_parse = str_to_parse.splitlines()
     function_call_json = []
     try: # every function call has to be valid json
         for l in list_of_str_to_parse:
             fc = json.loads(l)
-            fc["arguments"] = json.dumps(fc["arguments"])
+            if type(fc["arguments"]) != str:
+                fc["arguments"] = json.dumps(fc["arguments"])
             function_call_json.append(fc)
     except Exception as e:
         print(f"Error : {e}")
     res = []
     for fc in function_call_json:
         res.append({
             "id": uuid.uuid4().hex[:8],
```

### Comparing `llama_tools-0.1.3/llama_tools/preprocess.py` & `llama_tools-0.1.4/llama_tools/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 import json
 
 
 TOOL_SYSTEM_PROMPT_RUBRA = (
-    "You have access to the following tools: {tool_text}\n"
+    "You have access to the following tools:\n {tool_text}\n"
     "You can choose to respond with one or more tool calls at once, or with a chat message back to the user. "
     "Ensure you have all necessary details before making tool calls. If additional information is needed, "
     "ask the user appropriately. Any tool call you make must correspond to the functions listed above.\n"
     "If you decide to call tools, format your response in JSONL. Start with the keyword `<functions>` followed by the JSON object:\n"
     '`<functions>{{"name": "<function_name>", "arguments": {{"<arg1_name>": "<arg1_value>", "<arg2_name>": "<arg2_value>", ...}}}}`'
 )
 
@@ -221,15 +221,15 @@
 
 def construct_tool_call_str(tool_calls, func_observation_map) -> str:
     tool_list = []
     for tool_call in tool_calls:
         tool_call_id = tool_call["id"]
         func_observation_map[tool_call_id] = ""  # Initialize with empty value, updated later from the message with tool role
         
-        tool_list.append(json.dumps(tool_call["function"]))
+        tool_list.append(str(tool_call["function"]))
 
     # Converting the Python dictionary to a YAML formatted string
     tool_call_str = "<functions>" + "\n".join(tool_list)
     return tool_call_str
 
 
 if __name__ == "__main__":
```

### Comparing `llama_tools-0.1.3/pyproject.toml` & `llama_tools-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.3/PKG-INFO` & `llama_tools-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Llama Tools: A collection of utilities for handling function calls with local llama.cpp models.
 Home-page: https://yourpackage.example.com
 License: MIT
 Keywords: llama, function-call
 Author: Yingbei Tong
 Author-email: yingbei@acorn.io
 Requires-Python: >=3.8
```

