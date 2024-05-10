# Comparing `tmp/psycopg-pool-3.2.0.tar.gz` & `tmp/psycopg-pool-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg-pool-3.2.0.tar", last modified: Sat Nov 11 15:14:36 2023, max compression
+gzip compressed data, was "psycopg-pool-3.2.1.tar", last modified: Sun Jan  7 12:24:41 2024, max compression
```

## Comparing `psycopg-pool-3.2.0.tar` & `psycopg-pool-3.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 15:14:36.800819 psycopg-pool-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2023-11-11 15:14:36.800819 psycopg-pool-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 15:14:36.800819 psycopg-pool-3.2.0/psycopg_pool/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/_acompat.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/base_null_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/null_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/null_pool_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    35812 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    38392 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/pool_async.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/sched.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/sched_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/psycopg_pool/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 15:14:36.800819 psycopg-pool-3.2.0/psycopg_pool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2023-11-11 15:14:36.000000 psycopg-pool-3.2.0/psycopg_pool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-11-11 15:14:36.000000 psycopg-pool-3.2.0/psycopg_pool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-11 15:14:36.000000 psycopg-pool-3.2.0/psycopg_pool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-11 15:14:36.000000 psycopg-pool-3.2.0/psycopg_pool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-11 15:14:36.000000 psycopg-pool-3.2.0/psycopg_pool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-11 15:14:36.000000 psycopg-pool-3.2.0/psycopg_pool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-11 15:14:36.804819 psycopg-pool-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-11 15:14:26.000000 psycopg-pool-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 12:24:41.375857 psycopg-pool-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-01-07 12:24:41.375857 psycopg-pool-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 12:24:41.375857 psycopg-pool-3.2.1/psycopg_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/_acompat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/base_null_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/null_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/null_pool_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34852 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37352 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/pool_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/sched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/sched_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/psycopg_pool/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 12:24:41.375857 psycopg-pool-3.2.1/psycopg_pool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-01-07 12:24:41.000000 psycopg-pool-3.2.1/psycopg_pool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-07 12:24:41.000000 psycopg-pool-3.2.1/psycopg_pool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 12:24:41.000000 psycopg-pool-3.2.1/psycopg_pool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 12:24:41.000000 psycopg-pool-3.2.1/psycopg_pool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-07 12:24:41.000000 psycopg-pool-3.2.1/psycopg_pool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-07 12:24:41.000000 psycopg-pool-3.2.1/psycopg_pool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-01-07 12:24:41.375857 psycopg-pool-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-07 12:24:30.000000 psycopg-pool-3.2.1/setup.py
```

### Comparing `psycopg-pool-3.2.0/LICENSE.txt` & `psycopg-pool-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/PKG-INFO` & `psycopg-pool-3.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg-pool
-Version: 3.2.0
+Version: 3.2.1
 Summary: Connection Pool for Psycopg
 Home-page: https://psycopg.org/psycopg3/
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://psycopg.org/
 Project-URL: Documentation, https://www.psycopg.org/psycopg3/docs/advanced/pool.html
@@ -20,22 +20,24 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: typing-extensions>=3.10
+Requires-Dist: typing-extensions>=4.4
 
 Psycopg 3: PostgreSQL database adapter for Python - Connection Pool
 ===================================================================
 
 This distribution package is an optional component of `Psycopg 3`__: it
 contains the optional connection pool package `psycopg_pool`__.
