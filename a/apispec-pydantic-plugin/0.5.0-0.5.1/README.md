# Comparing `tmp/apispec_pydantic_plugin-0.5.0.tar.gz` & `tmp/apispec_pydantic_plugin-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apispec_pydantic_plugin-0.5.0.tar", max compression
+gzip compressed data, was "apispec_pydantic_plugin-0.5.1.tar", max compression
```

## Comparing `apispec_pydantic_plugin-0.5.0.tar` & `apispec_pydantic_plugin-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      354 2023-08-15 22:11:04.911004 apispec_pydantic_plugin-0.5.0/README.md
--rw-r--r--   0        0        0     2527 2023-12-07 14:29:42.008510 apispec_pydantic_plugin-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      662 2023-09-08 17:11:52.522630 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/__init__.py
--rw-r--r--   0        0        0       29 2023-09-25 12:57:59.691295 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/constants.py
--rw-r--r--   0        0        0      310 2023-08-15 22:11:04.912822 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/errors.py
--rw-r--r--   0        0        0      582 2023-12-07 14:29:42.009637 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/models.py
--rw-r--r--   0        0        0        0 2023-08-15 22:11:04.913622 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/py.typed
--rw-r--r--   0        0        0     2788 2023-12-07 13:14:34.026812 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/pydantic_plugin.py
--rw-r--r--   0        0        0      926 2023-12-07 14:29:42.010748 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/registry.py
--rw-r--r--   0        0        0     9552 2023-12-07 13:14:34.028356 apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/resolver.py
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 apispec_pydantic_plugin-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-08-15 22:11:04.911004 apispec_pydantic_plugin-0.5.1/README.md
+-rw-r--r--   0        0        0     2426 2024-03-20 20:19:17.722906 apispec_pydantic_plugin-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      672 2024-03-20 20:19:17.723550 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/__init__.py
+-rw-r--r--   0        0        0       29 2023-09-25 12:57:59.691295 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/constants.py
+-rw-r--r--   0        0        0      315 2024-03-20 20:19:17.724169 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/errors.py
+-rw-r--r--   0        0        0      582 2023-12-07 14:29:42.009637 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/models.py
+-rw-r--r--   0        0        0        0 2023-08-15 22:11:04.913622 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/py.typed
+-rw-r--r--   0        0        0     2852 2024-03-20 20:19:17.724661 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/pydantic_plugin.py
+-rw-r--r--   0        0        0      926 2023-12-07 14:29:42.010748 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/registry.py
+-rw-r--r--   0        0        0     9552 2023-12-18 14:16:01.607184 apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/resolver.py
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 apispec_pydantic_plugin-0.5.1/PKG-INFO
```

### Comparing `apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/__init__.py` & `apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from apispec_pydantic_plugin.errors import (
     ApispecPydanticPluginError,
     ApiSpecPydanticPluginKeyError,
     ApiSpecPydanticPluginValueError,
     ModelNotFoundError,
-    ResolverNotFound,
+    ResolverNotFoundError,
 )
 from apispec_pydantic_plugin.models import ApiBaseModel, ApiRootModel
 from apispec_pydantic_plugin.pydantic_plugin import PydanticPlugin
 from apispec_pydantic_plugin.registry import Registry
 
 # isort: unique-list
 __all__ = [
@@ -15,9 +15,9 @@
     "ApiRootModel",
     "ApiSpecPydanticPluginKeyError",
     "ApiSpecPydanticPluginValueError",
     "ApispecPydanticPluginError",
     "ModelNotFoundError",
     "PydanticPlugin",
     "Registry",
-    "ResolverNotFound",
+    "ResolverNotFoundError",
 ]
```

### Comparing `apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/models.py` & `apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/models.py`

 * *Files identical despite different names*

### Comparing `apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/pydantic_plugin.py` & `apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/pydantic_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from contextlib import suppress
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from apispec import APISpec, BasePlugin
 from apispec.exceptions import DuplicateComponentNameError
 from packaging.version import Version
 
-from apispec_pydantic_plugin.errors import ResolverNotFound
-from apispec_pydantic_plugin.models import BaseModelAlias
+from apispec_pydantic_plugin.errors import ResolverNotFoundError
 from apispec_pydantic_plugin.resolver import SchemaResolver
 
+if TYPE_CHECKING:
+    from apispec_pydantic_plugin.models import BaseModelAlias
+
 
 class PydanticPlugin(BasePlugin):
     """APISpec plugin for translating pydantic models to OpenAPI/JSONSchema format."""
 
     spec: APISpec | None
     openapi_version: Version | None
     resolver: SchemaResolver | None
@@ -44,15 +46,15 @@
             name: The identifier which a schema can be referenced.
             definition: Schema definition
             kwargs: All additional keyword arguments sent to `APISpec.schema()`
         """
         model: BaseModelAlias | None = kwargs.pop("model", None)
         if model:
             schema = model.model_json_schema(
-                ref_template="#/components/schemas/{model}"
+                ref_template="#/components/schemas/{model}"  # noqa: RUF027
             )
 
             # definitions is for Pydantic v1
             # $defs is for Pydantic v2
             # I kept both because this used to work, but I don't remember if it was
             # on an earlier version of v2 or the last version of 1. It shouldn't harm
             # anything though other than a slight performance hit for the looping
@@ -72,9 +74,9 @@
     def operation_helper(
         self,
         path: str | None = None,  # noqa: ARG002
         operations: dict[str, Any] | None = None,
         **kwargs: Any,
     ) -> None:
         if self.resolver is None:
-            raise ResolverNotFound("SchemaResolver was not initialized")
+            raise ResolverNotFoundError("SchemaResolver was not initialized")
         self.resolver.resolve_operations(operations=operations, kwargs=kwargs)
```

### Comparing `apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/registry.py` & `apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/registry.py`

 * *Files identical despite different names*

### Comparing `apispec_pydantic_plugin-0.5.0/src/apispec_pydantic_plugin/resolver.py` & `apispec_pydantic_plugin-0.5.1/src/apispec_pydantic_plugin/resolver.py`

 * *Files identical despite different names*

### Comparing `apispec_pydantic_plugin-0.5.0/PKG-INFO` & `apispec_pydantic_plugin-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apispec-pydantic-plugin
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: Kevin Kirsche
 Author-email: kevin.kirsche@one.verizon.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

