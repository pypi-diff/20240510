# Comparing `tmp/uiautodev-0.3.4.tar.gz` & `tmp/uiautodev-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautodev-0.3.4.tar", max compression
+gzip compressed data, was "uiautodev-0.3.5.tar", max compression
```

## Comparing `uiautodev-0.3.4.tar` & `uiautodev-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1068 2024-05-09 03:46:25.038415 uiautodev-0.3.4/LICENSE
--rw-r--r--   0        0        0     1191 2024-05-09 03:46:25.038415 uiautodev-0.3.4/README.md
--rw-r--r--   0        0        0     1091 2024-05-09 03:46:38.174371 uiautodev-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      267 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/__init__.py
--rw-r--r--   0        0        0      176 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/__main__.py
--rw-r--r--   0        0        0     2491 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/app.py
--rw-r--r--   0        0        0     1773 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/appium_proxy.py
--rw-r--r--   0        0        0     3919 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/case.py
--rw-r--r--   0        0        0     6234 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/cli.py
--rw-r--r--   0        0        0     4562 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/command_proxy.py
--rw-r--r--   0        0        0     1587 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/command_types.py
--rw-r--r--   0        0        0      534 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/common.py
--rw-r--r--   0        0        0     7043 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/android.py
--rw-r--r--   0        0        0     5308 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/appium.py
--rw-r--r--   0        0        0     2048 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/base_driver.py
--rw-r--r--   0        0        0     4353 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/ios.py
--rw-r--r--   0        0        0     2422 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/mock.py
--rw-r--r--   0        0        0  3675062 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
--rw-r--r--   0        0        0     8351 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/driver/udt/udt.py
--rw-r--r--   0        0        0      465 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/exceptions.py
--rw-r--r--   0        0        0      717 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/model.py
--rw-r--r--   0        0        0     2370 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/provider.py
--rw-r--r--   0        0        0     3862 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/router/device.py
--rw-r--r--   0        0        0      891 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/router/xml.py
--rw-r--r--   0        0        0     1240 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/static/demo.html
--rw-r--r--   0        0        0     4785 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/utils/common.py
--rw-r--r--   0        0        0      637 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/utils/exceptions.py
--rw-r--r--   0        0        0    17386 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/utils/usbmux.py
--rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 uiautodev-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-09 08:18:31.049571 uiautodev-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1191 2024-05-09 08:18:31.049571 uiautodev-0.3.5/README.md
+-rw-r--r--   0        0        0     1126 2024-05-09 08:18:49.505599 uiautodev-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      267 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/__main__.py
+-rw-r--r--   0        0        0     2491 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/app.py
+-rw-r--r--   0        0        0     1773 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/appium_proxy.py
+-rw-r--r--   0        0        0     3919 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/case.py
+-rw-r--r--   0        0        0     6234 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/cli.py
+-rw-r--r--   0        0        0     4562 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/command_proxy.py
+-rw-r--r--   0        0        0     1587 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/command_types.py
+-rw-r--r--   0        0        0      552 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/common.py
+-rw-r--r--   0        0        0     7043 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/driver/android.py
+-rw-r--r--   0        0        0     5308 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/driver/appium.py
+-rw-r--r--   0        0        0     2048 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/driver/base_driver.py
+-rw-r--r--   0        0        0     4353 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/driver/ios.py
+-rw-r--r--   0        0        0     2422 2024-05-09 08:18:31.053571 uiautodev-0.3.5/uiautodev/driver/mock.py
+-rw-r--r--   0        0        0  3675062 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
+-rw-r--r--   0        0        0     8351 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/driver/udt/udt.py
+-rw-r--r--   0        0        0      465 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/exceptions.py
+-rw-r--r--   0        0        0      717 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/model.py
+-rw-r--r--   0        0        0     2370 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/provider.py
+-rw-r--r--   0        0        0     4116 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/router/device.py
+-rw-r--r--   0        0        0      891 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/router/xml.py
+-rw-r--r--   0        0        0     1240 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/static/demo.html
+-rw-r--r--   0        0        0     4785 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/utils/common.py
+-rw-r--r--   0        0        0      637 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/utils/exceptions.py
+-rw-r--r--   0        0        0    17386 2024-05-09 08:18:31.065571 uiautodev-0.3.5/uiautodev/utils/usbmux.py
+-rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 uiautodev-0.3.5/PKG-INFO
```

### Comparing `uiautodev-0.3.4/LICENSE` & `uiautodev-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/README.md` & `uiautodev-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/pyproject.toml` & `uiautodev-0.3.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uiautodev"
-version = "0.3.4"
+version = "0.3.5"
 description = "Mobile UI Automation, include UI hierarchy inspector, script recorder"
 homepage = "https://uiauto.dev"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 click = "^8.1.7"
 pygments = ">=2"
 httpretty = {version = "^1.1.4", optional = true}
 appium-python-client = {version = "^4.0.0", optional = true}
 uiautomator2 = ">=2"
 httpx = "*"
 fastapi = "^0.111.0"
