# Comparing `tmp/multigather-0.0.6.tar.gz` & `tmp/multigather-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Admin\Desktop\testmygather\dist\.tmp-ksx_39bd\multigather-0.0.6.tar", last modified: Fri May 10 08:27:02 2024, max compression
+gzip compressed data, was "C:\Users\Admin\Desktop\testmygather\dist\.tmp-5nikshxa\multigather-0.0.7.tar", last modified: Fri May 10 08:52:10 2024, max compression
```

## Comparing `multigather-0.0.6.tar` & `multigather-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:02.603116 multigather-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:02.572134 multigather-0.0.6/MultiGather/
--rw-rw-rw-   0        0        0     2389 2024-05-10 08:24:56.000000 multigather-0.0.6/MultiGather/Client.py
--rw-rw-rw-   0        0        0      901 2024-05-10 08:24:56.000000 multigather-0.0.6/MultiGather/Types.py
--rw-rw-rw-   0        0        0      232 2024-05-10 08:24:56.000000 multigather-0.0.6/MultiGather/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:02.596122 multigather-0.0.6/MultiGather.egg-info/
--rw-rw-rw-   0        0        0     2257 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-10 08:27:02.000000 multigather-0.0.6/MultiGather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2257 2024-05-10 08:27:02.600119 multigather-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2024-05-10 08:24:56.000000 multigather-0.0.6/README.md
--rw-rw-rw-   0        0        0      504 2024-05-10 08:26:07.000000 multigather-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 08:27:02.603116 multigather-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 08:52:10.393503 multigather-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-10 08:52:10.386496 multigather-0.0.7/MultiGather.egg-info/
+-rw-rw-rw-   0        0        0     2268 2024-05-10 08:52:10.000000 multigather-0.0.7/MultiGather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-05-10 08:52:10.000000 multigather-0.0.7/MultiGather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:52:10.000000 multigather-0.0.7/MultiGather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:52:10.000000 multigather-0.0.7/MultiGather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2268 2024-05-10 08:52:10.387494 multigather-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1769 2024-05-10 08:51:22.000000 multigather-0.0.7/README.md
+-rw-rw-rw-   0        0        0      504 2024-05-10 08:48:01.000000 multigather-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:52:10.394492 multigather-0.0.7/setup.cfg
```

### Comparing `multigather-0.0.6/MultiGather.egg-info/PKG-INFO` & `multigather-0.0.7/MultiGather.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.6
+Version: 0.0.7
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,25 +18,25 @@
 ```bash
 pip install MultiGather
 ```
 
 **Simple example for POST:**
 ```python
 import asyncio
-from MultiGather import Client
+from MultiGather.Client import Connection
 from MultiGather.Types import Config, Request
 
 # Replace with the actual URL for your POST endpoint.
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
-    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a POST request object
     post_request = Request(method="POST", url=url, json=data, amount=5) ## gonna send 5 requests
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(post_request)
 
@@ -45,21 +45,22 @@
         print(f"POST response status: {response.status}")
 
 asyncio.run(main())
 ```
 **Simple example for GET:**
 ```python
 import asyncio
-from MultiGather import Client
+from MultiGather.Client import Connection
 from MultiGather.Types import Config, Request
-# Replace with the actual URL for your GET endpoint
+
+# Replace with the actual URL for your GET endpoint.
 url = "https://your-api-endpoint/posts"
 
 async def main():
-    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a GET request object
     get_request = Request(method="GET", url=url, amount=5) # send 5 requests.
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(get_request)
```

### Comparing `multigather-0.0.6/PKG-INFO` & `multigather-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.6
+Version: 0.0.7
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,25 +18,25 @@
 ```bash
 pip install MultiGather
 ```
 
 **Simple example for POST:**
 ```python
 import asyncio
-from MultiGather import Client
+from MultiGather.Client import Connection
 from MultiGather.Types import Config, Request
 
 # Replace with the actual URL for your POST endpoint.
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
-    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a POST request object
     post_request = Request(method="POST", url=url, json=data, amount=5) ## gonna send 5 requests
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(post_request)
 
@@ -45,21 +45,22 @@
         print(f"POST response status: {response.status}")
 
 asyncio.run(main())
 ```
 **Simple example for GET:**
 ```python
 import asyncio
-from MultiGather import Client
+from MultiGather.Client import Connection
 from MultiGather.Types import Config, Request
-# Replace with the actual URL for your GET endpoint
+
+# Replace with the actual URL for your GET endpoint.
 url = "https://your-api-endpoint/posts"
 
 async def main():
-    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a GET request object
     get_request = Request(method="GET", url=url, amount=5) # send 5 requests.
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(get_request)
```

### Comparing `multigather-0.0.6/README.md` & `multigather-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 ```bash
 pip install MultiGather
 ```
 
 **Simple example for POST:**
 ```python
 import asyncio
-from MultiGather import Client
+from MultiGather.Client import Connection
 from MultiGather.Types import Config, Request
 
 # Replace with the actual URL for your POST endpoint.
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
-    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a POST request object
     post_request = Request(method="POST", url=url, json=data, amount=5) ## gonna send 5 requests
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(post_request)
 
@@ -32,27 +32,28 @@
         print(f"POST response status: {response.status}")
 
 asyncio.run(main())
 ```
 **Simple example for GET:**
 ```python
 import asyncio
-from MultiGather import Client
+from MultiGather.Client import Connection
 from MultiGather.Types import Config, Request
-# Replace with the actual URL for your GET endpoint
+
+# Replace with the actual URL for your GET endpoint.
 url = "https://your-api-endpoint/posts"
 
 async def main():
-    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a GET request object
     get_request = Request(method="GET", url=url, amount=5) # send 5 requests.
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(get_request)
 
     # Print the status code for each response
     for response in responses:
         print(f"GET response status: {response.status}")
 
 asyncio.run(main())
-```
+```
```

