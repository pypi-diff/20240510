# Comparing `tmp/pydid-0.4.3.tar.gz` & `tmp/pydid-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydid-0.4.3.tar", max compression
+gzip compressed data, was "pydid-0.5.0.tar", max compression
```

## Comparing `pydid-0.4.3.tar` & `pydid-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-01-05 18:08:04.705254 pydid-0.4.3/LICENSE
--rw-r--r--   0        0        0      848 2024-01-05 18:08:04.705254 pydid-0.4.3/README.md
--rw-r--r--   0        0        0     1713 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/__init__.py
--rw-r--r--   0        0        0      318 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/common.py
--rw-r--r--   0        0        0     2294 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/did.py
--rw-r--r--   0        0        0     2773 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/did_url.py
--rw-r--r--   0        0        0      582 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/doc/__init__.py
--rw-r--r--   0        0        0     8609 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/doc/builder.py
--rw-r--r--   0        0        0     2524 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/doc/corrections.py
--rw-r--r--   0        0        0     7863 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/doc/doc.py
--rw-r--r--   0        0        0     1807 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/doc/generic.py
--rw-r--r--   0        0        0     4682 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/resource.py
--rw-r--r--   0        0        0     1604 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/service.py
--rw-r--r--   0        0        0     1002 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/validation.py
--rw-r--r--   0        0        0     8659 2024-01-05 18:08:04.705254 pydid-0.4.3/pydid/verification_method.py
--rw-r--r--   0        0        0     1505 2024-01-05 18:08:04.705254 pydid-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 pydid-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 01:26:05.173672 pydid-0.5.0/LICENSE
+-rw-r--r--   0        0        0      833 2024-05-10 01:26:05.173672 pydid-0.5.0/README.md
+-rw-r--r--   0        0        0     1713 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/__init__.py
+-rw-r--r--   0        0        0      319 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/common.py
+-rw-r--r--   0        0        0     2864 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/did.py
+-rw-r--r--   0        0        0     3213 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/did_url.py
+-rw-r--r--   0        0        0      580 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/doc/__init__.py
+-rw-r--r--   0        0        0     8622 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/doc/builder.py
+-rw-r--r--   0        0        0     2524 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/doc/corrections.py
+-rw-r--r--   0        0        0     7860 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/doc/doc.py
+-rw-r--r--   0        0        0     1706 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/doc/generic.py
+-rw-r--r--   0        0        0     4638 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/resource.py
+-rw-r--r--   0        0        0     1530 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/service.py
+-rw-r--r--   0        0        0     1101 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/validation.py
+-rw-r--r--   0        0        0     9353 2024-05-10 01:26:05.173672 pydid-0.5.0/pydid/verification_method.py
+-rw-r--r--   0        0        0     1517 2024-05-10 01:26:05.173672 pydid-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 pydid-0.5.0/PKG-INFO
```

### Comparing `pydid-0.4.3/LICENSE` & `pydid-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydid-0.4.3/pydid/__init__.py` & `pydid-0.5.0/pydid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from typing import Callable, List, Optional, Type
 
 from .common import DIDError
 from .did import DID, InvalidDIDError
 from .did_url import DIDUrl, InvalidDIDUrlError
