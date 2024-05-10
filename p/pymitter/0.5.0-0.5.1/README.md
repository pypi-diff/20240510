# Comparing `tmp/pymitter-0.5.0.tar.gz` & `tmp/pymitter-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymitter-0.5.0.tar", last modified: Wed Nov 22 14:30:53 2023, max compression
+gzip compressed data, was "pymitter-0.5.1.tar", last modified: Fri May 10 07:37:38 2024, max compression
```

## Comparing `pymitter-0.5.0.tar` & `pymitter-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 14:30:53.647124 pymitter-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-22 14:30:36.000000 pymitter-0.5.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-22 14:30:36.000000 pymitter-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-22 14:30:36.000000 pymitter-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2023-11-22 14:30:53.647124 pymitter-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2023-11-22 14:30:36.000000 pymitter-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 14:30:53.647124 pymitter-0.5.0/pymitter/
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2023-11-22 14:30:37.000000 pymitter-0.5.0/pymitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 14:30:53.647124 pymitter-0.5.0/pymitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2023-11-22 14:30:53.000000 pymitter-0.5.0/pymitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-11-22 14:30:53.000000 pymitter-0.5.0/pymitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 14:30:53.000000 pymitter-0.5.0/pymitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-22 14:30:53.000000 pymitter-0.5.0/pymitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-22 14:30:53.000000 pymitter-0.5.0/pymitter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-11-22 14:30:37.000000 pymitter-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 14:30:37.000000 pymitter-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-22 14:30:37.000000 pymitter-0.5.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-22 14:30:53.647124 pymitter-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:37:38.843501 pymitter-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 07:37:28.000000 pymitter-0.5.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 07:37:28.000000 pymitter-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 07:37:28.000000 pymitter-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-10 07:37:38.843501 pymitter-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-10 07:37:28.000000 pymitter-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:37:38.839501 pymitter-0.5.1/pymitter/
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-05-10 07:37:28.000000 pymitter-0.5.1/pymitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:37:38.843501 pymitter-0.5.1/pymitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-10 07:37:38.000000 pymitter-0.5.1/pymitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-10 07:37:38.000000 pymitter-0.5.1/pymitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:37:38.000000 pymitter-0.5.1/pymitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 07:37:38.000000 pymitter-0.5.1/pymitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 07:37:38.000000 pymitter-0.5.1/pymitter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-10 07:37:28.000000 pymitter-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:37:28.000000 pymitter-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-10 07:37:28.000000 pymitter-0.5.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:37:38.843501 pymitter-0.5.1/setup.cfg
```

### Comparing `pymitter-0.5.0/LICENSE` & `pymitter-0.5.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2014-2023, Marcel Rieger
+Copyright (c) 2014-2024, Marcel Rieger
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pymitter-0.5.0/PKG-INFO` & `pymitter-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymitter
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python port of the extended Node.js EventEmitter 2 approach providing namespaces, wildcards and TTL.
 Author-email: Marcel Rieger <github.riga@icloud.com>
-License: Copyright (c) 2014-2023, Marcel Rieger
+License: Copyright (c) 2014-2024, Marcel Rieger
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
@@ -48,17 +48,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: flake8>=4.0; extra == "dev"
-Requires-Dist: flake8-commas>=2.1; extra == "dev"
-Requires-Dist: flake8-quotes>=3.3; extra == "dev"
+Requires-Dist: mypy~=1.9.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: flake8~=7.0.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: flake8~=5.0.0; python_version < "3.8" and extra == "dev"
+Requires-Dist: flake8-commas~=2.1.0; extra == "dev"
+Requires-Dist: flake8-quotes~=3.3.2; extra == "dev"
+Requires-Dist: types-docutils~=0.20.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0; extra == "dev"
 
 <!-- marker-before-logo -->
 
 <p align="center">
   <img src="https://media.githubusercontent.com/media/riga/pymitter/master/assets/logo.png" width="400" />
 </p>
