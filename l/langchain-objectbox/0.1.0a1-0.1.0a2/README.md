# Comparing `tmp/langchain_objectbox-0.1.0a1.tar.gz` & `tmp/langchain_objectbox-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_objectbox-0.1.0a1.tar", max compression
+gzip compressed data, was "langchain_objectbox-0.1.0a2.tar", max compression
```

## Comparing `langchain_objectbox-0.1.0a1.tar` & `langchain_objectbox-0.1.0a2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2024-04-29 16:27:47.475174 langchain_objectbox-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     3874 2024-04-30 13:28:53.923651 langchain_objectbox-0.1.0a1/README.md
--rw-r--r--   0        0        0       86 2024-04-29 16:12:03.665330 langchain_objectbox-0.1.0a1/langchain_objectbox/__init__.py
--rw-r--r--   0        0        0     8618 2024-04-30 11:50:45.356521 langchain_objectbox-0.1.0a1/langchain_objectbox/vectorstores.py
--rw-r--r--   0        0        0      661 2024-04-30 13:30:58.130738 langchain_objectbox-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     4538 1970-01-01 00:00:00.000000 langchain_objectbox-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-30 06:48:53.171402 langchain_objectbox-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     3874 2024-05-02 20:45:15.040493 langchain_objectbox-0.1.0a2/README.md
+-rw-r--r--   0        0        0       86 2024-04-30 06:48:53.171402 langchain_objectbox-0.1.0a2/langchain_objectbox/__init__.py
+-rw-r--r--   0        0        0     9659 2024-05-09 16:02:05.896141 langchain_objectbox-0.1.0a2/langchain_objectbox/vectorstores.py
+-rw-r--r--   0        0        0      661 2024-05-09 16:11:25.286811 langchain_objectbox-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4538 1970-01-01 00:00:00.000000 langchain_objectbox-0.1.0a2/PKG-INFO
```

### Comparing `langchain_objectbox-0.1.0a1/LICENSE` & `langchain_objectbox-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_objectbox-0.1.0a1/README.md` & `langchain_objectbox-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_objectbox-0.1.0a1/langchain_objectbox/vectorstores.py` & `langchain_objectbox-0.1.0a2/langchain_objectbox/vectorstores.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 import shutil
 from typing import *
 import numpy as np
 import objectbox
+import time
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 from objectbox.model.entity import Entity
 from objectbox.model.model import IdUid
 from objectbox.model.properties import (
     HnswDistanceType,
     HnswIndex,
     Id,
     Property,
     PropertyType,
 )
 
-DIRECTORY = "data"
+DIRECTORY = "objectbox"
 
 
 class ObjectBox(VectorStore):
     """
     ObjectBox as Vector Store.
     To use, you should have the `objectbox` python package installed and `flatbuffers`.
     Args:
@@ -36,23 +37,25 @@
     def __init__(
         self,
         embedding: Embeddings,
         embedding_dimensions: int,
         distance_type: HnswDistanceType = HnswDistanceType.EUCLIDEAN,
         db_directory: Optional[str] = None,
         clear_db: Optional[bool] = False,
+        do_log: Optional[bool] = False,
     ):
         self._embedding = embedding
         self._embedding_dimensions = embedding_dimensions
         self._distance_type = distance_type
         self.db_directory = db_directory
         self._clear_db = clear_db
         self._entity_model = self._create_entity_class()
         self._db = self._create_objectbox_db()
         self._vector_box = objectbox.Box(self._db, self._entity_model)
+        self._do_log = do_log
 
     @property
     def embeddings(self) -> Optional[Embeddings]:
         return self._embedding if isinstance(self._embedding, Embeddings) else None
 
     def add_texts(
         self,
@@ -62,30 +65,45 @@
     ) -> List[str]:
         """Add list of text along with embeddings to the vector store
         Args:
             texts (Iterable[str]): collection of text to add to the database
         Returns:
             List of ids for the newly inserted documents
         """
-        embeddings = self._embedding.embed_documents(list(texts))
+
+        texts_list = list(texts)
+        start = time.perf_counter()
+        embeddings = self._embedding.embed_documents(texts_list)
+
+        if self._do_log:
+            end = time.perf_counter()
+            print(f"Embedded  {len(texts_list)} documents in {end - start} seconds")
+        
         ids = []
 
         if not metadatas:
             metadatas = [{} for _ in texts]
 
+        start = time.perf_counter()
+
         with self._db.write_tx():
             for text, metadata, embedding in zip(texts, metadatas, embeddings):
                 object_id = self._vector_box.put(
                     self._entity_model(
                         text=text,
                         metadata=metadata,
                         embeddings=embedding
                     )
                 )
                 ids.append(object_id)
+
+        if self._do_log:
+            end = time.perf_counter()
+            print(f"ObjectBox stored {len(ids)} documents in { end - start} seconds")
+
         return ids
 
     def similarity_search(
         self, query: str, k: int = 4, **kwargs: Any
     ) -> List[Document]:
         """Run similarity search on query
         Args:
