# Comparing `tmp/voluptuous-openapi-0.0.1.tar.gz` & `tmp/voluptuous_openapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voluptuous-openapi-0.0.1.tar", last modified: Tue Apr  9 22:05:47 2024, max compression
+gzip compressed data, was "voluptuous_openapi-0.0.2.tar", last modified: Fri May 10 13:12:46 2024, max compression
```

## Comparing `voluptuous-openapi-0.0.1.tar` & `voluptuous_openapi-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:05:47.976345 voluptuous-openapi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-09 22:05:38.000000 voluptuous-openapi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 22:05:38.000000 voluptuous-openapi-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 22:05:47.976345 voluptuous-openapi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-09 22:05:38.000000 voluptuous-openapi-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 22:05:47.976345 voluptuous-openapi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-09 22:05:38.000000 voluptuous-openapi-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:05:47.976345 voluptuous-openapi-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-09 22:05:38.000000 voluptuous-openapi-0.0.1/tests/test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:05:47.976345 voluptuous-openapi-0.0.1/voluptuous_openapi/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-09 22:05:38.000000 voluptuous-openapi-0.0.1/voluptuous_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:05:47.976345 voluptuous-openapi-0.0.1/voluptuous_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 22:05:47.000000 voluptuous-openapi-0.0.1/voluptuous_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 22:05:47.000000 voluptuous-openapi-0.0.1/voluptuous_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:05:47.000000 voluptuous-openapi-0.0.1/voluptuous_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 22:05:47.000000 voluptuous-openapi-0.0.1/voluptuous_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 22:05:47.000000 voluptuous-openapi-0.0.1/voluptuous_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:05:47.000000 voluptuous-openapi-0.0.1/voluptuous_openapi.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/voluptuous_openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/voluptuous_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/zip-safe
```

### Comparing `voluptuous-openapi-0.0.1/LICENSE` & `voluptuous_openapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voluptuous-openapi-0.0.1/README.md` & `voluptuous_openapi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `voluptuous-openapi-0.0.1/voluptuous_openapi/__init__.py` & `voluptuous_openapi-0.0.2/voluptuous_openapi/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Module to convert voluptuous schemas to dictionaries."""
 
 from collections.abc import Callable, Mapping, Sequence
 from enum import Enum
-from typing import Any
+from typing import Any, TypeVar, Union, get_args, get_origin, get_type_hints
+from types import NoneType, UnionType
+from inspect import signature
 
 import voluptuous as vol
 
 
 TYPES_MAP = {
     int: "integer",
     str: "string",
@@ -16,25 +18,41 @@
 
 UNSUPPORTED = object()
 
 
 def convert(schema: Any, *, custom_serializer: Callable | None = None) -> dict:
     """Convert a voluptuous schema to a OpenAPI Schema object."""
     # pylint: disable=too-many-return-statements,too-many-branches
+
+    def ensure_default(value: dict[str:Any]):
+        """Make sure that type is set."""
+        if all(
+            x not in value for x in ("type", "enum", "anyOf", "oneOf", "allOf", "not")
+        ):
+            value["type"] = "string"  # Type not determined, using default
+        return value
+
     additional_properties = None
     if isinstance(schema, vol.Schema):
         if schema.extra == vol.ALLOW_EXTRA:
             additional_properties = True
         schema = schema.schema
 
     if custom_serializer:
         val = custom_serializer(schema)
         if val is not UNSUPPORTED:
             return val
 
+    if isinstance(schema, vol.Object):
+        schema = schema.schema
+        if custom_serializer:
+            val = custom_serializer(schema)
+            if val is not UNSUPPORTED:
+                return val
+
     if isinstance(schema, Mapping):
         properties = {}
         required = []
 
         # Unfold vol.Any in keys
         if vol.Any in [type(k) for k in schema.keys()]:
             pschema = {}
@@ -63,14 +81,15 @@
             if description:
                 pval["description"] = key.description
 
             if isinstance(key, (vol.Required, vol.Optional)):
                 if key.default is not vol.UNDEFINED:
                     pval["default"] = key.default()
 
+            pval = ensure_default(pval)
             pkey = str(pkey)
             properties[pkey] = pval
 
             if isinstance(key, vol.Required):
                 required.append(pkey)
 
         val = {"type": "object", "properties": properties, "required": required}
@@ -90,15 +109,15 @@
                 # Some of the keys are intersecting - fallback to allOf
                 fallback = True
             allOf.append(v)
             if not fallback:
                 val.update(v)
         if fallback:
             return {"allOf": allOf}
-        return val
+        return ensure_default(val)
 
     if isinstance(schema, (vol.Clamp, vol.Range)):
         val = {}
         if schema.min is not None:
             if isinstance(schema, vol.Clamp) or schema.min_included:
                 val["minimum"] = schema.min
             else:
@@ -139,46 +158,93 @@
 
     if schema in (vol.Email, vol.Url, vol.FqdnUrl):
         return {
             "format": schema.__name__.lower(),
         }
 
     if isinstance(schema, vol.Any):
-        # vol.Maybe
-        if len(schema.validators) == 2 and schema.validators[0] is None:
-            result = convert(schema.validators[1], custom_serializer=custom_serializer)
+        schema = schema.validators
+        if None in schema or NoneType in schema:
+            schema = [val for val in schema if val is not None and val is not NoneType]
+            nullable = True
+        else:
+            nullable = False
+        if len(schema) == 1:
+            result = convert(schema[0], custom_serializer=custom_serializer)
+        else:
+            result = {
+                "anyOf": [
+                    convert(val, custom_serializer=custom_serializer) for val in schema
+                ]
+            }
+        if nullable:
             result["nullable"] = True
-            return result
-
-        return {
-            "anyOf": [
-                convert(val, custom_serializer=custom_serializer)
-                for val in schema.validators
-            ]
-        }
+        return result
 
     if isinstance(schema, vol.Coerce):
         schema = schema.type
 
     if isinstance(schema, (str, int, float, bool)) or schema is None:
         return {"enum": [schema]}
 
     if isinstance(schema, Sequence):
         if len(schema) == 1:
             return {
                 "type": "array",
-                "items": convert(schema[0], custom_serializer=custom_serializer),
+                "items": ensure_default(
+                    convert(schema[0], custom_serializer=custom_serializer)
+                ),
             }
         return {
             "type": "array",
             "items": [
-                convert(s, custom_serializer=custom_serializer) for s in schema.items()
+                ensure_default(convert(s, custom_serializer=custom_serializer))
+                for s in schema.items()
             ],
         }
 
     if schema in TYPES_MAP:
         return {"type": TYPES_MAP[schema]}
 
-    if isinstance(schema, type) and issubclass(schema, Enum):
-        return {"enum": [item.value for item in schema]}
+    if schema is list or schema is set:
+        return {"type": "array", "items": ensure_default({})}
+
+    if schema is dict:
+        return {"type": "object", "additionalProperties": True}
+
+    if isinstance(schema, type):
+        if issubclass(schema, Enum):
+            return {"enum": [item.value for item in schema]}
+        elif schema is NoneType:
+            return {"enum": [None]}
+
+    if callable(schema):
+        schema = get_type_hints(schema).get(
+            list(signature(schema).parameters.keys())[0], Any
+        )
+        if schema is Any or isinstance(schema, TypeVar):
+            return {}
+        if isinstance(schema, UnionType) or get_origin(schema) is Union:
+            schema = [t for t in get_args(schema) if not isinstance(t, TypeVar)]
+            if len(schema) > 1:
+                schema = vol.Any(*schema)
+            elif len(schema) == 1 and schema[0] is not NoneType:
+                schema = schema[0]
+            else:
+                return {}
+        if get_origin(schema) is dict:
+            schema = get_args(schema)[1]
+            if schema is Any or isinstance(schema, TypeVar):
+                schema = dict
+            else:
+                return {
+                    "type": "object",
+                    "additionalProperties": convert(
+                        schema, custom_serializer=custom_serializer
+                    ),
+                }
+        if get_origin(schema) is list or get_origin(schema) is set:
+            schema = [get_args(schema)[0]]
+
+        return convert(schema, custom_serializer=custom_serializer)
 
     raise ValueError("Unable to convert schema: {}".format(schema))
```

