# Comparing `tmp/geoglows-1.5.0.tar.gz` & `tmp/geoglows-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.5.0.tar", last modified: Thu May  2 23:49:10 2024, max compression
+gzip compressed data, was "geoglows-1.6.0.tar", last modified: Fri May 10 15:06:43 2024, max compression
```

## Comparing `geoglows-1.5.0.tar` & `geoglows-1.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-02 23:49:02.000000 geoglows-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 23:49:02.000000 geoglows-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-02 23:49:10.469408 geoglows-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 23:49:02.000000 geoglows-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_download_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-02 23:49:02.000000 geoglows-1.5.0/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:49:10.469408 geoglows-1.5.0/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 23:49:10.000000 geoglows-1.5.0/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 23:49:02.000000 geoglows-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:49:10.469408 geoglows-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-02 23:49:02.000000 geoglows-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-10 15:06:34.000000 geoglows-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 15:06:34.000000 geoglows-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 15:06:43.936335 geoglows-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 15:06:34.000000 geoglows-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_download_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-10 15:06:34.000000 geoglows-1.6.0/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:06:43.936335 geoglows-1.6.0/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:06:43.000000 geoglows-1.6.0/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 15:06:34.000000 geoglows-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:06:43.936335 geoglows-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-10 15:06:34.000000 geoglows-1.6.0/setup.py
```

### Comparing `geoglows-1.5.0/LICENSE` & `geoglows-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/PKG-INFO` & `geoglows-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.5.0
+Version: 1.6.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.5.0/README.md` & `geoglows-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_download_decorators.py` & `geoglows-1.6.0/geoglows/_download_decorators.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_plots/__init__.py` & `geoglows-1.6.0/geoglows/_plots/__init__.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_plots/format_tools.py` & `geoglows-1.6.0/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.6.0/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.6.0/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_plots/plotly_helpers.py` & `geoglows-1.6.0/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.6.0/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/_plots/plots.py` & `geoglows-1.6.0/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/analyze.py` & `geoglows-1.6.0/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/bias.py` & `geoglows-1.6.0/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/data.py` & `geoglows-1.6.0/geoglows/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import warnings
 
 import pandas as pd
 import xarray as xr
 
-from ._constants import METADATA_TABLE_PATH
+from ._constants import get_metadata_table_path
 from ._download_decorators import _forecast, _retrospective
 
 from .analyze import (
     daily_averages as calc_daily_averages,
     monthly_averages as calc_monthly_averages,
     annual_averages as calc_annual_averages,
 )
@@ -196,28 +196,32 @@
     Returns:
         pd.DataFrame
     """
     pass
 
 
 # model config and supplementary data
-def metadata_tables(columns: list = None) -> pd.DataFrame:
+def metadata_tables(columns: list = None, metadata_table_path: str = None) -> pd.DataFrame:
     """
     Retrieves the master table of rivers metadata and properties as a pandas DataFrame
     Args:
         columns (list): optional subset of columns names to read from the parquet
+        metadata_table_path (str): optional path to a local copy of the metadata table
 
     Returns:
         pd.DataFrame
     """
-    if os.path.exists(METADATA_TABLE_PATH):
-        return pd.read_parquet(METADATA_TABLE_PATH, columns=columns)
+    if metadata_table_path:
+        return pd.read_parquet(metadata_table_path, columns=columns)
+    metadata_table_path = get_metadata_table_path()
+    if os.path.exists(metadata_table_path):
+        return pd.read_parquet(metadata_table_path, columns=columns)
     warn = f"""
-    Local copy of geoglows v2 metadata table not found. You should download a copy for optimal performance and 
-    to make the data available when you are offline. A copy of the table will be cached at {METADATA_TABLE_PATH}.
-    Alternatively, set the environment variable PYGEOGLOWS_METADATA_TABLE_PATH to the path of the table.
+    Local copy of geoglows v2 metadata table not found.
+    A copy of the table has been cached at {metadata_table_path} which you can move as desired.
+    You should set the environment variable PYGEOGLOWS_METADATA_TABLE_PATH or provide the metadata_table_path argument.
     """
     warnings.warn(warn)
-    df = pd.read_parquet('https://geoglows-v2.s3-website-us-west-2.amazonaws.com/tables/package-metadata-table.parquet')
-    os.makedirs(os.path.dirname(METADATA_TABLE_PATH), exist_ok=True)
-    df.to_parquet(METADATA_TABLE_PATH)
+    df = pd.read_parquet('http://geoglows-v2.s3-website-us-west-2.amazonaws.com/tables/package-metadata-table.parquet')
+    os.makedirs(os.path.dirname(metadata_table_path), exist_ok=True)
+    df.to_parquet(metadata_table_path)
     return df[columns] if columns else df
```

### Comparing `geoglows-1.5.0/geoglows/streamflow.py` & `geoglows-1.6.0/geoglows/streamflow.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows/tables.py` & `geoglows-1.6.0/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/geoglows.egg-info/PKG-INFO` & `geoglows-1.6.0/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.5.0
+Version: 1.6.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.5.0/geoglows.egg-info/SOURCES.txt` & `geoglows-1.6.0/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.5.0/setup.py` & `geoglows-1.6.0/setup.py`

 * *Files identical despite different names*

