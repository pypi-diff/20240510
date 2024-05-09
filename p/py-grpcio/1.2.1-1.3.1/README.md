# Comparing `tmp/py_grpcio-1.2.1.tar.gz` & `tmp/py_grpcio-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.2.1.tar", max compression
+gzip compressed data, was "py_grpcio-1.3.1.tar", max compression
```

## Comparing `py_grpcio-1.2.1.tar` & `py_grpcio-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1076 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/LICENSE
--rw-r--r--   0        0        0     2836 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/README.md
--rw-r--r--   0        0        0      119 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/__init__.py
--rw-r--r--   0        0        0      277 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1422 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     2769 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/method.py
--rw-r--r--   0        0        0     3263 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3685 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      682 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     1873 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/service.py
--rw-r--r--   0        0        0     2417 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 py_grpcio-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4581 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/README.md
+-rw-r--r--   0        0        0      119 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/__init__.py
+-rw-r--r--   0        0        0      750 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1809 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     4190 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/method.py
+-rw-r--r--   0        0        0     4639 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3818 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      682 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     1873 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/server.py
+-rw-r--r--   0        0        0      924 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/service.py
+-rw-r--r--   0        0        0     2417 2024-05-09 22:05:04.794626 py_grpcio-1.3.1/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-09 22:05:04.794626 py_grpcio-1.3.1/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-09 22:05:04.794626 py_grpcio-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.3.1/PKG-INFO
```

### Comparing `py_grpcio-1.2.1/LICENSE` & `py_grpcio-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.2.1/py_grpcio/interceptor.py` & `py_grpcio-1.3.1/py_grpcio/interceptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from grpc.aio import ServicerContext
 from grpc_interceptor.exceptions import GrpcException
 from grpc_interceptor.server import AsyncServerInterceptor
 
 from google.protobuf.message import Message
 
 from py_grpcio.method import ServerMethodGRPC
