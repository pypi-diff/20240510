# Comparing `tmp/aiostream-0.5.2.tar.gz` & `tmp/aiostream-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiostream-0.5.2.tar", last modified: Tue Oct 24 10:11:23 2023, max compression
+gzip compressed data, was "aiostream-0.6.0rc1.tar", last modified: Fri May 10 10:30:26 2024, max compression
```

## Comparing `aiostream-0.5.2.tar` & `aiostream-0.6.0rc1.tar`

### file list

```diff
@@ -1,30 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-10-24 10:11:20.000000 aiostream-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-10-24 10:11:23.284700 aiostream-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2023-10-24 10:11:20.000000 aiostream-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/aiostream/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/aiter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/aiostream/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8969 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/aiostream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-10-24 10:11:23.000000 aiostream-0.5.2/aiostream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-24 10:11:23.284700 aiostream-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-24 10:11:20.000000 aiostream-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.068953 aiostream-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50736 2024-05-10 10:30:26.068953 aiostream-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.060953 aiostream-0.6.0rc1/aiostream/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/aiter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24871 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.064953 aiostream-0.6.0rc1/aiostream/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/stream/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/aiostream/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.064953 aiostream-0.6.0rc1/aiostream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50736 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 10:30:26.000000 aiostream-0.6.0rc1/aiostream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:30:26.068953 aiostream-0.6.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:30:26.064953 aiostream-0.6.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_aiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_task_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-10 10:30:21.000000 aiostream-0.6.0rc1/tests/test_transform.py
```

### Comparing `aiostream-0.5.2/LICENSE` & `aiostream-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.2/README.rst` & `aiostream-0.6.0rc1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,12 @@
 aiostream
 =========
 
 
-.. image:: https://readthedocs.org/projects/aiostream/badge/?version=latest
-   :target: http://aiostream.readthedocs.io/en/latest/?badge=latest
-   :alt:
-
-.. image:: https://codecov.io/gh/vxgmichel/aiostream/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/vxgmichel/aiostream
-   :alt:
-
-.. image:: https://travis-ci.org/vxgmichel/aiostream.svg?branch=master
-   :target: https://travis-ci.org/vxgmichel/aiostream
-   :alt:
-
-.. image:: https://img.shields.io/pypi/v/aiostream.svg
-   :target: https://pypi.python.org/pypi/aiostream
-   :alt:
-
-.. image:: https://img.shields.io/pypi/pyversions/aiostream.svg
-   :target: https://pypi.python.org/pypi/aiostream/
-   :alt:
+|docs-badge| |cov-badge| |ci-badge| |version-badge| |pyversion-badge|
 
 Generator-based operators for asynchronous iteration
 
 
 Synopsis
 --------
 
@@ -39,22 +21,14 @@
 - **Repeatability** - every iteration creates a different iterator
 - **Safe iteration context** - using ``async with`` and the ``stream`` method
 - **Simplified execution** - get the last element from a stream using ``await``
 - **Slicing and indexing** - using square brackets ``[]``
 - **Concatenation** - using addition symbol ``+``
 
 
-Requirements
-------------
-
-The stream operators rely heavily on asynchronous generators (`PEP 525`_):
-
-- python >= 3.6
-
-
 Stream operators
 ----------------
 
 The `stream operators`_ are separated in 7 categories:
 
 +--------------------+---------------------------------------------------------------------------------------+
 | **creation**       | iterate_, preserve_, just_, call_, empty_, throw_, never_, repeat_, count_, range_    |
@@ -76,15 +50,15 @@
 
 
 Demonstration
 -------------
 
 The following example demonstrates most of the streams capabilities:
 
-.. sourcecode:: python
+.. code:: python
 
     import asyncio
     from aiostream import stream, pipe
 
 
     async def main():
 
@@ -187,7 +161,23 @@
 
 .. _spaceout: http://aiostream.readthedocs.io/en/latest/operators.html#aiostream.stream.spaceout
 .. _delay: http://aiostream.readthedocs.io/en/latest/operators.html#aiostream.stream.delay
 .. _timeout: http://aiostream.readthedocs.io/en/latest/operators.html#aiostream.stream.timeout
 
 .. _action: http://aiostream.readthedocs.io/en/latest/operators.html#aiostream.stream.action
 .. _print: http://aiostream.readthedocs.io/en/latest/operators.html#aiostream.stream.print
