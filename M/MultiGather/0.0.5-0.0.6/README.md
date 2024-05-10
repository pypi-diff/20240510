# Comparing `tmp/multigather-0.0.5.tar.gz` & `tmp/multigather-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Admin\Desktop\gathernous\dist\.tmp-70_4f6c_\multigather-0.0.5.tar", last modified: Thu May  9 07:48:57 2024, max compression
+gzip compressed data, was "C:\Users\Admin\Desktop\testmygather\dist\.tmp-ksx_39bd\multigather-0.0.6.tar", last modified: Fri May 10 08:27:02 2024, max compression
```

## Comparing `multigather-0.0.5.tar` & `multigather-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 07:48:57.844391 multigather-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-09 07:48:57.819516 multigather-0.0.5/MultiGather/
--rw-rw-rw-   0        0        0     1869 2024-05-09 07:48:30.000000 multigather-0.0.5/MultiGather/Client.py
--rw-rw-rw-   0        0        0      708 2024-05-09 07:31:32.000000 multigather-0.0.5/MultiGather/Types.py
--rw-rw-rw-   0        0        0       45 2024-05-09 07:42:54.000000 multigather-0.0.5/MultiGather/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 07:48:57.837073 multigather-0.0.5/MultiGather.egg-info/
--rw-rw-rw-   0        0        0     2256 2024-05-09 07:48:57.000000 multigather-0.0.5/MultiGather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-09 07:48:57.000000 multigather-0.0.5/MultiGather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 07:48:57.000000 multigather-0.0.5/MultiGather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 07:48:57.000000 multigather-0.0.5/MultiGather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2256 2024-05-09 07:48:57.838580 multigather-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2024-05-09 07:37:15.000000 multigather-0.0.5/README.md
--rw-rw-rw-   0        0        0      504 2024-05-09 07:48:50.000000 multigather-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 07:48:57.844391 multigather-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 08:27:02.603116 multigather-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-10 08:27:02.572134 multigather-0.0.6/MultiGather/
+-rw-rw-rw-   0        0        0     2389 2024-05-10 08:24:56.000000 multigather-0.0.6/MultiGather/Client.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 08:24:56.000000 multigather-0.0.6/MultiGather/Types.py
+-rw-rw-rw-   0        0        0      232 2024-05-10 08:24:56.000000 multigather-0.0.6/MultiGather/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:27:02.596122 multigather-0.0.6/MultiGather.egg-info/
+-rw-rw-rw-   0        0        0     2257 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2257 2024-05-10 08:27:02.600119 multigather-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1756 2024-05-10 08:24:56.000000 multigather-0.0.6/README.md
+-rw-rw-rw-   0        0        0      504 2024-05-10 08:26:07.000000 multigather-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:27:02.603116 multigather-0.0.6/setup.cfg
```

### Comparing `multigather-0.0.5/MultiGather/Client.py` & `multigather-0.0.6/MultiGather/Client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import aiohttp
 import asyncio
-from .Types import Response as _Response, Request as _Request, Config as _Config
+from Types import Response, Request, Config
 
 class Connection:
-    def __init__(self, request: _Config):
+    def __init__(self, request: Config):
         self.connector = aiohttp.TCPConnector(limit=request.max_connection_limit)  # Set connection limit
-    async def sendRequest(self, request: _Request):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=_Config.timeout)) as session:
+        
+    async def sendRequest(self, request: Request):
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=Config.timeout)) as session:
+            
             tasks = [self._sendRequest(request=request, session=session) for _ in range(request.amount)]
-            return await asyncio.gather(*tasks) ## send Requests, and return them as generator.
-
-    async def _sendRequest(self, session: aiohttp.ClientSession, request: _Request):
+            return await asyncio.gather(*tasks) ## Send the tasks to be processed.
+    async def _sendRequest(self, session: aiohttp.ClientSession, request: Request):
         try:
             async with session.request(
                     method=request.method, url=request.url,
                     headers=request.headers, json=request.json,
-                    data=request.data, params=request.params
+                    data=request.data, params=request.params,
+                    proxy=request.proxy
             ) as response:
+                
                 response.raise_for_status()
-                content_type = response.headers.get('content-type')
-                json_content = None
-                if content_type and 'application/json' in content_type:
-                    json_content = await response.json()
-                return _Response(
+                content_type = response.headers.get('content-type', '')
+                json_content = await response.json() if 'application/json' in content_type else None
+                
+                if request.onlySuccess and response.status != 200:
+                    return Response(status=response.status if response.status else 0, url=request.url, headers={}, content=None, exception=False, proxy=request.proxy, params=request.params)
+                return Response(
                     status=response.status, url=str(response.url),
                     headers=response.headers, json=json_content,
-                    text=await response.text(), content=await response.read()
+                    text=await response.text(), content=await response.read(), exception=False,
+                    proxy=request.proxy, params=request.params
                 )
-        except (aiohttp.ClientError, aiohttp.ServerTimeoutError) as e:
-            return _Response(status=609, url=request.url, headers={}, content=str(e), exception=True)
+        except (aiohttp.ClientError, aiohttp.ServerTimeoutError, aiohttp.ClientProxyConnectionError) as e:
+            return Response(status=response.status if response.status else 0, url=request.url, headers={}, content=str(e), exception=True, proxy=request.proxy, params=request.params)
         except Exception as e:
-            return _Response(status=609, url=request.url, headers={}, content=str(e), exception=True)
-
+            return Response(status=response.status if response.status else 0, url=request.url, headers={}, content=str(e), exception=True, proxy=request.proxy, params=request.params)
```

### Comparing `multigather-0.0.5/MultiGather.egg-info/PKG-INFO` & `multigather-0.0.6/MultiGather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.5
+Version: 0.0.6
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 
 **Simple example for POST:**
 ```python
 import asyncio
 from MultiGather import Client
 from MultiGather.Types import Config, Request
 
-# Replace with the actual URL for your POST endpoint
+# Replace with the actual URL for your POST endpoint.
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
     client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
```

### Comparing `multigather-0.0.5/PKG-INFO` & `multigather-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.5
+Version: 0.0.6
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 
 **Simple example for POST:**
 ```python
 import asyncio
 from MultiGather import Client
 from MultiGather.Types import Config, Request
 
-# Replace with the actual URL for your POST endpoint
+# Replace with the actual URL for your POST endpoint.
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
     client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
```

### Comparing `multigather-0.0.5/README.md` & `multigather-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 **Simple example for POST:**
 ```python
 import asyncio
 from MultiGather import Client
 from MultiGather.Types import Config, Request
 
-# Replace with the actual URL for your POST endpoint
+# Replace with the actual URL for your POST endpoint.
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
     client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
```

