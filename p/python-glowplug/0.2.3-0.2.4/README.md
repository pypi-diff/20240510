# Comparing `tmp/python_glowplug-0.2.3.tar.gz` & `tmp/python_glowplug-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glowplug-0.2.3.tar", max compression
+gzip compressed data, was "python_glowplug-0.2.4.tar", max compression
```

## Comparing `python_glowplug-0.2.3.tar` & `python_glowplug-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.3/LICENSE
--rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.3/README.md
--rw-r--r--   0        0        0      499 2024-05-10 20:33:49.374816 python_glowplug-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.3/src/glowplug/__init__.py
--rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.3/src/glowplug/base.py
--rw-r--r--   0        0        0     2596 2024-05-10 20:56:51.254691 python_glowplug-0.2.3/src/glowplug/mssql.py
--rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.3/src/glowplug/pg.py
--rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.3/src/glowplug/sqlite.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.4/LICENSE
+-rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.4/README.md
+-rw-r--r--   0        0        0      499 2024-05-10 21:10:27.221950 python_glowplug-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.4/src/glowplug/__init__.py
+-rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.4/src/glowplug/base.py
+-rw-r--r--   0        0        0     2600 2024-05-10 21:11:10.946316 python_glowplug-0.2.4/src/glowplug/mssql.py
+-rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.4/src/glowplug/pg.py
+-rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.4/src/glowplug/sqlite.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.4/PKG-INFO
```

### Comparing `python_glowplug-0.2.3/LICENSE` & `python_glowplug-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.3/README.md` & `python_glowplug-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.3/src/glowplug/base.py` & `python_glowplug-0.2.4/src/glowplug/base.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.3/src/glowplug/mssql.py` & `python_glowplug-0.2.4/src/glowplug/mssql.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,29 +29,29 @@
         engine = create_async_engine(f"mssql+aioodbc://{path}")
         async with engine.connect() as conn:
             # Check if the database exists
             result = await conn.execute(
                 text("SELECT name FROM sys.databases WHERE name = :db"),
                 {"db": database},
             )
-            row = await result.fetchone()
+            row = result.fetchone()
             return row is not None
 
     async def create(self) -> None:
         """Create the database."""
         # Get a database-less path and the db name
         path, database = self._split_path()
         # Connect to the database-less path
         engine = create_async_engine(f"mssql+aioodbc://{path}")
-        # Create a raw connection with autocommit on.
+        # Need to run this with autocommit=True to avoid a transaction error
         # See: https://stackoverflow.com/a/42008664
-        conn = await engine.raw_connection()
-        conn.driver_connection.autocommit = True
-        await conn.driver_connection.execute(f"CREATE DATABASE {database}")
-        conn.close()
+        async with engine.connect() as conn:
+            await conn.execute(
+                text(f"CREATE DATABASE {database}").execution_options(autocommit=True)
+            )
 
     @property
     def async_uri(self) -> str:
         """Connect with aioodbc."""
         return f"mssql+aioodbc://{self.path}"
 
     @property
```

### Comparing `python_glowplug-0.2.3/src/glowplug/pg.py` & `python_glowplug-0.2.4/src/glowplug/pg.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.3/src/glowplug/sqlite.py` & `python_glowplug-0.2.4/src/glowplug/sqlite.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.3/PKG-INFO` & `python_glowplug-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-glowplug
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Home-page: https://github.com/jnu/python-glowplug
 License: MIT
 Author: Joe Nudell
 Author-email: jnudell@hks.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

