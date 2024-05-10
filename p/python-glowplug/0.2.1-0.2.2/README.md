# Comparing `tmp/python_glowplug-0.2.1.tar.gz` & `tmp/python_glowplug-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glowplug-0.2.1.tar", max compression
+gzip compressed data, was "python_glowplug-0.2.2.tar", max compression
```

## Comparing `python_glowplug-0.2.1.tar` & `python_glowplug-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.1/LICENSE
--rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.1/README.md
--rw-r--r--   0        0        0      499 2024-05-10 20:09:09.267101 python_glowplug-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.1/src/glowplug/__init__.py
--rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.1/src/glowplug/base.py
--rw-r--r--   0        0        0     2094 2024-05-10 18:24:29.874971 python_glowplug-0.2.1/src/glowplug/mssql.py
--rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.1/src/glowplug/pg.py
--rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.1/src/glowplug/sqlite.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.2/LICENSE
+-rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.2/README.md
+-rw-r--r--   0        0        0      499 2024-05-10 20:30:31.034919 python_glowplug-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.2/src/glowplug/__init__.py
+-rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.2/src/glowplug/base.py
+-rw-r--r--   0        0        0     2381 2024-05-10 20:28:55.716437 python_glowplug-0.2.2/src/glowplug/mssql.py
+-rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.2/src/glowplug/pg.py
+-rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.2/src/glowplug/sqlite.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.2/PKG-INFO
```

### Comparing `python_glowplug-0.2.1/LICENSE` & `python_glowplug-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.1/README.md` & `python_glowplug-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.1/src/glowplug/base.py` & `python_glowplug-0.2.2/src/glowplug/base.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.1/src/glowplug/mssql.py` & `python_glowplug-0.2.2/src/glowplug/mssql.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 
 
 class MsSqlDriver(DbDriver):
     """Microsoft SQL Server database driver."""
 
     path: str
 
-    def __init__(self, path: str, **kwargs):
+    maintenance_db: str
+
+    def __init__(self, path: str, maintenance_db: str = "master", **kwargs):
         """Initialize the driver.
 
         Args:
             path (str): The path to connect to the database.
+            maintenance_db (str, optional): The database to connect to for maintenance. Defaults to "master".
         """
         super().__init__(**kwargs)
         self.path = path
+        self.maintenance_db = maintenance_db
 
     async def exists(self) -> bool:
         """Check if the database exists."""
         # Get a database-less path and the db name
         path, database = self._split_path()
         # Connect to the database-less path
         engine = create_async_engine(f"mssql+aioodbc://{path}")
@@ -52,10 +56,11 @@
 
     def _split_path(self) -> tuple[str, str]:
         """Extract the database name from the rest of the path."""
         # Split the path into everything before the / and after
         head, tail = self.path.split("/", 1)
         # Extract the database name from the tail
         database, query = tail.split("?", 1)
-        # Re-join the query to the beginning of the path
-        path = f"{head}/?{query}"
+        # Re-join the query to the beginning of the path, with the
+        # name of the maintenance database.
+        path = f"{head}/{self.maintenance_db}?{query}"
         return path, database
```

### Comparing `python_glowplug-0.2.1/src/glowplug/pg.py` & `python_glowplug-0.2.2/src/glowplug/pg.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.1/src/glowplug/sqlite.py` & `python_glowplug-0.2.2/src/glowplug/sqlite.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.1/PKG-INFO` & `python_glowplug-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-glowplug
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/jnu/python-glowplug
 License: MIT
 Author: Joe Nudell
 Author-email: jnudell@hks.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

