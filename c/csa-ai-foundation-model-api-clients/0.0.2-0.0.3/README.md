# Comparing `tmp/csa_ai_foundation_model_api_clients-0.0.2.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.0.3.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.0.2.tar` & `csa_ai_foundation_model_api_clients-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,17 @@
--rwxr-xr-x   0        0        0      210 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/manual-package-update.md
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/__init__.py
--rwxr-xr-x   0        0        0     3802 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/foundation_model_api_clients.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3178 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2690 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/claude.py
--rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/gemini.py
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     4081 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2515 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      574 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/tests/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      568 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/tests/ask-claude-the-capital-of-france.py~
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/LICENSE
--rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/README.md
--rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/manual-package-update.md
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     4081 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2515 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/tests/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/tests/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/tests/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/README.md
+-rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 
-import argparse
 import os
+import argparse
 import json
 from ai_client import claude, chatgpt, gemini
 
 class FoundationModelAPIClient:
-    def __init__(self, model_name):
+    def __init__(self, model_name, api_key=None):
         self.model_name = model_name
-        self.api_key = self.get_model_api_key()
+        self.api_key = api_key or self.get_model_api_key()
         self.model_mapping = self.get_model_mapping()
 
     def get_model_mapping(self):
         model_mapping = {
             'chatgpt': 'gpt-4-turbo-preview',
             'claude': 'claude-3-opus-20240229',
             'claude-haiku': 'claude-3-haiku-20240307',
@@ -33,25 +33,31 @@
         }
         api_key_env = model_api_key.get(self.model_name, model_api_key)
         api_key = os.getenv(api_key_env)
         if not api_key:
             raise ValueError("API KEY environment variable not set.")
         return api_key
 
-    def generate_response(self, system_prompt, user_prompt, user_data, args):
+    def generate_response(self, system_prompt, user_prompt, user_data=None, output_file=None, **kwargs):
         user_prompt_full = self.prepare_prompt(user_prompt, user_data)
         if self.model_name.startswith('claude'):
-            return claude.generate_response(self.model_mapping, self.api_key, system_prompt, user_prompt_full, args)
+            response = claude.generate_response(self.model_mapping, self.api_key, system_prompt, user_prompt_full, **kwargs)
         elif self.model_name.startswith('chatgpt'):
-            return chatgpt.generate_response(self.model_mapping, self.api_key, system_prompt, user_prompt_full, args)
+            response = chatgpt.generate_response(self.model_mapping, self.api_key, system_prompt, user_prompt_full, **kwargs)
         elif self.model_name.startswith('gemini'):
-            return gemini.generate_response(self.model_mapping, self.api_key, system_prompt, user_prompt_full, args)
+            response = gemini.generate_response(self.model_mapping, self.api_key, system_prompt, user_prompt_full, **kwargs)
         else:
             raise ValueError(f"Unsupported model: {self.model_name}")
 
+        if output_file:
+            with open(output_file, 'w') as file:
+                json.dump(response, file, indent=2)
+
+        return response
+
     def prepare_prompt(self, user_prompt, user_data):
         if user_data:
             return f"{user_prompt}\n{user_data}"
         return user_prompt
 
 def main():
     parser = argparse.ArgumentParser(description='AI Model Client')
@@ -69,14 +75,14 @@
     with open(args.system_prompt, 'r', encoding='utf-8') as file:
         system_prompt = file.read().strip()
     with open(args.user_prompt, 'r', encoding='utf-8') as file:
         user_prompt = file.read().strip()
     with open(args.user_data, 'r', encoding='utf-8') as file:
         user_data = file.read().strip()
 
-    response = client.generate_response(system_prompt, user_prompt, user_data, args)
+    response = client.generate_response(system_prompt, user_prompt, user_data, temperature=args.temperature, max_tokens=args.max_tokens)
     
     with open(args.output_file, 'w', encoding='utf-8') as file:
         json.dump(response, file, sort_keys=True, indent=2)
 
 if __name__ == '__main__':
     main()
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 #!/usr/bin/env python3
 
-# Weird spacing so all three files line up in an editor
-
 import openai
-
-
 import datetime
 
-def generate_response(model_name, api_key, system_prompt, user_prompt, args):
-
+def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
     TIME_START = datetime.datetime.now().isoformat()
 
-    #
-    # OpenAI ChatGPT API: https://platform.openai.com/docs/api-reference
-    #
-
     openai.api_key = api_key
 
