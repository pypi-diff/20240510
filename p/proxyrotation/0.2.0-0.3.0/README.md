# Comparing `tmp/proxyrotation-0.2.0.tar.gz` & `tmp/proxyrotation-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyrotation-0.2.0.tar", max compression
+gzip compressed data, was "proxyrotation-0.3.0.tar", max compression
```

## Comparing `proxyrotation-0.2.0.tar` & `proxyrotation-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/LICENSE
--rw-r--r--   0        0        0     1444 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/proxyrotation/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/proxyrotation/common.py
--rw-r--r--   0        0        0     1192 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/proxyrotation/modelling.py
--rw-r--r--   0        0        0     1091 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/proxyrotation/repository/__init__.py
--rw-r--r--   0        0        0     3190 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/proxyrotation/repository/async.py
--rw-r--r--   0        0        0     2344 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/proxyrotation/repository/sequential.py
--rw-r--r--   0        0        0     7316 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/proxyrotation/rotator.py
--rw-r--r--   0        0        0     1133 2024-05-06 17:10:09.824601 proxyrotation-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2214 1970-01-01 00:00:00.000000 proxyrotation-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1444 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/README.md
+-rw-r--r--   0        0        0       74 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/proxyrotation/__init__.py
+-rw-r--r--   0        0        0     1498 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/proxyrotation/common.py
+-rw-r--r--   0        0        0     1192 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/proxyrotation/modelling.py
+-rw-r--r--   0        0        0     1153 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/proxyrotation/repository/__init__.py
+-rw-r--r--   0        0        0     3528 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/proxyrotation/repository/async.py
+-rw-r--r--   0        0        0     2557 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/proxyrotation/repository/sequential.py
+-rw-r--r--   0        0        0     7440 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/proxyrotation/rotator.py
+-rw-r--r--   0        0        0     1133 2024-05-10 15:52:13.761004 proxyrotation-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2214 1970-01-01 00:00:00.000000 proxyrotation-0.3.0/PKG-INFO
```

### Comparing `proxyrotation-0.2.0/LICENSE` & `proxyrotation-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyrotation-0.2.0/README.md` & `proxyrotation-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `proxyrotation-0.2.0/proxyrotation/common.py` & `proxyrotation-0.3.0/proxyrotation/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ipaddress
 import typing
 
 from bs4 import BeautifulSoup as BS
 
-from proxyrotation.modelling import Anonymity, Proxy
+from .modelling import Anonymity, Proxy
 
 
 try:
     import aiohttp
     import aiostream
 
     has_async = True
```

### Comparing `proxyrotation-0.2.0/proxyrotation/modelling.py` & `proxyrotation-0.3.0/proxyrotation/modelling.py`

 * *Files identical despite different names*

### Comparing `proxyrotation-0.2.0/proxyrotation/repository/__init__.py` & `proxyrotation-0.3.0/proxyrotation/repository/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import importlib
 from abc import ABC, abstractmethod
 from typing import Any
 
-from proxyrotation.modelling import Proxy
+from ..modelling import Proxy
 
 
 URL_freesources = [
     "https://free-proxy-list.net",
     "https://free-proxy-list.net/uk-proxy.html",
     "https://sslproxies.org",
     "https://www.us-proxy.org",
 ]
 
 URL_sanity = "{scheme}://www.google.com"
 
 
 class abc_Repository(ABC):
     _batchsize: int
+    _timeout: float
 
-    def __init__(self, batchsize: int = 10) -> None:
+    def __init__(self, batchsize: int = 10, timeout: float = 5.0) -> None:
         self._batchsize = batchsize
+        self._timeout = timeout
 
     @abstractmethod
     def batch_download(self) -> set[Proxy]:
         """downloads batch of proxy addresses from free public sources"""
 
     @abstractmethod
     def reachability(self, available: set[Proxy]) -> tuple[set[Proxy], set[Proxy]]:
```

### Comparing `proxyrotation-0.2.0/proxyrotation/repository/async.py` & `proxyrotation-0.3.0/proxyrotation/repository/async.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import asyncio
 import platform
 from functools import reduce
 
 import aiohttp
 import aiostream
 
-from proxyrotation.common import batch_response_parsing
-from proxyrotation.modelling import Proxy
-from proxyrotation.repository import URL_freesources, URL_sanity, abc_Repository
+from ..common import batch_response_parsing
+from ..modelling import Proxy
+from ..repository import URL_freesources, URL_sanity, abc_Repository
 
 
 # https://github.com/MagicStack/uvloop/issues/14
 if platform.system().lower() != "windows":
     import uvloop
 
     #
     asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+else:
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 
 async def _batch_download(session: aiohttp.ClientSession, endpoint: str) -> set[Proxy]:
     """downloads batch of proxy addresses from a free public source"""
