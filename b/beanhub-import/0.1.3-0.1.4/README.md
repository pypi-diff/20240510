# Comparing `tmp/beanhub_import-0.1.3.tar.gz` & `tmp/beanhub_import-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.1.3.tar", max compression
+gzip compressed data, was "beanhub_import-0.1.4.tar", max compression
```

## Comparing `beanhub_import-0.1.3.tar` & `beanhub_import-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-05-09 19:08:49.072095 beanhub_import-0.1.3/LICENSE
--rw-r--r--   0        0        0    22266 2024-05-09 19:08:49.072095 beanhub_import-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/__init__.py
--rw-r--r--   0        0        0      231 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/constants.py
--rw-r--r--   0        0        0     4617 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/data_types.py
--rw-r--r--   0        0        0     7962 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/post_processor.py
--rw-r--r--   0        0        0    10490 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/processor.py
--rw-r--r--   0        0        0      276 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/templates.py
--rw-r--r--   0        0        0      757 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    23189 1970-01-01 00:00:00.000000 beanhub_import-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/LICENSE
+-rw-r--r--   0        0        0    22473 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/beanhub_import/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/beanhub_import/constants.py
+-rw-r--r--   0        0        0     4617 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     7958 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0    10490 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/beanhub_import/processor.py
+-rw-r--r--   0        0        0      276 2024-05-09 19:51:22.510969 beanhub_import-0.1.4/beanhub_import/templates.py
+-rw-r--r--   0        0        0      757 2024-05-09 19:51:22.514969 beanhub_import-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    23396 1970-01-01 00:00:00.000000 beanhub_import-0.1.4/PKG-INFO
```

### Comparing `beanhub_import-0.1.3/LICENSE` & `beanhub_import-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.3/README.md` & `beanhub_import-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# beanhub-import
+# beanhub-import [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-import/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-import/tree/master)
 
 Beanhub-import is a simple, smart, and easy-to-use library for importing extracted transactions from beanhub-extract.
 It generates Beancount transactions based on predefined rules.
 
 **Note**: This project is still in early stage, still subject to rapid major changes
 
 ## Features
```

### Comparing `beanhub_import-0.1.3/beanhub_import/data_types.py` & `beanhub_import-0.1.4/beanhub_import/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.3/beanhub_import/post_processor.py` & `beanhub_import-0.1.4/beanhub_import/post_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,18 @@
 ) -> dict[pathlib.Path, ChangeSet]:
     generated_id_txns = {txn.id: txn for txn in generated_txns}
     imported_id_txns = {txn.id: txn for txn in imported_txns}
 
     to_remove = collections.defaultdict(list)
     for txn in imported_txns:
         generated_txn = generated_id_txns.get(txn.id)
-        generated_file = (work_dir / generated_txn.file).resolve()
-        if generated_txn is not None and txn.file.resolve() != generated_file:
+        if (
+            generated_txn is not None
+            and txn.file.resolve() != (work_dir / generated_txn.file).resolve()
+        ):
             # it appears that the generated txn's file is different from the old one, let's remove it
             to_remove[txn.file].append(txn)
 
     to_add = collections.defaultdict(list)
     to_update = collections.defaultdict(dict)
     for txn in generated_txns:
         imported_txn = imported_id_txns.get(txn.id)
```

### Comparing `beanhub_import-0.1.3/beanhub_import/processor.py` & `beanhub_import-0.1.4/beanhub_import/processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.3/pyproject.toml` & `beanhub_import-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.1.3"
+version = "0.1.4"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.1.3/PKG-INFO` & `beanhub_import-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.1.3
+Version: 0.1.4
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: beanhub-extract (>=0.0.7,<0.1.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
-# beanhub-import
+# beanhub-import [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-import/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-import/tree/master)
 
 Beanhub-import is a simple, smart, and easy-to-use library for importing extracted transactions from beanhub-extract.
 It generates Beancount transactions based on predefined rules.
 
 **Note**: This project is still in early stage, still subject to rapid major changes
 
 ## Features
```