+    temperature = kwargs.get('temperature', 1)
+    max_tokens = kwargs.get('max_tokens', 4096)
+
     completion = openai.chat.completions.create(
         model=model_name,
-        temperature=args.temperature,
-        max_tokens=args.max_tokens,
+        temperature=temperature,
+        max_tokens=max_tokens,
         messages=[
             {"role": "system", "content": system_prompt},
             {"role": "user", "content": user_prompt}
         ]
     )
 
-
-
-
     TIME_FINISHED = datetime.datetime.now().isoformat()
 
     time_start = datetime.datetime.fromisoformat(TIME_START)
     time_complete = datetime.datetime.fromisoformat(TIME_FINISHED)
 
-    # Calculate the duration
     duration = time_complete - time_start
     TIME_TO_RUN = duration.total_seconds()
 
     try:
         tokens_input = completion.usage.prompt_tokens
         tokens_output = completion.usage.completion_tokens
         total_tokens = completion.usage.total_tokens
@@ -72,30 +62,28 @@
         response_message = completion.choices[0].message.content
     except AttributeError:
         response_message = None
 
     ai_output = {
         "$id": "csa-ai-toolkit-openai-chatgpt4-JSON-v1_00",
         "metadata": {
-            "system": args.system_prompt,
-            "user-prompt": args.user_prompt,
-            "user-data": args.user_data,
-            "output": args.output_file,                        
+            "system": system_prompt,
+            "user-prompt": user_prompt,
+            "user-data": kwargs.get('user_data'),
+            "output": kwargs.get('output_file'),                        
             "model_name": model_name,
-            "temperature": args.temperature,
-            "max_tokens": args.max_tokens,
+            "temperature": temperature,
+            "max_tokens": max_tokens,
             "tokens_input": tokens_input,
             "tokens_output": tokens_output,
             "tokens_total": total_tokens,
             "time_start": TIME_START,
             "time_complete": TIME_FINISHED,
             "time_to_run": TIME_TO_RUN
         },
         "extracted_data": response_message,
         "completion": serialized_completion
     }
 
-    ai_output.update(vars(args))  # Merging argparse arguments
-
     ai_output = {key: value for key, value in ai_output.items() if value is not None}
 
-    return ai_output#
+    return ai_output
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 #!/usr/bin/env python3
 
-# Weird spacing so all three files line up in an editor
-
 import anthropic
-
-
 import datetime
 
-def generate_response(model_name, api_key, system_prompt, user_prompt, args):
-
+def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
     TIME_START = datetime.datetime.now().isoformat()
 
-    #
-    # Anthropic Claude API: https://docs.anthropic.com/claude/reference/messages_post
-    #
-        
     client = anthropic.Anthropic(api_key=api_key)
 
+    temperature = kwargs.get('temperature', 1)
+    max_tokens = kwargs.get('max_tokens', 4096)
+
     completion = client.messages.create(
         model=model_name,        
-        temperature=args.temperature,
-        max_tokens=args.max_tokens,
+        temperature=temperature,
+        max_tokens=max_tokens,
         system=system_prompt,
         messages=[
             {"role": "user", "content": user_prompt}
         ],
     )
 
-
-
-
     TIME_FINISHED = datetime.datetime.now().isoformat()
 
     time_start = datetime.datetime.fromisoformat(TIME_START)
     time_complete = datetime.datetime.fromisoformat(TIME_FINISHED)
 
-    # Calculate the duration
     duration = time_complete - time_start
     TIME_TO_RUN = duration.total_seconds()
 
     try:
         tokens_input = completion.usage.input_tokens
         tokens_output = completion.usage.output_tokens
         total_tokens = completion.usage.input_tokens + completion.usage.output_tokens
@@ -61,30 +51,28 @@
         response_message = completion.content[0].text
     except AttributeError:
         response_message = None
 
     ai_output = {
         "$id": "csa-ai-toolkit-anthropic-claude3-JSON-v1_00",
         "metadata": {
-            "system": args.system_prompt,
-            "user-prompt": args.user_prompt,
-            "user-data": args.user_data,
-            "output": args.output_file,                        
+            "system": system_prompt,
+            "user-prompt": user_prompt,
+            "user-data": kwargs.get('user_data'),
+            "output": kwargs.get('output_file'),                        
             "model_name": model_name,
-            "temperature": args.temperature,
-            "max_tokens": args.max_tokens,
+            "temperature": temperature,
+            "max_tokens": max_tokens,
             "tokens_input": tokens_input,
             "tokens_output": tokens_output,
             "tokens_total": total_tokens,
             "time_start": TIME_START,
             "time_complete": TIME_FINISHED,
             "time_to_run": TIME_TO_RUN
         },
         "extracted_data": response_message,
         "completion": serialized_completion
     }
 
