# Comparing `tmp/postgresql_lock-0.1.5.tar.gz` & `tmp/postgresql_lock-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgresql_lock-0.1.5.tar", max compression
+gzip compressed data, was "postgresql_lock-0.1.6.tar", max compression
```

## Comparing `postgresql_lock-0.1.5.tar` & `postgresql_lock-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgresql_lock-0.1.5/LICENSE
--rw-r--r--   0        0        0     3926 2023-09-05 16:22:20.944144 postgresql_lock-0.1.5/README.md
--rw-r--r--   0        0        0      347 2023-09-05 16:23:03.857155 postgresql_lock-0.1.5/postgresql_lock/__init__.py
--rw-r--r--   0        0        0     2451 2023-09-05 16:18:11.625934 postgresql_lock-0.1.5/postgresql_lock/asyncpg.py
--rw-r--r--   0        0        0      565 2023-09-05 16:18:11.625934 postgresql_lock-0.1.5/postgresql_lock/errors.py
--rw-r--r--   0        0        0     9707 2023-09-05 16:23:21.965578 postgresql_lock-0.1.5/postgresql_lock/lock.py
--rw-r--r--   0        0        0     2583 2023-09-05 16:18:11.625934 postgresql_lock-0.1.5/postgresql_lock/psycopg2.py
--rw-r--r--   0        0        0     3007 2023-09-05 16:18:11.629934 postgresql_lock-0.1.5/postgresql_lock/psycopg3.py
--rw-r--r--   0        0        0        0 2023-09-05 16:18:11.629934 postgresql_lock-0.1.5/postgresql_lock/py.typed
--rw-r--r--   0        0        0     2848 2023-09-05 16:18:11.629934 postgresql_lock-0.1.5/postgresql_lock/sqlalchemy.py
--rw-r--r--   0        0        0      550 2023-09-05 16:22:50.580844 postgresql_lock-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4723 1970-01-01 00:00:00.000000 postgresql_lock-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgresql_lock-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4044 2024-05-10 15:37:51.574848 postgresql_lock-0.1.6/README.md
+-rw-r--r--   0        0        0      347 2023-09-05 16:23:03.857155 postgresql_lock-0.1.6/postgresql_lock/__init__.py
+-rw-r--r--   0        0        0     2451 2023-09-05 16:18:11.625934 postgresql_lock-0.1.6/postgresql_lock/asyncpg.py
+-rw-r--r--   0        0        0      565 2023-09-05 16:18:11.625934 postgresql_lock-0.1.6/postgresql_lock/errors.py
+-rw-r--r--   0        0        0     9755 2024-05-10 15:21:39.731474 postgresql_lock-0.1.6/postgresql_lock/lock.py
+-rw-r--r--   0        0        0     2583 2023-09-05 16:18:11.625934 postgresql_lock-0.1.6/postgresql_lock/psycopg2.py
+-rw-r--r--   0        0        0     3021 2024-05-10 15:36:17.036935 postgresql_lock-0.1.6/postgresql_lock/psycopg3.py
+-rw-r--r--   0        0        0        0 2023-09-05 16:18:11.629934 postgresql_lock-0.1.6/postgresql_lock/py.typed
+-rw-r--r--   0        0        0     2848 2023-09-05 16:18:11.629934 postgresql_lock-0.1.6/postgresql_lock/sqlalchemy.py
+-rw-r--r--   0        0        0      550 2024-05-10 15:36:29.629191 postgresql_lock-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 postgresql_lock-0.1.6/PKG-INFO
```

### Comparing `postgresql_lock-0.1.5/LICENSE` & `postgresql_lock-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `postgresql_lock-0.1.5/README.md` & `postgresql_lock-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -171,14 +171,17 @@
 lock = Lock(conn, "shared-identifier", rollback_on_error=False)
 
 # do things with the lock
 ```
 
 ### Changelog
 
+- **0.1.6**
+  - Use int.from_bytes() to convert lock key into integer
+  - Fix: psygopg3 close() not being awaited bug
 - **0.1.5**
   - Rename package from postgres-lock to postgresql-lock
 - **0.1.4**
   - Add py.typed for mypy
 - **0.1.3**
   - Key can be any object
 - **0.1.2**
