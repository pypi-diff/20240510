# Comparing `tmp/addemongo-0.0.3.tar.gz` & `tmp/addemongo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addemongo-0.0.3.tar", last modified: Thu May  9 21:08:43 2024, max compression
+gzip compressed data, was "addemongo-0.0.4.tar", last modified: Fri May 10 03:56:06 2024, max compression
```

## Comparing `addemongo-0.0.3.tar` & `addemongo-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      115 2024-05-09 21:08:35.017607 addemongo-0.0.3/LICENSE
--rw-r--r--   0        0        0      128 2024-05-09 21:08:35.017607 addemongo-0.0.3/README.md
--rw-r--r--   0        0        0     3133 2024-05-09 21:08:43.441622 addemongo-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       65 2024-05-09 21:08:35.017607 addemongo-0.0.3/src/addemongo/__init__.py
--rw-r--r--   0        0        0       22 2024-05-09 21:08:35.017607 addemongo-0.0.3/src/addemongo/__version__.py
--rw-r--r--   0        0        0     1206 2024-05-09 21:08:35.017607 addemongo-0.0.3/src/addemongo/_base_client.py
--rw-r--r--   0        0        0        0 2024-05-09 21:08:35.017607 addemongo-0.0.3/src/addemongo/_motor/__init__.py
--rw-r--r--   0        0        0     4088 2024-05-09 21:08:35.017607 addemongo-0.0.3/src/addemongo/_motor/_client.py
--rw-r--r--   0        0        0        0 2024-05-09 21:08:35.017607 addemongo-0.0.3/src/addemongo/_pymongo/__init__.py
--rw-r--r--   0        0        0     4010 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/_pymongo/_client.py
--rw-r--r--   0        0        0      267 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/_types.py
--rw-r--r--   0        0        0      126 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/builders/__init__.py
--rw-r--r--   0        0        0     3079 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/builders/aggregation.py
--rw-r--r--   0        0        0     3508 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/builders/query.py
--rw-r--r--   0        0        0     1407 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/connection.py
--rw-r--r--   0        0        0        0 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/models/__init__.py
--rw-r--r--   0        0        0      193 2024-05-09 21:08:35.021607 addemongo-0.0.3/src/addemongo/models/pagination.py
--rw-r--r--   0        0        0        0 2024-05-09 21:08:35.021607 addemongo-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3802 2024-05-09 21:08:35.021607 addemongo-0.0.3/tests/addemongo/test_async_functions.py
--rw-r--r--   0        0        0      960 2024-05-09 21:08:35.021607 addemongo-0.0.3/tests/addemongo/test_client.py
--rw-r--r--   0        0        0     2482 2024-05-09 21:08:35.021607 addemongo-0.0.3/tests/addemongo/test_sync_functions.py
--rw-r--r--   0        0        0      216 2024-05-09 21:08:35.021607 addemongo-0.0.3/tests/motor/test_motor.py
--rw-r--r--   0        0        0      227 2024-05-09 21:08:35.021607 addemongo-0.0.3/tests/pymongo/test_pymongo.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 addemongo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      115 2024-05-10 03:55:56.812131 addemongo-0.0.4/LICENSE
+-rw-r--r--   0        0        0      128 2024-05-10 03:55:56.812131 addemongo-0.0.4/README.md
+-rw-r--r--   0        0        0     3133 2024-05-10 03:56:06.644127 addemongo-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/__version__.py
+-rw-r--r--   0        0        0     1421 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_base_client.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_motor/__init__.py
+-rw-r--r--   0        0        0     4088 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_motor/_client.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_pymongo/__init__.py
+-rw-r--r--   0        0        0     4010 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_pymongo/_client.py
+-rw-r--r--   0        0        0      267 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_types.py
+-rw-r--r--   0        0        0      126 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/builders/__init__.py
+-rw-r--r--   0        0        0     3079 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/builders/aggregation.py
+-rw-r--r--   0        0        0     3508 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/builders/query.py
+-rw-r--r--   0        0        0     1407 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/connection.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/models/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/models/pagination.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3802 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/addemongo/test_async_functions.py
+-rw-r--r--   0        0        0      960 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/addemongo/test_client.py
+-rw-r--r--   0        0        0     2482 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/addemongo/test_sync_functions.py
+-rw-r--r--   0        0        0      216 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/motor/test_motor.py
+-rw-r--r--   0        0        0      227 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/pymongo/test_pymongo.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 addemongo-0.0.4/PKG-INFO
```

### Comparing `addemongo-0.0.3/pyproject.toml` & `addemongo-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     { name = "Victor Gabriel", email = "victordeonroyale@gmail.com" },
 ]
 maintainers = [
     { name = "Gabriel Silva", email = "gabrieltkdnobrega63@gmail.com" },
     { name = "Victor Gabriel", email = "victordeonroyale@gmail.com" },
 ]
 dynamic = []
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Company = "https://addebitare.com.br"
 Repository = "https://github.com/biellSilva/addemongo.git"
