# Comparing `tmp/logfunc-2.4.3.tar.gz` & `tmp/logfunc-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-2.4.3.tar", last modified: Tue Feb 27 23:55:55 2024, max compression
+gzip compressed data, was "logfunc-2.5.0.tar", last modified: Fri May 10 01:42:01 2024, max compression
```

## Comparing `logfunc-2.4.3.tar` & `logfunc-2.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-02-27 23:55:55.553682 logfunc-2.4.3/
--rw-r--r--   0 mym2       (501) staff       (20)     1068 2023-09-03 19:49:58.000000 logfunc-2.4.3/LICENSE
--rw-r--r--   0 mym2       (501) staff       (20)     7500 2024-02-27 23:55:55.553535 logfunc-2.4.3/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)     6544 2024-02-27 23:40:32.000000 logfunc-2.4.3/README.md
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-02-27 23:55:55.552665 logfunc-2.4.3/logfunc/
--rw-r--r--   0 mym2       (501) staff       (20)       23 2024-02-07 17:14:28.000000 logfunc-2.4.3/logfunc/__init__.py
--rw-r--r--   0 mym2       (501) staff       (20)     2923 2024-02-27 23:54:40.000000 logfunc-2.4.3/logfunc/config.py
--rw-r--r--   0 mym2       (501) staff       (20)       21 2024-02-07 05:27:07.000000 logfunc-2.4.3/logfunc/defaults.py
--rw-r--r--   0 mym2       (501) staff       (20)     7431 2024-02-27 23:53:18.000000 logfunc-2.4.3/logfunc/main.py
--rw-r--r--   0 mym2       (501) staff       (20)      673 2024-02-23 01:13:48.000000 logfunc-2.4.3/logfunc/msgs.py
--rw-r--r--   0 mym2       (501) staff       (20)     3083 2024-02-27 23:54:57.000000 logfunc-2.4.3/logfunc/utils.py
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-02-27 23:55:55.553249 logfunc-2.4.3/logfunc.egg-info/
--rw-r--r--   0 mym2       (501) staff       (20)     7500 2024-02-27 23:55:55.000000 logfunc-2.4.3/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)      257 2024-02-27 23:55:55.000000 logfunc-2.4.3/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 mym2       (501) staff       (20)        1 2024-02-27 23:55:55.000000 logfunc-2.4.3/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 mym2       (501) staff       (20)        8 2024-02-27 23:55:55.000000 logfunc-2.4.3/logfunc.egg-info/top_level.txt
--rw-r--r--   0 mym2       (501) staff       (20)       38 2024-02-27 23:55:55.553728 logfunc-2.4.3/setup.cfg
--rw-r--r--   0 mym2       (501) staff       (20)     1237 2024-02-27 23:55:14.000000 logfunc-2.4.3/setup.py
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-10 01:42:01.585718 logfunc-2.5.0/
+-rw-r--r--   0 mym2       (501) staff       (20)     1068 2023-09-03 19:49:58.000000 logfunc-2.5.0/LICENSE
+-rw-r--r--   0 mym2       (501) staff       (20)     7172 2024-05-10 01:42:01.585615 logfunc-2.5.0/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)     6216 2024-05-10 01:36:04.000000 logfunc-2.5.0/README.md
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-10 01:42:01.585004 logfunc-2.5.0/logfunc/
+-rw-r--r--   0 mym2       (501) staff       (20)       23 2024-04-25 21:42:01.000000 logfunc-2.5.0/logfunc/__init__.py
+-rw-r--r--   0 mym2       (501) staff       (20)     2750 2024-05-10 01:36:11.000000 logfunc-2.5.0/logfunc/config.py
+-rw-r--r--   0 mym2       (501) staff       (20)       21 2024-04-27 03:32:02.000000 logfunc-2.5.0/logfunc/defaults.py
+-rw-r--r--   0 mym2       (501) staff       (20)     5800 2024-05-10 01:40:23.000000 logfunc-2.5.0/logfunc/main.py
+-rw-r--r--   0 mym2       (501) staff       (20)      673 2024-02-23 01:13:48.000000 logfunc-2.5.0/logfunc/msgs.py
+-rw-r--r--   0 mym2       (501) staff       (20)     3012 2024-05-10 01:36:21.000000 logfunc-2.5.0/logfunc/utils.py
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-10 01:42:01.585438 logfunc-2.5.0/logfunc.egg-info/
+-rw-r--r--   0 mym2       (501) staff       (20)     7172 2024-05-10 01:42:01.000000 logfunc-2.5.0/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)      257 2024-05-10 01:42:01.000000 logfunc-2.5.0/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        1 2024-05-10 01:42:01.000000 logfunc-2.5.0/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        8 2024-05-10 01:42:01.000000 logfunc-2.5.0/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 mym2       (501) staff       (20)       38 2024-05-10 01:42:01.585752 logfunc-2.5.0/setup.cfg
+-rw-r--r--   0 mym2       (501) staff       (20)     1237 2024-05-10 01:40:24.000000 logfunc-2.5.0/setup.py
```

### Comparing `logfunc-2.4.3/LICENSE` & `logfunc-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-2.4.3/PKG-INFO` & `logfunc-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 2.4.3
+Version: 2.5.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -75,38 +75,34 @@
 - `level`: Set the log level (DEBUG, INFO, WARNING, etc.).
 - `log_args` & `log_return`: Control whether to log arguments and return values.
 - `max_str_len`: Limit the length of logged strings.
 - `log_exec_time`: Option to log the execution time.
 - `single_msg`: Consolidate all log data into a single message.
 - `use_print`: Choose to `print()` log messages instead of using standard logging.
 - `log_stack_info`: Pass `stack_info=$x` to `.log()` but not print
