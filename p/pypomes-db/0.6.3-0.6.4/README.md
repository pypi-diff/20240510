# Comparing `tmp/pypomes_db-0.6.3.tar.gz` & `tmp/pypomes_db-0.6.4.tar.gz`

## Comparing `pypomes_db-0.6.3.tar` & `pypomes_db-0.6.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24802 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24791 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    23014 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.4/PKG-INFO
```

### Comparing `pypomes_db-0.6.3/src/pypomes_db/__init__.py` & `pypomes_db-0.6.4/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.3/src/pypomes_db/db_common.py` & `pypomes_db-0.6.4/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.3/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.4/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.3/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.4/src/pypomes_db/oracle_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,20 +106,21 @@
                                       require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
@@ -160,20 +161,21 @@
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.executemany(statement=insert_stmt,
                                parameters=insert_vals)
             result = len(insert_vals)
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
@@ -247,22 +249,23 @@
                 rows = cursor.fetchmany(batch_size)
 
         # commit the source and target transactions
         curr_conn.commit()
         if target_conn:
             target_conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
@@ -382,22 +385,23 @@
                     # no, increment the LOB migration counter
                     result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
@@ -462,20 +466,21 @@
                     cursor.execute(statement=update_stmt,
                                    parameters=(lob_data, *pk_vals))
                     lob_data = file.read(chunk_size)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             err_msg=err_msg,
             engine="oracle",
             errors=errors,
@@ -519,20 +524,21 @@
         with curr_conn.cursor() as cursor:
             cursor.execute(statement=exc_stmt,
                            parameters=bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
@@ -597,20 +603,21 @@
                             parameters=proc_vals)
 
             # retrieve the returned tuples
             result = list(cursor)
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
```

### Comparing `pypomes_db-0.6.3/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.4/src/pypomes_db/postgres_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,20 +106,21 @@
                                       require_max=require_max):
                 # yes, retrieve the returned tuples
                 result = list(cursor)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
@@ -166,49 +167,54 @@
             result = len(insert_vals)
         # commit the transaction
         curr_conn.commit()
     except ValueError as e:
         curr_conn.rollback()
         # is the exception ValueError("A string literal cannot contain NUL (0x00) characters.") ?
         if "contain NUL" in e.args[0]:
-            # yes, log the occurence, remove the NULLs, and try again
+            # yes, log the occurrence, remove the NULLs, and try again
             _db_log(logger=logger,
                     engine="postgres",
                     level=WARNING,
                     stmt=f"Found NULLs in values for {insert_stmt}")
             # search for NULLs in input data
-            clean_rows: list[tuple[int, list]] = []
+            cleaned_rows: list[tuple[int, list]] = []
             for inx, vals in enumerate(insert_vals):
-                replace: bool = False
-                clean_row: list = []
+                is_cleaned: bool = False
+                cleaned_row: list = []
                 for val in vals:
+                    # is 'val' a string containing NULLs ?
                     if isinstance(val, str) and val.count(chr(0)) > 0:
+                        # yes, clean it up and mark the row as cleaned
                         clean_val: str = val.replace(chr(0), "")
-                        replace = True
+                        is_cleaned = True
                     else:
                         clean_val: str = val
-                    clean_row.append(clean_val)
-                if replace:
-                    clean_rows.append((inx, clean_row))
-            # remove them
-            for clean_row in clean_rows:
-                insert_vals[clean_row[0]] = tuple(clean_row[1])
-            # insert the clean data
+                    cleaned_row.append(clean_val)
+                # has the row been cleaned ?
+                if is_cleaned:
+                    # yes, register it
+                    cleaned_rows.append((inx, cleaned_row))
+            # replace the cleaned rows
+            for cleaned_row in cleaned_rows:
+                insert_vals[cleaned_row[0]] = tuple(cleaned_row[1])
+            # bulk insert the cleaned data
             db_bulk_insert(errors=errors,
                            insert_stmt=insert_stmt,
                            insert_vals=insert_vals,
                            conn=conn,
                            logger=logger)
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
@@ -281,22 +287,23 @@
                 rows = cursor.fetchmany(batch_size)
 
         # commit the source and target transactions
         curr_conn.commit()
         if target_conn:
           target_conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
@@ -416,22 +423,23 @@
                     # no, increment the LOB migration counter
                     result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
         if lob_file.exists():
             lob_file.unlink()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
@@ -496,20 +504,21 @@
                     cursor.execute(statement=update_stmt,
                                    parameters=(Binary(lob_data), *pk_vals))
                     lob_data = file.read(chunk_size)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
@@ -553,20 +562,21 @@
         with curr_conn.cursor() as cursor:
             cursor.execute(query=f"{exc_stmt};",
                            vars=bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
@@ -610,20 +620,21 @@
             cursor.execute(query=proc_stmt,
                            argslist=proc_vals)
             # retrieve the returned tuples
             result = list(cursor)
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
```

### Comparing `pypomes_db-0.6.3/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.4/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,20 +103,21 @@
                                       require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list[Row] = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
@@ -160,20 +161,21 @@
                 cursor.executemany(insert_stmt, insert_vals)
                 result = len(insert_vals)
             except Exception:
                 conn.rollback()
                 raise
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
@@ -247,22 +249,23 @@
                 rows = cursor.fetchmany(batch_size)
 
         # commit the source and target transactions
         curr_conn.commit()
         if target_conn:
             target_conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
@@ -382,22 +385,23 @@
                     # no, increment the LOB migration counter
                     result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
@@ -459,20 +463,21 @@
                 while lob_data:
                     cursor.execute(update_stmt, (Binary(lob_data), *pk_vals))
                     lob_data = file.read(chunk_size)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
@@ -515,20 +520,21 @@
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(exc_stmt, bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
@@ -572,20 +578,21 @@
             cursor.execute(proc_stmt, proc_vals)
             # retrieve the returned tuples
             rows: list[Row] = cursor.fetchall()
             result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
-        curr_conn.rollback()
+        if curr_conn:
+            curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
-        if not conn:
+        if curr_conn and not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
```

### Comparing `pypomes_db-0.6.3/LICENSE` & `pypomes_db-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.3/pyproject.toml` & `pypomes_db-0.6.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.3"
+version = "0.6.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.3/PKG-INFO` & `pypomes_db-0.6.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.3
+Version: 0.6.4
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

