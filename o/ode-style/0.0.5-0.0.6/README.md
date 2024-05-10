# Comparing `tmp/ode_style-0.0.5.tar.gz` & `tmp/ode_style-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ode_style-0.0.5.tar", last modified: Thu May  9 11:17:28 2024, max compression
+gzip compressed data, was "ode_style-0.0.6.tar", last modified: Thu May  9 18:00:09 2024, max compression
```

## Comparing `ode_style-0.0.5.tar` & `ode_style-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:28.099196 ode_style-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 11:17:28.099196 ode_style-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:24.000000 ode_style-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:28.099196 ode_style-0.0.5/ode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/callback_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/chained_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/composite_job_disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/dispatcher_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/error_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/guard_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/internet_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/sequence_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/value_out_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:28.099196 ode_style-0.0.5/ode_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:17:28.099196 ode_style-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 11:17:24.000000 ode_style-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:09.794512 ode_style-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 18:00:09.794512 ode_style-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:05.000000 ode_style-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:09.794512 ode_style-0.0.6/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/authentication_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/callback_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/chained_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/composite_job_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/dispatcher_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/error_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/guard_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/internet_connection_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/sequence_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/use_case_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/use_case_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/value_out_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:09.794512 ode_style-0.0.6/ode_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:00:09.794512 ode_style-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 18:00:05.000000 ode_style-0.0.6/setup.py
```

### Comparing `ode_style-0.0.5/ode/base_controller.py` & `ode_style-0.0.6/ode/base_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Callable, Optional, TypeVar
 
+from ode.dispatcher_decorator import UseCaseDispatcher
 from ode.use_case import UseCase
 from ode.callback_decorator import CallbackDecorator
 
 from ode.composite_job_disposable import CompositeJobDisposable
 from ode.output import Output
-from ode.use_case_dispatcher import UseCaseDispatcher
+
 from ode.use_case_unit import UseCaseUnit
 
 P = TypeVar('P', bound=object)
 R = TypeVar('R', bound=object)
 
 class BaseController(object):
     composite_job_disposable: Optional[CompositeJobDisposable] = None
```

### Comparing `ode_style-0.0.5/ode/callback_decorator.py` & `ode_style-0.0.6/ode/callback_decorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 from ode.use_case_decorator import UseCaseDecorator
 from typing import Callable, TypeVar
 
 P = TypeVar('P')
 R = TypeVar('R')
 
 class CallbackDecorator(UseCaseDecorator[P, R]):
+    
     def __init__(self, use_case: UseCase[P, R], callback: Callable[[Output[R]], None]):
         super().__init__(use_case)
         self.callback = callback
 
     def on_result(self, output: Output[R]):
-        super().on_result(output)
         self.callback(output)
 
     def on_error(self, error: Exception):
-        super().on_error(error)
         self.callback(ErrorOutput(error))
```

### Comparing `ode_style-0.0.5/ode/chained_use_case.py` & `ode_style-0.0.6/ode/chained_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.5/ode/composite_job_disposable.py` & `ode_style-0.0.6/ode/composite_job_disposable.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.5/ode/dispatcher_decorator.py` & `ode_style-0.0.6/ode/dispatcher_decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from abc import abstractmethod
-from typing import TypeVar, Optional
-from ode.use_case import UseCase
-from ode.output import Output
+from typing import TypeVar
 from ode.use_case_decorator import UseCaseDecorator
-import asyncio
+import threading
 
 P = TypeVar('P')
 R = TypeVar('R')
 
-class DispatcherDecorator(UseCaseDecorator[P, R]):
-    def __init__(
-        self,
-        use_case: UseCase[P, R],
-        execute_on: asyncio.AbstractEventLoop = None,
-        result_on: asyncio.AbstractEventLoop = None
-    ):
+class UseCaseDispatcher:
+    def __init__(self, use_case, execute_on=None, result_on=None):
+        self.decorator = DispatcherDecorator(use_case, execute_on, result_on)
+
+    def dispatch(self, param=None):
+        return self.decorator.dispatch(param)
+
+class DispatcherDecorator(UseCaseDecorator):
+    def __init__(self, use_case, execute_on=None, result_on=None):
         super().__init__(use_case)
         self.execute_on = execute_on
         self.result_on = result_on
 
-    def dispatch(self, param: Optional[P] = None):
-        return asyncio.create_task(self.process(param), loop=self.execute_on)
+    def dispatch(self, param=None):
+        return threading.Thread(target=self.process, args=(param,)).start()
 
-    def on_error(self, error: Exception):
-        asyncio.to_thread(self.use_case.on_error, error, loop=self.result_on)
+    def on_error(self, error):
+        threading.Thread(target=lambda: self.use_case.on_error(error)).start()
 
-    def on_result(self, output: Output[R]):
-        asyncio.to_thread(self.use_case.on_result, output, loop=self.result_on)
+    def on_result(self, output):
+        threading.Thread(target=lambda: self.use_case.on_result(output)).start()
```

### Comparing `ode_style-0.0.5/ode/sequence_use_case.py` & `ode_style-0.0.6/ode/sequence_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.5/ode/use_case_decorator.py` & `ode_style-0.0.6/ode/use_case_decorator.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.5/ode/use_case_dispatcher.py` & `ode_style-0.0.6/ode/use_case_unit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-from abc import abstractmethod
-from typing import TypeVar, Optional
-from ode.dispatcher_decorator import DispatcherDecorator
+from typing import TypeVar, Generic, Optional
+from ode.callback_decorator import CallbackDecorator
+from ode.output import Output
+from ode.value_out_put import ValueOutput
+
 from ode.use_case import UseCase
-import asyncio
 
 P = TypeVar('P')
 R = TypeVar('R')
 
-class UseCaseDispatcher:
-    def __init__(
-        self,
-        use_case: UseCase[P, R],
-        execute_on: asyncio.AbstractEventLoop = None,
-        result_on: asyncio.AbstractEventLoop = None
-    ):
-        self.decorator = DispatcherDecorator(use_case, execute_on, result_on)
+class UseCaseUnit(Generic[P, R]):
+    def __init__(self, use_case: UseCase[P, R], param: Optional[P] = None):
+        self.use_case = use_case
+        self.param = param
+
+    def process(self) -> Output[R]:
+        callback = self.Callback()
+        decorator = CallbackDecorator(self.use_case, callback.set)
+        decorator.process(self.param)
+        return callback.output
+
+    class Callback:
+        def __init__(self):
+            self.output = ValueOutput()
 
-    def dispatch(self, param: Optional[P] = None):
-        return self.decorator.dispatch(param)
+        def set(self, value: Output[R]):
+            self.output = value
```

### Comparing `ode_style-0.0.5/ode_style.egg-info/SOURCES.txt` & `ode_style-0.0.6/ode_style.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,13 @@
 ode/guard_exception.py
 ode/http_exception.py
 ode/internet_connection_exception.py
 ode/output.py
 ode/sequence_use_case.py
 ode/use_case.py
 ode/use_case_decorator.py
-ode/use_case_dispatcher.py
 ode/use_case_unit.py
 ode/value_out_put.py
 ode_style.egg-info/PKG-INFO
 ode_style.egg-info/SOURCES.txt
 ode_style.egg-info/dependency_links.txt
 ode_style.egg-info/top_level.txt
```