-- `use_logger`: Pass a logger name or logger object to use instead of logging.lo
-- `log_exception`: Log exceptions if they occur before they are raised.
-- `single_exception`: Consolidate all exception log data into a single message (intended to be used with `log_exception`).
+- `use_logger`: Pass a logger name or logger object to use instead of logging.log
 
 **print_all** used to be an env var, now just unset LOGF_LEVEL and set USE_PRINT=True for the same effect.
 
 ### Environment Variable Overrides
 
 Modify the behavior of `@logf()` using environment variables:
 
-| Env Var               | Example Values       |
-| --------------------- | -------------------- |
-| LOGF_LEVEL            | DEBUG, INFO, WARNING |
-| LOGF_MAX_STR_LEN      | 10, 50, 10000000     |
-| LOGF_SINGLE_MSG       | True, False          |
-| LOGF_USE_PRINT        | True, False          |
-| LOGF_STACK_INFO       | True, False          |
-| LOGF_LOG_EXEC_TIME    | True, False          |
-| LOGF_LOG_ARGS         | True, False          |
-| LOGF_LOG_RETURN       | True, False          |
-| LOGF_LOG_EXCEPTION    | True, False          |
-| LOGF_USE_LOGGER       | 'logger_name'        |
-| LOGF_SINGLE_EXCEPTION | True, False          |
-| LOGF_LOG_LEVEL        | DEBUG, INFO, WARNING |
+| Env Var            | Example Values       |
+| ------------------ | -------------------- |
+| LOGF_LEVEL         | DEBUG, INFO, WARNING |
+| LOGF_MAX_STR_LEN   | 10, 50, 10000000     |
+| LOGF_SINGLE_MSG    | True, False          |
+| LOGF_USE_PRINT     | True, False          |
+| LOGF_STACK_INFO    | True, False          |
+| LOGF_LOG_EXEC_TIME | True, False          |
+| LOGF_LOG_ARGS      | True, False          |
+| LOGF_LOG_RETURN    | True, False          |
+| LOGF_USE_LOGGER    | 'logger_name'        |
+| LOGF_LOG_LEVEL     | DEBUG, INFO, WARNING |
 
 See the following output for an example of how an env var will affect `@logf()` behaviour:
 
 Without `LOGF_USE_PRINT`:
 
 ```
 mym2@Carys-MacBook-Pro liberfy-cli % ./cli user me
```

