# Comparing `tmp/ode_style-0.0.6.tar.gz` & `tmp/ode_style-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ode_style-0.0.6.tar", last modified: Thu May  9 18:00:09 2024, max compression
+gzip compressed data, was "ode_style-0.0.7.tar", last modified: Fri May 10 16:04:20 2024, max compression
```

## Comparing `ode_style-0.0.6.tar` & `ode_style-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:09.794512 ode_style-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 18:00:09.794512 ode_style-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:05.000000 ode_style-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:09.794512 ode_style-0.0.6/ode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/callback_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/chained_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/composite_job_disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/dispatcher_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/error_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/guard_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/internet_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/sequence_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/use_case_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/use_case_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 18:00:05.000000 ode_style-0.0.6/ode/value_out_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:00:09.794512 ode_style-0.0.6/ode_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 18:00:09.000000 ode_style-0.0.6/ode_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:00:09.794512 ode_style-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 18:00:05.000000 ode_style-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:20.239594 ode_style-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 16:04:20.239594 ode_style-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:14.000000 ode_style-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:20.235593 ode_style-0.0.7/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/authentication_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/callback_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/chained_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/composite_job_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/dispatcher_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/error_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/guard_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/internet_connection_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/sequence_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/use_case_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/use_case_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/value_out_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:20.239594 ode_style-0.0.7/ode_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:04:20.239594 ode_style-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-10 16:04:14.000000 ode_style-0.0.7/setup.py
```

### Comparing `ode_style-0.0.6/ode/base_controller.py` & `ode_style-0.0.7/ode/base_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         
         return job
     
     def process_use_case(self, param: P, use_case: UseCase[P, R]) -> Output[R]:
         callback = UseCaseUnit.Callback()
         CallbackDecorator(use_case, callback.set).process(param)
 
-        return callback.output
+        return callback.output
```

### Comparing `ode_style-0.0.6/ode/chained_use_case.py` & `ode_style-0.0.7/ode/chained_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.6/ode/composite_job_disposable.py` & `ode_style-0.0.7/ode/composite_job_disposable.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,7 +30,43 @@
         for job in self.list:
             try:
                 if job.isActive():
                     job.cancel()
             except:
                 pass
         self.list.clear()
+import sched
+import threading
+import time
+
+class CompositeJobDisposable:
+    def __init__(self):
+        self.scheduler = sched.scheduler(time.time, time.sleep)
+        self.executor = threading.Thread(target=self.scheduler.run)
+        self.list = []
+
+        def purge():
+            self.executor = threading.Thread(target=self.scheduler.run)
+            self.executor.start()
+            if len(self.list) > 0:
+                filtered = [job for job in self.list if job.isCancelled() or job.isCompleted()]
+                for job in filtered:
+                    self.list.remove(job)
+
+        self.scheduler.enter(120, 1, purge, ())
+        self.scheduler.run()
+
+    def add(self, job):
+        if job:
+            self.list.append(job)
+
+    def remove(self, job):
+        self.list.remove(job)
+
+    def cancel(self):
+        for job in self.list:
+            try:
+                if job.isActive():
+                    job.cancel()
+            except:
+                pass
+        self.list.clear()
```

### Comparing `ode_style-0.0.6/ode/dispatcher_decorator.py` & `ode_style-0.0.7/ode/use_case_decorator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 from abc import abstractmethod
-from typing import TypeVar
-from ode.use_case_decorator import UseCaseDecorator
-import threading
+from typing import TypeVar, Optional
+from ode.use_case import UseCase
+from ode.output import Output
 
 P = TypeVar('P')
 R = TypeVar('R')
 
-class UseCaseDispatcher:
-    def __init__(self, use_case, execute_on=None, result_on=None):
-        self.decorator = DispatcherDecorator(use_case, execute_on, result_on)
-
-    def dispatch(self, param=None):
-        return self.decorator.dispatch(param)
-
-class DispatcherDecorator(UseCaseDecorator):
-    def __init__(self, use_case, execute_on=None, result_on=None):
-        super().__init__(use_case)
-        self.execute_on = execute_on
-        self.result_on = result_on
+class UseCaseDecorator(UseCase[P, R]):
+    def __init__(self, use_case: UseCase[P, R]):
+        self.use_case = use_case
 
-    def dispatch(self, param=None):
-        return threading.Thread(target=self.process, args=(param,)).start()
+    def on_error(self, error: Exception):
+        self.use_case.on_error(error)
 
