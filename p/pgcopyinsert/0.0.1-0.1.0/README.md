# Comparing `tmp/pgcopyinsert-0.0.1.tar.gz` & `tmp/pgcopyinsert-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgcopyinsert-0.0.1.tar", last modified: Thu Apr  4 18:40:27 2024, max compression
+gzip compressed data, was "pgcopyinsert-0.1.0.tar", last modified: Fri May 10 18:47:35 2024, max compression
```

## Comparing `pgcopyinsert-0.0.1.tar` & `pgcopyinsert-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2024-04-04 17:56:48.000000 pgcopyinsert-0.0.1/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1047 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2661 2024-04-04 18:33:36.000000 pgcopyinsert-0.0.1/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      823 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2024-04-04 17:53:44.000000 pgcopyinsert-0.0.1/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      283 2024-04-04 18:18:12.000000 pgcopyinsert-0.0.1/src/pgcopyinsert/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      656 2024-04-04 17:28:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert/context.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      654 2024-04-04 17:36:50.000000 pgcopyinsert-0.0.1/src/pgcopyinsert/copy.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2993 2024-04-04 18:30:36.000000 pgcopyinsert-0.0.1/src/pgcopyinsert/copyinsert.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      613 2024-04-04 17:42:17.000000 pgcopyinsert-0.0.1/src/pgcopyinsert/insert.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      625 2024-04-04 17:24:48.000000 pgcopyinsert-0.0.1/src/pgcopyinsert/temp.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1047 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      439 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      146 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)       13 2024-04-04 18:40:27.000000 pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     1068 2024-04-04 19:22:24.000000 pgcopyinsert-0.1.0/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1025 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/PKG-INFO
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     3799 2024-05-10 18:46:44.000000 pgcopyinsert-0.1.0/README.md
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     1013 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/setup.cfg
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)       68 2024-04-04 19:22:25.000000 pgcopyinsert-0.1.0/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      260 2024-05-10 18:39:51.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/__init__.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      219 2024-05-08 17:17:01.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/drivers.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      857 2024-05-10 17:21:10.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/insert.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      520 2024-05-08 13:13:58.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/names.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      645 2024-05-08 17:13:13.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/temp.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1025 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/PKG-INFO
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      493 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/SOURCES.txt
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)        1 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/dependency_links.txt
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)        1 2024-04-09 14:12:13.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/not-zip-safe
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      134 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/requires.txt
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)       13 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/tests/
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     6488 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_copy.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      642 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_copyinsert.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     1820 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_insert.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      785 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_temp.py
```

### Comparing `pgcopyinsert-0.0.1/LICENSE` & `pgcopyinsert-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.0.1/PKG-INFO` & `pgcopyinsert-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgcopyinsert
-Version: 0.0.1
+Version: 0.1.0
 Summary: Functions for faster PostgreSQL bulk inserts by copying to temp table then inserting from temp table.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
@@ -13,18 +13,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: sqlalchemy
-Requires-Dist: psycopg2[binary]
-Requires-Dist: pandas
-Requires-Dist: polars
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: mypy>=0.910; extra == "testing"
 Requires-Dist: flake8>=3.9; extra == "testing"
 Requires-Dist: tox>=3.24; extra == "testing"
 Requires-Dist: pytest==6.2.5; extra == "testing"
 Requires-Dist: pytest-cov==2.12.1; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
+Requires-Dist: testing.postgresql; extra == "testing"
```

### Comparing `pgcopyinsert-0.0.1/README.md` & `pgcopyinsert-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,70 +6,99 @@
 
 ## Main Features
 Here are just a few of the things that pgcopyinsert does:
 
   - Copy CSV directly to database table
   - Create temp table based of database table columns (names and types, no constraints)
   - Copy CSV to temp table then insert records from temp table to target table
+  - Synchronous and Asynchronous copy and copyinsert functions
   - "ON CONFLICT DO NOTHING" and "ON CONFLICT DO UPDATE" insert options
   - 3X faster inserts for Pandas DataFrames
   - Polars DataFrame upserts
-
+  - Works with psycopg and psycopg2 synchronously
+  - Works with psycopg and asyncpg asychronously
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/pgcopyinsert
 
 ```sh
 # PyPI
 pip install pgcopyinsert
+
+# install with a PostgreSQL driver
+pip install pgcopyinsert[psycopg]
+pip install pgcopyinsert[psycopg2]
+pip install pgcopyinsert[asyncpg]
+
+# install with a PostgreSQL driver and pandas/polars
+pip install pgcopyinsert[psycopg, pandas]
+pip install pgcopyinsert[asyncpg, polars]
 ```
 
 ## Dependencies