### Comparing `logfunc-2.4.3/README.md` & `logfunc-2.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,38 +52,34 @@
 - `level`: Set the log level (DEBUG, INFO, WARNING, etc.).
 - `log_args` & `log_return`: Control whether to log arguments and return values.
 - `max_str_len`: Limit the length of logged strings.
 - `log_exec_time`: Option to log the execution time.
 - `single_msg`: Consolidate all log data into a single message.
 - `use_print`: Choose to `print()` log messages instead of using standard logging.
 - `log_stack_info`: Pass `stack_info=$x` to `.log()` but not print
-- `use_logger`: Pass a logger name or logger object to use instead of logging.lo
-- `log_exception`: Log exceptions if they occur before they are raised.
-- `single_exception`: Consolidate all exception log data into a single message (intended to be used with `log_exception`).
+- `use_logger`: Pass a logger name or logger object to use instead of logging.log
 
 **print_all** used to be an env var, now just unset LOGF_LEVEL and set USE_PRINT=True for the same effect.
 
 ### Environment Variable Overrides
 
 Modify the behavior of `@logf()` using environment variables:
 
-| Env Var               | Example Values       |
-| --------------------- | -------------------- |
-| LOGF_LEVEL            | DEBUG, INFO, WARNING |
-| LOGF_MAX_STR_LEN      | 10, 50, 10000000     |
-| LOGF_SINGLE_MSG       | True, False          |
-| LOGF_USE_PRINT        | True, False          |
-| LOGF_STACK_INFO       | True, False          |
-| LOGF_LOG_EXEC_TIME    | True, False          |
-| LOGF_LOG_ARGS         | True, False          |
-| LOGF_LOG_RETURN       | True, False          |
-| LOGF_LOG_EXCEPTION    | True, False          |
-| LOGF_USE_LOGGER       | 'logger_name'        |
-| LOGF_SINGLE_EXCEPTION | True, False          |
-| LOGF_LOG_LEVEL        | DEBUG, INFO, WARNING |
+| Env Var            | Example Values       |
+| ------------------ | -------------------- |
+| LOGF_LEVEL         | DEBUG, INFO, WARNING |
+| LOGF_MAX_STR_LEN   | 10, 50, 10000000     |
+| LOGF_SINGLE_MSG    | True, False          |
+| LOGF_USE_PRINT     | True, False          |
+| LOGF_STACK_INFO    | True, False          |
+| LOGF_LOG_EXEC_TIME | True, False          |
+| LOGF_LOG_ARGS      | True, False          |
+| LOGF_LOG_RETURN    | True, False          |
+| LOGF_USE_LOGGER    | 'logger_name'        |
+| LOGF_LOG_LEVEL     | DEBUG, INFO, WARNING |
 
 See the following output for an example of how an env var will affect `@logf()` behaviour:
 
 Without `LOGF_USE_PRINT`:
 
 ```
 mym2@Carys-MacBook-Pro liberfy-cli % ./cli user me
```

### Comparing `logfunc-2.4.3/logfunc/config.py` & `logfunc-2.5.0/logfunc/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import os
+import random as ran
+import string as s
 from typing import Optional as Opt, Union
 from logging import getLogger
 
+import random as ran
+import string as s
+
+
+ID_CHARS = s.ascii_letters + s.digits + '_-'
+ID_LEN = 6  # 68719476736 possible combinations
 
 EVARS = (
     'LOGF_USE_PRINT',
     'LOGF_SINGLE_MSG',
     'LOGF_MAX_STR_LEN',
     'LOGF_LEVEL',
     'LOGF_LOG_ARGS',
     'LOGF_LOG_RETURN',
     'LOGF_LOG_EXEC_TIME',
     'LOGF_USE_LOGGER',
-    'LOGF_STACK_INFO',
-    'LOGF_LOG_EXCEPTION',
-    'LOGF_SINGLE_EXCEPTION',
     'LOGF_LOG_LEVEL',
+    'LOGF_STACK_INFO',
 )
 
 
 class Cfg:
     def __init__(self, **kwargs):
         self.level = kwargs.get('level')
         self.max_str = kwargs.get('max_str_len')
         self.log_time = kwargs.get('log_exec_time')
         self.single = kwargs.get('single_msg')