```

### Comparing `psycopg-pool-3.2.0/README.rst` & `psycopg-pool-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/psycopg_pool/__init__.py` & `psycopg-pool-3.2.1/psycopg_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/psycopg_pool/_acompat.py` & `psycopg-pool-3.2.1/psycopg_pool/_acompat.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 when generating the sync version.
 """
 
 # Copyright (C) 2023 The Psycopg Team
 
 from __future__ import annotations
 
+import time
 import queue
 import asyncio
 import logging
 import threading
-from typing import Any, Callable, Coroutine, TypeVar, TYPE_CHECKING
+from typing import Any, Callable, Coroutine, TYPE_CHECKING
 
 from typing_extensions import TypeAlias
 
+from ._compat import TypeVar
+
 logger = logging.getLogger("psycopg.pool")
 T = TypeVar("T")
 
 # Re-exports
 Event = threading.Event
 Condition = threading.Condition
 Lock = threading.RLock
 ALock = asyncio.Lock
+sleep = time.sleep
 
 Worker: TypeAlias = threading.Thread
 AWorker: TypeAlias = "asyncio.Task[None]"
 
 # Hack required on Python 3.8 because subclassing Queue[T] fails at runtime.
 # https://stackoverflow.com/questions/45414066/mypy-how-to-define-a-generic-subclass
 if TYPE_CHECKING:
@@ -156,7 +160,14 @@
     for t in tasks:
         if not t.is_alive():
             continue
         t.join(timeout)
         if not t.is_alive():
             continue
         logger.warning("couldn't stop thread %r within %s seconds", t.name, timeout)
+
+
+def asleep(seconds: float) -> Coroutine[Any, Any, None]:
+    """
+    Equivalent to asyncio.sleep(), converted to time.sleep() by async_to_sync.
+    """
+    return asyncio.sleep(seconds)
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool/abc.py` & `psycopg-pool-3.2.1/psycopg_pool/abc.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 Types used in the psycopg_pool package
 """
 
 # Copyright (C) 2023 The Psycopg Team
 
 from __future__ import annotations
 
-from typing import Any, Awaitable, Callable, TypeVar, Union, TYPE_CHECKING
+from typing import Any, Awaitable, Callable, Union, TYPE_CHECKING
 
 from typing_extensions import TypeAlias
 
+from ._compat import TypeVar
+
 if TYPE_CHECKING:
     from .pool import ConnectionPool
     from .pool_async import AsyncConnectionPool
-    from psycopg import Connection, AsyncConnection
+    from psycopg import Connection, AsyncConnection  # noqa: F401
+    from psycopg.rows import TupleRow  # noqa: F401
 
 # Connection types to make the pool generic
-CT = TypeVar("CT", bound="Connection[Any]")
-ACT = TypeVar("ACT", bound="AsyncConnection[Any]")
+CT = TypeVar("CT", bound="Connection[Any]", default="Connection[TupleRow]")
+ACT = TypeVar("ACT", bound="AsyncConnection[Any]", default="AsyncConnection[TupleRow]")
 
 # Callbacks taking a connection from the pool
 ConnectionCB: TypeAlias = Callable[[CT], None]
 AsyncConnectionCB: TypeAlias = Callable[[ACT], Awaitable[None]]
 
 # Callbacks to pass the pool to on connection failure
 ConnectFailedCB: TypeAlias = Callable[["ConnectionPool[Any]"], None]
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool/base.py` & `psycopg-pool-3.2.1/psycopg_pool/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,35 +196,37 @@
         """Set an expiry date on a connection.
 
         Add some randomness to avoid mass reconnection.
         """
         conn._expire_at = monotonic() + self._jitter(self.max_lifetime, -0.05, 0.0)
 
 
-class ConnectionAttempt:
-    """Keep the state of a connection attempt."""
+class AttemptWithBackoff:
+    """
+    Keep the state of a repeated operation attempt with exponential backoff.
+    """
 
     INITIAL_DELAY = 1.0
     DELAY_JITTER = 0.1
     DELAY_BACKOFF = 2.0
 
-    def __init__(self, *, reconnect_timeout: float):
-        self.reconnect_timeout = reconnect_timeout
+    def __init__(self, *, timeout: float):
+        self.timeout = timeout
         self.delay = 0.0
         self.give_up_at = 0.0
 
     def update_delay(self, now: float) -> None:
         """Calculate how long to wait for a new connection attempt"""
         if self.delay == 0.0:
-            self.give_up_at = now + self.reconnect_timeout
+            self.give_up_at = now + self.timeout
             self.delay = BasePool._jitter(
                 self.INITIAL_DELAY, -self.DELAY_JITTER, self.DELAY_JITTER
             )
         else:
             self.delay *= self.DELAY_BACKOFF
 
         if self.delay + now > self.give_up_at:
             self.delay = max(0.0, self.give_up_at - now)
 
     def time_to_give_up(self, now: float) -> bool:
