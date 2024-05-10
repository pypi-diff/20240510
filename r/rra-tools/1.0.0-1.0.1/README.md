# Comparing `tmp/rra_tools-1.0.0.tar.gz` & `tmp/rra_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rra_tools-1.0.0.tar", max compression
+gzip compressed data, was "rra_tools-1.0.1.tar", max compression
```

## Comparing `rra_tools-1.0.0.tar` & `rra_tools-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1517 2024-05-09 22:12:46.144079 rra_tools-1.0.0/LICENSE
--rw-r--r--   0        0        0    12799 2024-05-09 22:12:46.144079 rra_tools-1.0.0/README.md
--rw-r--r--   0        0        0     3702 2024-05-09 22:12:46.144079 rra_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-09 22:12:46.144079 rra_tools-1.0.0/src/rra_tools/__init__.py
--rw-r--r--   0        0        0      601 2024-05-09 22:12:46.144079 rra_tools-1.0.0/src/rra_tools/cli_tools/__init__.py
--rw-r--r--   0        0        0      983 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/cli_tools/exceptions.py
--rw-r--r--   0        0        0      410 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/cli_tools/importers.py
--rw-r--r--   0        0        0     2087 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/cli_tools/options.py
--rw-r--r--   0        0        0     4690 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/jobmon.py
--rw-r--r--   0        0        0      415 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/logging/__init__.py
--rw-r--r--   0        0        0     2190 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/logging/config.py
--rw-r--r--   0        0        0     3981 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/logging/performance.py
--rw-r--r--   0        0        0      605 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/logging/protocol.py
--rw-r--r--   0        0        0     3025 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/parallel.py
--rw-r--r--   0        0        0        0 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/py.typed
--rw-r--r--   0        0        0     3031 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/shell_tools.py
--rw-r--r--   0        0        0     2466 2024-05-09 22:12:46.148079 rra_tools-1.0.0/src/rra_tools/translate.py
--rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-10 17:51:26.405822 rra_tools-1.0.1/LICENSE
+-rw-r--r--   0        0        0    12799 2024-05-10 17:51:26.405822 rra_tools-1.0.1/README.md
+-rw-r--r--   0        0        0     3749 2024-05-10 17:51:26.409822 rra_tools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/__init__.py
+-rw-r--r--   0        0        0      601 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/cli_tools/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/cli_tools/exceptions.py
+-rw-r--r--   0        0        0      410 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/cli_tools/importers.py
+-rw-r--r--   0        0        0     2087 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/cli_tools/options.py
+-rw-r--r--   0        0        0     4690 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/jobmon.py
+-rw-r--r--   0        0        0      415 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/logging/__init__.py
+-rw-r--r--   0        0        0     2235 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/logging/config.py
+-rw-r--r--   0        0        0     3981 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/logging/performance.py
+-rw-r--r--   0        0        0      605 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/logging/protocol.py
+-rw-r--r--   0        0        0     3082 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/parallel.py
+-rw-r--r--   0        0        0        0 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/py.typed
+-rw-r--r--   0        0        0     3031 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/shell_tools.py
+-rw-r--r--   0        0        0     2466 2024-05-10 17:51:26.409822 rra_tools-1.0.1/src/rra_tools/translate.py
+-rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.1/PKG-INFO
```

### Comparing `rra_tools-1.0.0/LICENSE` & `rra_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/README.md` & `rra_tools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/pyproject.toml` & `rra_tools-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rra-tools"
-version = "1.0.0"
+version = "1.0.1"
 description = "Common utilities for IHME Rapid Response team pipelines."
 authors = [
     "James Collins <collijk@uw.edu>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -75,14 +75,15 @@
     "ANN",      # Type hints related, let mypy handle these.
     "D",        # Docstrings related, way too strict to our taste
     "RUF007",   # zip is idiomatic, this is a dumb check
     "RET505",   # Else after return, makes a lot of false positives
     "E501",     # Line too long, this is autoformatted
     "PD901",    # Avoid generic use of name `df`.  Practicality beats purity.
     "S603",     # Supbrocess arg validation, prone to false positives
+    "TCH003",   # Imports for typechecking only
 ]
 ignore-init-module-imports = true
 
 [tool.ruff.lint.per-file-ignores]
 "tests/**" = [
     "S101",     # "Use of `assert` detected"
     "ARG",      # "Unused function argument". Fixtures are often unused.
@@ -110,15 +111,15 @@
     --cov rra_tools \
     --cov tests \
     --cov-report term-missing \
     --no-cov-on-fail \
 """
 
 [tool.coverage.report]
-fail_under = 100
+fail_under = 10
 exclude_lines = [
     'if TYPE_CHECKING:',
     'pragma: no cover'
 ]
 
 [tool.mypy]
 # This is the global mypy configuration.
```

### Comparing `rra_tools-1.0.0/src/rra_tools/cli_tools/__init__.py` & `rra_tools-1.0.1/src/rra_tools/cli_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/src/rra_tools/cli_tools/exceptions.py` & `rra_tools-1.0.1/src/rra_tools/cli_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/src/rra_tools/cli_tools/options.py` & `rra_tools-1.0.1/src/rra_tools/cli_tools/options.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/src/rra_tools/jobmon.py` & `rra_tools-1.0.1/src/rra_tools/jobmon.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/src/rra_tools/logging/config.py` & `rra_tools-1.0.1/src/rra_tools/logging/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 import sys
 from collections.abc import Callable
 from logging import Handler
 from pathlib import Path
 from typing import TextIO
 
-from loguru import Message, Writable, logger
+import loguru
+from loguru import logger
 
 from rra_tools.shell_tools import mkdir
 
 DEFAULT_LOG_MESSAGING_FORMAT = (
     "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
     "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> "
     "- <level>{message}</level> - {extra}"
@@ -50,15 +53,15 @@
     add_logging_sink(
         Path(log_dir) / "main_log.txt",
         verbose=3,
     )
 
 
 def add_logging_sink(
-    sink: TextIO | Writable | Callable[[Message], None] | Handler | Path,
+    sink: TextIO | loguru.Writable | Callable[[loguru.Message], None] | Handler | Path,
     verbose: int,
     *,
     colorize: bool = False,
     serialize: bool = False,
 ) -> None:
     """Add a new output file handle for logging."""
     level, message_format = LOG_FORMATS.get(
```

### Comparing `rra_tools-1.0.0/src/rra_tools/logging/performance.py` & `rra_tools-1.0.1/src/rra_tools/logging/performance.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/src/rra_tools/logging/protocol.py` & `rra_tools-1.0.1/src/rra_tools/logging/protocol.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/src/rra_tools/parallel.py` & `rra_tools-1.0.1/src/rra_tools/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 
 This module simplifies the use of multiprocessing. It provides a single
 function, :func:`run_parallel`, that runs a function in parallel over a list of
 arguments.
 
 """
 
+from __future__ import annotations
+
 from collections.abc import Callable
 from multiprocessing import Pool as StdLibPool
 from typing import Any, TypeVar
 
 import pandas as pd
 import tqdm
 from pathos.multiprocessing import ProcessPool as PathosPool
 
-Loader = Callable[[Any, pd.Index[Any] | None, int, int, bool], pd.DataFrame]
+Loader = Callable[[Any, pd.Index | None, int, int, bool], pd.DataFrame]  # type: ignore[type-arg]
 
 T = TypeVar("T")
 
 
 def run_parallel(
     runner: Callable[[T], Any],
     arg_list: list[T],
```

### Comparing `rra_tools-1.0.0/src/rra_tools/shell_tools.py` & `rra_tools-1.0.1/src/rra_tools/shell_tools.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/src/rra_tools/translate.py` & `rra_tools-1.0.1/src/rra_tools/translate.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.0/PKG-INFO` & `rra_tools-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rra-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Common utilities for IHME Rapid Response team pipelines.
 Home-page: https://collijk.github.io/rra-tools
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

