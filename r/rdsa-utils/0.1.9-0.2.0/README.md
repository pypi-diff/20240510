# Comparing `tmp/rdsa-utils-0.1.9.tar.gz` & `tmp/rdsa_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdsa-utils-0.1.9.tar", last modified: Wed Apr  3 11:07:34 2024, max compression
+gzip compressed data, was "rdsa_utils-0.2.0.tar", last modified: Fri May 10 11:25:17 2024, max compression
```

## Comparing `rdsa-utils-0.1.9.tar` & `rdsa_utils-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.160247 rdsa-utils-0.1.9/rdsa_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.160247 rdsa-utils-0.1.9/rdsa_utils/cdsw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/hdfs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/impala.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/cdsw/io/pipeline_runlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/gcp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/gcp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/io/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/gcp/io/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/helpers/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/helpers/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/rdsa_utils/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/methods/averaging_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/rdsa_utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/rdsa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 11:07:34.000000 rdsa-utils-0.1.9/rdsa_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-03 11:07:34.168247 rdsa-utils-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:34.164247 rdsa-utils-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-03 11:07:30.000000 rdsa-utils-0.1.9/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.965220 rdsa_utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-10 11:25:17.965220 rdsa_utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.957219 rdsa_utils-0.2.0/rdsa_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.957219 rdsa_utils-0.2.0/rdsa_utils/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.957219 rdsa_utils-0.2.0/rdsa_utils/cdp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/helpers/hdfs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/helpers/impala.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils/cdp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/cdp/io/pipeline_runlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils/gcp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/gcp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/gcp/helpers/gcp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils/gcp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/gcp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/gcp/io/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/gcp/io/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/helpers/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/helpers/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/methods/averaging_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/rdsa_utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/rdsa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-10 11:25:17.000000 rdsa_utils-0.2.0/rdsa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 11:25:17.000000 rdsa_utils-0.2.0/rdsa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:25:17.000000 rdsa_utils-0.2.0/rdsa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 11:25:17.000000 rdsa_utils-0.2.0/rdsa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 11:25:17.000000 rdsa_utils-0.2.0/rdsa_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-10 11:25:17.965220 rdsa_utils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:25:17.961219 rdsa_utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-10 11:25:11.000000 rdsa_utils-0.2.0/tests/test_validation.py
```

### Comparing `rdsa-utils-0.1.9/LICENSE` & `rdsa_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/hdfs_utils.py` & `rdsa_utils-0.2.0/rdsa_utils/cdp/helpers/hdfs_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/cdsw/helpers/impala.py` & `rdsa_utils-0.2.0/rdsa_utils/cdp/helpers/impala.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/cdsw/io/input.py` & `rdsa_utils-0.2.0/rdsa_utils/cdp/io/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Read inputs on CDSW."""
+"""Read inputs on CDP."""
 import logging
 from typing import Tuple
 
 from pyspark.sql import DataFrame as SparkDF
 from pyspark.sql import SparkSession
 
 from rdsa_utils.exceptions import DataframeEmptyError
```

### Comparing `rdsa-utils-0.1.9/rdsa_utils/cdsw/io/output.py` & `rdsa_utils-0.2.0/rdsa_utils/cdp/io/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Write outputs on CDSW."""
+"""Write outputs on CDP."""
 import logging
 from typing import Union
 
 from pyspark.sql import DataFrame as SparkDF
 from pyspark.sql import SparkSession
 from pyspark.sql import functions as F
 from pyspark.sql.utils import AnalysisException
 
-from rdsa_utils.cdsw.helpers.hdfs_utils import delete_path, file_exists, rename
-from rdsa_utils.cdsw.io.input import load_and_validate_table
+from rdsa_utils.cdp.helpers.hdfs_utils import delete_path, file_exists, rename
+from rdsa_utils.cdp.io.input import load_and_validate_table
 from rdsa_utils.exceptions import (
     ColumnNotInDataframeError,
     DataframeEmptyError,
     TableNotFoundError,
 )
 from rdsa_utils.helpers.pyspark import is_df_empty