```

### Comparing `addemongo-0.0.3/src/addemongo/_base_client.py` & `addemongo-0.0.4/src/addemongo/_base_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import TYPE_CHECKING, Any, Generic, Type
 
 from pydantic import BaseModel as _PydanticBaseModel
 
-
 from ._types import BM
 
 if TYPE_CHECKING:
     from addemongo.connection import AddeMongoConnection
 
 
 class AddeMongoBaseClient(Generic[BM]):
     def __init__(
         self,
-        connection: 'AddeMongoConnection',
+        connection: "AddeMongoConnection",
         database: str,
         collection: str,
         response_class: Type[BM],
     ) -> None:
         self.connection = connection
         self.database_name = database
         self.collection_name = collection
@@ -26,15 +25,21 @@
         annotations: dict[str, Any] = {}
         self.__create_projection_schema(self.response_class, annotations)
         return annotations
 
     def __create_projection_schema(
         self, document: type[_PydanticBaseModel], base: dict[str, Any]
     ) -> dict[str, Any]:
+        if document.__bases__:
+            for base_class in document.__bases__:
+                if issubclass(base_class, _PydanticBaseModel):
+                    self.__create_projection_schema(base_class, base)
+
         annotations = document.__annotations__.copy()
+
         for key, value in annotations.items():
             if issubclass(value, _PydanticBaseModel):
                 base[key] = self.__create_projection_schema(value, {})
             else:
                 base[key] = 1
 
         return base
```

### Comparing `addemongo-0.0.3/src/addemongo/_motor/_client.py` & `addemongo-0.0.4/src/addemongo/_motor/_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/src/addemongo/_pymongo/_client.py` & `addemongo-0.0.4/src/addemongo/_pymongo/_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/src/addemongo/builders/aggregation.py` & `addemongo-0.0.4/src/addemongo/builders/aggregation.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/src/addemongo/builders/query.py` & `addemongo-0.0.4/src/addemongo/builders/query.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/src/addemongo/connection.py` & `addemongo-0.0.4/src/addemongo/connection.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/tests/addemongo/test_async_functions.py` & `addemongo-0.0.4/tests/addemongo/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/tests/addemongo/test_client.py` & `addemongo-0.0.4/tests/addemongo/test_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/tests/addemongo/test_sync_functions.py` & `addemongo-0.0.4/tests/addemongo/test_sync_functions.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.3/PKG-INFO` & `addemongo-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addemongo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Private mongo repository for Addebitare company
 Author-Email: Gabriel Silva <gabrieltkdnobrega63@gmail.com>, Victor Gabriel <victordeonroyale@gmail.com>
 Maintainer-Email: Gabriel Silva <gabrieltkdnobrega63@gmail.com>, Victor Gabriel <victordeonroyale@gmail.com>
 License: All Rights Reserved.
         
         (c) Copyright 2024 Gabriel Nobrega, Victor Gabriel and Addebitare Team, all rights reserved.
 Project-URL: Company, https://addebitare.com.br
```

