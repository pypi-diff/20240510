# Comparing `tmp/prodiapy-5.1.2.tar.gz` & `tmp/prodiapy-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-5.1.2.tar", max compression
+gzip compressed data, was "prodiapy-5.1.3.tar", max compression
```

## Comparing `prodiapy-5.1.2.tar` & `prodiapy-5.1.3.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1070 2024-03-27 07:35:41.079293 prodiapy-5.1.2/LICENSE
--rw-r--r--   0        0        0      605 2024-03-27 07:35:41.079293 prodiapy-5.1.2/README.md
--rw-r--r--   0        0        0      182 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/__init__.py
--rw-r--r--   0        0        0     1584 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/_client.py
--rw-r--r--   0        0        0      466 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/_exceptions.py
--rw-r--r--   0        0        0     1658 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/aio.py
--rw-r--r--   0        0        0      354 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__init__.py
--rw-r--r--   0        0        0      542 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3539 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     3055 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/engine.cpython-310.pyc
--rw-r--r--   0        0        0     1357 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc
--rw-r--r--   0        0        0     2883 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/general.cpython-310.pyc
--rw-r--r--   0        0        0      212 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0      799 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/response.cpython-310.pyc
--rw-r--r--   0        0        0     7010 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc
--rw-r--r--   0        0        0     5509 2024-03-27 07:35:41.079293 prodiapy-5.1.2/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc
--rw-r--r--   0        0        0     1606 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/__pycache__/upscale.cpython-310.pyc
--rw-r--r--   0        0        0      387 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      159 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/constants.py
--rw-r--r--   0        0        0     1611 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/engine.py
--rw-r--r--   0        0        0     1766 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/facerestore.py
--rw-r--r--   0        0        0     1792 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/faceswap.py
--rw-r--r--   0        0        0     6092 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/general.py
--rw-r--r--   0        0        0       58 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/logger.py
--rw-r--r--   0        0        0      439 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/response.py
--rw-r--r--   0        0        0     4643 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/stablediffusion.py
--rw-r--r--   0        0        0    14541 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/stablediffusiongeneral.py
--rw-r--r--   0        0        0      639 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/stablediffusionxl.py
--rw-r--r--   0        0        0     2020 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/upscale.py
--rw-r--r--   0        0        0      658 2024-03-27 07:35:41.083293 prodiapy-5.1.2/prodiapy/resources/utils.py
--rw-r--r--   0        0        0      401 2024-03-27 07:35:41.083293 prodiapy-5.1.2/pyproject.toml
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 prodiapy-5.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-09 20:03:10.895299 prodiapy-5.1.3/LICENSE
+-rw-r--r--   0        0        0      605 2024-05-09 20:03:10.895299 prodiapy-5.1.3/README.md
+-rw-r--r--   0        0        0      183 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/__init__.py
+-rw-r--r--   0        0        0     1629 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/_client.py
+-rw-r--r--   0        0        0      466 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/_exceptions.py
+-rw-r--r--   0        0        0     1703 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/aio.py
+-rw-r--r--   0        0        0      180 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__init__.py
+-rw-r--r--   0        0        0      542 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3539 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     3055 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/engine.cpython-310.pyc
+-rw-r--r--   0        0        0     1357 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc
+-rw-r--r--   0        0        0     2883 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/general.cpython-310.pyc
+-rw-r--r--   0        0        0      212 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0      799 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/response.cpython-310.pyc
+-rw-r--r--   0        0        0     7010 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc
+-rw-r--r--   0        0        0     5509 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc
+-rw-r--r--   0        0        0     1606 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/upscale.cpython-310.pyc
+-rw-r--r--   0        0        0      387 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/constants.py
+-rw-r--r--   0        0        0     1608 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/engine.py
+-rw-r--r--   0        0        0     1766 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/facerestore.py
+-rw-r--r--   0        0        0     1792 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/faceswap.py
+-rw-r--r--   0        0        0     6279 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/general.py
+-rw-r--r--   0        0        0       58 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/logger.py
+-rw-r--r--   0        0        0     2755 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/photomaker.py
+-rw-r--r--   0        0        0      482 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/response.py
+-rw-r--r--   0        0        0      116 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/__init__.py
+-rw-r--r--   0        0        0     4595 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/sd15.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/sdxl.py
+-rw-r--r--   0        0        0    14541 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/template.py
+-rw-r--r--   0        0        0     2020 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/upscale.py
+-rw-r--r--   0        0        0      469 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/utils.py
+-rw-r--r--   0        0        0      401 2024-05-09 20:03:10.895299 prodiapy-5.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 prodiapy-5.1.3/PKG-INFO
```

### Comparing `prodiapy-5.1.2/LICENSE` & `prodiapy-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/README.md` & `prodiapy-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/_client.py` & `prodiapy-5.1.3/prodiapy/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         )
 
         self.sd = resources.StableDiffusion(self)
         self.sdxl = resources.StableDiffusionXL(self)
 
         general = resources.General(self)
 
