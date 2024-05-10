# Comparing `tmp/typedmongo-1.5.1.tar.gz` & `tmp/typedmongo-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.5.1.tar", last modified: Thu May  9 01:34:36 2024, max compression
+gzip compressed data, was "typedmongo-1.6.0.tar", last modified: Fri May 10 06:25:38 2024, max compression
```

## Comparing `typedmongo-1.5.1.tar` & `typedmongo-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-09 01:34:23.896498 typedmongo-1.5.1/LICENSE
--rw-r--r--   0        0        0     3808 2024-05-09 01:34:23.896498 typedmongo-1.5.1/README.md
--rw-r--r--   0        0        0     1441 2024-05-09 01:34:36.312549 typedmongo-1.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     6050 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     4229 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/sync.py
--rw-r--r--   0        0        0     5798 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/test_client.py
--rw-r--r--   0        0        0     3031 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/test_marshamallow.py
--rw-r--r--   0        0        0     4221 2024-05-09 01:34:23.896498 typedmongo-1.5.1/tests/test_table.py
--rw-r--r--   0        0        0      926 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/__init__.py
--rw-r--r--   0        0        0      926 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    10328 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9999 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     8420 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    10122 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5468 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/expressions.py
--rw-r--r--   0        0        0     9999 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/fields.py
--rw-r--r--   0        0        0      849 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1384 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/shortcuts.py
--rw-r--r--   0        0        0     1325 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/sync.py
--rw-r--r--   0        0        0     8420 2024-05-09 01:34:23.896498 typedmongo-1.5.1/typedmongo/table.py
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 06:25:25.596997 typedmongo-1.6.0/LICENSE
+-rw-r--r--   0        0        0     4654 2024-05-10 06:25:25.596997 typedmongo-1.6.0/README.md
+-rw-r--r--   0        0        0     1441 2024-05-10 06:25:38.117135 typedmongo-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     6352 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     4229 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/sync.py
+-rw-r--r--   0        0        0     6070 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/test_client.py
+-rw-r--r--   0        0        0     3031 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     4221 2024-05-10 06:25:25.596997 typedmongo-1.6.0/tests/test_table.py
+-rw-r--r--   0        0        0      926 2024-05-10 06:25:25.596997 typedmongo-1.6.0/typedmongo/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-10 06:25:25.596997 typedmongo-1.6.0/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    13074 2024-05-10 06:25:25.596997 typedmongo-1.6.0/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9999 2024-05-10 06:25:25.596997 typedmongo-1.6.0/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8420 2024-05-10 06:25:25.596997 typedmongo-1.6.0/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    12781 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5468 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9999 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/fields.py
+-rw-r--r--   0        0        0      849 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1384 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/shortcuts.py
+-rw-r--r--   0        0        0     1879 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/sync.py
+-rw-r--r--   0        0        0     8420 2024-05-10 06:25:25.600997 typedmongo-1.6.0/typedmongo/table.py
+-rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 typedmongo-1.6.0/PKG-INFO
```

### Comparing `typedmongo-1.5.1/LICENSE` & `typedmongo-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/pyproject.toml` & `typedmongo-1.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.5.1"
+version = "1.6.0"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.5.1/tests/asyncio/test_client.py` & `typedmongo-1.6.0/tests/asyncio/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,7 +204,14 @@
         mongo.EndsWith("R", case_sensitive=False),
     ],
 )
 async def test_shortcut(documents_id, shortcut):
     user = await User.objects.find_one(User.name == shortcut)
     assert user is not None
     assert user.name == "Aber"
+
+
+async def test_transaction(documents_id):
+    async with User.objects.use_session() as session:
+        await User.objects.update_many({}, {"$set": {"age": 20}})
+        await User.objects.delete_many(User.name == "Aber")
+        await User.objects.insert_one(User.load({"name": "Aber", "age": 18}))
```

### Comparing `typedmongo-1.5.1/tests/asyncio/test_table.py` & `typedmongo-1.6.0/tests/asyncio/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/tests/sync.py` & `typedmongo-1.6.0/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/tests/test_client.py` & `typedmongo-1.6.0/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,7 +204,14 @@
         mongo.EndsWith("R", case_sensitive=False),
     ],
 )
 def test_shortcut(documents_id, shortcut):
     user = User.objects.find_one(User.name == shortcut)
     assert user is not None
     assert user.name == "Aber"
