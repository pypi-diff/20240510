# Comparing `tmp/edgegap_scheduling-1.7.0.tar.gz` & `tmp/edgegap_scheduling-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-1.7.0.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.7.1.tar", max compression
```

## Comparing `edgegap_scheduling-1.7.0.tar` & `edgegap_scheduling-1.7.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1993 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/LICENSE
--rw-r--r--   0        0        0     2164 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/README.md
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/BUILD
--rw-r--r--   0        0        0      380 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0     4688 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     5621 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1375 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1468 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      550 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     4351 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/errors/BUILD
--rw-r--r--   0        0        0      133 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-05-07 13:27:48.727497 edgegap_scheduling-1.7.0/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      691 2024-05-07 13:29:49.184527 edgegap_scheduling-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/LICENSE
+-rw-r--r--   0        0        0     2164 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/README.md
+-rw-r--r--   0        0        0      447 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0      124 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_model.py
+-rw-r--r--   0        0        0     4642 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     5724 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1285 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1468 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      550 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     4381 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0      133 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-09 20:08:16.398640 edgegap_scheduling-1.7.1/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      691 2024-05-09 20:08:28.274661 edgegap_scheduling-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.7.1/PKG-INFO
```

### Comparing `edgegap_scheduling-1.7.0/LICENSE` & `edgegap_scheduling-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.0/README.md` & `edgegap_scheduling-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.0/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.7.1/edgegap_scheduling/_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         if isinstance(delay, str):
             self.__task.delay = delay or None
 
         if isinstance(parameters, dict):
             self.__task.parameters = self.__task.parameters.model_copy(update=parameters)
 
-    async def run(self, parameters: BaseModel | type[BaseModel] | None = None):
+    async def run(self, parameters: BaseModel):
         await self.__run(parameters)
 
     def __update_task_start(self):
         self.__task.state = TaskState.RUNNING
         self.__task.started_at = datetime.now(tz=timezone.utc)
         self.__task.sleep_at = None
         self.__task.begin_at = None
@@ -66,29 +66,29 @@
                     await self.__sleep(self.__task.identifier, self.__task.delay_in_seconds)
 
                 if self.__task.need_to_loop:
                     await self.__loop()
                     self.__task.state = TaskState.STOPPED
                     logger.info(f'{self.__task} Stopped')
                 else:
-                    await self.__run()
+                    await self.__run(self.__task.parameters)
                     self.__task.state = TaskState.COMPLETED
                     logger.info(f'{self.__task} Completed')
             except Exception as e:
                 logger.exception(f'{self.__task} raised an exception: {e}')
                 self.__task.state = TaskState.ERROR
                 self.__task.error = str(e)
 
             self.__task.stopped_at = datetime.now(tz=timezone.utc)
 
     async def __loop(self):
         while self.__task.state == TaskState.RUNNING:
             try:
                 self.__task.begin_at = datetime.now(tz=timezone.utc)
-                await self.__run()
+                await self.__run(self.__task.parameters)
             except Exception as e:
                 if self.__task.continue_on_exception:
                     logger.exception(f'{self.__task} raised an exception, continuing since defined by the task: {e}')
                 else:
                     raise e
 
             if self.__task.every_in_seconds is None:
@@ -102,16 +102,16 @@
             elif sleep_duration == 0 and self.__task.remove_running_time:
                 logger.warning(f'{self.__task.name} process for too long and the sleep duration is zero!')
 
             self.__task.sleep_at = datetime.now(tz=timezone.utc)
 
             await self.__sleep(self.__task.identifier, sleep_duration)
 
-    async def __run(self, parameters: BaseModel | type[BaseModel] | None = None):
-        arguments, generators = self.__signature.get_arguments(parameters or self.__task.parameters)
+    async def __run(self, parameters: BaseModel):
+        arguments, generators = self.__signature.get_arguments(parameters)
 
         try:
             for name, generator in generators.items():
                 arguments[name] = (
                     await generator.__anext__() if isinstance(generator, AsyncGeneratorType) else next(generator)
                 )
```

### Comparing `edgegap_scheduling-1.7.0/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.7.1/edgegap_scheduling/_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 
 from edgegap_logging import Color, Format
 from pydantic import BaseModel
 
+from ._model import UndefinedParameters
 from ._runner import TaskRunner
 from ._sleep import AsyncSleep
 from ._task import Task
 from .errors import ManualRunNotAllowedError
 
 
 class Scheduler:
@@ -22,35 +23,37 @@
         every: str = None,
         name: str = None,
         delay: str = None,
         identifier: str = None,
         continue_on_exception: bool = True,
         manual_run_allowed: bool = False,
         remove_running_time: bool = False,
