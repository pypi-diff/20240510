# Comparing `tmp/ahk-1.7.1.tar.gz` & `tmp/ahk-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.7.1.tar", last modified: Sun Apr 21 20:29:50 2024, max compression
+gzip compressed data, was "ahk-1.7.2.tar", last modified: Fri May 10 07:59:38 2024, max compression
```

## Comparing `ahk-1.7.1.tar` & `ahk-1.7.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:50.134316 ahk-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-21 20:29:43.000000 ahk-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-21 20:29:43.000000 ahk-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-04-21 20:29:50.134316 ahk-1.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:50.130316 ahk-1.7.1/ahk/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:50.134316 ahk-1.7.1/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   206741 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    47611 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17091 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:50.134316 ahk-1.7.1/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   199988 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    42661 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:50.134316 ahk-1.7.1/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/templates/daemon-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/templates/hotkeys-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-21 20:29:43.000000 ahk-1.7.1/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:50.134316 ahk-1.7.1/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-04-21 20:29:50.000000 ahk-1.7.1/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-21 20:29:50.000000 ahk-1.7.1/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:29:50.000000 ahk-1.7.1/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-21 20:29:50.000000 ahk-1.7.1/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 20:29:50.000000 ahk-1.7.1/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-21 20:29:43.000000 ahk-1.7.1/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:50.134316 ahk-1.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-04-21 20:29:43.000000 ahk-1.7.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-21 20:29:43.000000 ahk-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-21 20:29:50.134316 ahk-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 20:29:43.000000 ahk-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.646675 ahk-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-10 07:59:31.000000 ahk-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 07:59:31.000000 ahk-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-10 07:59:38.646675 ahk-1.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.638675 ahk-1.7.2/ahk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   206949 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47647 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   200233 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42697 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/daemon-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/hotkeys-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-10 07:59:31.000000 ahk-1.7.2/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-05-10 07:59:31.000000 ahk-1.7.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 07:59:31.000000 ahk-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-10 07:59:38.646675 ahk-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:59:31.000000 ahk-1.7.2/setup.py
```

### Comparing `ahk-1.7.1/LICENSE` & `ahk-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/PKG-INFO` & `ahk-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.7.1
+Version: 1.7.2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.7.1/ahk/__init__.py` & `ahk-1.7.2/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/_async/engine.py` & `ahk-1.7.2/ahk/_async/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,43 +29,37 @@
 from .._utils import MsgBoxButtons
 from .._utils import MsgBoxDefaultButton
 from .._utils import MsgBoxIcon
 from .._utils import MsgBoxModality
 from .._utils import MsgBoxOtherOptions
 from .._utils import type_escape
 from ..directives import Directive
-
-if sys.version_info < (3, 10):
-    from typing_extensions import TypeAlias
-else:
-    from typing import TypeAlias
-
-from ..extensions import (
-    Extension,
-    _ExtensionMethodRegistry,
-    _extension_registry,
-    _resolve_extensions,
-)
+from ..extensions import _extension_registry
+from ..extensions import _ExtensionMethodRegistry
+from ..extensions import _resolve_extensions
+from ..extensions import Extension
 from ..keys import Key
 from .transport import AsyncDaemonProcessTransport
 from .transport import AsyncFutureResult
 from .transport import AsyncTransport
 from .window import AsyncControl
 from .window import AsyncWindow
+from ahk._types import _BUTTONS
+from ahk._types import Coordinates
+from ahk._types import CoordModeRelativeTo
+from ahk._types import CoordModeTargets
+from ahk._types import MouseButton
+from ahk._types import Position
+from ahk._types import SendMode
+from ahk._types import TitleMatchMode
 
-from ahk._types import (
-    Position,
-    CoordModeTargets,
-    CoordModeRelativeTo,
-    TitleMatchMode,
-    _BUTTONS,
-    MouseButton,
-    SendMode,
-    Coordinates,
-)
+if sys.version_info < (3, 10):
+    from typing_extensions import TypeAlias
+else:
+    from typing import TypeAlias
 
 async_sleep = asyncio.sleep  # unasync: remove
 sleep = time.sleep
 
 AsyncFilterFunc: TypeAlias = Callable[[AsyncWindow], Awaitable[bool]]  # unasync: remove
 SyncFilterFunc: TypeAlias = Callable[[AsyncWindow], bool]
 
