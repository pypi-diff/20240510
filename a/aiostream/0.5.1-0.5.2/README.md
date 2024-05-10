# Comparing `tmp/aiostream-0.5.1.tar.gz` & `tmp/aiostream-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiostream-0.5.1.tar", last modified: Thu Sep 28 23:04:56 2023, max compression
+gzip compressed data, was "aiostream-0.5.2.tar", last modified: Tue Oct 24 10:11:23 2023, max compression
```

## Comparing `aiostream-0.5.1.tar` & `aiostream-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 23:04:56.283627 aiostream-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-09-28 23:04:54.000000 aiostream-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-09-28 23:04:56.283627 aiostream-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2023-09-28 23:04:54.000000 aiostream-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 23:04:56.279627 aiostream-0.5.1/aiostream/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/aiter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16937 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 23:04:56.283627 aiostream-0.5.1/aiostream/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8969 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/stream/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-09-28 23:04:54.000000 aiostream-0.5.1/aiostream/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 23:04:56.283627 aiostream-0.5.1/aiostream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-09-28 23:04:56.000000 aiostream-0.5.1/aiostream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-09-28 23:04:56.000000 aiostream-0.5.1/aiostream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 23:04:56.000000 aiostream-0.5.1/aiostream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-28 23:04:56.000000 aiostream-0.5.1/aiostream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-28 23:04:56.000000 aiostream-0.5.1/aiostream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-09-28 23:04:56.283627 aiostream-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-09-28 23:04:54.000000 aiostream-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-10-24 10:11:20.000000 aiostream-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-10-24 10:11:23.284700 aiostream-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2023-10-24 10:11:20.000000 aiostream-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/aiostream/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/aiter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/aiostream/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/stream/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-10-24 10:11:20.000000 aiostream-0.5.2/aiostream/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 10:11:23.284700 aiostream-0.5.2/aiostream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2023-10-24 10:11:23.000000 aiostream-0.5.2/aiostream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-24 10:11:22.000000 aiostream-0.5.2/aiostream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-24 10:11:23.284700 aiostream-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-24 10:11:20.000000 aiostream-0.5.2/setup.py
```

### Comparing `aiostream-0.5.1/LICENSE` & `aiostream-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/PKG-INFO` & `aiostream-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiostream
-Version: 0.5.1
+Version: 0.5.2
 Summary: Generator-based operators for asynchronous iteration
 Home-page: https://github.com/vxgmichel/aiostream
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Description: aiostream
         =========
```

### Comparing `aiostream-0.5.1/README.rst` & `aiostream-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/__init__.py` & `aiostream-0.5.2/aiostream/__init__.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/aiter_utils.py` & `aiostream-0.5.2/aiostream/aiter_utils.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/core.py` & `aiostream-0.5.2/aiostream/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,31 +105,31 @@
     def __await__(self) -> Generator[Any, None, T]:
         """Await protocol.
 
         Safely iterate and return the last element.
         """
         return wait_stream(self).__await__()
 
-    def __or__(self, func: Callable[[BaseStream[T]], BaseStream[X]]) -> BaseStream[X]:
+    def __or__(self, func: Callable[[BaseStream[T]], X]) -> X:
         """Pipe protocol.
 
         Allow to pipe stream operators.
         """
         return func(self)
 
-    def __add__(self, value: BaseStream[X]) -> BaseStream[Union[X, T]]:
+    def __add__(self, value: AsyncIterable[X]) -> Stream[Union[X, T]]:
         """Addition protocol.
 
         Concatenate with a given asynchronous sequence.
         """
         from .stream import chain
 
         return chain(self, value)
 
-    def __getitem__(self, value: Union[int, slice]) -> BaseStream[T]:
+    def __getitem__(self, value: Union[int, slice]) -> Stream[T]:
         """Get item protocol.
 
         Accept index or slice to extract the corresponding item(s)
         """
         from .stream import getitem
 
         return getitem(self, value)
@@ -272,15 +272,17 @@
         ...
 
     def raw(
         self, source: AsyncIterable[A], /, *args: P.args, **kwargs: P.kwargs
     ) -> AsyncIterator[T]:
         ...
 
-    def pipe(self, source: AsyncIterable[A]) -> Stream[T]:
+    def pipe(
+        self, *args: P.args, **kwargs: P.kwargs
+    ) -> Callable[[AsyncIterable[A]], Stream[T]]:
         ...
 
 
 # Operator decorator
 
 
 def operator(
@@ -551,15 +553,15 @@
     # Gather attributes
     attrs = {
         "__init__": init,
         "__module__": module,
         "__doc__": doc,
         "raw": staticmethod(raw),
         "original": staticmethod(original),
-        "pipe": classmethod(pipe),
+        "pipe": classmethod(pipe),  # type: ignore[arg-type]
     }
 
     # Create operator class
     return cast(
         "PipableOperatorType[X, P, T]",
         type(name, bases, attrs),
     )
```

### Comparing `aiostream-0.5.1/aiostream/manager.py` & `aiostream-0.5.2/aiostream/manager.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/advanced.py` & `aiostream-0.5.2/aiostream/stream/advanced.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/aggregate.py` & `aiostream-0.5.2/aiostream/stream/aggregate.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/combine.py` & `aiostream-0.5.2/aiostream/stream/combine.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/create.py` & `aiostream-0.5.2/aiostream/stream/create.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/misc.py` & `aiostream-0.5.2/aiostream/stream/misc.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/select.py` & `aiostream-0.5.2/aiostream/stream/select.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/time.py` & `aiostream-0.5.2/aiostream/stream/time.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/stream/transform.py` & `aiostream-0.5.2/aiostream/stream/transform.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream/test_utils.py` & `aiostream-0.5.2/aiostream/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/aiostream.egg-info/PKG-INFO` & `aiostream-0.5.2/aiostream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiostream
-Version: 0.5.1
+Version: 0.5.2
 Summary: Generator-based operators for asynchronous iteration
 Home-page: https://github.com/vxgmichel/aiostream
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Description: aiostream
         =========
```

### Comparing `aiostream-0.5.1/aiostream.egg-info/SOURCES.txt` & `aiostream-0.5.2/aiostream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiostream-0.5.1/setup.py` & `aiostream-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 UPLOAD = "upload_sphinx" in sys.argv
 
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="aiostream",
-    version="0.5.1",
+    version="0.5.2",
     packages=["aiostream", "aiostream.stream"],
     python_requires=">=3.8",
     install_requires=["typing-extensions"],
     setup_requires=["pytest-runner" if TESTING else ""],
     tests_require=["pytest", "pytest-asyncio", "pytest-cov"],
     package_data={
         "aiostream": ["py.typed"],
```

