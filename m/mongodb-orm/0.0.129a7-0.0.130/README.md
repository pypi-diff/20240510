# Comparing `tmp/mongodb_orm-0.0.129a7.tar.gz` & `tmp/mongodb_orm-0.0.130.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.129a7.tar", last modified: Fri May 10 08:29:34 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.130.tar", last modified: Fri May  3 12:50:20 2024, max compression
```

## Comparing `mongodb_orm-0.0.129a7.tar` & `mongodb_orm-0.0.130.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.706421 mongodb_orm-0.0.129a7/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      335 2024-05-10 08:29:34.705629 mongodb_orm-0.0.129a7/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.129a7/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.687300 mongodb_orm-0.0.129a7/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.129a7/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.129a7/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.691501 mongodb_orm-0.0.129a7/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.129a7/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.0.129a7/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.692601 mongodb_orm-0.0.129a7/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.129a7/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      468 2024-05-10 08:21:28.000000 mongodb_orm-0.0.129a7/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.693569 mongodb_orm-0.0.129a7/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.129a7/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.129a7/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.695874 mongodb_orm-0.0.129a7/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.129a7/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.0.129a7/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7659 2024-05-10 08:21:28.000000 mongodb_orm-0.0.129a7/mongodb_orm/interfaces/mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.0.129a7/mongodb_orm/interfaces/mongodb_model_events.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.696390 mongodb_orm-0.0.129a7/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.129a7/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.697399 mongodb_orm-0.0.129a7/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.129a7/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.129a7/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.697952 mongodb_orm-0.0.129a7/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.129a7/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.698822 mongodb_orm-0.0.129a7/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.129a7/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.129a7/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.702110 mongodb_orm-0.0.129a7/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.129a7/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.129a7/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.129a7/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      421 2024-05-10 08:21:28.000000 mongodb_orm-0.0.129a7/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      772 2024-05-10 08:21:28.000000 mongodb_orm-0.0.129a7/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.129a7/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.0.129a7/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.703095 mongodb_orm-0.0.129a7/mongodb_orm/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.129a7/mongodb_orm/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2122 2024-05-10 08:27:16.000000 mongodb_orm-0.0.129a7/mongodb_orm/utils/helpers.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.704065 mongodb_orm-0.0.129a7/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.129a7/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4008 2024-05-10 08:21:28.000000 mongodb_orm-0.0.129a7/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-10 08:29:34.704803 mongodb_orm-0.0.129a7/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      335 2024-05-10 08:29:34.000000 mongodb_orm-0.0.129a7/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-05-10 08:29:34.000000 mongodb_orm-0.0.129a7/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-05-10 08:29:34.000000 mongodb_orm-0.0.129a7/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-05-10 08:29:34.000000 mongodb_orm-0.0.129a7/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-05-10 08:29:34.000000 mongodb_orm-0.0.129a7/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-05-10 08:29:34.706597 mongodb_orm-0.0.129a7/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      602 2024-05-10 08:29:24.000000 mongodb_orm-0.0.129a7/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.011392 mongodb_orm-0.0.130/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-05-03 12:50:20.010628 mongodb_orm-0.0.130/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.130/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.987397 mongodb_orm-0.0.130/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.130/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.130/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.991405 mongodb_orm-0.0.130/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.130/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.0.130/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.992785 mongodb_orm-0.0.130/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.130/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.994312 mongodb_orm-0.0.130/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.130/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.998052 mongodb_orm-0.0.130/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7653 2024-05-03 12:47:26.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/mongodb_model_events.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.999053 mongodb_orm-0.0.130/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.130/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.000015 mongodb_orm-0.0.130/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.130/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.000897 mongodb_orm-0.0.130/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.130/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.001907 mongodb_orm-0.0.130/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.006272 mongodb_orm-0.0.130/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-05-03 12:47:26.000000 mongodb_orm-0.0.130/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.130/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.0.130/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.007400 mongodb_orm-0.0.130/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.130/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1163 2024-04-26 10:44:00.000000 mongodb_orm-0.0.130/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.008773 mongodb_orm-0.0.130/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.130/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.009786 mongodb_orm-0.0.130/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-05-03 12:50:20.011546 mongodb_orm-0.0.130/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-05-03 12:50:10.000000 mongodb_orm-0.0.130/setup.py
```

### Comparing `mongodb_orm-0.0.129a7/README.md` & `mongodb_orm-0.0.130/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.0.130/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.130/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.0.130/mongodb_orm/interfaces/mongodb_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self._result: Cursor | InsertOneResult | dict | None = None
         self.chained = True
 
     def query(self) -> 'MongoDBModel':
         self.chained = False
         return self
 
