# Comparing `tmp/rate_control-4.1.0.tar.gz` & `tmp/rate_control-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rate_control-4.1.0.tar", max compression
+gzip compressed data, was "rate_control-4.1.1.tar", max compression
```

## Comparing `rate_control-4.1.0.tar` & `rate_control-4.1.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1101 2024-05-04 07:19:02.649495 rate_control-4.1.0/LICENSE
--rw-r--r--   0        0        0     3849 2024-05-04 07:19:02.649495 rate_control-4.1.0/README.rst
--rw-r--r--   0        0        0     2828 2024-05-04 07:19:06.373528 rate_control-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      620 2024-05-04 07:19:02.649495 rate_control-4.1.0/rate_control/__init__.py
--rw-r--r--   0        0        0     3858 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_bucket_group.py
--rw-r--r--   0        0        0      267 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/__init__.py
--rw-r--r--   0        0        0      344 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_abc.py
--rw-r--r--   0        0        0     2539 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_base_rate.py
--rw-r--r--   0        0        0      744 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_capacity_updating.py
--rw-r--r--   0        0        0      948 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_token_based.py
--rw-r--r--   0        0        0      997 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_windowed.py
--rw-r--r--   0        0        0     1074 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_fixed_window_counter.py
--rw-r--r--   0        0        0     1412 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_leaky_bucket.py
--rw-r--r--   0        0        0      679 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_sliding_window_log.py
--rw-r--r--   0        0        0      246 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/__init__.py
--rw-r--r--   0        0        0     1434 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_abc.py
--rw-r--r--   0        0        0     4580 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_bucket_based.py
--rw-r--r--   0        0        0     1632 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_noop_controller.py
--rw-r--r--   0        0        0     1172 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_rate_limiter.py
--rw-r--r--   0        0        0     8333 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_scheduler.py
--rw-r--r--   0        0        0      111 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_enums/__init__.py
--rw-r--r--   0        0        0      262 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_enums/_duration.py
--rw-r--r--   0        0        0      350 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_enums/_priority.py
--rw-r--r--   0        0        0      297 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_errors.py
--rw-r--r--   0        0        0      105 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/__init__.py
--rw-r--r--   0        0        0      781 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_mk_repr.py
--rw-r--r--   0        0        0      492 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_protocols.py
--rw-r--r--   0        0        0     1502 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_request.py
--rw-r--r--   0        0        0     1673 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_validation.py
--rw-r--r--   0        0        0        0 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/py.typed
--rw-r--r--   0        0        0      202 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/__init__.py
--rw-r--r--   0        0        0     1559 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_abc.py
--rw-r--r--   0        0        0     1365 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_fifo.py
--rw-r--r--   0        0        0     1340 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_lifo.py
--rw-r--r--   0        0        0     1687 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_priority.py
--rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 rate_control-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-05-10 08:45:40.565254 rate_control-4.1.1/LICENSE
+-rw-r--r--   0        0        0     3849 2024-05-10 08:45:40.565254 rate_control-4.1.1/README.rst
+-rw-r--r--   0        0        0     2828 2024-05-10 08:45:49.745347 rate_control-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      620 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/__init__.py
+-rw-r--r--   0        0        0     3809 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_bucket_group.py
+-rw-r--r--   0        0        0      267 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_base/__init__.py
+-rw-r--r--   0        0        0     1774 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_base/_abc.py
+-rw-r--r--   0        0        0     2613 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_base/_base_rate.py
+-rw-r--r--   0        0        0      724 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_base/_capacity_updating.py
+-rw-r--r--   0        0        0      906 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_base/_token_based.py
+-rw-r--r--   0        0        0      977 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_base/_windowed.py
+-rw-r--r--   0        0        0     1034 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_fixed_window_counter.py
+-rw-r--r--   0        0        0     1372 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_leaky_bucket.py
+-rw-r--r--   0        0        0      659 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_buckets/_sliding_window_log.py
+-rw-r--r--   0        0        0      246 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_controllers/__init__.py
+-rw-r--r--   0        0        0     1414 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_controllers/_abc.py
+-rw-r--r--   0        0        0     4482 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_controllers/_bucket_based.py
+-rw-r--r--   0        0        0     1616 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_controllers/_noop_controller.py
+-rw-r--r--   0        0        0     1152 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_controllers/_rate_limiter.py
+-rw-r--r--   0        0        0     8411 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_controllers/_scheduler.py
+-rw-r--r--   0        0        0      150 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_enums/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_enums/_duration.py
+-rw-r--r--   0        0        0      350 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_enums/_priority.py
+-rw-r--r--   0        0        0      431 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_enums/_state.py
+-rw-r--r--   0        0        0      297 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_errors.py
+-rw-r--r--   0        0        0      166 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_helpers/__init__.py
+-rw-r--r--   0        0        0     1640 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_helpers/_context_aware.py
+-rw-r--r--   0        0        0      781 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_helpers/_mk_repr.py
+-rw-r--r--   0        0        0      492 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_helpers/_protocols.py
+-rw-r--r--   0        0        0     1502 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_helpers/_request.py
+-rw-r--r--   0        0        0     1673 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/_helpers/_validation.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/py.typed
+-rw-r--r--   0        0        0      202 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/queues/__init__.py
+-rw-r--r--   0        0        0     1559 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/queues/_abc.py
+-rw-r--r--   0        0        0     1365 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/queues/_fifo.py
+-rw-r--r--   0        0        0     1340 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/queues/_lifo.py
+-rw-r--r--   0        0        0     1687 2024-05-10 08:45:40.569254 rate_control-4.1.1/rate_control/queues/_priority.py
+-rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 rate_control-4.1.1/PKG-INFO
```

### Comparing `rate_control-4.1.0/LICENSE` & `rate_control-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/README.rst` & `rate_control-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/pyproject.toml` & `rate_control-4.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rate-control"
-version = "4.1.0"
+version = "4.1.1"
 description = "Versatile rate controlling in Python"
 authors = ["Corentin Régent <corentin.regent.pro@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/corentin-regent/rate-control"
 repository = "https://github.com/corentin-regent/rate-control"
 documentation = "https://rate-control.readthedocs.io/"
```

### Comparing `rate_control-4.1.0/rate_control/__init__.py` & `rate_control-4.1.1/rate_control/__init__.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/rate_control/_bucket_group.py` & `rate_control-4.1.1/rate_control/_bucket_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 __all__ = [
     'BucketGroup',
 ]
 
 import sys
 from contextlib import AsyncExitStack, suppress
-from typing import Any, Iterator
+from typing import Any, Iterator, Optional
 
 from anyio import WouldBlock, create_memory_object_stream, create_task_group
 
 from rate_control._buckets import Bucket
-from rate_control._helpers import mk_repr
+from rate_control._helpers import ContextAware, mk_repr
 
 if sys.version_info >= (3, 9):
     from collections.abc import Iterable
 else:
     from typing import Iterable
 
 if sys.version_info >= (3, 11):
@@ -23,26 +23,16 @@
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
-class BucketGroup(Bucket, Iterable[Bucket]):
-    """Bucket that aggregates other buckets."""
-
-    __slots__ = (
-        '_buckets',
-        '_recv_stream',
-        '_refill_event',
-        '_send_stream',
-        '_should_enter_context',
-        '_stack',
-        '_task_group',
-    )
+class BucketGroup(ContextAware, Bucket, Iterable[Bucket]):
+    """Composite bucket that aggregates other buckets."""
 
     def __init__(self, *buckets: Bucket, should_enter_context: bool = True, **kwargs: Any) -> None:
         """
         Args:
             buckets: The buckets to aggregate within this bucket group.
             should_enter_context: Whether entering the context of the bucket group
                 should also enter the context of the underlying buckets.
@@ -55,23 +45,25 @@
 
     @override
     def __repr__(self) -> str:
         return mk_repr(self, *self._buckets, should_enter_context=self._should_enter_context)
 
     @override
     async def __aenter__(self) -> Self:
+        await super().__aenter__()
         self._stack = await AsyncExitStack().__aenter__()
         self._task_group = await self._stack.enter_async_context(create_task_group())
         await self._init_buckets()
         return self
 
     @override
-    async def __aexit__(self, *exc_info: Any) -> None:
+    async def __aexit__(self, *exc_info: Any) -> Optional[bool]:
         self._task_group.cancel_scope.cancel()
         await self._stack.__aexit__(*exc_info)
+        return await super().__aexit__(*exc_info)
 
     @override
     def __iter__(self) -> Iterator[Bucket]:
         return iter(self._buckets)
 
     async def _init_buckets(self) -> None:
         for bucket in self._buckets:
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_base/_abc.py` & `rate_control-4.1.1/rate_control/_buckets/_base/_abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,18 @@
 from rate_control._errors import RateLimit
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-if sys.version_info >= (3, 12):
-    pass
-else:
-    pass
-
 
 class Bucket(ABC):
     """Abstract base class for buckets."""
 
-    __slots__ = ()
-
     async def __aenter__(self) -> Self:
         """Enter the bucket context.
 
         It may for example start scheduling replenishments.
         """
         return self
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_base/_base_rate.py` & `rate_control-4.1.1/rate_control/_buckets/_base/_base_rate.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,48 +4,49 @@
 
 import sys
 from abc import ABC, abstractmethod
 from typing import Any, Optional
 
 from anyio import Event, create_task_group, sleep
 
+from rate_control._buckets._base._abc import Bucket
 from rate_control._buckets._base._token_based import TokenBasedBucket
+from rate_control._helpers import ContextAware
 from rate_control._helpers._validation import validate_delay
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
-class BaseRateBucket(TokenBasedBucket, ABC):
+class BaseRateBucket(TokenBasedBucket, ContextAware, Bucket, ABC):
     """Base class for token buckets that refill at a certain rate."""
 
-    __slots__ = ('_delay', '_refill_event', '_task_group')
-
     def __init__(self, capacity: float, delay: float, **kwargs: Any) -> None:
         """
         Args:
             capacity: The number of tokens that can be acquired within `delay`.
             delay: The refill delay in seconds.
         """
         super().__init__(capacity, **kwargs)
         validate_delay(delay)
         self._delay = delay
         self._refill_event = Event()
 
     @override
     async def __aenter__(self) -> Self:
+        await super().__aenter__()
         self._task_group = await create_task_group().__aenter__()
-        return await super().__aenter__()
+        return self
 
     @override
     async def __aexit__(self, *exc_info: Any) -> Optional[bool]:
         self._task_group.cancel_scope.cancel()
         await self._task_group.__aexit__(*exc_info)
         return await super().__aexit__(*exc_info)
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_base/_capacity_updating.py` & `rate_control-4.1.1/rate_control/_buckets/_base/_capacity_updating.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from rate_control._buckets._base._token_based import TokenBasedBucket
 from rate_control._helpers._validation import validate_capacity
 
 
 class CapacityUpdatingBucket(TokenBasedBucket):
     """Mixin for buckets which token capacity can be updated."""
 
-    __slots__ = ()
-
     def update_capacity(self, new_capacity: float) -> None:
         """Update the bucket's token capacity.
 
         Changes take effect instantly, and the amount of remaining tokens is updated accordingly.
 
         Args:
             new_capacity: The new token capacity of the bucket.
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_base/_token_based.py` & `rate_control-4.1.1/rate_control/_buckets/_base/_token_based.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 else:
     from typing_extensions import override
 
 
 class TokenBasedBucket(Bucket, ABC):
     """Base class for buckets that monitor the requests using tokens."""
 
-    __slots__ = ('_capacity', '_tokens')
-
     def __init__(self, capacity: float, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         validate_capacity(capacity)
         self._tokens = self._capacity = capacity
 
     @override
     def can_acquire(self, tokens: float) -> bool:
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_base/_windowed.py` & `rate_control-4.1.1/rate_control/_buckets/_base/_windowed.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 else:
     from typing_extensions import override
 
 
 class BaseWindowedTokenBucket(BaseRateBucket, ABC):
     """Base class for token buckets that follow strategies based on time windows."""
 
-    __slots__ = ()
-
     def __init__(self, capacity: float, duration: float, **kwargs: Any) -> None:
         """
         Args:
             capacity: The number of tokens that can be acquired within ``duration``.
             duration: The window duration in seconds.
         """
         super().__init__(capacity, duration, **kwargs)
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_fixed_window_counter.py` & `rate_control-4.1.1/rate_control/_buckets/_fixed_window_counter.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 class FixedWindowCounter(BaseWindowedTokenBucket, CapacityUpdatingBucket):
     """Bucket whose refill strategy follows the fixed window counter algorithm.
 
     The bucket refills once every ``duration`` seconds, to cap its tokens back to ``capacity``.
     """
 
-    __slots__ = ('_scheduled_refill',)
-
     def __init__(self, capacity: float, duration: float, **kwargs: Any) -> None:
         super().__init__(capacity, duration, **kwargs)
         self._scheduled_refill = False
 
     @override
     def _should_schedule_refill(self) -> bool:
         if self._scheduled_refill:
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_leaky_bucket.py` & `rate_control-4.1.1/rate_control/_buckets/_leaky_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
 class LeakyBucket(BaseRateBucket):
     """Bucket whose refill strategy follows the leaky bucket algorithm.
 
     Only one request can get executed every ``delay`` seconds.
     """
 
-    __slots__ = ('_can_pass_through',)
-
     def __init__(self, delay: float, **kwargs: Any) -> None:
         """
         Args:
             delay: The delay before a new request can pass through.
         """
         super().__init__(capacity=math.inf, delay=delay, **kwargs)
         self._can_pass_through = True
```

### Comparing `rate_control-4.1.0/rate_control/_buckets/_sliding_window_log.py` & `rate_control-4.1.1/rate_control/_buckets/_sliding_window_log.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 class SlidingWindowLog(BaseWindowedTokenBucket, CapacityUpdatingBucket):
     """Bucket whose refill strategy follows the sliding window log algorithm.
 
     Every consumed tokens get replenished after ``duration`` seconds.
     """
 
-    __slots__ = ()
-
     @override
     def _should_schedule_refill(self) -> bool:
         return True
 
     @override
     def _refill(self, tokens: float) -> None:
         self._tokens += tokens
```

### Comparing `rate_control-4.1.0/rate_control/_controllers/_abc.py` & `rate_control-4.1.1/rate_control/_controllers/_abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 else:
     from typing_extensions import Self
 
 
 class RateController(ABC):
     """Abstract base class for rate controllers."""
 
-    __slots__ = ()
-
     async def __aenter__(self) -> Self:
         """Enter the controller's context."""
         return self
 
     async def __aexit__(self, *_: Any) -> Optional[bool]:
         """Exit the controller's context."""
         return False
```

### Comparing `rate_control-4.1.0/rate_control/_controllers/_bucket_based.py` & `rate_control-4.1.1/rate_control/_controllers/_bucket_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 else:
     from typing_extensions import override
 
 
 class BucketBasedRateController(RateController, ABC):
     """Mixin for rate controllers that use buckets."""
 
-    __slots__ = ('_bucket', '_concurrent_requests', '_max_concurrency', '_should_enter_context')
-
     def __init__(
         self,
         *buckets: Bucket,
         should_enter_context: bool = True,
         max_concurrency: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
```

### Comparing `rate_control-4.1.0/rate_control/_controllers/_noop_controller.py` & `rate_control-4.1.1/rate_control/_controllers/_noop_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,24 @@
 else:
     from typing_extensions import override
 
 
 class NoopController(RateController):
     """Rate controller that accepts all requests and does nothing."""
 
-    __slots__ = ()
-
     _instance: ClassVar['NoopController']
 
     def __new__(cls, *_: Any, **kwargs: Any) -> 'NoopController':
         """
         Positional arguments, accepted for consistency with other rate controllers, are ignored.
         Keyword arguments are passed to the super class constructor.
 
         Note:
             Implementation detail: The ``__new__`` method returns
-            a singleton instance, for optimal memory usage.
+            a singleton instance, for better memory management.
         """
         try:
             return cls._instance
         except AttributeError:
             cls._instance = super().__new__(cls, **kwargs)
             return cls._instance
```

### Comparing `rate_control-4.1.0/rate_control/_controllers/_rate_limiter.py` & `rate_control-4.1.1/rate_control/_controllers/_rate_limiter.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 else:
     from typing_extensions import override
 
 
 class RateLimiter(BucketBasedRateController):
     """Rate controller that raises an error if a request cannot be fulfilled instantly."""
 
-    __slots__ = ()
-
     @asynccontextmanager
     @override
     async def request(self, tokens: float = 1, **_: Any) -> AsyncIterator[None]:
         """Context manager that acquires the given amount of tokens while holding concurrency.
 
         Args:
             tokens: The number of tokens to acquire.
```

### Comparing `rate_control-4.1.0/rate_control/_controllers/_scheduler.py` & `rate_control-4.1.1/rate_control/_controllers/_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from contextlib import asynccontextmanager, suppress
 from typing import Any, NoReturn, Optional
 
 from anyio import create_task_group, get_cancelled_exc_class
 from anyio.lowlevel import checkpoint
 
 from rate_control._buckets import Bucket
+from rate_control._controllers._abc import RateController
 from rate_control._controllers._bucket_based import BucketBasedRateController
-from rate_control._enums import Priority
+from rate_control._enums import Priority, State
 from rate_control._errors import RateLimit, ReachedMaxPending
-from rate_control._helpers import Request, mk_repr
+from rate_control._helpers import ContextAware, Request, mk_repr
 from rate_control._helpers._validation import validate_max_pending
 from rate_control.queues import PriorityQueue, Queue
 
 if sys.version_info >= (3, 9):
     from collections.abc import AsyncIterator, Callable
 else:
     from typing import AsyncIterator, Callable
@@ -29,19 +30,17 @@
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
-class Scheduler(BucketBasedRateController):
+class Scheduler(BucketBasedRateController, ContextAware, RateController):
     """Rate controller that schedules requests for later processing."""
 
-    __slots__ = ('_max_pending', '_pending_requests', '_queues', '_task_group')
-
     def __init__(
         self,
         *buckets: Bucket,
         should_enter_context: bool = True,
         max_concurrency: Optional[int] = None,
         max_pending: Optional[int] = None,
         queue_factory: Callable[[], Queue[Request]] = PriorityQueue,
@@ -127,16 +126,18 @@
                 Defaults to `False`.
 
         Raises:
             RateLimit: The request cannot be processed instantly
                 but the ``fill_or_kill`` flag was set to `True`.
             ReachedMaxPending: The limit of pending requests was reached.
         """
-        if not hasattr(self, '_task_group'):
-            raise RuntimeError(f"Make sure to enter the scheduler's context using 'async with {self}'")
+        if self._state is not State.ENTERED:
+            raise RuntimeError(
+                f"Make sure to enter the scheduler's context using 'async with {type(self).__name__}(...)'"
+            )
         if not self.can_acquire(tokens):
             if fill_or_kill:
                 raise RateLimit(f'Cannot process the request for {tokens} tokens.')
             else:
                 await self._schedule_request(tokens, priority)
         if self._bucket is not None:
             self._bucket.acquire(tokens)
```

### Comparing `rate_control-4.1.0/rate_control/_helpers/_mk_repr.py` & `rate_control-4.1.1/rate_control/_helpers/_mk_repr.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/rate_control/_helpers/_request.py` & `rate_control-4.1.1/rate_control/_helpers/_request.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/rate_control/_helpers/_validation.py` & `rate_control-4.1.1/rate_control/_helpers/_validation.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/rate_control/queues/_abc.py` & `rate_control-4.1.1/rate_control/queues/_abc.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/rate_control/queues/_fifo.py` & `rate_control-4.1.1/rate_control/queues/_fifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/rate_control/queues/_lifo.py` & `rate_control-4.1.1/rate_control/queues/_lifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/rate_control/queues/_priority.py` & `rate_control-4.1.1/rate_control/queues/_priority.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.1.0/PKG-INFO` & `rate_control-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rate-control
-Version: 4.1.0
+Version: 4.1.1
 Summary: Versatile rate controlling in Python
 Home-page: https://github.com/corentin-regent/rate-control
 License: MIT
 Keywords: async,rate limit,schedule,throttle,token bucket
 Author: Corentin Régent
 Author-email: corentin.regent.pro@gmail.com
 Requires-Python: >=3.8,<4.0
```

