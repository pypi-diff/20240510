# Comparing `tmp/fiboa_cli-0.3.9.tar.gz` & `tmp/fiboa_cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa_cli-0.3.9.tar", last modified: Wed May  1 21:44:17 2024, max compression
+gzip compressed data, was "fiboa_cli-0.4.0.tar", last modified: Thu May  9 22:16:02 2024, max compression
```

## Comparing `fiboa_cli-0.3.9.tar` & `fiboa_cli-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/create_geoparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/rename_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/tests/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:16:02.071392 fiboa_cli-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-09 22:16:02.071392 fiboa_cli-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:16:02.067392 fiboa_cli-0.4.0/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/create_geoparquet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:16:02.071392 fiboa_cli-0.4.0/fiboa_cli/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/de_bb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/de_nds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/de_nrw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/de_sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/de_th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/ec_fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/datasets/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/rename_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:16:02.071392 fiboa_cli-0.4.0/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-09 22:16:02.000000 fiboa_cli-0.4.0/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 22:16:02.000000 fiboa_cli-0.4.0/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:16:02.000000 fiboa_cli-0.4.0/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 22:16:02.000000 fiboa_cli-0.4.0/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 22:16:02.000000 fiboa_cli-0.4.0/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 22:16:02.000000 fiboa_cli-0.4.0/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:16:02.071392 fiboa_cli-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:16:02.071392 fiboa_cli-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 22:15:58.000000 fiboa_cli-0.4.0/tests/test_jsonschema.py
```

### Comparing `fiboa_cli-0.3.9/LICENSE` & `fiboa_cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.9/PKG-INFO` & `fiboa_cli-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.9
+Version: 0.4.0
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Requires-Dist: pyarrow>=14.0
 Requires-Dist: fsspec>=2024.0
 Requires-Dist: click>=8.1
 Requires-Dist: geopandas>=0.14
 Requires-Dist: requests>=2.30
 Requires-Dist: aiohttp>=3.9
 Requires-Dist: shapely>=2.0
