# Comparing `tmp/hilcat-1.1.0.tar.gz` & `tmp/hilcat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilcat-1.1.0.tar", last modified: Fri Apr 19 02:16:15 2024, max compression
+gzip compressed data, was "hilcat-1.2.0.tar", last modified: Thu May  9 12:41:37 2024, max compression
```

## Comparing `hilcat-1.1.0.tar` & `hilcat-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.053067 hilcat-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-19 02:16:15.053067 hilcat-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-19 02:16:09.000000 hilcat-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.049067 hilcat-1.1.0/hilcat/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 02:16:14.000000 hilcat-1.1.0/hilcat/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.053067 hilcat-1.1.0/hilcat/db/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/relational.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.053067 hilcat-1.1.0/hilcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-19 02:16:15.000000 hilcat-1.1.0/hilcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 02:16:15.000000 hilcat-1.1.0/hilcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:16:15.000000 hilcat-1.1.0/hilcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-19 02:16:09.000000 hilcat-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:16:15.053067 hilcat-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:41:37.317727 hilcat-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-09 12:41:37.317727 hilcat-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-09 12:41:32.000000 hilcat-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:41:37.313727 hilcat-1.2.0/hilcat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 12:41:37.000000 hilcat-1.2.0/hilcat/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:41:37.317727 hilcat-1.2.0/hilcat/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/db/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/db/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37624 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/db/relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/db/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 12:41:32.000000 hilcat-1.2.0/hilcat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:41:37.317727 hilcat-1.2.0/hilcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-09 12:41:37.000000 hilcat-1.2.0/hilcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-09 12:41:37.000000 hilcat-1.2.0/hilcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:41:37.000000 hilcat-1.2.0/hilcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 12:41:32.000000 hilcat-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:41:37.317727 hilcat-1.2.0/setup.cfg
```

### Comparing `hilcat-1.1.0/PKG-INFO` & `hilcat-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilcat
-Version: 1.1.0
+Version: 1.2.0
 Summary: High Level Cache Tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/hilcat
 Description-Content-Type: text/x-rst
 
 ==========
 HiLCaT
@@ -26,14 +26,33 @@
 
 In some implements, :code:`scope` may be always :code:`None` and should be ignored, thus unique node determined only by :code:`key`.
 
 
 Init by different backends
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+auto backend
+^^^^^^^^^^^^^^^^^
+
+create a cache based on redis
+
+.. code-block:: python
+
+  from hilcat import Cache
+
+  cache = Cache.from_uri('redis://localhost:1458')
+
+create a cache based on sqlite
+
+.. code-block:: python
+
+  from hilcat import Cache
+
+  cache = Cache.from_uri('sqlite:///t.db')
+
 in memory cache
 ^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
   from hilcat import MemoryCache
 
@@ -119,79 +138,79 @@
   ])
 
 cache api
 ~~~~~~~~~~~~~~~~~~~~
 
 Assume there is a cache named :code:`cache`.
 