-    def json(self) -> Union[List[dict], dict]:
+    def json(self) -> List[dict] | dict:
         if self._result is None:
             raise ChainingError(message='you can not call json directly, it needs to be chained')
         if isinstance(self._result, Cursor):
             return [Helper.standardize_dict(item, underscore=True) for item in list(self._result)]
         else:
             return Helper.standardize_dict(self._result, underscore=True)
```

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm/interfaces/mongodb_model_events.py` & `mongodb_orm-0.0.130/mongodb_orm/interfaces/mongodb_model_events.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.0.130/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm/types/model_schema.py` & `mongodb_orm-0.0.130/mongodb_orm/types/model_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     properties: Optional[Dict[str, 'PropertySchema']]  # Optional
 
 
 class ModelSchema(TypedDict):
     bsonType: str
     title: Optional[str]  # Optional
     required: Optional[List[str]]  # Optional
-    properties: Dict[str, Union[PropertySchema, dict]]  # Optional
+    properties: Dict[str, PropertySchema | dict]  # Optional
```

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.130/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from pymongo.results import InsertOneResult
 from rest_framework.response import Response
 from rest_framework.decorators import action
 from rest_framework.viewsets import ViewSet
 from ..interfaces.mongodb_model import MongoDBModel
-from ..utils.helpers import Helper
 
 
 class MongoDBAPIModelView(MongoDBModel, ViewSet):
 
     def list(self: MongoDBModel, request, *args, **kwargs) -> Response:
         MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
         page: int = request.query_params.get('page', 1)
@@ -43,32 +42,32 @@
         except Exception as e:
             return Response({'success': False, 'error': str(e)})
         return Response({'success': True, 'result': result.json()})
 
     def create(self, request, *args, **kwargs) -> Response:
         MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
         try:
-            new_record: InsertOneResult = MongoDBModel.post(self, Helper.standard_record(request.data))
+            new_record: InsertOneResult = MongoDBModel.post(self, request.data)
             retrieve_record: dict = MongoDBModel.get(self, pk=str(new_record.inserted_id)).json()
         except Exception as e:
             return Response({'success': False, 'error': str(e)})
         return Response({'success': True, 'record': retrieve_record})
 
     def update(self, request, *args, **kwargs) -> Response:
         MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
         try:
-            MongoDBModel.put(self, pk=str(kwargs.get('pk')), record=Helper.standard_record(request.data))
+            MongoDBModel.put(self, pk=str(kwargs.get('pk')), record=request.data)
         except Exception as e:
             return Response({'success': False, 'error': str(e)})
         return Response({'success': True})
 
     def partial_update(self, request, *args, **kwargs) -> Response:
         MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
         try:
-            MongoDBModel.patch(self, pk=str(kwargs.get('pk')), record=Helper.standard_record(request.data))
+            MongoDBModel.patch(self, pk=str(kwargs.get('pk')), record=request.data)
         except Exception as e:
             return Response({'success': False, 'error': str(e)})
         return Response({'success': True})
 
     def destroy(self, request, *args, **kwargs) -> Response:
         MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
         try:
```

### Comparing `mongodb_orm-0.0.129a7/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.130/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a7/setup.py` & `mongodb_orm-0.0.130/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.0.129-alpha.7",
+    version="0.0.130",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