+
+
+def test_transaction(documents_id):
+    with User.objects.use_session() as session:
+        User.objects.update_many({}, {"$set": {"age": 20}})
+        User.objects.delete_many(User.name == "Aber")
+        User.objects.insert_one(User.load({"name": "Aber", "age": 18}))
```

### Comparing `typedmongo-1.5.1/tests/test_expressions.py` & `typedmongo-1.6.0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/tests/test_marshamallow.py` & `typedmongo-1.6.0/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/tests/test_table.py` & `typedmongo-1.6.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/__init__.py` & `typedmongo-1.6.0/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/asyncio/__init__.py` & `typedmongo-1.6.0/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/asyncio/client.py` & `typedmongo-1.6.0/typedmongo/asyncio/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from __future__ import annotations
 
 import dataclasses
 import decimal
+from contextlib import asynccontextmanager
+from contextvars import ContextVar
 from typing import (
     TYPE_CHECKING,
     Any,
+    AsyncGenerator,
     AsyncIterable,
     Generic,
     Literal,
     Mapping,
     NoReturn,
     Optional,
     TypeAlias,
     TypeVar,
     overload,
 )
 
 from bson.codec_options import CodecOptions, TypeCodec, TypeRegistry
 from bson.decimal128 import Decimal128
+from pymongo.client_session import TransactionOptions
 from pymongo.operations import DeleteMany as MongoDeleteMany
 from pymongo.operations import DeleteOne as MongoDeleteOne
 from pymongo.operations import InsertOne as MongoInsertOne
 from pymongo.operations import ReplaceOne as MongoReplaceOne
 from pymongo.operations import UpdateMany as MongoUpdateMany
 from pymongo.operations import UpdateOne as MongoUpdateOne
+from pymongo.read_concern import ReadConcern
+from pymongo.read_preferences import _ServerMode
+from pymongo.write_concern import WriteConcern
 
 if TYPE_CHECKING:
+    from motor.motor_asyncio import AsyncIOMotorClientSession as MongoSession
     from motor.motor_asyncio import AsyncIOMotorCollection as MongoCollection
     from motor.motor_asyncio import AsyncIOMotorDatabase as MongoDatabase
     from pymongo.results import BulkWriteResult as MongoBlukWriteResult
     from pymongo.results import DeleteResult as MongoDeleteResult
     from pymongo.results import UpdateResult as MongoUpdateResult
 
     from .table import Table
@@ -112,32 +120,87 @@
         (order_by.field.field_name, order_by.order)
         if isinstance(order_by, OrderBy)
         else order_by
         for order_by in s
     ]
 )
 
+SESSION: ContextVar[Optional[MongoSession]] = ContextVar("session", default=None)
+
 
 class Objects(Generic[T]):
     def __init__(self, table: type[T]) -> None:
         self.table = table
 
     @property
     def collection(self) -> MongoCollection:
         return self.table.__collection__
 
+    @asynccontextmanager
+    async def use_session(
+        self,
+        causal_consistency: bool | None = None,
+        default_transaction_options: TransactionOptions | None = None,
+        snapshot: bool | None = False,
+    ) -> AsyncGenerator[MongoSession, None]:
+        """
+        Use a session to execute operations, for example:
+
+        ```python
+        async with Table.objects.use_session() as session:
+            await Table.objects.insert_one(document)
+        """
+        async with await self.collection.database.client.start_session(
+            causal_consistency=causal_consistency,
+            default_transaction_options=default_transaction_options,
+            snapshot=snapshot,
+        ) as session:
+            token = SESSION.set(session)
+            try:
+                yield session
+            finally:
+                SESSION.reset(token)
+
+    @asynccontextmanager
+    async def use_transaction(
+        self,
+        read_concern: Optional[ReadConcern] = None,
+        write_concern: Optional[WriteConcern] = None,
+        read_preference: Optional[_ServerMode] = None,
+        max_commit_time_ms: Optional[int] = None,
+    ) -> AsyncGenerator[None, None]:
+        """
+        Use a transaction to execute operations, for example:
+
+        ```python
+        async with Table.objects.use_transaction():
+            await Table.objects.insert_one(document)
+        """
+        async with self.use_session() as session:
+            async with session.start_transaction(
+                read_concern=read_concern,
+                write_concern=write_concern,
+                read_preference=read_preference,
+                max_commit_time_ms=max_commit_time_ms,
+            ):
+                yield
+
     async def insert_one(self, document: T) -> DocumentId:
-        insert_result = await self.collection.insert_one(document.to_mongo())
+        insert_result = await self.collection.insert_one(
+            document.to_mongo(), session=SESSION.get()
+        )
         return insert_result.inserted_id
 
     async def insert_many(
         self, *documents: T, ordered: bool = True
     ) -> list[DocumentId]:
         insert_result = await self.collection.insert_many(
-            [document.to_mongo() for document in documents], ordered=ordered
+            [document.to_mongo() for document in documents],
+            ordered=ordered,
+            session=SESSION.get(),
         )
         return insert_result.inserted_ids
 
     async def find(
         self,
         filter: Optional[Filter] = None,
         projection: Optional[Projection] = None,
@@ -149,14 +212,15 @@
         async for document in self.collection.find(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             skip=skip,
             limit=limit,
             sort=translate_sort(sort),
             allow_disk_use=allow_disk_use,
+            session=SESSION.get(),
         ):
             yield self.table.load(document, partial=True)
 
     async def find_one(
         self,
         filter: Optional[Filter] = None,
         projection: Optional[Projection] = None,
@@ -166,14 +230,15 @@
     ) -> T | None:
         document = await self.collection.find_one(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             skip=skip,
             sort=translate_sort(sort),
             allow_disk_use=allow_disk_use,
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     async def find_one_and_delete(
         self,
@@ -181,14 +246,15 @@
         projection: Optional[Projection] = None,
         sort: Optional[Sort] = None,
     ) -> T | None:
         document = await self.collection.find_one_and_delete(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             sort=translate_sort(sort),
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     async def find_one_and_replace(
         self,
@@ -202,14 +268,15 @@
         document = await self.collection.find_one_and_replace(
             filter=translate_filter(filter),
             replacement=replacement.to_mongo(),
             projection=translate_projection(projection),
             sort=translate_sort(sort),
             upsert=upsert,
             return_document=after_document,
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     async def find_one_and_update(
         self,
@@ -223,73 +290,87 @@
         document = await self.collection.find_one_and_update(
             filter=translate_filter(filter),
             update=update,
             projection=translate_projection(projection),
             sort=translate_sort(sort),
             upsert=upsert,
             return_document=after_document,
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     async def delete_one(
         self,
         filter: Optional[Filter] = None,
     ) -> MongoDeleteResult:
-        return await self.collection.delete_one(translate_filter(filter))
+        return await self.collection.delete_one(
+            translate_filter(filter),
+            session=SESSION.get(),
+        )
 
     async def delete_many(
         self,
         filter: Optional[Filter] = None,
     ) -> MongoDeleteResult:
-        return await self.collection.delete_many(translate_filter(filter))
+        return await self.collection.delete_many(
+            translate_filter(filter),
+            session=SESSION.get(),
+        )
 
     async def update_one(
         self,
         filter: Filter,
         update: Mapping[str, Any] | list[Mapping[str, Any]],
         upsert: bool = False,
     ) -> MongoUpdateResult:
         return await self.collection.update_one(
             translate_filter(filter),
             update,
             upsert=upsert,
+            session=SESSION.get(),
         )
 
     async def update_many(
         self,
         filter: Filter,
         update: Mapping[str, Any] | list[Mapping[str, Any]],
         upsert: bool = False,
     ) -> MongoUpdateResult:
         return await self.collection.update_many(
             translate_filter(filter),
             update,
             upsert=upsert,
+            session=SESSION.get(),
         )
 
     async def count_documents(
         self,
         filter: Filter,
     ) -> int:
-        return await self.collection.count_documents(translate_filter(filter))
+        return await self.collection.count_documents(
+            translate_filter(filter),
+            session=SESSION.get(),
+        )
 
     async def bulk_write(
         self,
         *requests: DeleteMany
         | DeleteOne
         | InsertOne[T]
         | ReplaceOne[T]
         | UpdateMany
         | UpdateOne,
         ordered: bool = True,
     ) -> MongoBlukWriteResult:
         return await self.collection.bulk_write(
-            [r.to_mongo() for r in requests], ordered=ordered
+            [r.to_mongo() for r in requests],
+            ordered=ordered,
+            session=SESSION.get(),
         )
 
 
 @dataclasses.dataclass
 class DeleteMany:
     filter: Filter
```

### Comparing `typedmongo-1.5.1/typedmongo/asyncio/fields.py` & `typedmongo-1.6.0/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/asyncio/table.py` & `typedmongo-1.6.0/typedmongo/asyncio/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/client.py` & `typedmongo-1.6.0/typedmongo/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from __future__ import annotations
 
 import dataclasses
 import decimal
+from contextlib import contextmanager
+from contextvars import ContextVar
 from typing import (
     TYPE_CHECKING,
     Any,
+    Generator,
     Iterable,
     Generic,
     Literal,
     Mapping,
     NoReturn,
     Optional,
     TypeAlias,
     TypeVar,
     overload,
 )
 
 from bson.codec_options import CodecOptions, TypeCodec, TypeRegistry
 from bson.decimal128 import Decimal128
+from pymongo.client_session import TransactionOptions
 from pymongo.operations import DeleteMany as MongoDeleteMany
 from pymongo.operations import DeleteOne as MongoDeleteOne
 from pymongo.operations import InsertOne as MongoInsertOne
 from pymongo.operations import ReplaceOne as MongoReplaceOne
 from pymongo.operations import UpdateMany as MongoUpdateMany
 from pymongo.operations import UpdateOne as MongoUpdateOne
+from pymongo.read_concern import ReadConcern
+from pymongo.read_preferences import _ServerMode
+from pymongo.write_concern import WriteConcern
 
 if TYPE_CHECKING:
+    from pymongo.client_session import ClientSession as MongoSession
     from pymongo.collection import Collection as MongoCollection
     from pymongo.database import Database as MongoDatabase
     from pymongo.results import BulkWriteResult as MongoBlukWriteResult
     from pymongo.results import DeleteResult as MongoDeleteResult
     from pymongo.results import UpdateResult as MongoUpdateResult
 
     from .table import Table
@@ -112,32 +120,87 @@
         (order_by.field.field_name, order_by.order)
         if isinstance(order_by, OrderBy)
         else order_by
         for order_by in s
     ]
 )
 
+SESSION: ContextVar[Optional[MongoSession]] = ContextVar("session", default=None)
+
 
 class Objects(Generic[T]):
     def __init__(self, table: type[T]) -> None:
         self.table = table
 
     @property
     def collection(self) -> MongoCollection:
         return self.table.__collection__
 
+    @contextmanager
+    def use_session(
+        self,
+        causal_consistency: bool | None = None,
+        default_transaction_options: TransactionOptions | None = None,
+        snapshot: bool | None = False,
+    ) -> Generator[MongoSession, None, None]:
+        """
+        Use a session to execute operations, for example:
+
+        ```python
+        with Table.objects.use_session() as session:
+            Table.objects.insert_one(document)
+        """
+        with self.collection.database.client.start_session(
+            causal_consistency=causal_consistency,
+            default_transaction_options=default_transaction_options,
+            snapshot=snapshot,
+        ) as session:
+            token = SESSION.set(session)
+            try:
+                yield session
+            finally:
+                SESSION.reset(token)
+
+    @contextmanager
+    def use_transaction(
+        self,
+        read_concern: Optional[ReadConcern] = None,
+        write_concern: Optional[WriteConcern] = None,
+        read_preference: Optional[_ServerMode] = None,
+        max_commit_time_ms: Optional[int] = None,
+    ) -> Generator[None, None, None]:
+        """
+        Use a transaction to execute operations, for example:
+
+        ```python
+        with Table.objects.use_transaction():
+            Table.objects.insert_one(document)
+        """
+        with self.use_session() as session:
+            with session.start_transaction(
+                read_concern=read_concern,
+                write_concern=write_concern,
+                read_preference=read_preference,
+                max_commit_time_ms=max_commit_time_ms,
+            ):
+                yield
+
     def insert_one(self, document: T) -> DocumentId:
-        insert_result = self.collection.insert_one(document.to_mongo())
+        insert_result = self.collection.insert_one(
+            document.to_mongo(), session=SESSION.get()
+        )
         return insert_result.inserted_id
 
     def insert_many(
         self, *documents: T, ordered: bool = True
     ) -> list[DocumentId]:
         insert_result = self.collection.insert_many(
-            [document.to_mongo() for document in documents], ordered=ordered
+            [document.to_mongo() for document in documents],
+            ordered=ordered,
+            session=SESSION.get(),
         )
         return insert_result.inserted_ids
 
     def find(
         self,
         filter: Optional[Filter] = None,
         projection: Optional[Projection] = None,
@@ -149,14 +212,15 @@
         for document in self.collection.find(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             skip=skip,
             limit=limit,
             sort=translate_sort(sort),
             allow_disk_use=allow_disk_use,
+            session=SESSION.get(),
         ):
             yield self.table.load(document, partial=True)
 
     def find_one(
         self,
         filter: Optional[Filter] = None,
         projection: Optional[Projection] = None,
@@ -166,14 +230,15 @@
     ) -> T | None:
         document = self.collection.find_one(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             skip=skip,
             sort=translate_sort(sort),
             allow_disk_use=allow_disk_use,
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     def find_one_and_delete(
         self,
@@ -181,14 +246,15 @@
         projection: Optional[Projection] = None,
         sort: Optional[Sort] = None,
     ) -> T | None:
         document = self.collection.find_one_and_delete(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             sort=translate_sort(sort),
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     def find_one_and_replace(
         self,
@@ -202,14 +268,15 @@
         document = self.collection.find_one_and_replace(
             filter=translate_filter(filter),
             replacement=replacement.to_mongo(),
             projection=translate_projection(projection),
             sort=translate_sort(sort),
             upsert=upsert,
             return_document=after_document,
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     def find_one_and_update(
         self,
@@ -223,73 +290,87 @@
         document = self.collection.find_one_and_update(
             filter=translate_filter(filter),
             update=update,
             projection=translate_projection(projection),
             sort=translate_sort(sort),
             upsert=upsert,
             return_document=after_document,
+            session=SESSION.get(),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
     def delete_one(
         self,
         filter: Optional[Filter] = None,
     ) -> MongoDeleteResult:
-        return self.collection.delete_one(translate_filter(filter))
+        return self.collection.delete_one(
+            translate_filter(filter),
+            session=SESSION.get(),
+        )
 
     def delete_many(
         self,
         filter: Optional[Filter] = None,
     ) -> MongoDeleteResult:
-        return self.collection.delete_many(translate_filter(filter))
+        return self.collection.delete_many(
+            translate_filter(filter),
+            session=SESSION.get(),
+        )
 
     def update_one(
         self,
         filter: Filter,
         update: Mapping[str, Any] | list[Mapping[str, Any]],
         upsert: bool = False,
     ) -> MongoUpdateResult:
         return self.collection.update_one(
             translate_filter(filter),
             update,
             upsert=upsert,
+            session=SESSION.get(),
         )
 
     def update_many(
         self,
         filter: Filter,
         update: Mapping[str, Any] | list[Mapping[str, Any]],
         upsert: bool = False,
     ) -> MongoUpdateResult:
         return self.collection.update_many(
             translate_filter(filter),
             update,
             upsert=upsert,
+            session=SESSION.get(),
         )
 
     def count_documents(
         self,
         filter: Filter,
     ) -> int:
-        return self.collection.count_documents(translate_filter(filter))
+        return self.collection.count_documents(
+            translate_filter(filter),
+            session=SESSION.get(),
+        )
 
     def bulk_write(
         self,
         *requests: DeleteMany
         | DeleteOne
         | InsertOne[T]
         | ReplaceOne[T]
         | UpdateMany
         | UpdateOne,
         ordered: bool = True,
     ) -> MongoBlukWriteResult:
         return self.collection.bulk_write(
-            [r.to_mongo() for r in requests], ordered=ordered
+            [r.to_mongo() for r in requests],
+            ordered=ordered,
+            session=SESSION.get(),
         )
 
 
 @dataclasses.dataclass
 class DeleteMany:
     filter: Filter
```

### Comparing `typedmongo-1.5.1/typedmongo/expressions.py` & `typedmongo-1.6.0/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/fields.py` & `typedmongo-1.6.0/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/marshamallow.py` & `typedmongo-1.6.0/typedmongo/marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/shortcuts.py` & `typedmongo-1.6.0/typedmongo/shortcuts.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/typedmongo/sync.py` & `typedmongo-1.6.0/typedmongo/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,30 @@
                 "from motor.motor_asyncio import AsyncIOMotorCollection",
                 "from pymongo.collection import Collection",
             )
             .replace(
                 "from motor.motor_asyncio import AsyncIOMotorDatabase",
                 "from pymongo.database import Database",
             )
+            .replace(
+                "from motor.motor_asyncio import AsyncIOMotorClientSession as MongoSession",
+                "from pymongo.client_session import ClientSession as MongoSession",
+            )
             .replace("async def ", "def ")
             .replace("await ", "")
             .replace("async for ", "for ")
             .replace("async with ", "with ")
             .replace("AsyncIterable", "Iterable")
+            .replace(
+                "AsyncGenerator[MongoSession, None]",
+                "Generator[MongoSession, None, None]",
+            )
+            .replace("AsyncGenerator[None, None]", "Generator[None, None, None]")
+            .replace("AsyncGenerator", "Generator")
+            .replace("asynccontextmanager", "contextmanager")
         )
         if just_check:
             if content != new_file_path.read_text():
                 print(f"File {new_file_path} is not synchronized.")
                 exit_code = 1
         else:
             new_file_path.write_text(content)
```

### Comparing `typedmongo-1.5.1/typedmongo/table.py` & `typedmongo-1.6.0/typedmongo/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.5.1/PKG-INFO` & `typedmongo-1.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: typedmongo
-Version: 1.5.1
-Summary: A production-ready modern Python MongoDB ODM
-Author-Email: abersheeran <me@abersheeran.com>
-License: Apache2.0
-Requires-Python: >=3.10
-Requires-Dist: pymongo>=4.6.3
-Requires-Dist: motor>=3.4.0
-Requires-Dist: marshmallow>=3.21.1
-Requires-Dist: typing-extensions>=4.11.0
-Description-Content-Type: text/markdown
-
 # Typed Mongo
 
 A production-ready modern Python MongoDB ODM
 
 In addition to synchronous mode, you can use asynchronous mode, just export from `typedmongo.asyncio`.
 
 ## Install
@@ -156,7 +143,27 @@
 - `~((Table.field == value) & (Table.field == value))`
 - `~((Table.field == value) | (Table.field == value))`
 
 ### Sort expressions
 
 - `+Table.field`: Ascending
 - `-Table.field`: Descending
+
+## Objects
+
+- `Table.objects`: The object manager of the table.
+  - `collection`: The collection of the table.
+  - `use_session`: Use session for the operations. (Use `contextvars`, so you don't need to pass the session to the function parameters)
+  - `use_transaction`: Use transaction for the operations.
+  - `insert_one`: Insert one document.
+  - `insert_many`: Insert many documents.
+  - `find`: Find many documents.
+  - `find_one`: Find one document.
+  - `find_one_and_update`: Find one and update.
+  - `find_one_and_replace`: Find one and replace.
+  - `find_one_and_delete`: Find one and delete.
+  - `delete_one`: Delete one document.
+  - `delete_many`: Delete many documents.
+  - `update_one`: Update one document.
+  - `update_many`: Update many documents.
+  - `count_documents`: Count documents.
+  - `bulk_write`: Bulk write operations.
```