@@ -88,15 +82,15 @@
     if isinstance(button, str):
         button = button.lower()
 
     if button in _BUTTONS:
         resolved_button = _BUTTONS[button]
     elif isinstance(button, int) and button > 3:
         #  for addtional mouse buttons
-        resolved_button = f'X{button-3}'
+        resolved_button = f'X{button - 3}'
     else:
         assert isinstance(button, str)
         resolved_button = button
     return resolved_button
 
 
 T_AHKVersion = TypeVar('T_AHKVersion', bound=Optional[Literal['v1', 'v2']])
@@ -1085,27 +1079,27 @@
             await self.send_input(key.UP, blocking=True)
             return None
         else:
             return await self.send_input(key.UP, blocking=False)
 
     # fmt: off
     @overload
-    async def key_wait(self, key_name: str, *, timeout: Optional[int] = None, logical_state: bool = False, released: bool = False) -> bool: ...
+    async def key_wait(self, key_name: str, *, timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False) -> bool: ...
     @overload
-    async def key_wait(self, key_name: str, *, blocking: Literal[True], timeout: Optional[int] = None, logical_state: bool = False, released: bool = False) -> bool: ...
+    async def key_wait(self, key_name: str, *, blocking: Literal[True], timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False) -> bool: ...
     @overload
-    async def key_wait(self, key_name: str, *, blocking: Literal[False], timeout: Optional[int] = None, logical_state: bool = False, released: bool = False) -> AsyncFutureResult[bool]: ...
+    async def key_wait(self, key_name: str, *, blocking: Literal[False], timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False) -> AsyncFutureResult[bool]: ...
     @overload
-    async def key_wait(self, key_name: str, *, timeout: Optional[int] = None, logical_state: bool = False, released: bool = False, blocking: bool = True) -> Union[bool, AsyncFutureResult[bool]]: ...
+    async def key_wait(self, key_name: str, *, timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False, blocking: bool = True) -> Union[bool, AsyncFutureResult[bool]]: ...
     # fmt: on
     async def key_wait(
         self,
         key_name: str,
         *,
-        timeout: Optional[int] = None,
+        timeout: Optional[int | float] = None,
         logical_state: bool = False,
         released: bool = False,
         blocking: bool = True,
     ) -> Union[bool, AsyncFutureResult[bool]]:
         """
         Analog for `KeyWait <https://www.autohotkey.com/docs/commands/KeyWait.htm>`_
         """
```

### Comparing `ahk-1.7.1/ahk/_async/transport.py` & `ahk-1.7.2/ahk/_async/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ahk._hotkey import Hotkey
 from ahk._hotkey import Hotstring
 from ahk._hotkey import ThreadedHotkeyTransport
 from ahk._types import Coordinates
 from ahk._types import FunctionName
 from ahk._types import Position
 from ahk._utils import _version_detection_script
+from ahk._utils import try_remove
 from ahk.directives import Directive
 from ahk.exceptions import AHKProtocolError
 from ahk.extensions import _resolve_includes
 from ahk.extensions import Extension
 from ahk.message import _message_registry
 from ahk.message import RequestMessage
 from ahk.message import ResponseMessage
@@ -664,23 +665,23 @@
                 script_text = self._render_script()
                 with tempfile.NamedTemporaryFile(
                     mode='w', prefix='python-ahk-', suffix='.ahk', delete=False
                 ) as tempscriptfile:
                     tempscriptfile.write(script_text)  # XXX: can we make this async?
                 self._temp_script = tempscriptfile.name
                 daemon_script = self._temp_script
-                atexit.register(os.remove, tempscriptfile.name)
+                atexit.register(try_remove, tempscriptfile.name)
             else:
                 daemon_script = self._temp_script
         else:
             script_text = self._render_script(template=template, **template_kwargs)
             with tempfile.NamedTemporaryFile(mode='w', prefix='python-ahk-', suffix='.ahk', delete=False) as tempscript:
                 tempscript.write(script_text)
             daemon_script = tempscript.name