@@ -130,19 +148,26 @@
             query (str): Query
             k (int): Number of Documents to return. Defaults to 4.
 
         Returns:
             List of Documents with score most similar to the query vector.
         """
         embedded_query = self._embedding.embed_query(query)
+
+        start = time.perf_counter()
         embeddings_prop = self._entity_model.get_property("embeddings")
         qb = self._vector_box.query()
         qb.nearest_neighbors_f32(embeddings_prop, embedded_query, k)
         query = qb.build()
         results = query.find_with_scores()
+
+        if self._do_log:
+            end = time.perf_counter()
+            print(f"ObjectBox retrieved {len(results)} vectors in { end - start} seconds")
+
         return [
             (Document(page_content=obj.text, metadata=obj.metadata), score)
             for obj, score in results
         ]
 
     def similarity_search_by_vector(
         self, embedding: List[float], k: int = 4, **kwargs: Any
@@ -152,19 +177,26 @@
         Args:
             embedding (List[float]): Embedding to look up documents similar to.
             k (int): Number of Documents to return. Defaults to 4.
 
         Returns:
             List of Documents most similar to the query vector.
         """
+        start = time.perf_counter()
+
         embeddings_prop = self._entity_model.get_property("embeddings")
         qb = self._vector_box.query()
         qb.nearest_neighbors_f32(embeddings_prop, embedding, k)
         query = qb.build()
         results = query.find_with_scores()
+
+        if self._do_log:
+            end = time.perf_counter()
+            print(f"ObjectBox retrieved {len(results)} vectors in { end - start} seconds")
+
         return [
             Document(page_content=obj.text, metadata=obj.metadata)
             for obj, _ in results
         ]
 
     @classmethod
     def from_texts(
@@ -197,19 +229,24 @@
         with self._db.write_tx():
             for id in ids:
                 try:
                     int_id = int(id)
                 except ValueError:
                     raise ValueError("invalid id input")
                 self._vector_box.remove(int_id)
+
+        if self._do_log:
+            end = time.perf_counter()
+            print(f"ObjectBox deleted {len(ids)} vectors in { end - start} seconds")
+
         return True
 
     def _create_objectbox_db(self) -> objectbox:
         """registering the VectorEntity model and setting up objectbox database"""
-        db_path = "data" if self.db_directory is None else self.db_directory
+        db_path = DIRECTORY if self.db_directory is None else self.db_directory
         if self._clear_db and os.path.exists(db_path):
             shutil.rmtree(db_path)
         model = objectbox.Model()
         model.entity(self._entity_model, last_property_id=IdUid(4, 1004))
         model.last_entity_id = IdUid(1, 1)
         model.last_index_id = IdUid(3, 10001)
         return objectbox.Builder().model(model).directory(db_path).build()
```

### Comparing `langchain_objectbox-0.1.0a1/pyproject.toml` & `langchain_objectbox-0.1.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-objectbox"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Integration package connecting ObjectBox and LangChain"
 authors = ["ObjectBox" ]
 license = "MIT" 
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License"
 ]
 [tool.poetry.dependencies]
 python = "^3.8.1" 
 langchain-core = "^0.1.45"
-objectbox = "0.7.0a7"
+objectbox = "0.7.0a9"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 langchain = "^0.1.16"
 numpy = [ 
     { version = "^1.26", python = "^3.12" },
```

### Comparing `langchain_objectbox-0.1.0a1/PKG-INFO` & `langchain_objectbox-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-objectbox
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Integration package connecting ObjectBox and LangChain
 License: MIT
 Author: ObjectBox
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain-core (>=0.1.45,<0.2.0)
-Requires-Dist: objectbox (==0.7.0a7)
+Requires-Dist: objectbox (==0.7.0a9)
 Description-Content-Type: text/markdown
 
 # langchain-objectbox
 
 ## About
 
 This package contains the [ObjectBox](https://objectbox.io) integrations for [LangChain](https://www.langchain.com).
```