-        self.log_ex = kwargs.get('log_exception')
-        self.single_ex = kwargs.get('single_exception')
-        self.log_stack = kwargs.get('log_stack_info')
         self.use_print = kwargs.get('use_print')
         self.log_args = kwargs.get('log_args')
         self.log_return = kwargs.get('log_return')
         self.use_logger = kwargs.get('use_logger')
         self.logf_log_level = kwargs.get('logf_log_level')
+        self.log_stack = kwargs.get('log_stack_info')
 
         # Override attributes based on environment variables
         for ev in EVARS:
             _ev = os.environ.get(ev)
             if _ev is not None:
                 if ev == 'LOGF_MAX_STR_LEN':
                     self.max_str = None if _ev.lower() == 'none' else int(_ev)
@@ -50,33 +54,28 @@
                     self.log_return = _ev.lower() == 'true'
                 elif ev == 'LOGF_LOG_EXEC_TIME':
                     self.log_time = _ev.lower() == 'true'
                 elif ev == 'LOGF_USE_LOGGER':
                     self.use_logger = getLogger(_ev) if _ev else None
                 elif ev == 'LOGF_STACK_INFO':
                     self.log_stack = _ev.lower() == 'true'
-                elif ev == 'LOGF_LOG_EXCEPTION':
-                    self.log_ex = _ev.lower() == 'true'
                 elif ev == 'LOGF_SINGLE_EXCEPTION':
                     self.single_ex = _ev.lower() == 'true'
                 elif ev == 'LOGF_LOG_LEVEL':
                     self.logf_log_level = str(_ev).upper()
 
 
 ARGSSTR = '{func_args} {func_kwargs}'
 ENTER_MSG = '{func_name}() | {args_str}'
 EXIT_MSG_NO_RETURN = '{func_name}() {exec_time}s'
 EXIT_MSG = '{func_name}() {exec_time}s | {result}'
 SINGLE_MSG = '{func_name}() {exec_time}s | {args_str} | {result}'
 ENTER_MSG_NO_ARGS = '{func_name}()'
 
-ERROR_MSG = 'error in {func_name}() {exc_type}: {exc_val}'
-
 
 class MSG_FORMATS:
     argstr = ARGSSTR
     enter = ENTER_MSG
     enter_no_args = ENTER_MSG_NO_ARGS
     exit = EXIT_MSG
     exit_no_return = EXIT_MSG_NO_RETURN
     single = SINGLE_MSG
-    error = ERROR_MSG
```

### Comparing `logfunc-2.4.3/logfunc/main.py` & `logfunc-2.5.0/logfunc/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     log_return: bool = True,
     max_str_len: U[int, None] = TRUNC_STR_LEN,
     log_exec_time: bool = True,
     single_msg: bool = False,
     use_print: bool = False,
     use_logger: Opt[U[Logger, str]] = None,
     log_stack_info: bool = False,
-    log_exception: bool = True,
-    single_exception: bool = True,
     **kwargs
 ) -> U[Call[..., Any], Co[Any, Any, Any]]:
     """A highly customizable function decorator meant for effortless
     leave-and-forget logging of function calls, both synchronous and
     asynchronous. Logs the function name, arguments, return value and
     execution time.
     Args:
@@ -66,28 +64,23 @@
         use_print (bool): Should the log messages be printed instead of logged?
             Default False
         use_logger (Optional[Union[Logger, str]]): logger/logger name
             to use for  Defaults to None. If None, log is used.
         log_stack_info (bool): stack_info kwarg for log
             Can be overridden by the evar LOGF_STACK_INFO.
             Defaults to False
-        log_exception (bool): Should exceptions be logged? Defaults to True.
-        single_exception (bool): Should only the last exception be logged?
-            Defaults to True.
     Returns:
         The executed decorated function or coroutine result.
     """
 
     cfg = Cfg(
         level=level,
         max_str_len=max_str_len,
         log_exec_time=kwargs.get('measure_time', log_exec_time),
         single_msg=single_msg,
-        log_exception=log_exception,
-        single_exception=single_exception,
         log_stack_info=log_stack_info,
         use_print=use_print,
         log_args=log_args,
         log_return=log_return,
         use_logger=use_logger,
     )
 
