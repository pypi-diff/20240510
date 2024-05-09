# Comparing `tmp/clean_ioc-0.9.0.tar.gz` & `tmp/clean_ioc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.9.0.tar", max compression
+gzip compressed data, was "clean_ioc-1.0.0.tar", max compression
```

## Comparing `clean_ioc-0.9.0.tar` & `clean_ioc-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     2051 2023-08-31 08:36:53.269066 clean_ioc-0.9.0/CHANGES.rst
--rw-r--r--   0        0        0     1067 2023-01-24 06:53:30.309697 clean_ioc-0.9.0/LICENSE
--rw-r--r--   0        0        0    20308 2024-01-24 14:07:23.249191 clean_ioc-0.9.0/README.md
--rw-r--r--   0        0        0    45213 2024-01-29 21:28:48.975881 clean_ioc-0.9.0/clean_ioc/__init__.py
--rw-r--r--   0        0        0     1790 2024-01-23 15:03:27.389899 clean_ioc-0.9.0/clean_ioc/bundles.py
--rw-r--r--   0        0        0       34 2024-01-29 21:28:48.960772 clean_ioc-0.9.0/clean_ioc/ext/fastapi/__init__.py
--rw-r--r--   0        0        0     1261 2024-01-29 21:28:48.961191 clean_ioc-0.9.0/clean_ioc/ext/fastapi/core.py
--rw-r--r--   0        0        0      680 2024-01-24 13:17:58.247187 clean_ioc-0.9.0/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-03-01 21:27:40.225942 clean_ioc-0.9.0/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0      558 2023-07-26 15:24:12.965511 clean_ioc-0.9.0/clean_ioc/list_reduction_filters.py
--rw-r--r--   0        0        0     1251 2024-01-25 23:41:53.115843 clean_ioc-0.9.0/clean_ioc/modules.py
--rw-r--r--   0        0        0      405 2023-07-26 19:42:13.609646 clean_ioc-0.9.0/clean_ioc/parent_context_filters.py
--rw-r--r--   0        0        0     2228 2023-07-05 20:43:32.736456 clean_ioc-0.9.0/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-01-24 16:24:19.736817 clean_ioc-0.9.0/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6555 2023-07-26 09:59:03.030145 clean_ioc-0.9.0/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1399 2024-01-17 20:22:28.453624 clean_ioc-0.9.0/clean_ioc/utils.py
--rw-r--r--   0        0        0      603 2024-01-29 21:28:48.962161 clean_ioc-0.9.0/clean_ioc/value_factories.py
--rw-r--r--   0        0        0     1415 2024-01-29 21:28:48.976503 clean_ioc-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    21037 1970-01-01 00:00:00.000000 clean_ioc-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3641 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/CHANGES.rst
+-rw-r--r--   0        0        0     1067 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/LICENSE
+-rw-r--r--   0        0        0    20278 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/README.md
+-rw-r--r--   0        0        0       20 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/bundles.py
+-rw-r--r--   0        0        0    62149 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/core.py
+-rw-r--r--   0        0        0       20 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     1909 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/core.py
+-rw-r--r--   0        0        0     1255 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/py.typed
+-rw-r--r--   0        0        0     1262 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     2662 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0      563 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/list_reduction_filters.py
+-rw-r--r--   0        0        0     1779 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/node_filters.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/py.typed
+-rw-r--r--   0        0        0     4807 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      962 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6920 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1828 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/utils.py
+-rw-r--r--   0        0        0      564 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/value_factories.py
+-rw-r--r--   0        0        0     2146 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    21058 1970-01-01 00:00:00.000000 clean_ioc-1.0.0/PKG-INFO
```

### Comparing `clean_ioc-0.9.0/LICENSE` & `clean_ioc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.9.0/README.md` & `clean_ioc-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -568,24 +568,24 @@
 container.register(A, instance=a1, tags=[Tag("a", "a1")])
 container.register(A, instance=a2, tags=[Tag("a")])
 container.register(A, instance=a3)
 
 ar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1
 al1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]
 al2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]
-al3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]
-al4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]
+al3 = container.resolve(list[A], filter=~has_tag("a", "a1"))  # returns [a3, a2]
+al4 = container.resolve(list[A], filter=~has_tag("a")) # returns [a3]
 al5 = container.resolve(list[A]) # returns [a3, a2, a1]
 ```
 
 
 
-## Parent Context Filters
+## Parent Node Filters
 
-Registrations can also specify that should only apply to certain parents objects by setting the parent_context_filter
+Registrations can also specify that should only apply to certain parents objects by setting the parent_node_filter
 
 ```python
 class A:
     pass
 
 class B(A):
     pass
