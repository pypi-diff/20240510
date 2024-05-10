# Comparing `tmp/sgn-0.0.1.tar.gz` & `tmp/sgn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgn-0.0.1.tar", last modified: Wed May  8 09:52:53 2024, max compression
+gzip compressed data, was "sgn-0.0.2.tar", last modified: Fri May 10 10:57:55 2024, max compression
```

## Comparing `sgn-0.0.1.tar` & `sgn-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.074600 sgn-0.0.1/
--rw-r--r--   0 channa     (502) staff       (20)       12 2024-05-07 19:42:52.000000 sgn-0.0.1/.gitignore
--rw-r--r--   0 channa     (502) staff       (20)    16756 2024-05-08 09:20:34.000000 sgn-0.0.1/LICENSE
--rw-r--r--   0 channa     (502) staff       (20)     2188 2024-05-08 09:52:53.074461 sgn-0.0.1/PKG-INFO
--rw-r--r--   0 channa     (502) staff       (20)     1558 2024-05-07 19:42:52.000000 sgn-0.0.1/README.md
--rw-r--r--   0 channa     (502) staff       (20)      694 2024-05-08 09:52:27.000000 sgn-0.0.1/pyproject.toml
--rw-r--r--   0 channa     (502) staff       (20)      865 2024-05-08 09:52:53.075557 sgn-0.0.1/setup.cfg
--rw-r--r--   0 channa     (502) staff       (20)       93 2024-05-08 09:33:19.000000 sgn-0.0.1/setup.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.067587 sgn-0.0.1/src/
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.070440 sgn-0.0.1/src/sgn/
--rw-r--r--   0 channa     (502) staff       (20)        0 2024-05-07 19:42:52.000000 sgn-0.0.1/src/sgn/__init__.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.071816 sgn-0.0.1/src/sgn/apps/
--rw-r--r--   0 channa     (502) staff       (20)     3719 2024-05-07 19:42:52.000000 sgn-0.0.1/src/sgn/apps/__init__.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.072094 sgn-0.0.1/src/sgn/base/
--rw-r--r--   0 channa     (502) staff       (20)     6815 2024-05-07 19:42:52.000000 sgn-0.0.1/src/sgn/base/__init__.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.072404 sgn-0.0.1/src/sgn/sinks/
--rw-r--r--   0 channa     (502) staff       (20)     1088 2024-05-07 19:42:52.000000 sgn-0.0.1/src/sgn/sinks/__init__.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.072717 sgn-0.0.1/src/sgn/sources/
--rw-r--r--   0 channa     (502) staff       (20)     1027 2024-05-07 19:42:52.000000 sgn-0.0.1/src/sgn/sources/__init__.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.073152 sgn-0.0.1/src/sgn/transforms/
--rw-r--r--   0 channa     (502) staff       (20)     1332 2024-05-07 19:42:52.000000 sgn-0.0.1/src/sgn/transforms/__init__.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-08 09:52:53.073835 sgn-0.0.1/src/sgn.egg-info/
--rw-r--r--   0 channa     (502) staff       (20)     2188 2024-05-08 09:52:53.000000 sgn-0.0.1/src/sgn.egg-info/PKG-INFO
--rw-r--r--   0 channa     (502) staff       (20)      346 2024-05-08 09:52:53.000000 sgn-0.0.1/src/sgn.egg-info/SOURCES.txt
--rw-r--r--   0 channa     (502) staff       (20)        1 2024-05-08 09:52:53.000000 sgn-0.0.1/src/sgn.egg-info/dependency_links.txt
--rw-r--r--   0 channa     (502) staff       (20)        4 2024-05-08 09:52:53.000000 sgn-0.0.1/src/sgn.egg-info/top_level.txt
--rwxr-xr-x   0 channa     (502) staff       (20)     2402 2024-05-08 09:43:09.000000 sgn-0.0.1/test
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.125065 sgn-0.0.2/
+-rw-r--r--   0 channa     (502) staff       (20)       12 2024-05-07 19:42:52.000000 sgn-0.0.2/.gitignore
+-rw-r--r--   0 channa     (502) staff       (20)    16756 2024-05-08 09:20:34.000000 sgn-0.0.2/LICENSE
+-rw-r--r--   0 channa     (502) staff       (20)     2914 2024-05-10 10:57:55.124906 sgn-0.0.2/PKG-INFO
+-rw-r--r--   0 channa     (502) staff       (20)     2284 2024-05-08 12:49:08.000000 sgn-0.0.2/README.md
+-rw-r--r--   0 channa     (502) staff       (20)      694 2024-05-10 10:57:37.000000 sgn-0.0.2/pyproject.toml
+-rw-r--r--   0 channa     (502) staff       (20)      865 2024-05-10 10:57:55.125829 sgn-0.0.2/setup.cfg
+-rw-r--r--   0 channa     (502) staff       (20)       93 2024-05-08 09:33:19.000000 sgn-0.0.2/setup.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.114512 sgn-0.0.2/src/
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.119167 sgn-0.0.2/src/sgn/
+-rw-r--r--   0 channa     (502) staff       (20)        0 2024-05-07 19:42:52.000000 sgn-0.0.2/src/sgn/__init__.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.121224 sgn-0.0.2/src/sgn/apps/
+-rw-r--r--   0 channa     (502) staff       (20)     2646 2024-05-10 10:04:39.000000 sgn-0.0.2/src/sgn/apps/__init__.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.121627 sgn-0.0.2/src/sgn/base/
+-rw-r--r--   0 channa     (502) staff       (20)     8653 2024-05-10 10:55:59.000000 sgn-0.0.2/src/sgn/base/__init__.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.122055 sgn-0.0.2/src/sgn/sinks/
+-rw-r--r--   0 channa     (502) staff       (20)      856 2024-05-10 10:49:36.000000 sgn-0.0.2/src/sgn/sinks/__init__.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.122512 sgn-0.0.2/src/sgn/sources/
+-rw-r--r--   0 channa     (502) staff       (20)      770 2024-05-10 10:51:06.000000 sgn-0.0.2/src/sgn/sources/__init__.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.123003 sgn-0.0.2/src/sgn/transforms/
+-rw-r--r--   0 channa     (502) staff       (20)      882 2024-05-10 10:50:29.000000 sgn-0.0.2/src/sgn/transforms/__init__.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.124287 sgn-0.0.2/src/sgn.egg-info/
+-rw-r--r--   0 channa     (502) staff       (20)     2914 2024-05-10 10:57:55.000000 sgn-0.0.2/src/sgn.egg-info/PKG-INFO
+-rw-r--r--   0 channa     (502) staff       (20)      361 2024-05-10 10:57:55.000000 sgn-0.0.2/src/sgn.egg-info/SOURCES.txt
+-rw-r--r--   0 channa     (502) staff       (20)        1 2024-05-10 10:57:55.000000 sgn-0.0.2/src/sgn.egg-info/dependency_links.txt
+-rw-r--r--   0 channa     (502) staff       (20)        4 2024-05-10 10:57:55.000000 sgn-0.0.2/src/sgn.egg-info/top_level.txt
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-05-10 10:57:55.123635 sgn-0.0.2/tests/
+-rwxr-xr-x   0 channa     (502) staff       (20)     3884 2024-05-10 10:48:36.000000 sgn-0.0.2/tests/test_graph.py
```

### Comparing `sgn-0.0.1/LICENSE` & `sgn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sgn-0.0.1/pyproject.toml` & `sgn-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sgn"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Chad Hanna", email="crh184@psu.edu" },
 ]
 description = "Streaming Graph Navigator. A framework to help navigate buffers through a graph. The buffers must flow."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sgn-0.0.1/setup.cfg` & `sgn-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sgn-0.0.1/src/sgn/base/__init__.py` & `sgn-0.0.2/src/sgn/base/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,202 +1,247 @@
