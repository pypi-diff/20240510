# Comparing `tmp/pastperfect-0.1.0.tar.gz` & `tmp/pastperfect-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastperfect-0.1.0.tar", max compression
+gzip compressed data, was "pastperfect-0.1.1.tar", max compression
```

## Comparing `pastperfect-0.1.0.tar` & `pastperfect-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-05-02 19:59:02.121990 pastperfect-0.1.0/LICENSE
--rw-r--r--   0        0        0      870 2024-05-02 20:50:55.470882 pastperfect-0.1.0/README.md
--rw-r--r--   0        0        0     1097 2024-05-07 21:05:35.228887 pastperfect-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       42 2024-05-02 19:59:02.125536 pastperfect-0.1.0/src/pastperfect/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-07 21:04:43.334099 pastperfect-0.1.0/src/pastperfect/events.py
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 pastperfect-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-02 19:59:02.121990 pastperfect-0.1.1/LICENSE
+-rw-r--r--   0        0        0      915 2024-05-09 15:38:32.222021 pastperfect-0.1.1/README.md
+-rw-r--r--   0        0        0     1061 2024-05-10 07:13:51.730753 pastperfect-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-05-02 19:59:02.125536 pastperfect-0.1.1/src/pastperfect/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-07 21:04:43.334099 pastperfect-0.1.1/src/pastperfect/events.py
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 pastperfect-0.1.1/PKG-INFO
```

### Comparing `pastperfect-0.1.0/LICENSE` & `pastperfect-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pastperfect-0.1.0/src/pastperfect/events.py` & `pastperfect-0.1.1/src/pastperfect/events.py`

 * *Files identical despite different names*

### Comparing `pastperfect-0.1.0/PKG-INFO` & `pastperfect-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastperfect
-Version: 0.1.0
+Version: 0.1.1
 Summary: An experience on storing events.
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -16,37 +16,38 @@
 
 # Past Perfect
 
 [![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
 
 An experience on storing events.
 
-## How to use
+## How to use ?
 
-Create a table in your database:
-```sql
-CREATE TABLE IF NOT EXISTS event (
-    id INTEGER PRIMARY KEY,
-    name VARCHAR(30) NOT NULL,
-    data JSON NOT NULL,
-    created_at DATETIME NOT NULL,
-    UNIQUE(name, data, created_at)
+Create the [event table](./migrations/01%20-%20Initial.sql) in your database.
+
+```python
+from pastperfect import Events
+
+db_session = ... # db_session from sqlachemy
+events = Events(db_session)
+events.append(
+    Event(name="SomethingHappened", data={"key": "value"}),
 )
 ```
 
 ## Setup Development Environment
 
 You need the following tools installed on your machine:
 
 - [Poetry](https://python-poetry.org) for Python package management.
 - [Poetry Plugin: Export](https://github.com/python-poetry/poetry-plugin-export)
   for exporting dependencies.
 - [Poetry Plugin: up](https://github.com/MousaZeidBaker/poetry-plugin-up)
   for updating dependencies.
 
-Ensure you have Python 3.9 or above installed by running:
+Ensure you have Python 3.9 and above installed by running:
 
 ```bash
 python --version
 # Python 3.9.x
 ```
```