@@ -599,16 +599,16 @@
 
 class E:
     def __init__(self, a: A):
         self.a = a
 
 container = Container()
 
-container.register(A, B, parent_context_filter=parent_implementation_is(E))
-container.register(A, C, parent_context_filter=parent_implementation_is(D))
+container.register(A, B, parent_node_filter=implementation_type_is(E))
+container.register(A, C, parent_node_filter=implementation_type_is(D))
 container.register(D)
 container.register(E)
 
 e = container.resolve(E)
 d = container.resolve(D)
 
 type(e.a) # returns B
```

### Comparing `clean_ioc-0.9.0/clean_ioc/functional_utils.py` & `clean_ioc-1.0.0/clean_ioc/functional_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,20 @@
-from typing import TypeVar
 from collections.abc import Callable
+from typing import TypeVar
 
 TArg = TypeVar("TArg")
 
 
-def no_op(*args, **kwargs):
-    pass
-
-
-def identity(val: TArg) -> TArg:
-    return val
-
-
 def constant(val: TArg) -> Callable[..., TArg]:
     def fun(*_):
         return val
 
     return fun
 
 
-def compose(*funcs: Callable):
-    backwards = list(reversed(funcs))
-    initial, *rest = backwards
-
-    def composed_function(*args, **kwargs):
-        value = initial(*args, **kwargs)
-        for func in rest:
-            value = func(value)
-        return value
-
-    return composed_function
-
-
 def fn_not(func: Callable[..., bool]):
     def predicate(*args, **kwargs):
         return not func(*args, **kwargs)
 
     return predicate
 
 
@@ -60,7 +39,65 @@
 
 
 def fn_xor(*funcs: Callable[..., bool]):
     def predicate(*args, **kwargs):
         return len([f for f in funcs if f(*args, **kwargs)]) % 2 == 1
 
     return predicate
+
+
+def _predicate_and(left: Callable, right: Callable):
+    return lambda *args, **kwargs: left(*args, **kwargs) and right(*args, **kwargs)
+
+
+def _predicate_or(left: Callable, right: Callable):
+    return lambda *args, **kwargs: left(*args, **kwargs) or right(*args, **kwargs)
+
+
+def _predicate_xor(left: Callable, right: Callable):
+    return lambda *args, **kwargs: left(*args, **kwargs) ^ right(*args, **kwargs)
+
+
+def _predicate_not(func: Callable):
+    return lambda *args, **kwargs: not func(*args, **kwargs)
+
+
+class Predicate:
+    def __init__(self, func: Callable[..., bool]):
+        self.func = func
+
+    def __call__(self, *args, **kwargs):
+        return self.func(*args, **kwargs)
+
+    def __and__(self, other: Callable[..., bool]):
+        return Predicate(_predicate_and(self.func, other))
+
+    def __rand__(self, other: Callable[..., bool]):
+        return Predicate(_predicate_and(other, self.func))
+
+    def __or__(self, other: Callable[..., bool]):
+        return Predicate(_predicate_or(self.func, other))
+
+    def __ror__(self, other: Callable[..., bool]):
+        return Predicate(_predicate_or(other, self.func))
+
+    def __xor__(self, other: Callable[..., bool]):
+        return Predicate(_predicate_xor(self.func, other))
+
+    def __rxor__(self, other: Callable[..., bool]):
+        return Predicate(_predicate_xor(other, self.func))
+
+    def __invert__(self):
+        return Predicate(_predicate_not(self.func))
+
+    def __repr__(self) -> str:
+        return f"predicate({self.func.__name__})"
+
+
+def predicate(func: Callable[..., bool]):
+    if isinstance(func, Predicate):
+        return func
+    return Predicate(func)
+
+
+always_false = predicate(constant(False))
+always_true = predicate(constant(True))
```

### Comparing `clean_ioc-0.9.0/clean_ioc/typing_utils.py` & `clean_ioc-1.0.0/clean_ioc/typing_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,83 @@
-from typing import _GenericAlias, _SpecialGenericAlias, Protocol  # type: ignore
-from typing import Generic, TypeVar
-from collections.abc import Callable
-from typing import get_type_hints
 import types
+from collections.abc import Callable
 from queue import Queue