+from py_grpcio.exceptions import RunTimeServerError
 
 
 class ServerInterceptor(AsyncServerInterceptor):
     async def intercept(
         self: 'ServerInterceptor',
         route: ServerMethodGRPC,
         message: Message,
@@ -27,14 +28,21 @@
         except GrpcException as grpc_exc:
             logger.error(
                 f'{context.peer()} - {route.__qualname__} | '
                 f'{grpc_exc.__class__.__name__} | {grpc_exc.status_code} | {grpc_exc.details}'
             )
             context.set_code(grpc_exc.status_code)
             context.set_details(grpc_exc.details)
+        except RunTimeServerError as py_grpc_io_exc:
+            logger.error(py_grpc_io_exc)
+            context.set_code(py_grpc_io_exc.status_code)
+            context.set_details(
+                'Internal Server Error'
+                if py_grpc_io_exc.status_code == StatusCode.INTERNAL else py_grpc_io_exc.details
+            )
         except ValidationError as exc:
             context.set_code(StatusCode.INVALID_ARGUMENT)
             context.set_details(exc.json())
         except Exception as exc:
             logger.exception(exc)
             context.set_code(StatusCode.INTERNAL)
             context.set_details('Internal Server Error')
```

### Comparing `py_grpcio-1.2.1/py_grpcio/proto/parser.py` & `py_grpcio-1.3.1/py_grpcio/proto/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from uuid import UUID
+from enum import Enum
 from inspect import isclass
 from datetime import datetime
 
 from pydantic import BaseModel
 
 from types import UnionType, NoneType
 from typing import Any, Annotated, Union, Iterable, get_origin
@@ -76,11 +77,13 @@
         if origin in (Union, UnionType):
             return parse_type_union(field_name=field_name, field_type=field_type, args=args)
         if issubclass(origin, dict):
             return parse_type_mapping(field_name=field_name, field_type=field_type, args=args)
         if issubclass(origin, Iterable):  # noqa: origin
             return parse_type_sequence(field_name=field_name, field_type=field_type, args=args)
         raise TypeError(f'Field unsupported type `{field_type}`')
-    elif isclass(field_type) and issubclass(field_type, BaseModel):
-        return {'name': field_name, 'type': field_type.__name__}
-    else:
-        raise TypeError(f'Field unsupported type `{field_type}`')
+    elif isclass(field_type):
+        if issubclass(field_type, BaseModel):
+            return {'name': field_name, 'type': field_type.__name__}
+        elif issubclass(field_type, Enum):
+            return {'name': field_name, 'type': ProtoBufTypes.STRING}
+    raise TypeError(f'Field unsupported type `{field_type}`')
```

### Comparing `py_grpcio-1.2.1/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.3.1/py_grpcio/proto/templates/service.proto.template`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.2.1/py_grpcio/server.py` & `py_grpcio-1.3.1/py_grpcio/server.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.2.1/py_grpcio/service.py` & `py_grpcio-1.3.1/py_grpcio/service.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.2.1/py_grpcio/service_meta.py` & `py_grpcio-1.3.1/py_grpcio/service_meta.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.2.1/py_grpcio/utils.py` & `py_grpcio-1.3.1/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.2.1/pyproject.toml` & `py_grpcio-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.2.1"
+version = "1.3.1"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.2.1/PKG-INFO` & `py_grpcio-1.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.2.1
+Version: 1.3.1
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -49,22 +49,39 @@
 from uuid import UUID, uuid4
 from datetime import datetime
 
 from pydantic import Field
 
 from py_grpcio import Message
 
+from example.server.service.enums import Names
+
 
 class PingRequest(Message):
     id: UUID = Field(default_factory=uuid4)
 
 
 class PingResponse(Message):
     id: UUID
     timestamp: datetime = Field(default_factory=datetime.now)
+
+
+class ComplexModel(Message):
+    name: Names
+
+
+class ComplexRequest(Message):
+    id: UUID
+    model: ComplexModel
+
+
+class ComplexResponse(Message):
+    id: UUID
+    model: ComplexModel
+
 ```
 
 ---
 
 ### Server
 
 Basic implementation of **gRPC** services on the server side.
@@ -73,42 +90,61 @@
 
 
 ```python
 from abc import abstractmethod
 
 from py_grpcio import BaseService
 
-from example.server.core.models import PingRequest, PingResponse
+from example.server.service.models import PingRequest, PingResponse, ComplexRequest, ComplexResponse
 
 
 class BaseExampleService(BaseService):
     @abstractmethod
-    async def ping(self, request: PingRequest) -> PingResponse:
+    async def ping(self: 'BaseExampleService', request: PingRequest) -> PingResponse:
         ...
+
+    @abstractmethod
+    async def complex(self: 'BaseExampleService', request: ComplexRequest) -> ComplexResponse:
+        ...
+
 ```
 
 ---
 
 Full implementation of the **gRPC** service with methods.
 
 ```python
-from example.server.core import BaseExampleService, PingRequest, PingResponse
-
-from py_grpcio import BaseServer
+from example.server.service.base import BaseExampleService
+from example.server.service.models import PingRequest, PingResponse, ComplexRequest, ComplexResponse
 
 
 class ExampleService(BaseExampleService):
-    async def ping(self, request: PingRequest) -> PingResponse:
+    async def ping(self: 'ExampleService', request: PingRequest) -> PingResponse:
         return PingResponse(id=request.id)
 
+    async def complex(self: 'BaseExampleService', request: ComplexRequest) -> ComplexResponse:
+        return ComplexResponse(**request.model_dump())
+
+```
+
+---
+
+Run the ExampleService on Server.
+
+```python
+from py_grpcio import BaseServer
+
+from example.server.service import ExampleService
+
 
 if __name__ == '__main__':
     server: BaseServer = BaseServer()
     server.add_service(service=ExampleService)
     server.run()
+
 ```
 
 ---
 
 Note that on the client side, this class must be named the same as it is named in the full server-side implementation.
 
 That is, if on the server we call the base class as `BaseExampleService` and the class with the implementation of 
@@ -118,26 +154,63 @@
 ### Client
 
 ```python
 from abc import abstractmethod
 
 from py_grpcio import BaseService
 
-from example.client.core.models import PingRequest, PingResponse
+from example.server.service.models import PingRequest, PingResponse, ComplexRequest, ComplexResponse
 
 
 class ExampleService(BaseService):
     @abstractmethod
-    async def ping(self, request: PingRequest) -> PingResponse:
+    async def ping(self: 'ExampleService', request: PingRequest) -> PingResponse:
+        ...
+
+    @abstractmethod
+    async def complex(self: 'ExampleService', request: ComplexRequest) -> ComplexResponse:
         ...
 
 ```
 
 ---
 
+Calling the ExampleService endpoints by Client.
+
+```python
+from uuid import uuid4
+from asyncio import run
+
+from loguru import logger
+
+from example.client.services.example.enums import Names
+from example.client.services.example import (
+    ExampleService, PingRequest, PingResponse, ComplexModel, ComplexRequest, ComplexResponse
+)
+
+service: ExampleService = ExampleService(host='127.0.0.1')
+
+
+async def main() -> None:
+    response: PingResponse = await service.ping(request=PingRequest())
+    logger.info(f'ping response: {response}')
+
+    response: ComplexResponse = await service.complex(
+        request=ComplexRequest(id=uuid4(), model=ComplexModel(name=Names.NAME_1))
+    )
+    logger.info(f'complex response: {response}')
+
+
+if __name__ == '__main__':
+    run(main())
+
+```
+
+---
+
 ### Notes
 
 * You can use the library on the client side even if the server is implemented differently 
 by simply describing it as an abstract service
 
 * The client can also be implemented using other libraries, the server that uses `py-grpcio` 
 will still be able to accept such requests
```

