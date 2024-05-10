# Comparing `tmp/gdatalog-0.3.3.tar.gz` & `tmp/gdatalog-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdatalog-0.3.3.tar", max compression
+gzip compressed data, was "gdatalog-0.3.4.tar", max compression
```

## Comparing `gdatalog-0.3.3.tar` & `gdatalog-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2022-04-12 16:40:14.248719 gdatalog-0.3.3/LICENSE
--rw-r--r--   0        0        0        0 2022-03-14 14:53:06.573903 gdatalog-0.3.3/gdatalog/__init__.py
--rwxr-xr-x   0        0        0       99 2022-09-15 18:33:51.662671 gdatalog-0.3.3/gdatalog/__main__.py
--rw-r--r--   0        0        0     5574 2024-03-23 13:20:56.849761 gdatalog-0.3.3/gdatalog/cli.py
--rw-r--r--   0        0        0     7357 2024-03-23 15:04:54.736506 gdatalog-0.3.3/gdatalog/delta_terms.py
--rw-r--r--   0        0        0     7387 2024-03-23 15:03:14.192566 gdatalog-0.3.3/gdatalog/program.py
--rw-r--r--   0        0        0     1316 2024-05-10 16:25:13.501431 gdatalog-0.3.3/gdatalog/server.py
--rw-r--r--   0        0        0     1662 2024-03-20 13:41:27.185221 gdatalog-0.3.3/gdatalog/utils.py
--rw-r--r--   0        0        0      527 2024-05-10 16:17:15.970401 gdatalog-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 gdatalog-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-04-12 16:40:14.248719 gdatalog-0.3.4/LICENSE
+-rw-r--r--   0        0        0        0 2022-03-14 14:53:06.573903 gdatalog-0.3.4/gdatalog/__init__.py
+-rwxr-xr-x   0        0        0       99 2022-09-15 18:33:51.662671 gdatalog-0.3.4/gdatalog/__main__.py
+-rw-r--r--   0        0        0     6120 2024-05-10 16:29:31.514830 gdatalog-0.3.4/gdatalog/cli.py
+-rw-r--r--   0        0        0     7357 2024-03-23 15:04:54.736506 gdatalog-0.3.4/gdatalog/delta_terms.py
+-rw-r--r--   0        0        0     7387 2024-03-23 15:03:14.192566 gdatalog-0.3.4/gdatalog/program.py
+-rw-r--r--   0        0        0     1293 2024-05-10 16:27:30.078185 gdatalog-0.3.4/gdatalog/server.py
+-rw-r--r--   0        0        0     1662 2024-03-20 13:41:27.185221 gdatalog-0.3.4/gdatalog/utils.py
+-rw-r--r--   0        0        0      527 2024-05-10 16:29:31.506831 gdatalog-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 gdatalog-0.3.4/PKG-INFO
```

### Comparing `gdatalog-0.3.3/LICENSE` & `gdatalog-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.3/gdatalog/cli.py` & `gdatalog-0.3.4/gdatalog/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 from functools import reduce
 from pathlib import Path
 from typing import List
 
 import typer
+import uvicorn
 from dumbo_utils.console import console
 from dumbo_utils.validation import validate
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import Progress
 from rich.table import Table
 
@@ -38,15 +39,15 @@
         else:
             console.print(f"[red bold]Error:[/red bold] {e}")
 
 
 @app.callback()
 def main(
         filenames: List[Path] = typer.Option(
-            ...,
+            [],
             "--filename",
             "-f",
             help="One or more files to parse",
         ),
         number_of_models: int = typer.Option(
             0,
             "--number-of-models",
@@ -161,7 +162,20 @@
             early_stop = res.repeat(n)
             if early_stop:
                 to_be_done = 0
                 number_of_times = res.number_of_calls
             else:
                 to_be_done -= n
             live.update(stats_table(res))
+
+
+@app.command(name="server")
+def command_server(
+        port: int = typer.Option(8000, "--port", "-p",
+                                 help="An available port to listen for incoming requests"),
+        reload: bool = typer.Option(False, "--reload",
+                                    help="Reload server if source code changes (for development)")
+) -> None:
+    """
+    Run a server for GDatalog (program and other options are provided by JSON requests).
+    """
+    uvicorn.run("gdatalog.server:app", port=port, reload=reload)
```

### Comparing `gdatalog-0.3.3/gdatalog/delta_terms.py` & `gdatalog-0.3.4/gdatalog/delta_terms.py`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.3/gdatalog/program.py` & `gdatalog-0.3.4/gdatalog/program.py`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.3/gdatalog/server.py` & `gdatalog-0.3.4/gdatalog/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         return wrapped
     return wrapper
 
 
 app = FastAPI()
 app.add_middleware(
     CORSMiddleware,
-    allow_origins=["http://localhost:8000"],
+    allow_origins=[],
     allow_credentials=False,
     allow_methods=["POST"],
     allow_headers=["*"],
 )
 
 
 @app.post("/run/")
```

### Comparing `gdatalog-0.3.3/gdatalog/utils.py` & `gdatalog-0.3.4/gdatalog/utils.py`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.3/pyproject.toml` & `gdatalog-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gdatalog"
-version = "0.3.3"
+version = "0.3.4"
 description = "Genereative Datalog with stable negation"
 authors = ["Mario Alviano <mario.alviano@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = "^0.12.3"
 rich = "^13.7.1"
```

### Comparing `gdatalog-0.3.3/PKG-INFO` & `gdatalog-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdatalog
-Version: 0.3.3
+Version: 0.3.4
 Summary: Genereative Datalog with stable negation
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