+from typing import (  # type: ignore
+    Generic,
+    Protocol,
+    TypeVar,
+    _GenericAlias,  # type: ignore
+    _SpecialGenericAlias,  # type: ignore
+    get_type_hints,
+)
+
+TypingGenericAlias = (_GenericAlias, _SpecialGenericAlias, types.GenericAlias)
+
+
+class GenericTypeMap:
+    def __init__(self, initial_map: dict[TypeVar | str, type | TypeVar] = {}):
+        self.inner_map: dict[str, TypeVar | type] = {}
+
+        for k, v in initial_map.items():
+            self[k] = v
+
+    @staticmethod
+    def from_type(type_cls: type):
+        generic_definitions = get_open_generic_aliases(type_cls)
+
+        generic_implementations = get_generic_aliases(type_cls)
+
+        generic_implementations = generic_implementations[: len(generic_definitions)]
+
+        generic_definitions.reverse()
+        generic_implementations.reverse()
+
+        mapping = {}
+
+        for idx, definition in enumerate(generic_definitions):
+            implementation = generic_implementations[idx]
+            additions = dict(zip(definition.__args__, implementation.__args__))
+            mapping = {**mapping, **additions}
+
+        return GenericTypeMap(mapping)
+
+    @classmethod
+    def _lookup_key(cls, key: TypeVar | str) -> str:
+        if isinstance(key, TypeVar):
+            return key.__name__
+        return key
+
+    def is_generic_mapping_open(self):
+        for k, v in self.inner_map.items():
+            if isinstance(v, TypeVar):
+                return True
+        return False
 
+    def is_generic_mapping_closed(self):
+        return not self.is_generic_mapping_open()
 
-typingGenericAlias = (_GenericAlias, _SpecialGenericAlias, types.GenericAlias)
+    def __getitem__(self, key: TypeVar | str):
+        return self.inner_map[self._lookup_key(key)]
+
+    def __setitem__(self, key: TypeVar | str, value: type | TypeVar):
+        self.inner_map[self._lookup_key(key)] = value
+
+    def values(self):
+        return self.inner_map.values()
+
+    def get(self, key: TypeVar | str, default=None):
+        return self.inner_map.get(self._lookup_key(key), default)
+
+    def items(self):
+        return self.inner_map.items()
+
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, GenericTypeMap):
+            return False
+        return self.inner_map == __value.inner_map
 
 
 def get_subclasses(cls: type, filter: Callable[[type], bool] = lambda t: True):
     queue = Queue()
     queue.put(cls)
     items = []
     while not queue.empty():
@@ -40,19 +107,16 @@
             if filter(sub):
                 items.append(sub)
 
     return items
 
 
 def is_generic_type_closed(cls: type):
-    m = get_typevar_to_type_mapping(cls)
-    for k, v in m.items():
-        if k == v:
-            return False
-    return True
+    m = GenericTypeMap.from_type(cls)
+    return m.is_generic_mapping_closed()
 
 
 def get_type_args(cls: type):
     return getattr(cls, "__args__", ())
 
 
 def is_generic_type(tp: type):
