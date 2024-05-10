# Comparing `tmp/anything_world-0.1.4.tar.gz` & `tmp/anything_world-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anything_world-0.1.4.tar", last modified: Fri Jan 26 12:34:23 2024, max compression
+gzip compressed data, was "anything_world-0.1.5.tar", last modified: Mon Mar 18 10:55:08 2024, max compression
```

## Comparing `anything_world-0.1.4.tar` & `anything_world-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.556725 anything_world-0.1.4/
--rw-r--r--   0 vilson     (501) staff       (20)     1071 2023-12-15 20:15:20.000000 anything_world-0.1.4/LICENSE
--rw-r--r--   0 vilson     (501) staff       (20)      241 2024-01-15 19:55:45.000000 anything_world-0.1.4/MANIFEST.in
--rw-r--r--   0 vilson     (501) staff       (20)     5409 2024-01-26 12:34:23.556355 anything_world-0.1.4/PKG-INFO
--rw-r--r--   0 vilson     (501) staff       (20)     4777 2024-01-26 12:32:00.000000 anything_world-0.1.4/README.md
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.551205 anything_world-0.1.4/anything_world/
--rw-r--r--   0 vilson     (501) staff       (20)        0 2024-01-18 15:29:04.000000 anything_world-0.1.4/anything_world/__init__.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.553420 anything_world-0.1.4/anything_world/async_api/
--rw-r--r--   0 vilson     (501) staff       (20)       32 2024-01-18 15:29:04.000000 anything_world-0.1.4/anything_world/async_api/__init__.py
--rw-r--r--   0 vilson     (501) staff       (20)    12001 2024-01-26 12:20:47.000000 anything_world-0.1.4/anything_world/async_api/api_client.py
--rw-r--r--   0 vilson     (501) staff       (20)     3163 2024-01-18 15:29:04.000000 anything_world-0.1.4/anything_world/async_api/utils.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.554325 anything_world-0.1.4/anything_world/sync_api/
--rw-r--r--   0 vilson     (501) staff       (20)       32 2024-01-18 15:29:04.000000 anything_world-0.1.4/anything_world/sync_api/__init__.py
--rw-r--r--   0 vilson     (501) staff       (20)    11825 2024-01-26 12:20:47.000000 anything_world-0.1.4/anything_world/sync_api/api_client.py
--rw-r--r--   0 vilson     (501) staff       (20)     2755 2024-01-18 15:29:04.000000 anything_world-0.1.4/anything_world/sync_api/utils.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.554637 anything_world-0.1.4/anything_world/utils/
--rw-r--r--   0 vilson     (501) staff       (20)     2872 2024-01-18 15:29:04.000000 anything_world-0.1.4/anything_world/utils/__init__.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.555992 anything_world-0.1.4/anything_world.egg-info/
--rw-r--r--   0 vilson     (501) staff       (20)     5409 2024-01-26 12:34:23.000000 anything_world-0.1.4/anything_world.egg-info/PKG-INFO
--rw-r--r--   0 vilson     (501) staff       (20)      634 2024-01-26 12:34:23.000000 anything_world-0.1.4/anything_world.egg-info/SOURCES.txt
--rw-r--r--   0 vilson     (501) staff       (20)        1 2024-01-26 12:34:23.000000 anything_world-0.1.4/anything_world.egg-info/dependency_links.txt
--rw-r--r--   0 vilson     (501) staff       (20)       46 2024-01-26 12:34:23.000000 anything_world-0.1.4/anything_world.egg-info/entry_points.txt
--rw-r--r--   0 vilson     (501) staff       (20)      119 2024-01-26 12:34:23.000000 anything_world-0.1.4/anything_world.egg-info/requires.txt
--rw-r--r--   0 vilson     (501) staff       (20)       23 2024-01-26 12:34:23.000000 anything_world-0.1.4/anything_world.egg-info/top_level.txt
--rw-r--r--   0 vilson     (501) staff       (20)      132 2024-01-12 14:53:25.000000 anything_world-0.1.4/env.example
--rw-r--r--   0 vilson     (501) staff       (20)      829 2024-01-26 12:33:23.000000 anything_world-0.1.4/pyproject.toml
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.554855 anything_world-0.1.4/scripts/
--rw-r--r--   0 vilson     (501) staff       (20)       95 2024-01-26 12:20:47.000000 anything_world-0.1.4/scripts/cli.py
--rw-r--r--   0 vilson     (501) staff       (20)       38 2024-01-26 12:34:23.556786 anything_world-0.1.4/setup.cfg
--rw-r--r--   0 vilson     (501) staff       (20)       91 2024-01-12 14:53:25.000000 anything_world-0.1.4/setup.py
-drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-01-26 12:34:23.555509 anything_world-0.1.4/tests/
--rw-r--r--   0 vilson     (501) staff       (20)     2110 2024-01-22 18:22:58.000000 anything_world-0.1.4/tests/test_async_api.py
--rw-r--r--   0 vilson     (501) staff       (20)     2006 2024-01-22 18:22:58.000000 anything_world-0.1.4/tests/test_sync_api.py
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.997630 anything_world-0.1.5/
+-rw-r--r--   0 vilson     (501) staff       (20)     1071 2023-12-15 20:15:20.000000 anything_world-0.1.5/LICENSE
+-rw-r--r--   0 vilson     (501) staff       (20)      241 2024-01-15 19:55:45.000000 anything_world-0.1.5/MANIFEST.in
+-rw-r--r--   0 vilson     (501) staff       (20)     4500 2024-03-18 10:55:08.997323 anything_world-0.1.5/PKG-INFO
+-rw-r--r--   0 vilson     (501) staff       (20)     3868 2024-03-18 10:45:06.000000 anything_world-0.1.5/README.md
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.991317 anything_world-0.1.5/anything_world/
+-rw-r--r--   0 vilson     (501) staff       (20)        0 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/__init__.py
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.993810 anything_world-0.1.5/anything_world/async_api/
+-rw-r--r--   0 vilson     (501) staff       (20)       32 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/async_api/__init__.py
+-rw-r--r--   0 vilson     (501) staff       (20)    12407 2024-03-18 10:41:48.000000 anything_world-0.1.5/anything_world/async_api/api_client.py
+-rw-r--r--   0 vilson     (501) staff       (20)     3163 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/async_api/utils.py
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.995184 anything_world-0.1.5/anything_world/sync_api/
+-rw-r--r--   0 vilson     (501) staff       (20)       32 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/sync_api/__init__.py
+-rw-r--r--   0 vilson     (501) staff       (20)    12250 2024-03-18 10:38:29.000000 anything_world-0.1.5/anything_world/sync_api/api_client.py
+-rw-r--r--   0 vilson     (501) staff       (20)     2755 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/sync_api/utils.py
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.995511 anything_world-0.1.5/anything_world/utils/
+-rw-r--r--   0 vilson     (501) staff       (20)     2872 2024-01-18 15:29:04.000000 anything_world-0.1.5/anything_world/utils/__init__.py
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.996955 anything_world-0.1.5/anything_world.egg-info/
+-rw-r--r--   0 vilson     (501) staff       (20)     4500 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/PKG-INFO
+-rw-r--r--   0 vilson     (501) staff       (20)      634 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/SOURCES.txt
+-rw-r--r--   0 vilson     (501) staff       (20)        1 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/dependency_links.txt
+-rw-r--r--   0 vilson     (501) staff       (20)       46 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/entry_points.txt
+-rw-r--r--   0 vilson     (501) staff       (20)      119 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/requires.txt
+-rw-r--r--   0 vilson     (501) staff       (20)       23 2024-03-18 10:55:08.000000 anything_world-0.1.5/anything_world.egg-info/top_level.txt
+-rw-r--r--   0 vilson     (501) staff       (20)      132 2024-01-12 14:53:25.000000 anything_world-0.1.5/env.example
+-rw-r--r--   0 vilson     (501) staff       (20)      829 2024-03-18 10:50:07.000000 anything_world-0.1.5/pyproject.toml
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.995712 anything_world-0.1.5/scripts/
+-rw-r--r--   0 vilson     (501) staff       (20)       95 2024-01-26 12:20:47.000000 anything_world-0.1.5/scripts/cli.py
+-rw-r--r--   0 vilson     (501) staff       (20)       38 2024-03-18 10:55:08.997680 anything_world-0.1.5/setup.cfg
+-rw-r--r--   0 vilson     (501) staff       (20)       91 2024-01-12 14:53:25.000000 anything_world-0.1.5/setup.py
+drwxr-xr-x   0 vilson     (501) staff       (20)        0 2024-03-18 10:55:08.996568 anything_world-0.1.5/tests/
+-rw-r--r--   0 vilson     (501) staff       (20)     2110 2024-01-22 18:22:58.000000 anything_world-0.1.5/tests/test_async_api.py
+-rw-r--r--   0 vilson     (501) staff       (20)     2006 2024-01-22 18:22:58.000000 anything_world-0.1.5/tests/test_sync_api.py
```

### Comparing `anything_world-0.1.4/LICENSE` & `anything_world-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.4/PKG-INFO` & `anything_world-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anything_world
-Version: 0.1.4
+Version: 0.1.5
 Summary: Anything World API wrapper library and CLI
 Author-email: Anything World <support@anything.world>
 License: MIT
 Project-URL: Homepage, https://anything.world
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -70,66 +70,41 @@
 # Create a client to be able to query Anything World's API
 client = AWClient()
 
 # Search for 3D models of `cats`:
 response = client.find('cats')
 
 # Upload files from ./examples/cat folder to be animated
