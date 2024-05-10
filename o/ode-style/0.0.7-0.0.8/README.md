# Comparing `tmp/ode_style-0.0.7.tar.gz` & `tmp/ode_style-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ode_style-0.0.7.tar", last modified: Fri May 10 16:04:20 2024, max compression
+gzip compressed data, was "ode_style-0.0.8.tar", last modified: Fri May 10 17:04:52 2024, max compression
```

## Comparing `ode_style-0.0.7.tar` & `ode_style-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:20.239594 ode_style-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 16:04:20.239594 ode_style-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:14.000000 ode_style-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:20.235593 ode_style-0.0.7/ode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/callback_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/chained_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/composite_job_disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/dispatcher_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/error_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/guard_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/internet_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/sequence_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/use_case_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/use_case_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 16:04:14.000000 ode_style-0.0.7/ode/value_out_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:04:20.239594 ode_style-0.0.7/ode_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 16:04:20.000000 ode_style-0.0.7/ode_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:04:20.239594 ode_style-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-10 16:04:14.000000 ode_style-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:04:52.137508 ode_style-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 17:04:52.137508 ode_style-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:04:48.000000 ode_style-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:04:52.137508 ode_style-0.0.8/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/authentication_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/callback_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/chained_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/composite_job_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/dispatcher_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/error_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/guard_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/internet_connection_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/sequence_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/use_case_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/use_case_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 17:04:48.000000 ode_style-0.0.8/ode/value_out_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:04:52.137508 ode_style-0.0.8/ode_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 17:04:52.000000 ode_style-0.0.8/ode_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 17:04:52.000000 ode_style-0.0.8/ode_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:04:52.000000 ode_style-0.0.8/ode_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 17:04:52.000000 ode_style-0.0.8/ode_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:04:52.137508 ode_style-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-10 17:04:48.000000 ode_style-0.0.8/setup.py
```

### Comparing `ode_style-0.0.7/ode/base_controller.py` & `ode_style-0.0.8/ode/base_controller.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode/callback_decorator.py` & `ode_style-0.0.8/ode/callback_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,9 @@
         self.callback = callback
 
     def task_done(self, output: Output[R]):
         if(output.is_success):
             self.callback(output)
             return
         
-        self.callback(ErrorOutput(output.error))
+        self.callback(ErrorOutput(output.error))
+
```

### Comparing `ode_style-0.0.7/ode/chained_use_case.py` & `ode_style-0.0.8/ode/chained_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode/composite_job_disposable.py` & `ode_style-0.0.8/ode/composite_job_disposable.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode/dispatcher_decorator.py` & `ode_style-0.0.8/ode/dispatcher_decorator.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode/sequence_use_case.py` & `ode_style-0.0.8/ode/sequence_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode/use_case.py` & `ode_style-0.0.8/ode/use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode/use_case_decorator.py` & `ode_style-0.0.8/ode/use_case_decorator.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode/use_case_unit.py` & `ode_style-0.0.8/ode/use_case_unit.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.7/ode_style.egg-info/SOURCES.txt` & `ode_style-0.0.8/ode_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