+from .doc import corrections, generic
 from .doc.builder import DIDDocumentBuilder
 from .doc.doc import (
     BaseDIDDocument,
     BasicDIDDocument,
     DIDDocument,
     DIDDocumentError,
     NonconformantDocument,
@@ -17,15 +18,14 @@
 from .resource import Resource
 from .service import DIDCommService, Service
 from .verification_method import (
     VerificationMaterial,
     VerificationMaterialUnknown,
     VerificationMethod,
 )
-from .doc import generic, corrections
 
 __all__ = [
     "BasicDIDDocument",
     "DID",
     "DIDCommService",
     "DIDDocument",
     "DIDDocumentBuilder",
```

### Comparing `pydid-0.4.3/pydid/did.py` & `pydid-0.5.0/pydid/did.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """W3C DID Representation.
 
-DID Parsing rules derived from W3C Decentrialized Identifiers v1.0 Working Draft 18
+DID Parsing rules derived from W3C Decentralized Identifiers v1.0 Working Draft 18
 January 2021:
 
     https://w3c.github.io/did-core/
 
 """
 
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
+
+from pydantic import GetCoreSchemaHandler, GetJsonSchemaHandler
+from pydantic.json_schema import JsonSchemaValue
+from pydantic_core import CoreSchema, core_schema
 
 from .common import DID_PATTERN, DIDError
 from .did_url import DIDUrl
 
 
 class InvalidDIDError(DIDError, ValueError):
     """Invalid DID."""
@@ -31,22 +35,28 @@
         matched = DID_PATTERN.match(did)
         if not matched:
             raise InvalidDIDError("Unable to parse DID {}".format(did))
         self._method = matched.group(1)
         self._id = matched.group(2)
 
     @classmethod
-    def __get_validators__(cls):
-        """Yield validators for pydantic."""
-        yield cls._validate
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        """Get core schema."""
+        return core_schema.no_info_after_validator_function(cls, handler(str))
 
     @classmethod
-    def __modify_schema__(cls, field_schema):  # pragma: no cover
+    def __get_pydantic_json_schema__(
+        cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+    ) -> JsonSchemaValue:
         """Update schema fields."""
-        field_schema.update(pattern=DID_PATTERN)
+        json_schema = handler(core_schema)
+        json_schema["pattern"] = DID_PATTERN
+        return json_schema
 
     @property
     def method(self):
         """Return the method of this DID."""
         return self._method
 
     @property
@@ -69,17 +79,22 @@
 
     @classmethod
     def is_valid(cls, did: str):
         """Return if the passed string is a valid DID."""
         return DID_PATTERN.match(did)
 
     @classmethod
-    def validate(cls, did: str):
+    def model_validate(cls, did: str):
         """Validate the given string as a DID."""
         if not cls.is_valid(did):
             raise InvalidDIDError('"{}" is not a valid DID'.format(did))
         return did
 
     @classmethod
+    def validate(cls, did: str):
+        """Validate the given string as a DID."""
+        return cls.model_validate(did)
+
+    @classmethod
     def _validate(cls, did):
         """Pydantic validator."""
         return cls(did)
```

### Comparing `pydid-0.4.3/pydid/did_url.py` & `pydid-0.5.0/pydid/did_url.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """DID URL Object."""
-from typing import Dict, Optional, TYPE_CHECKING
+
+from typing import TYPE_CHECKING, Any, Dict, Optional
 from urllib.parse import parse_qsl, urlencode, urlparse
 
-from .common import DID_URL_DID_PART_PATTERN, DIDError, DID_URL_RELATIVE_FRONT
+from pydantic import GetCoreSchemaHandler, GetJsonSchemaHandler
+from pydantic.json_schema import JsonSchemaValue
+from pydantic_core import CoreSchema, core_schema
+
+from .common import DID_URL_DID_PART_PATTERN, DID_URL_RELATIVE_FRONT, DIDError
 
 if TYPE_CHECKING:  # pragma: no cover
     from .did import DID
 
 
 class InvalidDIDUrlError(DIDError, ValueError):
     """Invalid DID."""
@@ -34,22 +39,28 @@
 
         parts = urlparse(url_component)
         self.path = parts.path or None
         self.query = dict(parse_qsl(parts.query)) if parts.query else None
         self.fragment = parts.fragment or None
 
     @classmethod
-    def __get_validators__(cls):
-        """Yield validators."""
-        yield cls.validate
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        """Get core schema."""
+        return core_schema.no_info_after_validator_function(cls, handler(str))
 
     @classmethod
-    def __modify_schema__(cls, field_schema):  # pragma: no cover
+    def __get_pydantic_json_schema__(
+        cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+    ) -> JsonSchemaValue:
         """Update schema fields."""
-        field_schema.update(examples=["did:example:123/some/path?query=test#fragment"])
+        json_schema = handler(core_schema)
+        json_schema["examples"] = ["did:example:123/some/path?query=test#fragment"]
+        return json_schema
 
     @classmethod
     def parse(cls, url: str):
         """Parse DID URL from string."""
         return cls(url)
 
     @classmethod
```

### Comparing `pydid-0.4.3/pydid/doc/__init__.py` & `pydid-0.5.0/pydid/doc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """DID Document classes."""
 
+from .builder import (
+    DIDDocumentBuilder,
+    RelationshipBuilder,
+    ServiceBuilder,
+    VerificationMethodBuilder,
+)
 from .doc import (
-    IdentifiedResourceMismatch,
-    IDNotFoundError,
-    DIDDocumentRoot,
     BasicDIDDocument,
     DIDDocument,
     DIDDocumentError,
+    DIDDocumentRoot,
+    IdentifiedResourceMismatch,
+    IDNotFoundError,
 )
 
-from .builder import (
-    VerificationMethodBuilder,
-    RelationshipBuilder,
-    ServiceBuilder,
-    DIDDocumentBuilder,
-)
-
-
 __all__ = [
     "DIDDocumentError",
     "IdentifiedResourceMismatch",
     "IDNotFoundError",
     "DIDDocumentRoot",
     "BasicDIDDocument",
     "DIDDocument",
```

### Comparing `pydid-0.4.3/pydid/doc/builder.py` & `pydid-0.5.0/pydid/doc/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """VerificationMethod scoped builder."""
 
     def __init__(
         self,
         did: DID,
         *,
         id_base: str = None,
-        methods: Optional[List[VerificationMethod]] = None
+        methods: Optional[List[VerificationMethod]] = None,
     ):
         """Initialize builder."""
         self._did = did
         self.methods = methods or []
         self._id_base = id_base or "key"
         self._id_generator = self._default_id_generator()
 
@@ -38,15 +38,15 @@
         yield from _default_id_generator(self._id_base, start=len(self.methods))
 
     def add(
         self,
         type_: Type[VerificationMethod],
         ident: Optional[str] = None,
         controller: DID = None,
-        **kwargs
+        **kwargs,
     ):
         """Add verification method from parts and context."""
         ident = ident or next(self._id_generator)
         controller = controller or self._did
         vmethod = type_.make(id=self._did.ref(ident), controller=controller, **kwargs)
         self.methods.append(vmethod)
         return vmethod
@@ -60,15 +60,15 @@
     """Builder for relationships."""
 
     def __init__(
         self,
         did: DID,
         id_base: str,
         *,
-        methods: Optional[List[Union[VerificationMethod, DIDUrl]]] = None
+        methods: Optional[List[Union[VerificationMethod, DIDUrl]]] = None,
     ):
         """Initialize builder."""
         super().__init__(did, id_base=id_base)
         self.methods = methods or []
 
     def _default_id_generator(self):
         """Default ID generator."""
@@ -128,29 +128,29 @@
     ):
         """Add service."""
         ident = ident or next(self._id_generator)
         service = Service.make(
             id=self._did.ref(ident),
             type=type_,
             service_endpoint=service_endpoint,
-            **extra
+            **extra,
         )
         self.services.append(service)
         return service
 
     def add_didcomm(
         self,
         service_endpoint: str,
         recipient_keys: List[Union[VerificationMethod, DIDUrl, str]],
         routing_keys: Optional[List[Union[VerificationMethod, DIDUrl, str]]] = None,
         *,
         priority: Optional[int] = None,
         type_: Optional[str] = None,
         ident: Optional[str] = None,
-        accept: Optional[List[str]] = None
+        accept: Optional[List[str]] = None,
     ):
         """Add DIDComm Service."""
         ident = ident or next(self._id_generator)
         routing_keys = routing_keys or []
         priority = priority or self._determine_next_priority()
         service = DIDCommService.make(
             id=self._did.ref(ident),
@@ -180,15 +180,15 @@
 
     def __init__(
         self,
         id: Union[str, DID],
         context: List[str] = None,
         *,
         also_known_as: List[str] = None,
-        controller: Union[List[str], List[DID]] = None
+        controller: Union[List[str], List[DID]] = None,
     ):
         """Initliaze builder."""
         self.id: DID = DID(id)
         self.context = context or self.__default_context()
         self.also_known_as = also_known_as
         self.controller = controller
         self.verification_method = VerificationMethodBuilder(self.id)
@@ -236,21 +236,21 @@
             doc.id, "capability-delegation", methods=doc.capability_delegation
         )
         builder.service = ServiceBuilder(doc.id, services=doc.service)
         return builder
 
     def build(self) -> DIDDocument:
         """Build document."""
-        return DIDDocument.construct(
+        return DIDDocument.model_construct(
             id=self.id,
             context=self.context,
             also_known_as=self.also_known_as,
             controller=self.controller,
             verification_method=self.verification_method.methods or None,
             authentication=self.authentication.methods or None,
             assertion_method=self.assertion_method.methods or None,
             key_agreement=self.key_agreement.methods or None,
             capability_invocation=self.capability_invocation.methods or None,
             capability_delegation=self.capability_delegation.methods or None,
             service=self.service.services or None,
-            **self.extra
+            **self.extra,
         )
```

### Comparing `pydid-0.4.3/pydid/doc/corrections.py` & `pydid-0.5.0/pydid/doc/corrections.py`

 * *Files identical despite different names*

### Comparing `pydid-0.4.3/pydid/doc/doc.py` & `pydid-0.5.0/pydid/doc/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """DID Document Object."""
 
 from abc import ABC
 from typing import Any, List, Optional, Union
 
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 from typing_extensions import Annotated
 
 from ..did import DID, InvalidDIDError
 from ..did_url import DIDUrl, InvalidDIDUrlError
 from ..resource import IndexedResource, Resource
 from ..service import DIDCommV1Service, DIDCommV2Service, Service, UnknownService
 from ..verification_method import (
@@ -28,36 +28,34 @@
 class IDNotFoundError(DIDDocumentError):
     """Raised when Resource ID not found in DID Document."""
 
 
 class DIDDocumentRoot(Resource):
     """Representation of DID Document."""
 
-    context: Annotated[
-        List[Union[str, dict]], Field(alias="@context")
-    ] = [  # noqa: F722
+    context: Annotated[List[Union[str, dict]], Field(alias="@context")] = [
         "https://www.w3.org/ns/did/v1"
-    ]
+    ]  # noqa: F722
     id: DID
     also_known_as: Optional[List[str]] = None
     controller: Optional[List[DID]] = None
     verification_method: Optional[List[VerificationMethod]] = None
     authentication: Optional[List[Union[DIDUrl, VerificationMethod]]] = None
     assertion_method: Optional[List[Union[DIDUrl, VerificationMethod]]] = None
     key_agreement: Optional[List[Union[DIDUrl, VerificationMethod]]] = None
     capability_invocation: Optional[List[Union[DIDUrl, VerificationMethod]]] = None
     capability_delegation: Optional[List[Union[DIDUrl, VerificationMethod]]] = None
     service: Optional[List[Service]] = None
 
-    @validator("context", "controller", pre=True, allow_reuse=True)
+    @field_validator("context", "controller", mode="before")
     @classmethod
-    def _listify(cls, value):
+    def _listify(cls, value) -> Optional[list]:
         """Transform values into lists that are allowed to be a list or single."""
         if value is None:
-            return value
+            return
         if isinstance(value, list):
             return value
         return [value]
 
 
 class BaseDIDDocument(DIDDocumentRoot, IndexedResource, ABC):
     """Abstract BaseDIDDocument class."""
```

### Comparing `pydid-0.4.3/pydid/doc/generic.py` & `pydid-0.5.0/pydid/doc/generic.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 
 If using Python 3.7+, these can be used to simplify subclassing a DID Document.
 These classes are experimental and subject to change without notice. Use at
 your own risk.
 """
 
 import sys
+from typing import List, Optional, TypeVar, Union
+
+from pydantic import BaseModel
 
-from typing import TypeVar, Optional, List, Union
-from .doc import DIDDocumentRoot, BasicDIDDocument
-from ..verification_method import VerificationMethod
-from ..service import Service
 from ..did_url import DIDUrl
+from ..service import Service
+from ..verification_method import VerificationMethod
+from .doc import BasicDIDDocument, DIDDocumentRoot
 
 if sys.version_info >= (3, 7):  # pragma: no cover
-    # In Python 3.7+, we can use Generics with Pydantic to simplify subclassing
-    from pydantic.generics import GenericModel
     from typing import Generic
 
     VM = TypeVar("VM", bound=VerificationMethod)
     SV = TypeVar("SV", bound=Service)
     Methods = Optional[List[VM]]
     Relationships = Optional[List[Union[DIDUrl, VM]]]
     Services = Optional[List[SV]]
 
-    class GenericDIDDocumentRoot(DIDDocumentRoot, GenericModel, Generic[VM, SV]):
+    class GenericDIDDocumentRoot(DIDDocumentRoot, BaseModel, Generic[VM, SV]):
         """DID Document Root with Generics."""
 
         verification_method: Methods[VM] = None
         authentication: Relationships[VM] = None
         assertion_method: Relationships[VM] = None
         key_agreement: Relationships[VM] = None
         capability_invocation: Relationships[VM] = None
         capability_delegation: Relationships[VM] = None
         service: Services[SV] = None
 
-    class GenericBasicDIDDocument(BasicDIDDocument, GenericModel, Generic[VM, SV]):
+    class GenericBasicDIDDocument(BasicDIDDocument, BaseModel, Generic[VM, SV]):
         """BasicDIDDocument with Generics."""
 
         verification_method: Methods[VM] = None
         authentication: Relationships[VM] = None
         assertion_method: Relationships[VM] = None
         key_agreement: Relationships[VM] = None
         capability_invocation: Relationships[VM] = None
```

### Comparing `pydid-0.4.3/pydid/resource.py` & `pydid-0.5.0/pydid/resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Resource class that forms the base of all DID Document components."""
-from abc import ABC, abstractmethod
+
 import json
+from abc import ABC, abstractmethod
 from typing import Any, Dict, Type, TypeVar
 
-from inflection import camelize
-from pydantic import BaseModel, Extra, parse_obj_as
-from typing_extensions import Literal
 import typing_extensions
+from pydantic import BaseModel, ConfigDict, TypeAdapter, alias_generators
+from typing_extensions import Literal
 
 from .validation import wrap_validation_error
 
-
 ResourceType = TypeVar("ResourceType", bound="Resource")
 
 
 if hasattr(typing_extensions, "get_args"):  # pragma: no cover
     from typing_extensions import get_args, get_origin
 
     def get_literal_values(literal):
@@ -37,68 +36,65 @@
         """Return if type is literal."""
         return isinstance(type_, _Literal)
 
 
 class Resource(BaseModel):
     """Base class for DID Document components."""
 
-    class Config:
-        """Configuration for Resources."""
-
-        underscore_attrs_are_private = True
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        allow_mutation = False
-
-        @classmethod
-        def alias_generator(cls, string: str) -> str:
-            """Transform snake_case to camelCase."""
-            return camelize(string, uppercase_first_letter=False)
+    model_config = ConfigDict(
+        populate_by_name=True,
+        extra="allow",
+        alias_generator=alias_generators.to_camel,
+    )
 
     def serialize(self):
         """Return serialized representation of Resource."""
-        return self.dict(exclude_none=True, by_alias=True)
+        return self.model_dump(exclude_none=True, by_alias=True)
 
     @classmethod
     def deserialize(cls: Type[ResourceType], value: dict) -> ResourceType:
-        """Deserialize into VerificationMethod."""
+        """Deserialize into Resource subtype."""
         with wrap_validation_error(
             ValueError,
-            message="Failed to deserialize {}".format(cls.__name__),
+            message=f"Failed to deserialize {cls.__name__}",
         ):
-            return parse_obj_as(cls, value)
+            resource_adapter = TypeAdapter(cls)
+            return resource_adapter.validate_python(value)
 
     @classmethod
     def from_json(cls, value: str):
         """Deserialize Resource from JSON."""
         loaded: dict = json.loads(value)
         return cls.deserialize(loaded)
 
     def to_json(self):
         """Serialize Resource to JSON."""
-        return self.json(exclude_none=True, by_alias=True)
+        return self.model_dump_json(exclude_none=True, by_alias=True)
 
     @classmethod
     def _fill_in_required_literals(cls, **kwargs) -> Dict[str, Any]:
         """Return dictionary of field name to value from literals."""
-        for field in cls.__fields__.values():
+        for field in cls.model_fields.values():
+            field_name = field.alias
+            field_type = field.annotation
             if (
-                field.required
-                and is_literal(field.type_)
-                and (field.name not in kwargs or kwargs[field.name] is None)
+                field.is_required()
+                and is_literal(field_type)
+                and (field_name not in kwargs or kwargs[field_name] is None)
             ):
-                kwargs[field.name] = get_literal_values(field.type_)[0]
+                kwargs[field_name] = get_literal_values(field_type)[0]
         return kwargs
 
     @classmethod
     def _overwrite_none_with_defaults(cls, **kwargs) -> Dict[str, Any]:
         """Overwrite none values in kwargs with defaults for corresponding field."""
-        for field in cls.__fields__.values():
-            if field.name in kwargs and kwargs[field.name] is None:
-                kwargs[field.name] = field.get_default()
+        for field in cls.model_fields.values():
+            field_name = field.alias
+            if field_name in kwargs and kwargs[field_name] is None:
+                kwargs[field_name] = field.get_default()
         return kwargs
 
     @classmethod
     def make(cls: Type[ResourceType], **kwargs) -> ResourceType:
         """Create instance of class, filling in literals."""
         kwargs = cls._fill_in_required_literals(**kwargs)
         kwargs = cls._overwrite_none_with_defaults(**kwargs)
@@ -121,23 +117,21 @@
 
     @abstractmethod
     def dereference(self, reference: str) -> Resource:
         """Dereference a nested object."""
 
     def dereference_as(self, typ: Type[ResourceType], reference: str) -> ResourceType:
         """Dereference a resource to a specific type."""
-        resource = self.dereference(reference)
-        try:
-            return parse_obj_as(typ, resource.dict())
-        except ValueError as error:
-            raise ValueError(
-                "Dereferenced resource {} could not be parsed as {}".format(
-                    resource, typ
-                )
-            ) from error
+        with wrap_validation_error(
+            ValueError,
+            message=f"Dereferenced resource {reference} could not be parsed as {typ}",
+        ):
+            resource = self.dereference(reference)
+            resource_adapter: TypeAdapter[ResourceType] = TypeAdapter(typ)
+            return resource_adapter.validate_python(resource.model_dump())
 
     @classmethod
-    def construct(cls, **data):
+    def model_construct(cls, **data):
         """Construct and index."""
-        resource = super(Resource, cls).construct(**data)
+        resource = super(Resource, cls).model_construct(**data)
         resource._index_resources()
         return resource
```

### Comparing `pydid-0.4.3/pydid/service.py` & `pydid-0.5.0/pydid/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """DID Doc Service."""
 
 from typing import Any, List, Mapping, Optional, Union
-from typing_extensions import Literal
 
-from pydantic import AnyUrl, Extra, StrictStr
+from pydantic import AnyUrl, ConfigDict, StrictStr
+from typing_extensions import Literal
 
 from .did import DID
 from .did_url import DIDUrl
 from .resource import Resource
 
-
 EndpointStrings = Union[DID, DIDUrl, AnyUrl, StrictStr]
 
 
 class Service(Resource):
     """Representation of DID Document Services."""
 
     id: DIDUrl
@@ -24,22 +23,19 @@
         Mapping[str, Any],
     ]
 
 
 class DIDCommV1Service(Service):
     """DID Communication Service."""
 
-    class Config:
-        """DIDComm Service Config."""
+    model_config = ConfigDict(extra="forbid")
 
-        extra = Extra.forbid
-
-    type: Literal[
-        "IndyAgent", "did-communication", "DIDCommMessaging"
-    ] = "did-communication"
+    type: Literal["IndyAgent", "did-communication", "DIDCommMessaging"] = (
+        "did-communication"
+    )
     service_endpoint: EndpointStrings
     recipient_keys: List[DIDUrl]
     routing_keys: List[DIDUrl] = []
     accept: Optional[List[str]] = None
     priority: int = 0
 
 
@@ -53,18 +49,15 @@
     accept: Optional[List[str]] = None
     routing_keys: List[DIDUrl] = []
 
 
 class DIDCommV2Service(Service):
     """DID Communication V2 Service."""
 
-    class Config:
-        """DIDComm Service Config."""
-
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     type: Literal["DIDCommMessaging"] = "DIDCommMessaging"
     service_endpoint: Union[List[DIDCommV2ServiceEndpoint], DIDCommV2ServiceEndpoint]
 
 
 class UnknownService(Service):
     """Unknown Service."""
```

### Comparing `pydid-0.4.3/pydid/validation.py` & `pydid-0.5.0/pydid/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """Validation tools and helpers."""
 
 from contextlib import contextmanager
 from typing import Set, Type
 
-from pydantic import ValidationError, root_validator
+from pydantic import ValidationError, ValidationInfo, model_validator
 
 
 @contextmanager
 def wrap_validation_error(error_to_raise: Type[Exception], message: str = None):
-    """Wrap validation erros with more friendly errors."""
+    """Wrap validation errors with more friendly errors."""
     try:
         yield
     except ValidationError as error:
         raise error_to_raise(
             ":\n".join([message, str(error)]) if message else str(error)
         ) from error
 
 
 def required_group(props: Set[str]):
     """Require at least one of the properties to be present."""
 
-    def _require_group(_model, values: dict):
+    def _require_group(_model, _: ValidationInfo):
+        if not isinstance(_model, dict):
+            _model = _model.__dict__
+
         defined_props = props & {
-            key for key, value in values.items() if value is not None
+            key for key, value in _model.items() if value is not None
         }
         if len(defined_props) < 1:
             raise ValueError(
                 "At least one of {} was required; none found".format(props)
             )
-        return values
+        return _model
 
-    return root_validator(allow_reuse=True)(_require_group)
+    return model_validator(mode="after")(_require_group)
```

### Comparing `pydid-0.4.3/pydid/verification_method.py` & `pydid-0.5.0/pydid/verification_method.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 """DID Doc Verification Method."""
 
-from pydid.validation import required_group
 from typing import ClassVar, Optional, Set, Type, Union
 
 from inflection import underscore
-from pydantic import create_model
-from pydantic.class_validators import root_validator, validator
+from pydantic import create_model, field_validator, model_validator, alias_generators
 from typing_extensions import Literal
 
+from pydid.validation import required_group
+
 from .did import DID
 from .did_url import DIDUrl, InvalidDIDUrlError
 from .resource import Resource
 
+set_of_material_properties = {
+    "blockchain_account_id",
+    "ethereum_address",
+    "public_key_base58",
+    "public_key_gpg",
+    "public_key_hex",
+    "public_key_jwk",
+    "public_key_pem",
+    "public_key_multibase",
+}
+material_properties_camel = {
+    alias_generators.to_camel(prop) for prop in set_of_material_properties
+}
+
 
 class VerificationMaterial:
     """Type annotation marker for the material attribute of a verification method."""
 
 
 class VerificationMaterialUnknown(NotImplementedError):
     """Raised when verification material is unknown but access is attempted."""
 
 
 class VerificationMethod(Resource):
     """Representation of DID Document Verification Methods."""
 
-    material_properties: ClassVar[Set[str]] = {
-        "blockchain_account_id",
-        "ethereum_address",
-        "public_key_base58",
-        "public_key_gpg",
-        "public_key_hex",
-        "public_key_jwk",
-        "public_key_pem",
-        "public_key_multibase",
-    }
+    material_properties: ClassVar[Set[str]] = set_of_material_properties
 
     id: DIDUrl
     type: str
     controller: DID
     public_key_hex: Optional[str] = None
     public_key_base58: Optional[str] = None
     public_key_pem: Optional[str] = None
@@ -55,84 +60,96 @@
     @classmethod
     def suite(cls: Type, typ: str, material: str, material_type: Type):
         """Return a subclass of VerificationMethod for a given type."""
         model = create_model(
             typ,
             __module__=cls.__module__,
             __base__=cls,
-            type=(Literal[typ], ...),
+            type=(Literal[typ], ...),  # type:ignore
             **{underscore(material): (material_type, ...)},
         )
         model.material = property(
             lambda self: getattr(self, underscore(material)),
             lambda self, value: setattr(self, underscore(material), value),
         )
         model._material_prop = underscore(material)
         return model
 
-    @validator("type", pre=True)
+    @field_validator("type", mode="before")
     @classmethod
-    def _allow_type_list(cls, value: Union[str, list]):
+    def _allow_type_list(cls, value: Union[str, list[str]]) -> str:
         """Unwrap type list.
 
         This validator handles a common DID Document mutation.
         """
         if isinstance(value, list):
             return value[0]
         return value
 
-    @validator("controller", pre=True)
+    @field_validator("controller", mode="before")
     @classmethod
-    def _allow_controller_list(cls, value: Union[str, list]):
+    def _allow_controller_list(cls, value: Union[DID, list[DID]]) -> DID:
         """Unwrap controller list.
 
         This validator handles a common DID Document mutation.
         """
         if isinstance(value, list):
             return value[0]
         return value
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
-    def _allow_missing_controller(cls, values: dict):
+    def _allow_missing_controller(cls, values: Union[dict, "VerificationMethod"]):
         """Derive controller value from ID.
 
         This validator handles a common DID Document mutation.
         """
+        if not isinstance(values, dict):
+            values = values.__dict__
+
         if "controller" not in values:
             if "id" not in values:
                 raise ValueError(
                     "Could not derive controller: no id present in verification method"
                 )
             try:
                 ident = DIDUrl.parse(values["id"])
-            except InvalidDIDUrlError:
-                return values
-            else:
                 values["controller"] = ident.did
+            except InvalidDIDUrlError:
+                pass
         return values
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
-    def _method_appears_to_contain_material(cls, values: dict):
+    def _method_appears_to_contain_material(
+        cls, values: Union[dict, "VerificationMethod"]
+    ):
         """Validate that the method appears to contain verification material."""
-        if len(values) < 4:
+        if not isinstance(values, dict):
+            values = values.__dict__
+
+        if values.get("controller") and len(values) < 4:
             raise ValueError(
                 "Key material expected, found: {}".format(list(values.keys()))
             )
         return values
 
-    @root_validator
+    @model_validator(mode="before")
     @classmethod
-    def _no_more_than_one_material_prop(cls, values: dict):
+    def _no_more_than_one_material_prop(cls, values: Union[dict, "VerificationMethod"]):
         """Validate that exactly one material property was specified on method."""
-        set_material_properties = cls.material_properties & {
-            key for key, value in values.items() if value is not None
-        }
-        if len(set_material_properties) > 1:
+        if not isinstance(values, dict):
+            values = values.__dict__
+
+        model_properties = {key for key, value in values.items() if value is not None}
+
+        set_material_properties = set_of_material_properties & model_properties
+        set_material_properties_camel = material_properties_camel & model_properties
+
+        if len(set_material_properties | set_material_properties_camel) > 1:
             raise ValueError(
                 "Found properties {}; only one is allowed".format(
                     ", ".join(set_material_properties)
                 )
             )
         return values
 
@@ -211,18 +228,18 @@
 class Bls1238G2Key2020(VerificationMethod):
     """Bls1238G2Key2020 VerificationMethod."""
 
     type: Literal["Bls1238G2Key2020"]
     public_key_base58: str
 
 
-class GpgVerifcationKey2020(VerificationMethod):
-    """GpgVerifcationKey2020 VerificationMethod."""
+class GpgVerificationKey2020(VerificationMethod):
+    """GpgVerificationKey2020 VerificationMethod."""
 
-    type: Literal["GpgVerifcationKey2020"]
+    type: Literal["GpgVerificationKey2020"]
     public_key_gpg: str
 
 
 class RsaVerificationKey2018(VerificationMethod):
     """RsaVerificationKey2018 VerificationMethod."""
 
     type: Literal["RsaVerificationKey2018"]
@@ -277,15 +294,15 @@
     Ed25519VerificationKey2018,
     Ed25519VerificationKey2020,
     OpenPgpVerificationKey2019,
     JsonWebKey2020,
     EcdsaSecp256k1VerificationKey2019,
     Bls1238G1Key2020,
     Bls1238G2Key2020,
-    GpgVerifcationKey2020,
+    GpgVerificationKey2020,
     RsaVerificationKey2018,
     X25519KeyAgreementKey2019,
     X25519KeyAgreementKey2020,
     SchnorrSecp256k1VerificationKey2019,
     EcdsaSecp256k1RecoveryMethod2020,
     Multikey,
 ]
```

### Comparing `pydid-0.4.3/pyproject.toml` & `pydid-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydid"
-version = "0.4.3"
+version = "0.5.0"
 description = "Python library for validating, constructing, and representing DIDs and DID Documents"
 authors = ["Daniel Bluhm <dbluhm@pm.me>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/Indicio-tech/pydid"
 repository = "https://github.com/Indicio-tech/pydid"
 keywords = [
@@ -12,50 +12,50 @@
 ]
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
-pydantic = "^1.10.0"
-typing-extensions = "^4.5.0"
+python = "^3.9.0"
+pydantic = "^2.7.0"
+typing-extensions = "^4.7.0"
 inflection = "^0.5.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4.0"
-black = "^23.7.0"
+pytest = "^8.1.1"
+black = "^24.4.0"
 poetry = "^1.5.0"
 pre-commit = "^3.3.0"
-ruff = "^0.0.287"
+ruff = "^0.4.3"
 pytest-coverage = "^0.0"
-aiohttp = "^3.8.0"
-pytest-asyncio = "^0.21.0"
-coverage = {extras = ["toml"], version = "^7.2.0"}
+aiohttp = "^3.9.5"
+pytest-asyncio = "^0.23.6"
+coverage = {extras = ["toml"], version = "^7.5.1"}
 
 [tool.pytest.ini_options]
 addopts = "-p no:warnings --cov pydid --doctest-modules"
 markers = "int: integration tests"
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "@abstract"
 ]
 precision = 2
 show_missing = true
 
 [tool.ruff]
-select = ["E", "F", "C", "D"]
+lint.select = ["E", "F", "C", "D"]
 
-ignore = [
+lint.ignore = [
     # Google Python Doc Style
     "D203", "D204", "D213", "D215", "D400", "D401", "D404", "D406", "D407",
     "D408", "D409", "D413",
     "D202", # Allow blank line after docstring
     "D104", # Don't require docstring in public package
 ]
 
 line-length = 90
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "**/{tests}/*" = ["F841", "D", "E501"]
```

### Comparing `pydid-0.4.3/PKG-INFO` & `pydid-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: pydid
-Version: 0.4.3
+Version: 0.5.0
 Summary: Python library for validating, constructing, and representing DIDs and DID Documents
 Home-page: https://github.com/Indicio-tech/pydid
 License: Apache 2.0
 Keywords: decentralized,identity,ssi,DID,DID Document
 Author: Daniel Bluhm
 Author-email: dbluhm@pm.me
-Requires-Python: >=3.8.0,<4.0.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.7.0,<5.0.0)
 Project-URL: Repository, https://github.com/Indicio-tech/pydid
 Description-Content-Type: text/markdown
 
 # PyDID
 
 [![pypi release](https://img.shields.io/pypi/v/pydid)](https://pypi.org/project/pydid/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
@@ -29,36 +28,35 @@
 Python library for validating, constructing, and representing DIDs and DID Documents.
 
 ## Installation
 
 Using a virtual environment is generally recommended:
 
 ```sh
-$ python -m venv env
-$ source env/bin/activate
+python -m venv env
+source env/bin/activate
 ```
 
 Install with pip:
 
 ```sh
-$ pip install pydid
+pip install pydid
 ```
 
 ## Development
 
 This project is managed with [Poetry](https://python-poetry.org/).
 
 To begin making code changes, clone this repo and do the following to install
 dependencies:
 
 ```sh
-$ python -m venv env
-$ source env/bin/activate
-$ pip install poetry
-$ poetry install
+python -m venv env
+source env/bin/activate
+pip install poetry
+poetry install
 ```
 
-
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md).
```