```

### Comparing `pymitter-0.5.0/README.md` & `pymitter-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pymitter-0.5.0/pymitter/__init__.py` & `pymitter-0.5.1/pymitter/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 Python port of the extended Node.js EventEmitter 2 approach providing namespaces, wildcards and TTL.
 """
 
 from __future__ import annotations
 
 __author__ = "Marcel Rieger"
 __author_email__ = "github.riga@icloud.com"
-__copyright__ = "Copyright 2014-2023, Marcel Rieger"
+__copyright__ = "Copyright 2014-2024, Marcel Rieger"
 __credits__ = ["Marcel Rieger"]
 __contact__ = "https://github.com/riga/pymitter"
 __license__ = "BSD-3-Clause"
 __status__ = "Development"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 __all__ = ["EventEmitter", "Listener"]
 
 import time
-import collections
 import fnmatch
 import asyncio
-from typing import Callable, Awaitable, Sequence, Any
+from typing import Callable, Awaitable, Sequence, Any, Generator
 
 
 class EventEmitter(object):
     """
     The EventEmitter class, ported from Node.js EventEmitter 2.
 
     When *wildcard* is *True*, wildcards in event names are taken into account. Event names have
@@ -34,15 +33,15 @@
     is registered with arguments ``(func, event=None)``. *max_listeners* configures the total
     maximum number of event listeners. A negative numbers means that this number is unlimited.
     """
 
     new_listener_event = "new_listener"
 
     def __init__(
-        self: EventEmitter,
+        self,
         *,
         delimiter: str = ".",
         wildcard: bool = False,
         new_listener: bool = False,
         max_listeners: int = -1,
     ) -> None:
         super().__init__()
@@ -51,22 +50,22 @@
         self.new_listener = new_listener
         self.max_listeners = max_listeners
 
         # tree of nodes keeping track of nested events
         self._event_tree = Tree(wildcard=wildcard, delimiter=delimiter)
 
         # flat list of listeners triggerd on "any" event
-        self._any_listeners = []
+        self._any_listeners: list[Listener] = []
 
     @property
-    def num_listeners(self: EventEmitter) -> int:
+    def num_listeners(self) -> int:
         return self._event_tree.num_listeners() + len(self._any_listeners)
 
     def on(
-        self: EventEmitter,
+        self,
         event: str,
         func: Callable | None = None,
         ttl: int = -1,
     ) -> Callable:
         """
         Registers a function to an event. *ttl* defines the times to listen with negative values
         meaning infinity. When *func* is *None*, decorator usage is assumed. Returns the wrapped
@@ -81,92 +80,92 @@
             self._event_tree.add_listener(event, Listener(func, event, ttl))
 
             if self.new_listener and event != self.new_listener_event:
                 self.emit(self.new_listener_event, func, event)
 
             return func
 
-        return on(func) if func else on
+        return on(func) if func else on  # type: ignore[return-value]
 
-    def once(self: EventEmitter, event: str, func: Callable | None = None) -> Callable:
+    def once(self, event: str, func: Callable | None = None) -> Callable:
         """
         Registers a function to an event that is called once. When *func* is *None*, decorator usage
         is assumed. Returns the wrapped function.
         """
         return self.on(event, func=func, ttl=1)
 
-    def on_any(self: EventEmitter, func: Callable | None = None, ttl: int = -1) -> Callable:
+    def on_any(self, func: Callable | None = None, ttl: int = -1) -> Callable:
         """
         Registers a function that is called every time an event is emitted. *ttl* defines the times
         to listen with negative values meaning infinity. When *func* is *None*, decorator usage is
         assumed. Returns the wrapped function.
         """
         def on_any(func: Callable) -> Callable:
             # do not register the function when the maximum would be exceeded
             if 0 <= self.max_listeners <= self.num_listeners:
                 return func
 
             # create a new listener and add it
-            self._any_listeners.append(Listener(func, None, ttl))
+            self._any_listeners.append(Listener(func, "", ttl))
 
             if self.new_listener:
                 self.emit(self.new_listener_event, func)
 
             return func
 
-        return on_any(func) if func else on_any
+        return on_any(func) if func else on_any  # type: ignore[return-value]
 
-    def off(self: EventEmitter, event: str, func: Callable | None = None) -> Callable:
+    def off(self, event: str, func: Callable | None = None) -> Callable:
         """
         Removes a function that is registered to an event. When *func* is *None*, decorator usage is
         assumed. Returns the wrapped function.
         """
         def off(func: Callable) -> Callable:
             self._event_tree.remove_listeners_by_func(event, func)
 
             return func
 
