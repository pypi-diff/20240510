# Comparing `tmp/sqlexecx-0.1.0.tar.gz` & `tmp/sqlexecx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecx-0.1.0.tar", last modified: Sun May  5 01:41:08 2024, max compression
+gzip compressed data, was "sqlexecx-0.3.0.tar", last modified: Fri May 10 12:27:21 2024, max compression
```

## Comparing `sqlexecx-0.1.0.tar` & `sqlexecx-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-05 01:41:08.624506 sqlexecx-0.1.0/
--rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.1.0/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-05 01:41:08.623703 sqlexecx-0.1.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.1.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-05 01:41:08.624765 sqlexecx-0.1.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1328 2024-05-05 01:40:54.000000 sqlexecx-0.1.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-05 01:41:08.606921 sqlexecx-0.1.0/sqlexecx/
--rw-r--r--   0 summy      (501) staff       (20)     2468 2024-05-05 01:28:17.000000 sqlexecx-0.1.0/sqlexecx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.1.0/sqlexecx/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     8887 2024-05-04 09:44:00.000000 sqlexecx-0.1.0/sqlexecx/dialect.py
--rw-r--r--   0 summy      (501) staff       (20)    18625 2024-05-04 08:51:07.000000 sqlexecx-0.1.0/sqlexecx/exec.py
--rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.1.0/sqlexecx/loader.py
--rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.1.0/sqlexecx/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlexecx-0.1.0/sqlexecx/page_exec.py
--rw-r--r--   0 summy      (501) staff       (20)    15899 2024-05-04 09:35:22.000000 sqlexecx-0.1.0/sqlexecx/sql_exec.py
--rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.1.0/sqlexecx/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)    18462 2024-05-04 04:35:20.000000 sqlexecx-0.1.0/sqlexecx/table_exec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-05 01:41:08.621444 sqlexecx-0.1.0/sqlexecx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-05 01:41:08.000000 sqlexecx-0.1.0/sqlexecx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-05 01:41:08.000000 sqlexecx-0.1.0/sqlexecx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-05 01:41:08.000000 sqlexecx-0.1.0/sqlexecx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 04:37:35.000000 sqlexecx-0.1.0/sqlexecx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-05 01:41:08.000000 sqlexecx-0.1.0/sqlexecx.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-05 01:41:08.000000 sqlexecx-0.1.0/sqlexecx.egg-info/top_level.txt
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-05 01:41:08.622354 sqlexecx-0.1.0/test/
--rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.1.0/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.594502 sqlexecx-0.3.0/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.3.0/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 12:27:21.593293 sqlexecx-0.3.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.3.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-10 12:27:21.594796 sqlexecx-0.3.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1328 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.583775 sqlexecx-0.3.0/sqlexecx/
+-rw-r--r--   0 summy      (501) staff       (20)     2468 2024-05-05 01:28:17.000000 sqlexecx-0.3.0/sqlexecx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.3.0/sqlexecx/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     8887 2024-05-04 09:44:00.000000 sqlexecx-0.3.0/sqlexecx/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    18625 2024-05-04 08:51:07.000000 sqlexecx-0.3.0/sqlexecx/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.3.0/sqlexecx/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.3.0/sqlexecx/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     3231 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/sqlexecx/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    20095 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/sqlexecx/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.3.0/sqlexecx/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    18712 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/sqlexecx/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.590549 sqlexecx-0.3.0/sqlexecx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.591460 sqlexecx-0.3.0/test/
+-rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.3.0/test/test.py
```

### Comparing `sqlexecx-0.1.0/LICENSE` & `sqlexecx-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/PKG-INFO` & `sqlexecx-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.1.0
+Version: 0.3.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.     It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecx-0.1.0/README.rst` & `sqlexecx-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/setup.py` & `sqlexecx-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 setup(
     name='sqlexecx',
     packages=['sqlexecx'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.\
      It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.1.0',
+    version='0.3.0',
     install_requires=[
-        'sqlexecutorx>=0.6.0',
+        'sqlexecutorx>=0.8.0',
     ],
     url='https://gitee.com/summry/sqlexecx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
```

### Comparing `sqlexecx-0.1.0/sqlexecx/__init__.py` & `sqlexecx-0.3.0/sqlexecx/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/sqlexecx/constant.py` & `sqlexecx-0.3.0/sqlexecx/constant.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/sqlexecx/dialect.py` & `sqlexecx-0.3.0/sqlexecx/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/sqlexecx/exec.py` & `sqlexecx-0.3.0/sqlexecx/exec.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/sqlexecx/loader.py` & `sqlexecx-0.3.0/sqlexecx/loader.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/sqlexecx/log_support.py` & `sqlexecx-0.3.0/sqlexecx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/sqlexecx/sql_exec.py` & `sqlexecx-0.3.0/sqlexecx/sql_exec.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,109 +10,227 @@
 
     def __init__(self, sql: str, page_exec: PageExec):
         self.sql = sql
         self.page_exec = page_exec
 
     def query(self, *args, **kwargs):
         """
-        Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Execute select SQL and return list results(dict).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10).query('张三', 20)
+        [{'id': 3, 'name': '张三', 'age': 20}]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').page(1, 10).query(name='张三', age=20)
+        [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.page_exec.query(self.sql, *args, **kwargs)
 
     def select(self, *args, **kwargs):
         """
-        Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Execute select SQL and return unique result or list results(tuple).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10).select('张三', 20)
+        [(3, '张三', 20)]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').page(1, 10).select(name='张三', age=20)
+        [(3, '张三', 20)]
         """
         return self.page_exec.select(self.sql, *args, **kwargs)
 
     def do_query(self, *args):
         """
-        Execute select SQL and return list results(dict).
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+        Execute select SQL and return unique result or list results(tuple).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10).do_query('张三', 20)
+        [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.page_exec.do_query(self.sql, *args)
 
     def do_select(self, *args):
         """
-        Execute select SQL and return list results(dict).
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+        Execute select SQL and return unique result or list results(tuple).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10).do_select('张三', 20)
+        [(3, '张三', 20)]
         """
         return self.page_exec.do_select(self.sql, *args)
 
 
 class ParamPageExec:
 
     def __init__(self, sql_page_exec: SqlPageExec, *args, **kwargs):
         self.sql_page_exec = sql_page_exec
         self.args = args
         self.kwargs = kwargs
 
     def query(self):
+        """
+        Execute select SQL and return list results(dict).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 20).page(1, 10).query()
+        [{'id': 3, 'name': '张三', 'age': 20}]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).page(1, 10).query()
+        [{'id': 3, 'name': '张三', 'age': 20}]
+        """
         return self.sql_page_exec.query(*self.args, **self.kwargs)
 
     def select(self):
+        """
+        Execute select SQL and return unique result or list results(tuple).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 20).page(1, 10).select()
+        [(3, '张三', 20)]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).page(1, 10).select()
+        [(3, '张三', 20)]
+        """
         return self.sql_page_exec.select(*self.args, **self.kwargs)
 
 
 class Param:
 
     def __init__(self, sql_exec, *args, **kwargs):
         self.sql_exec = sql_exec
         self.args = args
         self.kwargs = kwargs
 
     def execute(self) -> int:
         """
-        sqlexecx.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).execute()
+        Execute sql return effected rowcount
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).execute()
+        1
+        >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').param(name='张三', age=20).execute()
+        1
         """
         return self.sql_exec.execute(*self.args, **self.kwargs)
 
     def save(self):
         """
-        sqlexecx.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).save('SELECT LAST_INSERT_ID()')
+        Insert data into table, return primary key.
+
+        :param args:
+        :return: Primary key
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).save()
+        3
+        >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').param(name='张三', age=20).save()
+        3
         """
         return self.sql_exec.save(*self.args, **self.kwargs)
 
     def save_select_key(self, select_key: str):
         """
-        sqlexecx.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).save('SELECT LAST_INSERT_ID()')
+        Insert data into table, return primary key.
+
+        :param select_key: sql for select primary key
+        :param args:
+        :return: Primary key
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> select_key = 'SELECT LAST_INSERT_ID()'
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 20).save_select_key(select_key)
+        3
+        >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').param(name='张三', age=20).save_select_key(select_key)
+        3
         """
         return self.sql_exec.save_select_key(select_key, *self.args, **self.kwargs)
 
     def get(self):
         """
-        sqlexecx.sql('SELECT count(1) FROM person WHERE name=? and age=? limit 1').param('张三', 18).get()
+        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+
+        MultiColumnsError: Expect only one column.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT count(1) FROM person WHERE name=? and age=? LIMIT 1').param('张三', 18).get()
+        1
+        >>> db.sql('SELECT count(1) FROM person WHERE name=:name and age=:age LIMIT 1').param(name='张三', age=20).get()
+        1
         """
         return self.sql_exec.get(*self.args, **self.kwargs)
 
     def select(self):
         """
-        sqlexecx.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).select()
+        Execute select SQL and return unique result or list results(tuple).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 18).select()
+        [(3, '张三', 20)]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).select()
+        [(3, '张三', 20)]
         """
         return self.sql_exec.select(*self.args, **self.kwargs)
 
     def select_one(self):
         """
-        sqlexecx.sql('SELECT * FROM person WHERE name=? and age=? limit 1').param('张三', 18).select_one()
+        Execute select SQL and return unique result(tuple), SQL contain 'limit'.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1').param('张三', 18).select_one()
+        (3, '张三', 20)
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age LIMIT 1').param(name='张三', age=20).select_one()
+        (3, '张三', 20)
         """
         return self.sql_exec.select_one(*self.args, **self.kwargs)
 
     def query(self):
         """
-        sqlexecx.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).query()
+        Execute select SQL and return list results(dict).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 20).query()
+        [{'id': 3, 'name': '张三', 'age': 20}]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).query()
+        [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.sql_exec.query(*self.args, **self.kwargs)
 
     def query_one(self):
         """
-        sqlexecx.sql('SELECT * FROM person WHERE name=? and age=? limit 1').param('张三', 18).query_one()
+        Execute select SQL and return unique result(dict), SQL contain 'limit'.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 20).query_one()
+        {'id': 3, 'name': '张三', 'age': 20}
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).query_one()
+        {'id': 3, 'name': '张三', 'age': 20}
         """
         return self.sql_exec.query_one(*self.args, **self.kwargs)
 
     def to_csv(self, file_name: str, delimiter=',', header=True, encoding='utf-8'):
         """
         Execute select SQL and sava as a csv file.
 
