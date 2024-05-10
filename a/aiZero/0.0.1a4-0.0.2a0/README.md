# Comparing `tmp/aiZero-0.0.1a4.tar.gz` & `tmp/aiZero-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiZero-0.0.1a4.tar", last modified: Thu May  9 02:39:58 2024, max compression
+gzip compressed data, was "aiZero-0.0.2a0.tar", last modified: Fri May 10 09:53:41 2024, max compression
```

## Comparing `aiZero-0.0.1a4.tar` & `aiZero-0.0.2a0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.439221 aiZero-0.0.1a4/
--rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.1a4/MANIFEST.in
--rw-r--r--   0 emhang     (501) staff       (20)     9606 2024-05-09 02:39:58.439050 aiZero-0.0.1a4/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)     9059 2024-05-09 02:38:31.000000 aiZero-0.0.1a4/README.md
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.435054 aiZero-0.0.1a4/aiZero/
--rw-r--r--   0 emhang     (501) staff       (20)    18610 2024-05-08 02:22:35.000000 aiZero-0.0.1a4/aiZero/__init__.py
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.433799 aiZero-0.0.1a4/aiZero/static/
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.436658 aiZero-0.0.1a4/aiZero/static/audios/
--rw-r--r--   0 emhang     (501) staff       (20)   276040 2024-05-07 07:22:42.000000 aiZero-0.0.1a4/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.438169 aiZero-0.0.1a4/aiZero/static/js/
--rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.1a4/aiZero/static/js/marked.min.js
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.438604 aiZero-0.0.1a4/aiZero/templates/
--rw-r--r--   0 emhang     (501) staff       (20)    28097 2024-04-17 06:07:29.000000 aiZero-0.0.1a4/aiZero/templates/index.html
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.436437 aiZero-0.0.1a4/aiZero.egg-info/
--rw-r--r--   0 emhang     (501) staff       (20)     9606 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)      319 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/SOURCES.txt
--rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/dependency_links.txt
--rw-r--r--   0 emhang     (501) staff       (20)       40 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/requires.txt
--rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/top_level.txt
--rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-09 02:39:58.439271 aiZero-0.0.1a4/setup.cfg
--rw-r--r--   0 emhang     (501) staff       (20)      820 2024-05-09 02:39:01.000000 aiZero-0.0.1a4/setup.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-10 09:53:41.093221 aiZero-0.0.2a0/
+-rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.2a0/MANIFEST.in
+-rw-r--r--   0 emhang     (501) staff       (20)    12929 2024-05-10 09:53:41.093085 aiZero-0.0.2a0/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)    12382 2024-05-10 09:53:00.000000 aiZero-0.0.2a0/README.md
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-10 09:53:41.090951 aiZero-0.0.2a0/aiZero/
+-rw-r--r--   0 emhang     (501) staff       (20)    19874 2024-05-10 09:34:48.000000 aiZero-0.0.2a0/aiZero/__init__.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-10 09:53:41.090323 aiZero-0.0.2a0/aiZero/static/
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-10 09:53:41.092182 aiZero-0.0.2a0/aiZero/static/js/
+-rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.2a0/aiZero/static/js/marked.min.js
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-10 09:53:41.092625 aiZero-0.0.2a0/aiZero/templates/
+-rw-r--r--   0 emhang     (501) staff       (20)    28537 2024-05-10 09:45:01.000000 aiZero-0.0.2a0/aiZero/templates/index.html
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-10 09:53:41.092049 aiZero-0.0.2a0/aiZero.egg-info/
+-rw-r--r--   0 emhang     (501) staff       (20)    12929 2024-05-10 09:53:41.000000 aiZero-0.0.2a0/aiZero.egg-info/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)      257 2024-05-10 09:53:41.000000 aiZero-0.0.2a0/aiZero.egg-info/SOURCES.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-10 09:53:41.000000 aiZero-0.0.2a0/aiZero.egg-info/dependency_links.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       40 2024-05-10 09:53:41.000000 aiZero-0.0.2a0/aiZero.egg-info/requires.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-10 09:53:41.000000 aiZero-0.0.2a0/aiZero.egg-info/top_level.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-10 09:53:41.093263 aiZero-0.0.2a0/setup.cfg
+-rw-r--r--   0 emhang     (501) staff       (20)      819 2024-05-10 08:35:41.000000 aiZero-0.0.2a0/setup.py
```

### Comparing `aiZero-0.0.1a4/PKG-INFO` & `aiZero-0.0.2a0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: aiZero
-Version: 0.0.1a4
-Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
-Home-page: UNKNOWN
-Author: emhang
-Author-email: emhang@126.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 aiZero是一个简单易用的可以连接常用人工智能接口，快速搭建可视化本地web应用的Python第三方库，适配幻码人工智能初阶课程。
 
 ### 快速开始
 
 ```python
 from aiZero import AIWebApp
 
@@ -311,15 +299,15 @@
 app.add_record()
 app.add_submit(my_ai_function)
 app.run(port=6060)
 ```
 
 #### 同时输出多种不同类型的信息
 
