# Comparing `tmp/llama_index_storage_kvstore_redis-0.1.4.tar.gz` & `tmp/llama_index_storage_kvstore_redis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_kvstore_redis-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_storage_kvstore_redis-0.1.5.tar", max compression
```

## Comparing `llama_index_storage_kvstore_redis-0.1.4.tar` & `llama_index_storage_kvstore_redis-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/README.md
--rw-r--r--   0        0        0       92 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/llama_index/storage/kvstore/redis/__init__.py
--rw-r--r--   0        0        0     5319 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/llama_index/storage/kvstore/redis/base.py
--rw-r--r--   0        0        0     1466 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_redis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-10 17:32:03.605523 llama_index_storage_kvstore_redis-0.1.5/README.md
+-rw-r--r--   0        0        0       92 2024-05-10 17:32:03.605523 llama_index_storage_kvstore_redis-0.1.5/llama_index/storage/kvstore/redis/__init__.py
+-rw-r--r--   0        0        0     6813 2024-05-10 17:32:03.605523 llama_index_storage_kvstore_redis-0.1.5/llama_index/storage/kvstore/redis/base.py
+-rw-r--r--   0        0        0     1466 2024-05-10 17:32:03.605523 llama_index_storage_kvstore_redis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_redis-0.1.5/PKG-INFO
```

### Comparing `llama_index_storage_kvstore_redis-0.1.4/llama_index/storage/kvstore/redis/base.py` & `llama_index_storage_kvstore_redis-0.1.5/llama_index/storage/kvstore/redis/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import json
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import Any, Dict, List, Optional, Tuple
 
 from llama_index.core.storage.kvstore.types import (
     DEFAULT_BATCH_SIZE,
     DEFAULT_COLLECTION,
     BaseKVStore,
 )
 
+from redis.asyncio import Redis as AsyncRedis
 from redis import Redis
 
 
 class RedisKVStore(BaseKVStore):
-    """Redis KV Store.
+    """
+    Redis KV Store.
 
     Args:
+        redis_uri (str): Redis URI
         redis_client (Any): Redis client
-        redis_url (Optional[str]): Redis server URI
+        async_redis_client (Any): Async Redis client
 
     Raises:
             ValueError: If redis-py is not installed
 
     Examples:
         >>> from llama_index.storage.kvstore.redis import RedisKVStore
         >>> # Create a RedisKVStore
@@ -27,61 +30,84 @@
         >>>     redis_url="redis://127.0.0.1:6379")
 
     """
 
     def __init__(
         self,
         redis_uri: Optional[str] = "redis://127.0.0.1:6379",
+        redis_client: Optional[Redis] = None,
+        async_redis_client: Optional[AsyncRedis] = None,
         **kwargs: Any,
     ) -> None:
         # user could inject customized redis client.
         # for instance, redis have specific TLS connection, etc.
-        if "redis_client" in kwargs:
-            self._redis_client = cast(Redis, kwargs["redis_client"])
+        if redis_client is not None:
+            self._redis_client = redis_client
+
+            # create async client from sync client
+            if async_redis_client is not None:
+                self._async_redis_client = async_redis_client
+            else:
+                try:
+                    self._async_redis_client = AsyncRedis.from_url(
+                        self._redis_client.connection_pool.connection_kwargs["url"]
+                    )
+                except Exception:
+                    print(
+                        "Could not create async redis client from sync client, "
+                        "pass in `async_redis_client` explicitly."
+                    )
+                    self._async_redis_client = None
         elif redis_uri is not None:
             # otherwise, try initializing redis client
             try:
                 # connect to redis from url
                 self._redis_client = Redis.from_url(redis_uri, **kwargs)
+                self._async_redis_client = AsyncRedis.from_url(redis_uri, **kwargs)
             except ValueError as e:
                 raise ValueError(f"Redis failed to connect: {e}")
         else:
             raise ValueError("Either 'redis_client' or redis_url must be provided.")
 
     def put(self, key: str, val: dict, collection: str = DEFAULT_COLLECTION) -> None:
-        """Put a key-value pair into the store.
+        """
+        Put a key-value pair into the store.
 
         Args:
             key (str): key
             val (dict): value
             collection (str): collection name
 
         """
         self._redis_client.hset(name=collection, key=key, value=json.dumps(val))
 
     async def aput(
         self, key: str, val: dict, collection: str = DEFAULT_COLLECTION
     ) -> None:
-        """Put a key-value pair into the store.
+        """
+        Put a key-value pair into the store.
 
         Args:
             key (str): key
             val (dict): value
             collection (str): collection name
 
         """
-        raise NotImplementedError
+        await self._async_redis_client.hset(
+            name=collection, key=key, value=json.dumps(val)
+        )
 
     def put_all(
         self,
         kv_pairs: List[Tuple[str, dict]],
         collection: str = DEFAULT_COLLECTION,
         batch_size: int = DEFAULT_BATCH_SIZE,
     ) -> None:
-        """Put a dictionary of key-value pairs into the store.
+        """
+        Put a dictionary of key-value pairs into the store.
 
         Args:
             kv_pairs (List[Tuple[str, dict]]): key-value pairs
             collection (str): collection name
 
         """
         with self._redis_client.pipeline() as pipe:
@@ -94,87 +120,101 @@
                     cur_batch = 0
                     pipe.execute()
 
             if cur_batch > 0:
                 pipe.execute()
 
     def get(self, key: str, collection: str = DEFAULT_COLLECTION) -> Optional[dict]:
-        """Get a value from the store.
+        """
+        Get a value from the store.
 
         Args:
             key (str): key
             collection (str): collection name
 
         """
         val_str = self._redis_client.hget(name=collection, key=key)
         if val_str is None:
             return None
         return json.loads(val_str)
 
     async def aget(
         self, key: str, collection: str = DEFAULT_COLLECTION
     ) -> Optional[dict]:
-        """Get a value from the store.
+        """
+        Get a value from the store.
 
         Args:
             key (str): key
             collection (str): collection name
 
         """
-        raise NotImplementedError
+        val_str = await self._async_redis_client.hget(name=collection, key=key)
+        if val_str is None:
+            return None
+        return json.loads(val_str)
 
     def get_all(self, collection: str = DEFAULT_COLLECTION) -> Dict[str, dict]:
         """Get all values from the store."""
         collection_kv_dict = {}
         for key, val_str in self._redis_client.hscan_iter(name=collection):
             value = dict(json.loads(val_str))
             collection_kv_dict[key.decode()] = value
         return collection_kv_dict
 
     async def aget_all(self, collection: str = DEFAULT_COLLECTION) -> Dict[str, dict]:
         """Get all values from the store."""
-        raise NotImplementedError
+        collection_kv_dict = {}
+        async for key, val_str in self._async_redis_client.hscan_iter(name=collection):
+            value = dict(json.loads(val_str))
+            collection_kv_dict[key.decode()] = value
+        return collection_kv_dict
 
     def delete(self, key: str, collection: str = DEFAULT_COLLECTION) -> bool:
-        """Delete a value from the store.
+        """
+        Delete a value from the store.
 
         Args:
             key (str): key
             collection (str): collection name
 
         """
         deleted_num = self._redis_client.hdel(collection, key)
         return bool(deleted_num > 0)
 
     async def adelete(self, key: str, collection: str = DEFAULT_COLLECTION) -> bool:
-        """Delete a value from the store.
+        """
+        Delete a value from the store.
 
         Args:
             key (str): key
             collection (str): collection name
 
         """
-        raise NotImplementedError
+        deleted_num = await self._async_redis_client.hdel(collection, key)
+        return bool(deleted_num > 0)
 
     @classmethod
     def from_host_and_port(
         cls,
         host: str,
         port: int,
     ) -> "RedisKVStore":
-        """Load a RedisKVStore from a Redis host and port.
+        """
+        Load a RedisKVStore from a Redis host and port.
 
         Args:
             host (str): Redis host
             port (int): Redis port
         """
         url = f"redis://{host}:{port}".format(host=host, port=port)
         return cls(redis_uri=url)
 
     @classmethod
     def from_redis_client(cls, redis_client: Any) -> "RedisKVStore":
-        """Load a RedisKVStore from a Redis Client.
+        """
+        Load a RedisKVStore from a Redis Client.
 
         Args:
             redis_client (Redis): Redis client
         """
         return cls(redis_client=redis_client)
```

### Comparing `llama_index_storage_kvstore_redis-0.1.4/pyproject.toml` & `llama_index_storage_kvstore_redis-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index kvstore redis integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-kvstore-redis"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 redis = "^5.0.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_storage_kvstore_redis-0.1.4/PKG-INFO` & `llama_index_storage_kvstore_redis-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-kvstore-redis
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index kvstore redis integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