+
+.. |docs-badge| image:: https://readthedocs.org/projects/aiostream/badge/?version=latest
+   :target: http://aiostream.readthedocs.io/en/latest/?badge=latest
+   :alt:
+..  |cov-badge| image:: https://codecov.io/gh/vxgmichel/aiostream/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/vxgmichel/aiostream
+   :alt:
+.. |ci-badge| image:: https://github.com/vxgmichel/aiostream/workflows/CI/badge.svg
+   :target: https://github.com/vxgmichel/aiostream/actions/workflows/ci.yml?query=branch%3Amain
+   :alt:
+.. |version-badge| image:: https://img.shields.io/pypi/v/aiostream.svg
+   :target: https://pypi.python.org/pypi/aiostream
+   :alt:
+.. |pyversion-badge| image:: https://img.shields.io/pypi/pyversions/aiostream.svg
+   :target: https://pypi.python.org/pypi/aiostream/
+   :alt:
```

### Comparing `aiostream-0.5.2/aiostream/__init__.py` & `aiostream-0.6.0rc1/aiostream/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 - test_utils: utilities for testing stream operators (require pytest)
 """
 
 from . import stream, pipe
 from .aiter_utils import async_, await_
 from .core import StreamEmpty, operator, pipable_operator, streamcontext
 
+__version__ = "0.6.0rc1"
+
 __all__ = [
     "stream",
     "pipe",
     "async_",
     "await_",
     "operator",
     "pipable_operator",
     "streamcontext",
     "StreamEmpty",
+    "__version__",
 ]
```

### Comparing `aiostream-0.5.2/aiostream/aiter_utils.py` & `aiostream-0.6.0rc1/aiostream/aiter_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Utilities for asynchronous iteration."""
+
 from __future__ import annotations
+
+import sys
 from types import TracebackType
 
 import warnings
 import functools
 from typing import (
     TYPE_CHECKING,
     AsyncContextManager,
@@ -11,14 +14,15 @@
     AsyncIterable,
     Awaitable,
     Callable,
     Type,
     TypeVar,
     AsyncIterator,
     Any,
+    cast,
 )
 
 if TYPE_CHECKING:
     from typing_extensions import ParamSpec
 
     P = ParamSpec("P")
 
@@ -99,19 +103,21 @@
     """
     if not is_async_iterator(obj):
         raise TypeError(f"{type(obj).__name__!r} object is not an async iterator")
 
 
 # Async iterator context
 
-T = TypeVar("T")
+T = TypeVar("T", covariant=True)
 Self = TypeVar("Self", bound="AsyncIteratorContext[Any]")
 
 
-class AsyncIteratorContext(AsyncIterator[T], AsyncContextManager[Any]):
+class AsyncIteratorContext(
+    AsyncIterator[T], AsyncContextManager["AsyncIteratorContext[T]"]
+):
     """Asynchronous iterator with context management.
 
     The context management makes sure the aclose asynchronous method
     of the corresponding iterator has run before it exits. It also issues
     warnings and RuntimeError if it is used incorrectly.
 
     Correct usage::
@@ -179,27 +185,32 @@
                 # Prevent GeneratorExit from being silenced
                 if typ is GeneratorExit:
                     return False
 
                 # No method to throw
                 if not hasattr(self._aiterator, "athrow"):
                     return False
+                self._aiterator = cast(AsyncGenerator[T, None], self._aiterator)
 
                 # No frame to throw
                 if not getattr(self._aiterator, "ag_frame", True):
                     return False
 
                 # Cannot throw at the moment
                 if getattr(self._aiterator, "ag_running", False):
                     return False
 
                 # Throw
                 try:
                     assert isinstance(self._aiterator, AsyncGenerator)
-                    await self._aiterator.athrow(typ, value, traceback)
+                    if sys.version_info >= (3, 12):
+                        assert value is not None
+                        await self._aiterator.athrow(value)
+                    else:
+                        await self._aiterator.athrow(typ, value, traceback)
                     raise RuntimeError("Async iterator didn't stop after athrow()")
 
                 # Exception has been (most probably) silenced
                 except StopAsyncIteration as exc:
                     return exc is not value
 
                 # A (possibly new) exception has been raised
@@ -229,14 +240,15 @@
     async def aclose(self) -> None:
         await self.__aexit__(None, None, None)
 
     async def athrow(self, exc: Exception) -> T:
         if self._state == self._FINISHED:
             raise RuntimeError(f"{type(self).__name__} is closed and cannot be used")
         assert isinstance(self._aiterator, AsyncGenerator)