-        """Return True if we are tired of trying to connect. Meh."""
+        """Return True if we are tired of trying this attempt. Meh."""
         return self.give_up_at > 0.0 and now >= self.give_up_at
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool/base_null_pool.py` & `psycopg-pool-3.2.1/psycopg_pool/base_null_pool.py`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/psycopg_pool/errors.py` & `psycopg-pool-3.2.1/psycopg_pool/errors.py`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/psycopg_pool/null_pool.py` & `psycopg-pool-3.2.1/psycopg_pool/null_pool.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,78 +6,30 @@
 """
 
 # Copyright (C) 2022 The Psycopg Team
 
 from __future__ import annotations
 
 import logging
-from typing import Any, cast, Dict, Optional, overload, Type
+from typing import Any, cast, Dict, Optional, Type
 
 from psycopg import Connection
 from psycopg.pq import TransactionStatus
-from psycopg.rows import TupleRow
 
 from .abc import CT, ConnectionCB, ConnectFailedCB
 from .errors import PoolTimeout, TooManyRequests
 from ._compat import ConnectionTimeout
 from ._acompat import Event
 from .base_null_pool import _BaseNullConnectionPool
 from .pool import ConnectionPool, AddConnection
 
 logger = logging.getLogger("psycopg.pool")
 
 
 class NullConnectionPool(_BaseNullConnectionPool, ConnectionPool[CT]):
-    @overload
-    def __init__(
-        self: NullConnectionPool[Connection[TupleRow]],
-        conninfo: str = "",
-        *,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[ConnectionCB[CT]] = ...,
-        check: Optional[ConnectionCB[CT]] = ...,
-        reset: Optional[ConnectionCB[CT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[ConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
-    @overload
-    def __init__(
-        self: NullConnectionPool[CT],
-        conninfo: str = "",
-        *,
-        connection_class: Type[CT] = ...,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[ConnectionCB[CT]] = ...,
-        check: Optional[ConnectionCB[CT]] = ...,
-        reset: Optional[ConnectionCB[CT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[ConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
     def __init__(
         self,
         conninfo: str = "",
         *,
         connection_class: Type[CT] = cast(Type[CT], Connection),
         kwargs: Optional[Dict[str, Any]] = None,
         min_size: int = 0,
@@ -140,14 +92,17 @@
         with self._lock:
             assert self._pool_full_event
             self._pool_full_event = None
 
         logger.info("pool %r is ready to use", self.name)
 
     def _get_ready_connection(self, timeout: Optional[float]) -> Optional[CT]:
+        if timeout is not None and timeout <= 0.0:
+            raise PoolTimeout()
+
         conn: Optional[CT] = None
         if self.max_size == 0 or self._nconns < self.max_size:
             # Create a new connection for the client
             try:
                 conn = self._connect(timeout=timeout)
             except ConnectionTimeout as ex:
                 raise PoolTimeout(str(ex)) from None
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool/null_pool_async.py` & `psycopg-pool-3.2.1/psycopg_pool/null_pool_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,78 +3,30 @@
 """
 
 # Copyright (C) 2022 The Psycopg Team
 
 from __future__ import annotations
 
 import logging
-from typing import Any, cast, Dict, Optional, overload, Type
+from typing import Any, cast, Dict, Optional, Type
 
 from psycopg import AsyncConnection
 from psycopg.pq import TransactionStatus
-from psycopg.rows import TupleRow
 
 from .abc import ACT, AsyncConnectionCB, AsyncConnectFailedCB
 from .errors import PoolTimeout, TooManyRequests
 from ._compat import ConnectionTimeout
 from ._acompat import AEvent
 from .base_null_pool import _BaseNullConnectionPool
 from .pool_async import AsyncConnectionPool, AddConnection
 
 logger = logging.getLogger("psycopg.pool")
 
 
 class AsyncNullConnectionPool(_BaseNullConnectionPool, AsyncConnectionPool[ACT]):
