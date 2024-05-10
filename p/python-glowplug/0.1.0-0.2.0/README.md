# Comparing `tmp/python_glowplug-0.1.0.tar.gz` & `tmp/python_glowplug-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glowplug-0.1.0.tar", max compression
+gzip compressed data, was "python_glowplug-0.2.0.tar", max compression
```

## Comparing `python_glowplug-0.1.0.tar` & `python_glowplug-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.1.0/LICENSE
--rw-r--r--   0        0        0      460 2024-05-10 18:24:31.267938 python_glowplug-0.1.0/README.md
--rw-r--r--   0        0        0      482 2024-05-10 18:34:30.234109 python_glowplug-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.1.0/src/glowplug/__init__.py
--rw-r--r--   0        0        0     1870 2024-05-10 18:26:01.970209 python_glowplug-0.1.0/src/glowplug/base.py
--rw-r--r--   0        0        0     2094 2024-05-10 18:24:29.874971 python_glowplug-0.1.0/src/glowplug/mssql.py
--rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.1.0/src/glowplug/pg.py
--rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.1.0/src/glowplug/sqlite.py
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 python_glowplug-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.0/LICENSE
+-rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.0/README.md
+-rw-r--r--   0        0        0      499 2024-05-10 19:16:21.052178 python_glowplug-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.0/src/glowplug/__init__.py
+-rw-r--r--   0        0        0     2800 2024-05-10 19:18:04.572166 python_glowplug-0.2.0/src/glowplug/base.py
+-rw-r--r--   0        0        0     2094 2024-05-10 18:24:29.874971 python_glowplug-0.2.0/src/glowplug/mssql.py
+-rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.0/src/glowplug/pg.py
+-rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.0/src/glowplug/sqlite.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.0/PKG-INFO
```

### Comparing `python_glowplug-0.1.0/LICENSE` & `python_glowplug-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.1.0/src/glowplug/mssql.py` & `python_glowplug-0.2.0/src/glowplug/mssql.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.1.0/src/glowplug/pg.py` & `python_glowplug-0.2.0/src/glowplug/pg.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.1.0/src/glowplug/sqlite.py` & `python_glowplug-0.2.0/src/glowplug/sqlite.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.1.0/PKG-INFO` & `python_glowplug-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: python-glowplug
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/jnu/python-glowplug
 License: MIT
 Author: Joe Nudell
 Author-email: jnudell@hks.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: alembic (>=1.5,<2.0)
 Requires-Dist: sqlalchemy (>=2,<3)
 Project-URL: Repository, https://github.com/jnu/python-glowplug
 Description-Content-Type: text/markdown
 
 Glowplug
 ===
 
 A consistent interface for maintenance operations on database engines not covered by SQLAlchemy.
 
-Chooses opinionated drivers with both async + sync support.
+Chooses opinionated drivers with both async + sync support, as well as support for Alembic.
 
 ## Supported operations
 
  - `exists` - Check if database exists
  - `create` - Create a new database
  - `init` - Create all tables in the given database, optionally dropping first
+ - `alembic` - Run any of the alembic commands on the given database
 
 ## Supported databases
 
  - SQLite (`aiosqlite`)
  - Postgres (`asyncpg`)
  - MS Sql (`pyodbc` and `aioodbc`)
```

