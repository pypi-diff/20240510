# Comparing `tmp/llama_index_vector_stores_mongodb-0.1.4.tar.gz` & `tmp/llama_index_vector_stores_mongodb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_mongodb-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_mongodb-0.1.5.tar", max compression
```

## Comparing `llama_index_vector_stores_mongodb-0.1.4.tar` & `llama_index_vector_stores_mongodb-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2024-02-13 13:53:02.011358 llama_index_vector_stores_mongodb-0.1.4/README.md
--rw-r--r--   0        0        0      116 2024-02-13 13:53:02.011553 llama_index_vector_stores_mongodb-0.1.4/llama_index/vector_stores/mongodb/__init__.py
--rw-r--r--   0        0        0     7772 2024-02-14 19:04:12.013150 llama_index_vector_stores_mongodb-0.1.4/llama_index/vector_stores/mongodb/base.py
--rw-r--r--   0        0        0     1488 2024-02-21 23:31:34.426937 llama_index_vector_stores_mongodb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 llama_index_vector_stores_mongodb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5949 2024-05-10 18:12:43.900771 llama_index_vector_stores_mongodb-0.1.5/README.md
+-rw-r--r--   0        0        0      116 2024-05-10 18:12:43.900771 llama_index_vector_stores_mongodb-0.1.5/llama_index/vector_stores/mongodb/__init__.py
+-rw-r--r--   0        0        0     9187 2024-05-10 18:12:43.900771 llama_index_vector_stores_mongodb-0.1.5/llama_index/vector_stores/mongodb/base.py
+-rw-r--r--   0        0        0     1604 2024-05-10 18:12:43.900771 llama_index_vector_stores_mongodb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6540 1970-01-01 00:00:00.000000 llama_index_vector_stores_mongodb-0.1.5/PKG-INFO
```

### Comparing `llama_index_vector_stores_mongodb-0.1.4/llama_index/vector_stores/mongodb/base.py` & `llama_index_vector_stores_mongodb-0.1.5/llama_index/vector_stores/mongodb/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,14 +40,53 @@
     """MongoDB Atlas Vector Store.
 
     To use, you should have both:
     - the ``pymongo`` python package installed
     - a connection string associated with a MongoDB Atlas Cluster
     that has an Atlas Vector Search index
 
+    To get started head over to the [Atlas quick start](https://www.mongodb.com/docs/atlas/getting-started/).
+
+    Once your store is created, be sure to enable indexing in the Atlas GUI.
+
+    Please refer to the [documentation](https://www.mongodb.com/docs/atlas/atlas-vector-search/create-index/)
+    to get more details on how to define an Atlas Vector Search index. You can name the index {ATLAS_VECTOR_SEARCH_INDEX_NAME}
+    and create the index on the namespace {DB_NAME}.{COLLECTION_NAME}.
+    Finally, write the following definition in the JSON editor on MongoDB Atlas:
+
+    ```
+    {
+        "name": "index_name",
+        "type": "vectorSearch",
+        "fields":[
+            {
+            "type": "vector",
+            "path": "embedding",
+            "numDimensions": 1536,
+            "similarity": "cosine"
+            }
+        ]
+    }
+    ```
+
+
+    Examples:
+        `pip install llama-index-vector-stores-mongodb`
+
+        ```python
+        import pymongo
+        from llama_index.vector_stores.mongodb import MongoDBAtlasVectorSearch
+
+        # Ensure you have the MongoDB URI with appropriate credentials
+        mongo_uri = "mongodb+srv://<username>:<password>@<host>?retryWrites=true&w=majority"
+        mongodb_client = pymongo.MongoClient(mongo_uri)
+
+        # Create an instance of MongoDBAtlasVectorSearch
+        vector_store = MongoDBAtlasVectorSearch(mongodb_client)
+        ```
     """
 
     stores_text: bool = True
     flat_metadata: bool = True
 
     _mongodb_client: Any = PrivateAttr()
     _collection: Any = PrivateAttr()
@@ -60,15 +99,15 @@
 
     def __init__(
         self,
         mongodb_client: Optional[Any] = None,
         db_name: str = "default_db",
         collection_name: str = "default_collection",
         index_name: str = "default",
-        id_key: str = "id",
+        id_key: str = "_id",
         embedding_key: str = "embedding",
         text_key: str = "text",
         metadata_key: str = "metadata",
         insert_kwargs: Optional[Dict] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize the vector store.
@@ -85,21 +124,21 @@
             metadata_key: A MongoDB field that will contain
             the metadata for each document.
             insert_kwargs: The kwargs used during `insert`.
         """
         if mongodb_client is not None:
             self._mongodb_client = cast(MongoClient, mongodb_client)
         else:
-            if "MONGO_URI" not in os.environ:
+            if "MONGODB_URI" not in os.environ:
                 raise ValueError(
-                    "Must specify MONGO_URI via env variable "
+                    "Must specify MONGODB_URI via env variable "
                     "if not directly passing in client."
                 )
             self._mongodb_client = MongoClient(
-                os.environ["MONGO_URI"],
+                os.environ["MONGODB_URI"],
                 driver=DriverInfo(name="llama-index", version=version("llama-index")),
             )
 
         self._collection = self._mongodb_client[db_name][collection_name]
         self._index_name = index_name
         self._embedding_key = embedding_key
         self._id_key = id_key
@@ -150,15 +189,15 @@
         Delete nodes using with ref_doc_id.
 
         Args:
             ref_doc_id (str): The doc_id of the document to delete.
 
         """
         # delete by filtering on the doc_id metadata
-        self._collection.delete_one(
+        self._collection.delete_many(
             filter={self._metadata_key + ".ref_doc_id": ref_doc_id}, **delete_kwargs
         )
 
     @property
     def client(self) -> Any:
         """Return MongoDB client."""
         return self._mongodb_client
```

### Comparing `llama_index_vector_stores_mongodb-0.1.4/pyproject.toml` & `llama_index_vector_stores_mongodb-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -17,30 +17,35 @@
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+authors = [
+    "The MongoDB Python Team",
+]
 description = "llama-index vector_stores mongodb integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-mongodb"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymongo = "^4.6.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
+llama-index-embeddings-openai = "^0.1.5"
+llama-index-llms-openai = "^0.1.13"
+llama-index-readers-file = "^0.1.4"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
 pytest = "7.2.1"
 pytest-mock = "3.11.1"
 ruff = "0.0.292"
 tree-sitter-languages = "^1.8.0"
```

