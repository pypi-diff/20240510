# Comparing `tmp/flexible_dict-2.0.0.tar.gz` & `tmp/flexible_dict-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-2.0.0.tar", last modified: Thu May  9 12:39:05 2024, max compression
+gzip compressed data, was "flexible_dict-2.0.1.tar", last modified: Fri May 10 09:42:00 2024, max compression
```

## Comparing `flexible_dict-2.0.0.tar` & `flexible_dict-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/flexible_dict/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/json_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/flexible_dict/script/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/script/class_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/flexible_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/run_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:42:00.050504 flexible_dict-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-10 09:42:00.050504 flexible_dict-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:42:00.050504 flexible_dict-2.0.1/flexible_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-10 09:41:59.000000 flexible_dict-2.0.1/flexible_dict/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25168 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/json_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:42:00.050504 flexible_dict-2.0.1/flexible_dict/script/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/script/class_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/flexible_dict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:42:00.050504 flexible_dict-2.0.1/flexible_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-10 09:42:00.000000 flexible_dict-2.0.1/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 09:42:00.000000 flexible_dict-2.0.1/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:42:00.000000 flexible_dict-2.0.1/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-10 09:42:00.000000 flexible_dict-2.0.1/flexible_dict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/run_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:42:00.050504 flexible_dict-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 09:41:54.000000 flexible_dict-2.0.1/tox.ini
```

### Comparing `flexible_dict-2.0.0/PKG-INFO` & `flexible_dict-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 2.0.0
+Version: 2.0.1
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-2.0.0/README.md` & `flexible_dict-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.0/flexible_dict/__main__.py` & `flexible_dict-2.0.1/flexible_dict/__main__.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.0/flexible_dict/adapter.py` & `flexible_dict-2.0.1/flexible_dict/adapter.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.0/flexible_dict/json_object.py` & `flexible_dict-2.0.1/flexible_dict/json_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,16 @@
     Optional, Type,
 )
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 import sys
-import re
 import types
 import builtins
-import warnings
 import dataclasses
 from .adapter import (
     _ENCODER_TYPE, _DECODER_TYPE,
     get_encoder_func,
     get_decoder_func,
     AdapterDetector,
 )
@@ -46,47 +44,19 @@
 class _FIELD_BASE:
     def __init__(self, name):
         self.name = name
     def __repr__(self):
         return self.name
 _FIELD_DICTKEY = _FIELD_BASE('_FIELD_DICTKEY')
 _FIELD_CLASSVAR = _FIELD_BASE('_FIELD_CLASSVAR')
-_FIELD_OBJECTVAR = _FIELD_BASE('_FIELD_OBJECTVAR')
-_FIELD_INITVAR = _FIELD_BASE('_FIELD_INITVAR')
 
 # The name of an attribute on the class where we store the Field
 # objects.  Also used to check if a class is a json_object class.
 _FIELDS = '__json_object_fields__'
 
-# The name of the function, that if it exists, is called at the end of
-# __init__.
-_POST_INIT_NAME = '__post_init__'
-
-# String regex that string annotations for ClassVar or InitVar must match.
-# Allows "identifier.identifier[" or "identifier[".
-# https://bugs.python.org/issue33453 for details.
-_MODULE_IDENTIFIER_RE = re.compile(r'^(?:\s*(\w+)\s*\.)?\s*(\w+)')
-
-class ObjectVar:
-    __slots__ = ('type', )
-    def __init__(self, type):
-        self.type = type
-    def __repr__(self):
-        is_type = isinstance(self.type, type)
-        if is_type and sys.version_info >= (3, 9):
-            is_type = not isinstance(self.type, types.GenericAlias)
-        if is_type:
-            type_name = self.type.__name__
-        else:
-            # typing objects, e.g. List[int]
-            type_name = repr(self.type)
-        return f'flexible_dict.ObjectVar[{type_name}]'
-    def __class_getitem__(cls, type):
-        return ObjectVar(type)
-
 @dataclasses.dataclass
 class Field:
     # the key stored in the dict; same as name if set as MISSING
     key: str = MISSING
 
     # access control
     readable: bool = True
@@ -270,15 +240,15 @@
             # Should I check for other field settings? default_factory
             # seems the most serious to check for.  Maybe add others.  For
             # example, how about init=False (or really,
             # init=<not-the-default-init-value>)?  It makes no sense for
             # ClassVar and InitVar to specify init=<anything>.
 
         # For real fields, disallow mutable defaults for known types.
