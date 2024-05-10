# Comparing `tmp/luxos-0.0.6b22.tar.gz` & `tmp/luxos-0.0.7b23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.6b22.tar", last modified: Sun May  5 23:56:46 2024, max compression
+gzip compressed data, was "luxos-0.0.7b23.tar", last modified: Thu May  9 14:13:23 2024, max compression
```

## Comparing `luxos-0.0.6b22.tar` & `luxos-0.0.7b23.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:46.391699 luxos-0.0.6b22/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-05 23:56:46.391699 luxos-0.0.6b22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-05 23:56:16.000000 luxos-0.0.6b22/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-05 23:56:44.000000 luxos-0.0.6b22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 23:56:46.391699 luxos-0.0.6b22/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:46.383699 luxos-0.0.6b22/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:46.387699 luxos-0.0.6b22/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 23:56:44.000000 luxos-0.0.6b22/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:46.387699 luxos-0.0.6b22/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:46.387699 luxos-0.0.6b22/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-05 23:56:16.000000 luxos-0.0.6b22/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:46.391699 luxos-0.0.6b22/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-05 23:56:46.000000 luxos-0.0.6b22/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 23:56:46.000000 luxos-0.0.6b22/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 23:56:46.000000 luxos-0.0.6b22/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 23:56:46.000000 luxos-0.0.6b22/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 23:56:46.000000 luxos-0.0.6b22/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 23:56:46.000000 luxos-0.0.6b22/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:56:46.391699 luxos-0.0.6b22/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 23:56:16.000000 luxos-0.0.6b22/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-05 23:56:16.000000 luxos-0.0.6b22/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-05 23:56:16.000000 luxos-0.0.6b22/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-05 23:56:16.000000 luxos-0.0.6b22/tests/test_luxos_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-05 23:56:16.000000 luxos-0.0.6b22/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-09 14:13:23.571790 luxos-0.0.7b23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-09 14:12:51.000000 luxos-0.0.7b23/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-09 14:13:21.000000 luxos-0.0.7b23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:13:23.571790 luxos-0.0.7b23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.563790 luxos-0.0.7b23/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.567790 luxos-0.0.7b23/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-09 14:13:21.000000 luxos-0.0.7b23/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.567790 luxos-0.0.7b23/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-09 14:12:51.000000 luxos-0.0.7b23/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 14:13:23.000000 luxos-0.0.7b23/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:13:23.571790 luxos-0.0.7b23/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_luxos_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-09 14:12:51.000000 luxos-0.0.7b23/tests/test_utils.py
```

### Comparing `luxos-0.0.6b22/PKG-INFO` & `luxos-0.0.7b23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.6b22
+Version: 0.0.7b23
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.6b22/README.md` & `luxos-0.0.7b23/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/pyproject.toml` & `luxos-0.0.7b23/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.6b22"
+version = "0.0.7b23"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.6b22/src/luxos/api.json` & `luxos-0.0.7b23/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/src/luxos/api.py` & `luxos-0.0.7b23/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/src/luxos/asyncops.py` & `luxos-0.0.7b23/src/luxos/asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/src/luxos/cli/v1.py` & `luxos-0.0.7b23/src/luxos/cli/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,20 +207,21 @@
 def cli(
     add_arguments: Callable[[argparse.ArgumentParser], None] | None = None,
     process_args: (
         Callable[[argparse.Namespace], argparse.Namespace | None] | None
     ) = None,
 ):
     def _cli1(function):
+        module = inspect.getmodule(function)
+
         @contextlib.contextmanager
         def setup():
             sig = inspect.signature(function)
 
             module_variables = MODULE_VARIABLES.copy()