-aiZero支持输出文字、音频和图像等多种不同类型的信息，但每种类型的信息只能为一个（即不支持一次性输出2张图像、2段音频），且必须同时推送到前端。例如，我们可以输入文字，同时以文本和音频形式输出AI的响应。
+aiZero支持同时输出文字、音频和图像等多种不同类型的信息，但每种类型的信息只能为一个。例如，我们可以输入文字，同时以文本和音频形式输出AI的响应。
 
 ```python
 from aiZero import AIWebApp, text_generation, speech_synthesis
 
 def my_ai_function():
     text = app.input_text
     chat_history.append(text)
@@ -332,9 +320,91 @@
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
 app.add_input_text()
 app.add_submit(my_ai_function)
 app.run(port=6060)
 ```
 
+#### 同次分时输出多个信息
+
+`aiZero`也支持在一次大模型交互的输出时，分不同时间输出不同信息。例如，我们制作一个绘图助手，它可以将用户输入的简易文字信息扩充为详细的画面信息后，再交给图像生成功能完成图像的创作。在这个功能设计中，AI的文字回复响应很快而图像生成响应较慢，因此应当在不同时间推送至前端。
+
+```python
+from aiZero import AIWebApp, text_generation, image_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    reply = text_generation(chat_history, prompt='你是一个人工智能绘图助手，你负责将用户输入信息中描述的画面扩充为详细的绘图AI的提示词')
+    chat_history.append(reply)
+    # 结果推送时包含'running'键，则会继续监听输出结果
+    app.results.append({'text': reply, 'running': True})
+    img = image_generation(reply)
+    # 结果推送时不包含'running'键，则输出结束
+    app.results.append({'image': img})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+为了能让前端在收到第一次的文本输出后不会结束对其他输出的监听，必须在输出未完全结束时，在结果中添加`'running'`键，而在输出完全结束时，推送不包含`'running'`键的结果。
+
+#### 文本流式输出
+
+在大模型文字交互（`text_generation`）、图像理解（`image_understanding`）、声音理解（`audio_understanding`）等功能中，大模型回复的文本信息支持以流式形式输出，即逐步输出文本内容而非一次性输出全部文本。设置方法只需要将函数的可选参数`stream`设为`True`即可，以基础的文字交互为例：
+
+```python
+from aiZero import AIWebApp, text_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    # 设置stream参数值为True，返回值是一个生成器，可用for循环迭代地输出结果
+    reply = text_generation(chat_history, stream=True)
+    for r in reply:
+        # 流式输出过程中，结果推送时须包含'running'键
+        app.results.append({'text': r, 'running': True})
+    chat_history.append(r)
+    # 最后，必须再次推送一个不包含'running'键的结果，才能结束输出
+    app.results.append({'text': r})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+#### 错误信息的捕获与处理
+
+在`aiZero`中，所有错误信息都会以`'错误:'`作为开始部分输出，因此，可以在获取输出信息时，先判断是否为错误信息，再进行相应的推送。
+
+```python
+from aiZero import AIWebApp, text_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    reply = text_generation(chat_history)
+    if reply.startswith('错误:'):
+        app.results.append({'text': reply})
+        chat_history.pop()
+    else:
+        chat_history.append(reply)
+        app.results.append({'text': reply})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
 
 
+####
```

### Comparing `aiZero-0.0.1a4/README.md` & `aiZero-0.0.2a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: aiZero
+Version: 0.0.2a0
+Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
+Home-page: UNKNOWN
+Author: emhang
+Author-email: emhang@126.com
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 aiZero是一个简单易用的可以连接常用人工智能接口，快速搭建可视化本地web应用的Python第三方库，适配幻码人工智能初阶课程。
 
 ### 快速开始
 
 ```python
 from aiZero import AIWebApp
 
@@ -299,15 +311,15 @@
 app.add_record()
 app.add_submit(my_ai_function)
 app.run(port=6060)
 ```
 
 #### 同时输出多种不同类型的信息
 