-    async with session.get(endpoint) as response:
-        if response.status != 200:
-            return set()
-
-        response = await response.text()
+    try:
+        async with session.get(endpoint) as response:
+            if response.status != 200:
+                return set()
+
+            response = await response.text()
+    except asyncio.TimeoutError:
+        return set()
 
     available = batch_response_parsing(response)
 
     return available
 
 
-async def _is_proxy_working(session: aiohttp.ClientSession, proxy: Proxy) -> bool:
+async def _is_proxy_working(
+    session: aiohttp.ClientSession, proxy: Proxy, timeout: float = 5.0
+) -> bool:
     """If proxy address is reachable and working"""
     try:
         async with session.get(
             URL_sanity.format(scheme=proxy.scheme),
             proxy=f"http://{proxy.peername}",
             allow_redirects=False,
-            timeout=1.0,
+            timeout=timeout,
         ) as response:
             peername = response.connection.transport.get_extra_info("peername")
 
             if not peername:
                 return False
 
             return peername[0] == proxy.host
@@ -58,42 +65,49 @@
     def batch_download(self) -> set[Proxy]:
         return asyncio.run(self._batch_download())
 
     def reachability(self, available: set[Proxy]) -> tuple[set[Proxy], set[Proxy]]:
         return asyncio.run(self._reachability(available))
 
     async def _batch_download(self) -> set[Proxy]:
-        timeout = aiohttp.ClientTimeout(sock_connect=5.0, sock_read=5.0)
+        timeout = aiohttp.ClientTimeout(
+            sock_connect=self._timeout, sock_read=self._timeout
+        )
 
         async with aiohttp.ClientSession(timeout=timeout) as session:
             available = await asyncio.gather(
                 *[_batch_download(session, endpoint) for endpoint in URL_freesources]
             )
 
         available = reduce(lambda x, y: x | y, available)
         return available
 
     async def _reachability(
         self, available: set[Proxy]
     ) -> tuple[set[Proxy], set[Proxy]]:
-        timeout = aiohttp.ClientTimeout(sock_connect=5.0, sock_read=5.0)
+        timeout = aiohttp.ClientTimeout(
+            sock_connect=self._timeout, sock_read=self._timeout
+        )
 
         positive = set()
         negative = set()
 
         batchsize = self._batchsize if self._batchsize > 0 else len(available)
         batchsize = min(batchsize, len(available))
 
         async with aiohttp.ClientSession(timeout=timeout) as session:
             iterator = aiostream.stream.iterate(available)
             iterator = aiostream.stream.chunks(iterator, batchsize)
 
             async with iterator.stream() as chunkset:
                 async for batchset in chunkset:
                     response = await asyncio.gather(
-                        *[_is_proxy_working(session, proxy) for proxy in batchset]
+                        *[
+                            _is_proxy_working(session, proxy, self._timeout)
+                            for proxy in batchset
+                        ]
                     )
 
                     for x in zip(response, batchset):
                         positive.add(x[1]) if x[0] else negative.add(x[1])
 
         return positive, negative
```

### Comparing `proxyrotation-0.2.0/proxyrotation/repository/sequential.py` & `proxyrotation-0.3.0/proxyrotation/repository/sequential.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-from functools import reduce
+from functools import partial, reduce
 
 import requests
 from more_itertools import chunked
 
-from proxyrotation.common import batch_response_parsing
-from proxyrotation.modelling import Proxy
-from proxyrotation.repository import URL_freesources, URL_sanity, abc_Repository
+from ..common import batch_response_parsing
+from ..modelling import Proxy
+from ..repository import URL_freesources, URL_sanity, abc_Repository
 
 
-def _batch_download(endpoint: str) -> set[Proxy]:
+def _batch_download(endpoint: str, timeout: float = 5.0) -> set[Proxy]:
     """downloads batch of proxy addresses from a free public source"""
-    with requests.get(endpoint, timeout=(5.0, 5.0)) as response:
-        if response.status_code != 200:
-            return set()
-
-        response = response.text
+    try:
+        with requests.get(endpoint, timeout=(timeout, timeout)) as response:
+            if response.status_code != 200:
+                return set()
+
+            response = response.text
+    except requests.exceptions.ReadTimeout:
+        return set()
 
     available = batch_response_parsing(response)
 
     return available
 
 
-def _is_proxy_working(proxy: Proxy) -> bool:
+def _is_proxy_working(proxy: Proxy, timeout: float = 5.0) -> bool:
     """If proxy address is reachable and working"""
     try:
         with requests.get(
             URL_sanity.format(scheme=proxy.scheme),
             proxies={"http": proxy.peername, "https": proxy.peername},
             allow_redirects=False,
-            timeout=1.0,
+            timeout=timeout,
             stream=True,
         ) as response:
             socket = response.raw.connection.sock
 
             if not socket:
                 return False
 
