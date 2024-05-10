# Comparing `tmp/tulona-0.7.5.tar.gz` & `tmp/tulona-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.7.5.tar", last modified: Sat May  4 04:39:33 2024, max compression
+gzip compressed data, was "tulona-0.7.6.tar", last modified: Fri May 10 05:16:28 2024, max compression
```

## Comparing `tulona-0.7.5.tar` & `tulona-0.7.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.949408 tulona-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-04 04:39:27.000000 tulona-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-04 04:39:33.949408 tulona-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-04 04:39:27.000000 tulona-0.7.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.937408 tulona-0.7.5/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.941408 tulona-0.7.5/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.941408 tulona-0.7.5/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.941408 tulona-0.7.5/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-04 04:39:27.000000 tulona-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:39:33.949408 tulona-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.648059 tulona-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-10 05:16:18.000000 tulona-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-10 05:16:28.648059 tulona-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-10 05:16:18.000000 tulona-0.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.640059 tulona-0.7.6/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.640059 tulona-0.7.6/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.648059 tulona-0.7.6/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.648059 tulona-0.7.6/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-10 05:16:18.000000 tulona-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:16:28.648059 tulona-0.7.6/setup.cfg
```

### Comparing `tulona-0.7.5/LICENSE` & `tulona-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/PKG-INFO` & `tulona-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.7.5
+Version: 0.7.6
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.7.5/README.rst` & `tulona-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/adapter/connection.py` & `tulona-0.7.6/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/adapter/mssql.py` & `tulona-0.7.6/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/adapter/mysql.py` & `tulona-0.7.6/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/adapter/postgres.py` & `tulona-0.7.6/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/adapter/snowflake.py` & `tulona-0.7.6/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/cli/base.py` & `tulona-0.7.6/core/tulona/cli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import traceback
+from datetime import datetime
 from pathlib import Path
 
 import click
 
 from tulona.cli import params as p
 from tulona.config.profile import Profile
 from tulona.config.project import Project
@@ -11,20 +12,32 @@
 from tulona.exceptions import TulonaMissingPropertyError
 from tulona.task.compare import CompareColumnTask, CompareRowTask, CompareTask
 from tulona.task.ping import PingTask
 from tulona.task.profile import ProfileTask
 from tulona.task.scan import ScanTask
 from tulona.util.filesystem import get_final_outdir
 
-log = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format="[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s",
+log = logging.getLogger()
+log_formatter = logging.Formatter(
+    "[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s"
 )
 
+consloe_handler = logging.StreamHandler()
+consloe_handler.setFormatter(log_formatter)
+consloe_handler.setLevel(logging.INFO)
+log.addHandler(consloe_handler)
+
+log_dir = Path(Path().absolute(), "log")
+log_dir.mkdir(parents=True, exist_ok=True)
+log_file_fqn = Path(log_dir, f"tulona_{datetime.now().strftime('%Y%m%d%H%M%S')}.log")
+file_handler = logging.FileHandler(log_file_fqn)
+file_handler.setFormatter(log_formatter)
+file_handler.setLevel(logging.DEBUG)
+log.addHandler(file_handler)
+
 
 # command: tulona
 @click.group(
     context_settings={"help_option_names": ["-h", "--help"]},
     no_args_is_help=True,
     epilog="Execute: tulona <command> -h/--help for more help with specific commands",
 )
```

### Comparing `tulona-0.7.5/core/tulona/cli/params.py` & `tulona-0.7.6/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/config/profile.py` & `tulona-0.7.6/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/config/project.py` & `tulona-0.7.6/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/exceptions.py` & `tulona-0.7.6/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/task/base.py` & `tulona-0.7.6/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/task/compare.py` & `tulona-0.7.6/core/tulona/task/compare.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/task/helper.py` & `tulona-0.7.6/core/tulona/task/helper.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/task/ping.py` & `tulona-0.7.6/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/task/profile.py` & `tulona-0.7.6/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/task/scan.py` & `tulona-0.7.6/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/util/database.py` & `tulona-0.7.6/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/util/dataframe.py` & `tulona-0.7.6/core/tulona/util/dataframe.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from typing import List, Tuple, Union
 
 import pandas as pd
 
 from tulona.exceptions import TulonaFundamentalError
 
+log = logging.getLogger(__name__)
+
 
 def apply_column_exclusion(
     df: pd.DataFrame,
     primary_key: Union[List, Tuple, str],
     exclude_columns: list,
     ds_name: str,
 ) -> Union[pd.DataFrame, None]:
@@ -19,13 +22,13 @@
 
     missing_cols = []
     for col in exclude_columns:
         if col not in df.columns.tolist():
             missing_cols.append(col)
 
     if len(missing_cols) > 0:
-        raise ValueError(
-            f"Columns [{missing_cols}] to be excluded are not present in {ds_name}"
-        )
+        log.warning(f"Columns {missing_cols} to be excluded are not present in {ds_name}")
+        exclude_columns = list(set(exclude_columns) - set(missing_cols))
 
-    df = df.drop(columns=exclude_columns)
+    if len(exclude_columns):
+        df = df.drop(columns=exclude_columns)
     return df
```

### Comparing `tulona-0.7.5/core/tulona/util/excel.py` & `tulona-0.7.6/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/util/filesystem.py` & `tulona-0.7.6/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/util/profiles.py` & `tulona-0.7.6/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona/util/sql.py` & `tulona-0.7.6/core/tulona/util/sql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/core/tulona.egg-info/PKG-INFO` & `tulona-0.7.6/core/tulona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.7.5
+Version: 0.7.6
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.7.5/core/tulona.egg-info/SOURCES.txt` & `tulona-0.7.6/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.7.5/pyproject.toml` & `tulona-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.7.5"
+version = "0.7.6"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -111,15 +111,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.7.5"
+current_version = "0.7.6"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