@@ -70,19 +134,15 @@
         is_generic_type(Generic[T]) == True
         is_generic_type(Iterable[int]) == True
         is_generic_type(Mapping) == True
         is_generic_type(MutableMapping[T, List[int]]) == True
         is_generic_type(Sequence[Union[str, bytes]]) == True
     """
 
-    return (
-        isinstance(tp, type)
-        and issubclass(tp, Generic)
-        or isinstance(tp, typingGenericAlias)
-    )
+    return isinstance(tp, type) and issubclass(tp, Generic) or isinstance(tp, TypingGenericAlias)
 
 
 def is_open_generic_type(cls: type):
     type_args = get_type_args(cls)
     if type_args:
         return any([isinstance(t, TypeVar) for t in type_args])
     else:
@@ -101,51 +161,14 @@
         for base in getattr(type_check, "__orig_bases__", ()):
             queue.put(base)
             queue.put(base.__origin__)
 
     return ()
 
 
-## OLD
-def get_closed_open_generic_alias(cls: type):
-    queue = Queue()
-    queue.put(cls)
-
-    while not queue.empty():
-        type_check = queue.get()
-        if type(type_check) == _GenericAlias:
-            return type_check
-
-        for base in getattr(type_check, "__orig_bases__", ()):
-            queue.put(base)
-            queue.put(base.__origin__)
-
-    return None
-
-
-def get_first_open_generic_alias(cls: type):
-    queue = Queue()
-    queue.put(cls)
-
-    if root_origin := (getattr(cls, "__origin__", None)):
-        queue.put(root_origin)
-
-    while not queue.empty():
-        type_check = queue.get()
-        if getattr(type_check, "__origin__", None) == Generic:
-            return type_check
-
-        for base in getattr(type_check, "__orig_bases__", ()):
-            queue.put(base)
-            if orig := getattr(base, "__origin__", None):
-                queue.put(orig)
-
-    return None
-
-
 ## NEW
 def get_open_generic_aliases(cls: type):
     queue = Queue()
     queue.put(cls)
     aliases = []
 
     if root_origin := (getattr(cls, "__origin__", None)):
@@ -180,45 +203,26 @@
             queue.put(base)
             if base_orig := getattr(base, "__origin__", None):
                 queue.put(base_orig)
 
     return aliases
 
 
-def get_typevar_to_type_mapping(cls: type) -> dict[type | TypeVar, type]:
-    generic_definitions = get_open_generic_aliases(cls)
-    generic_implementations = get_generic_aliases(cls)
-
-    generic_implementations = generic_implementations[: len(generic_definitions)]
-
-    generic_definitions.reverse()
-    generic_implementations.reverse()
-
-    mapping = {}
-
-    for idx, definition in enumerate(generic_definitions):
-        implementation = generic_implementations[idx]
-        additions = dict(zip(definition.__args__, implementation.__args__))
-        mapping = {**mapping, **additions}
-
-    return mapping
-
-
 def get_generic_types(cls: type):
-    mapping = get_typevar_to_type_mapping(cls)
+    mapping = GenericTypeMap.from_type(cls)
     return tuple(mapping.values())
 
 
 def try_to_complete_generic(open_type: _GenericAlias, closed_type: type) -> type:
     if not getattr(open_type, "__args__", None):
         return open_type
     if is_generic_type_closed(open_type):
         return open_type
 
-    mapping = get_typevar_to_type_mapping(closed_type)
+    mapping = GenericTypeMap.from_type(closed_type)
     new_args = tuple([mapping.get(a, a) for a in open_type.__args__])
     return open_type[new_args]
 
 
 def get_type_args_for_function(fn: Callable) -> dict[str, type]:
     return {k: v for k, v in get_type_hints(fn).items() if k != "return"}
```

### Comparing `clean_ioc-0.9.0/clean_ioc/value_factories.py` & `clean_ioc-1.0.0/clean_ioc/value_factories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any
-from . import _empty
-from .functional_utils import constant
 
-all_registrations = constant(True)
+from .core import EMPTY
+from .functional_utils import constant
 
 
 def use_default_value(default_value: Any, *_):
     """
     Returns the default value provided.
 
     Args:
@@ -26,8 +25,8 @@
 
     Returns:
         None
     """
     return constant(value)
 
 
-dont_use_default_parameter = constant(_empty())
+dont_use_default_value = constant(EMPTY)
```

### Comparing `clean_ioc-0.9.0/PKG-INFO` & `clean_ioc-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: clean-ioc
-Version: 0.9.0
+Name: clean_ioc
+Version: 1.0.0
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fastapi
 Requires-Dist: fastapi (>=0.101.0,<0.102.0) ; extra == "fastapi"
 Project-URL: Documentation, https://github.com/peter-daly/clean_ioc
 Project-URL: Repository, https://github.com/peter-daly/clean_ioc
 Description-Content-Type: text/markdown
 
 # Clean IoC
@@ -587,24 +588,24 @@
 container.register(A, instance=a1, tags=[Tag("a", "a1")])
 container.register(A, instance=a2, tags=[Tag("a")])
 container.register(A, instance=a3)
 
 ar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1
 al1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]
 al2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]
-al3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]
-al4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]
+al3 = container.resolve(list[A], filter=~has_tag("a", "a1"))  # returns [a3, a2]
+al4 = container.resolve(list[A], filter=~has_tag("a")) # returns [a3]
 al5 = container.resolve(list[A]) # returns [a3, a2, a1]
 ```
 
 
 
-## Parent Context Filters
+## Parent Node Filters
 
-Registrations can also specify that should only apply to certain parents objects by setting the parent_context_filter
+Registrations can also specify that should only apply to certain parents objects by setting the parent_node_filter
 
 ```python
 class A:
     pass
 
 class B(A):
     pass
@@ -618,16 +619,16 @@
 
 class E:
     def __init__(self, a: A):
         self.a = a
 
 container = Container()
 
-container.register(A, B, parent_context_filter=parent_implementation_is(E))
-container.register(A, C, parent_context_filter=parent_implementation_is(D))
+container.register(A, B, parent_node_filter=implementation_type_is(E))
+container.register(A, C, parent_node_filter=implementation_type_is(D))
 container.register(D)
 container.register(E)
 
 e = container.resolve(E)
 d = container.resolve(D)
 
 type(e.a) # returns B
```