+        self._aiterator = cast(AsyncGenerator[T, None], self._aiterator)
         item: T = await self._aiterator.athrow(exc)
         return item
 
 
 def aitercontext(
     aiterable: AsyncIterable[T],
 ) -> AsyncIteratorContext[T]:
```

### Comparing `aiostream-0.5.2/aiostream/manager.py` & `aiostream-0.6.0rc1/aiostream/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Provide a context to easily manage several streamers running
 concurrently.
 """
+
 from __future__ import annotations
 
 import asyncio
 from .aiter_utils import AsyncExitStack
 
 from .aiter_utils import anext
 from .core import streamcontext
```

### Comparing `aiostream-0.5.2/aiostream/pipe.py` & `aiostream-0.6.0rc1/aiostream/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Gather the pipe operators."""
+
 from __future__ import annotations
 
 from . import stream
 
 accumulate = stream.accumulate.pipe
 action = stream.action.pipe
 amap = stream.amap.pipe
```

### Comparing `aiostream-0.5.2/aiostream/stream/advanced.py` & `aiostream-0.6.0rc1/aiostream/stream/advanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Advanced operators (to deal with streams of higher order) ."""
+
 from __future__ import annotations
 
 from typing import AsyncIterator, AsyncIterable, TypeVar, Union, cast
 from typing_extensions import ParamSpec
 
 from . import combine
 
@@ -42,17 +43,17 @@
 
     # Task limit
     if task_limit is not None and not task_limit > 0:
         raise ValueError("The task limit must be None or greater than 0")
 
     # Safe context
     async with StreamerManager[Union[AsyncIterable[T], T]]() as manager:
-        main_streamer: Streamer[
-            AsyncIterable[T] | T
-        ] | None = await manager.enter_and_create_task(source)
+        main_streamer: Streamer[AsyncIterable[T] | T] | None = (
+            await manager.enter_and_create_task(source)
+        )
 
         # Loop over events
         while manager.tasks:
             # Extract streamer groups
             substreamers = manager.streamers[1:]
             mainstreamers = [main_streamer] if main_streamer in manager.tasks else []
 
@@ -92,14 +93,15 @@
                 # Switch mecanism
                 if switch and streamer is main_streamer:
                     await manager.clean_streamers(substreamers)
 
                 # Setup a new source
                 if streamer is main_streamer:
                     assert isinstance(result, AsyncIterable)
+                    result = cast(AsyncIterable[T], result)
                     await manager.enter_and_create_task(result)
 
                     # Re-schedule the main streamer if task limit allows it
                     if task_limit is None or task_limit > len(manager.tasks):
                         manager.create_task(streamer)
 
                 # Yield the result
```

### Comparing `aiostream-0.5.2/aiostream/stream/aggregate.py` & `aiostream-0.6.0rc1/aiostream/stream/aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Aggregation operators."""
+
 from __future__ import annotations
 
 import asyncio
 import builtins
 import operator as op
 from typing import AsyncIterator, Awaitable, Callable, TypeVar, AsyncIterable, cast
