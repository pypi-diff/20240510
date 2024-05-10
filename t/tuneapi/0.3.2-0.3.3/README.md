# Comparing `tmp/tuneapi-0.3.2.tar.gz` & `tmp/tuneapi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.3.2.tar", max compression
+gzip compressed data, was "tuneapi-0.3.3.tar", max compression
```

## Comparing `tuneapi-0.3.2.tar` & `tuneapi-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.3.2/LICENSE
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.3.2/README.md
--rw-r--r--   0        0        0      712 2024-05-09 10:06:02.984896 tuneapi-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       78 2024-05-09 10:06:05.825963 tuneapi-0.3.2/tuneapi/__init__.py
--rw-r--r--   0        0        0      291 2024-04-23 00:52:16.205178 tuneapi-0.3.2/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6883 2024-05-09 10:05:18.103132 tuneapi-0.3.2/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     3159 2024-04-25 05:37:07.370133 tuneapi-0.3.2/tuneapi/apis/model_groq.py
--rw-r--r--   0        0        0     3177 2024-04-18 21:08:27.197387 tuneapi-0.3.2/tuneapi/apis/model_mistral.py
--rw-r--r--   0        0        0     6328 2024-04-26 00:29:23.039606 tuneapi-0.3.2/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5822 2024-04-22 20:41:11.558482 tuneapi-0.3.2/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0     3714 2024-04-23 01:23:26.207221 tuneapi-0.3.2/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-04-25 04:12:26.606262 tuneapi-0.3.2/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    15414 2024-04-24 21:00:11.105695 tuneapi-0.3.2/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1076 2024-05-06 20:32:10.727462 tuneapi-0.3.2/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.3.2/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2942 2024-05-06 20:31:58.365454 tuneapi-0.3.2/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.3.2/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.3.2/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.3.2/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.3.2/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4846 2024-04-25 22:30:49.313201 tuneapi-0.3.2/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0     1154 2024-04-30 05:41:11.504281 tuneapi-0.3.2/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.3.2/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5772 2024-04-23 00:48:09.361152 tuneapi-0.3.2/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.3.2/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 tuneapi-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.3.3/LICENSE
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.3.3/README.md
+-rw-r--r--   0        0        0      712 2024-05-10 05:33:00.755395 tuneapi-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-05-10 05:33:03.565847 tuneapi-0.3.3/tuneapi/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-23 00:52:16.205178 tuneapi-0.3.3/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6965 2024-05-10 05:19:42.218444 tuneapi-0.3.3/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     3159 2024-04-25 05:37:07.370133 tuneapi-0.3.3/tuneapi/apis/model_groq.py
+-rw-r--r--   0        0        0     3177 2024-04-18 21:08:27.197387 tuneapi-0.3.3/tuneapi/apis/model_mistral.py
+-rw-r--r--   0        0        0     6328 2024-04-26 00:29:23.039606 tuneapi-0.3.3/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5822 2024-04-22 20:41:11.558482 tuneapi-0.3.3/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0     3714 2024-04-23 01:23:26.207221 tuneapi-0.3.3/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-04-25 04:12:26.606262 tuneapi-0.3.3/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    15414 2024-04-24 21:00:11.105695 tuneapi-0.3.3/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1076 2024-05-06 20:32:10.727462 tuneapi-0.3.3/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.3.3/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2942 2024-05-06 20:31:58.365454 tuneapi-0.3.3/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.3.3/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.3.3/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.3.3/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.3.3/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4846 2024-04-25 22:30:49.313201 tuneapi-0.3.3/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0     1154 2024-04-30 05:41:11.504281 tuneapi-0.3.3/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.3.3/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5772 2024-04-23 00:48:09.361152 tuneapi-0.3.3/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.3.3/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 tuneapi-0.3.3/PKG-INFO
```

### Comparing `tuneapi-0.3.2/LICENSE` & `tuneapi-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/pyproject.toml` & `tuneapi-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.3.2"
+version = "0.3.3"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.3.2/tuneapi/apis/model_anthropic.py` & `tuneapi-0.3.3/tuneapi/apis/model_anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,22 +67,25 @@
         # create the anthropic style data
         system = ""
         claude_messages = []
         if messages[0]["role"] == Message.SYSTEM:
             system_message = messages.pop(0)
             system = system_message["content"]
         for m in messages:
+            # correct the role
             role = m["role"]
             if m["role"] == Message.HUMAN:
                 role = "user"
+            elif m["role"] == Message.GPT:
+                role = "assistant"
+
+            # correct content
             content = m["content"]
             if type(content) == str:
                 content = [{"type": "text", "text": content.strip()}]
-            elif m["role"] == Message.GPT:
-                role = "assistant"
             claude_messages.append(
                 {
                     "role": role,
                     "content": content,
                 }
             )
 
@@ -143,15 +146,15 @@
         self,
         chats: Thread | str,
         tools: Optional[List] = None,
         model: Optional[str] = None,
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
-        timeout=(5, 60),
+        timeout=(5, 30),
         raw: bool = False,
         **kwargs,
     ) -> Any:
         headers, system, claude_messages = self._process_input(
             chats=chats,
             tools=tools,
             token=token,
@@ -193,17 +196,17 @@
                                 {
                                     "choices": [
                                         {"delta": {"content": resp["delta"]["text"]}}
                                     ]
                                 },
                                 tight=True,
                             )
-                        ).encode()
+                        ).encode() + b"\r\n"
                 except:
-                    yield line.encode()
+                    yield line.encode() + b"\r\n"
                 continue
 
             # return token
             try:
                 resp = json.loads(line.replace("data:", "").strip())
                 if "delta" in resp:
                     yield resp["delta"]["text"]
```

### Comparing `tuneapi-0.3.2/tuneapi/apis/model_groq.py` & `tuneapi-0.3.3/tuneapi/apis/model_groq.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/apis/model_mistral.py` & `tuneapi-0.3.3/tuneapi/apis/model_mistral.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/apis/model_openai.py` & `tuneapi-0.3.3/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/apis/model_tune.py` & `tuneapi-0.3.3/tuneapi/apis/model_tune.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/apis/threads.py` & `tuneapi-0.3.3/tuneapi/apis/threads.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/types/chats.py` & `tuneapi-0.3.3/tuneapi/types/chats.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/__init__.py` & `tuneapi-0.3.3/tuneapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/fs.py` & `tuneapi-0.3.3/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/logger.py` & `tuneapi-0.3.3/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/mime.py` & `tuneapi-0.3.3/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/misc.py` & `tuneapi-0.3.3/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/networking.py` & `tuneapi-0.3.3/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/parallel.py` & `tuneapi-0.3.3/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/randomness.py` & `tuneapi-0.3.3/tuneapi/utils/randomness.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/serdeser.py` & `tuneapi-0.3.3/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/subway.py` & `tuneapi-0.3.3/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/tuneapi/utils/terminal.py` & `tuneapi-0.3.3/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.2/PKG-INFO` & `tuneapi-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: MIT
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