-        return off(func) if func else off
+        return off(func) if func else off  # type: ignore[return-value]
 
-    def off_any(self: EventEmitter, func: Callable | None = None) -> Callable:
+    def off_any(self, func: Callable | None = None) -> Callable:
         """
         Removes a function that was registered via :py:meth:`on_any`. When *func* is *None*,
         decorator usage is assumed. Returns the wrapped function.
         """
         def off_any(func: Callable) -> Callable:
             self._any_listeners[:] = [
                 listener
                 for listener in self._any_listeners
                 if listener.func != func
             ]
 
             return func
 
-        return off_any(func) if func else off_any
+        return off_any(func) if func else off_any  # type: ignore[return-value]
 
-    def off_all(self: EventEmitter) -> None:
+    def off_all(self) -> None:
         """
         Removes all registered functions.
         """
         self._event_tree.clear()
         del self._any_listeners[:]
 
-    def listeners(self: EventEmitter, event: str) -> list[Callable]:
+    def listeners(self, event: str) -> list[Callable]:
         """
         Returns all functions that are registered to an event.
         """
         return [listener.func for listener in self._event_tree.find_listeners(event)]
 
-    def listeners_any(self: EventEmitter) -> list[Callable]:
+    def listeners_any(self) -> list[Callable]:
         """
         Returns all functions that were registered using :py:meth:`on_any`.
         """
         return [listener.func for listener in self._any_listeners]
 
-    def listeners_all(self: EventEmitter) -> list[Callable]:
+    def listeners_all(self) -> list[Callable]:
         """
         Returns all registered functions, ordered by their registration time.
         """
         listeners = list(self._any_listeners)
         nodes = list(self._event_tree.nodes.values())
         while nodes:
             node = nodes.pop(0)
@@ -174,101 +173,101 @@
             listeners.extend(node.listeners)
 
         # sort them
         listeners = sorted(listeners, key=lambda listener: listener.time)
 
         return [listener.func for listener in listeners]
 
-    def _emit(self: EventEmitter, event: str, *args, **kwargs) -> list[Awaitable]:
+    def _emit(self, event: str, *args, **kwargs) -> list[Awaitable]:
         listeners = self._event_tree.find_listeners(event)
         if event != self.new_listener_event:
             listeners.extend(self._any_listeners)
         listeners = sorted(listeners, key=lambda listener: listener.time)
 
         # call listeners in order, keep track of awaitables from coroutines functions
         awaitables = []
         for listener in listeners:
             # since listeners can emit events themselves,
             # deregister them before calling if needed
             if listener.ttl == 1:
                 self.off(listener.event, func=listener.func)
 
             res = listener(*args, **kwargs)
-            if listener.is_coroutine:
+            if listener.is_coroutine or listener.is_async_callable:
                 awaitables.append(res)
 
         return awaitables
 
-    def emit(self: EventEmitter, event: str, *args, **kwargs) -> None:
+    def emit(self, event: str, *args, **kwargs) -> None:
         """
         Emits an *event*. All functions of events that match *event* are invoked with *args* and
         *kwargs* in the exact order of their registration, with the exception of async functions
         that are invoked in a separate event loop.
         """
         # emit normal functions and get awaitables of async ones
         awaitables = self._emit(event, *args, **kwargs)
 
         # handle awaitables
         if awaitables:
             async def start():
                 await asyncio.gather(*awaitables)
             asyncio.run(start())
 
-    async def emit_async(self: EventEmitter, event: str, *args, **kwargs) -> Awaitable:
+    async def emit_async(self, event: str, *args, **kwargs) -> None:
         """
         Awaitable version of :py:meth:`emit`. However, this method does not start a new event loop
         but uses the existing one.
         """
         # emit normal functions and get awaitables of async ones
         awaitables = self._emit(event, *args, **kwargs)
 
         # handle awaitables
         if awaitables:
             await asyncio.gather(*awaitables)
 