```

### Comparing `aiostream-0.5.2/aiostream/stream/combine.py` & `aiostream-0.6.0rc1/aiostream/stream/combine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Combination operators."""
+
 from __future__ import annotations
 
 import asyncio
 import builtins
 
 from typing import (
     Awaitable,
@@ -12,60 +13,57 @@
     AsyncIterator,
     Callable,
     cast,
 )
 from typing_extensions import ParamSpec
 
 from ..aiter_utils import AsyncExitStack, anext
-from ..core import streamcontext, pipable_operator
+from ..core import sources_operator, streamcontext, pipable_operator
 
 from . import create
 from . import select
 from . import advanced
 from . import aggregate
 
 __all__ = ["chain", "zip", "map", "merge", "ziplatest", "amap", "smap"]
 
 T = TypeVar("T")
 U = TypeVar("U")
 K = TypeVar("K")
 P = ParamSpec("P")
 
 
-@pipable_operator
-async def chain(
-    source: AsyncIterable[T], *more_sources: AsyncIterable[T]
-) -> AsyncIterator[T]:
+@sources_operator
+async def chain(*sources: AsyncIterable[T]) -> AsyncIterator[T]:
     """Chain asynchronous sequences together, in the order they are given.
 
     Note: the sequences are not iterated until it is required,
     so if the operation is interrupted, the remaining sequences
     will be left untouched.
     """
-    sources = source, *more_sources
     for source in sources:
         async with streamcontext(source) as streamer:
             async for item in streamer:
                 yield item
 
 
-@pipable_operator
-async def zip(
-    source: AsyncIterable[T], *more_sources: AsyncIterable[T]
-) -> AsyncIterator[tuple[T, ...]]:
+@sources_operator
+async def zip(*sources: AsyncIterable[T]) -> AsyncIterator[tuple[T, ...]]:
     """Combine and forward the elements of several asynchronous sequences.
 
     Each generated value is a tuple of elements, using the same order as
     their respective sources. The generation continues until the shortest
     sequence is exhausted.
 
     Note: the different sequences are awaited in parrallel, so that their
     waiting times don't add up.
     """
-    sources = source, *more_sources
+    # No sources
+    if not sources:
+        return
 
     # One sources
     if len(sources) == 1:
         (source,) = sources
         async with streamcontext(source) as streamer:
             async for item in streamer:
                 yield (item,)
@@ -89,26 +87,23 @@
 
 
 X = TypeVar("X", contravariant=True)
 Y = TypeVar("Y", covariant=True)
 
 
 class SmapCallable(Protocol[X, Y]):
-    def __call__(self, arg: X, /, *args: X) -> Y:
-        ...
+    def __call__(self, arg: X, /, *args: X) -> Y: ...
 
 
 class AmapCallable(Protocol[X, Y]):
-    async def __call__(self, arg: X, /, *args: X) -> Y:
-        ...
+    async def __call__(self, arg: X, /, *args: X) -> Y: ...
 
 
 class MapCallable(Protocol[X, Y]):
-    def __call__(self, arg: X, /, *args: X) -> Awaitable[Y] | Y:
-        ...
+    def __call__(self, arg: X, /, *args: X) -> Awaitable[Y] | Y: ...
 
 
 @pipable_operator
 async def smap(
     source: AsyncIterable[T],
     func: SmapCallable[T, U],
     *more_sources: AsyncIterable[T],
@@ -207,33 +202,31 @@
         return amap.raw(
             source, func, *more_sources, ordered=ordered, task_limit=task_limit
         )
     sync_func = cast("SmapCallable[T, U]", func)
     return smap.raw(source, sync_func, *more_sources)
 
 
-@pipable_operator
+@sources_operator
 def merge(
-    source: AsyncIterable[T], *more_sources: AsyncIterable[T]
+    *sources: AsyncIterable[T],
 ) -> AsyncIterator[T]:
     """Merge several asynchronous sequences together.
 
     All the sequences are iterated simultaneously and their elements
     are forwarded as soon as they're available. The generation continues
     until all the sequences are exhausted.
     """
-    sources = [source, *more_sources]
     source_stream: AsyncIterable[AsyncIterable[T]] = create.iterate.raw(sources)
     return advanced.flatten.raw(source_stream)
 
 
-@pipable_operator
+@sources_operator
 def ziplatest(
-    source: AsyncIterable[T],
-    *more_sources: AsyncIterable[T],
+    *sources: AsyncIterable[T],
     partial: bool = True,
     default: T | None = None,
 ) -> AsyncIterator[tuple[T | None, ...]]:
     """Combine several asynchronous sequences together, producing a tuple with
     the lastest element of each sequence whenever a new element is received.
 
     The value to use when a sequence has not procuded any element yet is given
@@ -242,15 +235,14 @@
     The producing of partial results can be disabled by setting the optional
     argument ``partial`` to ``False``.
 
     All the sequences are iterated simultaneously and their elements
     are forwarded as soon as they're available. The generation continues
     until all the sequences are exhausted.
     """
-    sources = source, *more_sources
     n = len(sources)
 
     # Custom getter
     def getter(dct: dict[int, T]) -> Callable[[int], T | None]:
         return lambda key: dct.get(key, default)
 
     # Add source index to the items
```

### Comparing `aiostream-0.5.2/aiostream/stream/create.py` & `aiostream-0.6.0rc1/aiostream/stream/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Non-pipable creation operators."""
+
 from __future__ import annotations
 
 import sys
 import asyncio
 import inspect
 import builtins
 import itertools
@@ -11,16 +12,17 @@
     AsyncIterable,
     Awaitable,
     Iterable,
     Protocol,
     TypeVar,
     AsyncIterator,
     cast,