-from functools import wraps
-import inspect
+from dataclasses import dataclass
+from typing import Callable
+import random
 
-# These could be moved out someday to other modules
-
-# From https://stackoverflow.com/questions/1389180/automatically-initialize-instance-variables
-def initializer(func):
-    """
-    Automatically assigns the parameters.
-
-    >>> class process:
-    ...     @initializer
-    ...     def __init__(self, cmd, reachable=False, user='root'):
-    ...         pass
-    >>> p = process('halt', True)
-    >>> p.cmd, p.reachable, p.user
-    ('halt', True, 'root')
-    """
-    names, varargs, keywords, defaults = inspect.getargspec(func)
-
-    @wraps(func)
-    def wrapper(self, *args, **kargs):
-        for name, arg in list(zip(names[1:], args)) + list(kargs.items()):
-            setattr(self, name, arg)
-
-        for name, default in zip(reversed(names), reversed(defaults or [])):
-            if not hasattr(self, name):
-                setattr(self, name, default)
-
-        func(self, *args, **kargs)
-
-    return wrapper
-
-class Buffer(object):
+@dataclass
+class Buffer:
     """
     A generic class to hold the basic unit of data that flows through a graph
-    """
-    @initializer
-    def __init__(self, **kwargs):
-        self.kwargs = kwargs
-    def __repr__(self):
-        return str(self.kwargs)
 
