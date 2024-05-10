# Comparing `tmp/zyte_api-0.5.1.tar.gz` & `tmp/zyte_api-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte_api-0.5.1.tar", last modified: Tue Apr 16 08:02:00 2024, max compression
+gzip compressed data, was "zyte_api-0.5.2.tar", last modified: Fri May 10 15:20:09 2024, max compression
```

## Comparing `zyte_api-0.5.1.tar` & `zyte_api-0.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.428574 zyte_api-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-16 08:01:49.000000 zyte_api-0.5.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-16 08:01:49.000000 zyte_api-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-16 08:01:49.000000 zyte_api-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-16 08:02:00.428574 zyte_api-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-16 08:01:49.000000 zyte_api-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 08:01:49.000000 zyte_api-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 08:02:00.428574 zyte_api-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-04-16 08:01:49.000000 zyte_api-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.424574 zyte_api-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/mockserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-16 08:01:49.000000 zyte_api-0.5.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.424574 zyte_api-0.5.1/zyte_api/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.428574 zyte_api-0.5.1/zyte_api/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/aio/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-16 08:01:49.000000 zyte_api-0.5.1/zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:02:00.428574 zyte_api-0.5.1/zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 08:02:00.000000 zyte_api-0.5.1/zyte_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.593583 zyte_api-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-10 15:19:57.000000 zyte_api-0.5.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 15:19:57.000000 zyte_api-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 15:19:57.000000 zyte_api-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-10 15:20:09.593583 zyte_api-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-10 15:19:57.000000 zyte_api-0.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 15:19:57.000000 zyte_api-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 15:20:09.593583 zyte_api-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-05-10 15:19:57.000000 zyte_api-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.589583 zyte_api-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/mockserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-10 15:19:57.000000 zyte_api-0.5.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.589583 zyte_api-0.5.2/zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.593583 zyte_api-0.5.2/zyte_api/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/aio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-10 15:19:57.000000 zyte_api-0.5.2/zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:09.593583 zyte_api-0.5.2/zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:20:09.000000 zyte_api-0.5.2/zyte_api.egg-info/top_level.txt
```

### Comparing `zyte_api-0.5.1/CHANGES.rst` & `zyte_api-0.5.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes
 =======
 
+0.5.2 (2024-05-10)
+------------------
+
+* :class:`~zyte_api.RequestError` now has a :data:`~zyte_api.RequestError.query`
+  attribute with the Zyte API request parameters that caused the error.
+
 0.5.1 (2024-04-16)
 ------------------
 
 * :class:`~zyte_api.ZyteAPI` and :class:`~zyte_api.AsyncZyteAPI` sessions no
   longer need to be used as context managers, and can instead be closed with a
   ``close()`` method.
```

### Comparing `zyte_api-0.5.1/LICENSE` & `zyte_api-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/PKG-INFO` & `zyte_api-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-api
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python interface to Zyte API
 Home-page: https://github.com/zytedata/python-zyte-api
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte_api-0.5.1/README.rst` & `zyte_api-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/setup.py` & `zyte_api-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/tests/mockserver.py` & `zyte_api-0.5.2/tests/mockserver.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/tests/test_async.py` & `zyte_api-0.5.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/tests/test_main.py` & `zyte_api-0.5.2/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,28 +150,30 @@
                 api_key="a",
                 stop_on_errors=False,
             )
 
 
 @pytest.mark.asyncio
 async def test_run_stop_on_errors_true(mockserver):
-    queries = [{"url": "https://exception.example", "httpResponseBody": True}]
+    query = {"url": "https://exception.example", "httpResponseBody": True}
+    queries = [query]
     with NamedTemporaryFile("w") as output_file:
         with pytest.warns(
             DeprecationWarning, match=r"^The stop_on_errors parameter is deprecated\.$"
         ):
-            with pytest.raises(RequestError):
+            with pytest.raises(RequestError) as exc_info:
                 await run(
                     queries=queries,
                     out=output_file,
                     n_conn=1,
                     api_url=mockserver.urljoin("/"),
                     api_key="a",
                     stop_on_errors=True,
                 )
+            assert exc_info.value.query == query
 
 
 def _run(*, input, mockserver, cli_params=None):
     cli_params = cli_params or tuple()
     with NamedTemporaryFile("w") as url_list:
         url_list.write(input)
         url_list.flush()
```

### Comparing `zyte_api-0.5.1/tests/test_sync.py` & `zyte_api-0.5.2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/tests/test_utils.py` & `zyte_api-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/__main__.py` & `zyte_api-0.5.2/zyte_api/__main__.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/_async.py` & `zyte_api-0.5.2/zyte_api/_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,18 @@
         response_stats = []
         start_global = time.perf_counter()
 
         async def request():
             stats = ResponseStats.create(start_global)
             self.agg_stats.n_attempts += 1
 
+            safe_query = _process_query(query)
             post_kwargs = dict(
                 url=self.api_url + endpoint,
-                json=_process_query(query),
+                json=safe_query,
                 auth=auth,
                 headers=headers,
             )
 
             try:
                 async with self._semaphore:
                     async with post(**post_kwargs) as resp:
@@ -141,14 +142,15 @@
                             raise RequestError(
                                 request_info=resp.request_info,
                                 history=resp.history,
                                 status=resp.status,
                                 message=resp.reason,
                                 headers=resp.headers,
                                 response_content=content,
+                                query=safe_query,
                             )
 
                         response = await resp.json()
                         stats.record_read(self.agg_stats)
                         return response
             except Exception as e:
                 if not isinstance(e, RequestError):
```

### Comparing `zyte_api-0.5.1/zyte_api/_retry.py` & `zyte_api-0.5.2/zyte_api/_retry.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/_sync.py` & `zyte_api-0.5.2/zyte_api/_sync.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/_utils.py` & `zyte_api-0.5.2/zyte_api/_utils.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/aio/__init__.py` & `zyte_api-0.5.2/zyte_api/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/apikey.py` & `zyte_api-0.5.2/zyte_api/apikey.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/errors.py` & `zyte_api-0.5.2/zyte_api/errors.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/stats.py` & `zyte_api-0.5.2/zyte_api/stats.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api/utils.py` & `zyte_api-0.5.2/zyte_api/utils.py`

 * *Files identical despite different names*

### Comparing `zyte_api-0.5.1/zyte_api.egg-info/PKG-INFO` & `zyte_api-0.5.2/zyte_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-api
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python interface to Zyte API
 Home-page: https://github.com/zytedata/python-zyte-api
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte_api-0.5.1/zyte_api.egg-info/SOURCES.txt` & `zyte_api-0.5.2/zyte_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

