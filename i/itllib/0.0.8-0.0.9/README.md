# Comparing `tmp/itllib-0.0.8.tar.gz` & `tmp/itllib-0.0.9.tar.gz`

## Comparing `itllib-0.0.8.tar` & `itllib-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 itllib-0.0.8/.git
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/__init__.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/__main__.py
--rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/clusters.py
--rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/controllers.py
--rw-r--r--   0        0        0    21545 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/itl.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/loops.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/piles.py
--rw-r--r--   0        0        0    49773 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/resources.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 itllib-0.0.8/src/itllib/secrets.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 itllib-0.0.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itllib-0.0.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itllib-0.0.8/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 itllib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 itllib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 itllib-0.0.9/.git
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/__init__.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/__main__.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/clusters.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/controllers.py
+-rw-r--r--   0        0        0    24649 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/itl.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/loops.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/piles.py
+-rw-r--r--   0        0        0    53650 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/resources.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 itllib-0.0.9/src/itllib/secrets.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 itllib-0.0.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itllib-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itllib-0.0.9/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 itllib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 itllib-0.0.9/PKG-INFO
```

### Comparing `itllib-0.0.8/src/itllib/__main__.py` & `itllib-0.0.9/src/itllib/__main__.py`

 * *Files identical despite different names*

### Comparing `itllib-0.0.8/src/itllib/clusters.py` & `itllib-0.0.9/src/itllib/clusters.py`

 * *Files identical despite different names*

### Comparing `itllib-0.0.8/src/itllib/itl.py` & `itllib-0.0.9/src/itllib/itl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import atexit
 import asyncio
 from collections import defaultdict
+from contextvars import Context
 import inspect
+import os
 import threading
+import time
 import typing
 from glob import glob
 import traceback
 from urllib.parse import urlparse
 
 import websockets
 import json
@@ -55,50 +59,55 @@
 
     return argument_type_hints
 
 
 class Itl:
     def __init__(self, *configs, client=None) -> None:
         # User-specified handlers
-        self._data_handlers = {}
+        self._data_handlers = defaultdict(lambda: defaultdict(list))
         self._controllers = {}
 
         # Async stuff
         self._connection_thread = None
         self._connection_looper = None
         self._connection_tasks = asyncio.Queue()
         self._callback_thread = None
+        self._callback_context = None
         self._callback_looper = None
         self._callback_tasks = asyncio.Queue()
+        self._disconnect_tasks = []
 
-        # Old stuff, to be removed
-        self._stop = False
+        self._ready_looper = None
+        self._finished_looper = None
+        self.ready_queue = asyncio.Queue()
+        self.finished_queue = asyncio.Queue()
+
+        self._started = False
+        self._stopped = False
 
         # Resources
         self._secrets = {}
         self._streams: dict[str, StreamOperations] = {}
         self._buckets = {}
         self._piles = {}
         self._clusters: dict[str, ClusterOperations] = {}
         self._loops: dict[str, LoopOperations] = {}
 
         # Stream interactions
-        self._downstreams = {}
-        self._upstreams = {}
         self._start_persistent_tasks = {}
         self._downstream_queues = defaultdict(asyncio.Queue)
         self._started_streams = set()
         self._start_ephemeral_tasks = []
-        self._post_connection_tasks = []
 
         self._resource_pile = ResourcePile()
         self._resolver = ResourceResolver(self._resource_pile)
         self._keys = defaultdict(lambda: None)
 
         self._apply_config(*configs, client=client)
+        atexit.register(self.stop)
 
     def _apply_config(self, *files, client=None):
         self._resource_pile.add(*files)
         self._resolver = ResourceResolver(self._resource_pile)
 
         # Get apikeys for the client
         if client != None:
@@ -251,28 +260,28 @@
         if identifier in self._start_persistent_tasks:
             return
 
         task = self._attach_stream, (identifier,)
         self._start_persistent_tasks[identifier] = task
         asyncio.create_task(self._attach_stream(identifier))
 
-    def ondata(self, stream=None, loop=None, streamId=None):
+    def ondata(self, stream=None, loop=None, streamId=None, key=None):
         if stream == None:
             loop_info = self._loops[loop]
-            stream = f'stream/{loop}/{streamId}'
+            stream = f"stream/{loop}/{streamId}"
             if stream not in self._streams:
                 self._streams[stream] = StreamOperations(
                     loop_info.connect_info.stream_connection_info(streamId),
                     loop_info.apikey,
                 )