+    Parameters
+    ----------
+    EOS : bool, optional
+        Whether this buffer indicates end of stream (EOS), default is false
+    is_gap : bool, optional
+        Whether this buffer is marked as a gap, default is False.
+    metadata : dict, optional
+        Metadata associated with this buffer.
+    """
+    EOS: bool = False
+    is_gap: bool = False
+    metadata: dict = None
+
+@dataclass
 class Base(object):
     """
     A generic class from which all classes that participate in an execution
     graph should be derived.  It enforces a unique name and hashes based on that
     name. 
-    """
-    registry = set()
 
-    @initializer
-    def __init__(self, **kwargs):
-        """
-        name must be in kwargs and must not have been used by any derived class instance
-        """
-        assert "name" in kwargs
-        assert kwargs["name"] not in Base.registry
-        Base.registry.add(kwargs["name"])
+    Parameters
+    ----------
+    name : str, optional
+        The unique name for this object, default is a random 64 bit integer
+    """
+    # according to the docs, this won't be initialized as an instance variable
+    # since it is missing the type hint. We want this to be a class variable.
+    registry = {}
+    name: str = str(random.getrandbits(64))
+
+    def __post_init__(self):
+        assert self.name not in Base.registry
+        Base.registry[self.name] = self
 
     def __hash__(self):
         return hash(self.name)
 
     def __eq__(self, other):
         return hash(self) == hash(other)
 
     def __repr__(self):
         return self.name
 
+@dataclass(repr=False)
+class Element(Base):
+    """
+    A basic container to hold source and sink pads. The assmption is that this
+    will be a base class for code that actually does something. It should never be
+    subclassed directly, instead subclass SourceElement, SinkElement or
+    TransformElement
+
+    Parameters
+    ----------
+    graph : dict, optional
+        The internal relationships between source and sink pads. This must be initialized as None and defaults to None.
+    source_pads: list, optional
+        The list of SourcePad objects. This must be given for SourceElements or TransformElements, default is None
+    sink_pads: list, optional
+        The list of SinkPad objects. This must be given for SinkElements or TransformElements, default is None
+    """
+    graph: dict = None
+    source_pads: list = None
+    sink_pads: list = None
+
+    def __post_init__(self):
+        assert self.graph is None
+        if self.graph is None:
+            self.graph = {}
+
+    @property
+    def source_pad_dict(self):
+        return {p.name:p for p in self.source_pads}
+
+    @property
+    def sink_pad_dict(self):
+        return {p.name:p for p in self.sink_pads}
+
+@dataclass(eq=False, repr=False)
 class Pad(Base):
     """
-    Pads are 1:1 with graph nodes but src and sink pads must be grouped into
-    elements in order to exchange data from sink->src.  src->sink exchanges happen
+    Pads are 1:1 with graph nodes but source and sink pads must be grouped into
+    elements in order to exchange data from sink->source.  source->sink exchanges happen
     between elements.
-    """
-    @initializer
-    def __init__(self, **kwargs):
-        """
-	A pad must belong to an element and that element must be provided as a
-        keyword argument called "element".  The element must also provide a call
-        function that will be executed when the pad is called
-        """
-        assert "element" in kwargs and "call" in kwargs
-        super(Pad, self).__init__(**kwargs)
 
+    A pad must belong to an element and that element must be provided as a
+    keyword argument called "element".  The element must also provide a call
+    function that will be executed when the pad is called. The call function must
+    take a pad as an argument, e.g., def call(pad):
+
+    Developers should not subclass or use Pad directly. Instead use SourcePad or SinkPad.
+
+    Parameters
+    ----------
+    element : Element, optional
+        The Element instance associated with this pad, default None
+    call : Callable, optional
+        The function that will be called during graph execution for this pad, default None
 
-class SrcPad(Pad):
     """
-    A pad that provides data through a buffer when asked
+    element: Element = None
+    call: Callable = None
+
+@dataclass(eq=False, repr=False)
+class SourcePad(Pad):
     """