```

### Comparing `rdsa-utils-0.1.9/rdsa_utils/cdsw/io/pipeline_runlog.py` & `rdsa_utils-0.2.0/rdsa_utils/cdp/io/pipeline_runlog.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql import functions as F
 from pyspark.sql.utils import AnalysisException
 
-from rdsa_utils.cdsw.helpers.hdfs_utils import create_txt_from_string
+from rdsa_utils.cdp.helpers.hdfs_utils import create_txt_from_string
 
 logger = logging.getLogger(__name__)
 
 
 def _write_entry(entry_df: DataFrame, log_table: str) -> None:
     """Write a DataFrame entry into a specified table.
```

### Comparing `rdsa-utils-0.1.9/rdsa_utils/exceptions.py` & `rdsa_utils-0.2.0/rdsa_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/gcp/helpers/gcp_utils.py` & `rdsa_utils-0.2.0/rdsa_utils/gcp/helpers/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/gcp/io/inputs.py` & `rdsa_utils-0.2.0/rdsa_utils/gcp/io/inputs.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/gcp/io/outputs.py` & `rdsa_utils-0.2.0/rdsa_utils/gcp/io/outputs.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/helpers/pyspark.py` & `rdsa_utils-0.2.0/rdsa_utils/helpers/pyspark.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/helpers/python.py` & `rdsa_utils-0.2.0/rdsa_utils/helpers/python.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/io/config.py` & `rdsa_utils-0.2.0/rdsa_utils/io/config.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/io/input.py` & `rdsa_utils-0.2.0/rdsa_utils/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/logging.py` & `rdsa_utils-0.2.0/rdsa_utils/logging.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/methods/averaging_methods.py` & `rdsa_utils-0.2.0/rdsa_utils/methods/averaging_methods.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/test_utils.py` & `rdsa_utils-0.2.0/rdsa_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/typing.py` & `rdsa_utils-0.2.0/rdsa_utils/typing.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils/validation.py` & `rdsa_utils-0.2.0/rdsa_utils/validation.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/rdsa_utils.egg-info/SOURCES.txt` & `rdsa_utils-0.2.0/rdsa_utils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 rdsa_utils/typing.py
 rdsa_utils/validation.py
 rdsa_utils.egg-info/PKG-INFO
 rdsa_utils.egg-info/SOURCES.txt
 rdsa_utils.egg-info/dependency_links.txt
 rdsa_utils.egg-info/requires.txt
 rdsa_utils.egg-info/top_level.txt
-rdsa_utils/cdsw/__init__.py
-rdsa_utils/cdsw/helpers/__init__.py
-rdsa_utils/cdsw/helpers/hdfs_utils.py
-rdsa_utils/cdsw/helpers/impala.py
-rdsa_utils/cdsw/io/__init__.py
-rdsa_utils/cdsw/io/input.py
-rdsa_utils/cdsw/io/output.py
-rdsa_utils/cdsw/io/pipeline_runlog.py
+rdsa_utils/cdp/__init__.py
+rdsa_utils/cdp/helpers/__init__.py
+rdsa_utils/cdp/helpers/hdfs_utils.py
+rdsa_utils/cdp/helpers/impala.py
+rdsa_utils/cdp/io/__init__.py
+rdsa_utils/cdp/io/input.py
+rdsa_utils/cdp/io/output.py
+rdsa_utils/cdp/io/pipeline_runlog.py
 rdsa_utils/gcp/__init__.py
 rdsa_utils/gcp/helpers/__init__.py
 rdsa_utils/gcp/helpers/gcp_utils.py
 rdsa_utils/gcp/io/__init__.py
 rdsa_utils/gcp/io/inputs.py
 rdsa_utils/gcp/io/outputs.py
 rdsa_utils/helpers/__init__.py
```

### Comparing `rdsa-utils-0.1.9/rdsa_utils.egg-info/requires.txt` & `rdsa_utils-0.2.0/rdsa_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/setup.cfg` & `rdsa_utils-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/tests/test_logging.py` & `rdsa_utils-0.2.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `rdsa-utils-0.1.9/tests/test_validation.py` & `rdsa_utils-0.2.0/tests/test_validation.py`

 * *Files identical despite different names*