+- [sqlalchemy](https://pypi.org/project/SQLAlchemy/)
+
+## Optional Dependencies
+- [psycopg](https://www.psycopg.org/psycopg3/)
 - [psycopg2](https://www.psycopg.org/docs/)
-- [sqlalchemy](https://pypi.org/project/SQLAlchemy/1.3.18/)
+- [asyncpg](https://magicstack.github.io/asyncpg/current/)
 - [polars](https://pola.rs)
 - [pandas](https://pandas.pydata.org/)
 
 # Example code
 ```sh
 import sqlalchemy as sa
 import pgcopyinsert as ci
 
 engine = sa.create_engine('postgresql+pyscopg2://scott:tiger@hostname/dbname')
 
 # Copy CSV directly to database table
 with open('data.csv', 'r') as csv_f:
-    ci.copy_csv(csv_f, 'table_name', 'table_name_temp', engine, schema='test')
+    with engine.connect() as connection:
+        ci.copy_csv(csv_f, 'table_name', 'table_name_temp', connection, schema='test')
+        connection.commit()
 
 # Create temp table based of database table columns (names and types, no constraints)
 meta = sa.MetaData()
 meta.reflect(engine)
 table = sa.Table('table_name', meta)
-temp_table = ci.create_temp_table_from_table(table, 'table_name_temp', meta)
+temp_table = ci.temp.create_temp_table_from_table(table, 'table_name_temp', meta)
 
 # Copy CSV to temp table then insert records from temp table to target table
 with open('data.csv', 'r') as csv_f:
-    ci.copyinsert_csv(csv_file, 'table_name_temp', 'table_name_temp', engine)
-
+    with engine.connect() as connection:
+        ci.copyinsert_csv(csv_file, 'table_name_temp', 'table_name_temp', connection)
+        connection.commit()
+        
 # "ON CONFLICT DO NOTHING" and "ON CONFLICT DO UPDATE" insert options
-on_conflict_do_nothing = ci.insert_from_table_stmt_ocdn
-on_conflict_do_update = ci.insert_from_table_stmt_ocdu
+on_conflict_do_nothing = ci.insert.insert_from_table_stmt_ocdn
+on_conflict_do_update = ci.insert.insert_from_table_stmt_ocdu
 
-with open('data.csv', 'r') as csv_f:
-    ci.copyinsert_csv(csv_file, 'table_name_temp', 'table_name_temp', engine, insert_function=on_conflict_do_nothing)
+with open('data.csv', 'r') as csv_f, :
+    with engine.connect() as connection:
+        ci.copyinsert_csv(csv_file, 'table_name_temp', 'table_name_temp', connection,
+                          insert_function=on_conflict_do_nothing, constraint='id')
+        connection.commit()
 
 with open('data.csv', 'r') as csv_f:
-    ci.copyinsert_csv(csv_file, 'table_name_temp', 'table_name_temp', engine, insert_function=on_conflict_do_update)
+    with engine.connect() as connection:
+        ci.copyinsert_csv(csv_file, 'table_name_temp', 'table_name_temp', connection,
+                          insert_function=on_conflict_do_update, constraint='id')
 
 # 3X faster inserts for Pandas DataFrames
 import pandas as pd
 
 df = pd.DataFrame({'x': range(1_000_000), 'y': range(1_000_000)})
-ci.copyinsert_dataframe(df, 'xy_table', 'xy_table_temp', engine)
+with engine.connect() as connection:
+    ci.copyinsert_dataframe(df, 'xy_table', 'xy_table_temp', connection)
+    connection.commit()
 
 # Polars DataFrame upserts
 import polars as pl
 
 df = pl.DataFrame({'x': range(1_000_000), 'y': range(1_000_000)})
-ci.copyinsert_polars(df, 'xy_table', 'xy_table_temp', engine, insert_function=on_conflict_do_update)
+with engine.connect() as connection:
+    ci.copyinsert_polars(df, 'xy_table', 'xy_table_temp', connection,
+                         insert_function=on_conflict_do_update, constraint='id')
+    connection.commit()
 ```
```

### Comparing `pgcopyinsert-0.0.1/src/pgcopyinsert/temp.py` & `pgcopyinsert-0.1.0/src/pgcopyinsert/temp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import typing as _t
 
-import sqlalchemy as sa
+import sqlalchemy as _sa
 
 
 def create_temp_table_from_table(
-    table: sa.Table,
+    table: _sa.Table,
     name: str,
-    meta: sa.MetaData,
+    meta: _sa.MetaData,
     columns: _t.Optional[list[str]] = None
-) -> sa.Table:
+) -> _sa.Table:
     column_names: list[str] = [] if columns is None else columns
-    temp_table = sa.Table(name, meta, prefixes=['TEMPORARY'])
+    temp_table = _sa.Table(name, meta, prefixes=['TEMPORARY'])
     for col in table.c:
         if columns is None or col.name in column_names:
-            temp_table.append_column(sa.Column(col.name, col.type))
+            temp_table.append_column(_sa.Column(col.name, col.type), replace_existing=True)
     return temp_table
-    
-    
+
+
 def create_table_stmt(
-    table: sa.Table,
-) -> sa.sql.ddl.CreateTable:
-    return sa.schema.CreateTable(table)
-    
+    table: _sa.Table,
+) -> _sa.sql.ddl.CreateTable:
+    return _sa.schema.CreateTable(table)
+
```

### Comparing `pgcopyinsert-0.0.1/src/pgcopyinsert.egg-info/PKG-INFO` & `pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgcopyinsert
-Version: 0.0.1
+Version: 0.1.0
 Summary: Functions for faster PostgreSQL bulk inserts by copying to temp table then inserting from temp table.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
@@ -13,18 +13,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: sqlalchemy
-Requires-Dist: psycopg2[binary]
-Requires-Dist: pandas
-Requires-Dist: polars
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: mypy>=0.910; extra == "testing"
 Requires-Dist: flake8>=3.9; extra == "testing"
 Requires-Dist: tox>=3.24; extra == "testing"
 Requires-Dist: pytest==6.2.5; extra == "testing"
 Requires-Dist: pytest-cov==2.12.1; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
+Requires-Dist: testing.postgresql; extra == "testing"
```

