# Comparing `tmp/promptlayer-0.5.6.tar.gz` & `tmp/promptlayer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlayer-0.5.6.tar", max compression
+gzip compressed data, was "promptlayer-1.0.0.tar", max compression
```

## Comparing `promptlayer-0.5.6.tar` & `promptlayer-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-04-10 15:56:24.553152 promptlayer-0.5.6/LICENSE
--rw-r--r--   0        0        0     3839 2024-04-10 15:56:24.553152 promptlayer-0.5.6/README.md
--rw-r--r--   0        0        0     1110 2024-04-10 15:56:24.553152 promptlayer-0.5.6/promptlayer/__init__.py
--rw-r--r--   0        0        0       67 2024-04-10 15:56:24.553152 promptlayer-0.5.6/promptlayer/groups/__init__.py
--rw-r--r--   0        0        0      139 2024-04-10 15:56:24.553152 promptlayer-0.5.6/promptlayer/groups/groups.py
--rw-r--r--   0        0        0     3736 2024-04-10 15:56:24.553152 promptlayer-0.5.6/promptlayer/promptlayer.py
--rw-r--r--   0        0        0      205 2024-04-10 15:56:24.553152 promptlayer-0.5.6/promptlayer/prompts/__init__.py
--rw-r--r--   0        0        0     2348 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/prompts/chat.py
--rw-r--r--   0        0        0     3215 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/prompts/prompts.py
--rw-r--r--   0        0        0       63 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/resources/__init__.py
--rw-r--r--   0        0        0      468 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/resources/base.py
--rw-r--r--   0        0        0      220 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/resources/prompt.py
--rw-r--r--   0        0        0      542 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/templates.py
--rw-r--r--   0        0        0      119 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/track/__init__.py
--rw-r--r--   0        0        0     1525 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/track/track.py
--rw-r--r--   0        0        0       61 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/types/__init__.py
--rw-r--r--   0        0        0     3813 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/types/prompt_template.py
--rw-r--r--   0        0        0    21269 2024-04-10 15:56:24.557152 promptlayer-0.5.6/promptlayer/utils.py
--rw-r--r--   0        0        0      487 2024-04-10 15:56:24.557152 promptlayer-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 promptlayer-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 19:19:57.139462 promptlayer-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3870 2024-05-10 19:19:57.139462 promptlayer-1.0.0/README.md
+-rw-r--r--   0        0        0     1565 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/groups/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/groups/groups.py
+-rw-r--r--   0        0        0     4035 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/promptlayer.py
+-rw-r--r--   0        0        0      717 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/templates.py
+-rw-r--r--   0        0        0      945 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/track/__init__.py
+-rw-r--r--   0        0        0     1610 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/track/track.py
+-rw-r--r--   0        0        0       61 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/types/__init__.py
+-rw-r--r--   0        0        0     3813 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/types/prompt_template.py
+-rw-r--r--   0        0        0    21130 2024-05-10 19:19:57.143462 promptlayer-1.0.0/promptlayer/utils.py
+-rw-r--r--   0        0        0      571 2024-05-10 19:19:57.143462 promptlayer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 promptlayer-1.0.0/PKG-INFO
```

### Comparing `promptlayer-0.5.6/LICENSE` & `promptlayer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.6/README.md` & `promptlayer-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,17 @@
 To get started, create an account by clicking “*Log in*” on [PromptLayer](https://promptlayer.com/). Once logged in, click the button to create an API key and save this in a secure location ([Guide to Using Env Vars](https://towardsdatascience.com/the-quick-guide-to-using-environment-variables-in-python-d4ec9291619e)).
 
 Once you have that all set up, [install PromptLayer using](https://pypi.org/project/promptlayer/) `pip`.
 
 In the Python file where you use OpenAI APIs, add the following. This allows us to keep track of your requests without needing any other code changes.
 
 ```python
-import promptlayer
-promptlayer.api_key = "<YOUR PromptLayer API KEY pl_xxxxxx>"
+from promptlayer import PromptLayer
+
+promptlayer = PromptLayer(api_key="<YOUR PromptLayer API KEY pl_xxxxxx>")
 openai = promptlayer.openai
 ```
 
 **You can then use `openai` as you would if you had imported it directly.**
 
 <aside>
 💡 Your OpenAI API Key is **never** sent to our servers. All OpenAI requests are made locally from your machine, PromptLayer just logs the request.
```

#### html2text {}

```diff
@@ -11,32 +11,32 @@
 clicking â*Log in*â on [PromptLayer](https://promptlayer.com/). Once logged
 in, click the button to create an API key and save this in a secure location (
 [Guide to Using Env Vars](https://towardsdatascience.com/the-quick-guide-to-
 using-environment-variables-in-python-d4ec9291619e)). Once you have that all
 set up, [install PromptLayer using](https://pypi.org/project/promptlayer/
 ) `pip`. In the Python file where you use OpenAI APIs, add the following. This
 allows us to keep track of your requests without needing any other code
-changes. ```python import promptlayer promptlayer.api_key = "" openai =
-promptlayer.openai ``` **You can then use `openai` as you would if you had
-imported it directly.** ð¡ Your OpenAI API Key is **never** sent to our
-servers. All OpenAI requests are made locally from your machine, PromptLayer
-just logs the request. ### Adding PromptLayer tags: `pl_tags` PromptLayer
-allows you to add tags through the `pl_tags` argument. This allows you to track
-and group requests in the dashboard. *Tags are not required but we recommend
-them!* ```python openai.Completion.create( engine="text-ada-001", prompt="My
-name is", pl_tags=["name-guessing", "pipeline-2"] ) ``` After making your first
-few requests, you should be able to see them in the PromptLayer dashboard! ##
-Using the REST API This Python library is a wrapper over PromptLayer's REST
-API. If you use another language, like Javascript, just interact directly with
-the API. Here is an example request below: ```jsx import requests
-request_response = requests.post( "https://api.promptlayer.com/track-request",
-json={ "function_name": "openai.Completion.create", "args": [], "kwargs":
-{"engine": "text-ada-001", "prompt": "My name is"}, "tags": ["hello", "world"],
-"request_response": {"id": "cmpl-6TEeJCRVlqQSQqhD8CYKd1HdCcFxM", "object":
-"text_completion", "created": 1672425843, "model": "text-ada-001", "choices": [
-{"text": " advocacy\"\n\nMy name is advocacy.", "index": 0, "logprobs": None,
-"finish_reason": "stop"}]}, "request_start_time": 1673987077.463504,
-"request_end_time": 1673987077.463504, "api_key": "pl_", }, ) ``` ##
-Contributing We welcome contributions to our open source project, including new
-features, infrastructure improvements, and better documentation. For more
-information or any questions, contact us at [hello@promptlayer.com](mailto:
-hello@promptlayer.com).
+changes. ```python from promptlayer import PromptLayer promptlayer =
+PromptLayer(api_key="") openai = promptlayer.openai ``` **You can then use
+`openai` as you would if you had imported it directly.** ð¡ Your OpenAI API
+Key is **never** sent to our servers. All OpenAI requests are made locally from
+your machine, PromptLayer just logs the request. ### Adding PromptLayer tags:
+`pl_tags` PromptLayer allows you to add tags through the `pl_tags` argument.
+This allows you to track and group requests in the dashboard. *Tags are not
+required but we recommend them!* ```python openai.Completion.create
+( engine="text-ada-001", prompt="My name is", pl_tags=["name-guessing",
+"pipeline-2"] ) ``` After making your first few requests, you should be able to
+see them in the PromptLayer dashboard! ## Using the REST API This Python
+library is a wrapper over PromptLayer's REST API. If you use another language,
+like Javascript, just interact directly with the API. Here is an example
+request below: ```jsx import requests request_response = requests.post( "https:
+//api.promptlayer.com/track-request", json={ "function_name":
+"openai.Completion.create", "args": [], "kwargs": {"engine": "text-ada-001",
+"prompt": "My name is"}, "tags": ["hello", "world"], "request_response": {"id":
+"cmpl-6TEeJCRVlqQSQqhD8CYKd1HdCcFxM", "object": "text_completion", "created":
+1672425843, "model": "text-ada-001", "choices": [{"text": " advocacy\"\n\nMy
+name is advocacy.", "index": 0, "logprobs": None, "finish_reason": "stop"}]},
+"request_start_time": 1673987077.463504, "request_end_time": 1673987077.463504,
+"api_key": "pl_", }, ) ``` ## Contributing We welcome contributions to our open
+source project, including new features, infrastructure improvements, and better
+documentation. For more information or any questions, contact us at
+[hello@promptlayer.com](mailto:hello@promptlayer.com).
```

### Comparing `promptlayer-0.5.6/promptlayer/promptlayer.py` & `promptlayer-1.0.0/promptlayer/promptlayer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import datetime
 import inspect
 import re
 
-from promptlayer.utils import async_wrapper, get_api_key, promptlayer_api_handler
+from promptlayer.utils import async_wrapper, promptlayer_api_handler
 
 
 class PromptLayerBase(object):
-    __slots__ = ["_obj", "__weakref__", "_function_name", "_provider_type"]
+    __slots__ = ["_obj", "__weakref__", "_function_name", "_provider_type", "_api_key"]
 
-    def __init__(self, obj, function_name="", provider_type="openai"):
+    def __init__(self, obj, function_name="", provider_type="openai", api_key=None):
         object.__setattr__(self, "_obj", obj)
         object.__setattr__(self, "_function_name", function_name)
         object.__setattr__(self, "_provider_type", provider_type)
+        object.__setattr__(self, "_api_key", api_key)
 
     def __getattr__(self, name):
         attr = getattr(object.__getattribute__(self, "_obj"), name)
         if (
             name != "count_tokens"  # fix for anthropic count_tokens
             and not re.match(
-                "<class 'anthropic\..*Error'>", str(attr)
+                r"<class 'anthropic\..*Error'>", str(attr)
             )  # fix for anthropic errors
             and not re.match(
-                "<class 'openai\..*Error'>", str(attr)
+                r"<class 'openai\..*Error'>", str(attr)
             )  # fix for openai errors
             and (
                 inspect.isclass(attr)
                 or inspect.isfunction(attr)
                 or inspect.ismethod(attr)
                 or str(type(attr))
                 == "<class 'anthropic.resources.completions.Completions'>"
                 or str(type(attr))
                 == "<class 'anthropic.resources.completions.AsyncCompletions'>"
                 or str(type(attr)) == "<class 'anthropic.resources.messages.Messages'>"
                 or str(type(attr))
                 == "<class 'anthropic.resources.messages.AsyncMessages'>"
-                or re.match("<class 'openai\.resources.*'>", str(type(attr)))
+                or re.match(r"<class 'openai\.resources.*'>", str(type(attr)))
             )
         ):
             return PromptLayerBase(
                 attr,
                 function_name=f'{object.__getattribute__(self, "_function_name")}.{name}',
                 provider_type=object.__getattribute__(self, "_provider_type"),
+                api_key=object.__getattribute__(self, "_api_key"),
             )
         return attr
 
     def __delattr__(self, name):
         delattr(object.__getattribute__(self, "_obj"), name)
 
     def __setattr__(self, name, value):
@@ -58,35 +60,37 @@
         request_start_time = datetime.datetime.now().timestamp()
         function_object = object.__getattribute__(self, "_obj")
         if inspect.isclass(function_object):
             return PromptLayerBase(
                 function_object(*args, **kwargs),
                 function_name=object.__getattribute__(self, "_function_name"),
                 provider_type=object.__getattribute__(self, "_provider_type"),
+                api_key=object.__getattribute__(self, "_api_key"),
             )
         function_response = function_object(*args, **kwargs)
         if inspect.iscoroutinefunction(function_object) or inspect.iscoroutine(
             function_response
         ):
             return async_wrapper(
                 function_response,
                 return_pl_id,
                 request_start_time,
                 object.__getattribute__(self, "_function_name"),
                 object.__getattribute__(self, "_provider_type"),
                 tags,
+                api_key=object.__getattribute__(self, "_api_key"),
                 *args,
                 **kwargs,
             )
         request_end_time = datetime.datetime.now().timestamp()
         return promptlayer_api_handler(
             object.__getattribute__(self, "_function_name"),
             object.__getattribute__(self, "_provider_type"),
             args,
             kwargs,
             tags,
             function_response,
             request_start_time,
             request_end_time,
-            get_api_key(),
+            object.__getattribute__(self, "_api_key"),
             return_pl_id=return_pl_id,
         )
```

### Comparing `promptlayer-0.5.6/promptlayer/track/track.py` & `promptlayer-1.0.0/promptlayer/track/track.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 from promptlayer.utils import (
-    get_api_key,
     promptlayer_track_group,
     promptlayer_track_metadata,
     promptlayer_track_prompt,
     promptlayer_track_score,
 )
 
 
-def prompt(request_id, prompt_name, prompt_input_variables, version=None, label=None):
+def prompt(
+    request_id,
+    prompt_name,
+    prompt_input_variables,
+    version=None,
+    label=None,
+    api_key: str = None,
+):
     if not isinstance(prompt_input_variables, dict):
         raise Exception("Please provide a dictionary of input variables.")
     return promptlayer_track_prompt(
-        request_id, prompt_name, prompt_input_variables, get_api_key(), version, label
+        request_id, prompt_name, prompt_input_variables, api_key, version, label
     )
 
 
-def metadata(request_id, metadata):
+def metadata(request_id, metadata, api_key: str = None):
     if not isinstance(metadata, dict):
         raise Exception("Please provide a dictionary of metadata.")
     for key, value in metadata.items():
         if not isinstance(key, str) or not isinstance(value, str):
             raise Exception(
                 "Please provide a dictionary of metadata with key value pair of strings."
             )
-    return promptlayer_track_metadata(request_id, metadata, get_api_key())
+    return promptlayer_track_metadata(request_id, metadata, api_key)
 
 
-def score(request_id, score, score_name=None):
+def score(request_id, score, score_name=None, api_key: str = None):
     if not isinstance(score, int):
         raise Exception("Please provide a int score.")
     if not isinstance(score_name, str) and score_name is not None:
         raise Exception("Please provide a string as score name.")
     if score < 0 or score > 100:
         raise Exception("Please provide a score between 0 and 100.")
-    return promptlayer_track_score(request_id, score, score_name, get_api_key())
+    return promptlayer_track_score(request_id, score, score_name, api_key)
 
 
-def group(request_id, group_id):
-    return promptlayer_track_group(request_id, group_id)
+def group(request_id, group_id, api_key: str = None):
+    return promptlayer_track_group(request_id, group_id, api_key)
```

### Comparing `promptlayer-0.5.6/promptlayer/types/prompt_template.py` & `promptlayer-1.0.0/promptlayer/types/prompt_template.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.6/promptlayer/utils.py` & `promptlayer-1.0.0/promptlayer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,27 @@
 import types
 from copy import deepcopy
 from enum import Enum
 from typing import List, Union
 
 import requests
 
-import promptlayer
 from promptlayer.types.prompt_template import (
     GetPromptTemplate,
     GetPromptTemplateResponse,
     ListPromptTemplateResponse,
     PublishPromptTemplate,
     PublishPromptTemplateResponse,
 )
 
 URL_API_PROMPTLAYER = os.environ.setdefault(
     "URL_API_PROMPTLAYER", "https://api.promptlayer.com"
 )
 
 
-def get_api_key():
-    # raise an error if the api key is not set
-    if promptlayer.api_key is None:
-        raise Exception(
-            "Please set your PROMPTLAYER_API_KEY environment variable or set API KEY in code using 'promptlayer.api_key = <your_api_key>' "
-        )
-    else:
-        return promptlayer.api_key
-
-
 def promptlayer_api_handler(
     function_name,
     provider_type,
     args,
     kwargs,
     tags,
     response,
@@ -62,14 +51,15 @@
                 "args": args,
                 "kwargs": kwargs,
                 "tags": tags,
                 "request_start_time": request_start_time,
                 "request_end_time": request_end_time,
                 "return_pl_id": return_pl_id,
             },
+            api_key,
         )
     else:
         request_id = promptlayer_api_request(
             function_name,
             provider_type,
             args,
             kwargs,
@@ -104,15 +94,15 @@
         provider_type,
         args,
         kwargs,
         tags,
         response,
         request_start_time,
         request_end_time,
-        get_api_key(),
+        api_key,
         return_pl_id=return_pl_id,
     )
 
 
 def convert_native_object_to_dict(native_object):
     if isinstance(native_object, dict):
         return {k: convert_native_object_to_dict(v) for k, v in native_object.items()}
@@ -341,31 +331,33 @@
             file=sys.stderr,
         )
         return False
     return True
 
 
 class GeneratorProxy:
-    def __init__(self, generator, api_request_arguments):
+    def __init__(self, generator, api_request_arguments, api_key):
         self.generator = generator
         self.results = []
         self.api_request_arugments = api_request_arguments
+        self.api_key = api_key
 
     def __iter__(self):
         return self
 
     def __aiter__(self):
         return self
 
     async def __aenter__(self):
         api_request_arguments = self.api_request_arugments
         if hasattr(self.generator, "_AsyncMessageStreamManager__api_request"):
             return GeneratorProxy(
                 await self.generator._AsyncMessageStreamManager__api_request,
                 api_request_arguments,
+                self.api_key,
             )
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         pass
 
     async def __anext__(self):
         result = await self.generator.__anext__()
@@ -374,15 +366,15 @@
     def __next__(self):
         result = next(self.generator)
         return self._abstracted_next(result)
 
     def __getattr__(self, name):
         if name == "text_stream":  # anthropic async stream
             return GeneratorProxy(
-                self.generator.text_stream, self.api_request_arugments
+                self.generator.text_stream, self.api_request_arugments, self.api_key
             )
         return getattr(self.generator, name)
 
     def _abstracted_next(self, result):
         self.results.append(result)
         provider_type = self.api_request_arugments["provider_type"]
         end_anthropic = False
@@ -404,15 +396,15 @@
                 self.api_request_arugments["provider_type"],
                 self.api_request_arugments["args"],
                 self.api_request_arugments["kwargs"],
                 self.api_request_arugments["tags"],
                 self.cleaned_result(),
                 self.api_request_arugments["request_start_time"],
                 self.api_request_arugments["request_end_time"],
-                get_api_key(),
+                self.api_key,
                 return_pl_id=self.api_request_arugments["return_pl_id"],
             )
             if self.api_request_arugments["return_pl_id"]:
                 return result, request_id
         if self.api_request_arugments["return_pl_id"]:
             return result, None
         return result