-    @initializer
-    def __init__(self, **kwargs):
-        super(SrcPad, self).__init__(**kwargs)
+    A pad that provides data through a buffer when called. 
+
+    Parameters
+    ----------
+    outbuf : Buffer, optional
+        This attribute is populated when the pad is called defined by the output of the Pad.call function.
+    """
+    outbuf: Buffer = None
 
     async def __call__(self):
         """
 	When called, a source pad receives a buffer from the element that the
         pad belongs to.
         """
         self.outbuf = self.call(pad = self)
 
 
-
+@dataclass(eq=False, repr=False)
 class SinkPad(Pad):
     """
     A pad that receives data from a buffer when asked.  When linked, it returns
     a dictionary suitable for building a graph in graphlib.
+
+    Parameters
+    ----------
+    other: Pad, optional
+        This holds the source pad that is linked to this sink pad, default None
+    inbuf: Buffer, optional
+        This holds the buffer provided by the linked source pad. Generally it gets set when this SinkPad is called, default None
     """
-    @initializer
-    def __init__(self, **kwargs):
-        super(SinkPad, self).__init__(**kwargs)
+    other: Pad = None
+    inbuf: Buffer = None
+
     def link(self, other):
         """
 	Only sink pads can be linked. A sink pad can be linked to only one
-	source pad, but multiple sink pads may link to the same src pad.
+	source pad, but multiple sink pads may link to the same source pad.
         Returns a dictionary of dependencies suitable for adding to a graphlib graph.
         """
         self.other = other
+        assert isinstance(self.other, SourcePad)
         return {self: set((other,))}
+
     async def __call__(self):
         """
 	When called, a sink pad gets the buffer from the linked source pad and
         then calls the element's provided call function.  NOTE: pads must be called in
         the correct order such that the upstream sources have new information by the
         time call is invoked.  This should be done within a directed acyclic graph such
         as those provided by the apps.Pipeline class.
         """
         self.inbuf = self.other.outbuf
         self.call(self, self.inbuf)
 
-class Element(Base):
+
+@dataclass(repr=False)
+class SourceElement(Element):
     """
-    A basic container to hold src and sink pads. The assmption is that this
-    will be a base class for code that actually does something. It should never be
-    subclassed directly, instead subclass SrcElement, SinkElement or
-    TransformElement
+    Initialize with a list of source pads. Every source pad is added to the graph with no dependencies.
+
+    Parameters
+    ----------
+    source_pad_names : list, optional
+        Set the list of source pad names. These need to be unique for an element but not for an application. The resulting full names will be made with "<self.name>:src:<source_pad_name>"
     """
 
-    @initializer
-    def __init__(self, **kwargs):
-        super(Element, self).__init__(**kwargs)
-        self.graph = {}
-    def link(self, other, **kwargs):
-        """
-        A element links to another element only on its sink pads.  This function offers a few rules:
-
-        1) If "other" is a source pad, it will be used
-        2) otherwise, if "other" is an element it **must** have only one source pad 
-        3) you must specify a sink pad name if this element instance has more than one sink pad.
-
-	it updates the elements internal dictionary which is suitable for being
-        added to a graphlib graph.
-        """
-        sink_pads_by_name = {p.name:p for p in self.sink_pads}
-        if isinstance(other, Pad):
-            src_pad = other
-        else:
-            assert len(other.src_pads) == 1
-            src_pad = other.src_pads[0]
-        if "sink_pad_name" not in kwargs:
-            assert len(self.sink_pads) == 1
-            sink_pad = self.sink_pads[0]
-        else:
-            sink_pad = sink_pads_by_name[kwargs["sink_pad_name"]]
-        self.graph.update(sink_pad.link(src_pad))
-
-class SrcElement(Element):
-    @initializer
-    def __init__(self, **kwargs):
-        """
-        "src_pads" (iterable) must be in kwargs.  Every source pad is added to the graph with no dependencies.
-        """
-        assert "src_pads" in kwargs
-        super(SrcElement, self).__init__(**kwargs)
-        self.graph.update({s: set() for s in self.src_pads})
-        self.src_pad_dict = {p.name:p for p in self.src_pads}
+    source_pad_names: list = None
 
-class TransformElement(Element):
-    @initializer
-    def __init__(self, **kwargs):
-        """
-	Both "src_pads" and "sink_pads" must be in kwargs.  All sink pads
-        depend on all source pads in a transform element. If you don't want that to be
-        true, write more than one transform element.
-        """
-        assert "src_pads" in kwargs and "sink_pads" in kwargs
-        super(TransformElement, self).__init__(**kwargs)
-        self.graph.update({s: set(self.sink_pads) for s in self.src_pads})
-        self.src_pad_dict = {p.name:p for p in self.src_pads}
-        self.sink_pad_dict = {p.name:p for p in self.sink_pads}
-        
+    def __post_init__(self):
+        self.source_pads = [SourcePad(name = "%s:src:%s" % (self.name, n), element=self, call = self.new_buffer) for n in self.source_pad_names]
+        super().__post_init__()
+        assert self.source_pads and not self.sink_pads
+        self.graph.update({s: set() for s in self.source_pads})
 
-class SinkElement(Element):
-    @initializer
-    def __init__(self, **kwargs):
+    def new_buffer(self, pad):
         """