-            atexit.register(os.remove, tempscript.name)
+            atexit.register(try_remove, tempscript.name)
         runargs = [self._executable_path, '/CP65001', '/ErrorStdOut', daemon_script]
         proc = AsyncAHKProcess(runargs=runargs)
         await proc.start()
         return proc
 
     async def _send_nonblocking(
         self, request: RequestMessage, engine: Optional[AsyncAHK[Any]] = None
```

### Comparing `ahk-1.7.1/ahk/_async/window.py` & `ahk-1.7.2/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/_constants.py` & `ahk-1.7.2/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/_hotkey.py` & `ahk-1.7.2/ahk/_hotkey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 from __future__ import annotations
 
 import atexit
 import functools
-import os
+import logging
 import re
 import subprocess
 import sys
+import tempfile
 import threading
 import time
 import warnings
 from abc import ABC
 from abc import abstractmethod
 from base64 import b64encode
+from queue import Queue
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Protocol
 from typing import runtime_checkable
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import jinja2
 
+from ._constants import HOTKEYS_SCRIPT_TEMPLATE as _HOTKEY_SCRIPT
+from ._constants import HOTKEYS_SCRIPT_V2_TEMPLATE as _HOTKEY_V2_SCRIPT
 from .directives import Directive
+from ahk._utils import hotkey_escape
+from ahk._utils import try_remove
 
 if sys.version_info >= (3, 10):
     from typing import ParamSpec
 else:
     from typing_extensions import ParamSpec
 
 
-import logging
-import tempfile
-from queue import Queue
-
-from ahk._utils import hotkey_escape
-from ._constants import HOTKEYS_SCRIPT_TEMPLATE as _HOTKEY_SCRIPT, HOTKEYS_SCRIPT_V2_TEMPLATE as _HOTKEY_V2_SCRIPT
-
 P_HotkeyCallbackParam = ParamSpec('P_HotkeyCallbackParam')
 T_HotkeyCallbackReturn = TypeVar('T_HotkeyCallbackReturn')
 
 _KEEPALIVE_SENTINEL = b'\xee\x80\x80'
 
 _CLIPBOARD_SENTINEL = '\ue001'
 
@@ -320,39 +319,41 @@
             directives=self._directives,
         )
         return ret
 
     def listener(self) -> None:
         hotkey_script_contents = self._render_hotkey_template()
         logging.debug('hotkey script contents:\n%s', hotkey_script_contents)
-        with tempfile.TemporaryDirectory(prefix='python-ahk') as tmpdirname:
-            exc_file = os.path.join(tmpdirname, 'executor.ahk')
-            with open(exc_file, 'w') as f:
-                f.write(hotkey_script_contents)
-            self._proc = subprocess.Popen(
-                [self._executable_path, '/CP65001', '/ErrorStdOut', exc_file],
-                stdin=subprocess.PIPE,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.STDOUT,
-            )
-            atexit.register(kill, self._proc)
-            assert self._proc.stdout is not None
-            assert self._proc.stdin is not None
-            while self._running:
-                line = self._proc.stdout.readline()
-                if line.rstrip(b'\n') == _KEEPALIVE_SENTINEL:
-                    logging.debug('keepalive received')
-                    self._proc.stdin.write(b'\xee\x80\x80\n')
-                    self._proc.stdin.flush()
-                    continue
-                if not line.strip():
-                    logging.debug('Listener: Process probably died, exiting')
-                    break
-                logging.debug(f'Received {line!r}')
-                self._callback_queue.put_nowait(line.decode('UTF-8').strip())
+        with tempfile.NamedTemporaryFile(mode='w', prefix='python-ahk-hotkeys-', suffix='.ahk', delete=False) as f:
+            f.write(hotkey_script_contents)
+        atexit.register(try_remove, f.name)
+        self._proc = subprocess.Popen(
+            [self._executable_path, '/CP65001', '/ErrorStdOut', f.name],
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+        )
+        atexit.register(kill, self._proc)
+        assert self._proc.stdout is not None
+        assert self._proc.stdin is not None
+        while self._running:
+            line = self._proc.stdout.readline()
+            if line.rstrip(b'\n') == _KEEPALIVE_SENTINEL:
+                logging.debug('keepalive received')
+                self._proc.stdin.write(b'\xee\x80\x80\n')
+                self._proc.stdin.flush()
+                continue
+            if not line.strip():
+                logging.debug('Listener: Process probably died, exiting')
+                break
+            logging.debug(f'Received {line!r}')
+            self._callback_queue.put_nowait(line.decode('UTF-8').strip())
+        # although redundant with the atexit handler, this will prevent
+        # excessive use of disk space in cases where the hotkey process is [re]started many times
+        try_remove(f.name)
 
 
 class Hotkey:
     def __init__(
         self, keyname: str, callback: Callable[[], Any], *, ex_handler: Optional[Callable[[str, Exception], Any]] = None
     ):
         self._keyname: str = keyname