-    def emit_future(self: EventEmitter, event: str, *args, **kwargs) -> None:
+    def emit_future(self, event: str, *args, **kwargs) -> None:
         """
         Deferred version of :py:meth:`emit` with all awaitable events being places at the end of the
         existing event loop (using :py:func:`asyncio.ensure_future`).
         """
         # emit normal functions and get awaitables of async ones
         awaitables = self._emit(event, *args, **kwargs)
 
         # handle awaitables
         if awaitables:
             asyncio.ensure_future(asyncio.gather(*awaitables))
 
 
 class BaseNode(object):
 
-    def __init__(self: BaseNode, wildcard: bool, delimiter: str) -> None:
+    def __init__(self, wildcard: bool, delimiter: str) -> None:
         super().__init__()
 
         self.wildcard = wildcard
         self.delimiter = delimiter
         self.parent = None
-        self.nodes = collections.OrderedDict()
+        self.nodes: dict[str, Node] = {}
 
-    def clear(self: BaseNode) -> None:
+    def clear(self) -> None:
         self.nodes.clear()
 
-    def add_node(self: BaseNode, node: "Node") -> "Node":
+    def add_node(self, node: "Node") -> "Node":
         # when there is a node with the exact same name (pattern), merge listeners
         if node.name in self.nodes:
             _node = self.nodes[node.name]
             _node.listeners.extend(node.listeners)
             return _node
 
         # otherwise add it and set its parent
         self.nodes[node.name] = node
-        node.parent = self
+        node.parent = self  # type: ignore[assignment]
 
         return node
 
-    def walk_nodes(self: BaseNode) -> None:
+    def walk_nodes(self) -> Generator[tuple[str, tuple[str, ...], list[str]], None, None]:
         queue = [
             (name, [name], node)
             for name, node in self.nodes.items()
         ]
         while queue:
             name, path, node = queue.pop(0)
 