-        if stream not in self._upstreams:
-            self._ensure_stream_connection([stream])
+
+        self._ensure_stream_connection([stream])
 
         def decorator(func):
-            self._data_handlers.setdefault(stream, []).append(func)
+            self._data_handlers[stream][key].append(func)
             return func
 
         return decorator
 
     def controller(
         self,
         cluster,
@@ -291,21 +300,26 @@
                     cluster,
                     event["group"],
                     event["version"],
                     event["kind"],
                     event["name"],
                     validate=validate,
                 )
-                async with operations:
-                    try:
-                        await func(operations)
-                    except Exception as e:
-                        print(
-                            f"Error in controller {func.__name__}: {traceback.format_exc()}"
-                        )
+                try:
+                    async with operations:
+                        try:
+                            await func(operations)
+                        except Exception as e:
+                            print(
+                                f"Error in controller {func.__name__}: {traceback.format_exc()}"
+                            )
+                except Exception as e:
+                    print(
+                        f"Error in controller {func.__name__}: {traceback.format_exc()}"
+                    )
 
             @self.ondata(stream)
             async def event_handler(*args, **event):
                 if event["event"] != "queue":
                     return
                 if group and event["group"] != group:
                     return
@@ -335,41 +349,57 @@
                 self._callback_tasks.put_nowait, (func, ())
             )
         else:
             self._start_ephemeral_tasks.append((func, ()))
 
         return func
 
+    def ondisconnect(self, func):
+        if self._stopped:
+            raise RuntimeError(
+                "Cannot add ondisconnect handler after itl has been stopped"
+            )
+        else:
+            self._disconnect_tasks.append(func)
+
+        return func
+
     async def _process_upstream_messages(self):
         def exec_callback(handler, args, kwargs):
             try:
                 if inspect.iscoroutinefunction(handler):
                     asyncio.create_task(handler(*args, **kwargs))
                 else:
                     handler(*args, **kwargs)
             except Exception as e:
                 print(f"Error in handler {handler.__name__}: {traceback.format_exc()}")
 
         def process_message(identifier, serialized_data):
             message = json.loads(serialized_data)
             # TODO: Run all handlers in parallel
-            for handler in self._data_handlers[identifier]:
-                if isinstance(message, dict):
-                    args = []
-                    kwargs = message
-                else:
-                    args = [message]
-                    kwargs = {}
+            for collection in self._data_handlers[identifier].values():
+                for handler in collection:
+                    if isinstance(message, dict):
+                        args = []
+                        kwargs = message
+                    else:
+                        args = [message]
+                        kwargs = {}
 
-                exec_callback(handler, args, kwargs)
+                    exec_callback(handler, args, kwargs)
+
+        for fn, args in self._start_ephemeral_tasks:
+            asyncio.create_task(fn(*args))
+
+        self._ready_looper.call_soon_threadsafe(self.ready_queue.put_nowait, None)
 
         while True:
             task = await self._callback_tasks.get()
 
-            if self._stop:
+            if self._stopped:
                 break
 
             if task == None:
                 continue
 
             identifier, serialized_data = task
 
@@ -379,63 +409,58 @@
                 else:
                     exec_callback(identifier, serialized_data, {})
             except asyncio.CancelledError:
                 pass
             except Exception as e:
                 print(f"Error in message processing: {traceback.format_exc()}")
 
+        for fn in self._disconnect_tasks:
+            fn()
+
+        self._finished_looper.call_soon_threadsafe(self.finished_queue.put_nowait, None)
+
     async def _post_stream_message(self, url, message):
         # call HTTP POST on key, passing message as data
         async with aiohttp.ClientSession() as session:
             async with session.post(url, data=json.dumps(message)) as response:
                 response.raise_for_status()
 
-    def stream_send(self, key=None, message=None, loop=None, streamId=None):
-        if key == None:
+    def stream_send(self, stream=None, message=None, loop=None, streamId=None):
+        if stream == None:
             loop_info = self._loops[loop]
