# Comparing `tmp/agentops-0.1.8.tar.gz` & `tmp/agentops-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.8.tar", last modified: Sat May  4 03:01:49 2024, max compression
+gzip compressed data, was "agentops-0.1.9.tar", last modified: Tue May  7 07:07:25 2024, max compression
```

## Comparing `agentops-0.1.8.tar` & `agentops-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.256699 agentops-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 03:01:44.000000 agentops-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-04 03:01:49.256699 agentops-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-04 03:01:44.000000 agentops-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.252699 agentops-0.1.8/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4857 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-04 03:01:44.000000 agentops-0.1.8/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.256699 agentops-0.1.8/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 03:01:49.000000 agentops-0.1.8/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-04 03:01:44.000000 agentops-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 03:01:49.256699 agentops-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:01:49.256699 agentops-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-04 03:01:44.000000 agentops-0.1.8/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.996352 agentops-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-07 07:07:19.000000 agentops-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-07 07:07:25.996352 agentops-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-07 07:07:19.000000 agentops-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.992352 agentops-0.1.9/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5027 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22363 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.992352 agentops-0.1.9/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-07 07:07:19.000000 agentops-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:07:25.996352 agentops-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.992352 agentops-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_teardown.py
```

### Comparing `agentops-0.1.8/LICENSE` & `agentops-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/PKG-INFO` & `agentops-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: packaging==23.2
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
 
 <div align="center">
   <a href="https://agentops.ai?ref=gh">
-    <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+    <img src="https://github.com/AgentOps-AI/agentops/blob/df22e9dffb7294fb977dc103a2ca3bcf8f04946f/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
   </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.8 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.9 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
 Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
 requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
 langchain>=0.0.354; extra == "langchain"
                                     _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
```

### Comparing `agentops-0.1.8/README.md` & `agentops-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
   <a href="https://agentops.ai?ref=gh">
-    <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+    <img src="https://github.com/AgentOps-AI/agentops/blob/df22e9dffb7294fb977dc103a2ca3bcf8f04946f/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
   </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
```

### Comparing `agentops-0.1.8/agentops/__init__.py` & `agentops-0.1.9/agentops/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # agentops/__init__.py
 from os import environ
-from typing import Optional, List
+from typing import Optional, List, Union
 
 from .client import Client
 from .config import Configuration
 from .event import Event, ActionEvent, LLMEvent, ToolEvent, ErrorEvent
 from .enums import Models
 from .decorators import record_function
 from .agent import track_agent
 from .log_config import set_logging_level_info, set_logging_level_critial