-uvicorn = "*"
+uvicorn = {version = "*", extras = ["standard"]}
 poetry = "^1.8.2"
 
 [tool.poetry.extras]
 appium = ["appium-python-client", "httppretty"]
 
 [tool.poetry.scripts]
 "uiauto.dev" = "uiautodev.__main__:main"
```

### Comparing `uiautodev-0.3.4/uiautodev/app.py` & `uiautodev-0.3.5/uiautodev/app.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/appium_proxy.py` & `uiautodev-0.3.5/uiautodev/appium_proxy.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/case.py` & `uiautodev-0.3.5/uiautodev/case.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/cli.py` & `uiautodev-0.3.5/uiautodev/cli.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/command_proxy.py` & `uiautodev-0.3.5/uiautodev/command_proxy.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/command_types.py` & `uiautodev-0.3.5/uiautodev/command_types.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/common.py` & `uiautodev-0.3.5/uiautodev/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import locale
 
 
 def is_chinese_language() -> bool:
     language_code, _ = locale.getdefaultlocale()
     
     # Check if the language code starts with 'zh' (Chinese)
-    if language_code.startswith('zh'):
+    if language_code and language_code.startswith('zh'):
         return True
     else:
         return False
     
     
 def get_webpage_url() -> str:
     web_url = "https://uiauto.dev"