-            key = f'stream/{loop}/{streamId}'
-            if key not in self._streams:
-                self._streams[key] = StreamOperations(
+            stream = f"stream/{loop}/{streamId}"
+            if stream not in self._streams:
+                self._streams[stream] = StreamOperations(
                     loop_info.connect_info.stream_connection_info(streamId),
                     loop_info.apikey,
                 )
 
-        if key not in self._streams and (
-            key.startswith("http://") or key.startswith("https://")
-        ):
-            asyncio.run_coroutine_threadsafe(
-                self._post_stream_message(key, message), self._connection_looper
-            )
-            return
-
-        self._ensure_stream_connection([key])
+        self._ensure_stream_connection([stream])
 
         if self._connection_looper:
             self._connection_looper.call_soon_threadsafe(
-                self._downstream_queues[key].put_nowait, message
+                self._downstream_queues[stream].put_nowait, message
             )
         else:
-            task = self._downstream_queues[key].put, (message,)
+            task = self._downstream_queues[stream].put, (message,)
             self._connection_looper.call_soon_threadsafe(
-                self._downstream_queues[key].put_nowait, task
+                self._downstream_queues[stream].put_nowait, task
             )
 
-    def stream_send_sync(self, key, message):
-        if key.startswith("http://") or key.startswith("https://"):
-            # call HTTP POST on key, passing message as data
-            requests.post(url=key, json=json.dumps(message))
-            return
+    def stream_send_sync(self, stream, message):
+        if self._started and self._stopped:
+            raise RuntimeError("Cannot send messages after itl has been stopped")
 
-        self._ensure_stream_connection([key])
+        self._ensure_stream_connection([stream])
 
         if self._connection_looper:
-            self._downstream_queues[key].put_nowait(message)
+            self._downstream_queues[stream].put_nowait(message)
         else:
-            task = self._downstream_queues[key].put, (message,)
-            self._downstream_queues[key].put_nowait(task)
+            task = self._downstream_queues[stream].put, (message,)
+            self._downstream_queues[stream].put_nowait(task)
 
     def _requeue(self, identifier, message):
         if message == None:
             return
 
         old_queue = self._downstream_queues[identifier]
         new_queue = asyncio.Queue()
@@ -460,15 +485,15 @@
         apikey = self._streams[identifier].apikey
 
         async def send_message():
             state.message = (
                 state.message or await self._downstream_queues[identifier].get()
             )
 
-            if self._stop:
+            if self._stopped:
                 self._requeue(identifier, state.message)
                 return False
 
             serialized_data = json.dumps(state.message)
 
             try:
                 await self._streams[identifier].send(serialized_data)
@@ -497,35 +522,35 @@
             )
 
             return True
 
         backoff_time = 0
         tasks = None
 
-        while not self._stop:
+        while not self._stopped:
             try:
                 if not tasks:
                     tasks = [
                         asyncio.create_task(asyncio.sleep(0)),
                         asyncio.create_task(asyncio.sleep(0)),
                     ]
 
                 ws_url = self._get_url(identifier)
                 if apikey:
-                     ws_url = ws_url + "/apikey/" + apikey
+                    ws_url = ws_url + "/apikey/" + apikey
 
                 async with websockets.connect(ws_url) as websocket:
                     backoff_time = 0
                     self._streams[identifier].socket = websocket
 
                     while True:
                         done, pending = await asyncio.wait(
                             tasks, return_when=asyncio.FIRST_COMPLETED
                         )
-                        if self._stop:
+                        if self._stopped:
                             return
 
                         connection_closed = False
 
                         for completed in done:
                             if completed.result() == False:
                                 connection_closed = True
@@ -539,95 +564,149 @@
                             break
 
             except websockets.exceptions.ConnectionClosedOK:
                 pass
             except websockets.exceptions.ConnectionClosedError:
                 pass
 
-            if self._stop:
+            if self._stopped:
                 return
 
             # Backoff before reconnecting
             backoff_time = await self._exponential_backoff(backoff_time)
 
     async def _exponential_backoff(self, current_backoff_time):
         """Sleeps the process for an exponential backoff time."""
         await asyncio.sleep(2**current_backoff_time)
         # Return the next backoff time, capped at 2**7 seconds
         return min(current_backoff_time + 1, 7)
 