+from .langchain_callback_handler import LangchainCallbackHandler, AsyncLangchainCallbackHandler
 
 
 def init(api_key: Optional[str] = None,
          parent_key: Optional[str] = None,
          endpoint: Optional[str] = None,
          max_wait_time: Optional[int] = None,
          max_queue_size: Optional[int] = None,
@@ -82,15 +83,15 @@
             tags (List[str], optional): Tags that can be used for grouping or sorting later.
                 e.g. ["test_run"].
             config: (Configuration, optional): Client configuration object
     """
     return Client().start_session(tags, config, inherited_session_id)
 
 
-def record(event: Event | ErrorEvent):
+def record(event: Union[Event, ErrorEvent]):
     """
         Record an event with the AgentOps service.
 
         Args:
             event (Event): The event to record.
     """
     Client().record(event)
@@ -124,7 +125,10 @@
     """
         Set the parent API key which has visibility to projects it is parent to.
 
         Args:
             parent_key (str): The API key of the parent organization to set.
     """
     Client().set_parent_key(parent_key)
+
+def stop_instrumenting():
+    Client().stop_instrumenting()
```

### Comparing `agentops-0.1.8/agentops/agent.py` & `agentops-0.1.9/agentops/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+from typing import Union
+
 from .log_config import logger
 from uuid import uuid4
 from agentops import Client
 from inspect import isclass, isfunction
 
 
-def track_agent(name: str | None = None):
+def track_agent(name: Union[str, None] = None):
     def decorator(obj):
         if name:
             obj.agent_ops_agent_name = name
 
         if isclass(obj):
             original_init = obj.__init__
 
             def new_init(self, *args, **kwargs):
                 try:
                     original_init(self, *args, **kwargs)
-                    self.agent_ops_agent_id = uuid4()
+                    self.agent_ops_agent_id = str(uuid4())
                     Client().create_agent(self.agent_ops_agent_id, self.agent_ops_agent_name)
                 except AttributeError as e:
                     logger.warning("AgentOps failed to track an agent. This often happens if agentops.init() was not "
                                   "called before initializing an agent with the @track_agent decorator.")
                     raise e
 
             obj.__init__ = new_init
 
         elif isfunction(obj):
-            obj.agent_ops_agent_id = uuid4()
+            obj.agent_ops_agent_id = str(uuid4())
             Client().create_agent(obj.agent_ops_agent_id, obj.agent_ops_agent_name)
 
         else:
             raise Exception("Invalid input, 'obj' must be a class or a function")
 
         return obj
```

### Comparing `agentops-0.1.8/agentops/client.py` & `agentops-0.1.9/agentops/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .event import ActionEvent, ErrorEvent, Event
 from .enums import EndState
 from .helpers import get_ISO_time, singleton, check_call_stack_for_agent_id
 from .session import Session
 from .worker import Worker
 from .host_env import get_host_env
 from uuid import uuid4
-from typing import Optional, List
+from typing import Optional, List, Union
 import traceback
 from .log_config import logger, set_logging_level_info
 from decimal import Decimal
 import inspect
 import atexit
 import signal
 import sys
@@ -69,17 +69,18 @@
                  ):
 
         if override is not None:
             logger.warning("🖇 AgentOps: The 'override' parameter is deprecated. Use 'instrument_llm_calls' instead.",
                            DeprecationWarning, stacklevel=2)
             instrument_llm_calls = instrument_llm_calls or override
 
-        self._session = None
-        self._worker = None
-        self._tags_for_future_session = None
+        self._session: Optional[Session] = None
+        self._worker: Optional[Worker] = None
+        self._tags: Optional[List[str]] = tags
+        self._tags_for_future_session: Optional[List[str]] = None
 
         self._env_data_opt_out = os.getenv('AGENTOPS_ENV_DATA_OPT_OUT') and os.getenv(
             'AGENTOPS_ENV_DATA_OPT_OUT').lower() == 'true'
 
         try:
             self.config = Configuration(api_key=api_key,
                                         parent_key=parent_key,
@@ -110,53 +111,53 @@
         if self._session.tags is not None:
             for tag in tags:
                 if tag not in self._session.tags:
                     self._session.tags.append(tag)
         else:
             self._session.tags = tags
 
-        if self._session is not None:
+        if self._session is not None and self._worker is not None:
             self._worker.update_session(self._session)
 
     def set_tags(self, tags: List[str]):
         """
             Replace session tags at runtime.
 
             Args:
                 tags (List[str]): The list of tags to set.
         """
         self._tags_for_future_session = tags
 
-        if self._session is not None:
+        if self._session is not None and self._worker is not None:
             self._session.tags = tags
             self._worker.update_session(self._session)
 
-    def record(self, event: Event | ErrorEvent):
+    def record(self, event: Union[Event, ErrorEvent]):
         """
             Record an event with the AgentOps service.
 
             Args:
                 event (Event): The event to record.
         """
         if self._session is None or self._session.has_ended:
             logger.warning("🖇 AgentOps: Cannot record event - no current session")
             return
 
-        # Need to update end_timestamp for ErrorEvent so creating this event_local pointer
-        event_local = event.trigger_event if isinstance(event, ErrorEvent) else event
-        if event_local:  # ErrorEvent may not have a trigger_event set
-            if not event_local.end_timestamp or event_local.init_timestamp == event_local.end_timestamp:
-                event_local.end_timestamp = get_ISO_time()
-
-            if isinstance(event, ErrorEvent):
-                # Extract trigger_event info from ErrorEvent and log trigger_event
-                event.trigger_event_id = event_local.id
-                event.trigger_event_type = event_local.event_type
-                self._worker.add_event(event_local.__dict__)
-                event.trigger_event = None  # removes trigger_event from serialization
+        if isinstance(event, Event):
+            if not event.end_timestamp or event.init_timestamp == event.end_timestamp:
+                event.end_timestamp = get_ISO_time()
+        elif isinstance(event, ErrorEvent):
+            if event.trigger_event:
+                if not event.trigger_event.end_timestamp or event.trigger_event.init_timestamp == event.trigger_event.end_timestamp:
+                    event.trigger_event.end_timestamp = get_ISO_time()
+
+            event.trigger_event_id = event.trigger_event.id
+            event.trigger_event_type = event.trigger_event.event_type
+            self._worker.add_event(event.trigger_event.__dict__)
+            event.trigger_event = None  # removes trigger_event from serialization
 
         self._worker.add_event(event.__dict__)
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
         func_args = inspect.signature(func).parameters
         arg_names = list(func_args.keys())
@@ -250,16 +251,16 @@
                                 tags or self._tags_for_future_session, host_env=get_host_env(self._env_data_opt_out))
         self._worker = Worker(config or self.config)
         start_session_result = self._worker.start_session(self._session)
         if not start_session_result:
             self._session = None
             return logger.warning("🖇 AgentOps: Cannot start session")
 
-        logger.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
-                    .format(self._session.session_id))
+        logger.info('View info on this session at https://app.agentops.ai/drilldown?session_id=%s', 
+                    self._session.session_id)
 
         return self._session.session_id
 
     def end_session(self,
                     end_state: str,
                     end_state_reason: Optional[str] = None,
                     video: Optional[str] = None):
@@ -272,49 +273,52 @@
                 video (str, optional): The video screen recording of the session
         """
         if self._session is None or self._session.has_ended:
             return logger.warning("🖇 AgentOps: Cannot end session - no current session")
 
         if not any(end_state == state.value for state in EndState):
             return logger.warning("🖇 AgentOps: Invalid end_state. Please use one of the EndState enums")
+        
+        if self._worker is None or self._worker._session is None:
+            return logger.warning("🖇 AgentOps: Cannot end session - no current worker or session")
 
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
         token_cost = self._worker.end_session(self._session)
+        
         if token_cost == 'unknown':
             print('🖇 AgentOps: Could not determine cost of run.')
         else:
             token_cost_d = Decimal(token_cost)
             print('🖇 AgentOps: This run cost ${}'.format('{:.2f}'.format(
                 token_cost_d) if token_cost_d == 0 else '{:.6f}'.format(token_cost_d)))
         self._session = None
         self._worker = None
 
     def create_agent(self, agent_id: str, name: str):
         if self._worker:
             self._worker.create_agent(agent_id, name)
 
     def _handle_unclean_exits(self):
-        def cleanup(end_state: Optional[str] = 'Fail', end_state_reason: Optional[str] = None):
+        def cleanup(end_state: str = 'Fail', end_state_reason: Optional[str] = None):
             # Only run cleanup function if session is created
             if self._session is not None:
                 self.end_session(end_state=end_state,
                                  end_state_reason=end_state_reason)
 
         def signal_handler(signum, frame):
             """
                 Signal handler for SIGINT (Ctrl+C) and SIGTERM. Ends the session and exits the program.
 
                 Args:
                     signum (int): The signal number.
                     frame: The current stack frame.
             """
             signal_name = 'SIGINT' if signum == signal.SIGINT else 'SIGTERM'
-            logger.info(
-                f'🖇 AgentOps: {signal_name} detected. Ending session...')
+            logger.info('🖇 AgentOps: %s detected. Ending session...', signal_name)
             self.end_session(end_state='Fail',
                              end_state_reason=f'Signal {signal_name} detected')
             sys.exit(0)
 
         def handle_exception(exc_type, exc_value, exc_traceback):
             """
                 Handle uncaught exceptions before they result in program termination.
@@ -359,7 +363,10 @@
         """
         if self._worker:
             self._worker.config.parent_key = parent_key
 
     @property
     def parent_key(self):
         return self.config.parent_key
+
+    def stop_instrumenting(self):
+        self.llm_tracker.stop_instrumenting()
```

### Comparing `agentops-0.1.8/agentops/config.py` & `agentops-0.1.9/agentops/config.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/agentops/decorators.py` & `agentops-0.1.9/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/agentops/enums.py` & `agentops-0.1.9/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/agentops/event.py` & `agentops-0.1.9/agentops/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 AgentOps events.
 
 Data Class:
     Event: Represents discrete events to be recorded.
 """
 
 from dataclasses import asdict, dataclass, field
-from typing import List, Optional
+from typing import Any, Dict, List, Optional, Sequence, Union
 from .helpers import get_ISO_time, check_call_stack_for_agent_id
 from .enums import EventType, Models
 from uuid import UUID, uuid4
 import traceback
 
 
 @dataclass
@@ -36,19 +36,18 @@
         return x+1
     }
     """
 
     event_type: str  # EventType.ENUM.value
     params: Optional[dict] = None
     returns: Optional[str] = None
-    init_timestamp: Optional[str] = field(default_factory=get_ISO_time)
-    end_timestamp: str = field(default_factory=get_ISO_time)
+    init_timestamp: str = field(default_factory=get_ISO_time)
+    end_timestamp: Optional[str] = None
     agent_id: Optional[UUID] = field(default_factory=check_call_stack_for_agent_id)
     id: UUID = field(default_factory=uuid4)
-    # TODO: has_been_recorded: bool = False
 
 
 @dataclass
 class ActionEvent(Event):
     """
     For generic events
 
@@ -56,22 +55,17 @@
     logs(str, optional): For detailed information/logging related to the action
     screenshot(str, optional): url to snapshot if agent interacts with UI
     """
 
     event_type: str = EventType.ACTION.value
     # TODO: Should not be optional, but non-default argument 'agent_id' follows default argument error
     action_type: Optional[str] = None
-    logs: Optional[str] = None
+    logs: Optional[Union[str, Sequence[Any]]] = None
     screenshot: Optional[str] = None
 
-    # May be needed if we keep Optional for agent_id
-    # def __post_init__(self):
-    #     if self.agent_id is None:
-    #         raise ValueError("agent_id is required for ActionEvent")
-
 
 @dataclass
 class LLMEvent(Event):
 
     """
     For recording calls to LLMs. AgentOps auto-instruments calls to the most popular LLMs e.g. GPT, Claude, Gemini, etc.
 
@@ -82,33 +76,33 @@
     completion_tokens(int, optional): The number of tokens in the completion message.
     model(Models, str, optional): LLM model e.g. "gpt-4". Models defined in enums.Models are more fully supported by AgentOps e.g. extra features in dashboard.
 
     """
 
     event_type: str = EventType.LLM.value
     thread_id: Optional[UUID] = None
-    prompt: str | List = None
+    prompt: Optional[Union[str, List]] = None
     prompt_tokens: Optional[int] = None
-    completion: str | object = None
+    completion: Union[str, object] = None
     completion_tokens: Optional[int] = None
-    model: Optional[Models | str] = None
+    model: Optional[Union[Models, str]] = None
 
 
 @dataclass
 class ToolEvent(Event):
     """
     For recording calls to tools e.g. searchWeb, fetchFromDB
 
     name(str, optional): A name describing the tool or the actual function name if applicable e.g. searchWeb, fetchFromDB.
     logs(str, dict, optional): For detailed information/logging related to the tool.
 
     """
     event_type: str = EventType.TOOL.value
     name: Optional[str] = None
-    logs: Optional[str | dict] = None
+    logs: Optional[Union[str, dict]] = None
 
 # Does not inherit from Event because error will (optionally) be linked to an ActionEvent, LLMEvent, etc that will have the details
 
 
 @dataclass
 class ErrorEvent():
 
@@ -125,15 +119,15 @@
 
     """
 
     trigger_event: Optional[Event] = None
     exception: Optional[BaseException] = None
     error_type: Optional[str] = None
     code: Optional[str] = None
-    details: Optional[str] = None
+    details: Optional[Union[str, Dict[str, str]]] = None
     logs: Optional[str] = field(default_factory=traceback.format_exc)
     timestamp: str = field(default_factory=get_ISO_time)
 
     def __post_init__(self):
         self.event_type = EventType.ERROR.value
         if self.exception:
             self.error_type = self.error_type or type(self.exception).__name__
```

### Comparing `agentops-0.1.8/agentops/helpers.py` & `agentops-0.1.9/agentops/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from pprint import pprint, pformat
+from pprint import pformat
 from functools import wraps
 import time
 from datetime import datetime
 import json
 import inspect
+from typing import Union
+
 from .log_config import logger
 from uuid import UUID
 import os
 from importlib.metadata import version
 
 
 def singleton(class_):
@@ -72,34 +74,34 @@
         else:
             return value
 
     cleaned_obj = remove_none_values(obj)
     return json.dumps(cleaned_obj, default=default)
 
 
-def check_call_stack_for_agent_id() -> str | None:
+def check_call_stack_for_agent_id() -> Union[UUID, None]:
     for frame_info in inspect.stack():
         # Look through the call stack for the class that called the LLM
         local_vars = frame_info.frame.f_locals
         for var in local_vars.values():
             # We stop looking up the stack at main because after that we see global variables
             if var == "__main__":
-                return
+                return None
             if hasattr(var, 'agent_ops_agent_id') and getattr(var, 'agent_ops_agent_id'):
-                logger.debug('LLM call from agent named: ' + getattr(var, 'agent_ops_agent_name'))
+                logger.debug('LLM call from agent named: %s', getattr(var, 'agent_ops_agent_name'))
                 return getattr(var, 'agent_ops_agent_id')
     return None
 
 
 def get_agentops_version():
     try:
         pkg_version = version("agentops")
         return pkg_version
     except Exception as e:
-        logger.warning(f"Error reading package version: {e}")
+        logger.warning('Error reading package version: %s', e)
         return None
 
 
 # Function decorator that prints function name and its arguments to the console for debug purposes
 # Example output:
     # <AGENTOPS_DEBUG_OUTPUT>
     # on_llm_start called with arguments:
```

### Comparing `agentops-0.1.8/agentops/host_env.py` & `agentops-0.1.9/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/agentops/http_client.py` & `agentops-0.1.9/agentops/http_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 
 
 class Response:
 
     def __init__(self, status: HttpStatus = HttpStatus.UNKNOWN, body: Optional[dict] = None):
         self.status: HttpStatus = status
         self.code: int = status.value
-        self.body = body
-        if not self.body:
-            self.body = {}
+        self.body = body if body else {}
 
     def parse(self, res: requests.models.Response):
         res_body = res.json()
         self.code = res.status_code
         self.status = self.get_status(self.code)
         self.body = res_body
         return self
@@ -83,25 +81,25 @@
             result.code = 408
             result.status = HttpStatus.TIMEOUT
             logger.warning(
                 '🖇 AgentOps: Could not post data - connection timed out')
         except requests.exceptions.HTTPError as e:
             try:
                 result.parse(e.response)
-            except:
+            except Exception:
                 result = Response()
                 result.code = e.response.status_code
                 result.status = Response.get_status(e.response.status_code)
                 result.body = {'error': str(e)}
         except requests.exceptions.RequestException as e:
             result.body = {'error': str(e)}
 
         if result.code == 401:
-            logger.warning(
-                f'🖇 AgentOps: Could not post data - API server rejected your API key: {api_key}')
+            logger.warning('🖇 AgentOps: Could not post data - API server rejected your API key: %s',
+                           api_key)
         if result.code == 400:
-            logger.warning(f'🖇 AgentOps: Could not post data - {result.body}')
+            logger.warning('🖇 AgentOps: Could not post data - %s', result.body)
         if result.code == 500:
             logger.warning(
-                f'🖇 AgentOps: Could not post data - internal server error')
+                '🖇 AgentOps: Could not post data - internal server error')
 
         return result
```

### Comparing `agentops-0.1.8/agentops/langchain_callback_handler.py` & `agentops-0.1.9/agentops/langchain_callback_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,29 @@
 from agentops import Client as AOClient
 from agentops import ActionEvent, LLMEvent, ToolEvent, ErrorEvent
 from agentops.helpers import get_ISO_time
 
 from .helpers import debug_print_function_params
 
 
+def get_model_from_kwargs(kwargs: any) -> str:
+    if 'model' in kwargs['invocation_params']:
+        return kwargs['invocation_params']['model']
+    elif '_type' in kwargs['invocation_params']:
+        return kwargs['invocation_params']['_type']
+    else:
+        return 'unknown_model'
+
+
+# def get_completion_from_response(response: LLMResult):
+#     if 'text' in response.generations[0][0]:
+#         return response.generations[0][0].text
+#     if ''
+#
+
 class Events:
     llm: Dict[str, LLMEvent] = {}
     tool: Dict[str, ToolEvent] = {}
     chain: Dict[str, ActionEvent] = {}
     retriever: Dict[str, ActionEvent] = {}
     error: Dict[str, ErrorEvent] = {}
 
@@ -30,15 +45,15 @@
 
     def __init__(self, api_key: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  max_wait_time: Optional[int] = None,
                  max_queue_size: Optional[int] = None,
                  tags: Optional[List[str]] = None):
 
-        client_params = {
+        client_params: Dict[str, Any] = {
             'api_key': api_key,
             'endpoint': endpoint,
             'max_wait_time': max_wait_time,
             'max_queue_size': max_queue_size,
             'tags': tags
         }
 
@@ -59,15 +74,15 @@
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         self.events.llm[str(run_id)] = LLMEvent(
             params={**serialized,
                     **({} if metadata is None else metadata),
                     **kwargs},  # TODO: params is inconsistent, in ToolEvent we put it in logs
-            model=kwargs['invocation_params']['model'],
+            model=get_model_from_kwargs(kwargs),
             prompt=prompts[0]
             # tags=tags # TODO
         )
 
     @debug_print_function_params
     def on_llm_error(
             self,
@@ -90,22 +105,23 @@
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         llm_event.returns = {
-            "content": response.generations[0][0].message.content,
+            "content": response.generations[0][0].text,
             "generations": response.generations
         }
         llm_event.end_timestamp = get_ISO_time()
+        llm_event.completion = response.generations[0][0].text
         if response.llm_output is not None:
-            llm_event.completion = response.generations[0][0].message.content  # TODO
             llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
+
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
             error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)], error_type="NoGenerations", details="on_llm_end: No generations")
             self.ao_client.record(error_event)
 
@@ -327,15 +343,15 @@
 
     def __init__(self, api_key: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  max_wait_time: Optional[int] = None,
                  max_queue_size: Optional[int] = None,
                  tags: Optional[List[str]] = None):
 
-        client_params = {
+        client_params: Dict[str, Any] = {
             'api_key': api_key,
             'endpoint': endpoint,
             'max_wait_time': max_wait_time,
             'max_queue_size': max_queue_size,
             'tags': tags
         }
 
@@ -414,20 +430,20 @@
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         llm_event.returns = {
-            "content": response.generations[0][0].message.content,
+            "content": response.generations[0][0].text,
             "generations": response.generations
         }
         llm_event.end_timestamp = get_ISO_time()
+        llm_event.completion = response.generations[0][0].text
         if response.llm_output is not None:
-            llm_event.completion = response.generations[0][0].message.content  # TODO
             llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
             error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)], error_type="NoGenerations", details="on_llm_end: No generations")
```

### Comparing `agentops-0.1.8/agentops/llm_tracker.py` & `agentops-0.1.9/agentops/llm_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from importlib import import_module
 from importlib.metadata import version
 from packaging.version import Version, parse
 from .log_config import logger
 from .event import LLMEvent, ErrorEvent
 from .helpers import get_ISO_time, check_call_stack_for_agent_id
 import inspect
+from typing import Optional
 import pprint
 
+original_create = None
+original_create_async = None
 
 class LlmTracker:
     SUPPORTED_APIS = {
         'litellm': {'1.3.1': ("openai_chat_completions.completion",)},
         'openai': {
             '1.0.0': (
                 "chat.completions.create",
@@ -23,14 +26,16 @@
                 "ChatCompletion.acreate",
             ),
         }
     }
 
     def __init__(self, client):
         self.client = client
+        self.completion = ""
+        self.llm_event: Optional[LLMEvent] = None
 
     def _handle_response_v0_openai(self, response, kwargs, init_timestamp):
         """Handle responses for OpenAI versions <v1.0.0"""
 
         self.llm_event = LLMEvent(
             init_timestamp=init_timestamp,
             params=kwargs
@@ -223,14 +228,15 @@
 
         return response
 
     def override_openai_v1_completion(self):
         from openai.resources.chat import completions
 
         # Store the original method
+        global original_create
         original_create = completions.Completions.create
 
         def patched_function(*args, **kwargs):
             init_timestamp = get_ISO_time()
             # Call the original function with its original arguments
             result = original_create(*args, **kwargs)
             return self._handle_response_v1_openai(result, kwargs, init_timestamp)
@@ -238,20 +244,21 @@
       # Override the original method with the patched one
         completions.Completions.create = patched_function
 
     def override_openai_v1_async_completion(self):
         from openai.resources.chat import completions
 
         # Store the original method
-        original_create = completions.AsyncCompletions.create
+        global original_create_async
+        original_create_async = completions.AsyncCompletions.create
 
         async def patched_function(*args, **kwargs):
             # Call the original function with its original arguments
             init_timestamp = get_ISO_time()
-            result = await original_create(*args, **kwargs)
+            result = await original_create_async(*args, **kwargs)
             return self._handle_response_v1_openai(result, kwargs, init_timestamp)
 
         # Override the original method with the patched one
         completions.AsyncCompletions.create = patched_function
 
     def override_litellm_completion(self):
         import litellm
@@ -338,7 +345,21 @@
                         if module_version >= parse('1.0.0'):
                             self.override_openai_v1_completion()
                             self.override_openai_v1_async_completion()
                         else:
                             # Patch openai <v1.0.0 methods
                             for method_path in self.SUPPORTED_APIS['openai']['0.0.0']:
                                 self._override_method(api, method_path, module)
+
+    def stop_instrumenting(self):
+        self.undo_override_openai_v1_async_completion()
+        self.undo_override_openai_v1_completion()
+
+    def undo_override_openai_v1_completion(self):
+        global original_create
+        from openai.resources.chat import completions
+        completions.Completions.create = original_create
+
+    def undo_override_openai_v1_async_completion(self):
+        global original_create_async
+        from openai.resources.chat import completions
+        original_create_async = completions.AsyncCompletions.create
```

### Comparing `agentops-0.1.8/agentops/meta_client.py` & `agentops-0.1.9/agentops/meta_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/agentops/session.py` & `agentops-0.1.9/agentops/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,32 +17,32 @@
         end_state (str, optional): The final state of the session. Suggested: "Success", "Fail", "Indeterminate"
         end_state_reason (str, optional): The reason for ending the session.
 
     """
 
     def __init__(self, session_id: UUID, tags: Optional[List[str]] = None, host_env: Optional[dict] = None):
         self.end_timestamp = None
-        self.end_state = None
+        self.end_state: Optional[str] = None
         self.session_id = session_id
         self.init_timestamp = get_ISO_time()
         self.tags = tags
-        self.video = None
-        self.end_state_reason = None
+        self.video: Optional[str] = None
+        self.end_state_reason: Optional[str] = None
         self.host_env = host_env
 
-    def set_session_video(self, video: str):
+    def set_session_video(self, video: str) -> None:
         """
         Sets a url to the video recording of the session.
 
         Args:
             video (str): The url of the video recording
         """
         self.video = video
 
-    def end_session(self, end_state: str = "Indeterminate", end_state_reason: Optional[str] = None):
+    def end_session(self, end_state: str = "Indeterminate", end_state_reason: Optional[str] = None) -> None:
         """
         End the session with a specified state, rating, and reason.
 
         Args:
             end_state (str, optional): The final state of the session. Options: "Success", "Fail", "Indeterminate"
             rating (str, optional): The rating for the session.
             end_state_reason (str, optional): The reason for ending the session. Provides context for why the session ended.
```

### Comparing `agentops-0.1.8/agentops/worker.py` & `agentops-0.1.9/agentops/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 import json
 import threading
 import time
 from .http_client import HttpClient
-from .config import Configuration, ConfigurationError
+from .config import Configuration
 from .session import Session
 from .helpers import safe_serialize, filter_unjsonable
-from typing import Dict
+from typing import Dict, Optional
+import os
 
 
 class Worker:
     def __init__(self, config: Configuration) -> None:
         self.config = config
         self.queue: list[Dict] = []
         self.lock = threading.Lock()
         self.stop_flag = threading.Event()
         self.thread = threading.Thread(target=self.run)
         self.thread.daemon = True
         self.thread.start()
-        self._session: Session | None = None
+        self._session: Optional[Session] = None
+        self._debug_mode = os.getenv('DEBUG_MODE') == 'Y'
 
     def add_event(self, event: dict) -> None:
         with self.lock:
             self.queue.append(event)
             if len(self.queue) >= self.config.max_queue_size:
                 self.flush_queue()
 
     def flush_queue(self) -> None:
         with self.lock:
             if len(self.queue) > 0:
                 events = self.queue
                 self.queue = []
 
                 payload = {
-                    "session_id": self._session.session_id,
+                    "session_id": getattr(self._session, "session_id", None),
                     "events": events
                 }
 
                 serialized_payload = safe_serialize(payload).encode("utf-8")
                 HttpClient.post(f'{self.config.endpoint}/events',
                                 serialized_payload,
                                 self.config.api_key,
                                 self.config.parent_key)
 
-    def start_session(self, session: Session) -> None:
+                if self._debug_mode:
+                    print("\n<AGENTOPS_DEBUG_OUTPUT>")
+                    print(f"Worker request to {self.config.endpoint}/events")
+                    print(serialized_payload)
+                    print("</AGENTOPS_DEBUG_OUTPUT>\n")
+
+    def start_session(self, session: Session) -> bool:
         self._session = session
         with self.lock:
             payload = {
                 "session": session.__dict__
             }
             serialized_payload = json.dumps(filter_unjsonable(payload)).encode("utf-8")
             res = HttpClient.post(f'{self.config.endpoint}/sessions',
@@ -90,15 +98,15 @@
                             self.config.api_key,
                             self.config.parent_key)
 
     def create_agent(self, agent_id, name):
         payload = {
             "id": agent_id,
             "name": name,
-            "session_id": self._session.session_id
+            "session_id": getattr(self._session, "session_id", None),
         }
 
         serialized_payload = \
             safe_serialize(payload).encode("utf-8")
         HttpClient.post(f'{self.config.endpoint}/agents',
                         serialized_payload,
                         self.config.api_key,
```

### Comparing `agentops-0.1.8/agentops.egg-info/PKG-INFO` & `agentops-0.1.9/agentops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: packaging==23.2
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
 
 <div align="center">
   <a href="https://agentops.ai?ref=gh">
-    <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+    <img src="https://github.com/AgentOps-AI/agentops/blob/df22e9dffb7294fb977dc103a2ca3bcf8f04946f/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
   </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.8 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.9 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
 Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
 requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
 langchain>=0.0.354; extra == "langchain"
                                     _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
```

### Comparing `agentops-0.1.8/agentops.egg-info/SOURCES.txt` & `agentops-0.1.9/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/pyproject.toml` & `agentops-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests==2.31.0",
```

### Comparing `agentops-0.1.8/tests/test_canary.py` & `agentops-0.1.9/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/tests/test_events.py` & `agentops-0.1.9/tests/test_events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import time
 import requests_mock
 import pytest
 import agentops
-from agentops import ActionEvent
+from agentops import ActionEvent, ErrorEvent
 
 
-@pytest.fixture
-def mock_req():
-    with requests_mock.Mocker() as m:
-        url = 'https://api.agentops.ai'
-        m.post(url + '/events', text='ok')
-        m.post(url + '/sessions', json={'status': 'success', 'token_cost': 5})
-        yield m
-
 class TestEvents:
     def setup_method(self):
         self.api_key = "random_api_key"
         self.event_type = 'test_event_type'
         self.config = agentops.Configuration(api_key=self.api_key, max_wait_time=50, max_queue_size=1)
 
-    def test_record_timestamp(self, mock_req):
+    def test_record_timestamp(self):
         agentops.init(api_key=self.api_key)
 
         event = ActionEvent()
         time.sleep(0.15)
         agentops.record(event)
 
-        assert event.init_timestamp != event.end_timestamp
+        assert event.init_timestamp != event.end_timestamp
+
+    def test_record_error_event(self):
+        agentops.init(api_key=self.api_key)
+
+        event = ErrorEvent()
+        time.sleep(0.15)
+        agentops.record(event)
+
```

### Comparing `agentops-0.1.8/tests/test_patcher.py` & `agentops-0.1.9/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/tests/test_record_function.py` & `agentops-0.1.9/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/tests/test_session.py` & `agentops-0.1.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.8/tests/test_teardown.py` & `agentops-0.1.9/tests/test_teardown.py`

 * *Files identical despite different names*