-        "sink_pads" must be in kwargs
+        New buffers are created on "pad". Must be provided by subclass
         """
-        assert "sink_pads" in kwargs
-        super(SinkElement, self).__init__(**kwargs)
-        self.graph = {}
-        self.sink_pad_dict = {p.name:p for p in self.sink_pads}
+        raise NotImplementedError
+
+@dataclass(repr=False)
+class TransformElement(Element):
+    """
+    Both "source_pads" and "sink_pads" must exist.  All sink pads
+    depend on all source pads in a transform element. If you don't want that to be
+    true, write more than one transform element.
+
+    Parameters
+    ----------
+    source_pad_names : list, optional
+        Set the list of source pad names. These need to be unique for an element but not for an application. The resulting full names will be made with "<self.name>:src:<source_pad_name>"
+    sink_pad_names : list, optional
+        Set the list of sink pad names. These need to be unique for an element but not for an application. The resulting full names will be made with "<self.name>:sink:<sink_pad_name>"
+    """
+
+    source_pad_names: list = None
+    sink_pad_names: list = None
+
+    def __post_init__(self):
+        self.source_pads = [SourcePad(name = "%s:src:%s" % (self.name, n), element = self, call = self.transform_buffer) for n in self.source_pad_names]
+        self.sink_pads = [SinkPad(name = "%s:sink:%s" % (self.name, n), element = self, call = self.get_buffer) for n in self.sink_pad_names]
+        super().__post_init__()
+        assert self.source_pads and self.sink_pads
+        self.graph.update({s: set(self.sink_pads) for s in self.source_pads})
+
+    def get_buffer(self, pad, buf):
+        raise NotImplementedError
+
+    def transform_buffer(self, pad):
+        raise NotImplementedError
+       
+
+@dataclass()
+class SinkElement(Element):
+    """
+    "sink_pads" must exist but not "source_pads"
+
+    Parameters
+    ----------
+    sink_pad_names : list, optional
+        Set the list of sink pad names. These need to be unique for an element but not for an application. The resulting full names will be made with "<self.name>:sink:<sink_pad_name>"
+    """
+
+    sink_pad_names: list = None
+
+    def __post_init__(self):
+        self.sink_pads = [SinkPad(name = "%s:sink:%s" % (self.name, n), element=self, call = self.get_buffer) for n in self.sink_pad_names]
+        super().__post_init__()
+        assert self.sink_pads and not self.source_pads
+
+    def get_buffer(self, pad, buf):
+        raise NotImplementedError
+
```

### Comparing `sgn-0.0.1/src/sgn/sinks/__init__.py` & `sgn-0.0.2/src/sgn/sinks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+from dataclasses import dataclass
 from ..base import *
 
-
+@dataclass
 class FakeSink(SinkElement):
-    @initializer
-    def __init__(self, **kwargs):
-        """
-	A fake sink element that has sink pads given by "channels" named
-        "name:channel:sink". "channels" is a required kwarg
-        """
-        kwargs["sink_pads"] = [SinkPad(name = "%s:%s:sink" % (kwargs["name"], channel), element=self, call = self.get_buffer) for channel in kwargs["channels"]]
-        super(FakeSink, self).__init__(**kwargs)
-        self.at_eos = {p:False for p in kwargs["sink_pads"]}
+    """
+    A fake sink element
+    """
+    def __post_init__(self):
+        self.inbuf = None
+        super().__post_init__()
+        self.at_eos = {p:False for p in self.sink_pads}
+
     def get_buffer(self, pad, buf):
         """
 	getting the buffer on the pad just modifies the name to show this final
         graph point and the prints it to prove it all works.
         """
         self.inbuf = buf
         self.at_eos[pad] = self.inbuf.EOS
-        print ("buffer flow: ", "%s -> '%s'" % (self.inbuf.name, pad.name))
+        print ("buffer flow: ", "%s -> '%s'" % (self.inbuf.metadata["name"], pad.name))
     @property
     def EOS(self):
         """
         If buffers on any sink pads are End of Stream (EOS), then mark this whole element as EOS
         """
         return any(self.at_eos.values())
```

### Comparing `sgn-0.0.1/src/sgn/sources/__init__.py` & `sgn-0.0.2/src/sgn/sources/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,22 @@
+from dataclasses import dataclass
 from .. base import *
 
-
-class FakeSrc(SrcElement):
-    @initializer
-    def __init__(self, **kwargs):
-        """
-        A fake source element "channels" are required and will be used to
-        create src pads with the name "name:channel:src". "num_buffers" is required and
-        sets how many buffers will be created before setting "EOS"
-        """
-        kwargs["src_pads"] = [SrcPad(name = "%s:%s:src" % (kwargs["name"], channel), element=self, call = self.new_buffer) for channel in kwargs["channels"]]
-        self.cnt = {p:0 for p in kwargs["src_pads"]}
-        super(FakeSrc, self).__init__(**kwargs)
+@dataclass
+class FakeSrc(SourceElement):
+    """
+    "num_buffers" is required and sets how many buffers will be created before setting "EOS"
+    """
+    num_buffers: int = 0
+    def __post_init__(self):
+        super().__post_init__()
+        self.cnt = {p:0 for p in self.source_pads}
     def new_buffer(self, pad):
         """
         New buffers are created on "pad" with an instance specific count and a
         name derived from the pad name. "EOS" is set if we have surpassed the requested
         number of buffers.
         """
         self.cnt[pad] += 1
-        return Buffer(cnt = self.cnt, name = "'%s'" % pad.name, EOS = self.cnt[pad] > self.num_buffers)
+        return Buffer(metadata = {"cnt":self.cnt, "name":"'%s'" % pad.name}, EOS = self.cnt[pad] > self.num_buffers)
 
 sources_registry = ("FakeSrc",)
```

### Comparing `sgn-0.0.1/src/sgn/transforms/__init__.py` & `sgn-0.0.2/src/sgn/transforms/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+from dataclasses import dataclass
 from .. base import *
 
-
+@dataclass
 class FakeTransform(TransformElement):
-    @initializer
-    def __init__(self, **kwargs):
-        """
-        A fake transform element with sink pads given by "in_channels" and source pads given by "out_channels". Names are "name:inchannel:sink" and "name:outchannel:src".
-        """
-        assert "in_channels" in kwargs and "out_channels" in kwargs
-        kwargs["src_pads"] = [SrcPad(name = "%s:%s:src" % (kwargs["name"], channel), element = self, call = self.transform_buffer) for channel in self.out_channels]
-        kwargs["sink_pads"] = [SinkPad(name = "%s:%s:sink" % (kwargs["name"], channel), element = self, call = self.get_buffer) for channel in self.in_channels]
-        super(FakeTransform, self).__init__(**kwargs)
+    """
+    A fake transform element.
+    """
+
+    def __post_init__(self):
         self.inbuf = {}
+        super().__post_init__()
 
     def get_buffer(self, pad, buf):
         self.inbuf[pad] = buf
 
     def transform_buffer(self, pad):
         """
 	The transform buffer just update the name to show the graph history.
         Useful for proving it works.  "EOS" is set if any input buffers are at EOS.
         """
         EOS = any(b.EOS for b in self.inbuf.values())
-        return Buffer(**{"cnt:%s" % b.name:b.cnt for b in self.inbuf.values()}, name = "%s -> '%s'" % ("+".join(b.name for b in self.inbuf.values()), pad.name), EOS = EOS)
+        metadata = {"cnt:%s" % b.metadata['name']:b.metadata['cnt'] for b in self.inbuf.values()}
+        metadata["name"] = "%s -> '%s'" % ("+".join(b.metadata["name"] for b in self.inbuf.values()), pad.name)
+        return Buffer(metadata = metadata, EOS = EOS)
 
 transforms_registry = ("FakeTransform",)
```

