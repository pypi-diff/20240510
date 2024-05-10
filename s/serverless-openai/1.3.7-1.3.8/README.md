# Comparing `tmp/serverless_openai-1.3.7.tar.gz` & `tmp/serverless_openai-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverless_openai-1.3.7.tar", last modified: Tue Apr 23 11:30:45 2024, max compression
+gzip compressed data, was "serverless_openai-1.3.8.tar", last modified: Fri May 10 09:16:06 2024, max compression
```

## Comparing `serverless_openai-1.3.7.tar` & `serverless_openai-1.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:30:45.400760 serverless_openai-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 11:30:45.396760 serverless_openai-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:30:41.000000 serverless_openai-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:30:45.396760 serverless_openai-1.3.7/serverless_openai/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 11:30:41.000000 serverless_openai-1.3.7/serverless_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-23 11:30:41.000000 serverless_openai-1.3.7/serverless_openai/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-23 11:30:41.000000 serverless_openai-1.3.7/serverless_openai/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:30:45.396760 serverless_openai-1.3.7/serverless_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 11:30:45.000000 serverless_openai-1.3.7/serverless_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 11:30:45.000000 serverless_openai-1.3.7/serverless_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:30:45.000000 serverless_openai-1.3.7/serverless_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 11:30:45.000000 serverless_openai-1.3.7/serverless_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 11:30:45.000000 serverless_openai-1.3.7/serverless_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:30:45.400760 serverless_openai-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 11:30:41.000000 serverless_openai-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:06.511249 serverless_openai-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 09:16:06.511249 serverless_openai-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 09:16:00.000000 serverless_openai-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:06.507249 serverless_openai-1.3.8/serverless_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 09:16:00.000000 serverless_openai-1.3.8/serverless_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-05-10 09:16:00.000000 serverless_openai-1.3.8/serverless_openai/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-10 09:16:00.000000 serverless_openai-1.3.8/serverless_openai/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:06.511249 serverless_openai-1.3.8/serverless_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 09:16:06.000000 serverless_openai-1.3.8/serverless_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 09:16:06.000000 serverless_openai-1.3.8/serverless_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:16:06.000000 serverless_openai-1.3.8/serverless_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 09:16:06.000000 serverless_openai-1.3.8/serverless_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 09:16:06.000000 serverless_openai-1.3.8/serverless_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:16:06.511249 serverless_openai-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 09:16:00.000000 serverless_openai-1.3.8/setup.py
```

### Comparing `serverless_openai-1.3.7/PKG-INFO` & `serverless_openai-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.7
+Version: 1.3.8
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.7/serverless_openai/apis.py` & `serverless_openai-1.3.8/serverless_openai/apis.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     class Config:  
         use_enum_values = True
     
     def chat_completion(
             self, 
             messages: Messages,
-            model: Union[TextCompletionModels, str] = TextCompletionModels.gpt4_0125,
+            model: Union[TextCompletionModels, str] = TextCompletionModels.gpt4_turbo,
             tries: int = 5,
             timeout: int = 500,
             temperature: Optional[float] = 1,
             frequency_penalty: Optional[float] = 0,
             # logit_bias: Union[str, None] = None,
             logit_bias: Optional[str] = None,
             logprobs: Optional[bool] = False,
@@ -183,15 +183,15 @@
                 return OpenAIResults(result=results['data'][0]['b64_json'], result_json=results)
             return OpenAIResults(result=results['data'][0]['url'], result_json=results)
         return OpenAIResults(result=False, result_json=results)
     
     def vision(
             self,
             messages: VisionMessage,
-            model: Union[VisionModels, str] = VisionModels.gpt4_vision,
+            model: Union[VisionModels, str] = VisionModels.gpt4_turbo,
             tries: int = 5,
             timeout: int = 500,
             temperature: Optional[float] = 1,
             max_tokens: Optional[int] = 1024,
         ) -> OpenAIResults:
 
         newm = [
@@ -228,19 +228,19 @@
             except Exception as e:
                 print("ERROR:", e)
         return OpenAIResults(result=False, result_json=res)
     
     def vision_longimage(
             self,
             messages: VisionMessage,
-            model: Union[VisionModels, str] = VisionModels.gpt4_vision,
+            model: Union[VisionModels, str] = VisionModels.gpt4_turbo,
             tries: int = 5,
             timeout: int = 500,
             temperature: Optional[float] = 1,
-            max_tokens: Optional[int] = 1024,
+            max_tokens: Optional[int] = 1024
         ) -> OpenAIResults:
         
         if isinstance(messages.image, list):
             img_b64_list = []
             for img in messages.image:
                 if 'data:image/jpeg;base64' in img:
                     image_np = b64_to_np(img)
@@ -293,14 +293,101 @@
                 res = requests.post(self.completion_url, headers=self.headers, json=data, timeout=timeout).json()
                 if 'choices' in res:
                     message = res['choices'][0]['message']
                     return OpenAIResults(result=message['content'], result_json=res)
             except Exception as e:
                 print("ERROR:", e)
         return OpenAIResults(result=False, result_json=res)
+    
+    def vision_tools(
+            self,
+            messages: VisionMessage,
+            model: Union[VisionModels, str] = VisionModels.gpt4_turbo,
+            tries: int = 5,
+            timeout: int = 500,
+            temperature: Optional[float] = 1,
+            max_tokens: Optional[int] = 1024,
+            tools: Optional[List[dict]] = None,
+            tool_choice: Optional[str] = None,
+            response_format: Optional[dict] = {"type": "json_object"},
+        ) -> OpenAIResults:
+
+        if isinstance(messages.image, list):
+            img_b64_list = []
+            for img in messages.image:
+                try:
+                    TypeAdapter(HttpUrl).validate_python(img)
+                    img_b64_list.append(img)
+                except:
+                    if 'data:image/jpeg;base64' in img:
+                        image_np = b64_to_np(img)
+                    else:
+                        image_np = urlimage_to_np(img)
+                    img_b64_list.extend(crop_image(image_np))
+
+        elif isinstance(messages.image, str):
+            if 'data:image/jpeg;base64' in messages.image:
+                image_np = b64_to_np(messages.image)
+            else:
+                image_np = urlimage_to_np(messages.image)
+            img_b64_list = crop_image(image_np)
+
+        elif isinstance(messages.image, np.ndarray):
+            image_np = messages.image
+            img_b64_list = crop_image(image_np)
+            
+        newm = [
+            {
+                "role": messages.role,
+                "content": [
+                    {
+                        "type": "text",
+                        "text": messages.text
+                    },
+                ]
+            }
+        ]
+        for b64 in img_b64_list:
+            newm[0]['content'].append(
+                {
+                    "type": "image_url",
+                    "image_url": {
+                        "url": b64,
+                        "detail": "high"
+                    }
+                }
+            )
+
+        data = {
+            "model": model,
+            "messages": newm,
+            "temperature": temperature,
+        }
+
+        if max_tokens:
+            data['max_tokens'] = max_tokens
+
+        if tool_choice:
+            data["response_format"] = response_format
+            data["tools"] = tools
+            data["tool_choice"] = {"type": "function", "function": {"name": tool_choice}}
+
+        results = {}
+        for _ in range(tries):
+            try:
+                results = requests.post(self.completion_url, headers=self.headers, json=data, timeout=timeout).json()
+                if 'choices' in results:
+                    res = results['choices'][0]['message']
+                    res_json = json.loads(res['tool_calls'][0]['function']['arguments'], strict=False)
+                    return OpenAIResults(result=res_json, result_json=results)
+                else:
+                    print("RESULTS:", results)
+            except Exception as e:
+                print("ERROR:", e)
+        return OpenAIResults(result=False, result_json=results)
 
     def embeddings(
             self,
             prompt: EmbeddingPrompts,
             model: EmbeddingModels = EmbeddingModels.te_ada2,
             dimensions: int = 1536,
             tries: int = 5,
```

### Comparing `serverless_openai-1.3.7/serverless_openai/helpers.py` & `serverless_openai-1.3.8/serverless_openai/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     user: str = 'user'
     system: str = 'system'
     assistant: str = 'assistant'
 
 class TextCompletionModels(str, ExtendedEnum):
     gpt4_1106 : str = "gpt-4-1106-preview"
     gpt4 : str = "gpt-4"
-    gpt4_turbo : str = "gpt-4-turbo-preview"
+    gpt4_turbo : str = "gpt-4-turbo"
+    gpt4_turbo_prev : str = "gpt-4-turbo-preview"
     gpt4_0125 : str = "gpt-4-0125-preview"
     gpt35_turbo_0125: str = "gpt-3.5-turbo-0125"
     gpt35_turbo_1106 : str = "gpt-3.5-turbo-1106"
     gpt35_turbo_16k : str = "gpt-3.5-turbo-16k"
     gpt35_turbo : str = "gpt-3.5-turbo"
 
 class Message(BaseModel):
@@ -41,14 +42,15 @@
 
 class ImageCreationModels(str, ExtendedEnum):
     dalle_2 : str = "dall-e-2"
     dalle_3 : str = "dall-e-3"
 
 class VisionModels(str, ExtendedEnum):
     gpt4_vision : str = "gpt-4-vision-preview"
+    gpt4_turbo : str = "gpt-4-turbo"
 
 class VisionMessage(BaseModel):
     text: str
     image: Union[str, np.ndarray, List[str]]
     role: Roles = Roles.user
     
     @validator('image', always=True)
```

### Comparing `serverless_openai-1.3.7/serverless_openai.egg-info/PKG-INFO` & `serverless_openai-1.3.8/serverless_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless_openai
-Version: 1.3.7
+Version: 1.3.8
 Summary: A package for using Openai in serverless environment
 Author: Jayr Castro
 Author-email: jayrcastro.py@gmail.com
 Keywords: serverless,openai,aws lambda,cloud functions,openai API
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `serverless_openai-1.3.7/setup.py` & `serverless_openai-1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.7'
+VERSION = '1.3.8'
 DESCRIPTION = "A package for using Openai in serverless environment"
 LONG_DESCRIPTION = 'A package for using Openai with scraping and etc. in serverless application such as AWS Lambda and GCP Cloud Function'
 
 # Setting up
 setup(
     name="serverless_openai",
     version=VERSION,
```

