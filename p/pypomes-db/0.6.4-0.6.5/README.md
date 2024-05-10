# Comparing `tmp/pypomes_db-0.6.4.tar.gz` & `tmp/pypomes_db-0.6.5.tar.gz`

## Comparing `pypomes_db-0.6.4.tar` & `pypomes_db-0.6.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24791 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    23014 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    25165 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24804 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    23090 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.5/PKG-INFO
```

### Comparing `pypomes_db-0.6.4/src/pypomes_db/__init__.py` & `pypomes_db-0.6.5/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.4/src/pypomes_db/db_common.py` & `pypomes_db-0.6.5/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.4/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.5/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.4/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.5/src/pypomes_db/oracle_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = lob_table
 
     # make sure to have a temporary file
-    lob_file: Any = _db_assert_temp_file(temp_file)
+    lob_file: Path = _db_assert_temp_file(temp_file)
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # buid the query
     pks: str = ", ".join(pk_columns)
@@ -395,14 +395,16 @@
             target_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
+        if lob_file and lob_file.exists():
+            lob_file.unlink()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
             stmt=(f"{result} LOBs migrated, "
```

### Comparing `pypomes_db-0.6.4/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.5/src/pypomes_db/postgres_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,15 +433,15 @@
             target_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
-        if lob_file.exists():
+        if lob_file and lob_file.exists():
             lob_file.unlink()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
```

### Comparing `pypomes_db-0.6.4/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.5/src/pypomes_db/sqlserver_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = lob_table
 
     # make sure to have a temporary file
-    lob_file: Any = _db_assert_temp_file(temp_file)
+    lob_file: Path = _db_assert_temp_file(temp_file)
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # buid the query
     pks: str = ", ".join(pk_columns)
@@ -395,14 +395,16 @@
             target_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
+        if lob_file and lob_file.exists():
+            lob_file.unlink()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             stmt=(f"{result} LOBs migrated, "
```

### Comparing `pypomes_db-0.6.4/LICENSE` & `pypomes_db-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.4/pyproject.toml` & `pypomes_db-0.6.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.4"
+version = "0.6.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.4/PKG-INFO` & `pypomes_db-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.4
+Version: 0.6.5
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