-aiZero支持输出文字、音频和图像等多种不同类型的信息，但每种类型的信息只能为一个（即不支持一次性输出2张图像、2段音频），且必须同时推送到前端。例如，我们可以输入文字，同时以文本和音频形式输出AI的响应。
+aiZero支持同时输出文字、音频和图像等多种不同类型的信息，但每种类型的信息只能为一个。例如，我们可以输入文字，同时以文本和音频形式输出AI的响应。
 
 ```python
 from aiZero import AIWebApp, text_generation, speech_synthesis
 
 def my_ai_function():
     text = app.input_text
     chat_history.append(text)
@@ -320,7 +332,93 @@
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
 app.add_input_text()
 app.add_submit(my_ai_function)
 app.run(port=6060)
 ```
 
+#### 同次分时输出多个信息
+
+`aiZero`也支持在一次大模型交互的输出时，分不同时间输出不同信息。例如，我们制作一个绘图助手，它可以将用户输入的简易文字信息扩充为详细的画面信息后，再交给图像生成功能完成图像的创作。在这个功能设计中，AI的文字回复响应很快而图像生成响应较慢，因此应当在不同时间推送至前端。
+
+```python
+from aiZero import AIWebApp, text_generation, image_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    reply = text_generation(chat_history, prompt='你是一个人工智能绘图助手，你负责将用户输入信息中描述的画面扩充为详细的绘图AI的提示词')
+    chat_history.append(reply)
+    # 结果推送时包含'running'键，则会继续监听输出结果
+    app.results.append({'text': reply, 'running': True})
+    img = image_generation(reply)
+    # 结果推送时不包含'running'键，则输出结束
+    app.results.append({'image': img})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+为了能让前端在收到第一次的文本输出后不会结束对其他输出的监听，必须在输出未完全结束时，在结果中添加`'running'`键，而在输出完全结束时，推送不包含`'running'`键的结果。
+
+#### 文本流式输出
+
+在大模型文字交互（`text_generation`）、图像理解（`image_understanding`）、声音理解（`audio_understanding`）等功能中，大模型回复的文本信息支持以流式形式输出，即逐步输出文本内容而非一次性输出全部文本。设置方法只需要将函数的可选参数`stream`设为`True`即可，以基础的文字交互为例：
+
+```python
+from aiZero import AIWebApp, text_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    # 设置stream参数值为True，返回值是一个生成器，可用for循环迭代地输出结果
+    reply = text_generation(chat_history, stream=True)
+    for r in reply:
+        # 流式输出过程中，结果推送时须包含'running'键
+        app.results.append({'text': r, 'running': True})
+    chat_history.append(r)
+    # 最后，必须再次推送一个不包含'running'键的结果，才能结束输出
+    app.results.append({'text': r})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+#### 错误信息的捕获与处理
+
+在`aiZero`中，所有错误信息都会以`'错误:'`作为开始部分输出，因此，可以在获取输出信息时，先判断是否为错误信息，再进行相应的推送。
+
+```python
+from aiZero import AIWebApp, text_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    reply = text_generation(chat_history)
+    if reply.startswith('错误:'):
+        app.results.append({'text': reply})
+        chat_history.pop()
+    else:
+        chat_history.append(reply)
+        app.results.append({'text': reply})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+
+
+#### 
+
+
```

### Comparing `aiZero-0.0.1a4/aiZero/__init__.py` & `aiZero-0.0.2a0/aiZero/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,21 @@
 
 
 def resolve_resource_path(path):
     return Path(RESOURCE_PATH / path).resolve()
 
 
 # 1. 大模型文字交互
-def text_generation(chat_history, prompt='你是一个人工智能助手，你的名字叫小H'):
+def text_generation(chat_history, prompt='你是一个人工智能助手，你的名字叫小H', stream=False):
+    def generator():
+        for r in response:
+            if r.status_code == HTTPStatus.OK:
+                yield r.output.choices[0]['message']['content']
+            else:
+                return "错误: " + r.message
     try:
         result = words_check(chat_history[-1])
         if result['status'] == 'error':
             return result['message']
         result = words_check(prompt)
         if result['status'] == 'error':
             return result['message']
