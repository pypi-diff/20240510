# Comparing `tmp/llama_tools-0.1.2.tar.gz` & `tmp/llama_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_tools-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llama_tools-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llama_tools-0.1.2.tar` & `llama_tools-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.2/.gitignore
--rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.2/README.md
--rw-r--r--   0        0        0      314 2024-05-09 03:10:59.458216 llama_tools-0.1.2/llama_tools/__init__.py
--rw-r--r--   0        0        0     1266 2024-05-09 03:05:39.781576 llama_tools-0.1.2/llama_tools/postprocess.py
--rw-r--r--   0        0        0    11029 2024-05-09 01:00:53.061092 llama_tools-0.1.2/llama_tools/preprocess.py
--rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.3/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      314 2024-05-09 22:16:44.058649 llama_tools-0.1.3/llama_tools/__init__.py
+-rw-r--r--   0        0        0     1626 2024-05-09 22:16:03.483726 llama_tools-0.1.3/llama_tools/postprocess.py
+-rw-r--r--   0        0        0    11029 2024-05-09 01:00:53.061092 llama_tools-0.1.3/llama_tools/preprocess.py
+-rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.3/PKG-INFO
```

### Comparing `llama_tools-0.1.2/llama_tools/postprocess.py` & `llama_tools-0.1.3/llama_tools/postprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,30 @@
     if not output_str.lstrip().startswith("<functions>"):
         return []
     str_to_parse = output_str.split("<functions>")[1]
     list_of_str_to_parse = str_to_parse.splitlines()
     function_call_json = []
     try: # every function call has to be valid json
         for l in list_of_str_to_parse:
-            function_call_json.append(json.loads(l))
+            fc = json.loads(l)
+            fc["arguments"] = json.dumps(fc["arguments"])
+            function_call_json.append(fc)
     except Exception as e:
-        print(e)
+        print(f"Error : {e}")
     res = []
     for fc in function_call_json:
         res.append({
             "id": uuid.uuid4().hex[:8],
             "function": fc,
             "type": "function",
         })
     return res
 
 if __name__ == "__main__":
-    output_str = "<functions>{\"name\": \"calculate_distance\", \"arguments\": \"{\\\"origin\\\":\\\"San \\nFrancisco\\\",\\\"destination\\\":\\\"Cupertino\\\",\\\"mode\\\":\\\"drive\\\"}\"}\n{\"name\": \"calculate_distance\", \"arguments\": \"{\\\"origin\\\":\\\"San \\nFrancisco\\\",\\\"destination\\\":\\\"Cupertino\\\",\\\"mode\\\":\\\"air\\\"}\"}"
+    # output_str = "<functions>{\"name\": \"calculate_distance\", \"arguments\": \"{\\\"origin\\\":\\\"San \\nFrancisco\\\",\\\"destination\\\":\\\"Cupertino\\\",\\\"mode\\\":\\\"drive\\\"}\"}\n{\"name\": \"calculate_distance\", \"arguments\": \"{\\\"origin\\\":\\\"San \\nFrancisco\\\",\\\"destination\\\":\\\"Cupertino\\\",\\\"mode\\\":\\\"air\\\"}\"}"
+    output_str = '<functions>{"name": "calculate_distance", "arguments": {"origin": "San Francisco", "destination": "Cupertino", "mode": "driving"}}\n{"name": "calculate_distance", "arguments": {"origin": "San Francisco", "destination": "Cupertino", "mode": "air"}}'
     parsed_json = postprocess_output(output_str)
     if parsed_json:
         print(f"PARSED_JSON type: {type(parsed_json)}")
         print(parsed_json)
     else :
         print(output_str)
```

### Comparing `llama_tools-0.1.2/llama_tools/preprocess.py` & `llama_tools-0.1.3/llama_tools/preprocess.py`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.2/pyproject.toml` & `llama_tools-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.2/PKG-INFO` & `llama_tools-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Llama Tools: A collection of utilities for handling function calls with local llama.cpp models.
 Home-page: https://yourpackage.example.com
 License: MIT
 Keywords: llama, function-call
 Author: Yingbei Tong
 Author-email: yingbei@acorn.io
 Requires-Python: >=3.8
```