+    Type,
 )
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, Never
 
 from ..stream import time
 from ..core import operator, streamcontext
 
 __all__ = [
     "iterate",
     "preserve",
@@ -91,21 +93,19 @@
         yield value
 
 
 Y = TypeVar("Y", covariant=True)
 
 
 class SyncCallable(Protocol[P, Y]):
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> Y:
-        ...
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> Y: ...
 
 
 class AsyncCallable(Protocol[P, Y]):
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> Awaitable[Y]:
-        ...
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> Awaitable[Y]: ...
 
 
 @operator
 async def call(
     func: SyncCallable[P, T] | AsyncCallable[P, T], *args: P.args, **kwargs: P.kwargs
 ) -> AsyncIterator[T]:
     """Call the given function and generate a single value.
@@ -117,30 +117,30 @@
         yield await async_func(*args, **kwargs)
     else:
         sync_func = cast("SyncCallable[P, T]", func)
         yield sync_func(*args, **kwargs)
 
 
 @operator
-async def throw(exc: Exception) -> AsyncIterator[None]:
+async def throw(exc: Exception | Type[Exception]) -> AsyncIterator[Never]:
     """Throw an exception without generating any value."""
     if False:
         yield
     raise exc
 
 
 @operator
-async def empty() -> AsyncIterator[None]:
+async def empty() -> AsyncIterator[Never]:
     """Terminate without generating any value."""
     if False:
         yield
 
 
 @operator
-async def never() -> AsyncIterator[None]:
+async def never() -> AsyncIterator[Never]:
     """Hang forever without generating any value."""
     if False:
         yield
     future: asyncio.Future[None] = asyncio.Future()
     try:
         await future
     finally:
```

### Comparing `aiostream-0.5.2/aiostream/stream/misc.py` & `aiostream-0.6.0rc1/aiostream/stream/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Extra operators."""
+
 from __future__ import annotations
 
 import asyncio
 import builtins
 
 from typing import TypeVar, Awaitable, Callable, AsyncIterable, AsyncIterator, Any
```

### Comparing `aiostream-0.5.2/aiostream/stream/select.py` & `aiostream-0.6.0rc1/aiostream/stream/select.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Selection operators."""
+
 from __future__ import annotations
 
 import asyncio
 import builtins
 import collections
 
 from typing import Awaitable, Callable, TypeVar, AsyncIterable, AsyncIterator
@@ -106,15 +107,15 @@
     async with streamcontext(enumerated) as streamer:
         async for i, item in streamer:
             if func(i):
                 yield item
 
 
 @pipable_operator
-def slice(source: AsyncIterable[T], *args: int) -> AsyncIterator[T]:
+def slice(source: AsyncIterable[T], *args: int | None) -> AsyncIterator[T]:
     """Slice an asynchronous sequence.
 
     The arguments are the same as the builtin type slice.
 
     There are two limitations compare to regular slices:
     - Positive stop index with negative start index is not supported
     - Negative step is not supported
```

### Comparing `aiostream-0.5.2/aiostream/stream/time.py` & `aiostream-0.6.0rc1/aiostream/stream/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Time-specific operators."""
+
 from __future__ import annotations
 import asyncio
 
 from ..aiter_utils import anext
 from ..core import streamcontext, pipable_operator
 
 from typing import TypeVar, AsyncIterable, AsyncIterator
```

### Comparing `aiostream-0.5.2/aiostream/stream/transform.py` & `aiostream-0.6.0rc1/aiostream/stream/transform.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 from . import select
 from . import create
 from . import aggregate
 from .combine import map, amap, smap
 
 __all__ = ["map", "enumerate", "starmap", "cycle", "chunks"]
 
-# map, amap and smap are also transform operators
-map, amap, smap
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 @pipable_operator
 async def enumerate(
@@ -45,21 +43,19 @@
 
 
 X = TypeVar("X", contravariant=True)
 Y = TypeVar("Y", covariant=True)
 
 
 class AsyncStarmapCallable(Protocol[X, Y]):
-    def __call__(self, arg: X, /, *args: X) -> Awaitable[Y]:
-        ...
+    def __call__(self, arg: X, /, *args: X) -> Awaitable[Y]: ...
 
 
 class SyncStarmapCallable(Protocol[X, Y]):
-    def __call__(self, arg: X, /, *args: X) -> Y:
-        ...
+    def __call__(self, arg: X, /, *args: X) -> Y: ...
 
 
 @pipable_operator
 def starmap(
     source: AsyncIterable[tuple[T, ...]],
     func: SyncStarmapCallable[T, U] | AsyncStarmapCallable[T, U],
     ordered: bool = True,
```

### Comparing `aiostream-0.5.2/aiostream/test_utils.py` & `aiostream-0.6.0rc1/aiostream/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,52 @@
 """Utilities for testing stream operators."""
+
 from __future__ import annotations
 
 import asyncio
-from unittest.mock import Mock
+from collections import deque
 from contextlib import contextmanager
+from unittest.mock import Mock
+from typing import (
+    TYPE_CHECKING,
+    Awaitable,
+    Callable,
+    List,
+    Protocol,
+    TypeVar,
+    AsyncIterable,
+    AsyncIterator,
+    ContextManager,
+    Iterator,
+    cast,
+    Any,
+)
 
 import pytest
 
 from .core import StreamEmpty, streamcontext, pipable_operator
-from typing import TYPE_CHECKING, Any, Callable, List
 
 if TYPE_CHECKING:
     from _pytest.fixtures import SubRequest
     from aiostream.core import Stream
 
-__all__ = ["add_resource", "assert_run", "event_loop"]
+__all__ = ["add_resource", "assert_run", "event_loop_policy", "assert_cleanup"]
+
+
+T = TypeVar("T")
 
 
 @pipable_operator
-async def add_resource(source, cleanup_time):
+async def add_resource(
+    source: AsyncIterable[T], cleanup_time: float
+) -> AsyncIterator[T]:
     """Simulate an open resource in a stream operator."""
+    loop = asyncio.get_running_loop()
+    assert isinstance(loop, TimeTrackingTestLoop)
     try:
-        loop = asyncio.get_event_loop()
         loop.open_resources += 1
         loop.resources += 1
         async with streamcontext(source) as streamer:
             async for item in streamer:
                 yield item
     finally:
         try:
@@ -39,36 +60,36 @@
     exc2: Exception,
 ) -> bool:
     """Compare two exceptions together."""
     return exc1 == exc2 or exc1.__class__ == exc2.__class__ and exc1.args == exc2.args
 
 
 async def assert_aiter(
-    source: Stream,
-    values: List[Any],
+    source: Stream[object],
+    values: List[object],
     exception: Exception | None = None,
 ) -> None:
     """Check the results of a stream using a streamcontext."""
-    results = []
+    results: list[object] = []
     exception_type = (type(exception),) if exception else ()
     try:
         async with streamcontext(source) as streamer:
             async for item in streamer:
                 results.append(item)
     except exception_type as exc:
         assert exception is not None
         assert compare_exceptions(exc, exception)
     else:
         assert exception is None
     assert results == values
 
 
 async def assert_await(
-    source: Stream,
-    values: List[Any],
+    source: Stream[object],
+    values: List[object],
     exception: Exception | None = None,
 ) -> None:
     """Check the results of a stream using by awaiting it."""
     exception_type = (type(exception),) if exception else ()
     try:
         result = await source
     except StreamEmpty:
@@ -78,96 +99,119 @@
         assert exception is not None
         assert compare_exceptions(exc, exception)
     else:
         assert result == values[-1]
         assert exception is None
 
 
-@pytest.fixture(params=[assert_aiter, assert_await], ids=["aiter", "await"])
-def assert_run(request: SubRequest) -> Callable:
+class AssertRunProtocol(Protocol):
+    def __call__(
+        self, source: Stream[object], values: List[object], exception: Exception | None
+    ) -> Awaitable[None]: ...
+
+
+@pytest.fixture(params=[assert_aiter, assert_await], ids=["aiter", "await"])  # type: ignore[misc]
+def assert_run(request: SubRequest) -> AssertRunProtocol:
     """Parametrized fixture returning a stream runner."""
-    return request.param
+    return cast(AssertRunProtocol, request.param)
 
 
-@pytest.fixture
-def event_loop():
+@pytest.fixture  # type: ignore[misc]
+def event_loop_policy() -> TimeTrackingTestLoopPolicy:
     """Fixture providing a test event loop.
 
     The event loop simulate and records the sleep operation,
     available as event_loop.steps
 
     It also tracks simulated resources and make sure they are
     all released before the loop is closed.
     """
+    return TimeTrackingTestLoopPolicy()
 
-    class TimeTrackingTestLoop(asyncio.BaseEventLoop):
-        stuck_threshold = 100
 
-        def __init__(self):
-            super().__init__()
-            self._time = 0
-            self._timers = []
-            self._selector = Mock()
-            self.clear()
-
-        # Loop internals
-
-        def _run_once(self):
-            super()._run_once()
-            # Update internals
-            self.busy_count += 1
-            self._timers = sorted(when for when in self._timers if when > loop.time())
-            # Time advance
-            if self.time_to_go:
-                when = self._timers.pop(0)
-                step = when - loop.time()
-                self.steps.append(step)
-                self.advance_time(step)
-                self.busy_count = 0
-
-        def _process_events(self, event_list):
-            return
-
-        def _write_to_self(self):
-            return
-
-        # Time management
-
-        def time(self):
-            return self._time
-
-        def advance_time(self, advance):
-            if advance:
-                self._time += advance
-
-        def call_at(self, when, callback, *args, **kwargs):
-            self._timers.append(when)
-            return super().call_at(when, callback, *args, **kwargs)
-
-        @property
-        def stuck(self):
-            return self.busy_count > self.stuck_threshold
-
-        @property
-        def time_to_go(self):
-            return self._timers and (self.stuck or not self._ready)
-
-        # Resource management
-
-        def clear(self):
-            self.steps = []
-            self.open_resources = 0
-            self.resources = 0
+@pytest.fixture  # type: ignore[misc]
+def assert_cleanup(
+    event_loop: TimeTrackingTestLoop,
+) -> Callable[[], ContextManager[TimeTrackingTestLoop]]:
+    """Fixture to assert cleanup of resources."""
+    return event_loop.assert_cleanup
+
+
+class BaseEventLoopWithInternals(asyncio.BaseEventLoop):
+    _ready: deque[asyncio.Handle]
+    _run_once: Callable[[], None]
+
+
+class TimeTrackingTestLoop(BaseEventLoopWithInternals):
+    stuck_threshold: int = 100
+
+    def __init__(self) -> None:
+        super().__init__()
+        self._time: float = 0.0
+        self._timers: list[float] = []
+        self._selector = Mock()
+
+        self.steps: list[float] = []
+        self.open_resources: int = 0
+        self.resources: int = 0
+        self.busy_count: int = 0
+
+    # Loop internals
+
+    def _run_once(self) -> None:  # type: ignore
+        super()._run_once()
+        # Update internals
+        self.busy_count += 1
+        self._timers = sorted(when for when in self._timers if when > self.time())
+        # Time advance
+        if self.time_to_go:
+            when = self._timers.pop(0)
+            step = when - self.time()
+            self.steps.append(step)
+            self.advance_time(step)
             self.busy_count = 0
 
-        @contextmanager
-        def assert_cleanup(self):
-            self.clear()
-            yield self
-            assert self.open_resources == 0
-            self.clear()
-
-    loop = TimeTrackingTestLoop()
-    asyncio.set_event_loop(loop)
-    with loop.assert_cleanup():
-        yield loop
-    loop.close()
+    def _process_events(self, event_list: object) -> None:
+        return
+
+    def _write_to_self(self) -> None:
+        return
+
+    # Time management
+
+    def time(self) -> float:
+        return self._time
+
+    def advance_time(self, advance: float) -> None:
+        if advance:
+            self._time += advance
+
+    def call_at(self, when: float, callback: Callable[..., None], *args: Any, **kwargs: Any) -> asyncio.TimerHandle:  # type: ignore
+        self._timers.append(when)
+        return super().call_at(when, callback, *args, **kwargs)
+
+    @property
+    def stuck(self) -> bool:
+        return self.busy_count > self.stuck_threshold
+
+    @property
+    def time_to_go(self) -> bool:
+        return bool(self._timers) and (self.stuck or not self._ready)
+
+    # Resource management
+
+    def clear(self) -> None:
+        self.steps = []
+        self.open_resources = 0
+        self.resources = 0
+        self.busy_count = 0
+
+    @contextmanager
+    def assert_cleanup(self) -> Iterator[TimeTrackingTestLoop]:
+        self.clear()
+        yield self
+        assert self.open_resources == 0
+        self.clear()
+
+
+class TimeTrackingTestLoopPolicy(asyncio.DefaultEventLoopPolicy):
+    _loop_factory = TimeTrackingTestLoop
```