-    async def _connect(self):
-        connection_tasks = []
-        for fn, args in self._start_persistent_tasks.values():
-            asyncio.create_task(fn(*args))
-        for fn, args in self._start_ephemeral_tasks:
-            connection_tasks.append(fn(*args))
-
-        await asyncio.gather(*connection_tasks)
-
-        post_connection_tasks = []
-        for fn, args in self._post_connection_tasks:
-            post_connection_tasks.append(fn(*args))
-
-        await asyncio.gather(*post_connection_tasks)
-
-        # if self._post_connect:
-        #     await self._post_connect()
+    def start(self, daemon=True):
+        if self._started:
+            if self._stopped:
+                raise RuntimeError("Cannot start the same itl twice")
+            return
+        self._started = True
+        self._ready_looper = asyncio.new_event_loop()
+        self._ready_looper.set_debug(True)
+        self._ready_looper.set_exception_handler(self.default_exception_handler)
+
+        self._finished_looper = asyncio.new_event_loop()
+        self._finished_looper.set_debug(True)
+        self._finished_looper.set_exception_handler(self.default_exception_handler)
 
-    def start(self):
         self._connection_thread = threading.Thread(
-            target=self._handle_connections_in_thread
+            target=self._handle_connections_in_thread, daemon=daemon
         )
         self._connection_thread.start()
 
         self._callback_thread = threading.Thread(
-            target=self._handle_callbacks_in_thread
+            target=self._handle_callbacks_in_thread, daemon=daemon
         )
         self._callback_thread.start()
 
+        self._ready_looper.run_until_complete(self.ready_queue.get())
+        self._ready_looper.run_until_complete(self.ready_queue.get())
+
     def _handle_connections_in_thread(self):
         self._connection_looper = looper = asyncio.new_event_loop()
         asyncio.set_event_loop(looper)
         looper.set_debug(True)
+        looper.set_exception_handler(self.default_exception_handler)
         looper.run_until_complete(self._start_routine())
-        looper.close()
 
     def _handle_callbacks_in_thread(self):
         self._callback_looper = looper = asyncio.new_event_loop()
+        self._callback_context = Context()
         asyncio.set_event_loop(looper)
         looper.set_debug(True)
+        looper.set_exception_handler(self.default_exception_handler)
         looper.run_until_complete(self._process_upstream_messages())
-        looper.close()
 
     def stop(self):
-        self._stop = True
+        if not self._started:
+            print("Warning: itl was never started")
+            return
+        if self._stopped:
+            return
+        self._stopped = True
+
+        if self._callback_looper == None or self._connection_looper == None:
+            print("Warning: itl did not finish starting")
+            return
+
         self._callback_looper.call_soon_threadsafe(
             self._callback_tasks.put_nowait, None
         )
+        self._callback_thread.join()
+
         self._connection_looper.call_soon_threadsafe(
             self._connection_tasks.put_nowait, None
         )
+        self._connection_thread.join()
+
+    def wait(self):
+        try:
+            self._finished_looper.run_until_complete(self.async_wait())
+            self._finished_looper.close()
+        except:
+            self.stop()
+
+    async def async_wait(self):
+        try:
+            await self.finished_queue.get()
+            await self.finished_queue.get()
+        except:
+            pass
 
     async def _start_routine(self):
         self._looper = asyncio.get_event_loop()
-        tasks = []
 
-        await self._connect()
-        await asyncio.gather(*tasks)
+        for fn, args in self._start_persistent_tasks.values():
+            asyncio.create_task(fn(*args))
+
+        self._ready_looper.call_soon_threadsafe(self.ready_queue.put_nowait, None)
 
         while True:
             task = await self._connection_tasks.get()
-            if self._stop:
+            if self._stopped:
                 break
             task()
 
         for queue in self._downstream_queues.values():
             queue.put_nowait(None)
 
         close_tasks = []
-        for stream in self._downstreams.values():
-            close_tasks.append(stream.close())
+        for stream in self._streams.values():
+            if stream.socket:
+                close_tasks.append(stream.socket.close())
+
+        await asyncio.gather(*close_tasks)
+        self._finished_looper.call_soon_threadsafe(self.finished_queue.put_nowait, None)
+
+    def default_exception_handler(self, loop, context):
+        # context["message"] will contain the error message
+        # context["exception"] will contain the actual exception object
+        if "exception" not in context:
+            return
 
-        for stream in self._upstreams.values():
-            close_tasks.append(stream.close())
+        exception = context["exception"]
 