-            module = inspect.getmodule(function)
             for name in list(module_variables):
                 module_variables[name] = getattr(module, name, None)
 
             if "args" in sig.parameters and "parser" in sig.parameters:
                 raise RuntimeError("cannot use args and parser at the same time")
 
             description, _, epilog = (
@@ -282,10 +283,13 @@
 
             @functools.wraps(function)
             def _cli2(*args, **kwargs):
                 with setup() as ba:
                     log_sys_info()
                     return function(*ba.args, **ba.kwargs)
 
+        _cli2.attributes = {
+            "doc": function.__doc__ or module.__doc__ or "",
+        }
         return _cli2
 
     return _cli1
```

### Comparing `luxos-0.0.6b22/src/luxos/exceptions.py` & `luxos-0.0.7b23/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/src/luxos/misc.py` & `luxos-0.0.7b23/src/luxos/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,26 @@
 # catch-all module (find later a better place)
 from __future__ import annotations
 import sys
 import itertools
 import ipaddress
 from typing import Generator
 
-
 if sys.version_info >= (3, 12):
     batched = itertools.batched
 else:
 
     def batched(iterable, n):
         if n < 1:
             raise ValueError("n must be at least one")
         it = iter(iterable)
         while batch := tuple(itertools.islice(it, n)):
             yield batch
 
 
-def indent(txt: str, pre: str = " " * 2) -> str:
-    """simple text indentation"""
-
-    from textwrap import dedent
-
-    txt = dedent(txt)
-    if txt.endswith("\n"):
-        last_eol = "\n"
-        txt = txt[:-1]
-    else:
-        last_eol = ""
-
-    result = pre + txt.replace("\n", "\n" + pre) + last_eol
-    return result if result.strip() else result.strip()
-
-
 def iter_ip_ranges(txt: str) -> Generator[str, None, None]:
     """iterate over ip ranges
 
     for ip in iter_ip_ranges("127.0.0.1-127.0.0.3:127.0.0.15"):
         print(ip)
 
     127.0.0.1
```

### Comparing `luxos-0.0.6b22/src/luxos/scripts/async_luxos.py` & `luxos-0.0.7b23/src/luxos/scripts/async_luxos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 import asyncio
 import json
 
 from .. import misc
+from .. import text
 from .. import asyncops
 
 
 async def run(
     ipaddresses: list[str],
     port: int,
     cmd: str,
@@ -40,15 +41,15 @@
     failures = [task for task in alltasks if isinstance(task, Exception)]
 
     # print a nice report
     print(f"task executed sucessfully (use -a|--all for details): {len(successes)}")
     if details:
         for (host, port), task in successes:  # type: ignore
             print(f"  > {host}:{port}")
-            print(misc.indent(json.dumps(task, indent=2, sort_keys=True), pre="  | "))
+            print(text.indent(json.dumps(task, indent=2, sort_keys=True), pre="  | "))
     print(f"task executed failures: {len(failures)}")
     for failure in failures:
         print(f"  {failure}")
 
 
 def main(*args, **kwargs) -> None:
     asyncio.run(run(*args, **kwargs))
```

### Comparing `luxos-0.0.6b22/src/luxos/scripts/health_checker.py` & `luxos-0.0.7b23/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/src/luxos/scripts/luxos.py` & `luxos-0.0.7b23/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/src/luxos/utils.py` & `luxos-0.0.7b23/src/luxos/utils.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.7b23/src/luxos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.6b22
+Version: 0.0.7b23
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.6b22/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.7b23/src/luxos.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/luxos/__main__.py
 src/luxos/api.json
 src/luxos/api.py
 src/luxos/asyncops.py
 src/luxos/exceptions.py
 src/luxos/misc.py
 src/luxos/py.typed
+src/luxos/text.py
 src/luxos/utils.py
 src/luxos.egg-info/PKG-INFO
 src/luxos.egg-info/SOURCES.txt
 src/luxos.egg-info/dependency_links.txt
 src/luxos.egg-info/entry_points.txt
 src/luxos.egg-info/requires.txt
 src/luxos.egg-info/top_level.txt
@@ -21,8 +22,9 @@
 src/luxos/scripts/async_luxos.py
 src/luxos/scripts/health_checker.py
 src/luxos/scripts/luxos.py
 tests/test_cli.py
 tests/test_luxos.py
 tests/test_luxos_asyncops.py
 tests/test_luxos_misc.py
+tests/test_text.py
 tests/test_utils.py
```

### Comparing `luxos-0.0.6b22/tests/test_luxos_asyncops.py` & `luxos-0.0.7b23/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.6b22/tests/test_utils.py` & `luxos-0.0.7b23/tests/test_utils.py`

 * *Files identical despite different names*

