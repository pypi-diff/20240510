# Comparing `tmp/ba_tsconcat-0.1.3.tar.gz` & `tmp/ba_tsconcat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ba_tsconcat-0.1.3.tar", max compression
+gzip compressed data, was "ba_tsconcat-0.1.4.tar", max compression
```

## Comparing `ba_tsconcat-0.1.3.tar` & `ba_tsconcat-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    26190 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/LICENSE
--rw-r--r--   0        0        0     2779 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/README.md
--rw-r--r--   0        0        0     1776 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      262 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/__init__.py
--rw-r--r--   0        0        0      608 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/b2t_columns.py
--rw-r--r--   0        0        0     7470 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/cli.py
--rw-r--r--   0        0        0     1565 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/concat.py
--rw-r--r--   0        0        0     2623 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/pretreeprint.py
--rw-r--r--   0        0        0     2962 2024-05-07 14:26:17.088379 ba_tsconcat-0.1.3/src/tsconcat/utils.py
--rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    26190 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2779 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/README.md
+-rw-r--r--   0        0        0     1798 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      262 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/src/tsconcat/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/src/tsconcat/b2t_columns.py
+-rw-r--r--   0        0        0     7574 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/src/tsconcat/cli.py
+-rw-r--r--   0        0        0     1565 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/src/tsconcat/concat.py
+-rw-r--r--   0        0        0     2623 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/src/tsconcat/pretreeprint.py
+-rw-r--r--   0        0        0     2962 2024-05-10 03:37:50.107058 ba_tsconcat-0.1.4/src/tsconcat/utils.py
+-rw-r--r--   0        0        0     3502 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.4/PKG-INFO
```

### Comparing `ba_tsconcat-0.1.3/LICENSE` & `ba_tsconcat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.3/README.md` & `ba_tsconcat-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.3/pyproject.toml` & `ba_tsconcat-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "ba-tsconcat"
-version = "0.1.3"
+version = "0.1.4"
 description = "BIDS App and Python library for concatenating MRI time series."
 authors = ["CMI DAIR Center <florian.rupprecht@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "tsconcat", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nibabel = "^5.2.0"
 numpy = "^1.26.3"
-pandas = ">1.0"
+pandas = "^2.2.0"
 rich = "^13.4.2"
 bids2table = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
+pytest = ">=7.4.3,<9.0.0"
 mypy = "^1.8.0"
 pre-commit = "^3.6.0"
-pytest-cov = "^4.1.0"
-ruff = "^0.1.8"
+pytest-cov = ">=4.1,<6.0"
+ruff = ">=0.1.8,<0.5.0"
 
 [tool.poetry.group.docs.dependencies]
 pdoc = "^14.4.0"
 
 [tool.poetry.scripts]
 ba-tsconcat = "tsconcat.cli:main"
```

### Comparing `ba_tsconcat-0.1.3/src/tsconcat/b2t_columns.py` & `ba_tsconcat-0.1.4/src/tsconcat/b2t_columns.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.3/src/tsconcat/cli.py` & `ba_tsconcat-0.1.4/src/tsconcat/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """CLI for tsconcat."""
 
 import argparse
 import json
+import logging
 import pathlib as pl
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any, List, Optional
 
 import bids2table.table
 import elbow.dtypes  # noqa  makes pandas load json types as dicts from parquet
@@ -18,14 +19,17 @@
 from .utils import (
     build_bidsapp_group_parser,
     file_path_from_b2table_row,
     file_paths_from_b2table,
     sidecar_path_from_b2table_row,
 )
 
+# Set bids2table logger to error
+logging.getLogger("bids2table").setLevel(logging.ERROR)
+
 REDUCE_COLUMNS = [
     B2tColumn.Dataset,
     B2tColumn.Subject,
     B2tColumn.Session,
     B2tColumn.Run,
     B2tColumn.Description,
     B2tColumn.Space,
@@ -83,15 +87,15 @@
 
         if group_callback is not None:
             group_callback(df_group)
 
         return first_row
 
     df_reduced = grouped.apply(func=_func_reduce, include_groups=False)
-    df_reduced = df_reduced.reset_index(drop=False)
+    df_reduced = df_reduced.reset_index(drop=True)
 
     return df_reduced
 
 
 def _read_if_parquet(p: pl.Path, *args, **kwargs) -> Optional[pd.DataFrame]:  # noqa
     try:
         return pd.read_parquet(p, *args, **kwargs)
```

### Comparing `ba_tsconcat-0.1.3/src/tsconcat/concat.py` & `ba_tsconcat-0.1.4/src/tsconcat/concat.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.3/src/tsconcat/pretreeprint.py` & `ba_tsconcat-0.1.4/src/tsconcat/pretreeprint.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.3/src/tsconcat/utils.py` & `ba_tsconcat-0.1.4/src/tsconcat/utils.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.3/PKG-INFO` & `ba_tsconcat-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ba-tsconcat
-Version: 0.1.3
+Version: 0.1.4
 Summary: BIDS App and Python library for concatenating MRI time series.
 License: LGPL-2.1
 Author: CMI DAIR Center
 Author-email: florian.rupprecht@childmind.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bids2table (>=0.1.0,<0.2.0)
 Requires-Dist: nibabel (>=5.2.0,<6.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
-Requires-Dist: pandas (>1.0)
+Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Description-Content-Type: text/markdown
 
 # `tsconcat`
 
 [![Build](https://github.com/childmindresearch/tsconcat/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/childmindresearch/tsconcat/actions/workflows/test.yaml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/childmindresearch/tsconcat/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/childmindresearch/tsconcat)
```