```

### Comparing `ahk-1.7.1/ahk/_sync/engine.py` & `ahk-1.7.2/ahk/_sync/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,34 +29,37 @@
 from .._utils import MsgBoxButtons
 from .._utils import MsgBoxDefaultButton
 from .._utils import MsgBoxIcon
 from .._utils import MsgBoxModality
 from .._utils import MsgBoxOtherOptions
 from .._utils import type_escape
 from ..directives import Directive
-
-if sys.version_info < (3, 10):
-    from typing_extensions import TypeAlias
-else:
-    from typing import TypeAlias
-
-from ..extensions import (
-    Extension,
-    _ExtensionMethodRegistry,
-    _extension_registry,
-    _resolve_extensions,
-)
+from ..extensions import _extension_registry
+from ..extensions import _ExtensionMethodRegistry
+from ..extensions import _resolve_extensions
+from ..extensions import Extension
 from ..keys import Key
 from .transport import DaemonProcessTransport
 from .transport import FutureResult
 from .transport import Transport
 from .window import Control
 from .window import Window
+from ahk._types import _BUTTONS
+from ahk._types import Coordinates
+from ahk._types import CoordModeRelativeTo
+from ahk._types import CoordModeTargets
+from ahk._types import MouseButton
+from ahk._types import Position
+from ahk._types import SendMode
+from ahk._types import TitleMatchMode
 
-from ahk._types import Position, CoordModeTargets, CoordModeRelativeTo, TitleMatchMode, _BUTTONS, MouseButton, SendMode, Coordinates
+if sys.version_info < (3, 10):
+    from typing_extensions import TypeAlias
+else:
+    from typing import TypeAlias
 
 sleep = time.sleep
 
 SyncFilterFunc: TypeAlias = Callable[[Window], bool]
 
 SyncPropertyReturnTupleIntInt: TypeAlias = Coordinates
 
@@ -75,15 +78,15 @@
     if isinstance(button, str):
         button = button.lower()
 
     if button in _BUTTONS:
         resolved_button = _BUTTONS[button]
     elif isinstance(button, int) and button > 3:
         #  for addtional mouse buttons
-        resolved_button = f'X{button-3}'
+        resolved_button = f'X{button - 3}'
     else:
         assert isinstance(button, str)
         resolved_button = button
     return resolved_button
 
 
 T_AHKVersion = TypeVar('T_AHKVersion', bound=Optional[Literal['v1', 'v2']])
@@ -1064,27 +1067,27 @@
             self.send_input(key.UP, blocking=True)
             return None
         else:
             return self.send_input(key.UP, blocking=False)
 
     # fmt: off
     @overload
-    def key_wait(self, key_name: str, *, timeout: Optional[int] = None, logical_state: bool = False, released: bool = False) -> bool: ...
+    def key_wait(self, key_name: str, *, timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False) -> bool: ...
     @overload
-    def key_wait(self, key_name: str, *, blocking: Literal[True], timeout: Optional[int] = None, logical_state: bool = False, released: bool = False) -> bool: ...
+    def key_wait(self, key_name: str, *, blocking: Literal[True], timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False) -> bool: ...
     @overload
-    def key_wait(self, key_name: str, *, blocking: Literal[False], timeout: Optional[int] = None, logical_state: bool = False, released: bool = False) -> FutureResult[bool]: ...
+    def key_wait(self, key_name: str, *, blocking: Literal[False], timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False) -> FutureResult[bool]: ...
     @overload
