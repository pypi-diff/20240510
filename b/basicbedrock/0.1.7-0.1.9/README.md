# Comparing `tmp/basicbedrock-0.1.7.tar.gz` & `tmp/basicbedrock-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.1.7.tar", last modified: Wed Apr 24 17:00:24 2024, max compression
+gzip compressed data, was "basicbedrock-0.1.9.tar", last modified: Mon Apr 29 19:41:40 2024, max compression
```

## Comparing `basicbedrock-0.1.7.tar` & `basicbedrock-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 17:00:24.537974 basicbedrock-0.1.7/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.7/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-24 17:00:24.537718 basicbedrock-0.1.7/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.7/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-24 17:00:16.000000 basicbedrock-0.1.7/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-24 17:00:24.538030 basicbedrock-0.1.7/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 17:00:24.533326 basicbedrock-0.1.7/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 17:00:24.534462 basicbedrock-0.1.7/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-24 17:00:16.000000 basicbedrock-0.1.7/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    16145 2024-04-23 14:50:11.000000 basicbedrock-0.1.7/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 17:00:24.536574 basicbedrock-0.1.7/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3215 2024-04-24 16:48:37.000000 basicbedrock-0.1.7/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.7/src/basicbedrock/models/ai21.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.7/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.7/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.7/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.7/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3312 2024-04-24 16:55:21.000000 basicbedrock-0.1.7/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.7/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 17:00:24.537418 basicbedrock-0.1.7/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-24 17:00:24.000000 basicbedrock-0.1.7/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-24 17:00:24.000000 basicbedrock-0.1.7/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-24 17:00:24.000000 basicbedrock-0.1.7/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-24 17:00:24.000000 basicbedrock-0.1.7/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-24 17:00:24.000000 basicbedrock-0.1.7/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 17:00:24.536726 basicbedrock-0.1.7/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.7/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.806318 basicbedrock-0.1.9/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.9/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-29 19:41:40.806097 basicbedrock-0.1.9/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.9/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-29 19:41:32.000000 basicbedrock-0.1.9/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-29 19:41:40.806373 basicbedrock-0.1.9/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.800719 basicbedrock-0.1.9/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.801654 basicbedrock-0.1.9/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-29 19:41:32.000000 basicbedrock-0.1.9/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    17519 2024-04-29 19:41:32.000000 basicbedrock-0.1.9/src/basicbedrock/basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.804847 basicbedrock-0.1.9/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3215 2024-04-24 16:48:37.000000 basicbedrock-0.1.9/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.9/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.9/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.9/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.9/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.9/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3312 2024-04-24 16:55:21.000000 basicbedrock-0.1.9/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.9/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.805839 basicbedrock-0.1.9/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.805110 basicbedrock-0.1.9/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.9/test/tests.py
```

### Comparing `basicbedrock-0.1.7/LICENSE` & `basicbedrock-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/PKG-INFO` & `basicbedrock-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.7
+Version: 0.1.9
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.7/README.md` & `basicbedrock-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/pyproject.toml` & `basicbedrock-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.1.7"
+version = "0.1.9"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
```

### Comparing `basicbedrock-0.1.7/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.1.9/src/basicbedrock/basicbedrock.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import typing
 import warnings
 
 import boto3
 import pydantic
 
 from models import *
+from src import basicbedrock
 
 
 class BasicBedrock(object):
     def __init__(self, session: boto3.session.Session = None, **kwargs):
         """
         Creates an instance of basic bedrock.
         session param is optional.  If omitted, a default session constructor will be used.
@@ -42,35 +43,70 @@
         self._t = self._default_t
         self._n = self._default_n
         self._s = self._default_stop
         # set params according to kwargs
         if kwargs:
             self.set_params(kwargs)
 
-    def print_available_models(self) -> None:
+        # determine which models are enabled in AWS account and also supported by BasicBedrock
+        _bedrock_cp = session.client("bedrock")
+        r = _bedrock_cp.list_foundation_models()
+        self.enabled_models = [
+            e.get('modelId') for e in r['modelSummaries'] if e.get('modelLifecycle').get('status') == 'ACTIVE'
+        ]
+        self.available_models = sorted(
+            list(
+                set(
+                    self.enabled_models
+                ).intersection(
+                    set(
+                        BasicBedrock.get_supported_models()
+                    )
+                )
+            )
+        )
+
+    def print_available_models(self):
+        """
+        Prints available models that are supported by BasicBedrock and enabled in the aws account
+        :return:
         """
-        Prints all available models line by line
+        print(os.linesep.join(self.available_models))
+
+
+    def get_available_models(self):
+        """
+        Gets a list of available models that are supported by BasicBedrock and enabled in the aws account
+        :return: list of models both enabled and suported
+        """
+        return self.available_models
+
+    @staticmethod
+    def print_supported_models() -> None:
+        """
+        Prints all models supported by BasicBedrock, which may not be the same models a user has enabled within their account
         :return: None
         """
-        print(os.linesep.join(self.get_available_models()))
+        print(os.linesep.join(BasicBedrock.get_supported_models()))
 
-    def get_available_models(self) -> list:
+    @staticmethod
+    def get_supported_models() -> list:
         """
