# Comparing `tmp/llama_tools-0.1.4.tar.gz` & `tmp/llama_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_tools-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llama_tools-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llama_tools-0.1.4.tar` & `llama_tools-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.4/.gitignore
--rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.4/README.md
--rw-r--r--   0        0        0      314 2024-05-10 00:33:36.280975 llama_tools-0.1.4/llama_tools/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-10 00:22:41.202663 llama_tools-0.1.4/llama_tools/postprocess.py
--rw-r--r--   0        0        0    11024 2024-05-10 00:27:14.907468 llama_tools-0.1.4/llama_tools/preprocess.py
--rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.5/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.5/README.md
+-rw-r--r--   0        0        0      314 2024-05-10 00:48:36.154726 llama_tools-0.1.5/llama_tools/__init__.py
+-rw-r--r--   0        0        0     1722 2024-05-10 00:43:53.515042 llama_tools-0.1.5/llama_tools/postprocess.py
+-rw-r--r--   0        0        0    10968 2024-05-10 00:45:15.623041 llama_tools-0.1.5/llama_tools/preprocess.py
+-rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.5/PKG-INFO
```

### Comparing `llama_tools-0.1.4/llama_tools/postprocess.py` & `llama_tools-0.1.5/llama_tools/postprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import uuid
 from typing import List
 
 def postprocess_output(output_str: str) -> List[dict]:
     if not output_str.lstrip().startswith("<functions>"):
         return []
     str_to_parse = output_str.split("<functions>")[1]
-    list_of_str_to_parse = str_to_parse.splitlines()
+    list_of_str_to_parse = str_to_parse.splitlines() # TODO: need better way to handle jsonl format
     function_call_json = []
     try: # every function call has to be valid json
         for l in list_of_str_to_parse:
             fc = json.loads(l)
             if type(fc["arguments"]) != str:
                 fc["arguments"] = json.dumps(fc["arguments"])
             function_call_json.append(fc)
```

### Comparing `llama_tools-0.1.4/llama_tools/preprocess.py` & `llama_tools-0.1.5/llama_tools/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     func_observation_map = {}
     processed_msg = []
 
     for i in range(len(messages)):
         if messages[i]["role"] != "tool" and len(func_observation_map) > 0:
             # Insert the observation from the tool call before the next message
             func_observation_array = list(func_observation_map.values())
-            observation_str = "<<observation>>" + json.dumps(func_observation_array)
+            observation_str = json.dumps(func_observation_array)
             observation_call = {"role": "observation", "content": observation_str}
             processed_msg.append(observation_call)
             func_observation_map.clear()
 
         if i == 0:
             if messages[0]["role"] == "system":
                 old_content = messages[0]["content"]
@@ -207,15 +207,15 @@
 
         else:
             processed_msg.append(messages[i])
 
     if len(func_observation_map) > 0:
         # Insert the observation from the tool call before the next message
         func_observation_array = list(func_observation_map.values())
-        observation_str = "<<observation>>" + json.dumps(func_observation_array)
+        observation_str = json.dumps(func_observation_array)
         observation_call = {"role": "observation", "content": observation_str}
         processed_msg.append(observation_call)
         func_observation_map.clear()
 
     return processed_msg
 
 
@@ -224,15 +224,15 @@
     for tool_call in tool_calls:
         tool_call_id = tool_call["id"]
         func_observation_map[tool_call_id] = ""  # Initialize with empty value, updated later from the message with tool role
         
         tool_list.append(str(tool_call["function"]))
 
     # Converting the Python dictionary to a YAML formatted string
-    tool_call_str = "<functions>" + "\n".join(tool_list)
+    tool_call_str = "\n".join(tool_list)
     return tool_call_str
 
 
 if __name__ == "__main__":
     tools = [{"type": "function","function":{"name":"calculate_distance","description":"Calculate the distance between two locations","parameters":{"type":"object","properties":{"origin":{"type":"string","description":"The starting location"},"destination":{"type":"string","description":"The destination location"},"mode":{"type":"string","description":"The mode of transportation"}},"required":["origin","destination","mode"]}}},{"type": "function","function":{"name":"generate_password","description":"Generate a random password","parameters":{"type":"object","properties":{"length":{"type":"integer","description":"The length of the password"}},"required":["length"]}}}]
     msgs = [{'role': 'system', 'content': 'You are a helpful assistant.'}, {'role': 'user', 'content': 'What is the distance between San Francisco and Cupertino by driving and by air from both directions?'}, {'role': 'assistant', 'tool_calls': [{'id': '0', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San \nFrancisco","destination":"Cupertino","mode":"drive"}'}, 'type': 'function'},{'id': '1', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San \nFrancisco","destination":"Cupertino","mode":"air"}'}, 'type': 'function'}]}, {'role': 'tool', 'tool_call_id': '0', 'name': 'calculate_distance', 'content': 'Distance is 50 miles.'}, {'role': 'tool', 'tool_call_id': '1', 'name': 'calculate_distance', 'content': 'Distance  by air is 50 miles.'}]
     new_msgs = preprocess_input(msgs, tools)
```

### Comparing `llama_tools-0.1.4/pyproject.toml` & `llama_tools-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.4/PKG-INFO` & `llama_tools-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Llama Tools: A collection of utilities for handling function calls with local llama.cpp models.
 Home-page: https://yourpackage.example.com
 License: MIT
 Keywords: llama, function-call
 Author: Yingbei Tong
 Author-email: yingbei@acorn.io
 Requires-Python: >=3.8
```