-        asyncio.gather(*close_tasks)
+        # Python uses a Runtime error to signal that the event loop is closed, so
+        # unfortunately there's not a great way to check for it. This is an ugly
+        # workaround.
+        if isinstance(exception, RuntimeError):
+            if (
+                str(exception)
+                == "cannot schedule new futures after interpreter shutdown"
+            ):
+                error_dir = os.path.dirname(
+                    exception.__traceback__.tb_frame.f_code.co_filename
+                )
+                current_dir = os.path.dirname(os.path.abspath(__file__))
+                if error_dir == current_dir:
+                    print(
+                        "Unexpected shutdown. Make sure to call itl.stop() before exiting the program."
+                    )
+
+        else:
+            print(f"Exception: {context}")
```

### Comparing `itllib-0.0.8/src/itllib/loops.py` & `itllib-0.0.9/src/itllib/loops.py`

 * *Files identical despite different names*

### Comparing `itllib-0.0.8/src/itllib/piles.py` & `itllib-0.0.9/src/itllib/piles.py`

 * *Files identical despite different names*

### Comparing `itllib-0.0.8/src/itllib/resources.py` & `itllib-0.0.9/src/itllib/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         ):
             raise ValueError()
         self.config = config
         self.name = config["metadata"]["name"]
         self.parent_ref_or_id = ResourceIdRef("Client", config["spec"]["ownerId"])
         self.remote = config["spec"]["remote"]
 
-    def resource_ids(self) -> ResourceIdRef:
+    def resource_ids(self) -> Generator[ResourceIdRef, None, None]:
         yield ResourceIdRef("Loop", self.config["spec"]["loopId"])
 
     def connection_info(self, resolver: "ResourceResolver"):
         loop_id = resolver.link(self.config["spec"]["loopId"])
 
         base = resolver.get_remote_config(self.remote)["loops"]
         rest_base, ws_base = _split_base_uri(base)
@@ -534,15 +534,29 @@
         yield
 
     def loop(self, resolver: "ResourceResolver") -> LoopResource:
         return self.parent(resolver)
 
     def connection_info(self, resolver: "ResourceResolver") -> StreamConnectionInfo:
         stream_id = resolver.link(self.config["spec"]["streamId"])
-        loop_info = self.loop(resolver).connection_info(resolver)
+
+        if "loopId" in self.config["spec"]:
+            loop_id = self.config["spec"]["loopId"]
+
+            base = resolver.get_remote_config(self.remote)["loops"]
+            rest_base, ws_base = _split_base_uri(base)
+            path = "/loop/" + loop_id
+
+            loop_info = LoopConnectionInfo(
+                rest_info=ConnectionInfo(rest_base, path),
+                ws_info=ConnectionInfo(ws_base, path),
+            )
+        else:
+            loop_info = self.loop(resolver).connection_info(resolver)
+
         group = None
         return loop_info.stream_connection_info(stream_id, group)
 
 
 class ClusterResource(Resource):
     def __init__(self, config):
         self.kind = "Cluster"
@@ -1002,80 +1016,154 @@
         new_config_sources = self.map_config_locations(new_configs)
         new_compiled_resources = self.compile_configs(new_configs)
 
         self.known_keys = new_keys
         self.config_sources = new_config_sources
         self.compiled_resources = new_compiled_resources
 