-        returns a list of all available models
+        returns a list of all models supported by BasicBedrock, which may not be the same models a user has enabled within their account
         :return: ["model1", "model2", "model3"...]
         """
         return sorted(model_request_mapping.keys())
 
     def get_model_schema_dict(self, model_id: str) -> dict:
         """
         returns a dict object representing the request scheme of model_id
         :param model_id:  the chosen model id
         :return: dict object representing the base request scheme of model_id
         """
-        if model_id not in self.get_available_models():
+        if model_id not in self.get_supported_models():
             raise ValueError(f"requested model {model_id} is not an available model")
         else:
             model = model_request_mapping.get(model_id)
             _inst = model()
             j = _inst.json()
             d = json.loads(j)
             return d
@@ -79,26 +115,26 @@
         """
         returns an instantiated object representing the schema for the chosen model.
         All these inherit from BaseSchemaAbstract.
         Its useful for when you want to use BaseSchemaAbstract to modify prompts and produce json or dicts manually
         :param model_id: the chosen model ID
         :return: the schema class object for the chosen model, it will be a subclass of a BaseAbstractRequest
         """
-        if model_id not in self.get_available_models():
+        if model_id not in self.get_supported_models():
             raise ValueError(f"requested model {model_id} is not an available model")
         _inst = model_request_mapping.get(model_id)()
         return _inst
 
     def get_model_request_json(self, model_id: str) -> str:
         """
         returns a string object representing the request scheme of model_id in json format
         :param model_id:  the chosen model id
         :return: a json string
         """
-        if model_id not in self.get_available_models():
+        if model_id not in self.get_supported_models():
             raise ValueError(f"requested model {model_id} is not an available model")
         else:
             model = model_request_mapping.get(model_id)
             _inst = model()
             j = _inst.json()
             return j
 
@@ -106,15 +142,15 @@
         """
         prints the request scheme of model_id in a pretty format.
         if indent is not None, indent the lines when printing
         :param model_id: the chosen model id
         :param indent: how many spaces to indent, default=4
         :return: None
         """
-        if model_id not in self.get_available_models():
+        if model_id not in self.get_supported_models():
             raise ValueError(f"requested model {model_id} is not an available model")
         else:
             model = model_request_mapping.get(model_id)
             _inst = model()
             j = _inst.json()
             if indent:
                 j = json.dumps(json.loads(j), indent=indent)
@@ -126,15 +162,15 @@
         but it will not invoke bedrock or pass it to boto3, it will simply return the boto3 'body' param as a string.
         Internally, this calls the update_prompt() function, not update_prompt_raw(), which means that it will take into account
         the expected calling convention of the underlying model by inserting things such as 'Human:' or '<s>[INST]' as appropriate
         :param model_id: the model to construct a boto3 body for
         :param prompt: the prompt to pass the model.
         :return: a string, representing the equivalent boto3 'body' parameter.
         """
-        if model_id not in self.get_available_models():
+        if model_id not in self.get_supported_models():
             raise ValueError(f"requested model {model_id} is not an available model")
         if not isinstance(prompt, str):
             raise ValueError(f"prompt must be a string, but got {type(prompt)}")
         schema = model_request_mapping.get(model_id)
         schema_inst: BaseAbstractRequest = schema()
         schema_inst.set_prompt(prompt)
         schema_inst.set_params(self.params)
@@ -426,7 +462,8 @@
     @stop_words.deleter
     def stop_words(self):
         """
         resets the stop_words parameter
         :return:
         """
         self._s = self._default_stop
+
```

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/__init__.py` & `basicbedrock-0.1.9/src/basicbedrock/models/__init__.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/ai21.py` & `basicbedrock-0.1.9/src/basicbedrock/models/ai21.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/amazon.py` & `basicbedrock-0.1.9/src/basicbedrock/models/amazon.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/anthropic.py` & `basicbedrock-0.1.9/src/basicbedrock/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.1.9/src/basicbedrock/models/baseclasses.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/cohere.py` & `basicbedrock-0.1.9/src/basicbedrock/models/cohere.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/meta.py` & `basicbedrock-0.1.9/src/basicbedrock/models/meta.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock/models/mistral.py` & `basicbedrock-0.1.9/src/basicbedrock/models/mistral.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.1.9/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.7
+Version: 0.1.9
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.7/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.1.9/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.7/test/tests.py` & `basicbedrock-0.1.9/test/tests.py`

 * *Files identical despite different names*