@@ -173,15 +291,14 @@
         --------
         >>> import sqlexecx as db
         >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').execute('张三', 20)
         1
         >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').execute(name='张三', age=20)
         1
         """
-
         return self.exec.execute(self.sql, *args, **kwargs)
 
     def save(self, *args, **kwargs):
         """
         Insert data into table, return primary key.
 
         :param args:
@@ -191,15 +308,14 @@
         --------
         >>> import sqlexecx as db
         >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').save('张三', 20)
         3
         >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').save(name='张三', age=20)
         3
         """
-
         return self.exec.save_sql(self.sql, *args, **kwargs)
 
     def save_select_key(self, select_key: str, *args, **kwargs):
         """
         Insert data into table, return primary key.
 
         :param select_key: sql for select primary key
@@ -211,15 +327,14 @@
         >>> import sqlexecx as db
         >>> select_key = 'SELECT LAST_INSERT_ID()'
         >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').save_select_key(select_key, '张三', 20)
         3
         >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').save_select_key(select_key, name='张三', age=20)
         3
         """
-
         return self.exec.save_sql_select_key(select_key, self.sql, *args, **kwargs)
 
     def get(self, *args, **kwargs):
         """
         Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
 
         MultiColumnsError: Expect only one column.
@@ -274,15 +389,15 @@
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').query(name='张三', age=20)
         [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.exec.query(self.sql, *args, **kwargs)
 
     def query_one(self, *args, **kwargs):
         """
-        execute select SQL and return unique result(dict), SQL contain 'limit'.
+        Execute select SQL and return unique result(dict), SQL contain 'limit'.
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').query_one('张三', 20)
         {'id': 3, 'name': '张三', 'age': 20}
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').query_one(name='张三', age=20)
```

### Comparing `sqlexecx-0.1.0/sqlexecx/sql_support.py` & `sqlexecx-0.3.0/sqlexecx/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.1.0/sqlexecx/table_exec.py` & `sqlexecx-0.3.0/sqlexecx/table_exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -328,26 +328,33 @@
         self.exec = _exec
         self.table = table_name
 
     def insert(self, **kwargs):
         """
         Insert data into table, return effect rowcount.
 
-        :param kwargs: {name='张三', age=20}
-        return: Effect rowcount
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').insert(name='张三', age=20)
+        1
         """
         return self.exec.insert(self.table, **kwargs)
 
     def save(self, **kwargs):
         """
         Insert data into table, return primary key.
 
-        :param select_key: sql for select primary key
-        :param kwargs:
         :return: Primary key
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').save(name='张三', age=20)
+        3
         """
         return self.exec.save(self.table, **kwargs)
 
     def save_select_key(self, select_key: str, **kwargs):
         """
         Insert data into table, return primary key.
 
@@ -449,14 +456,22 @@
         return ColumnExec(self, *columns)
 
     def page(self, page_num=1, page_size=10) -> TablePageExec:
         return TablePageExec(self,  page_num, page_size)
 
 
 def table(table_name: str) -> TableExec:
+    """
+    Get a TableExec instance
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.table('person')
+    """
     table_name = table_name.strip()
     assert table_name, "Parameter 'table' must not be none"
     return TableExec(exec, table_name)
 
 
 def get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
```

### Comparing `sqlexecx-0.1.0/sqlexecx.egg-info/PKG-INFO` & `sqlexecx-0.3.0/sqlexecx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.1.0
+Version: 0.3.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.     It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecx-0.1.0/test/test.py` & `sqlexecx-0.3.0/test/test.py`

 * *Files identical despite different names*