@@ -35,25 +41,29 @@
                     messages.append({'role': 'user', 'content': content})
                 else:
                     messages.append({'role': 'assistant', 'content': content})
             else:
                 return '输入参数错误'
         response = dashscope.Generation.call(model="qwen-plus",
                                              messages=messages,
-                                             result_format='message')
-        if response.status_code == HTTPStatus.OK:
-            return response.output.choices[0]['message']['content']
+                                             result_format='message',
+                                             stream=stream)
+        if stream:
+            return generator()
         else:
-            return "错误: " + response.message
+            if response.status_code == HTTPStatus.OK:
+                return response.output.choices[0]['message']['content']
+            else:
+                return "错误: " + response.message
     except Exception as e:
         return "错误: " + str(e)
 
 
 # 2. 大模型图像理解
-def image_understanding(img, chat_history, prompt='你是一名人工智能助手'):
+def image_understanding(img, chat_history, prompt='你是一名人工智能助手', stream=False):
     try:
         result = words_check(chat_history[-1])
         if result['status'] == 'error':
             return result['message']
         result = words_check(prompt)
         if result['status'] == 'error':
             return result['message']
@@ -63,25 +73,33 @@
 
         for index, content in enumerate(chat_history[1:]):
             if index % 2 == 0:
                 messages.append({'role': 'assistant', 'content': [{'text': content}]})
             else:
                 messages.append({'role': 'user', 'content': [{'text': content}]})
         response = dashscope.MultiModalConversation.call(model='qwen-vl-plus',
-                                                         messages=messages)
-        if response.status_code == HTTPStatus.OK:
-            return response.output.choices[0].message.content[0]['text']
+                                                         messages=messages,
+                                                         stream=stream)
+        if stream:
+            for r in response:
+                if r.status_code == HTTPStatus.OK:
+                    yield r.output.choices[0].message.content[0]['text']
+                else:
+                    return "错误: " + r.message
         else:
-            return "错误: " + response.message
+            if response.status_code == HTTPStatus.OK:
+                return response.output.choices[0].message.content[0]['text']
+            else:
+                return "错误: " + response.message
     except Exception as e:
         return "错误: " + str(e)
 
 
 # 3. 大模型声音理解
-def audio_understanding(audio, chat_history, prompt='你是一名人工智能助手'):
+def audio_understanding(audio, chat_history, prompt='你是一名人工智能助手', stream=False):
     try:
         result = words_check(chat_history[-1])
         if result['status'] == 'error':
             return result['message']
         result = words_check(prompt)
         if result['status'] == 'error':
             return result['message']
@@ -90,19 +108,27 @@
                     {'role': 'user', 'content': [{'audio': audio_url}, {'text': chat_history[0]}]}]
         for index, content in enumerate(chat_history[1:]):
             if index % 2 == 0:
                 messages.append({'role': 'assistant', 'content': [{'text': content}]})
             else:
                 messages.append({'role': 'user', 'content': [{'text': content}]})
         response = dashscope.MultiModalConversation.call(model='qwen-audio-turbo',
-                                                         messages=messages)
-        if response.status_code == HTTPStatus.OK:
-            return response.output.choices[0].message.content[0]['text']
+                                                         messages=messages,
+                                                         stream=stream)
+        if stream:
+            for r in response:
+                if r.status_code == HTTPStatus.OK:
+                    yield r.output.choices[0].message.content[0]['text']
+                else:
+                    return "错误: " + r.message
         else:
-            return "错误: " + response.message
+            if response.status_code == HTTPStatus.OK:
+                return response.output.choices[0].message.content[0]['text']
+            else:
+                return "错误: " + response.message
     except Exception as e:
         return "错误: " + str(e)
 
 
 # 4. 大模型图像生成
 def image_generation(prompt):
     try:
@@ -436,15 +462,19 @@
                 response['audio'] = self.input_audio
             return jsonify(response)
 
         @self.app.route('/result', methods=['GET'])
         def get_result():
             if self.results:
                 new_result = self.results.pop()
-                new_result['status'] = 'finish'
+                self.results.clear()
+                if 'running' in new_result:
+                    new_result['status'] = 'processing'
+                else:
+                    new_result['status'] = 'finish'
                 return jsonify(new_result)
             return jsonify({"status": "processing", "content": ""})
 
         @self.app.route('/static/audios/<filename>')
         def audio_file(filename):
             return send_from_directory('static/audios', filename)
