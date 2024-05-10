# Comparing `tmp/pytrivialsql-0.1.7.tar.gz` & `tmp/pytrivialsql-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.7.tar", last modified: Wed May  8 20:46:08 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.8.tar", last modified: Fri May 10 19:04:41 2024, max compression
```

## Comparing `pytrivialsql-0.1.7.tar` & `pytrivialsql-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.534484 pytrivialsql-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.7/LICENSE` & `pytrivialsql-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.7/PKG-INFO` & `pytrivialsql-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.7
+Version: 0.1.8
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.7/pyproject.toml` & `pytrivialsql-0.1.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.7/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.8/src/pytrivialsql/postgres.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,28 +59,38 @@
     def create(self, table_name, props):
         with self._conn.cursor() as cur:
             cur.execute(sql.create_q(table_name, props))
             self._commit()
             return True
 
     def select(
-        self, table_name, columns, where=None, order_by=None, limit=None, transform=None
+        self,
+        table_name,
+        columns,
+        distinct=None,
+        where=None,
+        order_by=None,
+        limit=None,
+        offset=None,
+        transform=None,
     ):
         try:
             with self._conn.cursor() as cur:
                 if columns is None:
                     columns = "*"
                 if type(columns) is str:
                     columns = [columns]
                 query, args = sql.select_q(
                     table_name,
                     columns,
                     where=where,
+                    distinct_on=distinct,
                     order_by=order_by,
                     limit=limit,
+                    offset=offset,
                     placeholder="%s",
                 )
                 cur.execute(query, args)
                 cols = [col.name for col in cur.description]
                 res = (dict(zip(cols, vals)) for vals in cur.fetchall())
                 if transform is not None:
                     return [transform(el) for el in res]
```

### Comparing `pytrivialsql-0.1.7/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.8/src/pytrivialsql/sql.py`

 * *Files 13% similar despite different names*

```diff
@@ -127,26 +127,41 @@
         tuple(vs),
     )
 
 
 def select_q(
     table_name,
     columns,
+    distinct=None,
+    distinct_on=None,
     where=None,
     join=None,
     order_by=None,
     limit=None,
     offset=None,
     placeholder=None,
 ):
+    assert (
+        distinct is None or distinct_on is None
+    ), "Only one of DISTINCT or DISTINCT ON can be passed"
     if placeholder is None:
         placeholder = "?"
     if type(columns) is str:
         columns = [columns]
-    query = f"SELECT {', '.join(columns)} FROM {table_name}"
+
+    d_key = "DISTINCT" if distinct else "DISTINCT ON"
+    d_cols = distinct or distinct_on
+    dist = ""
+    if d_cols:
+        if type(d_cols) is str:
+            dist = f" {d_key} ({d_cols})"
+        else:
+            dist = f" {d_key} ({', '.join(d_cols)})"
+
+    query = f"SELECT{dist} {', '.join(columns)} FROM {table_name}"
     args = ()
     if join is not None:
         query += join_to_string(join)
     if where is not None:
         where_str, where_args = where_to_string(where, placeholder)
         query += where_str
         args = where_args
```

### Comparing `pytrivialsql-0.1.7/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.8/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.7
+Version: 0.1.8
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.7/tests/test_postgres.py` & `pytrivialsql-0.1.8/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.7/tests/test_sql.py` & `pytrivialsql-0.1.8/tests/test_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,7 +215,47 @@
     def test_limit(self):
         self.assertEqual(
             sql.select_q(
                 "table_name", ["id", "prop", "propb"], where={"a": 1}, limit=2
             ),
             ("SELECT id, prop, propb FROM table_name WHERE a=? LIMIT 2", (1,)),
         )
+
+    def test_offset(self):
+        self.assertEqual(
+            sql.select_q(
+                "table_name", ["id", "prop", "propb"], where={"a": 1}, offset=5
+            ),
+            ("SELECT id, prop, propb FROM table_name WHERE a=? OFFSET 5", (1,)),
+        )
+
+    def test_distinct(self):
+        self.assertEqual(
+            sql.select_q(
+                "table_name", ["id", "prop", "propb"], where={"a": 1}, distinct="prop"
+            ),
+            ("SELECT DISTINCT (prop) id, prop, propb FROM table_name WHERE a=?", (1,)),
+        )
+        self.assertEqual(
+            sql.select_q(
+                "table_name",
+                ["id", "prop", "propb"],
+                where={"a": 1},
+                distinct_on="prop",
+            ),
+            (
+                "SELECT DISTINCT ON (prop) id, prop, propb FROM table_name WHERE a=?",
+                (1,),
+            ),
+        )
+        self.assertEqual(
+            sql.select_q(
+                "table_name",
+                ["id", "prop", "propb"],
+                where={"a": 1},
+                distinct_on=["prop", "propb"],
+            ),
+            (
+                "SELECT DISTINCT ON (prop, propb) id, prop, propb FROM table_name WHERE a=?",
+                (1,),
+            ),
+        )
```

### Comparing `pytrivialsql-0.1.7/tests/test_sqlite.py` & `pytrivialsql-0.1.8/tests/test_sqlite.py`

 * *Files identical despite different names*

