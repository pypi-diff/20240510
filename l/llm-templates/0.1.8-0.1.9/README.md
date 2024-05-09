# Comparing `tmp/llm-templates-0.1.8.tar.gz` & `tmp/llm_templates-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-templates-0.1.8.tar", last modified: Sun Mar 31 18:46:55 2024, max compression
+gzip compressed data, was "llm_templates-0.1.9.tar", last modified: Thu May  9 22:02:06 2024, max compression
```

## Comparing `llm-templates-0.1.8.tar` & `llm_templates-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:46:55.679192 llm-templates-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-31 18:46:51.000000 llm-templates-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-31 18:46:55.679192 llm-templates-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-03-31 18:46:51.000000 llm-templates-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:46:55.679192 llm-templates-0.1.8/llm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:46:55.679192 llm-templates-0.1.8/llm_templates/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/formats/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/formats/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/formats/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/formats/zephyr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-31 18:46:51.000000 llm-templates-0.1.8/llm_templates/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:46:55.679192 llm-templates-0.1.8/llm_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-31 18:46:55.000000 llm-templates-0.1.8/llm_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-31 18:46:55.000000 llm-templates-0.1.8/llm_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:46:55.000000 llm-templates-0.1.8/llm_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-31 18:46:55.000000 llm-templates-0.1.8/llm_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-31 18:46:55.000000 llm-templates-0.1.8/llm_templates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 18:46:55.679192 llm-templates-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-31 18:46:51.000000 llm-templates-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:02:06.261210 llm_templates-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-09 22:02:02.000000 llm_templates-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-09 22:02:06.261210 llm_templates-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-09 22:02:02.000000 llm_templates-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:02:06.257210 llm_templates-0.1.9/llm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:02:06.261210 llm_templates-0.1.9/llm_templates/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/formats/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/formats/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/formats/llama3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/formats/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/formats/zephyr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-09 22:02:02.000000 llm_templates-0.1.9/llm_templates/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:02:06.261210 llm_templates-0.1.9/llm_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-09 22:02:06.000000 llm_templates-0.1.9/llm_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 22:02:06.000000 llm_templates-0.1.9/llm_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:02:06.000000 llm_templates-0.1.9/llm_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 22:02:06.000000 llm_templates-0.1.9/llm_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 22:02:06.000000 llm_templates-0.1.9/llm_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:02:06.261210 llm_templates-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-09 22:02:02.000000 llm_templates-0.1.9/setup.py
```

### Comparing `llm-templates-0.1.8/LICENSE` & `llm_templates-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-templates-0.1.8/PKG-INFO` & `llm_templates-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-templates
-Version: 0.1.8
+Version: 0.1.9
 Summary: Instruction/chat prompts creation library for text generation LLMs. It supports local and Hugging Face models.
 Home-page: https://github.com/jpmanson/llm-templates
 Author: Juan Pablo Manson
 Author-email: jpmanson@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,17 +23,42 @@
 You can quick start with the library using the following [Colab notebook](https://colab.research.google.com/drive/187sA0rGwVLiP6A3IyvV0ICglsJQmvQa3#scrollTo=sUjN9PDx-dcp):
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/187sA0rGwVLiP6A3IyvV0ICglsJQmvQa3#scrollTo=sUjN9PDx-dcp)
 
 The library has built in templates for the following models:
 - `zephyr`
 - `llama2`
+- `llama3`
 - `mistral`
 - `gemma`
 
+This is a quick example with Llama3 model:
+```python
+from llm_templates import Formatter, Conversation, Content
+
+messages = [Content(role="user", content="Hello!"),
+            Content(role="assistant", content="How can I help you?"),
+            Content(role="user", content="Write a poem about the sea")]
+
+conversation = Conversation(model='llama3', messages=messages)
+conversation_str = Formatter().render(conversation, add_assistant_prompt=True)
+
+print(conversation_str)
+```
+And the result will be:
+```
+<|begin_of_text|><|start_header_id|>user<|end_header_id|>
+Hello!<|eot_id|>
+<|start_header_id|>assistant<|end_header_id|>
+How can I help you?<|eot_id|>
+<|start_header_id|>user<|end_header_id|>
+Write a poem about the sea<|eot_id|>
+<|start_header_id|>assistant<|end_header_id|>
+```
+
 And HuggingFace models, using [Jinja2](https://github.com/pallets/jinja) templates when tokenizer_config.json file is available.
 
 ## Introduction
 
 Many models are based on foundational or pre-trained LLMs, which are then retrained (fin-tuning) with specially designed instruction datasets to improve and refine the abilities of these models on specific tasks:
 
 ![transfer_learning](images/transfer_learning.png)
@@ -200,7 +225,8 @@
 ```
 
 ## References
 
 - [Chat Templates](https://huggingface.co/blog/chat-templates)
 - [stanford_alpaca](https://github.com/tatsu-lab/stanford_alpaca#data-release)
 - [Gemma Formatting](https://ai.google.dev/gemma/docs/formatting?hl=es-419)
+- [Meta Llama 3 chat](https://llama.meta.com/docs/model-cards-and-prompt-formats/meta-llama-3/)
```

### Comparing `llm-templates-0.1.8/README.md` & `llm_templates-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,42 @@
 You can quick start with the library using the following [Colab notebook](https://colab.research.google.com/drive/187sA0rGwVLiP6A3IyvV0ICglsJQmvQa3#scrollTo=sUjN9PDx-dcp):
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/187sA0rGwVLiP6A3IyvV0ICglsJQmvQa3#scrollTo=sUjN9PDx-dcp)
 
 The library has built in templates for the following models:
 - `zephyr`
 - `llama2`
+- `llama3`
 - `mistral`
 - `gemma`
 
+This is a quick example with Llama3 model:
+```python
+from llm_templates import Formatter, Conversation, Content
+
+messages = [Content(role="user", content="Hello!"),
+            Content(role="assistant", content="How can I help you?"),
+            Content(role="user", content="Write a poem about the sea")]
+
+conversation = Conversation(model='llama3', messages=messages)
+conversation_str = Formatter().render(conversation, add_assistant_prompt=True)
+
+print(conversation_str)
+```
+And the result will be:
+```
+<|begin_of_text|><|start_header_id|>user<|end_header_id|>
+Hello!<|eot_id|>
+<|start_header_id|>assistant<|end_header_id|>
+How can I help you?<|eot_id|>
+<|start_header_id|>user<|end_header_id|>
+Write a poem about the sea<|eot_id|>
+<|start_header_id|>assistant<|end_header_id|>
+```
+
 And HuggingFace models, using [Jinja2](https://github.com/pallets/jinja) templates when tokenizer_config.json file is available.
 
 ## Introduction
 
 Many models are based on foundational or pre-trained LLMs, which are then retrained (fin-tuning) with specially designed instruction datasets to improve and refine the abilities of these models on specific tasks:
 
 ![transfer_learning](images/transfer_learning.png)
@@ -186,8 +211,9 @@
 ....
 ```
 
 ## References
 
 - [Chat Templates](https://huggingface.co/blog/chat-templates)
 - [stanford_alpaca](https://github.com/tatsu-lab/stanford_alpaca#data-release)
-- [Gemma Formatting](https://ai.google.dev/gemma/docs/formatting?hl=es-419)
+- [Gemma Formatting](https://ai.google.dev/gemma/docs/formatting?hl=es-419)
+- [Meta Llama 3 chat](https://llama.meta.com/docs/model-cards-and-prompt-formats/meta-llama-3/)
```

### Comparing `llm-templates-0.1.8/llm_templates/common.py` & `llm_templates-0.1.9/llm_templates/common.py`

 * *Files identical despite different names*

### Comparing `llm-templates-0.1.8/llm_templates/formats/gemma.py` & `llm_templates-0.1.9/llm_templates/formats/gemma.py`

 * *Files identical despite different names*

### Comparing `llm-templates-0.1.8/llm_templates/formats/llama2.py` & `llm_templates-0.1.9/llm_templates/formats/llama2.py`

 * *Files identical despite different names*

### Comparing `llm-templates-0.1.8/llm_templates/formats/mistral.py` & `llm_templates-0.1.9/llm_templates/formats/mistral.py`

 * *Files identical despite different names*

### Comparing `llm-templates-0.1.8/llm_templates/formats/zephyr.py` & `llm_templates-0.1.9/llm_templates/formats/zephyr.py`

 * *Files identical despite different names*

### Comparing `llm-templates-0.1.8/llm_templates/formatter.py` & `llm_templates-0.1.9/llm_templates/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from llm_templates.common import Conversation, get_jinja_env
 import requests
 import os
 import json
-from llm_templates.formats import zephyr, mistral, llama2, gemma
+from llm_templates.formats import zephyr, mistral, llama2, gemma, llama3
 
 HF_URL = 'https://huggingface.co/'
 
 
 class Formatter:
     def __init__(self, model_name: str = None, use_cache: bool = True,
                  clear_cache_on_create: bool = False, huggingface_api_key: str = None):
```

### Comparing `llm-templates-0.1.8/llm_templates.egg-info/PKG-INFO` & `llm_templates-0.1.9/llm_templates.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-templates
-Version: 0.1.8
+Version: 0.1.9
 Summary: Instruction/chat prompts creation library for text generation LLMs. It supports local and Hugging Face models.
 Home-page: https://github.com/jpmanson/llm-templates
 Author: Juan Pablo Manson
 Author-email: jpmanson@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,17 +23,42 @@
 You can quick start with the library using the following [Colab notebook](https://colab.research.google.com/drive/187sA0rGwVLiP6A3IyvV0ICglsJQmvQa3#scrollTo=sUjN9PDx-dcp):
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/187sA0rGwVLiP6A3IyvV0ICglsJQmvQa3#scrollTo=sUjN9PDx-dcp)
 
 The library has built in templates for the following models:
 - `zephyr`
 - `llama2`
+- `llama3`
 - `mistral`
 - `gemma`
 
+This is a quick example with Llama3 model:
+```python
+from llm_templates import Formatter, Conversation, Content
+
+messages = [Content(role="user", content="Hello!"),
+            Content(role="assistant", content="How can I help you?"),
+            Content(role="user", content="Write a poem about the sea")]
+
+conversation = Conversation(model='llama3', messages=messages)
+conversation_str = Formatter().render(conversation, add_assistant_prompt=True)
+
+print(conversation_str)
+```
+And the result will be:
+```
+<|begin_of_text|><|start_header_id|>user<|end_header_id|>
+Hello!<|eot_id|>
+<|start_header_id|>assistant<|end_header_id|>
+How can I help you?<|eot_id|>
+<|start_header_id|>user<|end_header_id|>
+Write a poem about the sea<|eot_id|>
+<|start_header_id|>assistant<|end_header_id|>
+```
+
 And HuggingFace models, using [Jinja2](https://github.com/pallets/jinja) templates when tokenizer_config.json file is available.
 
 ## Introduction
 
 Many models are based on foundational or pre-trained LLMs, which are then retrained (fin-tuning) with specially designed instruction datasets to improve and refine the abilities of these models on specific tasks:
 
 ![transfer_learning](images/transfer_learning.png)
@@ -200,7 +225,8 @@
 ```
 
 ## References
 
 - [Chat Templates](https://huggingface.co/blog/chat-templates)
 - [stanford_alpaca](https://github.com/tatsu-lab/stanford_alpaca#data-release)
 - [Gemma Formatting](https://ai.google.dev/gemma/docs/formatting?hl=es-419)
+- [Meta Llama 3 chat](https://llama.meta.com/docs/model-cards-and-prompt-formats/meta-llama-3/)
```

### Comparing `llm-templates-0.1.8/setup.py` & `llm_templates-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 
 README = (Path(__file__).parent/"README.md").read_text()
 
 setuptools.setup(
     name="llm-templates",
-    version="0.1.8",
+    version="0.1.9",
     author="Juan Pablo Manson",
     author_email="jpmanson@gmail.com",
     description="Instruction/chat prompts creation library for text generation LLMs. It supports local and Hugging Face models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jpmanson/llm-templates",
     packages=setuptools.find_packages(),
```