-    @overload
-    def __init__(
-        self: AsyncNullConnectionPool[AsyncConnection[TupleRow]],
-        conninfo: str = "",
-        *,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[AsyncConnectionCB[ACT]] = ...,
-        check: Optional[AsyncConnectionCB[ACT]] = ...,
-        reset: Optional[AsyncConnectionCB[ACT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[AsyncConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
-    @overload
-    def __init__(
-        self: AsyncNullConnectionPool[ACT],
-        conninfo: str = "",
-        *,
-        connection_class: Type[ACT] = ...,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[AsyncConnectionCB[ACT]] = ...,
-        check: Optional[AsyncConnectionCB[ACT]] = ...,
-        reset: Optional[AsyncConnectionCB[ACT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[AsyncConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
     def __init__(
         self,
         conninfo: str = "",
         *,
         connection_class: Type[ACT] = cast(Type[ACT], AsyncConnection),
         kwargs: Optional[Dict[str, Any]] = None,
         min_size: int = 0,  # Note: min_size default value changed to 0.
@@ -137,14 +89,17 @@
         async with self._lock:
             assert self._pool_full_event
             self._pool_full_event = None
 
         logger.info("pool %r is ready to use", self.name)
 
     async def _get_ready_connection(self, timeout: Optional[float]) -> Optional[ACT]:
+        if timeout is not None and timeout <= 0.0:
+            raise PoolTimeout()
+
         conn: Optional[ACT] = None
         if self.max_size == 0 or self._nconns < self.max_size:
             # Create a new connection for the client
             try:
                 conn = await self._connect(timeout=timeout)
             except ConnectionTimeout as ex:
                 raise PoolTimeout(str(ex)) from None
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool/pool.py` & `psycopg-pool-3.2.1/psycopg_pool/pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,86 +11,37 @@
 
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from time import monotonic
 from types import TracebackType
 from typing import Any, Iterator, cast, Dict, Generic, List
-from typing import Optional, overload, Sequence, Type, TypeVar
+from typing import Optional, Sequence, Type
 from weakref import ref
 from contextlib import contextmanager
 
 from psycopg import errors as e
 from psycopg import Connection
 from psycopg.pq import TransactionStatus
-from psycopg.rows import TupleRow
 
 from .abc import CT, ConnectionCB, ConnectFailedCB
-from .base import ConnectionAttempt, BasePool
+from .base import AttemptWithBackoff, BasePool
 from .errors import PoolClosed, PoolTimeout, TooManyRequests
-from ._compat import Deque
+from ._compat import Deque, Self
 from ._acompat import Condition, Event, Lock, Queue, Worker, spawn, gather
-from ._acompat import current_thread_name
+from ._acompat import sleep, current_thread_name
 from .sched import Scheduler
 
 
 logger = logging.getLogger("psycopg.pool")
 
 
 class ConnectionPool(Generic[CT], BasePool):
-    _Self = TypeVar("_Self", bound="ConnectionPool[CT]")
     _pool: Deque[CT]
 
-    @overload
-    def __init__(
-        self: ConnectionPool[Connection[TupleRow]],
-        conninfo: str = "",
-        *,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[ConnectionCB[CT]] = ...,
-        check: Optional[ConnectionCB[CT]] = ...,
-        reset: Optional[ConnectionCB[CT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[ConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
-    @overload
-    def __init__(
-        self: ConnectionPool[CT],
-        conninfo: str = "",
-        *,
-        connection_class: Type[CT] = ...,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[ConnectionCB[CT]] = ...,
-        check: Optional[ConnectionCB[CT]] = ...,
-        reset: Optional[ConnectionCB[CT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[ConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
     def __init__(
         self,
         conninfo: str = "",
         *,
         connection_class: Type[CT] = cast(Type[CT], Connection),
         kwargs: Optional[Dict[str, Any]] = None,
         min_size: int = 4,
@@ -232,41 +183,58 @@
         You should preferably use `connection()`. Use this function only if
         it is not possible to use the connection as context manager.
 
         After using this function you *must* call a corresponding `putconn()`:
         failing to do so will deplete the pool. A depleted pool is a sad pool:
         you don't want a depleted pool.
         """
-        t0 = monotonic()
         if timeout is None:
             timeout = self.timeout
-        deadline = t0 + timeout
+        deadline = monotonic() + timeout
 
         logger.info("connection requested from %r", self.name)
         self._stats[self._REQUESTS_NUM] += 1
 
         self._check_open_getconn()
 
         try:
-            while True:
-                conn = self._getconn_unchecked(deadline - monotonic())
-                try:
-                    self._check_connection(conn)
-                except Exception:
-                    self._putconn(conn, from_getconn=True)
-                else:
-                    logger.info("connection given by %r", self.name)
-                    return conn
+            return self._getconn_with_check_loop(deadline)
         # Re-raise the timeout exception presenting the user the global
         # timeout, not the per-attempt one.
         except PoolTimeout:
             raise PoolTimeout(
                 f"couldn't get a connection after {timeout:.2f} sec"
             ) from None
 
+    def _getconn_with_check_loop(self, deadline: float) -> CT:
+        attempt: AttemptWithBackoff | None = None
+
+        while True:
+            conn = self._getconn_unchecked(deadline - monotonic())
+            try:
+                self._check_connection(conn)
+            except Exception:
+                self._putconn(conn, from_getconn=True)
+            else:
+                logger.info("connection given by %r", self.name)
+                return conn
+
+            # Delay further checks to avoid a busy loop, using the same
+            # backoff policy used in reconnection attempts.
+            now = monotonic()
+            if not attempt:
+                attempt = AttemptWithBackoff(timeout=deadline - now)
+            else:
+                attempt.update_delay(now)
+
+            if attempt.time_to_give_up(now):
+                raise PoolTimeout()
+            else:
+                sleep(attempt.delay)
+
     def _getconn_unchecked(self, timeout: float) -> CT:
         # Critical section: decide here if there's a connection ready
         # or if the client needs to wait.
         with self._lock:
             conn = self._get_ready_connection(timeout)
             if not conn:
                 # No connection available: put the client in the waiting queue
@@ -294,14 +262,17 @@
         # Note that this property shouldn't be set while the connection is in
         # the pool, to avoid to create a reference loop.
         conn._pool = self
         return conn
 
     def _get_ready_connection(self, timeout: Optional[float]) -> Optional[CT]:
         """Return a connection, if the client deserves one."""
+        if timeout is not None and timeout <= 0.0:
+            raise PoolTimeout()
+
         conn: Optional[CT] = None
         if self._pool:
             # Take a connection ready out of the pool
             conn = self._pool.popleft()
             if len(self._pool) < self._nconns_min:
                 self._nconns_min = len(self._pool)
         elif self.max_waiting and len(self._waiting) >= self.max_waiting:
@@ -487,15 +458,15 @@
             conn.close()
 
         # Wait for the worker tasks to terminate
         assert self._sched_runner is not None
         sched_runner, self._sched_runner = (self._sched_runner, None)
         gather(sched_runner, *workers, timeout=timeout)
 
-    def __enter__(self: _Self) -> _Self:
+    def __enter__(self) -> Self:
         self._open_implicit = False
         self.open()
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
@@ -622,15 +593,15 @@
         self._stats[self._CONNECTIONS_NUM] += 1
         kwargs = self.kwargs
         if timeout:
             kwargs = kwargs.copy()
             kwargs["connect_timeout"] = max(round(timeout), 1)
         t0 = monotonic()
         try:
-            conn: CT = cast(CT, self.connection_class.connect(self.conninfo, **kwargs))
+            conn = self.connection_class.connect(self.conninfo, **kwargs)
         except Exception:
             self._stats[self._CONNECTIONS_ERRORS] += 1
             raise
         else:
             t1 = monotonic()
             self._stats[self._CONNECTIONS_MS] += int(1000.0 * (t1 - t0))
 
@@ -647,26 +618,26 @@
                 )
 
         # Set an expiry date, with some randomness to avoid mass reconnection
         self._set_connection_expiry_date(conn)
         return conn
 
     def _add_connection(
-        self, attempt: Optional[ConnectionAttempt], growing: bool = False
+        self, attempt: Optional[AttemptWithBackoff], growing: bool = False
     ) -> None:
         """Try to connect and add the connection to the pool.
 
         If failed, reschedule a new attempt in the future for a few times, then
         give up, decrease the pool connections number and call
         `self.reconnect_failed()`.
 
         """
         now = monotonic()
         if not attempt:
-            attempt = ConnectionAttempt(reconnect_timeout=self.reconnect_timeout)
+            attempt = AttemptWithBackoff(timeout=self.reconnect_timeout)
 
         try:
             conn = self._connect()
         except Exception as ex:
             logger.warning(f"error connecting in {self.name!r}: {ex}")
             if attempt.time_to_give_up(now):
                 logger.warning(
@@ -953,15 +924,15 @@
         pass
 
 
 class AddConnection(MaintenanceTask):
     def __init__(
         self,
         pool: ConnectionPool[Any],
-        attempt: Optional[ConnectionAttempt] = None,
+        attempt: Optional[AttemptWithBackoff] = None,
         growing: bool = False,
     ):
         super().__init__(pool)
         self.attempt = attempt
         self.growing = growing
 
     def _run(self, pool: ConnectionPool[Any]) -> None:
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool/pool_async.py` & `psycopg-pool-3.2.1/psycopg_pool/pool_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,88 +8,39 @@
 
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from time import monotonic
 from types import TracebackType
 from typing import Any, AsyncIterator, cast, Dict, Generic, List
-from typing import Optional, overload, Sequence, Type, TypeVar
+from typing import Optional, Sequence, Type
 from weakref import ref
 from contextlib import asynccontextmanager
 
 from psycopg import errors as e
 from psycopg import AsyncConnection
 from psycopg.pq import TransactionStatus
-from psycopg.rows import TupleRow
 
 from .abc import ACT, AsyncConnectionCB, AsyncConnectFailedCB
-from .base import ConnectionAttempt, BasePool
+from .base import AttemptWithBackoff, BasePool
 from .errors import PoolClosed, PoolTimeout, TooManyRequests
-from ._compat import Deque
+from ._compat import Deque, Self
 from ._acompat import ACondition, AEvent, ALock, AQueue, AWorker, aspawn, agather
-from ._acompat import current_task_name
+from ._acompat import asleep, current_task_name
 from .sched_async import AsyncScheduler
 
 if True:  # ASYNC
     import asyncio
 
 logger = logging.getLogger("psycopg.pool")
 
 
 class AsyncConnectionPool(Generic[ACT], BasePool):
-    _Self = TypeVar("_Self", bound="AsyncConnectionPool[ACT]")
     _pool: Deque[ACT]
 
-    @overload
-    def __init__(
-        self: AsyncConnectionPool[AsyncConnection[TupleRow]],
-        conninfo: str = "",
-        *,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[AsyncConnectionCB[ACT]] = ...,
-        check: Optional[AsyncConnectionCB[ACT]] = ...,
-        reset: Optional[AsyncConnectionCB[ACT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[AsyncConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
-    @overload
-    def __init__(
-        self: AsyncConnectionPool[ACT],
-        conninfo: str = "",
-        *,
-        connection_class: Type[ACT] = ...,
-        kwargs: Optional[Dict[str, Any]] = ...,
-        min_size: int = ...,
-        max_size: Optional[int] = ...,
-        open: bool | None = ...,
-        configure: Optional[AsyncConnectionCB[ACT]] = ...,
-        check: Optional[AsyncConnectionCB[ACT]] = ...,
-        reset: Optional[AsyncConnectionCB[ACT]] = ...,
-        name: Optional[str] = ...,
-        timeout: float = ...,
-        max_waiting: int = ...,
-        max_lifetime: float = ...,
-        max_idle: float = ...,
-        reconnect_timeout: float = ...,
-        reconnect_failed: Optional[AsyncConnectFailedCB] = ...,
-        num_workers: int = ...,
-    ):
-        ...
-
     def __init__(
         self,
         conninfo: str = "",
         *,
         connection_class: Type[ACT] = cast(Type[ACT], AsyncConnection),
         kwargs: Optional[Dict[str, Any]] = None,
         min_size: int = 4,
@@ -252,42 +203,59 @@
         You should preferably use `connection()`. Use this function only if
         it is not possible to use the connection as context manager.
 
         After using this function you *must* call a corresponding `putconn()`:
         failing to do so will deplete the pool. A depleted pool is a sad pool:
         you don't want a depleted pool.
         """
-        t0 = monotonic()
         if timeout is None:
             timeout = self.timeout
-        deadline = t0 + timeout
+        deadline = monotonic() + timeout
 
         logger.info("connection requested from %r", self.name)
         self._stats[self._REQUESTS_NUM] += 1
 
         self._check_open_getconn()
 
         try:
-            while True:
-                conn = await self._getconn_unchecked(deadline - monotonic())
-                try:
-                    await self._check_connection(conn)
-                except Exception:
-                    await self._putconn(conn, from_getconn=True)
-                else:
-                    logger.info("connection given by %r", self.name)
-                    return conn
+            return await self._getconn_with_check_loop(deadline)
 
         # Re-raise the timeout exception presenting the user the global
         # timeout, not the per-attempt one.
         except PoolTimeout:
             raise PoolTimeout(
                 f"couldn't get a connection after {timeout:.2f} sec"
             ) from None
 
+    async def _getconn_with_check_loop(self, deadline: float) -> ACT:
+        attempt: AttemptWithBackoff | None = None
+
+        while True:
+            conn = await self._getconn_unchecked(deadline - monotonic())
+            try:
+                await self._check_connection(conn)
+            except Exception:
+                await self._putconn(conn, from_getconn=True)
+            else:
+                logger.info("connection given by %r", self.name)
+                return conn
+
+            # Delay further checks to avoid a busy loop, using the same
+            # backoff policy used in reconnection attempts.
+            now = monotonic()
+            if not attempt:
+                attempt = AttemptWithBackoff(timeout=deadline - now)
+            else:
+                attempt.update_delay(now)
+
+            if attempt.time_to_give_up(now):
+                raise PoolTimeout()
+            else:
+                await asleep(attempt.delay)
+
     async def _getconn_unchecked(self, timeout: float) -> ACT:
         # Critical section: decide here if there's a connection ready
         # or if the client needs to wait.
         async with self._lock:
             conn = await self._get_ready_connection(timeout)
             if not conn:
                 # No connection available: put the client in the waiting queue
@@ -315,14 +283,17 @@
         # Note that this property shouldn't be set while the connection is in
         # the pool, to avoid to create a reference loop.
         conn._pool = self
         return conn
 
     async def _get_ready_connection(self, timeout: Optional[float]) -> Optional[ACT]:
         """Return a connection, if the client deserves one."""
+        if timeout is not None and timeout <= 0.0:
+            raise PoolTimeout()
+
         conn: Optional[ACT] = None
         if self._pool:
             # Take a connection ready out of the pool
             conn = self._pool.popleft()
             if len(self._pool) < self._nconns_min:
                 self._nconns_min = len(self._pool)
         elif self.max_waiting and len(self._waiting) >= self.max_waiting:
@@ -515,15 +486,15 @@
             await conn.close()
 
         # Wait for the worker tasks to terminate
         assert self._sched_runner is not None
         sched_runner, self._sched_runner = self._sched_runner, None
         await agather(sched_runner, *workers, timeout=timeout)
 
-    async def __aenter__(self: _Self) -> _Self:
+    async def __aenter__(self) -> Self:
         self._open_implicit = False
         await self.open()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
@@ -666,17 +637,15 @@
         self._stats[self._CONNECTIONS_NUM] += 1
         kwargs = self.kwargs
         if timeout:
             kwargs = kwargs.copy()
             kwargs["connect_timeout"] = max(round(timeout), 1)
         t0 = monotonic()
         try:
-            conn: ACT = cast(
-                ACT, await self.connection_class.connect(self.conninfo, **kwargs)
-            )
+            conn = await self.connection_class.connect(self.conninfo, **kwargs)
         except Exception:
             self._stats[self._CONNECTIONS_ERRORS] += 1
             raise
         else:
             t1 = monotonic()
             self._stats[self._CONNECTIONS_MS] += int(1000.0 * (t1 - t0))
 
@@ -693,26 +662,26 @@
                 )
 
         # Set an expiry date, with some randomness to avoid mass reconnection
         self._set_connection_expiry_date(conn)
         return conn
 
     async def _add_connection(
-        self, attempt: Optional[ConnectionAttempt], growing: bool = False
+        self, attempt: Optional[AttemptWithBackoff], growing: bool = False
     ) -> None:
         """Try to connect and add the connection to the pool.
 
         If failed, reschedule a new attempt in the future for a few times, then
         give up, decrease the pool connections number and call
         `self.reconnect_failed()`.
 
         """
         now = monotonic()
         if not attempt:
-            attempt = ConnectionAttempt(reconnect_timeout=self.reconnect_timeout)
+            attempt = AttemptWithBackoff(timeout=self.reconnect_timeout)
 
         try:
             conn = await self._connect()
         except Exception as ex:
             logger.warning(f"error connecting in {self.name!r}: {ex}")
             if attempt.time_to_give_up(now):
                 logger.warning(
@@ -1004,15 +973,15 @@
         pass
 
 
 class AddConnection(MaintenanceTask):
     def __init__(
         self,
         pool: AsyncConnectionPool[Any],
-        attempt: Optional[ConnectionAttempt] = None,
+        attempt: Optional[AttemptWithBackoff] = None,
         growing: bool = False,
     ):
         super().__init__(pool)
         self.attempt = attempt
         self.growing = growing
 
     async def _run(self, pool: AsyncConnectionPool[Any]) -> None:
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool/sched.py` & `psycopg-pool-3.2.1/psycopg_pool/sched.py`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/psycopg_pool/sched_async.py` & `psycopg-pool-3.2.1/psycopg_pool/sched_async.py`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/psycopg_pool.egg-info/PKG-INFO` & `psycopg-pool-3.2.1/psycopg_pool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg-pool
-Version: 3.2.0
+Version: 3.2.1
 Summary: Connection Pool for Psycopg
 Home-page: https://psycopg.org/psycopg3/
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://psycopg.org/
 Project-URL: Documentation, https://www.psycopg.org/psycopg3/docs/advanced/pool.html
@@ -20,22 +20,24 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: typing-extensions>=3.10
+Requires-Dist: typing-extensions>=4.4
 
 Psycopg 3: PostgreSQL database adapter for Python - Connection Pool
 ===================================================================
 
 This distribution package is an optional component of `Psycopg 3`__: it
 contains the optional connection pool package `psycopg_pool`__.
```

### Comparing `psycopg-pool-3.2.0/psycopg_pool.egg-info/SOURCES.txt` & `psycopg-pool-3.2.1/psycopg_pool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psycopg-pool-3.2.0/setup.cfg` & `psycopg-pool-3.2.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = psycopg-pool
 description = Connection Pool for Psycopg
 url = https://psycopg.org/psycopg3/
 author = Daniele Varrazzo
 author_email = daniele.varrazzo@gmail.com
 license = GNU Lesser General Public License v3 (LGPLv3)
-version = 3.2.0
+version = 3.2.1
 project_urls = 
 	Homepage = https://psycopg.org/
 	Documentation = https://www.psycopg.org/psycopg3/docs/advanced/pool.html
 	Changes = https://psycopg.org/psycopg3/docs/news_pool.html
 	Code = https://github.com/psycopg/psycopg
 	Issue Tracker = https://github.com/psycopg/psycopg/issues
 	Download = https://pypi.org/project/psycopg-pool/
@@ -22,28 +22,30 @@
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
+	Programming Language :: Python :: Implementation :: CPython
+	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Database
 	Topic :: Database :: Front-Ends
 	Topic :: Software Development
 	Topic :: Software Development :: Libraries :: Python Modules
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license_files = LICENSE.txt
 
 [options]
 python_requires = >= 3.8
 packages = find:
 zip_safe = False
 install_requires = 
-	typing-extensions >= 3.10
+	typing-extensions >= 4.4
 
 [options.package_data]
 psycopg_pool = py.typed
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

