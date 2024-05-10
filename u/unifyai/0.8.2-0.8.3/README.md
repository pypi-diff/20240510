# Comparing `tmp/unifyai-0.8.2.tar.gz` & `tmp/unifyai-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.8.2.tar", max compression
+gzip compressed data, was "unifyai-0.8.3.tar", max compression
```

## Comparing `unifyai-0.8.2.tar` & `unifyai-0.8.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11336 2024-04-29 10:34:46.881584 unifyai-0.8.2/LICENSE
--rw-r--r--   0        0        0     6589 2024-04-29 19:44:46.290194 unifyai-0.8.2/README.md
--rw-r--r--   0        0        0     1041 2024-04-29 19:45:50.778195 unifyai-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      199 2024-04-29 19:44:46.294194 unifyai-0.8.2/unify/__init__.py
--rw-r--r--   0        0        0     6875 2024-04-29 19:44:46.294194 unifyai-0.8.2/unify/chat.py
--rw-r--r--   0        0        0    15137 2024-04-29 19:44:46.294194 unifyai-0.8.2/unify/clients.py
--rw-r--r--   0        0        0     1166 2024-04-29 10:34:46.885583 unifyai-0.8.2/unify/exceptions.py
--rw-r--r--   0        0        0     4321 2024-04-29 10:34:46.885583 unifyai-0.8.2/unify/tests.py
--rw-r--r--   0        0        0     3472 2024-04-29 19:44:46.302193 unifyai-0.8.2/unify/utils.py
--rw-r--r--   0        0        0     7250 1970-01-01 00:00:00.000000 unifyai-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-05-10 14:28:57.440153 unifyai-0.8.3/LICENSE
+-rw-r--r--   0        0        0     6589 2024-05-10 14:28:57.440153 unifyai-0.8.3/README.md
+-rw-r--r--   0        0        0     1041 2024-05-10 14:31:17.908152 unifyai-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-10 14:28:57.440153 unifyai-0.8.3/unify/__init__.py
+-rw-r--r--   0        0        0     6876 2024-05-10 14:28:57.440153 unifyai-0.8.3/unify/chat.py
+-rw-r--r--   0        0        0    15138 2024-05-10 14:28:57.440153 unifyai-0.8.3/unify/clients.py
+-rw-r--r--   0        0        0     1166 2024-05-10 14:28:57.440153 unifyai-0.8.3/unify/exceptions.py
+-rw-r--r--   0        0        0     4321 2024-05-10 14:28:57.440153 unifyai-0.8.3/unify/tests.py
+-rw-r--r--   0        0        0     3472 2024-05-10 14:28:57.444153 unifyai-0.8.3/unify/utils.py
+-rw-r--r--   0        0        0     7250 1970-01-01 00:00:00.000000 unifyai-0.8.3/PKG-INFO
```

### Comparing `unifyai-0.8.2/LICENSE` & `unifyai-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.2/README.md` & `unifyai-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.2/pyproject.toml` & `unifyai-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "unifyai"
 packages = [{include = "unify"}]
-version = "0.8.2"
+version = "0.8.3"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `unifyai-0.8.2/unify/chat.py` & `unifyai-0.8.3/unify/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,37 +6,38 @@
 
 
 class ChatBot:  # noqa: WPS338
     """Agent class represents an LLM chat agent."""
 
     def __init__(
         self,
-        api_key: Optional[str] = None,
         endpoint: Optional[str] = None,
         model: Optional[str] = None,
         provider: Optional[str] = None,
+        api_key: Optional[str] = None,
     ) -> None:
         """
         Initializes the ChatBot object.
 
         Args:
-            api_key (str, optional): API key for accessing the Unify API.
-                If None, it attempts to retrieve the API key from the
-                environment variable UNIFY_KEY.
-                Defaults to None.
-
             endpoint (str, optional): Endpoint name in OpenAI API format:
                 <uploaded_by>/<model_name>@<provider_name>
                 Defaults to None.
 
             model (str, optional): Name of the model. If None,
             endpoint must be provided.
 
             provider (str, optional): Name of the provider. If None,
             endpoint must be provided.
+
+            api_key (str, optional): API key for accessing the Unify API.
+                If None, it attempts to retrieve the API key from the
+                environment variable UNIFY_KEY.
+                Defaults to None.
+
         Raises:
             UnifyError: If the API key is missing.
         """
         self._message_history: List[Dict[str, str]] = []
         self._paused = False
         self._client = Unify(
             api_key=api_key,
```