-    ai_output.update(vars(args))  # Merging argparse arguments
-
     ai_output = {key: value for key, value in ai_output.items() if value is not None}
 
     return ai_output
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 #!/usr/bin/env python3
 
-# Weird spacing so all three files line up in an editor
-
 import google.generativeai as genai
 from google.generativeai import types
-
 import datetime
 
-def generate_response(model_name, api_key, system_prompt, user_prompt, args):
-
+def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
     TIME_START = datetime.datetime.now().isoformat()
 
-    #
-    # Google Gemini Python: https://ai.google.dev/gemini-api/docs/get-started/python
-    #
-
     genai.configure(api_key=api_key)
 
     gemini_model = genai.GenerativeModel(
         model_name=model_name,
         system_instruction=system_prompt
         )
 
+    temperature = kwargs.get('temperature', 1)
+    max_tokens = kwargs.get('max_tokens', 4096)
+
     config = types.GenerationConfig(
         candidate_count=1,
-        max_output_tokens=args.max_tokens,
-        temperature=args.temperature
+        max_output_tokens=max_tokens,
+        temperature=temperature
     )
 
     response = gemini_model.generate_content(user_prompt, generation_config=config)
 
     TIME_FINISHED = datetime.datetime.now().isoformat()
 
     time_start = datetime.datetime.fromisoformat(TIME_START)
     time_complete = datetime.datetime.fromisoformat(TIME_FINISHED)
 
-    # Calculate the duration
     duration = time_complete - time_start
     TIME_TO_RUN = duration.total_seconds()
 
     ai_output = {
         "$id": "csa-ai-toolkit-google-gemini1.5-JSON-v1_00",
         "metadata": {
-            "system": args.system_prompt,
-            "user-prompt": args.user_prompt,
-            "user-data": args.user_data,
-            "output": args.output_file,
+            "system": system_prompt,
+            "user-prompt": user_prompt,
+            "user-data": kwargs.get('user_data'),
+            "output": kwargs.get('output_file'),
             "model_name": model_name,
-            "temperature": args.temperature,
-            "max_tokens": args.max_tokens,
+            "temperature": temperature,
+            "max_tokens": max_tokens,
             "time_start": TIME_START,
             "time_complete": TIME_FINISHED,
             "time_to_run": TIME_TO_RUN
         },
-        #"response": response,
         "extracted_data": response.text
     }
 
-    ai_output.update(vars(args))  # Merging argparse arguments
     ai_output = {key: value for key, value in ai_output.items() if value is not None}
 
-    return ai_output
+    return ai_output
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/tests/ask-claude-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.0.3/tests/ask-gemini-the-capital-of-france.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 
 from foundation_model_api_clients import FoundationModelAPIClient
 
 def main():
-    model_name = 'claude'
-
+    model_name = 'gemini'
+    
     client = FoundationModelAPIClient(model_name)
 
     system_prompt = "You are a helpful assistant."
     user_prompt = "What is the capital of France?"
     user_data = None
-    output_file = 'response.json'
+    output_file = 'gemini-response.json'
 
     response = client.generate_response(
         system_prompt,
         user_prompt,
         user_data,
         temperature=0.7,
         max_tokens=100,
         output_file=output_file
     )
 
 if __name__ == '__main__':
     main()
-
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/tests/ask-claude-the-capital-of-france.py~` & `csa_ai_foundation_model_api_clients-0.0.3/tests/ask-claude-the-capital-of-france.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 #!/usr/bin/env python3
 
-
-
 from foundation_model_api_clients import FoundationModelAPIClient
 
 def main():
     model_name = 'claude'
-
+    
     client = FoundationModelAPIClient(model_name)
 
     system_prompt = "You are a helpful assistant."
     user_prompt = "What is the capital of France?"
     user_data = None
-    output_file = 'response.json'
-    
+    output_file = 'claude-response.json'
+
     response = client.generate_response(
         system_prompt,
         user_prompt,
         user_data,
         temperature=0.7,
-        max_tokens=100
+        max_tokens=100,
+        output_file=output_file
     )
 
-    print(response)
-
 if __name__ == '__main__':
     main()
-
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/.gitignore` & `csa_ai_foundation_model_api_clients-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/LICENSE` & `csa_ai_foundation_model_api_clients-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.2/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "anthropic",
+  "google-generativeai",
+  "openai",
+]
 
 [project.urls]
 Homepage = "https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients"
 Issues = "https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues"
```