-exists
-^^^^^^^
+exists(key, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Test if a key exists in cache for certain scope.
 
 
-fetch
-^^^^^^^^^^^^^^
+fetch(key, default=None, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If key not exists, return default value.
 
 .. code-block:: python
 
   value = cache.fetch('one', 1, scope='a')
 
-set
-^^^^^^
+set(key, value, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
   cache.set('one', 1, scope='a')
 
-update
-^^^^^^^^
+update(key, value, scope=None, \*\*kwargs)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Same as method :code:`set`, but return value may diff in some implements.
 
-get
-^^^^^^
+get(key, func=None, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If key exists, just return value stored in cache;
 else if key not exists, calculate value and store to cache, the return value.
 
 .. code-block:: python
 
   value = cache.get('one', lambda: 1, scope='a')
 
-pop
-^^^^^
+pop(key, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Delete value of given key for certain scope.
 
-scopes
-^^^^^^^
+scopes()
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Get all scopes in the cache.
 
 May not supported for some implements.
 
-keys
-^^^^^^
+keys(scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Get all keys for certain scope.
 
 May not supported for some implements.
 
-load
-^^^^^^
+load(scopes=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Load scope data from persistence storage.
 
 Some implements may have no persistence storage, thus this method do nothing.
 
-backup
-^^^^^^
+backup(scopes=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Save scope data to persistence storage.
 
 Some implements may have no persistence storage, thus this method do nothing.
 
 Decorate a function
 ~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `hilcat-1.1.0/README.rst` & `hilcat-1.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,33 @@
 
 In some implements, :code:`scope` may be always :code:`None` and should be ignored, thus unique node determined only by :code:`key`.
 
 
 Init by different backends
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+auto backend
+^^^^^^^^^^^^^^^^^
+
+create a cache based on redis
+
+.. code-block:: python
+
+  from hilcat import Cache
+
+  cache = Cache.from_uri('redis://localhost:1458')
+
+create a cache based on sqlite
+
+.. code-block:: python
+
+  from hilcat import Cache
+
+  cache = Cache.from_uri('sqlite:///t.db')
+
 in memory cache
 ^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
   from hilcat import MemoryCache
 
@@ -111,79 +130,79 @@
   ])
 
 cache api
 ~~~~~~~~~~~~~~~~~~~~
 
 Assume there is a cache named :code:`cache`.
 
-exists
-^^^^^^^
+exists(key, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Test if a key exists in cache for certain scope.
 
 
-fetch
-^^^^^^^^^^^^^^
+fetch(key, default=None, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If key not exists, return default value.
 
 .. code-block:: python
 
   value = cache.fetch('one', 1, scope='a')
 
-set
-^^^^^^
+set(key, value, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
   cache.set('one', 1, scope='a')
 
-update
-^^^^^^^^
+update(key, value, scope=None, \*\*kwargs)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Same as method :code:`set`, but return value may diff in some implements.
 
-get
-^^^^^^
+get(key, func=None, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If key exists, just return value stored in cache;
 else if key not exists, calculate value and store to cache, the return value.
 
 .. code-block:: python
 
   value = cache.get('one', lambda: 1, scope='a')
 
-pop
-^^^^^
+pop(key, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Delete value of given key for certain scope.
 
-scopes
-^^^^^^^
+scopes()
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Get all scopes in the cache.
 
 May not supported for some implements.
 
-keys
-^^^^^^
+keys(scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Get all keys for certain scope.
 
 May not supported for some implements.
 
-load
-^^^^^^
+load(scopes=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Load scope data from persistence storage.
 
 Some implements may have no persistence storage, thus this method do nothing.
 
-backup
-^^^^^^
+backup(scopes=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Save scope data to persistence storage.
 
 Some implements may have no persistence storage, thus this method do nothing.
 
 Decorate a function
 ~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `hilcat-1.1.0/hilcat/core.py` & `hilcat-1.2.0/hilcat/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 Core code for the high level abstract cache.
 """
 
 from typing import (
     Any, Dict, List,
     Callable, Iterable,
     Hashable, Optional,
-    Type,
+    Type, Union, Sequence,
 )
 from abc import (
     ABC, abstractmethod,
 )
 import os
 import sys
+import json
 import inspect
 import pathlib
 import warnings
 import builtins
 import functools
+import urllib.parse
 
 def _create_fn(name: str, args: List[str], body: List[str], *,
                _globals: Dict[str, Any] = None,
                _locals: Dict[str, Any] = None,
                return_type: Optional[Type] = None):
     _globals = _globals or {}
     # Note that we mutate locals when exec() is called.  Caller
@@ -96,24 +98,27 @@
     def update(self, key: Any, value: Any, scope: Any = None, **kwargs) -> Any:
         """
         Update value for the given key.
         """
         # default is same as set
         return self.set(key, value, scope=scope, **kwargs)
 
-    def get(self, key: Any, func: Callable[[], Any] = None, scope: Any = None, **kwargs) -> Any:
+    def get(self, key: Any, func: Callable = None, func_args: Sequence[Any] = None,
+            func_kwargs: Dict[str, Any] = None, scope: Any = None, **kwargs) -> Any:
         """
         If func is None, it's equal to method `fetch()`.
         If func not None,
             get value from cache if key exists;
             else run the func and save value to the cache.
         """
         if func is None or self.exists(key, scope=scope):
             return self.fetch(key, scope=scope)
-        value = func()
+        func_args = func_args or []
+        func_kwargs = func_kwargs or {}
+        value = func(*func_args, **func_kwargs)
         self.set(key, value, scope=scope)
         return value
 
     @abstractmethod
     def pop(self, key: Any, scope: Any = None, **kwargs) -> Any:
         """
         Delete value for the given key.
@@ -211,14 +216,29 @@
         return wrap(f)
 
 class Cache(Storage, ABC):
     """
     An abstract cache interface.
     """
 
+    @classmethod
+    def from_uri(cls, uri: str, **kwargs) -> 'Cache':
+        """
+        Create a cache base on given backend.
+        Auto-detect backend engine.
+        Subclass should override this method.
+        """
+        r = urllib.parse.urlsplit(uri)
+        engine = BACKENDS.get(r.scheme, DEFAULT_BACKEND)
+        if engine is not None:
+            return engine.from_uri(uri, **kwargs)
+        if r.scheme:
+            raise ValueError(f"schema not given: {uri}")
+        raise ValueError(f"Unsupported backend: {r.scheme}")
+
     def load(self, scopes: Iterable[Any] = None, **kwargs):
         """
         Load scope data from persistence storage.
         """
 
     def backup(self, scopes: Iterable[Any] = None, **kwargs):
         """
@@ -228,14 +248,35 @@
         """
 
     def save(self, scopes: Iterable[Any] = None, **kwargs):
         # backup has no ambiguity, save is going to be deprecated
         warnings.warn("use backup() instead", DeprecationWarning)
         self.backup(scopes, **kwargs)
 
+# schema -> cache builder; to build a cache from uri
+BACKENDS: Dict[str, Type[Cache]] = {}
+DEFAULT_BACKEND: Optional[Type[Cache]] = None
+
+def register_backend(schema: str, cls: Type[Cache]):
+    """
+    Register a backend, then we can get create the cache by `Cache.from_uri()`.
+    """
+    if schema in BACKENDS:
+        warnings.warn(f"Backend {schema} already defined, it will be overwritten.")
+    BACKENDS[schema] = cls
+
+class RegistrableCache(Cache, ABC):
+    """
+    Subclasses are forced to implement the `from_uri` method.
+    """
+    @classmethod
+    @abstractmethod
+    def from_uri(cls, uri: str, **kwargs) -> Cache:
+        pass
+
 class NoOpCache(Cache):
     """
     A cache placeholder, used when all values are calculated currently but may need a cache some day.
     """
     def exists(self, key: Any, scope: Any = None, **kwargs) -> bool:
         return False
 
@@ -396,17 +437,19 @@
         """
         self.root_dir = root_dir
         self.suf = suf
 
     def _get_filepath(self, key: str, scope: str = None) -> str:
         return os.path.join(self.root_dir, scope or '', key + self.suf)
 
-    def keys(self, scope: Any = None) -> Iterable[str]:
+    def keys(self, scope: str = None) -> Iterable[str]:
         # find all files under the directory
         root = pathlib.Path(self.root_dir)
+        if scope:
+            root = root.joinpath(scope)
         for f in root.rglob("*" + self.suf):
             if f.is_file():
                 key = f.relative_to(root).as_posix()
                 if self.suf:
                     key = key[:-len(self.suf)]
                 yield key
 
@@ -416,14 +459,26 @@
         BinaryFileCache.__init__(self)
 
 class SimpleTextFileCache(SimpleLocalFileCache, TextFileCache):
     def __init__(self, root_dir: str, suf: str = '', encoding='utf-8'):
         SimpleLocalFileCache.__init__(self, root_dir, suf)
         TextFileCache.__init__(self, encoding)
 
+class SimpleJsonFileCache(SimpleTextFileCache):
+    def __init__(self, root_dir: str, suf: str = '.json', encoding='utf-8'):
+        super().__init__(root_dir, suf, encoding)
+
+    def _read_file(self, filepath: str) -> Union[dict, list]:
+        with open(filepath, encoding=self.encoding) as f:
+            return json.load(f)
+
+    def _write_file0(self, filepath: str, content: Union[dict, list]):
+        with open(filepath, 'w', encoding=self.encoding) as f:
+            json.dump(content, f)
+
 class MiddleCache(Cache, ABC):
     """
     A cache which has a persistent storage.
 
     The storage is also a cache but ignore scope.
     The key of the storage corresponds to the scope of this cache.
     """
```

### Comparing `hilcat-1.1.0/hilcat/db/__init__.py` & `hilcat-1.2.0/hilcat/db/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     FormatSqlBuilder,
     PyformatSqlBuilder,
     RelationalDbScopeConfig,
     RelationalDbCache,
 )
 from .sqlite import (
     SqliteSqlBuilder,
-    SqliteScopeConfig,
     SqliteCache,
 )
 try:
     from .postgresql import (
         PostgresqlBuilder,
         PostgresqlScopeConfig,
         PostgresqlCache,
```

### Comparing `hilcat-1.1.0/hilcat/db/mysql.py` & `hilcat-1.2.0/hilcat/db/mysql.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,68 @@
 # -*- coding: utf-8 -*-
 
 from typing import (
-    Dict, Any, Tuple,
+    Dict, Any, Tuple, Sequence,
+    Hashable, Union, Literal,
 )
+import warnings
 from abc import ABC, abstractmethod
 from .relational import (
     FormatSqlBuilder,
+    BaseRelationalDbCache,
     RelationalDbScopeConfig,
-    RelationalDbCache, Operation,
+    RelationalDbCache,
+    SingleTableCache,
+    Operation, ValueAdapter,
 )
 
 class MysqlSqlBuilder(FormatSqlBuilder):
 
+    default_column_type = 'text'
+
     def get_value_type(self, value: Any) -> str:
         return 's'
 
     def build_select_all_table_operation(self) -> Operation:
         return Operation(statement="SHOW TABLES")
 
     def build_select_table_columns_operation(self, table: str, filter_uniq=False) -> Operation:
         if filter_uniq:
             stmt = f"SHOW INDEX FROM {table} WHERE key_name = 'PRIMARY'"
         else:
             stmt = f"DESCRIBE {table}"
         return Operation(statement=stmt)
 
+    def get_column_name_from_result(self, result: Sequence[Any]) -> str:
+        # 4th is column name.
+        return result[4]
+
     def _gen_update_statement(self, config: 'MysqlScopeConfig', value: Dict[str, Any]) -> Tuple[str, bool]:
         first = ','.join(self.config_variable(name=k, order=i, value=v)
                          for i, (k, v) in enumerate(value.items(), 1))
         second = ','.join(f'{k}={self.config_variable(name=k, order=i, value=v)}'
                           for i, (k, v) in enumerate(value.items(), 1))
         return (f"INSERT INTO {config.table}({','.join(value.keys())})"
                 f" VALUES ({first})"
                 f" ON DUPLICATE KEY"
                 f" UPDATE {second}"), False
 
 class MysqlScopeConfig(RelationalDbScopeConfig):
-    def get_column_type(self, col: str) -> str:
-        return self.column_types.get(col, 'text')
+    def __init__(self, scope: Hashable, table: str = None, uniq_column: str = None,
+                 uniq_columns: Sequence[str] = ('id',), columns: Sequence[str] = ('data',),
+                 column_types: Dict[str, str] = None,
+                 value_adapter: Union[Literal['auto', 'default', 'single', 'tuple', 'list'], ValueAdapter] = 'auto',
+                 default_column_type: str = None):
+        warnings.warn("use RelationalDbScopeConfig instead", DeprecationWarning)
+        super().__init__(scope, table, uniq_column, uniq_columns, columns, column_types, value_adapter,
+                         default_column_type)
 
-class BaseBackend(RelationalDbCache, ABC):
+class BaseBackend(BaseRelationalDbCache, ABC):
     """
-    Use mysql database as backend.
+    Base abstract class for mysql backend.
     """
     paramstyle = 'format'
     sql_builder = MysqlSqlBuilder()
 
     @abstractmethod
     def _connect_db0(self, **kwargs):
         """
@@ -57,32 +74,33 @@
         kwargs = dict(connect_args or {})
         if database is not None:
             # TODO 2023/10/12  parse uri
             import warnings
             warnings.warn("uri is ignored")
             return self._connect_db0(**kwargs)
 
-    def _get_unique_column_name(self, table: str) -> str:
-        operation = self.sql_builder.build_select_table_columns_operation(table, filter_uniq=True)
-        columns = self._execute(operation, fetch_size='all')
-        if len(columns) != 1:
-            raise ValueError(f"There should be exactly one uniq column, but {len(columns)} has given.")
-        # 4th is column name.
-        return columns[0][4]
-
-class PymysqlBackend(BaseBackend):
+class PymysqlBackend(BaseBackend, ABC):
     def _connect_db0(self, **kwargs):
         import pymysql
         return pymysql.connect(**kwargs)
 
-class MysqlConnectorBackend(BaseBackend):
+class MysqlConnectorBackend(BaseBackend, ABC):
     def _connect_db0(self, **kwargs):
         import mysql.connector
         return mysql.connector.connect(**kwargs)
 
 try:
     import pymysql
-    MysqlCache = PymysqlBackend
+    BaseMysqlCache = PymysqlBackend
 except ImportError:
     import mysql.connector
-    MysqlCache = MysqlConnectorBackend
+    BaseMysqlCache = MysqlConnectorBackend
 
+class MysqlCache(BaseMysqlCache, RelationalDbCache):
+    """
+    Use a mysql database as backend.
+    """
+
+class MysqlSingleTableCache(BaseMysqlCache, SingleTableCache):
+    """
+    Use one table of mysql as backend.
+    """
```

### Comparing `hilcat-1.1.0/hilcat/db/relational.py` & `hilcat-1.2.0/hilcat/db/relational.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # -*- coding: utf-8 -*-
 
 """
 Relational database can be used as a cache or a persistence storage.
 Actually, implement a cache is enough.
 """
 
+import collections
 from typing import (
     Any, Iterable, Dict,
-    List, Type,
+    List, Type, Optional,
     Sequence, Callable,
     Literal, Union,
     Tuple, Hashable,
 )
+import re
 from abc import ABC, abstractmethod
 from types import ModuleType
 import dataclasses
-from ..core import Cache
+import warnings
+from ..core import RegistrableCache
+
 
 _FETCH_SIZE_TYPE = Union[Literal['one', 'all'], int]
 _EXECUTE_PARAM_TYPE = Union[Sequence[Any], Dict[str, Any]]
-_KEY_TYPE = Union[str, int]
+_COLUMN_VALUE_TYPE = Union[str, int]
+_KEY_TYPE = Union[_COLUMN_VALUE_TYPE, Sequence[_COLUMN_VALUE_TYPE]]
+
 
+# cache data format may diff from db api, we need an adapter to bridging
 class ValueAdapter(ABC):
     """
     Method `build_column_values` and `parse_column_values` should be reversed one-to-one mapping.
     That is to say:
         parse_column_values(build_column_values(x)) == x
         build_column_values(parse_column_values(x)) == x
     """
@@ -75,81 +82,102 @@
 
     def build_column_values(self, value: Sequence[Any]) -> Dict[str, Any]:
         return dict(zip(self.cols, value))
 
     def parse_column_values(self, value: Dict[str, Any]) -> Sequence[Any]:
         return self.return_type(map(value.get, self.cols))
 
+
 @dataclasses.dataclass
-class RelationalDbScopeConfig:
-    scope: Hashable
-    table: str = None
-    uniq_column: str = 'id'     # unique column to identify rows
-    columns: Sequence[str] = ('data', )
-    columns_with_id: List[str] = dataclasses.field(init=False)
+class Operation:
+    """
+    define an operation for execute() or executemany()
+    """
+    statement: str       # arg operation for cursor.execute()
+    parameters: _EXECUTE_PARAM_TYPE = dataclasses.field(default_factory=list)  # arg parameters for cursor.execute()
 
-    # if column not specified here, type should be str
-    column_types: Dict[str, str] = dataclasses.field(default_factory=dict)
+    # many statements in template or not, if True, use cursor.executemany() instead of cursor.execute()
+    many: bool = False
 
-    # convert value when fetch and set
-    value_adapter: Union[Literal['auto', 'default', 'single', 'tuple', 'list'], ValueAdapter] = 'auto'
 
-    def _check_value_adapter(self, adapter) -> ValueAdapter:
+class BaseTableConfig:
+    def __init__(self, table: str,
+                 uniq_columns: Sequence[str] = ('id',),
+                 columns: Sequence[str] = ('data',),
+                 column_types: Dict[str, str] = None,
+                 value_adapter: Union[Literal['auto', 'default', 'single', 'tuple', 'list'], ValueAdapter] = 'auto',
+                 default_column_type: str = None):
+        """
+        :param table:
+        :param uniq_columns:    unique columns to identify rows
+        :param columns:         columns to select when invoke `cache.fetch()`
+        :param column_types:    if column not specified here, type should be str
+        :param value_adapter:   convert value when fetch and set
+        :param default_column_type:     if column type not specified, use this value as default
+        """
+        self.table = table
+        self.columns = columns
+        self.column_types = dict(column_types or {})
+        self.default_column_type = default_column_type
+        if isinstance(uniq_columns, str):
+            self.uniq_columns = (uniq_columns,)
+        else:
+            self.uniq_columns = uniq_columns
+        if not self.uniq_columns:
+            raise ValueError("uniq_columns cannot be empty.")
+        self.columns_with_id = [x for x in self.uniq_columns if x not in self.columns] + list(self.columns)
+        self.value_adapter = self._check_value_adapter(value_adapter, columns)
+
+    @staticmethod
+    def _check_value_adapter(adapter, columns: Sequence[str]) -> ValueAdapter:
         if adapter == 'auto':
-            if len(self.columns) == 1:
-                return SingleAdapter(self.columns[0])
+            if len(columns) == 1:
+                return SingleAdapter(columns[0])
             return DefaultAdapter()
         elif adapter == 'default':
             return DefaultAdapter()
         elif adapter == 'single':
-            if len(self.columns) != 1:
+            if len(columns) != 1:
                 raise ValueError(f"columns length should be 1 when value_adapter is 'single'.")
-            return SingleAdapter(self.columns[0])
+            return SingleAdapter(columns[0])
         elif adapter == 'tuple':
-            return SequenceAdapter(self.columns, return_type=tuple)
+            return SequenceAdapter(columns, return_type=tuple)
         elif adapter == 'list':
-            return SequenceAdapter(self.columns, return_type=list)
+            return SequenceAdapter(columns, return_type=list)
 
         if isinstance(adapter, ValueAdapter):
             return adapter
 
         if isinstance(adapter, str):
             msg = f"Unexpected value_adapter: {adapter}"
         else:
             msg = f"Unexpected value_adapter type: {type(adapter)}"
         raise ValueError(msg)
 
-    def __post_init__(self):
-        if self.uniq_column in self.columns:
-            self.columns_with_id = list(self.columns)
-        else:
-            self.columns_with_id = [self.uniq_column] + list(self.columns)
-
-        if not self.table:
-            if not isinstance(self.scope, str):
-                raise ValueError("Arg scope must be a str when table not given.")
-            self.table = self.scope
-
-        self.value_adapter = self._check_value_adapter(self.value_adapter)
-
     def get_column_type(self, col: str) -> str:
-        # this method should be overwritten for certain database
-        return self.column_types.get(col, 'text')
+        return self.column_types.get(col, self.default_column_type)
 
-@dataclasses.dataclass
-class Operation:
-    """
-    define an operation for execute() or executemany()
-    """
-    statement: str       # arg operation for cursor.execute()
-    parameters: _EXECUTE_PARAM_TYPE = dataclasses.field(default_factory=list)  # arg parameters for cursor.execute()
+    @staticmethod
+    def normalize_columns_values(value: Any, columns: Sequence[str]) -> Sequence[Any]:
+        n = len(columns)
+        if n > 1:
+            if not isinstance(value, (list, tuple)):
+                raise ValueError(f"value should be a list or tuple, got {type(value)}")
+            m = len(value)
+            if m != n:
+                raise ValueError(f"value size should be {n}, but got {m}")
+            return value
+        else:
+            return [value]
+
+    def normalize_uniq_column_values(self, key: Any) -> Sequence[Any]:
+        return self.normalize_columns_values(key, self.uniq_columns)
 
-    # many statements in template or not, if True, use cursor.executemany() instead of cursor.execute()
-    many: bool = False
 
+# sql syntax may diff for different db, each backend should implement it's sql_builder
 class SqlBuilder(ABC):
     """
     Build select, update, delete sql for relational database.
     It's used by relational cache to manipulate data.
     """
 
     def build_select_all_table_operation(self) -> Operation:
@@ -164,71 +192,93 @@
         Generate sql to select all columns for given table.
         Column name as first selected result.
         :param table:           the queried table
         :param filter_uniq:     return only id column
         """
         raise NotImplementedError()
 
+    def get_column_name_from_result(self, result: Sequence[Any]) -> str:
+        """
+        Get column name from result of operation generated by `build_select_table_columns_operation()`.
+        """
+        # assume first result is column name.
+        return result[0]
+
     @abstractmethod
-    def build_create_table_operation(self, *configs: RelationalDbScopeConfig, check_exists=True):
+    def build_create_table_operation(self, *configs: BaseTableConfig, check_exists=True):
         """
         Generate sql to create a table.
         """
 
     @abstractmethod
-    def build_select_operation(self, config: RelationalDbScopeConfig, key: _KEY_TYPE = None, limit: int = -1,
-                               select_columns: Sequence[str] = None) -> Operation:
+    def build_select_operation(self, config: BaseTableConfig, key: Sequence[Any] = None, limit: int = -1,
+                               select_columns: Sequence[str] = None, distinct=False) -> Operation:
         """
         Generate sql to select row for given key.
         :param config:          scope configuration
         :param key:             uniq key for the row, maybe `None` to select all rows in the table
         :param limit:           limit number
         :param select_columns:  columns to be selected, if not set, select all in config
+        :param distinct:        whether distinct select columns
         """
 
     @abstractmethod
-    def build_update_operation(self, config: RelationalDbScopeConfig,
-                               key: _KEY_TYPE, value: Dict[str, Any]) -> Operation:
+    def build_update_operation(self, config: BaseTableConfig, key: Sequence[Any], value: Dict[str, Any]) -> Operation:
         """
         Generate sql to update or insert row for given key with given value.
         :param config:      scope configuration
         :param key:         uniq key for the row
         :param value:       column values for given uniq key
         """
 
     @abstractmethod
-    def build_delete_operation(self, config: RelationalDbScopeConfig, key: _KEY_TYPE = None) -> Operation:
+    def build_delete_operation(self, config: BaseTableConfig, key: Sequence[Any] = None) -> Operation:
         """
         Generate sql to delete row for given key.
         :param config:      scope configuration
         :param key:         uniq key for the row, maybe `None` to delete all rows in the table, be careful
         """
 
 class SimpleSqlBuilder(SqlBuilder, ABC):
     """
     A simple implement of SqlBuilder.
     """
 
-    list_parameter = False      # pass parameters as a list
+    # whether to pass parameters as a list
+    list_parameter = False
+
+    # if column type not specified in the config, use this value as default
+    # should be overwritten for different backends
+    default_column_type = 'text'
+
+    def _get_column_type(self, col: str, config: BaseTableConfig) -> str:
+        return config.get_column_type(col) or self.default_column_type
+
+    def _gen_column_def(self, col: str, config: BaseTableConfig) -> str:
+        t = self._get_column_type(col, config)
+        s = f"{col} {t}"
+        # if col in config.uniq_columns:
+            # s += " UNIQUE"
+            # s += ' PRIMARY KEY'
+        return s
+
+    def _gen_column_defines(self, config: BaseTableConfig):
+        columns = [self._gen_column_def(x, config) for x in config.columns_with_id]
+        columns += [f" PRIMARY KEY ({','.join(config.uniq_columns)})"]
+        return ','.join(columns)
+
+    def _gen_create_table_sql(self, config: BaseTableConfig, check_exists=True) -> str:
+        sql = "CREATE TABLE"
+        if check_exists:
+            sql += " IF NOT EXISTS"
+        sql += f" {config.table} ({self._gen_column_defines(config)})"
+        return sql
 
-    def build_create_table_operation(self, *configs: RelationalDbScopeConfig, check_exists=True) -> Operation:
-        def gen_column_def(col: str, config: RelationalDbScopeConfig) -> str:
-            s = f"{col} {config.get_column_type(col)}"
-            if col == config.uniq_column:
-                s += ' PRIMARY KEY'
-            return s
-        def gen_column_defines(config: RelationalDbScopeConfig):
-            return ','.join(gen_column_def(x, config) for x in config.columns_with_id)
-        def gen_create_table_sql(config: RelationalDbScopeConfig) -> str:
-            sql = "CREATE TABLE"
-            if check_exists:
-                sql += " IF NOT EXISTS"
-            sql += f" {config.table} ({gen_column_defines(config)})"
-            return sql
-        lines = [gen_create_table_sql(x) + ";" for x in configs]
+    def build_create_table_operation(self, *configs: BaseTableConfig, check_exists=True) -> Operation:
+        lines = [self._gen_create_table_sql(x) + ";" for x in configs]
         return Operation(statement="\n".join(lines), many=len(configs) > 1)
 
     @abstractmethod
     def get_variable_placeholder(self, name: str = None, order: int = None, value: Any = None) -> str:
         """
         Get variable placeholder in operation template.
         :param name:                variable name, used for named and pyformat style
@@ -260,75 +310,87 @@
         """
         if self.list_parameter:
             if variable_names is not None:
                 return [variable_values[x] for x in variable_names]
             return list(variable_values.values())
         return variable_values
 
-    def build_select_operation(self, config: RelationalDbScopeConfig, key: _KEY_TYPE = None, limit: int = -1,
-                               select_columns: Sequence[str] = None) -> Operation:
+    def build_select_operation(self, config: BaseTableConfig, key: Sequence[Any] = None, limit: int = -1,
+                               select_columns: Sequence[str] = None, distinct=False) -> Operation:
         if select_columns is None:
             # only select configured columns; if id not configured, ignore it
             select_columns = config.columns
         elif isinstance(select_columns, str):
             select_columns = [select_columns]
-        stmt = f"SELECT {','.join(select_columns)} FROM {config.table}"
-        variable_values = {}
+        stmt = "SELECT"
+        if distinct:
+            stmt += f" DISTINCT"
+        stmt += f" {','.join(select_columns)} FROM {config.table}"
+        variable_values = collections.OrderedDict()
         if key is not None:
-            name = config.uniq_column
-            placeholder = self.config_variable(name=name, order=1, value=key, variable_mapping=variable_values)
-            stmt += f" WHERE {config.uniq_column} = {placeholder}"
+            assert len(config.uniq_columns) == len(key)
+            condition = []
+            for i, (name, k) in enumerate(zip(config.uniq_columns, key), 1):
+                placeholder = self.config_variable(name=name, order=i, value=k, variable_mapping=variable_values)
+                condition.append(f"{name} = {placeholder}")
+            condition = ' AND '.join(condition)
+            stmt += f" WHERE {condition}"
         if limit > 0:
             stmt += f" LIMIT {limit}"
         return Operation(statement=stmt, parameters=self.normalize_variable_values(variable_values))
 
-    def _gen_update_statement(self, config: RelationalDbScopeConfig, value: Dict[str, Any]) -> Tuple[str, bool]:
+    def _gen_update_statement(self, config: BaseTableConfig, value: Dict[str, Any]) -> Tuple[str, bool]:
         """
         Generate statement for Operation, data of uniq column have added to value.
         :return:    (statement, many or not)
         """
         # sql is writen based of syntax of sqlite, maybe is incapable with other database
         first = ','.join(self.config_variable(name=k, order=i, value=v)
                          for i, (k, v) in enumerate(value.items(), 1))
         second = ','.join(f'{k}={self.config_variable(name=k, order=i, value=v)}'
                           for i, (k, v) in enumerate(value.items(), 1))
         return (f"INSERT INTO {config.table}({','.join(value.keys())})"
                 f" VALUES ({first})"
-                f" ON CONFLICT({config.uniq_column}) DO UPDATE"
+                f" ON CONFLICT({','.join(config.uniq_columns)}) DO UPDATE"
                 f" SET {second}"), False
 
     def _gen_update_variables(self, value: Dict[str, Any]) -> Tuple[Dict[str, Any], Sequence[str]]:
         """
         Generate variable values and name list used when execute().
         :param value:   value with uniq column
         :return:    (variable_values, variable_name_list)
         """
         return value, list(value.keys()) * 2
 
-    def build_update_operation(self, config: RelationalDbScopeConfig,
-                               key: _KEY_TYPE, value: Dict[str, Any]) -> Operation:
-        # if uniq column not in value, add it
-        if config.uniq_column not in value:
-            value = dict(value)
-            value[config.uniq_column] = key
+    def build_update_operation(self, config: BaseTableConfig, key: Sequence[Any], value: Dict[str, Any]) -> Operation:
+        # add uniq column to value
+        assert len(config.uniq_columns) == len(key)
+        value = dict(value)
+        for name, k in zip(config.uniq_columns, key):
+            value[name] = k
 
         # gen statement and parameters
         stmt, many = self._gen_update_statement(config=config, value=value)
         variable_values, variable_names = self._gen_update_variables(value)
         parameters = self.normalize_variable_values(variable_values, variable_names)
 
         return Operation(statement=stmt, parameters=parameters, many=many)
 
-    def build_delete_operation(self, config: RelationalDbScopeConfig, key: _KEY_TYPE = None) -> Operation:
+    def build_delete_operation(self, config: BaseTableConfig, key: Sequence[Any] = None) -> Operation:
         stmt = f"DELETE FROM {config.table}"
-        variable_values = {}
+        variable_values = collections.OrderedDict()
         if key is not None:
-            placeholder = self.config_variable(name=config.uniq_column, order=1, value=key,
-                                               variable_mapping=variable_values)
-            stmt += f" WHERE {config.uniq_column} = {placeholder}"
+            assert len(config.uniq_columns) == len(key)
+            condition = []
+            for i, (name, k) in enumerate(zip(config.uniq_columns, key), 1):
+                placeholder = self.config_variable(name=name, order=1, value=k,
+                                                   variable_mapping=variable_values)
+                condition.append(f"{name} = {placeholder}")
+            condition = ' AND '.join(condition)
+            stmt += f" WHERE {condition}"
         return Operation(statement=stmt, parameters=self.normalize_variable_values(variable_values))
 
 class QmarkSqlBuilder(SimpleSqlBuilder):
 
     list_parameter = True
 
     def get_variable_placeholder(self, name: str = None, order: int = None, value: Any = None) -> str:
@@ -376,21 +438,16 @@
     "qmark": QmarkSqlBuilder(),
     "numeric": NumericSqlBuilder(),
     "named": NamedSqlBuilder(),
     "format": FormatSqlBuilder(),
     "pyformat": PyformatSqlBuilder(),
 }
 
-class RelationalDbCache(Cache, ABC):
-    """
-    Use a relational database as backend.
-    Each scope corresponds to a table, and each key corresponds to a row.
-    It's recommended to use a string as key, but other type such as int is also allowed.
-    """
 
+class BaseRelationalDbCache(RegistrableCache, ABC):
     # if given api_module, use the module to connect
     api_module: ModuleType
 
     # parameter marker format described in pep-0249
     paramstyle: Literal['qmark', 'numeric', 'named', 'format', 'pyformat']
 
     # how to build fetch, update and delete sql
@@ -416,87 +473,259 @@
         """
         Connect to a database, return a connection object described in pep-0249.
 
         If always given a connection when init, this method may never run.
         """
         return self.api_module.connect(database, **(connect_args or {}))
 
-    def __init__(self, connection=None, database: str = None, connect_args: Dict[str, Any] = None,
-                 scopes: List[RelationalDbScopeConfig] = None,
-                 new_scope_config: Callable[[str], RelationalDbScopeConfig] = None,
-                 all_table_as_scope=True):
+    @classmethod
+    def from_uri(cls, uri: str, **kwargs) -> 'BaseRelationalDbCache':
+        assert re.match(r'\w+://.+', uri), uri
+        schema, database = uri.split('://')
+        return cls(database=database, **kwargs)
+
+    def __init__(self, connection=None, database: str = None, connect_args: Dict[str, Any] = None):
         """
         Create a cache based on relational database.
         :param connection:          connection to the database
         :param database:            uri for the database
         :param connect_args:        custom connect args
-        :param scopes:              initialized scopes
-        :param new_scope_config:    when a new scope given, how to config it
-        :param all_table_as_scope:  if `True`, add all table in database to scopes
         """
         self.conn = connection or self.connect_db(database, connect_args)
         self.cursor = self.conn.cursor()
-        self._scopes = {}   # scope -> config
-        self._tables = {}   # table -> config, should correspond to _scopes
-        self._new_scope_config = new_scope_config
-        self._init_scopes(scopes=scopes, all_table_as_scope=all_table_as_scope)
 
     def close(self):
         self.cursor.close()
         self.conn.close()
 
-    def _add_scope(self, config: RelationalDbScopeConfig):
-        # scope and table should be uniq
-        if config.scope in self._scopes:
-            raise ValueError(f"duplicated scope: {config.scope}")
-        if config.table in self._tables:
-            raise ValueError(f"duplicated table: {config.table}")
-        self._scopes[config.scope] = config
-        self._tables[config.table] = config
-
-    def _create_table_if_not_exists(self, *scopes: RelationalDbScopeConfig):
+    def _create_table_if_not_exists(self, *scopes: BaseTableConfig):
         operations = [self.sql_builder.build_create_table_operation(config, check_exists=True)
                       for config in scopes]
         self._execute(*operations, cursor='new', commit=True)
 
+    def _fetch_data(self, cursor, size: _FETCH_SIZE_TYPE = None) -> Any:
+        if size is None:
+            size = 0
+        elif size == 'one':
+            size = 1
+        elif size == 'all':
+            size = -1
+        if not isinstance(size, int):
+            raise ValueError(f"Unexpected size type: {type(size)}")
+        if size == 0:
+            return None
+        elif size == 1:
+            return cursor.fetchone()
+        elif size < 0:
+            return cursor.fetchall()
+        else:
+            return cursor.fetchmany(size)
+
+    def _execute_many0(self, cursor, operation: Operation):
+        """
+        Some api not allow executemany(), in this case, overwrite this method.
+        """
+        cursor.executemany(operation.statement, operation.parameters)
+
+    def _execute(self, *operations: Union[str, Operation], cursor='new', auto_close_cursor=True,
+                 fetch_size: _FETCH_SIZE_TYPE = None, commit=False) -> Any:
+        """
+        Execute sql and fetch result.
+        :param operations:      sequence of operation, same as described in pep-0249
+        :param cursor:          if `None`, use global; if 'new', create a new cursor; else, use the given cursor
+        :param auto_close_cursor:   close cursor in the end
+        :param fetch_size:      how many rows should return
+        :param commit:          do commit to database or not
+        """
+        close_cursor = False
+        if cursor is None:
+            cursor = self.cursor
+        elif cursor == 'new':
+            cursor = self.conn.cursor()
+            close_cursor = auto_close_cursor
+        for operation in operations:
+            if isinstance(operation, str):
+                operation = Operation(statement=operation)
+            if operation.many:
+                self._execute_many0(cursor, operation)
+            else:
+                cursor.execute(operation.statement, operation.parameters)
+        result = self._fetch_data(cursor, size=fetch_size)
+        if commit:
+            self.conn.commit()
+        if close_cursor:
+            # close the cursor if it's created in this method
+            cursor.close()
+        return result
+
     def _get_all_table_names_in_db(self) -> List[str]:
         """
         Get all tables in the database, used when init scopes.
         """
         operation = self.sql_builder.build_select_all_table_operation()
         # assume first is table name
         return [x[0] for x in self._execute(operation, fetch_size='all')]
 
-    def _get_table_columns(self, table: str) -> List[Tuple[Any]]:
+    def _get_table_columns(self, table: str) -> List[Sequence[Any]]:
         """
         Get columns for given table.
         :return:    column names
         """
         operation = self.sql_builder.build_select_table_columns_operation(table)
         columns = self._execute(operation, fetch_size='all')
         return list(columns)
 
     def _get_table_column_names(self, table: str) -> List[str]:
         """
         Get column names for given table.
         """
         columns = self._get_table_columns(table)
-        # assume first result is column name.
-        return [x[0] for x in columns]
+        return [self.sql_builder.get_column_name_from_result(x) for x in columns]
 
-    def _get_unique_column_name(self, table: str) -> str:
+    def _get_unique_columns(self, table: str) -> List[Sequence[Any]]:
         """
-        Get uniq column name for given table.
+        Get uniq columns for given table.
         """
         operation = self.sql_builder.build_select_table_columns_operation(table, filter_uniq=True)
         columns = self._execute(operation, fetch_size='all')
+        return list(columns)
+
+    def _get_unique_column_names(self, table: str) -> List[str]:
+        """
+        Get uniq column names for given table.
+        """
+        columns = self._get_unique_columns(table)
+        return [self.sql_builder.get_column_name_from_result(x) for x in columns]
+
+    def _get_unique_column_name(self, table: str) -> str:
+        """
+        Get uniq column name for given table.
+        """
+        warnings.warn("Deprecated, use _get_unique_column_names() instead", DeprecationWarning)
+        columns = self._get_unique_column_names(table)
         if len(columns) != 1:
             raise ValueError(f"There should be exactly one uniq column, but {len(columns)} has given.")
-        # assume first result is column name.
-        return columns[0][0]
+        return columns[0]
+
+    def _exists(self, key: Sequence[Any], table: BaseTableConfig) -> bool:
+        """
+        Actual method to test if a key exists in the table.
+        :param key:         value of uniq columns
+        :param table:       table config
+        """
+        operation = self.sql_builder.build_select_operation(
+            config=table, key=key, limit=1,
+            select_columns=table.uniq_columns,
+        )
+        return self._execute(operation, fetch_size=1) is not None
+
+    def _fetch(self, key: Sequence[Any], table: BaseTableConfig, default: Any = None) -> Any:
+        """
+        Actual method to fetch data from table.
+        :param key:         value of uniq columns
+        :param table:       table config
+        :param default:     if select no data, return this value
+        """
+        operation = self.sql_builder.build_select_operation(
+            config=table, key=key, limit=1,
+            select_columns=table.columns,
+        )
+        row = self._execute(operation, fetch_size=1)
+        if row is None:
+            return default
+        value = dict(zip(table.columns, row))
+        return table.value_adapter.parse_column_values(value)
+
+    def _set(self, key: Sequence[Any], value: Any, table: BaseTableConfig) -> bool:
+        """
+        Actual method to update or insert row into table.
+        :param key:         value of uniq columns
+        :param value:       value of all other columns
+        :param table:       table config
+        """
+        value = table.value_adapter.build_column_values(value)
+        row = {}
+        for name, k in zip(table.uniq_columns, key):
+            if name in value and k != value[name]:
+                raise ValueError(f"column {name} key {k} is different from value {value[name]}")
+            row[name] = k
+        row.update((name, value[name]) for name in table.columns if name in value)
+        operation = self.sql_builder.build_update_operation(config=table, key=key, value=row)
+        self._execute(operation, cursor='new', auto_close_cursor=True, commit=True)
+        return True
+
+    def _pop(self, key: Sequence[Any], table: BaseTableConfig):
+        """
+        Actual method to remove row from table.
+        :param key:         value of uniq columns
+        :param table:       table config
+        """
+        operation = self.sql_builder.build_delete_operation(config=table, key=key)
+        self._execute(operation, cursor='new', auto_close_cursor=True, commit=True)
+
+
+class RelationalDbScopeConfig(BaseTableConfig):
+    def __init__(self, scope: Optional[Hashable], table: str = None,
+                 uniq_column: str = None,
+                 uniq_columns: Sequence[str] = ('id',),
+                 columns: Sequence[str] = ('data',),
+                 column_types: Dict[str, str] = None,
+                 value_adapter: Union[Literal['auto', 'default', 'single', 'tuple', 'list'], ValueAdapter] = 'auto',
+                 default_column_type: str = None):
+        self.scope = scope
+        if not table:
+            if not isinstance(scope, str):
+                raise ValueError("Arg scope must be a str when table not given.")
+            table = scope
+        if uniq_column:
+            warnings.warn("`uniq_column` is deprecated, use `uniq_columns` instead.", DeprecationWarning)
+            uniq_columns = (uniq_column,)
+        super().__init__(table, uniq_columns, columns, column_types, value_adapter, default_column_type)
+
+class RelationalDbCache(BaseRelationalDbCache, ABC):
+    """
+    Use a relational database as backend.
+    Each scope corresponds to a table, and each key corresponds to a row.
+    It's recommended to use a string as key, but other type such as int is also allowed.
+    """
+
+    @classmethod
+    def from_uri(cls, uri: str, **kwargs) -> 'RelationalDbCache':
+        assert re.match(r'\w+://.+', uri), uri
+        schema, database = uri.split('://')
+        return cls(database=database, **kwargs)
+
+    def __init__(self, connection=None, database: str = None, connect_args: Dict[str, Any] = None,
+                 scopes: List[RelationalDbScopeConfig] = None,
+                 new_scope_config: Callable[[str], RelationalDbScopeConfig] = None,
+                 all_table_as_scope=True):
+        """
+        Create a cache based on relational database.
+        :param connection:          connection to the database
+        :param database:            uri for the database
+        :param connect_args:        custom connect args
+        :param scopes:              initialized scopes
+        :param new_scope_config:    when a new scope given, how to config it
+        :param all_table_as_scope:  if `True`, add all table in database to scopes
+
+        """
+        super().__init__(connection, database, connect_args)
+        self._scopes = {}   # scope -> config
+        self._tables = {}   # table -> config, should correspond to _scopes
+        self._new_scope_config = new_scope_config
+        self._init_scopes(scopes=scopes, all_table_as_scope=all_table_as_scope)
+
+    def _add_scope(self, config: RelationalDbScopeConfig):
+        # scope and table should be uniq
+        if config.scope in self._scopes:
+            raise ValueError(f"duplicated scope: {config.scope}")
+        if config.table in self._tables:
+            raise ValueError(f"duplicated table: {config.table}")
+        self._scopes[config.scope] = config
+        self._tables[config.table] = config
 
     def _init_scopes(self, scopes: List[RelationalDbScopeConfig], all_table_as_scope: bool):
         # if some scopes have given, add to the scope mapper
         # if table not exists, create it
         if scopes:
             for config in scopes:
                 self._add_scope(config)
@@ -509,19 +738,19 @@
 
             # table should not bound to a scope, and should not be same as a scope, remove these tables
             table_names = [x for x in table_names if x not in self._tables and x not in self._scopes]
 
             # for retain tables, add to the cache
             for table in table_names:
                 columns = self._get_table_column_names(table)
-                uniq_column = self._get_unique_column_name(table)
+                uniq_columns = self._get_unique_column_names(table)
                 self._add_scope(RelationalDbScopeConfig(
                     scope=table,    # use table name as scope
                     table=table,
-                    uniq_column=uniq_column,     # uniq column as id
+                    uniq_columns=uniq_columns,     # uniq column as id
                     columns=columns,
                 ))
 
     def _get_scope_config(self, scope: str) -> RelationalDbScopeConfig:
         if scope in self._scopes:
             return self._scopes[scope]
         if not self._new_scope_config:
@@ -529,116 +758,138 @@
         config = self._new_scope_config(scope)
         if scope != config.scope:
             raise ValueError(f"conflict scope: {scope} {config.scope}")
         self._add_scope(config)
         self._create_table_if_not_exists(config)    # create table if not exists
         return config
 
-    def _fetch_data(self, cursor, size: _FETCH_SIZE_TYPE = None) -> Any:
-        if size is None:
-            size = 0
-        elif size == 'one':
-            size = 1
-        elif size == 'all':
-            size = -1
-        if not isinstance(size, int):
-            raise ValueError(f"Unexpected size type: {type(size)}")
-        if size == 0:
-            return None
-        elif size == 1:
-            return cursor.fetchone()
-        elif size < 0:
-            return cursor.fetchall()
-        else:
-            return cursor.fetchmany(size)
-
-    def _execute_many0(self, cursor, operation: Operation):
-        """
-        Some api not allow executemany(), in this case, overwrite this method.
-        """
-        cursor.executemany(operation.statement, operation.parameters)
-
-    def _execute(self, *operations: Union[str, Operation], cursor='new', auto_close_cursor=True,
-                 fetch_size: _FETCH_SIZE_TYPE = None, commit=False) -> Any:
-        """
-        Execute sql and fetch result.
-        :param operations:      sequence of operation, same as described in pep-0249
-        :param cursor:          if `None`, use global; if 'new', create a new cursor; else, use the given cursor
-        :param auto_close_cursor:   close cursor in the end
-        :param fetch_size:      how many rows should return
-        :param commit:          do commit to database or not
-        """
-        close_cursor = False
-        if cursor is None:
-            cursor = self.cursor
-        elif cursor == 'new':
-            cursor = self.conn.cursor()
-            close_cursor = auto_close_cursor
-        for operation in operations:
-            if isinstance(operation, str):
-                operation = Operation(statement=operation)
-            if operation.many:
-                self._execute_many0(cursor, operation)
-            else:
-                cursor.execute(operation.statement, operation.parameters)
-        result = self._fetch_data(cursor, size=fetch_size)
-        if commit:
-            self.conn.commit()
-        if close_cursor:
-            # close the cursor if it's created in this method
-            cursor.close()
-        return result
-
     def _check_key(self, key: _KEY_TYPE):
         if key is None:
             raise ValueError("Arg key should not be None.")
 
     def exists(self, key: _KEY_TYPE, scope: str = None, **kwargs) -> bool:
         self._check_key(key)
         config = self._get_scope_config(scope)
-        operation = self.sql_builder.build_select_operation(
-            config=config, key=key, limit=1,
-            select_columns=[config.uniq_column],
-        )
-        return self._execute(operation, fetch_size=1) is not None
+        key = config.normalize_uniq_column_values(key)
+        return self._exists(key, config)
 
     def fetch(self, key: _KEY_TYPE, default: Any = None, scope: Any = None, **kwargs) -> Any:
         self._check_key(key)
         config = self._get_scope_config(scope)
-        operation = self.sql_builder.build_select_operation(
-            config=config, key=key, limit=1,
-            select_columns=config.columns,
-        )
-        row = self._execute(operation, fetch_size=1)
-        if row is None:
-            return default
-        value = dict(zip(config.columns, row))
-        return config.value_adapter.parse_column_values(value)
+        key = config.normalize_uniq_column_values(key)
+        return self._fetch(key, config, default=default)
 
     def set(self, key: _KEY_TYPE, value: Any, scope: Any = None, **kwargs) -> bool:
         self._check_key(key)
         config = self._get_scope_config(scope)
-        value = config.value_adapter.build_column_values(value)
-        if config.uniq_column in value:
-            if key != value[config.uniq_column]:
-                raise ValueError(f"key {key} is different from value {value[config.uniq_column]}")
-            row = {name: value[name] for name in config.columns_with_id if name in value}
-        else:
-            row = {config.uniq_column: key}
-            row.update((name, value[name]) for name in config.columns if name in value)
-        operation = self.sql_builder.build_update_operation(config=config, key=key, value=row)
-        self._execute(operation, cursor='new', auto_close_cursor=True, commit=True)
-        return True
+        key = config.normalize_uniq_column_values(key)
+        return self._set(key, value, config)
 
     def pop(self, key: _KEY_TYPE, scope: str = None, **kwargs) -> None:
         self._check_key(key)
         config = self._get_scope_config(scope)
-        operation = self.sql_builder.build_delete_operation(config=config, key=key)
-        self._execute(operation, cursor='new', auto_close_cursor=True, commit=True)
+        key = config.normalize_uniq_column_values(key)
+        self._pop(key, config)
 
     def scopes(self) -> Iterable[str]:
         return self._scopes.keys()
 
     def keys(self, scope: str = None) -> Iterable[str]:
         config = self._get_scope_config(scope)
         operation = self.sql_builder.build_select_operation(config=config, key=None)
         return self._execute(operation, fetch_size='all', cursor='new')
+
+
+class SingleTableConfig(BaseTableConfig):
+    def __init__(self, table: str,
+                 scope_columns: Sequence[str] = ('scope',),
+                 key_columns: Sequence[str] = ('id',),
+                 columns: Sequence[str] = ('data',),
+                 column_types: Dict[str, str] = None,
+                 value_adapter: Union[Literal['auto', 'default', 'single', 'tuple', 'list'], ValueAdapter] = 'auto',
+                 default_column_type: str = None):
+        self.scope_columns = tuple(scope_columns)
+        self.key_columns = tuple(key_columns)
+        uniq_columns = self.scope_columns + self.key_columns
+        super().__init__(table, uniq_columns, columns, column_types, value_adapter, default_column_type)
+
+    def normalize_scope_column_values(self, scope: Any) -> Sequence[Any]:
+        return self.normalize_columns_values(scope, self.scope_columns)
+
+    def normalize_key_column_values(self, scope: Any) -> Sequence[Any]:
+        return self.normalize_columns_values(scope, self.key_columns)
+
+class SingleTableCache(BaseRelationalDbCache):
+    """
+    Use single table in the db as backend.
+    This is useful when data of different scopes stored in the same table.
+    """
+
+    @classmethod
+    def from_uri(cls, uri: str, **kwargs) -> 'SingleTableCache':
+        assert re.match(r'\w+://.+', uri), uri
+        schema, database = uri.split('://')
+        return cls(database=database, **kwargs)
+
+    def __init__(self, connection=None, database: str = None, connect_args: Dict[str, Any] = None,
+                 config: SingleTableConfig = None):
+        """
+        Create a cache based on relational database.
+        :param connection:          connection to the database
+        :param database:            uri for the database
+        :param connect_args:        custom connect args
+        :param config:              config columns for scope and uniq columns
+        """
+        super().__init__(connection, database, connect_args)
+        self.config = config
+
+    def _check_key(self, key: _KEY_TYPE, scope: _KEY_TYPE):
+        if key is None:
+            raise ValueError("Arg key should not be None.")
+        if scope is None:
+            raise ValueError("Arg scope should not be None.")
+
+    def _gen_uniq_column_values(self, key: _KEY_TYPE, scope: _KEY_TYPE) -> Sequence[Any]:
+        self._check_key(key, scope)
+        key = self.config.normalize_key_column_values(key)
+        scope = self.config.normalize_scope_column_values(scope)
+        return tuple(scope) + tuple(key)
+
+    def exists(self, key: _KEY_TYPE, scope: _KEY_TYPE = None, **kwargs) -> bool:
+        uniq_column_values = self._gen_uniq_column_values(key, scope)
+        return self._exists(uniq_column_values, self.config)
+
+    def fetch(self, key: _KEY_TYPE, default: Any = None, scope: _KEY_TYPE = None, **kwargs) -> Any:
+        uniq_column_values = self._gen_uniq_column_values(key, scope)
+        return self._fetch(uniq_column_values, self.config, default=default)
+
+    def set(self, key: _KEY_TYPE, value: Any, scope: _KEY_TYPE = None, **kwargs) -> Any:
+        uniq_column_values = self._gen_uniq_column_values(key, scope)
+        return self._set(uniq_column_values, value, self.config)
+
+    def pop(self, key: _KEY_TYPE, scope: _KEY_TYPE = None, **kwargs) -> Any:
+        uniq_column_values = self._gen_uniq_column_values(key, scope)
+        return self._pop(uniq_column_values, self.config)
+
+    def scopes(self) -> Iterable[Any]:
+        config = self.config
+        columns = config.scope_columns
+        operation = self.sql_builder.build_select_operation(config, select_columns=columns, distinct=True)
+        row = self._execute(operation, fetch_size='all')
+        if row is None:
+            return []
+        if len(columns) == 1:
+            return [x[0] for x in row]
+        return [tuple(x) for x in row]
+
+    def keys(self, scope: _KEY_TYPE = None) -> Iterable[Any]:
+        scope = self.config.normalize_scope_column_values(scope)
+        config = self.config
+        columns = config.key_columns
+        operation = self.sql_builder.build_select_operation(config, key=scope, select_columns=columns)
+        row = self._execute(operation, fetch_size='all')
+        if row is None:
+            return []
+        if len(columns) == 1:
+            return [x[0] for x in row]
+        return [tuple(x) for x in row]
+
```

### Comparing `hilcat-1.1.0/hilcat/es.py` & `hilcat-1.2.0/hilcat/es.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # -*- coding: utf-8 -*-
 
 from typing import (
     Any, Iterable,
     Dict,
 )
-from .core import Cache
+from .core import RegistrableCache
 import elasticsearch as es
 
-class ElasticSearchCache(Cache):
+class ElasticSearchCache(RegistrableCache):
     """
     Use elasticsearch as backend.
     Each scope corresponds to an index, and each key corresponds to a document.
     """
 
+    @classmethod
+    def from_uri(cls, uri: str, **kwargs) -> 'ElasticSearchCache':
+        if not uri.startswith('es://'):
+            raise ValueError(f"It's not a es uri: {uri}.")
+        connect_args = kwargs.copy()
+        connect_args['hosts'] = uri[5:]
+        return cls(connect_args=connect_args)
+
     def __init__(self, client: es.Elasticsearch = None, connect_args: Dict[str, Any] = None):
         """
         Create a cache based on elasticsearch.
         :param client:              es client
         :param connect_args:        args to create a client
         """
         self.client = client or es.Elasticsearch(**(connect_args or {}))
```

### Comparing `hilcat-1.1.0/hilcat/redis.py` & `hilcat-1.2.0/hilcat/redis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -*- coding: utf-8 -*-
 
 from typing import Any, Iterable, Union
 import redis
-from .core import Cache
+from .core import RegistrableCache
 
 _REDIS_KEY_TYPE = Union[str, bytes]
 
-class RedisCache(Cache):
+class RedisCache(RegistrableCache):
     """
     Use redis as backend.
     Ignore scope for all cache methods.
     """
 
+    @classmethod
+    def from_uri(cls, uri: str, **kwargs) -> 'RedisCache':
+        return cls(url=uri, **kwargs)
+
     def __init__(self, client: redis.Redis = None, url: str = None, host: str = None, port: int = None, db=0):
         if client is not None:
             self.client = client
         elif url is not None:
             self.client = redis.from_url(url)
         elif host is not None:
             self.client = redis.Redis(host=host, port=port, db=db)
```

### Comparing `hilcat-1.1.0/hilcat.egg-info/PKG-INFO` & `hilcat-1.2.0/hilcat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilcat
-Version: 1.1.0
+Version: 1.2.0
 Summary: High Level Cache Tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/hilcat
 Description-Content-Type: text/x-rst
 
 ==========
 HiLCaT
@@ -26,14 +26,33 @@
 
 In some implements, :code:`scope` may be always :code:`None` and should be ignored, thus unique node determined only by :code:`key`.
 
 
 Init by different backends
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+auto backend
+^^^^^^^^^^^^^^^^^
+
+create a cache based on redis
+
+.. code-block:: python
+
+  from hilcat import Cache
+
+  cache = Cache.from_uri('redis://localhost:1458')
+
+create a cache based on sqlite
+
+.. code-block:: python
+
+  from hilcat import Cache
+
+  cache = Cache.from_uri('sqlite:///t.db')
+
 in memory cache
 ^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
   from hilcat import MemoryCache
 
@@ -119,79 +138,79 @@
   ])
 
 cache api
 ~~~~~~~~~~~~~~~~~~~~
 
 Assume there is a cache named :code:`cache`.
 
-exists
-^^^^^^^
+exists(key, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Test if a key exists in cache for certain scope.
 
 
-fetch
-^^^^^^^^^^^^^^
+fetch(key, default=None, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If key not exists, return default value.
 
 .. code-block:: python
 
   value = cache.fetch('one', 1, scope='a')
 
-set
-^^^^^^
+set(key, value, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
   cache.set('one', 1, scope='a')
 
-update
-^^^^^^^^
+update(key, value, scope=None, \*\*kwargs)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Same as method :code:`set`, but return value may diff in some implements.
 
-get
-^^^^^^
+get(key, func=None, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If key exists, just return value stored in cache;
 else if key not exists, calculate value and store to cache, the return value.
 
 .. code-block:: python
 
   value = cache.get('one', lambda: 1, scope='a')
 
-pop
-^^^^^
+pop(key, scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Delete value of given key for certain scope.
 
-scopes
-^^^^^^^
+scopes()
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Get all scopes in the cache.
 
 May not supported for some implements.
 
-keys
-^^^^^^
+keys(scope=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Get all keys for certain scope.
 
 May not supported for some implements.
 
-load
-^^^^^^
+load(scopes=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Load scope data from persistence storage.
 
 Some implements may have no persistence storage, thus this method do nothing.
 
-backup
-^^^^^^
+backup(scopes=None)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Save scope data to persistence storage.
 
 Some implements may have no persistence storage, thus this method do nothing.
 
 Decorate a function
 ~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `hilcat-1.1.0/pyproject.toml` & `hilcat-1.2.0/pyproject.toml`

 * *Files identical despite different names*