+Requires-Dist: numpy>=1.20.0
 Provides-Extra: de-nrw
 
 # fiboa CLI
 
 A command-line interface (CLI) for working with fiboa.
 
 - [Getting Started](#getting-started)
@@ -50,24 +51,29 @@
 
 After the installation you should be able to run the following command: `fiboa`
 
 You should see usage instructions and [available commands](#commands) for the CLI.
 
 fiboa CLI supports various commands to work with the files:
 
-- [Inspect fiboa GeoParquet files](#inspect-fiboa-geoparquet-file)
-- [Validation fiboa GeoParquet and GeoJSON files](#validation)
-- [Convert existing non-fiboa datasets to a fiboa GeoParquet file](#converter-for-existing-datasets)
-- File Format Conversion:
-  - [Create a fiboa GeoParquet file from GeoJSON files](#create-fiboa-geoparquet-from-geojson)
-  - [Create fiboa GeoJSON files from a GeoParquet file](#create-fiboa-geojson-from-geoparquet)
-- Extension and Spec development:
-  - [Update an extension template with new names](#update-an-extension-template-with-new-names)
-  - [Validate a fiboa Schema](#validate-a-fiboa-schema)
-  - [Create JSON Schema from fiboa Schema](#create-json-schema-from-fiboa-schema)
+- [fiboa CLI](#fiboa-cli)
+  - [Getting Started](#getting-started)
+    - [Installation](#installation)
+    - [Execute a command](#execute-a-command)
+  - [Commands](#commands)
+    - [Validation](#validation)
+    - [Create fiboa GeoParquet from GeoJSON](#create-fiboa-geoparquet-from-geojson)
+    - [Create fiboa GeoJSON from GeoParquet](#create-fiboa-geojson-from-geoparquet)
+    - [Inspect fiboa GeoParquet file](#inspect-fiboa-geoparquet-file)
+    - [Create JSON Schema from fiboa Schema](#create-json-schema-from-fiboa-schema)
+    - [Validate a fiboa Schema](#validate-a-fiboa-schema)
+    - [Update an extension template with new names](#update-an-extension-template-with-new-names)
+    - [Converter for existing datasets](#converter-for-existing-datasets)
+  - [Development](#development)
+    - [Implement a converter](#implement-a-converter)
 
 ## Commands
 
 ### Validation
 
 To validate a fiboa GeoParquet or GeoJSON file, you can for example run:
 
@@ -144,24 +150,22 @@
 Then the following command could be used:
 - `fiboa rename-extension . -t Timestamps -p ts -s timestamps-extension -o fiboa`
 
 Check `fiboa rename-extension --help` for more details.
 
 ### Converter for existing datasets
 
-To convert an existing dataset to fiboa using the pre-defined converters:
+The CLI ships various converters for existing datasets.
 
-- `fiboa convert de_nrw`
+To get a list of available converters/datasets with title, license, etc. run:
+- `fiboa converters`
+
+Use any of the IDs from the list to convert an existing dataset to fiboa:
 
-Available converters:
-- `at` (Austria)
-- `de_bb` (Berlin/Brandenburh, Germany)
-- `de_nds` (Lowe Saxony, Germany)
-- `de_nrw` (North Rhine-Westphalia, Germany)
-- `de_sh` (Schleswig-Holstein, Germany)
+- `fiboa convert de_nrw`
 
 See [Implement a converter](#implement-a-converter) for details about how to 
 
 ## Development
 
 To install in development mode run `pip install -e .` in this folder.
```

### Comparing `fiboa_cli-0.3.9/README.md` & `fiboa_cli-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -28,24 +28,29 @@
 
 After the installation you should be able to run the following command: `fiboa`
 
 You should see usage instructions and [available commands](#commands) for the CLI.
 
 fiboa CLI supports various commands to work with the files:
 
-- [Inspect fiboa GeoParquet files](#inspect-fiboa-geoparquet-file)
-- [Validation fiboa GeoParquet and GeoJSON files](#validation)
-- [Convert existing non-fiboa datasets to a fiboa GeoParquet file](#converter-for-existing-datasets)
-- File Format Conversion:
-  - [Create a fiboa GeoParquet file from GeoJSON files](#create-fiboa-geoparquet-from-geojson)
-  - [Create fiboa GeoJSON files from a GeoParquet file](#create-fiboa-geojson-from-geoparquet)
-- Extension and Spec development:
-  - [Update an extension template with new names](#update-an-extension-template-with-new-names)
-  - [Validate a fiboa Schema](#validate-a-fiboa-schema)
-  - [Create JSON Schema from fiboa Schema](#create-json-schema-from-fiboa-schema)
+- [fiboa CLI](#fiboa-cli)
+  - [Getting Started](#getting-started)
+    - [Installation](#installation)
+    - [Execute a command](#execute-a-command)
+  - [Commands](#commands)
+    - [Validation](#validation)
+    - [Create fiboa GeoParquet from GeoJSON](#create-fiboa-geoparquet-from-geojson)
+    - [Create fiboa GeoJSON from GeoParquet](#create-fiboa-geojson-from-geoparquet)
+    - [Inspect fiboa GeoParquet file](#inspect-fiboa-geoparquet-file)
+    - [Create JSON Schema from fiboa Schema](#create-json-schema-from-fiboa-schema)
+    - [Validate a fiboa Schema](#validate-a-fiboa-schema)
+    - [Update an extension template with new names](#update-an-extension-template-with-new-names)
+    - [Converter for existing datasets](#converter-for-existing-datasets)
+  - [Development](#development)
+    - [Implement a converter](#implement-a-converter)
 
 ## Commands
 
 ### Validation
 
 To validate a fiboa GeoParquet or GeoJSON file, you can for example run:
 
@@ -122,24 +127,22 @@
 Then the following command could be used:
 - `fiboa rename-extension . -t Timestamps -p ts -s timestamps-extension -o fiboa`
 
 Check `fiboa rename-extension --help` for more details.
 
 ### Converter for existing datasets
 
-To convert an existing dataset to fiboa using the pre-defined converters:
+The CLI ships various converters for existing datasets.
 
-- `fiboa convert de_nrw`
+To get a list of available converters/datasets with title, license, etc. run:
+- `fiboa converters`
+
+Use any of the IDs from the list to convert an existing dataset to fiboa:
 
-Available converters:
-- `at` (Austria)
-- `de_bb` (Berlin/Brandenburh, Germany)
-- `de_nds` (Lowe Saxony, Germany)
-- `de_nrw` (North Rhine-Westphalia, Germany)
-- `de_sh` (Schleswig-Holstein, Germany)
+- `fiboa convert de_nrw`
 
 See [Implement a converter](#implement-a-converter) for details about how to 
 
 ## Development
 
 To install in development mode run `pip install -e .` in this folder.
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/__init__.py` & `fiboa_cli-0.4.0/fiboa_cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import click
-import sys
 import json
+import pandas as pd
 import os
+import sys
+import time
 
-from .convert import convert as convert_
+from .convert import convert as convert_, list_all_converter_ids, list_all_converters
 from .create_geoparquet import create_geoparquet as create_geoparquet_
 from .create_geojson import create_geojson as create_geojson_
 from .describe import describe as describe_
 from .jsonschema import jsonschema as jsonschema_
 from .rename_extension import rename_extension as rename_extension_
 from .validate import validate as validate_
 from .validate_schema import validate_schema as validate_schema_
@@ -92,38 +94,64 @@
 @click.option(
     '--data', '-d',
     is_flag=True,
     type=click.BOOL,
     help='EXPERIMENTAL: Validate the data in the GeoParquet file. Enabling this might be slow or exceed memory. Default is False.',
     default=False
 )
-def validate(files, schema, ext_schema, fiboa_version, collection, data):
+@click.option(
+    '--timer',
+    is_flag=True,
+    type=click.BOOL,
+    help='Measure the time the validation took.',
+    default=False,
+    hidden=True
+)
+def validate(files, schema, ext_schema, fiboa_version, collection, data, timer):
     """
     Validates a fiboa GeoParquet or GeoJSON file.
     """
+    start = time.perf_counter()
     log(f"fiboa CLI {__version__} - Validator\n", "success")
     config = {
         "schema": schema,
         "extension_schemas": ext_schema,
         "fiboa_version": fiboa_version,
         "collection": collection,
         "data": data,
     }
+
+    if len(files) == 0:
+        log("No files to validate", "error")
+        sys.exit(1)
+
+    exit = 0
     for file in files:
         log(f"Validating {file}", "info")
         try:
+            start_step = time.perf_counter()
             result = validate_(file, config)
             if result:
                 log("\n  => VALID\n", "success")
             else:
                 log("\n  => INVALID\n", "error")
-                sys.exit(1)
+                exit = 1
         except Exception as e:
             log(f"\n  => UNKNOWN: {e}\n", "error")
-            sys.exit(2)
+            exit = 2
+        finally:
+            if timer:
+                end_step = time.perf_counter()
+                log(f"Validated {file} in {end_step - start_step:0.4f} seconds")
+
+    if timer:
+        end = time.perf_counter()
+        log(f"All validated in {end - start:0.4f} seconds")
+
+    sys.exit(exit)
 
 
 ## VALIDATE SCHEMA
 @click.command()
 @click.argument('files', nargs=-1, callback=lambda ctx, param, value: valid_files_folders_for_cli(value, ["yaml", "yml"]))
 @click.option(
     '--metaschema', '-m',
@@ -135,21 +163,22 @@
     """
     Validates a fiboa schema file.
     """
     log(f"fiboa CLI {__version__} - Schema Validator\n", "success")
     config = {
         "metaschema": metaschema
     }
+    exit = 0
     for file in files:
         log(f"Validating {file}", "info")
         result = validate_schema_(file, config)
-        if result:
-            sys.exit(0)
-        else:
-            sys.exit(1)
+        if not result:
+            exit = 1
+
+    sys.exit(exit)
 
 
 ## CREATE PARQUET
 @click.command()
 @click.argument('files', nargs=-1, callback=lambda ctx, param, value: valid_files_folders_for_cli(value, ["json", "geojson"]))
 @click.option(
     '--out', '-o',
@@ -195,20 +224,19 @@
         "files": files,
         "out": out,
         "schema": schema,
         "collection": collection,
         "extension_schemas": ext_schema,
         "fiboa_version": fiboa_version
     }
-    create_geoparquet_(config)
-    # try:
-    #     create_geoparquet_(config)
-    # except Exception as e:
-    #     log(e, "error")
-    #     sys.exit(1)
+    try:
+        create_geoparquet_(config)
+    except Exception as e:
+        log(e, "error")
+        sys.exit(1)
 
 
 ## CREATE GEOJSON
 @click.command()
 @click.argument('file', nargs=1, callback=lambda ctx, param, value: valid_file_for_cli_with_ext(value, ["parquet", "geoparquet"]))
 @click.option(
     '--out', '-o',
@@ -294,25 +322,25 @@
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
 ## CONVERT
 @click.command()
-@click.argument('dataset', nargs=1)
+@click.argument('dataset', nargs=1, type=click.Choice(list_all_converter_ids()))
 @click.option(
     '--out', '-o',
     type=click.Path(exists=False),
     help='File to write the GeoParquet file to.',
     required=True
 )
 @click.option(
     '--cache', '-c',
     type=click.Path(exists=False),
-    help='For network requests: Local cache file to store the downloaded file to avoid multiple downloads.',
+    help='By default the CLI downloads the source data on every execution. Specify a local file path to avoid downloading the file again. If the file exists, reads from the path, otherwise stores the file there.',
     default=None
 )
 @click.option(
     '--source-coop', '-h',
     type=click.STRING,
     help='(Future) URL to the source cooperative repository, will be added to the Collection metadata.',
     default=None
@@ -320,26 +348,50 @@
 @click.option(
     '--collection',
     is_flag=True,
     type=click.BOOL,
     help='Export a Collection JSON alongside the data file.',
     default=False
 )
-def convert(dataset, out, cache, source_coop, collection):
+@click.option(
+    '--compression', '-pc',
+    type=click.Choice(["brotli", "gzip", "lz4", "snappy", "zstd", "none"]),
+    help='Compression method for the Parquet file. Defaults to zstd.',
+    default="zstd"
+)
+def convert(dataset, out, cache, source_coop, collection, compression):
     """
     Converts existing field boundary datasets to fiboa.
     """
     log(f"fiboa CLI {__version__} - Convert '{dataset}'\n", "success")
     try:
-        convert_(dataset, out, cache, source_coop, collection)
+        convert_(dataset, out, cache, source_coop, collection, compression)
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
+## CONVERTERS
+@click.command()
+def converters():
+    """
+    Lists all available converters.
+    """
+    log(f"fiboa CLI {__version__} - List of Converters\n", "success")
+
+    keys = ["TITLE", "LICENSE", "PROVIDER_NAME", "URI"]
+    converters = list_all_converters(keys)
+    df = pd.DataFrame.from_dict(converters, orient='index', columns=keys)
+
+    pd.set_option('display.max_columns', None)
+    pd.set_option('display.max_rows', None)
+
+    log(df)
+
+
 ## RENAME EXTENSION
 @click.command()
 @click.argument('folder', nargs=1, callback=valid_folder_for_cli)
 @click.option(
     '--title', '-t',
     type=click.STRING,
     help='Title of the extension, e.g. `Timestamps`',
@@ -378,11 +430,12 @@
 cli.add_command(describe)
 cli.add_command(validate)
 cli.add_command(validate_schema)
 cli.add_command(create_geoparquet)
 cli.add_command(create_geojson)
 cli.add_command(jsonschema)
 cli.add_command(convert)
+cli.add_command(converters)
 cli.add_command(rename_extension)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/convert_utils.py` & `fiboa_cli-0.4.0/fiboa_cli/convert_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,33 +16,38 @@
         url, columns,
         id, title, description, bbox,
         provider_name = None,
         provider_url = None,
         source_coop_url = None,
         extensions = [],
         missing_schemas = {},
+        column_additions = {},
         column_filters = {},
         column_migrations = {},
         migration = None,
         attribution = None,
         store_collection = False,
         license = None,
-        compression = "brotli",
+        compression = None,
         **kwargs):
     """
     Converts a German field boundary datasets to fiboa.
     """
     if not isinstance(get_fs(url), LocalFileSystem):
-        log("Loading file from: " + url)
+        log("Loading file")
     path = download_file(url, cache_file)
 
-    log("Local file is at: " + path)
-    gdf = gpd.read_file(path, **kwargs)
+    log("Reading into GeoDataFrame")
+    # If file is a parquet file then read with read_parquet
+    if path.endswith(".parquet") or path.endswith(".geoparquet"):
+        gdf = gpd.read_parquet(path, **kwargs)
+    else:
+        gdf = gpd.read_file(path, **kwargs)
 
-    log("Loaded into GeoDataFrame:")
+    log("GeoDataFrame created from source:")
     print(gdf.head())
 
     # 1. Run global migration
     has_migration = callable(migration)
     if has_migration:
         log("Applying global migrations")
         gdf = migration(gdf)
@@ -69,51 +74,59 @@
                     mask = result
 
                 # Filter columns based on the mask
                 gdf = gdf[mask]
             else:
                 log(f"Column '{key}' not found in dataset, skipping filter", "warning")
 
-    # 3. Run column migrations
+    # 3. Add constant columns
+    has_col_additions = len(column_additions) > 0
+    if has_col_additions:
+        log("Adding columns")
+        for key, value in column_additions.items():
+            gdf[key] = value
+            columns[key] = key
+
+    # 4. Run column migrations
     has_col_migrations = len(column_migrations) > 0
     if has_col_migrations:
         log("Applying column migrations")
         for key, fn in column_migrations.items():
             if key in gdf.columns:
                 gdf[key] = fn(gdf[key])
             else:
                 log(f"Column '{key}' not found in dataset, skipping migration", "warning")
 
-    if has_migration or has_col_migrations or has_col_filters:
+    if has_migration or has_col_migrations or has_col_filters or has_col_additions:
         log("GeoDataFrame after migrations and filters:")
         print(gdf.head())
 
-    # 4. Duplicate columns if needed
+    # 5. Duplicate columns if needed
     actual_columns = {}
     for old_key, new_key in columns.items():
         # If new keys are a list, duplicate the column
         if isinstance(new_key, list):
             for key in new_key:
                 gdf[key] = gdf.loc[:, old_key]
                 actual_columns[key] = key
         # If new key is a string, plan to rename the column
         elif old_key in gdf.columns:
             actual_columns[old_key] = new_key
         # If old key is not found, remove from the schema and warn
         else:
             log(f"Column '{old_key}' not found in dataset, removing from schema", "warning")
 
-    # 5. Rename columns
+    # 6. Rename columns
     gdf.rename(columns = actual_columns, inplace = True)
 
-    # 6. Remove all columns that are not listed
+    # 7. Remove all columns that are not listed
     drop_columns = list(set(gdf.columns) - set(actual_columns.values()))
     gdf.drop(columns = drop_columns, inplace = True)
 
-    log("Changed GeoDataFrame to:")
+    log("GeoDataFrame fully migrated:")
     print(gdf.head())
 
     collection = create_collection(
         gdf,
         id, title, description, bbox,
         provider_name = provider_name,
         provider_url = provider_url,
@@ -149,42 +162,42 @@
         extensions = [],
         attribution = None,
         license = None
     ):
     """
     Creates a collection for the field boundary datasets.
     """
-    if "determination_datetime" not in gdf.columns:
-        raise ValueError("determination_datetime column not available")
-
-    dates = pd.to_datetime(gdf['determination_datetime'])
-    min_time = to_iso8601(dates.min())
-    max_time = to_iso8601(dates.max())
-
     collection = {
         "fiboa_version": fiboa_version,
         "fiboa_extensions": extensions,
-        "stac_version": "1.0.0",
         "type": "Collection",
         "id": id,
         "title": title,
         "description": description,
         "license": "proprietary",
         "providers": [],
         "extent": {
             "spatial": {
                 "bbox": [bbox]
-            },
-            "temporal": {
-                "interval": [[min_time, max_time]]
             }
         },
         "links": []
     }
 
+    if "determination_datetime" in gdf.columns:
+        dates = pd.to_datetime(gdf['determination_datetime'])
+        min_time = to_iso8601(dates.min())
+        max_time = to_iso8601(dates.max())
+
+        collection["extent"]["temporal"] = {
+            "interval": [[min_time, max_time]]
+        }
+        # Without temporal extent it's not valid STAC
+        collection["stac_version"] = "1.0.0"
+
     # Add providers
     if provider_name is not None:
         collection["providers"].append({
             "name": provider_name,
             "roles": ["producer", "licensor"],
             "url": provider_url
         })
@@ -220,15 +233,15 @@
         elif license.lower() == "dl-de/zero-2-0":
             collection["links"].append({
                 "href": "https://www.govdata.de/dl-de/zero-2-0",
                 "title": "Data licence Germany - Zero - Version 2.0",
                 "type": "text/html",
                 "rel": "license"
             })
-        elif re.match(r"^[\w-]+$", license):
+        elif re.match(r"^[\w\.-]+$", license):
             collection["license"] = license
         else:
             log(f"Invalid license identifier: {license}", "warning")
     else:
         log(f"License information missing", "warning")
 
     return collection
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/create_geoparquet.py` & `fiboa_cli-0.4.0/fiboa_cli/create_geoparquet.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.9/fiboa_cli/describe.py` & `fiboa_cli-0.4.0/fiboa_cli/describe.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.9/fiboa_cli/geopandas.py` & `fiboa_cli-0.4.0/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.9/fiboa_cli/jsonschema.py` & `fiboa_cli-0.4.0/fiboa_cli/jsonschema.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,44 +58,53 @@
     if not isinstance(prop_schema, dict) or 'type' not in prop_schema:
         return prop_schema
     elif prop_schema['type'] not in datatypes:
         raise ValueError(f"Unknown datatype {prop_schema['type']}")
 
     datatype_schema = datatypes[prop_schema['type']].copy()
 
-    if required:
-        if '$ref' in datatype_schema:
+    if prop_schema['type'] == 'geometry':
+        geom_types = prop_schema.get('geometryTypes', [])
+        if isinstance(prop_schema.get('geometryTypes'), list):
             datatype_schema = {
-                "allOf": [
-                    datatype_schema,
-                    {
-                        "not": {
-                            "type": "null"
-                        }
-                    }
+                "anyOf": [
+                    {"$ref": f"https://geojson.org/schema/{type}.json"} for type in geom_types
                 ]
             }
+            del prop_schema['geometryTypes']
+
+    anyOf = datatype_schema.get('anyOf')
+    allOf = datatype_schema.get('allOf')
+    oneOf = datatype_schema.get('oneOf')
+    if required:
+        not_null_schema = { "not": { "type": "null" } }
+
+        if '$ref' in datatype_schema or isinstance(anyOf, list) or isinstance(oneOf, list):
+            datatype_schema = {
+                "allOf": [datatype_schema, not_null_schema]
+            }
+        elif (isinstance(allOf, list)):
+            allOf.append(not_null_schema)
+
     else:
-        if isinstance(datatype_schema.get('type'), str):
-            datatype_schema['type'] = [datatype_schema['type'], "null"]
-        elif '$ref' in datatype_schema:
+        schema_type = datatype_schema.get('type')
+        null_schema = { "type": "null" }
+
+        if '$ref' in datatype_schema:
             datatype_schema = {
-                "allOf": [
-                    datatype_schema,
-                    {
-                        "type": "null"
-                    }
-                ]
+                "allOf": [datatype_schema, null_schema]
             }
-        elif (isinstance(datatype_schema.get('type'), list)):
-            datatype_schema.get('type', []).append("null")
-        elif (isinstance(datatype_schema.get('oneOf'), list)):
-            datatype_schema.get('oneOf', []).append({"type": "null"})
-        elif (isinstance(datatype_schema.get('anyOf'), list)):
-            datatype_schema.get('anyOf', []).append({"type": "null"})
+        elif isinstance(schema_type, str):
+            datatype_schema['type'] = [datatype_schema['type'], "null"]
+        elif (isinstance(schema_type, list)):
+            datatype_schema["type"].append("null")
+        elif (isinstance(oneOf, list)):
+            datatype_schema["oneOf"].append(null_schema)
+        elif (isinstance(anyOf, list)):
+            datatype_schema["anyOf"].append(null_schema)
         else:
             log(f"Making schema {json.dumps(datatype_schema)} optional is not supported by this generator")
 
     # Avoid conflicting statements
     if 'exclusiveMaximum' in prop_schema:
         datatype_schema.pop('maximum', None)
     if 'exclusiveMinimum' in prop_schema:
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/jsonschema_template.py` & `fiboa_cli-0.4.0/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.9/fiboa_cli/parquet.py` & `fiboa_cli-0.4.0/fiboa_cli/parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from geopandas import GeoDataFrame
 from shapely.geometry import shape
 
 from .types import get_geopandas_dtype, get_pyarrow_type_for_geopandas, get_pyarrow_field
 from .util import log, load_fiboa_schema, load_file, merge_schemas
 from .geopandas import to_parquet
 
-def create_parquet(data, columns, collection, output_file, config, missing_schemas = {}, compression = "brotli"):
+def create_parquet(data, columns, collection, output_file, config, missing_schemas = {}, compression = None):
     # Load the data schema
     fiboa_schema = load_fiboa_schema(config)
     schemas = merge_schemas(missing_schemas, fiboa_schema)
 
     # Load all extension schemas
     extensions = {}
     if "fiboa_extensions" in collection and isinstance(collection["fiboa_extensions"], list):
@@ -65,14 +65,18 @@
         else:
             pq_fields.append(field)
 
     # Define the schema for the Parquet file
     pq_schema = pa.schema(pq_fields)
     pq_schema = pq_schema.with_metadata({"fiboa": json.dumps(collection).encode("utf-8")})
 
+    # See also https://github.com/fiboa/cli/pull/30
+    if compression is None:
+        compression = "zstd"
+
     # Write the data to the Parquet file
     # Proprietary function exported from geopandas to solve
     # https://github.com/geopandas/geopandas/issues/3182
     to_parquet(
         data,
         output_file,
         schema = pq_schema,
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/rename_extension.py` & `fiboa_cli-0.4.0/fiboa_cli/rename_extension.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.9/fiboa_cli/types.py` & `fiboa_cli-0.4.0/fiboa_cli/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+import datetime
 import pyarrow as pa
 import pyarrow.types as pat
 import pandas as pd
 import numpy as np
+from shapely.geometry.base import BaseGeometry
 
 def is_enum(schema):
     return isinstance(schema.get("enum"), list)
 
+def is_integer_type(dtype):
+    return dtype.startswith("int") or dtype.startswith("uint")
+
+def is_floating_type(dtype):
+    return dtype == "float" or dtype == "double"
+
+def is_numerical_type(dtype):
+    return is_integer_type(dtype) or is_floating_type(dtype)
+
+def is_temporal_type(dtype):
+    return dtype == "date" or dtype == "date-time"
+
+def is_scalar_type(dtype):
+    return dtype == "string" or dtype == "binary" or dtype == "boolean" or is_numerical_type(dtype) or is_temporal_type(dtype)
 
 def get_geopandas_dtype(type, required = False, schema = {}):
     """
     fiboa datatypes to geopandas datatypes
     """
-    if is_enum(schema) and (type == "string" or type.startswith("int") or type.startswith("uint")):
+    if is_enum(schema) and (type == "string" or is_integer_type(type)):
         return "category"
     elif type == "boolean":
         if required:
             return "bool"
         else:
             return "boolean"
     elif type == "int8":
@@ -80,15 +96,15 @@
     elif type == "object":
         return "object"
     elif type == "date" or type == "date-time":
         return lambda series: pd.to_datetime(series)
     elif type == "geometry":
         return None, # not a column, don't convert geometry
     elif type == "bounding-box":
-        raise Exception("Bounding boxes are not supported yet") # todo
+        return "object"
     else:
         return None
 
 
 def get_pyarrow_field(name, pa_type = None, schema = None, required = False):
     if pa_type is None:
         pa_type = get_pyarrow_type(schema)
@@ -101,24 +117,25 @@
 def get_pyarrow_type(schema):
     """
     fiboa datatypes to pyarrow datatypes
     """
     dtype = schema.get("type")
     if dtype == "boolean":
         return pa.bool_()
-    elif dtype.startswith("int") or dtype.startswith("uint") or dtype == "string" or dtype == "binary":
+    elif is_integer_type(dtype) or dtype == "string" or dtype == "binary":
         return getattr(pa, dtype)()
     elif dtype == "float":
         return pa.float32()
     elif dtype == "double":
         return pa.float64()
     elif dtype == "array":
         pa_subtype = get_pyarrow_type(schema.get("items", {}))
         return pa.list_(pa_subtype)
     elif dtype == "object":
+        # todo: add patternProperties
         additonal_properties = schema.get("additionalProperties", False)
         if additonal_properties is True:
             raise Exception("Additional properties for objects are not supported")
         else:
             properties = schema.get("properties", {})
             required_props = schema.get("required", [])
             fields = []
@@ -129,15 +146,21 @@
     elif dtype == "date":
         return pa.date32()
     elif dtype == "date-time":
         return pa.timestamp("ms", tz="UTC")
     elif dtype == "geometry":
         return pa.binary()
     elif dtype == "bounding-box":
-        raise Exception("Bounding boxes are not supported yet") # todo
+        coord_schema = {"type": "float"}
+        return pa.struct([
+            get_pyarrow_field("xmin", schema = coord_schema, required = True),
+            get_pyarrow_field("ymin", schema = coord_schema, required = True),
+            get_pyarrow_field("xmax", schema = coord_schema, required = True),
+            get_pyarrow_field("ymax", schema = coord_schema, required = True),
+        ])
     else:
         return None
 
 def get_pyarrow_type_for_geopandas(dtype):
     """
     geopandas datatypes to pyarrow datatypes
     """
@@ -150,15 +173,14 @@
     elif dtype.startswith("int") or dtype.startswith("uint") or dtype.startswith("float"): # float16/32/64
         return getattr(pa, dtype)()
     elif dtype == "object":
         return pa.string() # todo
     elif dtype == "datetime64":
         return pa.timestamp("ms", tz="UTC")
     else:
-        print(dtype)
         return None
 
 
 # checks pyarrow datatypes
 PA_TYPE_CHECK = {
     "boolean": pat.is_boolean,
     "int8": pat.is_int8,
@@ -170,19 +192,43 @@
     "int64": pat.is_int64,
     "uint64": pat.is_uint64,
     "float": pat.is_float32,
     "double": pat.is_float64,
     "binary": pat.is_binary,
     "string": pat.is_string,
     "array": pat.is_list,
-    "object": pat.is_map,
+    "object": lambda x: pat.is_struct(x) or pat.is_map(x),
     "date": pat.is_date32,
     "date-time": pat.is_timestamp,
-    "geometry": pat.is_binary, # todo: check more?
-    "bounding-box": None # todo
+    "geometry": pat.is_binary,
+    "bounding-box": pat.is_struct
+}
+
+
+# checks pyarrow datatypes
+PYTHON_TYPES = {
+    "boolean": (bool, np.bool_),
+    "int8": (int, np.int8),
+    "uint8": (int, np.uint8),
+    "int16": (int, np.int16),
+    "uint16": (int, np.uint16),
+    "int32": (int, np.int32),
+    "uint32": (int, np.uint32),
+    "int64": (int, np.int64),
+    "uint64": (int, np.uint64),
+    "float": (float, np.float32),
+    "double": (float, np.float64),
+    "binary": (str, np.bytes_),
+    "string": (str, np.str_),
+    "array": (list, np.ndarray),
+    "object": dict,
+    "date": (datetime.date, np.datetime64),
+    "date-time": (datetime.datetime, np.datetime64),
+    "geometry": BaseGeometry,
+    "bounding-box": dict
 }
 
 LOG_STATUS_COLOR = {
     "info": "white",
     "warning": "yellow",
     "error": "red",
     "success": "green"
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/util.py` & `fiboa_cli-0.4.0/fiboa_cli/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 from .const import LOG_STATUS_COLOR, SUPPORTED_PROTOCOLS, STAC_COLLECTION_SCHEMA, GEOPARQUET_SCHEMA
 from .geopandas import decode_metadata, arrow_to_geopandas
 
 small_file_cache = {}
 big_file_cache = {}
 
-def log(text: str, status="info"):
+def log(text: str, status="info", nl = True):
     """Log a message with a severity level (which leads to different colors)"""
-    click.echo(click.style(text, fg=LOG_STATUS_COLOR[status]))
+    click.echo(click.style(text, fg=LOG_STATUS_COLOR[status]), nl=nl)
 
 
 def stream_file(fs, src_uri, dst_file, chunk_size = 10 * 1024 * 1024):
     with fs.open(src_uri, mode='rb') as f:
         while True:
             chunk = f.read(chunk_size)
             if not chunk:
@@ -262,15 +262,16 @@
     return schema.copy()
 
 
 def parse_metadata(schema, key):
     if key in schema.metadata:
         return decode_metadata(schema.metadata[key])
     else:
-        log(f"Parquet file schema does not have a '{key}' key", "warning")
+        str_key = key.decode("utf-8")
+        log(f"Parquet file schema does not have a '{str_key}' key", "warning")
         return None
 
 
 def to_iso8601(dt):
     iso = dt.isoformat()
     if iso.endswith("+00:00"):
         return iso[:-6] + "Z"
@@ -291,13 +292,14 @@
     if "version" in obj:
         return load_file(GEOPARQUET_SCHEMA.format(version = obj["version"]))
     else:
         return None
 
 
 def log_extensions(collection, logger):
-    if len(collection["fiboa_extensions"]) == 0:
+    extensions = collection.get("fiboa_extension", [])
+    if len(extensions) == 0:
         logger("fiboa extensions: none")
     else:
         logger("fiboa extensions:")
-        for ext in collection["fiboa_extensions"]:
-            logger(f"  - {ext}")
+        for extension in extensions:
+            logger(f"  - {extension}")
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/validate.py` & `fiboa_cli-0.4.0/fiboa_cli/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,39 +19,41 @@
     else:
         return validate_parquet(file, config)
 
 
 def validate_collection(collection, config):
     valid = True
 
+    collection_verrsion = collection.get("fiboa_version")
+    config_version = config.get("fiboa_version")
+
     # Check fiboa version
-    if "fiboa_version" not in collection:
-        log("No fiboa_version found in collection metadata", "error")
+    if not isinstance(collection_verrsion, str):
+        log("No fiboa_version string found in collection metadata", "error")
         valid = False
-    elif config.get("fiboa_version") is None:
-        config["fiboa_version"] = collection["fiboa_version"]
 
-    log("fiboa version: " + collection["fiboa_version"])
+    log("fiboa version: " + config_version)
 
-    if collection["fiboa_version"] != config["fiboa_version"]:
-        log(f"fiboa versions differs: Collection is {collection['fiboa_version']} and requested specification version is {config['fiboa_version']}", "warning")
+    if isinstance(collection_verrsion, str) and collection_verrsion != config_version:
+        log(f"fiboa versions differs: Collection is {collection_verrsion} and requested specification version is {config_version}", "warning")
 
     # Check STAC Collection
     if not validate_colletion_schema(collection):
         valid = False
 
     # Check extensions
     extensions = {}
     if "fiboa_extensions" in collection:
-        if not isinstance(collection["fiboa_extensions"], list):
+        ext_list = collection.get("fiboa_extensions")
+        if not isinstance(ext_list, list):
             log("fiboa_extensions must be a list", "error")
             valid = False
         else:
             ext_map = config.get("extension_schemas", [])
-            for ext in collection["fiboa_extensions"]:
+            for ext in ext_list:
                 try:
                     if ext in ext_map:
                         path = ext_map[ext]
                         log(f"Redirecting {ext} to {path}", "info")
                     else:
                         path = ext
                     extensions[ext] = load_file(path)
@@ -61,26 +63,36 @@
 
     log_extensions(collection, lambda x: log(x, "info", False))
 
     return valid, extensions
 
 
 def validate_geojson(file, config):
+    valid = True
+    extensions = {}
+
     try:
         data = load_file(file)
     except Exception as error:
         log(error, "error")
         return False
 
     collection = get_collection(data, config.get("collection"), file)
     if collection is None:
         log("No collection specified", "error")
-        return False
+        valid = False
+
+    if config.get("fiboa_version") is None and collection.get("fiboa_version") is not None:
+        config["fiboa_version"] = collection.get("fiboa_version")
+
+    if collection is not None:
+        collection_valid, extensions = validate_collection(collection, config)
+        if not collection_valid:
+            valid = False
 
-    valid, extensions = validate_collection(collection, config)
     core_schema = load_fiboa_schema(config)
     datatypes = load_datatypes(config["fiboa_version"])
     schema = create_jsonschema(core_schema, datatypes)
 
     # Load extensions
     ext_errors = []
     for ext in extensions:
@@ -143,40 +155,45 @@
 
     return valid
 
 
 def validate_parquet(file, config):
     parquet_schema = load_parquet_schema(file)
     valid = True
+    extensions = {}
 
     # Validate geo metadata in Parquet header
     if b"geo" not in parquet_schema.metadata:
         log("Parquet file schema does not have 'geo' key", "error")
-        return False
+        valid = False
     else:
         geo = parse_metadata(parquet_schema, b"geo")
         if not validate_geoparquet_schema(geo):
             valid = False
 
     # Validate fiboa metadata in Parquet header
     collection = {}
     if b"fiboa" not in parquet_schema.metadata:
         log("Parquet file schema does not have a 'fiboa' key", "warning")
         if not config.get("collection"):
             log("No collection specified", "error")
-            return False
+            valid = False
         else:
             collection = load_file(config.get("collection"))
     else:
         collection = parse_metadata(parquet_schema, b"fiboa")
 
+    if config.get("fiboa_version") is None and collection.get("fiboa_version") is not None:
+        config["fiboa_version"] = collection.get("fiboa_version")
+
     # Validate Collection
-    valid_collection, extensions = validate_collection(collection, config)
-    if not valid_collection:
-        valid = False
+    if len(collection) > 0:
+        valid_collection, extensions = validate_collection(collection, config)
+        if not valid_collection:
+            valid = False
 
     # load the actual fiboa schema
     fiboa_schema = load_fiboa_schema(config)
 
     # Load data if needed
     gdf = None
     if config.get("data"):
@@ -235,17 +252,19 @@
         if dtype == "date-time":
             if pq_type.unit != "ms":
                 log(f"{key}: Timestamp unit differs, should be ms", "warning")
             if pq_type.tz != "UTC":
                 log(f"{key}: Timestamp timezone invalid, must be UTC", "error")
                 valid = False
         elif dtype == "object":
-            if not pat.is_string(pq_field.key_type):
-                log(f"{key}: Map key datatype is not string", "error")
+            if pat.is_map(pq_type) and not pat.is_string(pq_field.key_type):
+                log(f"{key}: Map keys must be strings", "error")
                 valid = False
+        elif dtype == "geometry":
+            valid = validate_geometry_column(key, prop_schema, geo, valid)
 
         # Validate data of the column
         if gdf is not None:
             issues = validate_column(gdf[key], prop_schema)
             if len(issues) > 0:
                 for issue in issues:
                     log(f"{key}: {issue}")
@@ -254,14 +273,34 @@
     # Show a note once if data was not validated
     if not config.get("data"):
         log("Data was not validated as the --data parameter was not provided", "info")
 
     return valid
 
 
+def validate_geometry_column(key, prop_schema, geo, valid = True):
+    columns = geo.get("columns", {})
+    if key not in columns:
+        log(f"{key}: Geometry column not found in GeoParquet metadata", "error")
+        valid = False
+
+    schema_geo_types = prop_schema.get("geometryTypes", [])
+    schema_geo_types.sort()
+    if len(schema_geo_types) > 0:
+        gp_geo_types = columns[key].get("geometry_types", [])
+        gp_geo_types.sort()
+        if len(gp_geo_types) == 0:
+            log(f"{key}: No geometry types specified in GeoParquet metadata", "warning")
+
+        if schema_geo_types != gp_geo_types:
+            log(f"{key}: GeoParquet geometry types differ, is {gp_geo_types} but must be {schema_geo_types}", "error")
+            valid = False
+
+    return valid
+
 # todo: use stac_validator instead of our own validation routine
 def validate_colletion_schema(obj):
     if "stac_version" in obj:
         try:
             schema = load_collection_schema(obj)
             errors = validate_json_schema(obj, schema)
             for error in errors:
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/validate_data.py` & `fiboa_cli-0.4.0/fiboa_cli/validate_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,95 @@
 import re
 import pandas as pd
+
 from urllib.parse import urlparse
+from shapely.validation import explain_validity
+
+from .types import PYTHON_TYPES, is_numerical_type, is_scalar_type
+
+REGEX_EMAIL = re.compile("[^@]+@[^@]+\.[^@]+")
+REGEX_UUID = re.compile("^[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}\Z")
 
 def validate_column(data, rules):
-    for _, value in data.items():
-        if pd.isna(value):
+    for value in data:
+        isna = pd.isna(value)
+        if isinstance(isna, bool) and isna:
             # Skip validation for NaN values or implement special handling if required
             continue
 
-        if isinstance(value, str):
+        dtype = rules.get("type")
+        expected_pytype = PYTHON_TYPES.get(dtype)
+        if expected_pytype is not None and not isinstance(value, expected_pytype):
+            actualy_pytype = type(value)
+            return [f"Value '{value}' is not of type {dtype}, is {actualy_pytype}"]
+
+        if dtype == "string":
             issues = validate_string(value, rules)
-        elif isinstance(value, (int, float)):
+        elif is_numerical_type(dtype):
             issues = validate_numerical(value, rules)
-        elif isinstance(value, list):
+        elif dtype == "array":
             issues = validate_array(value, rules)
-        elif isinstance(value, dict):
+        elif dtype == "geometry":
+            issues = validate_geometry(value, rules)
+        elif dtype == "bounding-box":
+            issues = validate_bbox(value, rules)
+        elif dtype == "object":
             issues = validate_object(value, rules)
         else:
             continue
 
-        if (len(issues) > 0):
+        if len(issues) > 0:
             return issues
 
     return []
 
+# Geometry validation
+def validate_bbox(value, rules):
+    issues = []
+
+    if value["xmin"] > value["xmax"]:
+        issues.append(f"Bounding box has xmin value greater than xmax value: {value['xmin']} > {value['xmax']}")
+    elif value["ymin"] > value["ymax"]:
+        issues.append(f"Bounding box has ymin value greater than ymax value: {value['ymin']} > {value['ymax']}")
+
+    return issues
+
+# Geometry validation
+def validate_geometry(value, rules):
+    issues = []
+
+    geom_types = rules.get("geometryTypes", [])
+    if len(geom_types) > 0 and value.geom_type not in geom_types:
+        allowed = ", ".join(geom_types)
+        issues.append(f"Geometry type '{value.geom_type}' is not one of the allowed types: {allowed}")
+
+    why = explain_validity(value)
+    if why != 'Valid Geometry':
+        issues.append(f"Geometry {value} is not valid: {why}")
+
+    return issues
+
 # String validation
 def validate_string(value, rules):
     issues = []
     if 'minLength' in rules and len(value) < rules['minLength']:
         issues.append(f"String '{value}' is shorter than the minimum length of {rules['minLength']}.")
     if 'maxLength' in rules and len(value) > rules['maxLength']:
         issues.append(f"String '{value}' is longer than the maximum length of {rules['maxLength']}.")
     if 'pattern' in rules and not re.match(rules['pattern'], value):
         issues.append(f"String '{value}' does not match the required pattern: {rules['pattern']}.")
     if 'enum' in rules and value not in rules['enum']:
         allowed = ", ".join(rules['enum'])
         issues.append(f"String '{value}' is not one of the allowed values in the enumeration: {allowed}")
     if 'format' in rules:
-        # todo: pre-compile regexes
-        if rules['format'] == 'email' and not re.match(r"[^@]+@[^@]+\.[^@]+", value):
+        if rules['format'] == 'email' and not REGEX_EMAIL.match(value):
             issues.append(f"String '{value}' is not a valid email address.")
         if rules['format'] == 'uri' and not urlparse(value).scheme:
             issues.append(f"String '{value}' is not a valid URI.")
-        if rules['format'] == 'uuid' and not re.match(r"^[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}\Z", value):
+        if rules['format'] == 'uuid' and not REGEX_UUID.match(value):
             issues.append(f"String '{value}' is not a valid UUID.")
     return issues
 
 # Numerical validation
 def validate_numerical(value, rules):
     issues = []
     if 'minimum' in rules and value < rules['minimum']:
@@ -55,30 +98,50 @@
         issues.append(f"Value {value} is greater than the maximum allowed value of {rules['maximum']}.")
     if 'exclusiveMinimum' in rules and value <= rules['exclusiveMinimum']:
         issues.append(f"Value {value} is less than or equal to the exclusive minimum value of {rules['exclusiveMinimum']}.")
     if 'exclusiveMaximum' in rules and value >= rules['exclusiveMaximum']:
         issues.append(f"Value {value} is greater than or equal to the exclusive maximum value of {rules['exclusiveMaximum']}.")
     if 'enum' in rules and value not in rules['enum']:
         allowed = ", ".join(map(str, rules['enum']))
-        issues.append(f"String '{value}' is not one of the allowed values in the enumeration: {allowed}")
+        issues.append(f"Integer '{value}' is not one of the allowed values in the enumeration: {allowed}")
     return issues
 
 # Array validation
 def validate_array(values, rules):
     issues = []
+
+    item_schema = rules.get('items', {})
+
     if 'minItems' in rules and len(values) < rules['minItems']:
         issues.append(f"Array has fewer items than the minimum of {rules['minItems']}.")
     if 'maxItems' in rules and len(values) > rules['maxItems']:
         issues.append(f"Array has more items than the maximum of {rules['maxItems']}.")
-    if 'uniqueItems' in rules and rules['uniqueItems'] and len(values) != len(set(values)):
-        issues.append("Array items are not unique.")
+
+    if 'uniqueItems' in rules and rules['uniqueItems']:
+        item_dtype = item_schema.get('type')
+        if is_scalar_type(item_dtype) and len(values) != len(set(values)):
+            issues.append("Array items are not unique.")
+        else:
+            pass # not supported for non-scalar types
+
+
     # todo: Further validation for 'items' if necessary
     return issues
 
 # Object validation
 def validate_object(value, rules):
     issues = []
-    for key, val in rules['properties'].items():
+
+    if 'minProperties' in rules and len(value) < rules['minProperties']:
+        issues.append(f"Object has fewer properties than the minimum of {rules['minProperties']}.")
+    if 'maxProperties' in rules and len(value) > rules['maxProperties']:
+        issues.append(f"Object has more properties than the maximum of {rules['maxProperties']}.")
+
+    props = rules.get('properties', {})
+    other_props = rules.get('additionalProperties', False)
+    pattern_props = rules.get('patternProperties', {})
+    for key, val in props.items():
         if key not in value:
             issues.append(f"Key '{key}' is missing from the object.")
         # todo: Further validation based on the type of property
+
     return issues
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli/validate_schema.py` & `fiboa_cli-0.4.0/fiboa_cli/validate_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def validate_schema(file, config):
     schema = load_file(file)
     if not isinstance(schema, dict):
         log("Schema must be an object", "error")
         return False
 
     metaschema_uri = config.get("metaschema")
-    if "$schema" in schema:
+    if metaschema_uri is None:
         metaschema_uri = schema.get("$schema", metaschema_uri)
     if metaschema_uri is None:
         log("No metaschema provided", "error")
         return False
 
     log(f"Metaschema: {metaschema_uri}", "info")
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli.egg-info/PKG-INFO` & `fiboa_cli-0.4.0/fiboa_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.9
+Version: 0.4.0
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Requires-Dist: pyarrow>=14.0
 Requires-Dist: fsspec>=2024.0
 Requires-Dist: click>=8.1
 Requires-Dist: geopandas>=0.14
 Requires-Dist: requests>=2.30
 Requires-Dist: aiohttp>=3.9
 Requires-Dist: shapely>=2.0
+Requires-Dist: numpy>=1.20.0
 Provides-Extra: de-nrw
 
 # fiboa CLI
 
 A command-line interface (CLI) for working with fiboa.
 
 - [Getting Started](#getting-started)
@@ -50,24 +51,29 @@
 
 After the installation you should be able to run the following command: `fiboa`
 
 You should see usage instructions and [available commands](#commands) for the CLI.
 
 fiboa CLI supports various commands to work with the files:
 
-- [Inspect fiboa GeoParquet files](#inspect-fiboa-geoparquet-file)
-- [Validation fiboa GeoParquet and GeoJSON files](#validation)
-- [Convert existing non-fiboa datasets to a fiboa GeoParquet file](#converter-for-existing-datasets)
-- File Format Conversion:
-  - [Create a fiboa GeoParquet file from GeoJSON files](#create-fiboa-geoparquet-from-geojson)
-  - [Create fiboa GeoJSON files from a GeoParquet file](#create-fiboa-geojson-from-geoparquet)
-- Extension and Spec development:
-  - [Update an extension template with new names](#update-an-extension-template-with-new-names)
-  - [Validate a fiboa Schema](#validate-a-fiboa-schema)
-  - [Create JSON Schema from fiboa Schema](#create-json-schema-from-fiboa-schema)
+- [fiboa CLI](#fiboa-cli)
+  - [Getting Started](#getting-started)
+    - [Installation](#installation)
+    - [Execute a command](#execute-a-command)
+  - [Commands](#commands)
+    - [Validation](#validation)
+    - [Create fiboa GeoParquet from GeoJSON](#create-fiboa-geoparquet-from-geojson)
+    - [Create fiboa GeoJSON from GeoParquet](#create-fiboa-geojson-from-geoparquet)
+    - [Inspect fiboa GeoParquet file](#inspect-fiboa-geoparquet-file)
+    - [Create JSON Schema from fiboa Schema](#create-json-schema-from-fiboa-schema)
+    - [Validate a fiboa Schema](#validate-a-fiboa-schema)
+    - [Update an extension template with new names](#update-an-extension-template-with-new-names)
+    - [Converter for existing datasets](#converter-for-existing-datasets)
+  - [Development](#development)
+    - [Implement a converter](#implement-a-converter)
 
 ## Commands
 
 ### Validation
 
 To validate a fiboa GeoParquet or GeoJSON file, you can for example run:
 
@@ -144,24 +150,22 @@
 Then the following command could be used:
 - `fiboa rename-extension . -t Timestamps -p ts -s timestamps-extension -o fiboa`
 
 Check `fiboa rename-extension --help` for more details.
 
 ### Converter for existing datasets
 
-To convert an existing dataset to fiboa using the pre-defined converters:
+The CLI ships various converters for existing datasets.
 
-- `fiboa convert de_nrw`
+To get a list of available converters/datasets with title, license, etc. run:
+- `fiboa converters`
+
+Use any of the IDs from the list to convert an existing dataset to fiboa:
 
-Available converters:
-- `at` (Austria)
-- `de_bb` (Berlin/Brandenburh, Germany)
-- `de_nds` (Lowe Saxony, Germany)
-- `de_nrw` (North Rhine-Westphalia, Germany)
-- `de_sh` (Schleswig-Holstein, Germany)
+- `fiboa convert de_nrw`
 
 See [Implement a converter](#implement-a-converter) for details about how to 
 
 ## Development
 
 To install in development mode run `pip install -e .` in this folder.
```

### Comparing `fiboa_cli-0.3.9/fiboa_cli.egg-info/SOURCES.txt` & `fiboa_cli-0.4.0/fiboa_cli.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -21,8 +21,17 @@
 fiboa_cli/version.py
 fiboa_cli.egg-info/PKG-INFO
 fiboa_cli.egg-info/SOURCES.txt
 fiboa_cli.egg-info/dependency_links.txt
 fiboa_cli.egg-info/entry_points.txt
 fiboa_cli.egg-info/requires.txt
 fiboa_cli.egg-info/top_level.txt
+fiboa_cli/datasets/__init__.py
+fiboa_cli/datasets/at.py
+fiboa_cli/datasets/de_bb.py
+fiboa_cli/datasets/de_nds.py
+fiboa_cli/datasets/de_nrw.py
+fiboa_cli/datasets/de_sh.py
+fiboa_cli/datasets/de_th.py
+fiboa_cli/datasets/ec_fr.py
+fiboa_cli/datasets/template.py
 tests/test_jsonschema.py
```

### Comparing `fiboa_cli-0.3.9/setup.py` & `fiboa_cli-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         "pyyaml>=6.0",
         "pyarrow>=14.0",
         "fsspec>=2024.0",
         "click>=8.1",
         "geopandas>=0.14",
         "requests>=2.30",
         "aiohttp>=3.9",
-        "shapely>=2.0"
+        "shapely>=2.0",
+        "numpy>=1.20.0"
     ],
     extras_require={
         # Optional dependencies for datasets converters go here
         'de_nrw': [
             # No optional dependencies for de_nrw datasets converter needed
         ]
     },
```