@@ -513,39 +505,40 @@
 async def async_wrapper(
     coroutine_obj,
     return_pl_id,
     request_start_time,
     function_name,
     provider_type,
     tags,
+    api_key: str = None,
     *args,
     **kwargs,
 ):
     response = await coroutine_obj
     request_end_time = datetime.datetime.now().timestamp()
     return await promptlayer_api_handler_async(
         function_name,
         provider_type,
         args,
         kwargs,
         tags,
         response,
         request_start_time,
         request_end_time,
-        get_api_key(),
+        api_key,
         return_pl_id=return_pl_id,
     )
 
 
-def promptlayer_create_group():
+def promptlayer_create_group(api_key: str = None):
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/create-group",
             json={
-                "api_key": get_api_key(),
+                "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
             warn_on_bad_response(
                 request_response,
                 "WARNING: While creating your group PromptLayer had the following error",
             )
@@ -554,20 +547,20 @@
         # I'm aiming for a more specific exception catch here
         raise Exception(
             f"PromptLayer had the following error while creating your group: {e}"
         )
     return request_response.json()["id"]
 
 
-def promptlayer_track_group(request_id, group_id):
+def promptlayer_track_group(request_id, group_id, api_key: str = None):
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/track-group",
             json={
-                "api_key": get_api_key(),
+                "api_key": api_key,
                 "request_id": request_id,
                 "group_id": group_id,
             },
         )
         if request_response.status_code != 200:
             warn_on_bad_response(
                 request_response,
@@ -575,26 +568,27 @@
             )
             return False
     except requests.exceptions.RequestException as e:
         # I'm aiming for a more specific exception catch here
         raise Exception(
             f"PromptLayer had the following error while tracking your group: {e}"
         )