-        if f._field_type in (_FIELD_DICTKEY, _FIELD_OBJECTVAR):
+        if f._field_type is _FIELD_DICTKEY:
             if isinstance(f.getter_default, (list, dict, set)):
                 raise ValueError(f'mutable getter_default {type(f.getter_default)} for field '
                                  f'{f.name} is not allowed: use getter_default_factory0 or getter_default_factory1')
             if isinstance(f.init_default, (list, dict, set)):
                 raise ValueError(f'mutable init_default {type(f.init_default)} for field '
                                  f'{f.name} is not allowed: use init_default_factory')
 
@@ -488,63 +458,62 @@
         _locals.update((f'_key_{f.name}', f.key) for f in fields)
 
         # all args
         args = [self_name, f'*{ds_name}:dict'] + [f'{f.name}:_type_{f.name}=MISSING' for f in fields]
         if kwargs_name:
             args.append(f'**{kwargs_name}')
 
-        # default values
         body_lines = []
-        for f in fields:
-            if not self.is_missing(f.init_default):
-                _locals[f'_default_{f.name}'] = f.init_default
-                body_lines.append(f"{self_name}[_key_{f.name}] = _default_{f.name}")
-            elif not self.is_missing(f.init_default_factory):
-                _locals[f'_default_{f.name}'] = f.init_default_factory
-                body_lines.append(f"{self_name}[_key_{f.name}] = _default_{f.name}()")
 
-        # update by given dicts
+        # update by given dicts, value would be encoded since it's set before walking fields
         body_lines.extend([
             f"for {d_name} in {ds_name}:",
             f" {self_name}.update({d_name})",
         ])
 
-        # update by kwargs
-        if kwargs_name:
-            body_lines.append(f"{self_name}.update({kwargs_name})")
-
-        # update by name
+        # walk fields to update and encode
         for f in fields:
             if f._field_type is _FIELD_DICTKEY:
                 # value stored in dict would be correctly encoded by setting with `.`
                 body_lines.extend([
                     f"if {f.name} is not MISSING:",
                     f" {self_name}.{f.name} = {f.name}",
                     f"elif _key_{f.name} in {self_name}:",
                     f" {self_name}.{f.name} = {self_name}[_key_{f.name}]",
                 ])
+                # set default value
+                if not self.is_missing(f.init_default):
+                    _locals[f'_default_{f.name}'] = f.init_default
+                    body_lines.extend([
+                        f"else:",
+                        f" {self_name}[_key_{f.name}] = _default_{f.name}",
+                    ])
+                elif not self.is_missing(f.init_default_factory):
+                    _locals[f'_default_{f.name}'] = f.init_default_factory
+                    body_lines.extend([
+                        f"else:",
+                        f"{self_name}[_key_{f.name}] = _default_{f.name}()"
+                    ])
             elif f._field_type is _FIELD_CLASSVAR:
                 body_lines.extend([
                     f"if {f.name} is not MISSING:",
                     f" {self_name}.{f.name} = {f.name}",
                 ])
 
+        # update by kwargs, value would not be encoded since it's set after walking fields
+        if kwargs_name:
+            body_lines.append(f"{self_name}.update({kwargs_name})")
+
         return self._create_fn('__init__', args, body_lines, _locals=_locals)
 
     def add_init_func(self):
         """
         add __init__ function
         """
-        # Include InitVars and regular fields (so, not ClassVars).
-        allowed_field_types = (
-            _FIELD_DICTKEY,
-            _FIELD_OBJECTVAR,
-            _FIELD_INITVAR,
-        )
-        fields = [f for f in self.fields.values() if f._field_type in allowed_field_types]
+        fields = [f for f in self.fields.values() if f._field_type is _FIELD_DICTKEY]
         self._set_new_attribute(self.cls, '__init__', self._init_fn(
             fields,
             'self',
             '_',
             '__',
             '___',
         ))
@@ -648,15 +617,15 @@
 
     def __call__(self, cls: type = None) -> Type[dict]:
         if cls is not None:
             self._reset(cls)
         self._process()
         return self.cls
 
-def json_object(_cls=None, processor=JsonObjectClassProcessor, config=None,
+def json_object(_cls=None, processor=JsonObjectClassProcessor, *, config=None,
                 getter_default=None, adapter_detector: AdapterDetector = None,
                 create_init_func=True, create_iter_func=True, iter_func_name='field_items',
                 **kwargs):
     """
     a decorator to mark a class as json format
     """
     if config is None:
```

### Comparing `flexible_dict-2.0.0/flexible_dict/script/class_builder.py` & `flexible_dict-2.0.1/flexible_dict/script/class_builder.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.0/flexible_dict.egg-info/PKG-INFO` & `flexible_dict-2.0.1/flexible_dict.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 2.0.0
+Version: 2.0.1
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-2.0.0/pyproject.toml` & `flexible_dict-2.0.1/pyproject.toml`

 * *Files identical despite different names*