-response = client.animate('./examples/cat', 'some_cat', 'cat', is_symmetric=True)
+response = client.animate(
+    files_dir='./examples/cat',
+    model_name='some_cat',
+    model_type='cat',
+    is_symmetric=True
+)
 
 # Response has the model_id of the 3D model that our AI pipeline is currently animating
 model_id = response["model_id"]
 
-# Runs a long-polling loop, starting it only after 2 minutes and after that,
+# Runs a long-polling loop, starting it only after 10 seconds and after that,
 # checking every 5 secs if the API is done animating the model
-model_data = client.get_animated_model(model_id, waiting_time=5, warmup_time=120)
+model_data = client.get_animated_model(
+    model_id=model_id,
+    waiting_time=5,
+    warmup_time=10,
+    verbose=True
+)
 
 # Check if our AI pipeline is done animating the model
 is_finished = client.is_animation_done(model_id)
 assert is_finished == True
 
 # Gets all model data
 model_data = client.get_model(model_id)
 ```
 
-## Async
-
-```python
-import asyncio
-from anything_world.async_api import AWClient
-
-# Create a client to be able to query Anything World's API
-client = AWClient()
-
-# Search for 3D models of `cats`:
-response = asyncio.run(
-    client.find('cats'))
-
-# Upload files from ./examples/cat folder to be animated
-response = asyncio.run(
-    client.animate('./examples/cat', 'some_cat', 'cat', is_symmetric=True))
-
-# Response has the model_id of the 3D model that our AI pipeline is currently animating
-model_id = response["model_id"]
-
-# Runs a long-polling loop, starting it only after 2 minutes and after that,
-# checking every 5 secs if the API is done animating the model.
-model_data = asyncio.run(
-    client.get_animated_model(model_id, waiting_time=5, warmup_time=120))
-
-# Check if our AI pipeline is done animating the model
-is_finished = asyncio.run(
-    client.is_animation_done(model_id))
-assert is_finished == True
-
-# Gets all model data
-model_data = async.run(
-    client.get_model(model_id))
-```
-
 ## From CLI
 
 All `AWClient` methods are exposed as commands of the `anything` CLI tool.
 Just call the `anything` tool and it will display a manual page of the
 available commands:
 
 ```bash
