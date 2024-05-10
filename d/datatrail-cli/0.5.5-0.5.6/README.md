# Comparing `tmp/datatrail_cli-0.5.5.tar.gz` & `tmp/datatrail_cli-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.5.5.tar", max compression
+gzip compressed data, was "datatrail_cli-0.5.6.tar", max compression
```

## Comparing `datatrail_cli-0.5.5.tar` & `datatrail_cli-0.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2024-05-02 00:08:23.777665 datatrail_cli-0.5.5/LICENSE
--rw-r--r--   0        0        0     3558 2024-05-02 00:08:23.777665 datatrail_cli-0.5.5/README.md
--rw-r--r--   0        0        0      214 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/__init__.py
--rw-r--r--   0        0        0     4590 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/clear.py
--rw-r--r--   0        0        0     1437 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/cli.py
--rw-r--r--   0        0        0     4037 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/config.py
--rw-r--r--   0        0        0     1062 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/config.yaml
--rw-r--r--   0        0        0     3924 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/ls.py
--rw-r--r--   0        0        0     7990 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/ps.py
--rw-r--r--   0        0        0     4576 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/pull.py
--rw-r--r--   0        0        0    15932 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/src/functions.py
--rw-r--r--   0        0        0     9241 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     3089 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1073 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-09 19:15:11.030850 datatrail_cli-0.5.6/LICENSE
+-rw-r--r--   0        0        0     3558 2024-05-09 19:15:11.030850 datatrail_cli-0.5.6/README.md
+-rw-r--r--   0        0        0      214 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/__init__.py
+-rw-r--r--   0        0        0     4759 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/clear.py
+-rw-r--r--   0        0        0     1437 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/cli.py
+-rw-r--r--   0        0        0     4037 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/config.yaml
+-rw-r--r--   0        0        0     4101 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/ls.py
+-rw-r--r--   0        0        0     8079 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/ps.py
+-rw-r--r--   0        0        0     4706 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/pull.py
+-rw-r--r--   0        0        0    15885 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/src/functions.py
+-rw-r--r--   0        0        0     9241 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     3206 2024-05-09 19:15:11.038850 datatrail_cli-0.5.6/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1073 2024-05-09 19:15:11.042850 datatrail_cli-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.6/PKG-INFO
```

### Comparing `datatrail_cli-0.5.5/LICENSE` & `datatrail_cli-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.5/README.md` & `datatrail_cli-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.5/dtcli/clear.py` & `datatrail_cli-0.5.6/dtcli/clear.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Datatrail Clear Command."""
 
 import logging
 import os
 
 import click
+from requests.exceptions import ConnectionError
 from rich.console import Console
 from rich.prompt import Confirm
 
 from dtcli.config import procure
 from dtcli.src.functions import clear_dataset_path, find_dataset_common_path
 from dtcli.utilities.utilities import set_log_level, validate_scope
 
@@ -87,18 +88,22 @@
     except Exception:
         logger.exception("Configuration missing!! Run `dtcli config init`.")
         raise click.Abort()
 
     if site not in ["local", "canfar"]:
         raise RuntimeError("Clear command not permitted at Chime or Outriggers!")
 
-    if not validate_scope(scope):
-        error_console.print("Scope does not exist!")
-        console.print("Valid scopes are:")
-        ctx.invoke(list)
+    try:
+        if not validate_scope(scope):
+            error_console.print("Scope does not exist!")
+            console.print("Valid scopes are:")
+            ctx.invoke(list)
+            return None
+    except ConnectionError as error:
+        error_console.print(error)
         return None
 
     # Find number of files in common directory and size.
     console.print(f"\nSearching for files for {dataset} {scope}...\n")
     common_path = find_dataset_common_path(scope, dataset, site, verbose, quiet)
     if common_path:
         common_path = (directory + common_path).replace("//", "/")
```

### Comparing `datatrail_cli-0.5.5/dtcli/cli.py` & `datatrail_cli-0.5.6/dtcli/cli.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.5/dtcli/config.py` & `datatrail_cli-0.5.6/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.5/dtcli/config.yaml` & `datatrail_cli-0.5.6/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.5/dtcli/ls.py` & `datatrail_cli-0.5.6/dtcli/ls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Datatrail List Command."""
 
 import json
 import logging
 from typing import Optional
 
 import click