### Comparing `unifyai-0.8.2/unify/clients.py` & `unifyai-0.8.3/unify/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,36 +11,37 @@
 
 
 class Unify:
     """Class for interacting with the Unify API."""
 
     def __init__(
         self,
-        api_key: Optional[str] = None,
         endpoint: Optional[str] = None,
         model: Optional[str] = None,
         provider: Optional[str] = None,
+        api_key: Optional[str] = None,
     ) -> None:  # noqa: DAR101, DAR401
         """Initialize the Unify client.
 
         Args:
-            api_key (str, optional): API key for accessing the Unify API.
-                If None, it attempts to retrieve the API key from the
-                environment variable UNIFY_KEY.
-                Defaults to None.
-
             endpoint (str, optional): Endpoint name in OpenAI API format:
                 <uploaded_by>/<model_name>@<provider_name>
                 Defaults to None.
 
             model (str, optional): Name of the model. If None,
             endpoint must be provided.
 
             provider (str, optional): Name of the provider. If None,
             endpoint must be provided.
+
+            api_key (str, optional): API key for accessing the Unify API.
+                If None, it attempts to retrieve the API key from the
+                environment variable UNIFY_KEY.
+                Defaults to None.
+
         Raises:
             UnifyError: If the API key is missing.
         """
         self._api_key = _validate_api_key(api_key)
         self._endpoint, self._model, self._provider = _validate_endpoint(  # noqa:WPS414
             endpoint,
             model,
@@ -118,31 +119,31 @@
         self._endpoint = value
         self._model, self._provider = value.split("@")  # noqa: WPS414
         if self._provider in _available_dynamic_modes:
             self._provider = None
 
     def generate(  # noqa: WPS234, WPS211
         self,
-        messages: Optional[List[Dict[str, str]]] = None,
         user_prompt: Optional[str] = None,
         system_prompt: Optional[str] = None,
+        messages: Optional[List[Dict[str, str]]] = None,
         stream: bool = False,
     ) -> Union[Generator[str, None, None], str]:  # noqa: DAR101, DAR201, DAR401
         """Generate content using the Unify API.
 
         Args:
-            messages (List[Dict[str, str]]): A list of dictionaries containing the
-            conversation history. If provided, user_prompt must be None.
-
             user_prompt (Optional[str]): A string containing the user prompt.
             If provided, messages must be None.
 
             system_prompt (Optional[str]): An optional string containing the
             system prompt.
 
+            messages (List[Dict[str, str]]): A list of dictionaries containing the
+            conversation history. If provided, user_prompt must be None.
+
             stream (bool): If True, generates content as a stream.
             If False, generates content as a single response.
             Defaults to False.
 
         Returns:
             Union[Generator[str, None, None], str]: If stream is True,
              returns a generator yielding chunks of content.
@@ -234,37 +235,37 @@
 
 
 class AsyncUnify:
     """Class for interacting asynchronously with the Unify API."""
 
     def __init__(
         self,
-        api_key: Optional[str] = None,
         endpoint: Optional[str] = None,
         model: Optional[str] = None,
         provider: Optional[str] = None,
+        api_key: Optional[str] = None,
     ) -> None:  # noqa:DAR101, DAR401
         """Initialize the AsyncUnify client.
 
         Args:
-            api_key (str, optional): API key for accessing the Unify API.
-            If None, it attempts to retrieve the API key from
-            the environment variable UNIFY_KEY.
-            Defaults to None.
-
             endpoint (str, optional): Endpoint name in OpenAI API format:
             <uploaded_by>/<model_name>@<provider_name>
             Defaults to None.
 
             model (str, optional): Name of the model. If None,
             endpoint must be provided.
 
             provider (str, optional): Name of the provider. If None,
             endpoint must be provided.
 
+            api_key (str, optional): API key for accessing the Unify API.
+            If None, it attempts to retrieve the API key from
+            the environment variable UNIFY_KEY.
+            Defaults to None.
+
         Raises:
             UnifyError: If the API key is missing.
         """
         self._api_key = _validate_api_key(api_key)
         self._endpoint, self._model, self._provider = (  # noqa: WPS414
             _validate_endpoint(
                 endpoint,
@@ -371,31 +372,31 @@
         except requests.RequestException as e:
             raise BadRequestError("There was an error with the request.") from e
         except (KeyError, ValueError) as e:
             raise ValueError("Error parsing JSON response.") from e
 
     async def generate(  # noqa: WPS234, WPS211
         self,
-        messages: Optional[List[Dict[str, str]]] = None,
         user_prompt: Optional[str] = None,
         system_prompt: Optional[str] = None,
+        messages: Optional[List[Dict[str, str]]] = None,
         stream: bool = False,
     ) -> Union[AsyncGenerator[str, None], str]:  # noqa: DAR101, DAR201, DAR401
         """Generate content asynchronously using the Unify API.
 
         Args:
-            messages (List[Dict[str, str]]): A list of dictionaries containing the
-            conversation history. If provided, user_prompt must be None.
-
             user_prompt (Optional[str]): A string containing the user prompt.
             If provided, messages must be None.
 
             system_prompt (Optional[str]): An optional string containing the
             system prompt.
 
+            messages (List[Dict[str, str]]): A list of dictionaries containing the
+            conversation history. If provided, user_prompt must be None.
+
             stream (bool): If True, generates content as a stream.
             If False, generates content as a single response.
             Defaults to False.
 
         Returns:
             Union[AsyncGenerator[str, None], List[str]]: If stream is True,
             returns an asynchronous generator yielding chunks of content.
```

### Comparing `unifyai-0.8.2/unify/exceptions.py` & `unifyai-0.8.3/unify/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.2/unify/tests.py` & `unifyai-0.8.3/unify/tests.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.2/unify/utils.py` & `unifyai-0.8.3/unify/utils.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.2/PKG-INFO` & `unifyai-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