-    def read_resource_configs_file(
-        self, file, read_fully=False
+    def read_resource_config_docs(
+        self, source, configs, read_fully=False
     ) -> Generator[LocatedConfig, None, None]:
-        try:
-            with open(file, "r") as f:
-                configs = list(yaml.safe_load_all(f.read()))
-        except Exception as e:
-            print(f"Failed to read file {file}:", e.args)
-            if read_fully:
-                raise e
-            return
-
         for i, config in enumerate(configs):
             if read_fully:
-                yield LocatedConfig(file, i, config)
+                yield LocatedConfig(source, i, config)
                 continue
 
             if "apiVersion" not in config:
-                print(f"Config in file {file} is missing apiVersion")
+                print(f"Config in file {source} is missing apiVersion")
                 continue
             if not isinstance(config["apiVersion"], str):
                 print(
-                    f"Config in file {file} has invalid apiVersion. It should be a string."
+                    f"Config in file {source} has invalid apiVersion. It should be a string."
                 )
                 continue
             if not re.match(r"^[a-z0-9.-]+/[a-z0-9.-]+$", config["apiVersion"]):
                 print(
-                    f"Config in file {file} has invalid apiVersion. It should be in the format group/version. Group and version should be lowercase alphanumeric characters, dots or dashes."
+                    f"Config in file {source} has invalid apiVersion. It should be in the format group/version. Group and version should be lowercase alphanumeric characters, dots or dashes."
                 )
                 continue
             if "kind" not in config:
-                print(f"Config in file {file} is missing kind")
+                print(f"Config in file {source} is missing kind")
                 continue
             if not isinstance(config["kind"], str):
-                print(f"Config in file {file} has invalid kind. It should be a string.")
+                print(
+                    f"Config in file {source} has invalid kind. It should be a string."
+                )
                 continue
             if "metadata" not in config:
-                print(f"Config in file {file} is missing metadata")
+                print(f"Config in file {source} is missing metadata")
                 continue
             if not isinstance(config["metadata"], dict):
                 print(
-                    f"Config in file {file} has invalid metadata. It should be a dict."
+                    f"Config in file {source} has invalid metadata. It should be a dict."
                 )
                 continue
             if "name" not in config["metadata"]:
-                print(f"Config in file {file} is missing metadata.name")
+                print(f"Config in file {source} is missing metadata.name")
                 continue
             if not isinstance(config["metadata"]["name"], str):
                 print(
-                    f"Config in file {file} has invalid metadata.name. It should be a string."
+                    f"Config in file {source} has invalid metadata.name. It should be a string."
                 )
                 continue
 
             if config["apiVersion"] != "thatone.ai/v1":
                 print(
-                    f"Skipping config in {file} with apiVersion {config['apiVersion']}."
+                    f"Skipping config in {source} with apiVersion {config['apiVersion']}."
                 )
                 continue
             if config["kind"] not in CONFIG_KINDS:
-                print(f"Skipping config in {file} with kind {config['kind']}.")
+                print(f"Skipping config in {source} with kind {config['kind']}.")
                 continue
 
-            yield LocatedConfig(file, i, config)
+            yield LocatedConfig(source, i, config)
+
+    def read_resource_configs_file(
+        self, file, read_fully=False
+    ) -> Generator[LocatedConfig, None, None]:
+        try:
+            with open(file, "r") as f:
+                configs = list(yaml.safe_load_all(f.read()))
+        except Exception as e:
+            print(f"Failed to read file {file}:", e.args)
+            if read_fully:
+                raise e
+            return
+
+        yield from self.read_resource_config_docs(file, configs)
+
+    def read_resource_configs_url(
+        self, url, read_fully=False
+    ) -> Generator[LocatedConfig, None, None]:
+        parsed_url = urlparse(url)
+
+        if parsed_url.netloc == "github.com":
+            path_parts = parsed_url.path.split("/", maxsplit=5)
+            if len(path_parts) < 6:
+                print(f"Invalid github link {url}")
+                return
+            print(path_parts)
+            _, user, project, link_type, branch, path_rest = path_parts
+
+            if link_type == "blob":
+                contents = httpx.get(
+                    f"https://raw.githubusercontent.com/{user}/{project}/{branch}/{path_rest}"
+                ).text
+                configs = list(yaml.safe_load_all(contents))
+                yield from self.read_resource_config_docs(
+                    url, configs, read_fully=read_fully
+                )
+            elif link_type == "tree":
+                files = httpx.get(
+                    f"https://api.github.com/repos/{user}/{project}/contents/{path_rest}?ref={branch}&recursive=1"
+                ).json()
+                for file in files:
+                    if file["type"] != "file":
+                        continue
+                    if not file["name"].endswith(".yaml"):
+                        continue
+                    contents = httpx.get(file["download_url"]).text
+                    configs = list(yaml.safe_load_all(contents))
+                    yield from self.read_resource_config_docs(
+                        file["download_url"], configs, read_fully=read_fully
+                    )
+            else:
+                print(f"Invalid github link {url}")
+        elif parsed_url.netloc == "gist.github.com":
+            _, user, path_parts = parsed_url.path.split("/", maxsplit=2)
+            id_parts = path_parts.split("/")
+            if len(id_parts) == 2:
+                gist_id, revision = id_parts
+                download_url = f"https://gist.githubusercontent.com/{user}/{gist_id}/raw/{revision}"
+            elif len(id_parts) == 1:
+                gist_id = id_parts[0]
+                download_url = (
+                    f"https://gist.githubusercontent.com/{user}/{gist_id}/raw"
+                )
+            else:
+                print(f"Invalid gist link {url}")
+                return
+            contents = httpx.get(download_url).text
+            configs = list(yaml.safe_load_all(contents))
+            yield from self.read_resource_config_docs(
+                download_url, configs, read_fully=read_fully
+            )
+
+        else:
+            contents = httpx.get(url).text
+            configs = list(yaml.safe_load_all(contents))
+            yield from self.read_resource_config_docs(
+                url, configs, read_fully=read_fully
+            )
 
     def read_resource_configs(self, dirpath, read_fully=False) -> List[LocatedConfig]:
         """Read the given file and return its contents."""
+        if dirpath.startswith("http:") or dirpath.startswith("https:"):
+            return list(self.read_resource_configs_url(dirpath, read_fully=read_fully))
+
         dirpath = os.path.realpath(dirpath)
         if os.path.isfile(dirpath):
             return list(self.read_resource_configs_file(dirpath, read_fully=read_fully))
 
         result: List[LocatedConfig] = []
         for root, dirs, files in os.walk(dirpath):
             for filepath in files:
@@ -1171,15 +1259,15 @@
 
         for located_config in new_configs:
             try:
                 generated_resources = self._compile_config(located_config)
                 for resource in generated_resources:
                     key = resource.reference
                     if key in new_compiled_resources:
-                        print("skipping", key, "since it was already generated")
+                        print("Skipping", key, "since it was already generated")
                         continue
                     new_compiled_resources[key] = resource
             except ValueError as e:
                 error = True
             except Exception as e:
                 raise e
 
@@ -1204,31 +1292,35 @@
         for located_config in prior_configs.values():
             updated_configs[located_config.path].append(located_config.config)
 
         for target_resource in unlinked_resources.values():
             reference = target_resource.reference
             if reference in prior_configs:
                 location = prior_configs[reference]
-                updated_configs[location.path][location.index] = target_resource.link(
-                    resolver
-                )
-                updated_yaml_files.add(location.path)
-            else:
-                if target_resource.kind == "ApiKey":
-                    target_file = resolver.create_secret_path(target_resource.config)
-                else:
-                    target_file = resolver.create_resource_path(target_resource.config)
-
-                try:
-                    updated_configs[target_file].append(target_resource.link(resolver))
-                except ValueError as e:
-                    print("Failed to generate config for", reference)
-                    error = True
+                if not location.path.startswith(
+                    "http://"
+                ) and not location.path.startswith("https://"):
+                    updated_configs[location.path][
+                        location.index
+                    ] = target_resource.link(resolver)
+                    updated_yaml_files.add(location.path)
                     continue
-                updated_yaml_files.add(target_file)
+
+            if target_resource.kind == "ApiKey":
+                target_file = resolver.create_secret_path(target_resource.config)
+            else:
+                target_file = resolver.create_resource_path(target_resource.config)
+
+            try:
+                updated_configs[target_file].append(target_resource.link(resolver))
+            except ValueError as e:
+                print("Failed to generate config for", reference)
+                error = True
+                continue
+            updated_yaml_files.add(target_file)
 
         if error:
             raise ValueError()
 
         return {x: updated_configs[x] for x in updated_yaml_files}
 
     def apply(
@@ -1244,14 +1336,15 @@
             with open(filepath, "w") as outp:
                 yaml.dump_all(
                     configs,
                     stream=outp,
                     default_flow_style=False,
                     sort_keys=False,
                     explicit_end=False,
+                    explicit_start=True,
                 )
 
         for resource in self.compiled_resources.values():
             try:
                 resource.apply(resolver)
             except Exception as e:
                 print(f"Failed to apply {resource.reference}")
@@ -1265,14 +1358,15 @@
             with open(path, "w") as outp:
                 yaml.dump(
                     apikey.link(resolver),
                     outp,
                     default_flow_style=False,
                     sort_keys=False,
                     explicit_end=False,
+                    explicit_start=True,
                 )
 
 
 class ResourceResolver:
     def __init__(
         self,
         prior_resources: ResourcePile,
```

### Comparing `itllib-0.0.8/src/itllib/secrets.py` & `itllib-0.0.9/src/itllib/secrets.py`

 * *Files identical despite different names*

### Comparing `itllib-0.0.8/.gitignore` & `itllib-0.0.9/.gitignore`

 * *Files identical despite different names*

