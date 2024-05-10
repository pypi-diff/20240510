# Comparing `tmp/pypomes_db-0.6.2.tar.gz` & `tmp/pypomes_db-0.6.3.tar.gz`

## Comparing `pypomes_db-0.6.2.tar` & `pypomes_db-0.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24802 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24802 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/PKG-INFO
```

### Comparing `pypomes_db-0.6.2/src/pypomes_db/__init__.py` & `pypomes_db-0.6.3/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.2/src/pypomes_db/db_common.py` & `pypomes_db-0.6.3/src/pypomes_db/db_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     return result
 
 
 def _db_assert_temp_file(temp_file: str | Path) -> Path:
 
     result: Path
     if temp_file is None:
-        result = Path(gettempdir(), str(uuid.uuid4()), ".bin")
+        result = Path(gettempdir(), str(uuid.uuid4()) + ".bin")
     elif isinstance(temp_file, str):
         result = Path(temp_file)
     else:
         result = temp_file
 
     return result
```

### Comparing `pypomes_db-0.6.2/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.3/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.2/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.3/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.2/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.3/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.2/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.3/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.2/LICENSE` & `pypomes_db-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.2/pyproject.toml` & `pypomes_db-0.6.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.2/PKG-INFO` & `pypomes_db-0.6.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.2
+Version: 0.6.3
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

