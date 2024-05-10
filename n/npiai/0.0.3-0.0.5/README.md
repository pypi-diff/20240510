# Comparing `tmp/npiai-0.0.3.tar.gz` & `tmp/npiai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npiai-0.0.3.tar", max compression
+gzip compressed data, was "npiai-0.0.5.tar", max compression
```

## Comparing `npiai-0.0.3.tar` & `npiai-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-18 05:31:48.474805 npiai-0.0.3/README.md
--rw-r--r--   0        0        0      151 2024-04-20 00:39:52.418936 npiai-0.0.3/npiai/__init__.py
--rw-r--r--   0        0        0      132 2024-04-20 00:26:15.294019 npiai-0.0.3/npiai/app/__init__.py
--rw-r--r--   0        0        0      282 2024-04-24 22:25:36.766045 npiai-0.0.3/npiai/app/browser.py
--rw-r--r--   0        0        0      278 2024-04-24 22:20:47.884237 npiai-0.0.3/npiai/app/discord.py
--rw-r--r--   0        0        0      277 2024-04-24 22:20:06.679823 npiai-0.0.3/npiai/app/github.py
--rw-r--r--   0        0        0      510 2024-04-20 00:09:40.569381 npiai-0.0.3/npiai/app/google.py
--rw-r--r--   0        0        0     1064 2024-04-24 22:19:56.249598 npiai-0.0.3/npiai/app/human_feedback.py
--rw-r--r--   0        0        0      279 2024-04-24 22:20:30.694448 npiai-0.0.3/npiai/app/twitter.py
--rw-r--r--   0        0        0       57 2024-04-20 00:26:15.289527 npiai-0.0.3/npiai/core/__init__.py
--rw-r--r--   0        0        0     6106 2024-04-20 00:09:40.560265 npiai-0.0.3/npiai/core/base.py
--rw-r--r--   0        0        0      312 2024-04-24 22:31:35.055119 npiai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 npiai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-02 23:10:36.742561 npiai-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-02 21:49:09.883864 npiai-0.0.5/README.md
+-rw-r--r--   0        0        0      151 2024-05-02 21:49:09.884168 npiai-0.0.5/npiai/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-02 21:49:09.884353 npiai-0.0.5/npiai/app/__init__.py
+-rw-r--r--   0        0        0      278 2024-05-02 21:49:09.884486 npiai-0.0.5/npiai/app/discord.py
+-rw-r--r--   0        0        0      275 2024-05-02 21:49:09.884617 npiai-0.0.5/npiai/app/github.py
+-rw-r--r--   0        0        0      510 2024-05-02 21:49:09.884749 npiai-0.0.5/npiai/app/google.py
+-rw-r--r--   0        0        0     1073 2024-05-02 21:49:09.884889 npiai-0.0.5/npiai/app/human_feedback.py
+-rw-r--r--   0        0        0       92 2024-05-02 21:49:09.885063 npiai-0.0.5/npiai/browser_app/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-02 21:49:09.885203 npiai-0.0.5/npiai/browser_app/browser.py
+-rw-r--r--   0        0        0      278 2024-05-02 21:49:09.885330 npiai-0.0.5/npiai/browser_app/twitter.py
+-rw-r--r--   0        0        0       57 2024-05-02 21:49:09.885499 npiai-0.0.5/npiai/core/__init__.py
+-rw-r--r--   0        0        0     7978 2024-05-10 17:29:39.177868 npiai-0.0.5/npiai/core/base.py
+-rw-r--r--   0        0        0     2137 2024-05-10 17:29:39.178174 npiai-0.0.5/npiai/core/hitl.py
+-rw-r--r--   0        0        0     1771 2024-05-10 17:29:39.178322 npiai-0.0.5/npiai/tools/hitl/console.py
+-rw-r--r--   0        0        0     2185 2024-05-10 17:29:39.178460 npiai-0.0.5/npiai/tools/hitl/twilio.py
+-rw-r--r--   0        0        0       49 2024-05-02 21:49:09.885976 npiai-0.0.5/npiai/utils/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-02 21:49:09.886103 npiai-0.0.5/npiai/utils/logger.py
+-rw-r--r--   0        0        0      380 2024-05-10 17:32:12.965041 npiai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 npiai-0.0.5/PKG-INFO
```

### Comparing `npiai-0.0.3/npiai/app/human_feedback.py` & `npiai-0.0.5/npiai/app/human_feedback.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             app_type=api_pb2.AppType.APP_UNKNOWN,
         )
 
     def schema(self):
         return {
             "type": "function",
             "function": {
-                "name": f"{ self.tool_name() }",
+                "name": f"{self.tool_name()}",
                 "description": "Ask the human for help",
                 "parameters": {
                     "type": "object",
                     "properties": {
                         "message": {
                             "type": "string",
                             "description": f"the task you want to ask for help",
@@ -28,11 +28,12 @@
                     },
                     "required": ["message"],
                 },
             },
         }
 
     def chat(self, msg: str) -> str:
-        response = input(colored(msg, 'green') + colored('\nType Your Response: ', 'magenta'))
+        print(colored(msg, 'green'))
+        response = input(colored('Type Your Response: ', 'magenta'))
         print()
         return response
```

### Comparing `npiai-0.0.3/npiai/core/base.py` & `npiai-0.0.5/npiai/core/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,174 @@
 import json
+import threading
+import traceback
 from typing import Union, List
 import grpc
 import uuid
 
 from openai import OpenAI
 from openai.types.chat import (
     ChatCompletionSystemMessageParam,
     ChatCompletionToolChoiceOptionParam,
     ChatCompletionToolParam,
     ChatCompletionUserMessageParam,
 )
 
 from npiai_proto import api_pb2_grpc, api_pb2
+from npiai.utils import logger
+from npiai.core import hitl
 
 
-# from npiai..api_pb2 import
-
 class App:
     __app_name: str
     __app_type: api_pb2.AppType
     __npi_endpoint: str
     stub: api_pb2_grpc.AppServerStub
+    hitl_handler: hitl.HITLHandler = None
 
-    def __init__(self, app_name: str, app_type: api_pb2.AppType, endpoint: str = "localhost:9140"):
+    def __init__(
+        self,
+        app_name: str,
+        app_type: api_pb2.AppType,
+        endpoint: str = "localhost:9140",
+        hitl_handler: hitl.HITLHandler = None,
+    ):
         self.__app_name = app_name
         if endpoint is None:
             endpoint = "localhost:9140"
         self.__npi_endpoint = endpoint
         self.__app_type = app_type
         channel = grpc.insecure_channel(self.__npi_endpoint)
         self.stub = api_pb2_grpc.AppServerStub(channel)
+        self.hitl_handler = hitl_handler
 
     def tool_name(self):
         return self.__app_name
 
     def schema(self):
         try:
-            resp = self.stub.GetAppSchema(api_pb2.AppSchemaRequest(
-                type=self.__app_type
-            ))
+            resp = self.stub.GetAppSchema(
+                api_pb2.AppSchemaRequest(
+                    type=self.__app_type
+                )
+            )
         except Exception as e:
-            print(e)
+            logger.error(e)
             return None
         return json.loads(resp.schema)
 
     def chat(self, msg: str) -> str:
-        resp = self.stub.Chat(api_pb2.Request(
-            code=api_pb2.RequestCode.CHAT,
-            chat_request=api_pb2.ChatRequest(
-                type=self.__app_type,
-                instruction=msg
+        resp = self.stub.Chat(
+            api_pb2.Request(
+                code=api_pb2.RequestCode.CHAT,
+                chat_request=api_pb2.ChatRequest(
+                    type=self.__app_type,
+                    instruction=msg
+                )
             )
-        ))
+        )
         while True:
             match resp.code:
                 case api_pb2.ResponseCode.FINISHED:
                     return resp.chat_response.message
                 case api_pb2.ResponseCode.MESSAGE:
-                    print(resp.chat_response.message)
-                    resp = self.stub.Chat(api_pb2.Request(
-                        code=api_pb2.RequestCode.FETCH,
-                        request_id=str(uuid.uuid4()),
-                        thread_id=resp.thread_id,
-                        chat_request=api_pb2.ChatRequest(
-                            type=self.__app_type,
+                    logger.info(f'[{self.__app_name}]: Received message: {resp.chat_response.message}')
+                    resp = self.stub.Chat(
+                        api_pb2.Request(
+                            code=api_pb2.RequestCode.FETCH,
+                            request_id=str(uuid.uuid4()),
+                            thread_id=resp.thread_id,
+                            chat_request=api_pb2.ChatRequest(
+                                type=self.__app_type,
+                            )
                         )
-                    ))
+                    )
                 case api_pb2.ResponseCode.SUCCESS:
-                    resp = self.stub.Chat(api_pb2.Request(
-                        code=api_pb2.RequestCode.FETCH,
-                        request_id=str(uuid.uuid4()),
-                        thread_id=resp.thread_id,
-                        chat_request=api_pb2.ChatRequest(
-                            type=self.__app_type,
+                    resp = self.stub.Chat(
+                        api_pb2.Request(
+                            code=api_pb2.RequestCode.FETCH,
+                            request_id=str(uuid.uuid4()),
+                            thread_id=resp.thread_id,
+                            chat_request=api_pb2.ChatRequest(
+                                type=self.__app_type,
+                            )
                         )
-                    ))
+                    )
                 case api_pb2.ResponseCode.ACTION_REQUIRED:
-                    ar = resp.action_response
-                    if ar.type is api_pb2.ActionType.HUMAN_FEEDBACK:
-                        fb = ar.human_feedback
-                        arr = api_pb2.ActionResultRequest(
-                            action_id=ar.action_id,
-                        )
+                    resp = self.stub.Chat(self.__call_human(resp))
+                case _:
+                    raise Exception("Error: failed to call function")
 
-                        if fb.type is api_pb2.HumanFeedbackActionType.INPUT:
-                            arr.action_result = input(f"Action Required: {fb.notice}\n")
+    def hitl(self, handler: hitl.HITLHandler):
+        self.hitl_handler = handler
 
-                        resp = self.stub.Chat(api_pb2.Request(
-                            code=api_pb2.RequestCode.ACTION_RESULT,
-                            request_id=str(uuid.uuid4()),
-                            thread_id=resp.thread_id,
-                            action_result_request=arr,
-                        ))
-                case _:
-                    return "Error: failed to call function"
+    def __call_human(self, resp: api_pb2.Response) -> api_pb2.Request:
+        human_resp = self.hitl_handler.handle(
+            hitl.convert_to_hitl_request(
+                req=resp.action_response,
+                app_name=self.__app_name
+            )
+        )
+        if human_resp is hitl.ACTION_APPROVED:
+            result = "approved"
+        else:
+            result = "denied"
+        return api_pb2.Request(
+            code=api_pb2.RequestCode.ACTION_RESULT,
+            request_id=str(uuid.uuid4()),
+            thread_id=resp.thread_id,
+            action_result_request=api_pb2.ActionResultRequest(
+                action_id=resp.action_response.action_id,
+                action_result=result,
+            )
+        )
 
 
 class Agent:
     __agent_name: str
     __npi_endpoint: str
     __prompt: str
     __description: str
     __llm: OpenAI
     tool_choice: ChatCompletionToolChoiceOptionParam = "auto"
     fn_map: dict = {}
+    hitl_handler: hitl.HITLHandler = None
 
-    def __init__(self,
-                 agent_name: str,
-                 description: str,
-                 prompt: str,
-                 endpoint: str = None,
-                 llm: OpenAI = None):
+    def __init__(
+        self,
+        agent_name: str,
+        description: str,
+        prompt: str,
+        endpoint: str = None,
+        llm: OpenAI = None,
+        hitl_handler: hitl.HITLHandler = None,
+    ):
         self.__agent_name = agent_name
         self.__description = description
         self.__prompt = prompt
         self.__npi_endpoint = endpoint
         self.__llm = llm
+        self.hitl_handler = hitl_handler
 
-    def use(self, *tools: Union['App']):
-        for app in tools:
+    def use(self, *apps: App):
+        for app in apps:
+            # inherit HITL handler
+            if app.hitl_handler is None:
+                app.hitl_handler = self.hitl_handler
             app_name = app.tool_name()
             self.fn_map[app_name] = app
 
+    def group(self, *agents: 'Agent'):
+        for agent in agents:
+            app_name = agent.__as_app().tool_name()
+            self.fn_map[app_name] = agent
+
+    def hitl(self, handler: hitl.HITLHandler):
+        self.hitl_handler = handler
+
     def run(self, msg: str) -> str:
 
         messages = [ChatCompletionSystemMessageParam(
             content=self.__prompt,
             role="system",
         ), ChatCompletionUserMessageParam(
             content=msg,
@@ -141,43 +184,72 @@
                 max_tokens=4096,
             )
             response_message = response.choices[0].message
 
             messages.append(response_message)
 
             if response_message.content:
-                print(response_message.content + '\n')
+                logger.info(response_message.content + '\n')
 
             tool_calls = response_message.tool_calls
 
             if tool_calls is None:
                 return response_message.content
 
             for tool_call in tool_calls:
                 fn_name = tool_call.function.name
                 args = json.loads(tool_call.function.arguments)
 
-                res = self.__call(fn_name, args)
-                print(f"Response: {res}")
+                try:
+                    res = self.__call(fn_name, args)
+                    # logger.info(f"Response: {res}")
+                    logger.debug(f'[{self.__agent_name}]: app `{fn_name}` returned: {res}')
+                except Exception as e:
+                    res = ''.join(traceback.format_exception(e))
+                    logger.error(res)
+
                 messages.append(
                     {
                         "tool_call_id": tool_call.id,
                         "role": "tool",
                         "name": fn_name,
                         "content": res,
                     }
                 )
-                # self.on_round_end(message)
+
+    def when(self, task: str):
+        running = True
+        msg = f'When {task}'
+
+        def _poll():
+            nonlocal running
+            while running:
+                self.run(msg)
+
+        def _stop():
+            nonlocal running
+            running = False
+
+        thread = threading.Thread(target=_poll)
+        # thread.daemon = True
+        thread.start()
+
+        return _stop
 
     def __call(self, fn_name: str, args: dict) -> str:
-        call_msg = f'Calling {fn_name}({args})'
-        print(call_msg)
+        call_msg = f'[{self.__agent_name}]: Calling {fn_name}({args})'
+        logger.info(call_msg)
+
+        if fn_name not in self.fn_map:
+            raise Exception(f"Tool {fn_name} not found.")
+
         fn = self.fn_map[fn_name]
-        if fn is not None:
-            return fn.chat(args['message'])
-        return "Error: tool not found"
+        return fn.chat(args['message'])
 
     def __tools(self) -> List[ChatCompletionToolParam]:
         tools = []
         for tool_name, tool in self.fn_map.items():
             tools.append(tool.schema())
         return tools
+
+    def __as_app(self) -> App:
+        return App(self.__agent_name, api_pb2.AppType.CHAT)
```