+    return True
 
 
 def get_prompt_template(
-    prompt_name: str, params: Union[GetPromptTemplate, None] = None
+    prompt_name: str, params: Union[GetPromptTemplate, None] = None, api_key: str = None
 ) -> GetPromptTemplateResponse:
     try:
-        json_body = {"api_key": get_api_key()}
+        json_body = {"api_key": api_key}
         if params:
             json_body = {**json_body, **params}
         response = requests.post(
             f"{URL_API_PROMPTLAYER}/prompt-templates/{prompt_name}",
-            headers={"X-API-KEY": get_api_key()},
+            headers={"X-API-KEY": api_key},
             json=json_body,
         )
         if response.status_code != 200:
             raise Exception(
                 f"PromptLayer had the following error while getting your prompt template: {response.text}"
             )
         return response.json()
@@ -602,19 +596,20 @@
         raise Exception(
             f"PromptLayer had the following error while getting your prompt template: {e}"
         )
 
 
 def publish_prompt_template(
     body: PublishPromptTemplate,
+    api_key: str = None,
 ) -> PublishPromptTemplateResponse:
     try:
         response = requests.post(
             f"{URL_API_PROMPTLAYER}/rest/prompt-templates",
-            headers={"X-API-KEY": get_api_key()},
+            headers={"X-API-KEY": api_key},
             json={
                 "prompt_template": {**body},
                 "prompt_version": {**body},
                 "release_labels": body.get("release_labels"),
             },
         )
         if response.status_code == 400:
