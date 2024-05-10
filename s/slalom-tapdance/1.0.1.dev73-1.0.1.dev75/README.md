# Comparing `tmp/slalom_tapdance-1.0.1.dev73.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev73.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev75.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev73.tar` & `slalom_tapdance-1.0.1.dev75.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-09 18:45:08.217168 slalom_tapdance-1.0.1.dev73/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/install_helper.py
--rw-r--r--   0        0        0    38838 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/states.py
--rw-r--r--   0        0        0    11998 2024-05-09 18:44:51.529078 slalom_tapdance-1.0.1.dev73/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev73/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-10 19:28:08.355472 slalom_tapdance-1.0.1.dev75/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38838 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/states.py
+-rw-r--r--   0        0        0    11998 2024-05-10 19:27:50.395519 slalom_tapdance-1.0.1.dev75/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev75/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev73/LICENSE` & `slalom_tapdance-1.0.1.dev75/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev73/pyproject.toml` & `slalom_tapdance-1.0.1.dev75/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.73"
+version = "1.0.1-dev.75"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev73/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev75/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev73/tapdance/config.py` & `slalom_tapdance-1.0.1.dev75/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev73/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev75/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev73/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev75/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev73/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev75/tapdance/plans.py`

 * *Files 0% similar despite different names*

```diff
@@ -881,15 +881,15 @@
     output_file = output_file or os.path.join(catalog_dir, f"{table_name}-catalog.json")
     included_table_objects = []
     catalog_full = json.loads(Path(source_catalog_path).read_text())
     # Loop through all the tables in the catalog
     for tbl in catalog_full["streams"]:
         stream_name = _get_stream_name(tbl)
         # Always add the current table to it's catalog
-        if stream_name in table_name:
+        if stream_name == table_name:
             _get_stream_metadata_object(tbl)["selected"] = True
             logging.info(f'Adding current table:{table_name} to catalog.')
             included_table_objects.append(tbl)
         # If all_table_catalog is set, add every table to the current table's catalog.
         elif stream_name not in table_name and all_table_catalog:
             logging.info('All Table Catalogs is selected. Adding all tables to catalog')
             _get_stream_metadata_object(tbl)["selected"] = False
```

### Comparing `slalom_tapdance-1.0.1.dev73/tapdance/states.py` & `slalom_tapdance-1.0.1.dev75/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev73/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev75/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev73/PKG-INFO` & `slalom_tapdance-1.0.1.dev75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev73
+Version: 1.0.1.dev75
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