@@ -103,22 +96,15 @@
         if _insp.iscoroutinefunction(func):
 
             @wraps(func)
             async def decorator(*args, **kwargs) -> Any:
 
                 _start = aio.get_event_loop().time() if cfg.log_time else None
                 argstr = _enter(fname, args, kwargs, cfg)
-                if cfg.log_ex:
-                    try:
-                        result = await func(*args, **kwargs)
-                    except Exception as e:
-                        _handle_ex(e, fname, cfg)
-                        raise e
-                else:
-                    result = await func(*args, **kwargs)
+                result = await func(*args, **kwargs)
 
                 _msg_exit(
                     result,
                     fname,
                     argstr,
                     _endtime(_start, aio.get_event_loop().time()),
                     cfg,
@@ -130,70 +116,39 @@
         else:
 
             @wraps(func)
             def decorator(*args, **kwargs) -> Any:
 
                 _start = time.time() if cfg.log_time else None
                 argstr = _enter(fname, args, kwargs, cfg)
-                if cfg.log_ex:
-                    try:
-
-                        result = func(*args, **kwargs)
-                    except Exception as e:
-                        _handle_ex(e, fname, cfg)
-                        raise e
-
-                else:
-                    result = func(*args, **kwargs)
+                result = func(*args, **kwargs)
 
                 _msg_exit(
                     result, fname, _endtime(_start, time.time()), argstr, cfg
                 )
                 return result
 
         return decorator
 
     return wrapper
 
 
-def _handle_ex(e: Exception, func_name: str, cfg: Cfg) -> None:
-    """Handles logging of exceptions raised in decorated functions."""
-    e._depth = getattr(e, '_depth', 0) + 1
-    log_ex = False
-    if not cfg.single_ex:
-        log_ex = True
-    elif cfg.single_ex and e._depth <= 1:
-        log_ex = True
-    if log_ex:
-        _ex(e, func_name, cfg)
-
-
-def _ex(e: Exception, func_name: str, cfg: Cfg) -> None:
-    """Handles logging of exceptions raised in decorated functions."""
-
-    logmsg = MSG_FORMATS.error.format(
-        func_name=func_name, exc_type=type(e).__name__, exc_val=e
-    )
-    if cfg.use_print:
-        fe = format_exception(e, value=e, tb=e.__traceback__)
-        print(''.join([logmsg] + fe).rstrip('\n'))
-    else:
-        handle_log(logmsg, 'ERROR', cfg.use_logger, False, True)
-
-
 def _msg_enter(func_name: str, args_str: str, cfg: Cfg) -> None:
     """Handles logging of the enter message for decorated functions."""
     if cfg.level is not None and cfg.logf_log_level is not None:
         if loglevel_int(cfg.level) < loglevel_int(cfg.logf_log_level):
             return
     logmsg = MSG_FORMATS.enter.format(func_name=func_name, args_str=args_str)
+
     if cfg.use_print:
         print(logmsg)
     else:
-        handle_log(logmsg, cfg.level, cfg.use_logger, cfg.log_stack)
+        handle_log(
+            logmsg, cfg.level, cfg.use_logger, log_stack_info=cfg.log_stack
+        )
 
 
 def _msg_exit(
     result: Any, func_name: str, end_time: str, args_str: str, cfg: Cfg
 ) -> None:
     """Handles logging of the exit message for decorated functions."""
     if cfg.level is not None and cfg.logf_log_level is not None:
@@ -202,14 +157,15 @@
     logmsg = msgs.exit_msg(
         cfg.single,
         func_name,
         end_time,
         args_str,
         trunc_str(result, cfg.max_str) if cfg.log_return else '',
     )
+
     if cfg.use_print:
         print(logmsg)
     else:
         handle_log(
             logmsg, cfg.level, cfg.use_logger, log_stack_info=cfg.log_stack
         )
```

### Comparing `logfunc-2.4.3/logfunc/msgs.py` & `logfunc-2.5.0/logfunc/msgs.py`

 * *Files identical despite different names*

### Comparing `logfunc-2.4.3/logfunc/utils.py` & `logfunc-2.5.0/logfunc/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 
 
 def handle_log(
     logmsg: str,
     level: Opt[Union[int, str]] = None,
     use_logger: Opt[logging.Logger] = None,
     log_stack_info: bool = False,
-    log_exception: bool = False,
 ) -> Union[Callable, None]:
     """Prints or logs the log message with improved logic for LOGF_USE_PRINT,
     LOGF_LEVEL, and LOGF_PRINT_ALL environment variables.
     Args:
         logmsg (str): The log message to print or log.
         level (Opt[Union[int, str]]): The logging level to use.
             Defaults to logging.INFO.
@@ -95,12 +94,10 @@
             Defaults to False
     Returns:
         Callable: The function used to print/log
     """
     level_int = loglevel_int(level) if level is not None else logging.DEBUG
 
     logfunc = logging.log if use_logger is None else use_logger.log
-    logfunc(
-        level_int, logmsg, stack_info=log_stack_info, exc_info=log_exception
-    )
+    logfunc(level_int, logmsg, stack_info=log_stack_info)
 
     return logfunc
```

### Comparing `logfunc-2.4.3/logfunc.egg-info/PKG-INFO` & `logfunc-2.5.0/logfunc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 2.4.3
+Version: 2.5.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -75,38 +75,34 @@
 - `level`: Set the log level (DEBUG, INFO, WARNING, etc.).
 - `log_args` & `log_return`: Control whether to log arguments and return values.
 - `max_str_len`: Limit the length of logged strings.
 - `log_exec_time`: Option to log the execution time.
 - `single_msg`: Consolidate all log data into a single message.
 - `use_print`: Choose to `print()` log messages instead of using standard logging.
 - `log_stack_info`: Pass `stack_info=$x` to `.log()` but not print
-- `use_logger`: Pass a logger name or logger object to use instead of logging.lo
-- `log_exception`: Log exceptions if they occur before they are raised.
-- `single_exception`: Consolidate all exception log data into a single message (intended to be used with `log_exception`).
+- `use_logger`: Pass a logger name or logger object to use instead of logging.log
 
 **print_all** used to be an env var, now just unset LOGF_LEVEL and set USE_PRINT=True for the same effect.
 
 ### Environment Variable Overrides
 
 Modify the behavior of `@logf()` using environment variables:
 
-| Env Var               | Example Values       |
-| --------------------- | -------------------- |
-| LOGF_LEVEL            | DEBUG, INFO, WARNING |
-| LOGF_MAX_STR_LEN      | 10, 50, 10000000     |
-| LOGF_SINGLE_MSG       | True, False          |
-| LOGF_USE_PRINT        | True, False          |
-| LOGF_STACK_INFO       | True, False          |
-| LOGF_LOG_EXEC_TIME    | True, False          |
-| LOGF_LOG_ARGS         | True, False          |
-| LOGF_LOG_RETURN       | True, False          |
-| LOGF_LOG_EXCEPTION    | True, False          |
-| LOGF_USE_LOGGER       | 'logger_name'        |
-| LOGF_SINGLE_EXCEPTION | True, False          |
-| LOGF_LOG_LEVEL        | DEBUG, INFO, WARNING |
+| Env Var            | Example Values       |
+| ------------------ | -------------------- |
+| LOGF_LEVEL         | DEBUG, INFO, WARNING |
+| LOGF_MAX_STR_LEN   | 10, 50, 10000000     |
+| LOGF_SINGLE_MSG    | True, False          |
+| LOGF_USE_PRINT     | True, False          |
+| LOGF_STACK_INFO    | True, False          |
+| LOGF_LOG_EXEC_TIME | True, False          |
+| LOGF_LOG_ARGS      | True, False          |
+| LOGF_LOG_RETURN    | True, False          |
+| LOGF_USE_LOGGER    | 'logger_name'        |
+| LOGF_LOG_LEVEL     | DEBUG, INFO, WARNING |
 
 See the following output for an example of how an env var will affect `@logf()` behaviour:
 
 Without `LOGF_USE_PRINT`:
 
 ```
 mym2@Carys-MacBook-Pro liberfy-cli % ./cli user me
```

### Comparing `logfunc-2.4.3/setup.py` & `logfunc-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='logfunc',
-    version='2.4.3',
+    version='2.5.0',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description=(
         'An EASY TO USE function decorator for advanced logging of function'
         ' execution, including arguments, return values, and execution time.'
```