@@ -625,20 +620,20 @@
     except requests.exceptions.RequestException as e:
         raise Exception(
             f"PromptLayer had the following error while publishing your prompt template: {e}"
         )
 
 
 def get_all_prompt_templates(
-    page: int = 1, per_page: int = 30
+    page: int = 1, per_page: int = 30, api_key: str = None
 ) -> List[ListPromptTemplateResponse]:
     try:
         response = requests.get(
             f"{URL_API_PROMPTLAYER}/prompt-templates",
-            headers={"X-API-KEY": get_api_key()},
+            headers={"X-API-KEY": api_key},
             params={"page": page, "per_page": per_page},
         )
         if response.status_code != 200:
             raise Exception(
                 f"PromptLayer had the following error while getting all your prompt templates: {response.text}"
             )
         items = response.json().get("items", [])
```

### Comparing `promptlayer-0.5.6/PKG-INFO` & `promptlayer-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.5.6
+Version: 1.0.0
 Summary: PromptLayer is a platform for prompt engineering and tracks your LLM requests.
 License: Apache-2.0
 Author: Magniv
 Author-email: hello@magniv.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: anthropic (>=0.25.8,<0.26.0)
+Requires-Dist: anyio (>=4.3.0,<5.0.0)
+Requires-Dist: openai (>=1.26.0,<2.0.0)
+Requires-Dist: pytest (>=8.2.0,<9.0.0)
+Requires-Dist: pytest-asyncio (>=0.23.6,<0.24.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # 🍰 PromptLayer
 
@@ -52,16 +57,17 @@
 To get started, create an account by clicking “*Log in*” on [PromptLayer](https://promptlayer.com/). Once logged in, click the button to create an API key and save this in a secure location ([Guide to Using Env Vars](https://towardsdatascience.com/the-quick-guide-to-using-environment-variables-in-python-d4ec9291619e)).
 
 Once you have that all set up, [install PromptLayer using](https://pypi.org/project/promptlayer/) `pip`.
 
 In the Python file where you use OpenAI APIs, add the following. This allows us to keep track of your requests without needing any other code changes.
 
 ```python
-import promptlayer
-promptlayer.api_key = "<YOUR PromptLayer API KEY pl_xxxxxx>"
+from promptlayer import PromptLayer
+
+promptlayer = PromptLayer(api_key="<YOUR PromptLayer API KEY pl_xxxxxx>")
 openai = promptlayer.openai
 ```
 
 **You can then use `openai` as you would if you had imported it directly.**
 
 <aside>
 💡 Your OpenAI API Key is **never** sent to our servers. All OpenAI requests are made locally from your machine, PromptLayer just logs the request.
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.5.6 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 1.0.0 Summary: PromptLayer is
 a platform for prompt engineering and tracks your LLM requests. License:
 Apache-2.0 Author: Magniv Author-email: hello@magniv.io Requires-Python:
 >=3.8.1,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Description-Content-Type: text/markdown
+Language :: Python :: 3.12 Requires-Dist: anthropic (>=0.25.8,<0.26.0)
+Requires-Dist: anyio (>=4.3.0,<5.0.0) Requires-Dist: openai (>=1.26.0,<2.0.0)
+Requires-Dist: pytest (>=8.2.0,<9.0.0) Requires-Dist: pytest-asyncio
+(>=0.23.6,<0.24.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Description-
+Content-Type: text/markdown
  # ð° PromptLayer **The first platform built for prompt engineers** _[_P_y_t_h_o_n_]
                            _[_D_o_c_s_]_[_D_e_m_o_ _w_i_t_h_ _L_o_o_m_]---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
 to track, manage, and share your GPT prompt engineering. PromptLayer acts a
 middleware between your code and OpenAIâs python library. PromptLayer records
 all your OpenAI API requests, allowing you to search and explore request
 history in the PromptLayer dashboard. This repo contains the Python wrapper
@@ -20,32 +23,32 @@
 clicking â*Log in*â on [PromptLayer](https://promptlayer.com/). Once logged
 in, click the button to create an API key and save this in a secure location (
 [Guide to Using Env Vars](https://towardsdatascience.com/the-quick-guide-to-
 using-environment-variables-in-python-d4ec9291619e)). Once you have that all
 set up, [install PromptLayer using](https://pypi.org/project/promptlayer/
 ) `pip`. In the Python file where you use OpenAI APIs, add the following. This
 allows us to keep track of your requests without needing any other code
-changes. ```python import promptlayer promptlayer.api_key = "" openai =
-promptlayer.openai ``` **You can then use `openai` as you would if you had
-imported it directly.** ð¡ Your OpenAI API Key is **never** sent to our
-servers. All OpenAI requests are made locally from your machine, PromptLayer
-just logs the request. ### Adding PromptLayer tags: `pl_tags` PromptLayer
-allows you to add tags through the `pl_tags` argument. This allows you to track
-and group requests in the dashboard. *Tags are not required but we recommend
-them!* ```python openai.Completion.create( engine="text-ada-001", prompt="My
-name is", pl_tags=["name-guessing", "pipeline-2"] ) ``` After making your first
-few requests, you should be able to see them in the PromptLayer dashboard! ##
-Using the REST API This Python library is a wrapper over PromptLayer's REST
-API. If you use another language, like Javascript, just interact directly with
-the API. Here is an example request below: ```jsx import requests
-request_response = requests.post( "https://api.promptlayer.com/track-request",
-json={ "function_name": "openai.Completion.create", "args": [], "kwargs":
-{"engine": "text-ada-001", "prompt": "My name is"}, "tags": ["hello", "world"],
-"request_response": {"id": "cmpl-6TEeJCRVlqQSQqhD8CYKd1HdCcFxM", "object":
-"text_completion", "created": 1672425843, "model": "text-ada-001", "choices": [
-{"text": " advocacy\"\n\nMy name is advocacy.", "index": 0, "logprobs": None,
-"finish_reason": "stop"}]}, "request_start_time": 1673987077.463504,
-"request_end_time": 1673987077.463504, "api_key": "pl_", }, ) ``` ##
-Contributing We welcome contributions to our open source project, including new
-features, infrastructure improvements, and better documentation. For more
-information or any questions, contact us at [hello@promptlayer.com](mailto:
-hello@promptlayer.com).
+changes. ```python from promptlayer import PromptLayer promptlayer =
+PromptLayer(api_key="") openai = promptlayer.openai ``` **You can then use
+`openai` as you would if you had imported it directly.** ð¡ Your OpenAI API
+Key is **never** sent to our servers. All OpenAI requests are made locally from
+your machine, PromptLayer just logs the request. ### Adding PromptLayer tags:
+`pl_tags` PromptLayer allows you to add tags through the `pl_tags` argument.
+This allows you to track and group requests in the dashboard. *Tags are not
+required but we recommend them!* ```python openai.Completion.create
+( engine="text-ada-001", prompt="My name is", pl_tags=["name-guessing",
+"pipeline-2"] ) ``` After making your first few requests, you should be able to
+see them in the PromptLayer dashboard! ## Using the REST API This Python
+library is a wrapper over PromptLayer's REST API. If you use another language,
+like Javascript, just interact directly with the API. Here is an example
+request below: ```jsx import requests request_response = requests.post( "https:
+//api.promptlayer.com/track-request", json={ "function_name":
+"openai.Completion.create", "args": [], "kwargs": {"engine": "text-ada-001",
+"prompt": "My name is"}, "tags": ["hello", "world"], "request_response": {"id":
+"cmpl-6TEeJCRVlqQSQqhD8CYKd1HdCcFxM", "object": "text_completion", "created":
+1672425843, "model": "text-ada-001", "choices": [{"text": " advocacy\"\n\nMy
+name is advocacy.", "index": 0, "logprobs": None, "finish_reason": "stop"}]},
+"request_start_time": 1673987077.463504, "request_end_time": 1673987077.463504,
+"api_key": "pl_", }, ) ``` ## Contributing We welcome contributions to our open
+source project, including new features, infrastructure improvements, and better
+documentation. For more information or any questions, contact us at
+[hello@promptlayer.com](mailto:hello@promptlayer.com).
```