@@ -51,26 +54,30 @@
     def batch_download(self) -> set[Proxy]:
         return self._batch_download()
 
     def reachability(self, available: set[Proxy]) -> tuple[set[Proxy], set[Proxy]]:
         return self._reachability(available)
 
     def _batch_download(self) -> set[Proxy]:
-        available = map(_batch_download, URL_freesources)
+        f = partial(_batch_download, timeout=self._timeout)
+
+        available = map(f, URL_freesources)
         available = reduce(lambda x, y: x | y, available)
 
         return available
 
     def _reachability(self, available: set[Proxy]) -> tuple[set[Proxy], set[Proxy]]:
         positive = set()
         negative = set()
 
         batchsize = self._batchsize if self._batchsize > 0 else len(available)
         batchsize = min(batchsize, len(available))
 
+        f = partial(_is_proxy_working, timeout=self._timeout)
+
         for batchset in chunked(available, batchsize):
-            response = map(_is_proxy_working, batchset)
+            response = map(f, batchset)
 
             for x in zip(response, batchset):
                 positive.add(x[1]) if x[0] else negative.add(x[1])
 
         return positive, negative
```

### Comparing `proxyrotation-0.2.0/proxyrotation/rotator.py` & `proxyrotation-0.3.0/proxyrotation/rotator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pathlib
 import pickle
 import random
 import typing
 from datetime import datetime
+from typing import Any
 
-from proxyrotation.common import has_async
-from proxyrotation.modelling import Anonymity, Proxy
-from proxyrotation.repository import abc_Repository, from_name
+from .common import has_async
+from .modelling import Anonymity, Proxy
+from .repository import abc_Repository, from_name
 
 
 _cachefile = "proxyrotation.pickle"
 
 
 class ProxyRotator:
     """class that automatically rotates proxy addresses for HTTP requests
@@ -38,14 +39,15 @@
         cachedir: The path to the cache dir. none disables caching
         countrycodeset: desired alpha-2 country codes. none disables filtering
         livecheck: whether non-working proxy addresses should be live checked while fetching
         maxshape: The max number of available proxy addresses to keep. 0 means unbounded
         repository: The repository to fetch free proxy address sources from; could be "async" or "sequential"
         schedule: The automatic refresh interval (seconds). 0.0 disables auto-refresh
         secure: whether secure connections (HTTPS) should be enforced
+        kwargs: The repository additional kwargs
 
     Raises:
         If cache dir is provided, but cache is invalid for criteria
     """
 
     _anonymity: typing.Optional[Anonymity]
     _blockedset: set[Proxy]
@@ -64,30 +66,33 @@
         self,
         *,
         anonymity: typing.Optional[Anonymity] = None,
         cachedir: typing.Optional[str] = None,
         countrycodeset: typing.Optional[set[str]] = None,
         livecheck: bool = True,
         maxshape: int = 0,
-        repository: typing.Union[str, abc_Repository] = (
-            "async" if has_async else "sequential"
-        ),
+        repository: typing.Union[
+            typing.Literal["async", "sequential"], abc_Repository
+        ] = ("async" if has_async else "sequential"),
         schedule: float = 0.0,
         secure: bool = True,
+        **kwargs: Any,
     ):
         self._anonymity = anonymity
         self._blockedset = set()
         self._cachedir = None
         self._countrycodeset = countrycodeset
         self._downloaded = None
         self._livecheck = livecheck
         self._maxshape = maxshape
         self._crawledset = set()
         self._repository = (
-            from_name(repository) if isinstance(repository, str) else repository
+            from_name(repository, **kwargs)
+            if isinstance(repository, str)
+            else repository
         )
         self._schedule = schedule
         self._secure = secure
         self._selected = None
 
         if cachedir:
             self._cachedir = pathlib.Path(cachedir).expanduser().resolve()
```

### Comparing `proxyrotation-0.2.0/pyproject.toml` & `proxyrotation-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "proxyrotation"
-version = "0.2.0"
+version = "0.3.0"
 description = "automatic free proxy rotation"
 authors = ["Federico Minutoli <fede97.minutoli@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["proxy-rotation", "web-scraping", "anonymity"]
 
 [tool.poetry.dependencies]
```

### Comparing `proxyrotation-0.2.0/PKG-INFO` & `proxyrotation-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyrotation
-Version: 0.2.0
+Version: 0.3.0
 Summary: automatic free proxy rotation
 License: MIT
 Keywords: proxy-rotation,web-scraping,anonymity
 Author: Federico Minutoli
 Author-email: fede97.minutoli@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