```

### Comparing `postgresql_lock-0.1.5/postgresql_lock/asyncpg.py` & `postgresql_lock-0.1.6/postgresql_lock/asyncpg.py`

 * *Files identical despite different names*

### Comparing `postgresql_lock-0.1.5/postgresql_lock/errors.py` & `postgresql_lock-0.1.6/postgresql_lock/errors.py`

 * *Files identical despite different names*

### Comparing `postgresql_lock-0.1.5/postgresql_lock/lock.py` & `postgresql_lock-0.1.6/postgresql_lock/lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,18 @@
             scope (str): Lock scope.
             shared (bool): Use a shared lock.
         """
         self.conn = conn
         self.interface = interface
         self.impl = self._load_impl()
         self.key = key
-        self.lock_id = int(
-            str(int(hashlib.sha1(str(key).encode("utf-8")).hexdigest(), 16))[:18]
+        self.lock_id = int.from_bytes(
+            hashlib.sha1(str(key).encode("utf-8")).digest()[:8],
+            byteorder="big",
+            signed=True,
         )
         self.rollback_on_error = rollback_on_error
         self.scope = scope
         self._locked = False
         self._ref_count = 0
         self._shared = shared
```

### Comparing `postgresql_lock-0.1.5/postgresql_lock/psycopg2.py` & `postgresql_lock-0.1.6/postgresql_lock/psycopg2.py`

 * *Files identical despite different names*

### Comparing `postgresql_lock-0.1.5/postgresql_lock/psycopg3.py` & `postgresql_lock-0.1.6/postgresql_lock/psycopg3.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         lock_func = lock.nonblocking_lock_func
 
     cursor = lock.conn.cursor()
 
     await cursor.execute(f"SELECT pg_catalog.{lock_func}({lock.lock_id})")
 
     result, *_ = await cursor.fetchone()
-    cursor.close()
+
+    await cursor.close()
 
     # lock function returns True/False in unblocking mode, and always None in blocking
     # mode
     return False if result is False else True
 
 
 def handle_error(lock: Lock, exc: BaseException) -> None:
@@ -119,10 +120,11 @@
         bool: True, if the lock was released, otherwise False.
     """
     cursor = lock.conn.cursor()
 
     await cursor.execute(f"SELECT pg_catalog.{lock.unlock_func}({lock.lock_id})")
 
     result, *_ = await cursor.fetchone()
-    cursor.close()
+
+    await cursor.close()
 
     return result
```

### Comparing `postgresql_lock-0.1.5/postgresql_lock/sqlalchemy.py` & `postgresql_lock-0.1.6/postgresql_lock/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `postgresql_lock-0.1.5/pyproject.toml` & `postgresql_lock-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgresql-lock"
-version = "0.1.5"
+version = "0.1.6"
 description = "Lock mechanism implemented with PostgreSQL advisory locks."
 license = "BSD-3-Clause"
 authors = ["Sean Kerr <sean@code-box.org>"]
 readme = "README.md"
 repository = "https://github.com/seankerr/py-postgresql-lock"
 keywords = ["postgresql", "postgres", "distributed", "lock"]
 packages = [{include = "postgresql_lock"}]
```

### Comparing `postgresql_lock-0.1.5/PKG-INFO` & `postgresql_lock-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgresql-lock
-Version: 0.1.5
+Version: 0.1.6
 Summary: Lock mechanism implemented with PostgreSQL advisory locks.
 Home-page: https://github.com/seankerr/py-postgresql-lock
 License: BSD-3-Clause
 Keywords: postgresql,postgres,distributed,lock
 Author: Sean Kerr
 Author-email: sean@code-box.org
 Requires-Python: >=3.7,<4.0
@@ -191,14 +191,17 @@
 lock = Lock(conn, "shared-identifier", rollback_on_error=False)
 
 # do things with the lock
 ```
 
 ### Changelog
 
+- **0.1.6**
+  - Use int.from_bytes() to convert lock key into integer
+  - Fix: psygopg3 close() not being awaited bug
 - **0.1.5**
   - Rename package from postgres-lock to postgresql-lock
 - **0.1.4**
   - Add py.typed for mypy
 - **0.1.3**
   - Key can be any object
 - **0.1.2**
```