+from requests.exceptions import ConnectionError
 from rich.console import Console
 from rich.table import Table
 
 from dtcli.src import functions
 from dtcli.utilities.utilities import set_log_level, validate_scope
 
 logger = logging.getLogger("ls")
@@ -56,18 +57,22 @@
     set_log_level(logger, verbose, quiet)
     logger.debug("`list` called with:")
     logger.debug(f"scope: {scope} [{type(scope)}]")
     logger.debug(f"datasets: {datasets} [{type(datasets)}]")
     logger.debug(f"verbose: {verbose} [{type(verbose)}]")
     logger.debug(f"quiet: {quiet} [{type(quiet)}]")
     if scope:
-        if not validate_scope(scope):
-            error_console.print("Scope does not exist!")
-            console.print("Valid scopes are:")
-            ctx.invoke(list)
+        try:
+            if not validate_scope(scope):
+                error_console.print("Scope does not exist!")
+                console.print("Valid scopes are:")
+                ctx.invoke(list)
+                return None
+        except ConnectionError as e:
+            error_console.print(e)
             return None
     results = functions.list(scope, datasets, verbose, quiet)
 
     # Display scopes.
     if "scopes" in results.keys():
         table = Table(
             title="Datatrail: Scopes",
```

### Comparing `datatrail_cli-0.5.5/dtcli/ps.py` & `datatrail_cli-0.5.6/dtcli/ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,40 +53,43 @@
     logger.debug("`ps` called with:")
     logger.debug(f"scope: {scope} [{type(scope)}]")
     logger.debug(f"dataset: {dataset} [{type(dataset)}]")
     logger.debug(f"show_files: {show_files} [{type(show_files)}]")
     logger.debug(f"verbose: {verbose} [{type(verbose)}]")
     logger.debug(f"quiet: {quiet} [{type(quiet)}]")
 
-    if not validate_scope(scope):
-        error_console.print("Scope does not exist!")
-        console.print("Valid scopes are:")
-        ctx.invoke(list)
+    try:
+        if not validate_scope(scope):
+            error_console.print("Scope does not exist!")
+            console.print("Valid scopes are:")
+            ctx.invoke(list)
+            return None
+    except Exception as e:
+        error_console.print(e)
         return None
     try:
         files, policies = functions.ps(scope, dataset, verbose, quiet)
     except Exception as e:
         logger.error(e)
         return None
 
-    if files and ("error" in files.keys()):
-        error_console.print(files["error"])
-        return None
-
     if show_files and files:
         # Files table
         file_table = create_files_table(dataset, scope, files)
 
         with console.pager():
             logger.debug("Showing file table.")
             console.print(file_table)
         return None
 
+    if files and ("error" in files.keys()):
+        error_console.print(files["error"])
+
     # Info table
-    if files:
+    elif files:
         if len(files["file_replica_locations"]) < 1:
             unregistered_info = functions.get_unregistered_dataset(dataset, scope)
             if unregistered_info:
                 console.print(
                     f":warning: {dataset} is an unregistered dataset :warning:",
                     style="bold yellow",
                     justify="center",
```

### Comparing `datatrail_cli-0.5.5/dtcli/pull.py` & `datatrail_cli-0.5.6/dtcli/pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Datatrail Pull Command."""
 
 import logging
 from os import cpu_count, path
 
 import click
-from requests.exceptions import SSLError
+from requests.exceptions import ConnectionError, SSLError
 from rich.console import Console
 from rich.prompt import Confirm
 
 from dtcli.config import procure
 from dtcli.src.functions import find_missing_dataset_files, get_files
 from dtcli.utilities.cadcclient import size
 from dtcli.utilities.utilities import set_log_level, validate_scope
@@ -83,18 +83,22 @@
             logger.info(f"No directory, setting to: {directory}.")
     except Exception:
         logger.exception(
             "Configuration Missing!! Run `datatrail config init`.",
         )
         raise click.Abort()
 
-    if not validate_scope(scope):
-        error_console.print("Scope does not exist!")
-        console.print("Valid scopes are:")
-        ctx.invoke(list)
+    try:
+        if not validate_scope(scope):
+            error_console.print("Scope does not exist!")
+            console.print("Valid scopes are:")
+            ctx.invoke(list)
+            return None
+    except ConnectionError as e:
+        error_console.print(e)
         return None
 
     # Find files missing from localhost.
     console.print(f"\nSearching for files for {dataset} {scope}...\n")
     files = find_missing_dataset_files(scope, dataset, directory, verbose)
     if len(files["missing"]) == 0 and len(files["existing"]) == 0:
         console.print("No files found at minoc.", style="bold red")
```

### Comparing `datatrail_cli-0.5.5/dtcli/src/functions.py` & `datatrail_cli-0.5.6/dtcli/src/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,20 +138,20 @@
 
         logger.info(f"Getting policy for {dataset} in {scope}.")
         url: str = str(base_url) + f"/query/dataset/{scope}/{dataset}"
         logger.debug(f"URL: {url}")
         r = requests.get(url)
         logger.debug(f"Status: {r.status_code}.")
         policy_response = utilities.decode_response(r)
-        if "object has no attribute" in policy_response and isinstance(
-            files_response, str
+        if ("object has no attribute" in policy_response) and (
+            "error" in files_response
         ):
-            raise Exception(f"Could not find {dataset} {scope} in Datatrail.")
-        elif isinstance(files_response, str):
-            return None, policy_response
+            raise Exception(files_response["error"])
+        elif "error" in files_response:
+            return None, policy_response  # type: ignore
         return files_response, policy_response  # type: ignore
 
     except requests.exceptions.ConnectionError as e:
         logger.error(e)
         raise ConnectionError("Datatrail Server at CHIME is not responding.")
 
 
@@ -215,16 +215,16 @@
         Dict: Dictionary of results.
     """
     # Set logging level.
     utilities.set_log_level(logger, verbose)
 
     # find dataset
     dataset_locations = get_dataset_file_info(scope, dataset, verbose=verbose)
-    if isinstance(dataset_locations, str):
-        print(f"Could not find the dataset: {scope}, {dataset}")
+    if "error" in dataset_locations:
+        print(dataset_locations["error"])
         return {}
 
     # check for local copy of the data.
     logger.info("Checking for local copies of files.")
     if dataset_locations["file_replica_locations"].get("minoc"):
         file_uris = dataset_locations["file_replica_locations"]["minoc"]
         file_paths = []
```

### Comparing `datatrail_cli-0.5.5/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.5.6/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.5/dtcli/utilities/utilities.py` & `datatrail_cli-0.5.6/dtcli/utilities/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         response (Response): Request response.
 
     Returns:
         Union[Dict, str]: JSON response or text.
     """
     if response.status_code in [200, 201]:
         return response.json()
+    elif response.status_code in [503]:
+        raise requests.exceptions.ConnectionError("Service not responding.")
     else:
         return response.text
 
 
 def split(data: List[Any], count: int) -> List[List[Any]]:
     """Split a list into batches.
```

### Comparing `datatrail_cli-0.5.5/pyproject.toml` & `datatrail_cli-0.5.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.5.5"
+version = "0.5.6"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.5.5/PKG-INFO` & `datatrail_cli-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.5.5
+Version: 0.5.6
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.5 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.6 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: cadcdata (>=2.5.0,<3.0.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