-    def key_wait(self, key_name: str, *, timeout: Optional[int] = None, logical_state: bool = False, released: bool = False, blocking: bool = True) -> Union[bool, FutureResult[bool]]: ...
+    def key_wait(self, key_name: str, *, timeout: Optional[int | float] = None, logical_state: bool = False, released: bool = False, blocking: bool = True) -> Union[bool, FutureResult[bool]]: ...
     # fmt: on
     def key_wait(
         self,
         key_name: str,
         *,
-        timeout: Optional[int] = None,
+        timeout: Optional[int | float] = None,
         logical_state: bool = False,
         released: bool = False,
         blocking: bool = True,
     ) -> Union[bool, FutureResult[bool]]:
         """
         Analog for `KeyWait <https://www.autohotkey.com/docs/commands/KeyWait.htm>`_
         """
```

### Comparing `ahk-1.7.1/ahk/_sync/transport.py` & `ahk-1.7.2/ahk/_sync/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ahk._hotkey import Hotkey
 from ahk._hotkey import Hotstring
 from ahk._hotkey import ThreadedHotkeyTransport
 from ahk._types import Coordinates
 from ahk._types import FunctionName
 from ahk._types import Position
 from ahk._utils import _version_detection_script
+from ahk._utils import try_remove
 from ahk.directives import Directive
 from ahk.exceptions import AHKProtocolError
 from ahk.extensions import _resolve_includes
 from ahk.extensions import Extension
 from ahk.message import _message_registry
 from ahk.message import RequestMessage
 from ahk.message import ResponseMessage
@@ -628,23 +629,23 @@
                 script_text = self._render_script()
                 with tempfile.NamedTemporaryFile(
                     mode='w', prefix='python-ahk-', suffix='.ahk', delete=False
                 ) as tempscriptfile:
                     tempscriptfile.write(script_text)  # XXX: can we make this async?
                 self._temp_script = tempscriptfile.name
                 daemon_script = self._temp_script
-                atexit.register(os.remove, tempscriptfile.name)
+                atexit.register(try_remove, tempscriptfile.name)
             else:
                 daemon_script = self._temp_script
         else:
             script_text = self._render_script(template=template, **template_kwargs)
             with tempfile.NamedTemporaryFile(mode='w', prefix='python-ahk-', suffix='.ahk', delete=False) as tempscript:
                 tempscript.write(script_text)
             daemon_script = tempscript.name
-            atexit.register(os.remove, tempscript.name)
+            atexit.register(try_remove, tempscript.name)
         runargs = [self._executable_path, '/CP65001', '/ErrorStdOut', daemon_script]
         proc = SyncAHKProcess(runargs=runargs)
         proc.start()
         return proc
 
     def _send_nonblocking(
         self, request: RequestMessage, engine: Optional[AHK[Any]] = None
```

### Comparing `ahk-1.7.1/ahk/_sync/window.py` & `ahk-1.7.2/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/_types.py` & `ahk-1.7.2/ahk/_types.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/_utils.py` & `ahk-1.7.2/ahk/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+import logging
 import os
 import re
 import subprocess
 import warnings
 from shutil import which
 from typing import Literal
 from typing import Optional
@@ -166,7 +167,14 @@
     major_version = match.group(1)
     if major_version == '1':
         return 'v1'
     elif major_version == '2':
         return 'v2'
     else:
         raise ValueError(f'Unexpected version {version!r}')
+
+
+def try_remove(name: str) -> None:
+    try:
+        os.remove(name)
+    except Exception as e:
+        logging.debug(f'Ignoring removal exception {e}')
```

### Comparing `ahk-1.7.1/ahk/directives.py` & `ahk-1.7.2/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/extensions.py` & `ahk-1.7.2/ahk/extensions.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/keys.py` & `ahk-1.7.2/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/message.py` & `ahk-1.7.2/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/templates/daemon-v2.ahk` & `ahk-1.7.2/ahk/templates/daemon-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/templates/daemon.ahk` & `ahk-1.7.2/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/templates/hotkeys-v2.ahk` & `ahk-1.7.2/ahk/templates/hotkeys-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk/templates/hotkeys.ahk` & `ahk-1.7.2/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/ahk.egg-info/PKG-INFO` & `ahk-1.7.2/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.7.1
+Version: 1.7.2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.7.1/ahk.egg-info/SOURCES.txt` & `ahk-1.7.2/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/buildunasync.py` & `ahk-1.7.2/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/docs/README.md` & `ahk-1.7.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.7.1/setup.cfg` & `ahk-1.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.7.1
+version = 1.7.2
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 project_urls =
```