-    def on_error(self, error):
-        threading.Thread(target=lambda: self.use_case.on_error(error)).start()
+    def execute(self, param: Optional[P] = None) -> Output[R]:
+        return self.use_case.execute(param)
 
-    def on_result(self, output):
-        threading.Thread(target=lambda: self.use_case.on_result(output)).start()
+    def on_result(self, output: Output[R]):
+        self.use_case.on_result(output)
+
+    def guard(self, param: Optional[P] = None) -> bool:
+        return self.use_case.guard(param)
```

### Comparing `ode_style-0.0.6/ode/sequence_use_case.py` & `ode_style-0.0.7/ode/sequence_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.6/ode/use_case.py` & `ode_style-0.0.7/ode/use_case.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def execute(self, param: P = None) -> Output[R]:
         pass
     
     def on_error(self, error: Exception):
         self.on_result(output=ErrorOutput(error))
 
     def on_result(self, output: Output[R]):
-        print("UseCase.on_result:", output.value)
+        pass
 
     def guard(self, param: P = None) -> bool:
         return True
 
     def on_guard_error(self):
         pass
```

### Comparing `ode_style-0.0.6/ode/use_case_decorator.py` & `ode_style-0.0.7/ode/use_case_unit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from abc import abstractmethod
-from typing import TypeVar, Optional
-from ode.use_case import UseCase
+from typing import TypeVar, Generic, Optional
+from ode.callback_decorator import CallbackDecorator
 from ode.output import Output
+from ode.value_out_put import ValueOutput
+
+from ode.use_case import UseCase
 
 P = TypeVar('P')
 R = TypeVar('R')
 
-class UseCaseDecorator(UseCase[P, R]):
-    def __init__(self, use_case: UseCase[P, R]):
+class UseCaseUnit(Generic[P, R]):
+    def __init__(self, use_case: UseCase[P, R], param: Optional[P] = None):
         self.use_case = use_case
+        self.param = param
 
-    def on_error(self, error: Exception):
-        self.use_case.on_error(error)
-
-    def execute(self, param: Optional[P] = None) -> Output[R]:
-        return self.use_case.execute(param)
-
-    def on_result(self, output: Output[R]):
-        self.use_case.on_result(output)
+    def process(self) -> Output[R]:
+        callback = self.Callback()
+        decorator = CallbackDecorator(self.use_case, callback.set)
+        decorator.process(self.param)
+        return callback.output
+
+    class Callback:
+        def __init__(self):
+            self.output = ValueOutput()
 
-    def guard(self, param: Optional[P] = None) -> bool:
-        return self.use_case.guard(param)
+        def set(self, value: Output[R]):
+            self.output = value
```

### Comparing `ode_style-0.0.6/ode/use_case_unit.py` & `ode_style-0.0.7/ode/callback_decorator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-from typing import TypeVar, Generic, Optional
-from ode.callback_decorator import CallbackDecorator
-from ode.output import Output
-from ode.value_out_put import ValueOutput
-
+from ode.error_output import ErrorOutput
 from ode.use_case import UseCase
+from ode.output import Output
+from ode.use_case_decorator import UseCaseDecorator
+from typing import Callable, TypeVar
 
 P = TypeVar('P')
 R = TypeVar('R')
 
-class UseCaseUnit(Generic[P, R]):
-    def __init__(self, use_case: UseCase[P, R], param: Optional[P] = None):
-        self.use_case = use_case
-        self.param = param
-
-    def process(self) -> Output[R]:
-        callback = self.Callback()
-        decorator = CallbackDecorator(self.use_case, callback.set)
-        decorator.process(self.param)
-        return callback.output
-
-    class Callback:
-        def __init__(self):
-            self.output = ValueOutput()
-
-        def set(self, value: Output[R]):
-            self.output = value
+class CallbackDecorator(UseCaseDecorator[P, R]):
+    
+    def __init__(self, use_case: UseCase[P, R], callback: Callable[[Output[R]], None]):
+        super().__init__(use_case)
+        self.callback = callback
+
+    def task_done(self, output: Output[R]):
+        if(output.is_success):
+            self.callback(output)
+            return
+        
+        self.callback(ErrorOutput(output.error))
```

### Comparing `ode_style-0.0.6/ode_style.egg-info/SOURCES.txt` & `ode_style-0.0.7/ode_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

