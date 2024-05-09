# Comparing `tmp/langgraph_sdk-0.1.5.tar.gz` & `tmp/langgraph_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_sdk-0.1.5.tar", max compression
+gzip compressed data, was "langgraph_sdk-0.1.6.tar", max compression
```

## Comparing `langgraph_sdk-0.1.5.tar` & `langgraph_sdk-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.5/README.md
--rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.5/langgraph_sdk/__init__.py
--rw-r--r--   0        0        0    10894 2024-05-08 19:15:33.076998 langgraph_sdk-0.1.5/langgraph_sdk/client.py
--rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.5/langgraph_sdk/schema.py
--rw-r--r--   0        0        0     1004 2024-05-08 19:48:34.135456 langgraph_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.6/langgraph_sdk/__init__.py
+-rw-r--r--   0        0        0    11445 2024-05-09 00:45:54.135870 langgraph_sdk-0.1.6/langgraph_sdk/client.py
+-rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.6/langgraph_sdk/schema.py
+-rw-r--r--   0        0        0     1004 2024-05-09 00:46:07.435262 langgraph_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.6/PKG-INFO
```

### Comparing `langgraph_sdk-0.1.5/langgraph_sdk/client.py` & `langgraph_sdk-0.1.6/langgraph_sdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import logging
 import sys
 from typing import Any, AsyncIterator, List, NamedTuple, Optional, Union
 
 import httpx
 import httpx_sse
 import orjson
 from httpx._types import QueryParamTypes
@@ -14,14 +15,16 @@
     Metadata,
     Run,
     RunEvent,
     StreamMode,
     Thread,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def get_client(*, url: str = "http://localhost:8123") -> "LangServeClient":
     client = httpx.AsyncClient(
         base_url=url,
         transport=httpx.AsyncHTTPTransport(retries=5),
         timeout=httpx.Timeout(connect=5, read=60, write=60, pool=5),
     )
@@ -47,66 +50,76 @@
 
     async def get(self, path: str, *, params: QueryParamTypes = None) -> dict:
         """Make a GET request."""
         r = await self.client.get(path, params=params)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
+            body = (await r.aread()).decode()
             if sys.version_info >= (3, 11):
-                e.add_note((await r.aread()).decode())
+                e.add_note(body)
+            logger.error(f"Error from langgraph-api: {body}", exc_info=e)
             raise e
         return await decode_json(r)
 
     async def post(self, path: str, *, json: dict) -> dict:
         """Make a POST request."""
         headers, content = await encode_json(json)
         r = await self.client.post(path, headers=headers, content=content)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
+            body = (await r.aread()).decode()
             if sys.version_info >= (3, 11):
-                e.add_note((await r.aread()).decode())
+                e.add_note(body)
+            logger.error(f"Error from langgraph-api: {body}", exc_info=e)
             raise e
         return await decode_json(r)
 
     async def put(self, path: str, *, json: dict) -> dict:
         """Make a PUT request."""
         headers, content = await encode_json(json)
         r = await self.client.put(path, headers=headers, content=content)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
+            body = (await r.aread()).decode()
             if sys.version_info >= (3, 11):
-                e.add_note((await r.aread()).decode())
+                e.add_note(body)
+            logger.error(f"Error from langgraph-api: {body}", exc_info=e)
             raise e
         return await decode_json(r)
 
     async def delete(self, path: str) -> None:
         """Make a DELETE request."""
         r = await self.client.delete(path)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
+            body = (await r.aread()).decode()
             if sys.version_info >= (3, 11):
-                e.add_note((await r.aread()).decode())
+                e.add_note(body)
+            logger.error(f"Error from langgraph-api: {body}", exc_info=e)
             raise e
 
     async def stream(
         self, path: str, method: str, *, json: dict = None
     ) -> AsyncIterator[StreamPart]:
         """Stream the results of a request using SSE."""
         headers, content = await encode_json(json)
         async with httpx_sse.aconnect_sse(
             self.client, method, path, headers=headers, content=content
         ) as sse:
             try:
                 sse.response.raise_for_status()
             except httpx.HTTPStatusError as e:
+                body = (await sse.response.aread()).decode()
                 if sys.version_info >= (3, 11):
-                    e.add_note((await sse.response.aread()).decode())
+                    e.add_note(body)
+                logger.error(f"Error from langgraph-api: {body}", exc_info=e)
                 raise e
             async for event in sse.aiter_sse():
                 yield StreamPart(
                     event.event, orjson.loads(event.data) if event.data else None
                 )
```

### Comparing `langgraph_sdk-0.1.5/langgraph_sdk/schema.py` & `langgraph_sdk-0.1.6/langgraph_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `langgraph_sdk-0.1.5/pyproject.toml` & `langgraph_sdk-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-sdk"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9.0,<4.0"
```

### Comparing `langgraph_sdk-0.1.5/PKG-INFO` & `langgraph_sdk-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langgraph-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Nuno Campos
 Author-email: nuno@langchain.dev
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