```

### Comparing `aiZero-0.0.1a4/aiZero/static/js/marked.min.js` & `aiZero-0.0.2a0/aiZero/static/js/marked.min.js`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a4/aiZero/templates/index.html` & `aiZero-0.0.2a0/aiZero/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,24 @@
       }
 
       .ai-display {
           background: #fff;
           padding: 10px;
       }
 
+      .ai-display-text {
+          background: #fff;
+          padding: 10px;
+      }
+
       .loading-message{
-        font-weight: bold;
-        color: #4CAF50;
-        margin: 20px 0;
+          height: 20px;
+          font-weight: bold;
+          color: #4CAF50;
+          margin: 10px 0;
         }
 
       img {
         max-width: 100%;
         height: auto;
       }
 
@@ -141,39 +147,39 @@
                 document.body.appendChild(outputArea);
             }
             return outputArea;
         }
 
         function updateContent(data) {
             const outputArea = createOrUpdateOutputArea();
-            // if (data.type === 'text') {
-            //     outputArea.innerHTML = `<p>${data.content}</p>`;
-            // } else if (data.type === 'image') {
-            //     outputArea.innerHTML = `<img src="${data.content}" alt="AI generated image" />`;
-            // } else if (data.type === 'audio') {
-            //     outputArea.innerHTML = `<audio controls src="${data.content}"></audio>`;
-            // }
             if (data.image) {
                 const userText = document.createElement('p');
                 userText.className = 'ai-display';
                 userText.innerHTML = `AI: <img src="${data.image}" alt="user input image" class="image-show" />`;
                 outputArea.appendChild(userText);
             }
             if (data.audio) {
                 const userText = document.createElement('p');
                 userText.className = 'ai-display';
                 userText.innerHTML = `AI: <audio controls autoplay src="${data.audio}"></audio>`;
                 outputArea.appendChild(userText);
             }
             if (data.text) {
-                const userText = document.createElement('p');
-                userText.className = 'ai-display';
-                userText.innerHTML = `${convertMarkdownToHTML('AI: ' + data.text)}`;
-                outputArea.appendChild(userText);
+                const textContent = convertMarkdownToHTML('AI: ' + data.text);
+                const existingTextElement = outputArea.querySelector('.ai-display-text');
+                if (existingTextElement) {
+                    existingTextElement.innerHTML = textContent;
+                } else {
+                    const userText = document.createElement('p');
+                    userText.className = 'ai-display-text';
+                    userText.innerHTML = textContent;
+                    outputArea.appendChild(userText);
+                }
             }
+            outputArea.scrollTop = outputArea.scrollHeight;
         }
 
         window.onload = function() {
             fetch('/get_components')
                 .then(response => response.json())
                 .then(components => {
                     components.forEach(component => {
@@ -308,31 +314,36 @@
                                         userText.innerHTML = `用户: <audio controls src="${data.audio}"></audio>`;
                                         outputArea.appendChild(userText);
                                     }
                                     if (data.text) {
                                         const userText = document.createElement('p');
                                         userText.className = 'user-display';
                                         userText.innerHTML = `${convertMarkdownToHTML('用户: ' + data.text.replace(/\n/g, "\n\n"))}`;
-                                        // userText.textContent = `用户: ${data.text}`;
                                         outputArea.appendChild(userText);
                                     }
+                                    outputArea.scrollTop = outputArea.scrollHeight;
                                     const loading = document.getElementById('loadingMsg');
                                     loading.textContent = '等待AI响应中';
                                     loading.style.display = 'flex';
                                     const submitButton = document.getElementById('submitButton');
                                     submitButton.disabled = true;
                                     const intervalId = setInterval(() => {
                                         fetch('/result')
                                         .then(response => response.json())
                                         .then(data => {
                                             updateContent(data);
                                             if (data.status !== "processing") {
                                                 clearInterval(intervalId);
-                                                loading.style.display = 'none';
+                                                // loading.style.display = 'none';
+                                                loading.textContent = '';
                                                 submitButton.disabled = false;
+                                                const textDiv = outputArea.querySelector('.ai-display-text');
+                                                if (textDiv){
+                                                    textDiv.className = 'ai-display';
+                                                }
                                             }
                                             else {
                                                 let text = loading.textContent;
                                                 if (text.length >= 17) {
                                                     loading.textContent = '等待AI响应中';
                                                 }
                                                 else {
```