```

### Comparing `anything_world-0.1.4/README.md` & `anything_world-0.1.5/anything_world.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: anything_world
+Version: 0.1.5
+Summary: Anything World API wrapper library and CLI
+Author-email: Anything World <support@anything.world>
+License: MIT
+Project-URL: Homepage, https://anything.world
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: python-dotenv==1.0.0
+Requires-Dist: requests==2.28.2
+Requires-Dist: pytest==7.2.2
+Requires-Dist: pytest-asyncio==0.21.0
+Requires-Dist: aiohttp==3.8.4
+Requires-Dist: aiofiles==23.2.1
+Requires-Dist: fire==0.5.0
+
 # Anything World Python Client
 
 Python library and CLI for Anything World API.
 
 To use this package you'll need to obtain a valid Anything World API key.
 Please, create an account in
 [our website](https://app.anything.world/register) and then visit
@@ -50,66 +70,41 @@
 # Create a client to be able to query Anything World's API
 client = AWClient()
 
 # Search for 3D models of `cats`:
 response = client.find('cats')
 
 # Upload files from ./examples/cat folder to be animated
-response = client.animate('./examples/cat', 'some_cat', 'cat', is_symmetric=True)
+response = client.animate(
+    files_dir='./examples/cat',
+    model_name='some_cat',
+    model_type='cat',
+    is_symmetric=True
+)
 
 # Response has the model_id of the 3D model that our AI pipeline is currently animating
 model_id = response["model_id"]
 
-# Runs a long-polling loop, starting it only after 2 minutes and after that,
+# Runs a long-polling loop, starting it only after 10 seconds and after that,
 # checking every 5 secs if the API is done animating the model
-model_data = client.get_animated_model(model_id, waiting_time=5, warmup_time=120)
+model_data = client.get_animated_model(
+    model_id=model_id,
+    waiting_time=5,
+    warmup_time=10,
+    verbose=True
+)
 
 # Check if our AI pipeline is done animating the model
 is_finished = client.is_animation_done(model_id)
 assert is_finished == True
 
 # Gets all model data
 model_data = client.get_model(model_id)
 ```
 
-## Async
-
-```python
-import asyncio
-from anything_world.async_api import AWClient
-
-# Create a client to be able to query Anything World's API
-client = AWClient()
-
-# Search for 3D models of `cats`:
-response = asyncio.run(
-    client.find('cats'))
-
-# Upload files from ./examples/cat folder to be animated
-response = asyncio.run(
-    client.animate('./examples/cat', 'some_cat', 'cat', is_symmetric=True))
-
-# Response has the model_id of the 3D model that our AI pipeline is currently animating
-model_id = response["model_id"]
-
-# Runs a long-polling loop, starting it only after 2 minutes and after that,
-# checking every 5 secs if the API is done animating the model.
-model_data = asyncio.run(
-    client.get_animated_model(model_id, waiting_time=5, warmup_time=120))
-
-# Check if our AI pipeline is done animating the model
-is_finished = asyncio.run(
-    client.is_animation_done(model_id))
-assert is_finished == True
-
-# Gets all model data
-model_data = async.run(
-    client.get_model(model_id))
-```
-
 ## From CLI
 
 All `AWClient` methods are exposed as commands of the `anything` CLI tool.
 Just call the `anything` tool and it will display a manual page of the
 available commands:
 
 ```bash
```

### Comparing `anything_world-0.1.4/anything_world/async_api/api_client.py` & `anything_world-0.1.5/anything_world/async_api/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
 
     async def get_animated_model(
             self,
             model_id: str,
             extra_formats: bool = False,
             waiting_time: Optional[int] = 5,
+            warmup_time: Optional[int] = 0,
             verbose: Optional[bool] = False) -> dict:
         """
         Asynchronously retrieves an animated model by polling.
 
         This function sends a GET request to the API to retrieve the animated model. It polls the API until the model
         reaches the finished stage expected for the /animate endpoint, waiting a specified amount of time
         between each request.
@@ -129,23 +130,27 @@
         formats are generated as well (`.gltf`, `.dae`), set the
         `extra_formats` param to `True`.   
 
         :param model_id: str, the ID of the model to retrieve.
         :param extra_formats: bool, optional, a flag indicating if the model
             should have extra formats in the response or not. Defaults to False.
         :param waiting_time: int, optional, the amount of time to wait between each request in seconds. Defaults to 5.
+        :param warmup_time: int, optional, the amount of time to wait before sending the first request in seconds.
+            This is useful specially for users with low connectivity, to avoid unnecessary requests, given that for
+            some models the API takes a while to the model ready. Defaults to 0.  
         :param verbose: bool, optional, a flag indicating whether to print detailed information about each request.
             Defaults to False.
         :return: dict, the JSON response from the API decoded as a dict.
         """
         expected_formats = "extra_formats" if extra_formats else "default"
         return await self._get_model_by_polling(
             model_id,
             expected_stages=self._finished_stages["animate"][expected_formats],
             waiting_time=waiting_time,
+            warmup_time=warmup_time,
             verbose=verbose)
 
 
     async def is_animation_done(self, model_id: str, extra_formats: bool=False) -> bool:
         """
         Checks if the animation of a model is done.
 
@@ -268,15 +273,15 @@
                 model_stage = model_json["stage"]
                 if model_stage in expected_stages:
                     if verbose:
                         print(f"{status_prefix} Done.")
                     return model_json
             else:
                 if verbose:
-                    print(f"{status_prefix} Model is not ready yet...")
+                    print(f"{status_prefix} Model {model_id} is not ready yet...")
             await asyncio.sleep(waiting_time)
 
 
     async def _is_model_done(
             self,
             model_id: str,
             endpoint: str,
```

### Comparing `anything_world-0.1.4/anything_world/async_api/utils.py` & `anything_world-0.1.5/anything_world/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.4/anything_world/sync_api/api_client.py` & `anything_world-0.1.5/anything_world/sync_api/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
    """
 
     # Stage names that identify the end of a process for a given endpoint name
     _finished_stages = {
         "animate": {
             # In these stages, basic formats are already generated
             "default": [
-                "format_conversion",
-                "thumbnails_generation",
+                "thumbnails_generation_finished",
+                "formats_conversion_finished",
                 "migrate_animation_finished"
             ],
             # In these stages, extra formats are already generated
             "extra_formats": [
                 "formats_conversion_finished"
             ]
         }
@@ -114,14 +114,15 @@
 
 
     def get_animated_model(
             self,
             model_id: str,
             extra_formats: bool = False,
             waiting_time: Optional[int] = 5,
+            warmup_time: Optional[int] = 0,
             verbose: Optional[bool] = False) -> dict:
         """
         Retrieves an animated model by polling.
 
         This function sends a GET request to the API to retrieve the animated model. It polls the API until the model
         reaches the finished stage expected for the /animate endpoint, waiting a specified amount of time
         between each request.
@@ -131,23 +132,27 @@
         formats are generated as well (`.gltf`, `.dae`), set the
         `extra_formats` param to `True`.   
 
         :param model_id: str, the ID of the model to retrieve.
         :param extra_formats: bool, optional, a flag indicating if the model
             should have extra formats in the response or not. Defaults to False.
         :param waiting_time: int, optional, the amount of time to wait between each request in seconds. Defaults to 5.
+        :param warmup_time: int, optional, the amount of time to wait before sending the first request in seconds.
+            This is useful specially for users with low connectivity, to avoid unnecessary requests, given that for
+            some models the API takes a while to the model ready. Defaults to 0.  
         :param verbose: bool, optional, a flag indicating whether to print detailed information about each request.
             Defaults to False.
         :return: dict, the JSON response from the API decoded as a dict.
         """    
         expected_formats = "extra_formats" if extra_formats else "default"
         return self._get_model_by_polling(
             model_id,
             expected_stages=self._finished_stages["animate"][expected_formats],
             waiting_time=waiting_time,
+            warmup_time=warmup_time,
             verbose=verbose)
 
 
     def is_animation_done(self, model_id: str, extra_formats: bool=False) -> bool:
         """
         Checks if the animation of a model is done.
 
@@ -270,15 +275,15 @@
                 model_stage = model_json["stage"]
                 if model_stage in expected_stages:
                     if verbose:
                         print(f"{status_prefix} Done.")
                     return model_json
             else:
                 if verbose:
-                    print(f"{status_prefix} Model is not ready yet...")
+                    print(f"{status_prefix} Model {model_id} is not ready yet...")
             time.sleep(waiting_time)
 
 
     def _is_model_done(
             self,
             model_id: str,
             endpoint: str,
```

### Comparing `anything_world-0.1.4/anything_world/sync_api/utils.py` & `anything_world-0.1.5/anything_world/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.4/anything_world/utils/__init__.py` & `anything_world-0.1.5/anything_world/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.4/anything_world.egg-info/PKG-INFO` & `anything_world-0.1.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: anything_world
-Version: 0.1.4
-Summary: Anything World API wrapper library and CLI
-Author-email: Anything World <support@anything.world>
-License: MIT
-Project-URL: Homepage, https://anything.world
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: requests==2.28.2
-Requires-Dist: pytest==7.2.2
-Requires-Dist: pytest-asyncio==0.21.0
-Requires-Dist: aiohttp==3.8.4
-Requires-Dist: aiofiles==23.2.1
-Requires-Dist: fire==0.5.0
-
 # Anything World Python Client
 
 Python library and CLI for Anything World API.
 
 To use this package you'll need to obtain a valid Anything World API key.
 Please, create an account in
 [our website](https://app.anything.world/register) and then visit
@@ -70,66 +50,41 @@
 # Create a client to be able to query Anything World's API
 client = AWClient()
 
 # Search for 3D models of `cats`:
 response = client.find('cats')
 
 # Upload files from ./examples/cat folder to be animated
-response = client.animate('./examples/cat', 'some_cat', 'cat', is_symmetric=True)
+response = client.animate(
+    files_dir='./examples/cat',
+    model_name='some_cat',
+    model_type='cat',
+    is_symmetric=True
+)
 
 # Response has the model_id of the 3D model that our AI pipeline is currently animating
 model_id = response["model_id"]
 
-# Runs a long-polling loop, starting it only after 2 minutes and after that,
+# Runs a long-polling loop, starting it only after 10 seconds and after that,
 # checking every 5 secs if the API is done animating the model
-model_data = client.get_animated_model(model_id, waiting_time=5, warmup_time=120)
+model_data = client.get_animated_model(
+    model_id=model_id,
+    waiting_time=5,
+    warmup_time=10,
+    verbose=True
+)
 
 # Check if our AI pipeline is done animating the model
 is_finished = client.is_animation_done(model_id)
 assert is_finished == True
 
 # Gets all model data
 model_data = client.get_model(model_id)
 ```
 
-## Async
-
-```python
-import asyncio
-from anything_world.async_api import AWClient
-
-# Create a client to be able to query Anything World's API
-client = AWClient()
-
-# Search for 3D models of `cats`:
-response = asyncio.run(
-    client.find('cats'))
-
-# Upload files from ./examples/cat folder to be animated
-response = asyncio.run(
-    client.animate('./examples/cat', 'some_cat', 'cat', is_symmetric=True))
-
-# Response has the model_id of the 3D model that our AI pipeline is currently animating
-model_id = response["model_id"]
-
-# Runs a long-polling loop, starting it only after 2 minutes and after that,
-# checking every 5 secs if the API is done animating the model.
-model_data = asyncio.run(
-    client.get_animated_model(model_id, waiting_time=5, warmup_time=120))
-
-# Check if our AI pipeline is done animating the model
-is_finished = asyncio.run(
-    client.is_animation_done(model_id))
-assert is_finished == True
-
-# Gets all model data
-model_data = async.run(
-    client.get_model(model_id))
-```
-
 ## From CLI
 
 All `AWClient` methods are exposed as commands of the `anything` CLI tool.
 Just call the `anything` tool and it will display a manual page of the
 available commands:
 
 ```bash
```

### Comparing `anything_world-0.1.4/anything_world.egg-info/SOURCES.txt` & `anything_world-0.1.5/anything_world.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.4/pyproject.toml` & `anything_world-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anything_world"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     {name = "Anything World", email = "support@anything.world"},
 ]
 description = "Anything World API wrapper library and CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
```

### Comparing `anything_world-0.1.4/tests/test_async_api.py` & `anything_world-0.1.5/tests/test_async_api.py`

 * *Files identical despite different names*

### Comparing `anything_world-0.1.4/tests/test_sync_api.py` & `anything_world-0.1.5/tests/test_sync_api.py`

 * *Files identical despite different names*

