# Comparing `tmp/llama_tools-0.1.1.tar.gz` & `tmp/llama_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_tools-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llama_tools-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llama_tools-0.1.1.tar` & `llama_tools-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.1/.gitignore
--rw-r--r--   0        0        0       14 2024-05-05 21:16:20.830394 llama_tools-0.1.1/README.md
--rw-r--r--   0        0        0      314 2024-05-06 23:17:32.283476 llama_tools-0.1.1/llama_tools/__init__.py
--rw-r--r--   0        0        0      878 2024-05-06 23:15:54.920164 llama_tools-0.1.1/llama_tools/postprocess.py
--rw-r--r--   0        0        0    10624 2024-05-05 23:37:22.150376 llama_tools-0.1.1/llama_tools/preprocess.py
--rw-r--r--   0        0        0      600 2024-05-06 23:16:40.823015 llama_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 llama_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.2/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      314 2024-05-09 03:10:59.458216 llama_tools-0.1.2/llama_tools/__init__.py
+-rw-r--r--   0        0        0     1266 2024-05-09 03:05:39.781576 llama_tools-0.1.2/llama_tools/postprocess.py
+-rw-r--r--   0        0        0    11029 2024-05-09 01:00:53.061092 llama_tools-0.1.2/llama_tools/preprocess.py
+-rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.2/PKG-INFO
```

### Comparing `llama_tools-0.1.1/llama_tools/postprocess.py` & `llama_tools-0.1.2/llama_tools/postprocess.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import json
 import uuid
 from typing import List
 
 def postprocess_output(output_str: str) -> List[dict]:
-    if not output_str.lstrip().startswith("<<functions>>"):
-        return []
-    str_to_parse = output_str.split("<<functions>>")[1]
-    try:
-        function_call_json = json.loads(str_to_parse)
-    except:
+    if not output_str.lstrip().startswith("<functions>"):
         return []
+    str_to_parse = output_str.split("<functions>")[1]
+    list_of_str_to_parse = str_to_parse.splitlines()
+    function_call_json = []
+    try: # every function call has to be valid json
+        for l in list_of_str_to_parse:
+            function_call_json.append(json.loads(l))
+    except Exception as e:
+        print(e)
     res = []
     for fc in function_call_json:
         res.append({
             "id": uuid.uuid4().hex[:8],
             "function": fc,
             "type": "function",
         })
     return res
 
 if __name__ == "__main__":
-    output_str = "<<functions>>[{\"name\": \"calculate_distance\", \"arguments\": \"{\\\"origin\\\":\\\"San Francisco\\\",\\\"destination\\\":\\\"Cupertino\\\",\\\"mode\\\":\\\"drive\\\"}\"}]"
+    output_str = "<functions>{\"name\": \"calculate_distance\", \"arguments\": \"{\\\"origin\\\":\\\"San \\nFrancisco\\\",\\\"destination\\\":\\\"Cupertino\\\",\\\"mode\\\":\\\"drive\\\"}\"}\n{\"name\": \"calculate_distance\", \"arguments\": \"{\\\"origin\\\":\\\"San \\nFrancisco\\\",\\\"destination\\\":\\\"Cupertino\\\",\\\"mode\\\":\\\"air\\\"}\"}"
     parsed_json = postprocess_output(output_str)
     if parsed_json:
+        print(f"PARSED_JSON type: {type(parsed_json)}")
         print(parsed_json)
     else :
         print(output_str)
```

### Comparing `llama_tools-0.1.1/llama_tools/preprocess.py` & `llama_tools-0.1.2/llama_tools/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import List
 import json
 
 
 TOOL_SYSTEM_PROMPT_RUBRA = (
-    "You have access to the following tools:\n{tool_text}"
-    "Use the following format if using a tool:\n<<functions>>[toolname1(arg1=value1, arg2=value2, ...), toolname2(arg1=value1, arg2=value2, ...)]"
-    "You can choose to respond with 1 or more tool calls at once, or with a chat message back to the user. Only make tool calls once you have all the details to fill in the required params. Feel free to ask the user for more info when appropriate. Any tool call you make must match the name of a function(s) provided above."
+    "You have access to the following tools: {tool_text}\n"
+    "You can choose to respond with one or more tool calls at once, or with a chat message back to the user. "
+    "Ensure you have all necessary details before making tool calls. If additional information is needed, "
+    "ask the user appropriately. Any tool call you make must correspond to the functions listed above.\n"
+    "If you decide to call tools, format your response in JSONL. Start with the keyword `<functions>` followed by the JSON object:\n"
+    '`<functions>{{"name": "<function_name>", "arguments": {{"<arg1_name>": "<arg1_value>", "<arg2_name>": "<arg2_value>", ...}}}}`'
 )
 
 def json_schema_to_typescript_type(schema, param_name):
     ts_type = "any"  # default type
     enum_comment = ""
     integer_comment = ""
     description_comment = ""
@@ -218,20 +221,20 @@
 
 def construct_tool_call_str(tool_calls, func_observation_map) -> str:
     tool_list = []
     for tool_call in tool_calls:
         tool_call_id = tool_call["id"]
         func_observation_map[tool_call_id] = ""  # Initialize with empty value, updated later from the message with tool role
         
-        tool_list.append(tool_call["function"])
+        tool_list.append(json.dumps(tool_call["function"]))
 
     # Converting the Python dictionary to a YAML formatted string
-    tool_call_str = "<<functions>>" + json.dumps(tool_list)
+    tool_call_str = "<functions>" + "\n".join(tool_list)
     return tool_call_str
 
 
 if __name__ == "__main__":
     tools = [{"type": "function","function":{"name":"calculate_distance","description":"Calculate the distance between two locations","parameters":{"type":"object","properties":{"origin":{"type":"string","description":"The starting location"},"destination":{"type":"string","description":"The destination location"},"mode":{"type":"string","description":"The mode of transportation"}},"required":["origin","destination","mode"]}}},{"type": "function","function":{"name":"generate_password","description":"Generate a random password","parameters":{"type":"object","properties":{"length":{"type":"integer","description":"The length of the password"}},"required":["length"]}}}]
-    msgs = [{'role': 'system', 'content': 'You are a helpful assistant.'}, {'role': 'user', 'content': 'What is the distance between San Francisco and Cupertino by driving and by air from both directions?'}, {'role': 'assistant', 'tool_calls': [{'id': '0', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San Francisco","destination":"Cupertino","mode":"drive"}'}, 'type': 'function'}]}, {'role': 'tool', 'tool_call_id': '0', 'name': 'calculate_distance', 'content': 'Distance is 50 miles.'}]
+    msgs = [{'role': 'system', 'content': 'You are a helpful assistant.'}, {'role': 'user', 'content': 'What is the distance between San Francisco and Cupertino by driving and by air from both directions?'}, {'role': 'assistant', 'tool_calls': [{'id': '0', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San \nFrancisco","destination":"Cupertino","mode":"drive"}'}, 'type': 'function'},{'id': '1', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San \nFrancisco","destination":"Cupertino","mode":"air"}'}, 'type': 'function'}]}, {'role': 'tool', 'tool_call_id': '0', 'name': 'calculate_distance', 'content': 'Distance is 50 miles.'}, {'role': 'tool', 'tool_call_id': '1', 'name': 'calculate_distance', 'content': 'Distance  by air is 50 miles.'}]
     new_msgs = preprocess_input(msgs, tools)
     print(json.dumps(new_msgs, indent=2))
```

