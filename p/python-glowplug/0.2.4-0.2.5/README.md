# Comparing `tmp/python_glowplug-0.2.4.tar.gz` & `tmp/python_glowplug-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glowplug-0.2.4.tar", max compression
+gzip compressed data, was "python_glowplug-0.2.5.tar", max compression
```

## Comparing `python_glowplug-0.2.4.tar` & `python_glowplug-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.4/LICENSE
--rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.4/README.md
--rw-r--r--   0        0        0      499 2024-05-10 21:10:27.221950 python_glowplug-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.4/src/glowplug/__init__.py
--rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.4/src/glowplug/base.py
--rw-r--r--   0        0        0     2600 2024-05-10 21:11:10.946316 python_glowplug-0.2.4/src/glowplug/mssql.py
--rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.4/src/glowplug/pg.py
--rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.4/src/glowplug/sqlite.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.5/LICENSE
+-rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.5/README.md
+-rw-r--r--   0        0        0      499 2024-05-10 21:17:44.071044 python_glowplug-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.5/src/glowplug/__init__.py
+-rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.5/src/glowplug/base.py
+-rw-r--r--   0        0        0     2635 2024-05-10 21:18:25.176417 python_glowplug-0.2.5/src/glowplug/mssql.py
+-rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.5/src/glowplug/pg.py
+-rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.5/src/glowplug/sqlite.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.5/PKG-INFO
```

### Comparing `python_glowplug-0.2.4/LICENSE` & `python_glowplug-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.4/README.md` & `python_glowplug-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.4/src/glowplug/base.py` & `python_glowplug-0.2.5/src/glowplug/base.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.4/src/glowplug/mssql.py` & `python_glowplug-0.2.5/src/glowplug/mssql.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         # Get a database-less path and the db name
         path, database = self._split_path()
         # Connect to the database-less path
         engine = create_async_engine(f"mssql+aioodbc://{path}")
         # Need to run this with autocommit=True to avoid a transaction error
         # See: https://stackoverflow.com/a/42008664
         async with engine.connect() as conn:
-            await conn.execute(
-                text(f"CREATE DATABASE {database}").execution_options(autocommit=True)
-            )
+            rc = await conn.get_raw_connection()
+            rc.driver_connection.autocommit = True
+            await conn.execute(text(f"CREATE DATABASE {database}"))
 
     @property
     def async_uri(self) -> str:
         """Connect with aioodbc."""
         return f"mssql+aioodbc://{self.path}"
 
     @property
```

### Comparing `python_glowplug-0.2.4/src/glowplug/pg.py` & `python_glowplug-0.2.5/src/glowplug/pg.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.4/src/glowplug/sqlite.py` & `python_glowplug-0.2.5/src/glowplug/sqlite.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.4/PKG-INFO` & `python_glowplug-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-glowplug
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Home-page: https://github.com/jnu/python-glowplug
 License: MIT
 Author: Joe Nudell
 Author-email: jnudell@hks.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