+        self.photomaker = general.photomaker
         self.faceswap = general.faceswap
         self.upscale = general.upscale
         self.create = general.create
         self.job = general.job
         self.constants = general.constants
         self.wait = general.wait
```

### Comparing `prodiapy-5.1.2/prodiapy/aio.py` & `prodiapy-5.1.3/prodiapy/aio.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         )
 
         self.sd = resources.AsyncStableDiffusion(self)
         self.sdxl = resources.AsyncStableDiffusionXL(self)
 
         general = resources.AsyncGeneral(self)
 
+        self.photomaker = general.photomaker
         self.faceswap = general.faceswap
         self.upscale = general.upscale
         self.create = general.create
         self.job = general.job
         self.constants = general.constants
         self.wait = general.wait
```

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/__init__.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/constants.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/constants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/engine.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/general.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/general.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/response.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/__pycache__/upscale.cpython-310.pyc` & `prodiapy-5.1.3/prodiapy/resources/__pycache__/upscale.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/engine.py` & `prodiapy-5.1.3/prodiapy/resources/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import aiohttp
 import requests
 from typing import Literal, Optional, Union
 from prodiapy.resources.utils import raise_exception
 
 
 class SyncAPIClient:
@@ -42,11 +43,7 @@
 
 class APIResource:
 
     def __init__(self, client: Union[SyncAPIClient, AsyncAPIClient]) -> None:
         self._client = client
         self._get = client.get
         self._post = client.post
-
-
-
-
```

### Comparing `prodiapy-5.1.2/prodiapy/resources/facerestore.py` & `prodiapy-5.1.3/prodiapy/resources/facerestore.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/faceswap.py` & `prodiapy-5.1.3/prodiapy/resources/faceswap.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/general.py` & `prodiapy-5.1.3/prodiapy/resources/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 
 from prodiapy.resources.engine import APIResource, SyncAPIClient, AsyncAPIClient
 from prodiapy.resources.facerestore import FaceRestore, AsyncFaceRestore
 from prodiapy.resources.faceswap import FaceSwap, AsyncFaceSwap
 from prodiapy.resources.upscale import Upscale, AsyncUpscale
+from prodiapy.resources.photomaker import PhotoMaker, AsyncPhotoMaker
 from prodiapy.resources.response import ProdiaResponse
 from prodiapy.resources.utils import form_body
 from prodiapy.resources import logger
 from prodiapy._exceptions import *
 
 import time
 import asyncio
@@ -17,14 +18,15 @@
 class General(APIResource):
     facerestore: FaceRestore.facerestore
     faceswap: FaceSwap.faceswap
     upscale: Upscale.upscale
 
     def __init__(self, client: SyncAPIClient) -> None:
         super().__init__(client)
+        self.photomaker = PhotoMaker(client).photomaker
         self.facerestore = FaceRestore(client).facerestore
         self.faceswap = FaceSwap(client).faceswap
         self.upscale = Upscale(client).upscale
 
     def create(
             self,
             endpoint: str = "/sd/generate",
@@ -102,14 +104,15 @@
 class AsyncGeneral(APIResource):
     facerestore: AsyncFaceRestore.facerestore
     faceswap: AsyncFaceSwap.faceswap
     upscale: AsyncUpscale.upscale
 
     def __init__(self, client: AsyncAPIClient) -> None:
         super().__init__(client)
+        self.photomaker = AsyncPhotoMaker(client).photomaker
         self.facerestore = AsyncFaceRestore(client).facerestore
         self.faceswap = AsyncFaceSwap(client).faceswap
         self.upscale = AsyncUpscale(client).upscale
 
     async def create(
             self,
             endpoint: str = "/sd/generate",
```

### Comparing `prodiapy-5.1.2/prodiapy/resources/stablediffusion.py` & `prodiapy-5.1.3/prodiapy/resources/stablediffusion/sd15.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
-from prodiapy.resources.engine import APIResource
 from typing import Union, Optional, Literal
-from prodiapy.resources.stablediffusiongeneral import StableDiffusionGeneral, AsyncStableDiffusionGeneral
+from prodiapy.resources.stablediffusion.template import StableDiffusionGeneral, AsyncStableDiffusionGeneral
 from prodiapy.resources.engine import SyncAPIClient, AsyncAPIClient
 from prodiapy.resources.utils import form_body
 
 
 class StableDiffusion(StableDiffusionGeneral):
     """class related to /sd endpoints, source: https://docs.prodia.com/reference/generate"""
     def __init__(self, client: SyncAPIClient) -> None:
```

### Comparing `prodiapy-5.1.2/prodiapy/resources/stablediffusiongeneral.py` & `prodiapy-5.1.3/prodiapy/resources/stablediffusion/template.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/prodiapy/resources/upscale.py` & `prodiapy-5.1.3/prodiapy/resources/upscale.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.2/PKG-INFO` & `prodiapy-5.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 5.1.2
+Version: 5.1.3
 Summary: Package for using Prodia API
 Author: zenafey
 Author-email: zenafey@eugw.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