### Comparing `aiZero-0.0.1a4/aiZero.egg-info/PKG-INFO` & `aiZero-0.0.2a0/aiZero.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiZero
-Version: 0.0.1a4
+Version: 0.0.2a0
 Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
 Home-page: UNKNOWN
 Author: emhang
 Author-email: emhang@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -311,15 +311,15 @@
 app.add_record()
 app.add_submit(my_ai_function)
 app.run(port=6060)
 ```
 
 #### 同时输出多种不同类型的信息
 
-aiZero支持输出文字、音频和图像等多种不同类型的信息，但每种类型的信息只能为一个（即不支持一次性输出2张图像、2段音频），且必须同时推送到前端。例如，我们可以输入文字，同时以文本和音频形式输出AI的响应。
+aiZero支持同时输出文字、音频和图像等多种不同类型的信息，但每种类型的信息只能为一个。例如，我们可以输入文字，同时以文本和音频形式输出AI的响应。
 
 ```python
 from aiZero import AIWebApp, text_generation, speech_synthesis
 
 def my_ai_function():
     text = app.input_text
     chat_history.append(text)
@@ -332,9 +332,93 @@
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
 app.add_input_text()
 app.add_submit(my_ai_function)
 app.run(port=6060)
 ```
 
+#### 同次分时输出多个信息
+
+`aiZero`也支持在一次大模型交互的输出时，分不同时间输出不同信息。例如，我们制作一个绘图助手，它可以将用户输入的简易文字信息扩充为详细的画面信息后，再交给图像生成功能完成图像的创作。在这个功能设计中，AI的文字回复响应很快而图像生成响应较慢，因此应当在不同时间推送至前端。
+
+```python
+from aiZero import AIWebApp, text_generation, image_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    reply = text_generation(chat_history, prompt='你是一个人工智能绘图助手，你负责将用户输入信息中描述的画面扩充为详细的绘图AI的提示词')
+    chat_history.append(reply)
+    # 结果推送时包含'running'键，则会继续监听输出结果
+    app.results.append({'text': reply, 'running': True})
+    img = image_generation(reply)
+    # 结果推送时不包含'running'键，则输出结束
+    app.results.append({'image': img})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+为了能让前端在收到第一次的文本输出后不会结束对其他输出的监听，必须在输出未完全结束时，在结果中添加`'running'`键，而在输出完全结束时，推送不包含`'running'`键的结果。
+
+#### 文本流式输出
+
+在大模型文字交互（`text_generation`）、图像理解（`image_understanding`）、声音理解（`audio_understanding`）等功能中，大模型回复的文本信息支持以流式形式输出，即逐步输出文本内容而非一次性输出全部文本。设置方法只需要将函数的可选参数`stream`设为`True`即可，以基础的文字交互为例：
+
+```python
+from aiZero import AIWebApp, text_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    # 设置stream参数值为True，返回值是一个生成器，可用for循环迭代地输出结果
+    reply = text_generation(chat_history, stream=True)
+    for r in reply:
+        # 流式输出过程中，结果推送时须包含'running'键
+        app.results.append({'text': r, 'running': True})
+    chat_history.append(r)
+    # 最后，必须再次推送一个不包含'running'键的结果，才能结束输出
+    app.results.append({'text': r})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+#### 错误信息的捕获与处理
+
+在`aiZero`中，所有错误信息都会以`'错误:'`作为开始部分输出，因此，可以在获取输出信息时，先判断是否为错误信息，再进行相应的推送。
+
+```python
+from aiZero import AIWebApp, text_generation
+
+def my_ai_function():
+    text = app.input_text
+    chat_history.append(text)
+    reply = text_generation(chat_history)
+    if reply.startswith('错误:'):
+        app.results.append({'text': reply})
+        chat_history.pop()
+    else:
+        chat_history.append(reply)
+        app.results.append({'text': reply})
+
+chat_history = []
+app = AIWebApp(title='人工智能助手')
+app.set_apikey('YOUR_API_KEY')
+app.add_input_text()
+app.add_submit(my_ai_function)
+app.run(port=6060)
+```
+
+
+
+####
```

### Comparing `aiZero-0.0.1a4/setup.py` & `aiZero-0.0.2a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiZero",
-    version="0.0.1a4",
+    version="0.0.2a",
     author="emhang",
     author_email="emhang@126.com",
     description="A simple and easy-to-use library that connects to common artificial intelligence interfaces, "
                 "allowing for quick development of local web applications. "
                 "It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