@@ -291,53 +290,53 @@
     Actual named nodes containing listeners.
     """
 
     @classmethod
     def str_is_pattern(cls, s: str) -> bool:
         return "*" in s or "?" in s
 
-    def __init__(self: Node, name: str, *args) -> None:
+    def __init__(self, name: str, *args) -> None:
         super().__init__(*args)
 
         self.name = name
-        self.listeners = []
+        self.listeners: list[Listener] = []
 
-    def num_listeners(self: Node, recursive: bool = True) -> int:
+    def num_listeners(self, recursive: bool = True) -> int:
         n = len(self.listeners)
 
         if recursive:
             n += sum(node.num_listeners(recursive=recursive) for node in self.nodes.values())
 
         return n
 
-    def remove_listeners_by_func(self: Node, func: Callable) -> None:
+    def remove_listeners_by_func(self, func: Callable) -> None:
         self.listeners[:] = [listener for listener in self.listeners if listener.func != func]
 
-    def add_listener(self: Node, listener: "Listener") -> None:
+    def add_listener(self, listener: Listener) -> None:
         self.listeners.append(listener)
 
-    def check_name(self: Node, pattern: str) -> bool:
+    def check_name(self, pattern: str) -> bool:
         if self.wildcard:
             if self.str_is_pattern(pattern):
                 return fnmatch.fnmatch(self.name, pattern)
             if self.str_is_pattern(self.name):
                 return fnmatch.fnmatch(pattern, self.name)
 
         return self.name == pattern
 
-    def find_nodes(self: Node, event: str | Sequence[str]) -> list[Node]:
+    def find_nodes(self, event: str | Sequence[str]) -> list[Node]:
         # trivial case
         if not event:
             return []
 
         # parse event
         if isinstance(event, (list, tuple)):
             pattern, sub_patterns = event[0], event[1:]
         else:
-            pattern, *sub_patterns = event.split(self.delimiter)
+            pattern, *sub_patterns = event.split(self.delimiter)  # type: ignore[attr-defined]
 
         # first make sure that pattern matches _this_ name
         if not self.check_name(pattern):
             return []
 
         # when there are no sub patterns, return this one
         if not sub_patterns:
@@ -348,43 +347,43 @@
 
 
 class Tree(BaseNode):
     """
     Top-level node without a name or listeners, but providing higher-level node access.
     """
 
-    def num_listeners(self: Tree) -> int:
+    def num_listeners(self) -> int:
         return sum(node.num_listeners(recursive=True) for node in self.nodes.values())
 
-    def find_nodes(self: Tree, *args, **kwargs) -> list[Node]:
+    def find_nodes(self, *args, **kwargs) -> list[Node]:
         return sum((node.find_nodes(*args, **kwargs) for node in self.nodes.values()), [])
 
-    def add_listener(self: Tree, event: str, listener: "Listener") -> None:
+    def add_listener(self, event: str, listener: Listener) -> None:
         # add nodes without evaluating wildcards, this is done during node lookup only
         names = event.split(self.delimiter)
 
         # lookup the deepest existing parent
         node = self
         while names:
             name = names.pop(0)
             if name in node.nodes:
-                node = node.nodes[name]
+                node = node.nodes[name]  # type: ignore[assignment]
             else:
                 new_node = Node(name, self.wildcard, self.delimiter)
                 node.add_node(new_node)
-                node = new_node
+                node = new_node  # type: ignore[assignment]
 
         # add the listeners
-        node.add_listener(listener)
+        node.add_listener(listener)  # type: ignore[arg-type, call-arg]
 
-    def remove_listeners_by_func(self: Tree, event: str, func: Callable) -> None:
+    def remove_listeners_by_func(self, event: str, func: Callable) -> None:
         for node in self.find_nodes(event):
             node.remove_listeners_by_func(func)
 
-    def find_listeners(self: Tree, event: str, sort: bool = True) -> list["Listener"]:
+    def find_listeners(self, event: str, sort: bool = True) -> list[Listener]:
         listeners = sum((node.listeners for node in self.find_nodes(event)), [])
 
         # sort by registration time
         if sort:
             listeners = sorted(listeners, key=lambda listener: listener.time)
 
         return listeners
@@ -403,18 +402,22 @@
         self.event = event
         self.ttl = ttl
 
         # store the registration time
         self.time = time.monotonic()
 
     @property
-    def is_coroutine(self: Listener) -> bool:
+    def is_coroutine(self) -> bool:
         return asyncio.iscoroutinefunction(self.func)
 
-    def __call__(self: Listener, *args, **kwargs) -> Any:
+    @property
+    def is_async_callable(self) -> bool:
+        return asyncio.iscoroutinefunction(getattr(self.func, "__call__", None))
+
+    def __call__(self, *args, **kwargs) -> Any:
         """
         Invokes the wrapped function when ttl is non-zero, decreases the ttl value when positive and
         returns its return value.
         """
         result = None
         if self.ttl != 0:
             result = self.func(*args, **kwargs)
```

### Comparing `pymitter-0.5.0/pymitter.egg-info/PKG-INFO` & `pymitter-0.5.1/pymitter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymitter
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python port of the extended Node.js EventEmitter 2 approach providing namespaces, wildcards and TTL.
 Author-email: Marcel Rieger <github.riga@icloud.com>
-License: Copyright (c) 2014-2023, Marcel Rieger
+License: Copyright (c) 2014-2024, Marcel Rieger
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
@@ -48,17 +48,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: flake8>=4.0; extra == "dev"
-Requires-Dist: flake8-commas>=2.1; extra == "dev"
-Requires-Dist: flake8-quotes>=3.3; extra == "dev"
+Requires-Dist: mypy~=1.9.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: flake8~=7.0.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: flake8~=5.0.0; python_version < "3.8" and extra == "dev"
+Requires-Dist: flake8-commas~=2.1.0; extra == "dev"
+Requires-Dist: flake8-quotes~=3.3.2; extra == "dev"
+Requires-Dist: types-docutils~=0.20.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0; extra == "dev"
 
 <!-- marker-before-logo -->
 
 <p align="center">
   <img src="https://media.githubusercontent.com/media/riga/pymitter/master/assets/logo.png" width="400" />
 </p>
```

### Comparing `pymitter-0.5.0/pyproject.toml` & `pymitter-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -59,7 +59,12 @@
 include-package-data = false
 
 
 [tool.setuptools.packages.find]
 
 include = ["pymitter"]
 exclude = ["tests/*"]
+
+
+[tool.mypy]
+
+exclude = '(?x)(docs|tests)'
```