-        parameters: BaseModel | type[BaseModel] | None = None,
+        parameters: BaseModel | type[BaseModel] = UndefinedParameters,
     ):
         def decorator(func):
             _name = name or func.__name__
             task = Task(
                 name=_name,
                 identifier=identifier or _name.lower().replace(' ', '_'),
                 func=func,
                 every=every,
                 delay=delay,
                 continue_on_exception=continue_on_exception,
                 manual_run_allowed=manual_run_allowed,
                 remove_running_time=remove_running_time,
-                parameters=parameters,
+                parameters=parameters if isinstance(parameters, BaseModel) else parameters(),
             )
             runner = TaskRunner(
                 task=task,
                 sleep=self.__async_sleep.sleep,
             )
             self.__register(task.identifier, runner)
 
+            return func
+
         return decorator
 
     def __register(self, identifier: str, runner: TaskRunner) -> None:
         if identifier in self.__runners.keys():
             self.logger.warning(f'Task {Format.squared(identifier, Color.RED)} already exists')
         else:
             self.__runners[identifier] = runner
@@ -159,15 +162,15 @@
         runner = self.__get_or_raise(name)
 
         task = runner.get_task()
 
         if not task.manual_run_allowed:
             raise ManualRunNotAllowedError(f'Task [{name}] is not allowed to be run manually')
 
-        params = task.parameters.model_copy(update=parameters) if isinstance(parameters, dict) else None
+        params = task.parameters.model_copy(update=parameters or {}, deep=True)
 
         await runner.run(params)
 
         return runner.get_task()
 
     async def stop_all(self) -> int:
         self.logger.info('Stopping All Running Tasks')
```

### Comparing `edgegap_scheduling-1.7.0/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.7.1/edgegap_scheduling/_signature.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self, identifier: str, name: str, func: Callable):
         self.__identifier = identifier
         self.__name = name
         self.__func = func
 
     def get_arguments(
         self,
-        parameters: BaseModel | type[BaseModel] | None = None,
+        parameters: BaseModel,
     ) -> tuple[dict[str, Any], dict[str, Any]]:
         specs = {}
         generators = {}
         signature = inspect.signature(self.__func)
 
         for name, param in signature.parameters.items():
             match param.default:
@@ -34,12 +34,10 @@
 
                     continue
 
             match param.annotation:
                 case logging.Logger:
                     specs[name] = logging.getLogger(f'scheduling.{self.__identifier}')
                 case parameters.__class__:
-                    specs[name] = parameters
-                case parameters:
-                    specs[name] = parameters()
+                    specs[name] = parameters.model_copy(deep=True)
 
         return specs, generators
```

### Comparing `edgegap_scheduling-1.7.0/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.7.1/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.0/edgegap_scheduling/_state.py` & `edgegap_scheduling-1.7.1/edgegap_scheduling/_state.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.7.0/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.7.1/edgegap_scheduling/_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime, timezone
 from typing import Callable
 
 from edgegap_logging import Color, Format
 from pydantic import BaseModel, Field, computed_field
 from pytimeparse import parse
 
+from ._model import UndefinedParameters
 from ._state import TaskState
 
 
 class Task(BaseModel):
     identifier: str = Field(default=None, description='The identifier of the Task')
     name: str = Field(..., description='The name of the Task')
     every: str | None = Field(default=None, description='The interval to run the Task')
@@ -20,16 +21,16 @@
     started_at: datetime | None = Field(default=None, description='The start time of the Task')
     begin_at: datetime | None = Field(default=None, description='The last time of the Task began')
     sleep_at: datetime | None = Field(default=None, description='The last time where the Task slept')
     stopped_at: datetime | None = Field(default=None, description='The Time the Task stopped')
     continue_on_exception: bool = Field(default=True, description='If the Task continue after an exception')
     manual_run_allowed: bool = Field(default=False, description='If the Task can be manually run')
     remove_running_time: bool = Field(default=False, description='If the Sleep needs to remove the running time')
-    parameters: BaseModel | type[BaseModel] | None = Field(
-        default=None,
+    parameters: BaseModel = Field(
+        default=UndefinedParameters,
         description='The parameters of the Task to inject on runtime',
     )
 
     def __str__(self):
         return (
             f'Task {Format.squared(self.name, Color.GREEN)} - '
             f'Every {Format.squared(self.every, Color.GREEN)} - '
```

### Comparing `edgegap_scheduling-1.7.0/pyproject.toml` & `edgegap_scheduling-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-scheduling"
-version = "1.7.0"
+version = "1.7.1"
 description = "The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.7.1"
```

### Comparing `edgegap_scheduling-1.7.0/PKG-INFO` & `edgegap_scheduling-1.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 1.7.0
+Version: 1.7.1
 Summary: The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