```

### Comparing `uiautodev-0.3.4/uiautodev/driver/android.py` & `uiautodev-0.3.5/uiautodev/driver/android.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/driver/appium.py` & `uiautodev-0.3.5/uiautodev/driver/appium.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/driver/base_driver.py` & `uiautodev-0.3.5/uiautodev/driver/base_driver.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/driver/ios.py` & `uiautodev-0.3.5/uiautodev/driver/ios.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/driver/mock.py` & `uiautodev-0.3.5/uiautodev/driver/mock.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk` & `uiautodev-0.3.5/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/driver/udt/udt.py` & `uiautodev-0.3.5/uiautodev/driver/udt/udt.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/model.py` & `uiautodev-0.3.5/uiautodev/model.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/provider.py` & `uiautodev-0.3.5/uiautodev/provider.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/router/device.py` & `uiautodev-0.3.5/uiautodev/router/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Created on Fri Mar 01 2024 14:00:10 by codeskyblue
 """
 
 import io
+import logging
 from typing import Any, List
 
 from fastapi import APIRouter, Response
 from pydantic import BaseModel
 
 from uiautodev import command_proxy
 from uiautodev.command_types import Command, CurrentAppResponse, InstallAppRequest, InstallAppResponse, TapRequest
 from uiautodev.model import DeviceInfo, Node, ShellResponse
 from uiautodev.provider import BaseProvider
 
 
+logger = logging.getLogger(__name__)
+
 class AndroidShellPayload(BaseModel):
     command: str
 
 
 def make_router(provider: BaseProvider) -> APIRouter:
     router = APIRouter()
 
@@ -27,25 +30,27 @@
     def _list() -> List[DeviceInfo]:
         """List of Android devices"""
         try:
             return provider.list_devices()
         except NotImplementedError as e:
             return Response(content="list_devices not implemented", media_type="text/plain", status_code=501)
         except Exception as e:
+            logger.exception("list_devices failed")
             return Response(content=str(e), media_type="text/plain", status_code=500)
 
     @router.post("/{serial}/shell")
     def android_shell(serial: str, payload: AndroidShellPayload) -> ShellResponse:
         """Run a shell command on an Android device"""
         try:
             driver = provider.get_device_driver(serial)
             return driver.shell(payload.command)
         except NotImplementedError as e:
             return Response(content="shell not implemented", media_type="text/plain", status_code=501)
         except Exception as e:
+            logger.exception("shell failed")
             return ShellResponse(output="", error=str(e))
 
     @router.get(
         "/{serial}/screenshot/{id}",
         responses={200: {"content": {"image/jpeg": {}}}},
         response_class=Response,
     )
@@ -55,24 +60,26 @@
             driver = provider.get_device_driver(serial)
             pil_img = driver.screenshot(id)
             buf = io.BytesIO()
             pil_img.save(buf, format="JPEG")
             image_bytes = buf.getvalue()
             return Response(content=image_bytes, media_type="image/jpeg")
         except Exception as e:
+            logger.exception("screenshot failed")
             return Response(content=str(e), media_type="text/plain", status_code=500)
 
     @router.get("/{serial}/hierarchy")
     def dump_hierarchy(serial: str) -> Node:
         """Dump the view hierarchy of an Android device"""
         try:
             driver = provider.get_device_driver(serial)
             xml_data, hierarchy = driver.dump_hierarchy()
             return hierarchy
         except Exception as e:
+            logger.exception("dump_hierarchy failed")
             return Response(content=str(e), media_type="text/plain", status_code=500)
     
     @router.post('/{serial}/command/tap')
     def command_tap(serial: str, params: TapRequest):
         """Run a command on the device"""
         driver = provider.get_device_driver(serial)
         command_proxy.tap(driver, params)
```

### Comparing `uiautodev-0.3.4/uiautodev/router/xml.py` & `uiautodev-0.3.5/uiautodev/router/xml.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/static/demo.html` & `uiautodev-0.3.5/uiautodev/static/demo.html`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/utils/common.py` & `uiautodev-0.3.5/uiautodev/utils/common.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/utils/exceptions.py` & `uiautodev-0.3.5/uiautodev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/uiautodev/utils/usbmux.py` & `uiautodev-0.3.5/uiautodev/utils/usbmux.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.4/PKG-INFO` & `uiautodev-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiautodev
-Version: 0.3.4
+Version: 0.3.5
 Summary: Mobile UI Automation, include UI hierarchy inspector, script recorder
 Home-page: https://uiauto.dev
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 Requires-Dist: httpretty (>=1.1.4,<2.0.0)
 Requires-Dist: httpx
 Requires-Dist: lxml
 Requires-Dist: pillow
 Requires-Dist: poetry (>=1.8.2,<2.0.0)
 Requires-Dist: pygments (>=2)
 Requires-Dist: uiautomator2 (>=2)
-Requires-Dist: uvicorn
+Requires-Dist: uvicorn[standard]
 Description-Content-Type: text/markdown
 
 # uiautodev
 [![codecov](https://codecov.io/gh/codeskyblue/appinspector/graph/badge.svg?token=aLTg4VOyQH)](https://codecov.io/gh/codeskyblue/appinspector)
 [![PyPI version](https://badge.fury.io/py/uiautodev.svg)](https://badge.fury.io/py/uiautodev)
 
 https://uiauto.dev
```

