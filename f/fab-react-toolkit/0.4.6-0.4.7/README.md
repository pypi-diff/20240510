# Comparing `tmp/fab_react_toolkit-0.4.6.tar.gz` & `tmp/fab_react_toolkit-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab_react_toolkit-0.4.6.tar", last modified: Wed May  8 11:13:43 2024, max compression
+gzip compressed data, was "fab_react_toolkit-0.4.7.tar", last modified: Fri May 10 12:09:45 2024, max compression
```

## Comparing `fab_react_toolkit-0.4.6.tar` & `fab_react_toolkit-0.4.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.347860 fab_react_toolkit-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.339860 fab_react_toolkit-0.4.6/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29193 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:13:43.347860 fab_react_toolkit-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:09:45.692305 fab_react_toolkit-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 12:09:45.692305 fab_react_toolkit-0.4.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:09:45.688305 fab_react_toolkit-0.4.7/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:09:45.688305 fab_react_toolkit-0.4.7/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:09:45.688305 fab_react_toolkit-0.4.7/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:09:45.692305 fab_react_toolkit-0.4.7/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    24059 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29193 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:09:45.692305 fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 12:09:45.000000 fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-10 12:09:45.000000 fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:09:45.000000 fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 12:09:45.000000 fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 12:09:45.000000 fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-10 12:09:35.000000 fab_react_toolkit-0.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:09:45.692305 fab_react_toolkit-0.4.7/setup.cfg
```

### Comparing `fab_react_toolkit-0.4.6/LICENSE` & `fab_react_toolkit-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/PKG-INFO` & `fab_react_toolkit-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.6
+Version: 0.4.7
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.6/example/app/__init__.py` & `fab_react_toolkit-0.4.7/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/example/app/apis.py` & `fab_react_toolkit-0.4.7/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/example/app/config.py` & `fab_react_toolkit-0.4.7/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/example/app/models.py` & `fab_react_toolkit-0.4.7/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/example/run.py` & `fab_react_toolkit-0.4.7/example/run.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit/__init__.py` & `fab_react_toolkit-0.4.7/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit/api/__init__.py` & `fab_react_toolkit-0.4.7/fab_react_toolkit/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import functools
+from inspect import isfunction
 import json
 import urllib
 from typing import Any, Callable, Optional, Dict
 import jsonschema
 import prison as prison
 from flask_appbuilder.api import BaseApi, ModelRestApi as FABModelRestApi, merge_response_func, expose, safe, rison, get_info_schema, get_item_schema
 from flask_appbuilder._compat import as_unicode
@@ -55,26 +56,27 @@
     Tuple,
     Type,
     TYPE_CHECKING,
     Union,
 )
 
 from flask_appbuilder.security.decorators import permission_name, protect
-from flask import  Response, request
+from flask import Response, request
 from flask_appbuilder.const import API_ADD_COLUMNS_RIS_KEY, API_ADD_TITLE_RIS_KEY, API_PERMISSIONS_RIS_KEY, \
     API_EDIT_COLUMNS_RIS_KEY, API_FILTERS_RIS_KEY, API_EDIT_TITLE_RIS_KEY, API_FILTERS_RES_KEY, \
     API_ORDER_COLUMNS_RIS_KEY, API_LABEL_COLUMNS_RIS_KEY, API_DESCRIPTION_COLUMNS_RIS_KEY, API_LIST_COLUMNS_RIS_KEY, \
     API_LIST_TITLE_RIS_KEY, API_URI_RIS_KEY
 from flask_appbuilder.api.schemas import get_list_schema
 from .convert import Model2SchemaConverter
 
 from copy import deepcopy
 
 ModelKeyType = Union[str, int]
 
+
 def better_rison(
         schema: Optional[Dict[str, Any]] = None
 ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
     """
     Use this decorator to parse URI *Rison* arguments to
     a python data structure, your method gets the data
     structure on kwargs['rison']. Response is HTTP 400
@@ -118,23 +120,25 @@
                         kwargs["rison"] = json.loads(value)
                     except Exception:
                         return self.response_400(
                             message="Not a valid rison/json argument"
                         )
             if schema:
                 try:
-                    jsonschema.validate(instance=kwargs["rison"], schema=schema)
+                    jsonschema.validate(
+                        instance=kwargs["rison"], schema=schema)
                 except jsonschema.ValidationError as e:
                     return self.response_400(message=f"Not a valid rison schema {e}")
             return f(self, *args, **kwargs)
 
         return functools.update_wrapper(wraps, f)
 
     return _rison
 
+
 class ModelRestApi(FABModelRestApi):
     allow_browser_login = True
     quick_filters = None
     filter_options = None
     search_model_schema = None
     search_query_rel_fields = None
     icon = "Table"
@@ -165,24 +169,29 @@
         if self.search_model_schema is None:
             self.search_model_schema = self.model2schemaconverter.convert(
                 self.search_columns,
                 nested=False,
                 parent_schema_name=self.search_model_schema_name,
             )
 
+        self._add_relation_column_order()
+        self._add_function_list_columns()
+
     def merge_relations_info(self, response, **kwargs):
         """
         Adds relationship information to the response
         :param response: The response object
         :param kwargs: api endpoint kwargs
         """
         relations = []
         for related_api in self.related_apis:
-            foreign_key = related_api.datamodel.get_related_fk(self.datamodel.obj)
-            relation_type = "rel_o_m" if related_api.datamodel.is_relation_many_to_one(foreign_key) else "rel_m_m"
+            foreign_key = related_api.datamodel.get_related_fk(
+                self.datamodel.obj)
+            relation_type = "rel_o_m" if related_api.datamodel.is_relation_many_to_one(
+                foreign_key) else "rel_m_m"
             relation = {
                 'name': related_api.list_title if related_api.list_title else self._prettify_name(
                     related_api.datamodel.model_name),
                 'foreign_key': foreign_key,
                 'type': relation_type,
                 "path": related_api.resource_name + '/' or type(related_api).__name__ + '/'}
 
@@ -296,17 +305,14 @@
             422:
               $ref: '#/components/responses/422'
             500:
               $ref: '#/components/responses/500'
         """
         return self.info_headless(**kwargs)
 
-
-
-
     @expose("/", methods=["GET"])
     @protect()
     @safe
     @permission_name("get")
     @better_rison(get_list_schema)
     @merge_response_func(FABModelRestApi.merge_order_columns, API_ORDER_COLUMNS_RIS_KEY)
     @merge_response_func(FABModelRestApi.merge_list_label_columns, API_LABEL_COLUMNS_RIS_KEY)
@@ -399,54 +405,54 @@
         return self.get_list_headless(**kwargs)
 
     @expose('/bulk/<string:handler>', methods=['POST'])
     @protect()
     @safe
     @permission_name('bulk')
     def post_bulk(self, handler, **kwargs: any) -> Response:
-            """
-            Perform a bulk operation for the specified handler.
+        """
+        Perform a bulk operation for the specified handler.
+
+        Args:
+            handler: The name of the handler to perform the bulk operation on.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            The response from the bulk operation.
+
+        """
+        id_list = request.get_json()
+        bulk_func = getattr(self, f"bulk_{handler}")
+        return bulk_func(id_list)
 
-            Args:
-                handler: The name of the handler to perform the bulk operation on.
-                **kwargs: Additional keyword arguments.
-
-            Returns:
-                The response from the bulk operation.
-
-            """
-            id_list = request.get_json()
-            bulk_func = getattr(self, f"bulk_{handler}")
-            return bulk_func(id_list)
-    
     @expose("/download", methods=["POST"])
     @protect(allow_browser_login=True)
     @safe
     @permission_name('download')
     def download(self):
         query_params = request.json.get("queryParams", "")
 
         query = self.datamodel.session.query(self.datamodel.obj)
 
-        
         self._filters.clear_filters()
 
         self._filters.rest_add_filters(query_params['filters'])
         filters = self._filters.get_joined_filters(self._base_filters)
 
         inner_filters = self.datamodel.get_inner_filters(filters)
         query = self.datamodel.apply_filters(query, inner_filters)
         result = query.yield_per(100)
 
-        response = Response(generate_report(result,self.list_columns, self.label_columns), mimetype='text/csv')
+        response = Response(generate_report(
+            result, self.list_columns, self.label_columns), mimetype='text/csv')
         response.headers['Content-Type'] = 'application/octet-stream'
-        response.headers['Content-Disposition'] = 'attachment; filename={name}.csv'.format(name='appbybu')
+        response.headers['Content-Disposition'] = 'attachment; filename={name}.csv'.format(
+            name='appbybu')
         return response
 
-
     @expose("/<pk>", methods=["GET"])
     @protect()
     @safe
     @permission_name("get")
     @rison(get_item_schema)
     @merge_response_func(FABModelRestApi.merge_show_label_columns, API_LABEL_COLUMNS_RIS_KEY)
     @merge_response_func(FABModelRestApi.merge_show_columns, API_SHOW_COLUMNS_RIS_KEY)
@@ -566,16 +572,15 @@
             404:
               $ref: '#/components/responses/404'
             422:
               $ref: '#/components/responses/422'
             500:
               $ref: '#/components/responses/500'
         """
-        return self.put_headless(pk)    
-
+        return self.put_headless(pk)
 
     @expose("/<pk>", methods=["DELETE"])
     @protect()
     @safe
     @permission_name("delete")
     def delete(self, pk: ModelKeyType) -> Response:
         """Delete item from Model
@@ -601,8 +606,51 @@
             404:
               $ref: '#/components/responses/404'
             422:
               $ref: '#/components/responses/422'
             500:
               $ref: '#/components/responses/500'
         """
-        return self.delete_headless(pk)
+        return self.delete_headless(pk)
+
+    def _add_relation_column_order(self, force=False) -> None:
+        """
+        Adds relation columns to the order_columns list if the order_columns list is the same as the default order_columns list.
+
+        Args:
+            force (bool, optional): If set to True, the relation columns will be added to the order_columns list regardless of the default order_columns list. Defaults to False.
+
+        Returns:
+            None
+        """
+        default_order_columns = self.datamodel.get_order_columns_list(
+            list_columns=self.list_columns)
+        set_default_order_columns = set(default_order_columns)
+        set_order_columns = set(self.order_columns)
+        if not set_default_order_columns == set_order_columns and not force:
+            return
+
+        order_relation_columns = [
+            f"{column}.id" for column in self.list_columns if self.datamodel.is_relation(column) and (self.datamodel.is_relation_many_to_one(column) or self.datamodel.is_relation_one_to_one(column))]
+        self.order_columns = self.order_columns + order_relation_columns
+
+    def _add_function_list_columns(self, force=False) -> None:
+        """
+        Adds function columns to the list_columns list if the list_columns list is the same as the default list_columns list.
+
+        Args:
+            force (bool, optional): If set to True, the function columns will be added to the list_columns list regardless of the default list_columns list. Defaults to False.
+
+        Returns:
+            None
+        """
+        default_columns = [x for x in self.datamodel.get_user_columns_list() if x not in self.list_exclude_columns
+                           ]
+        set_default_columns = set(default_columns)
+        set_list_columns = set(self.list_columns)
+        if not set_default_columns == set_list_columns and not force:
+            return
+
+        attrs = vars(self.datamodel.obj)
+        model_properties = [key for key, value in attrs.items(
+        ) if not key.startswith("_") and isfunction(value)]
+        self.list_columns = self.list_columns + model_properties
```

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit/api/convert.py` & `fab_react_toolkit-0.4.7/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit/api/utils.py` & `fab_react_toolkit-0.4.7/fab_react_toolkit/api/utils.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit/apis.py` & `fab_react_toolkit-0.4.7/fab_react_toolkit/apis.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit/filters.py` & `fab_react_toolkit-0.4.7/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit/views.py` & `fab_react_toolkit-0.4.7/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/PKG-INFO` & `fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.6
+Version: 0.4.7
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/SOURCES.txt` & `fab_react_toolkit-0.4.7/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.6/pyproject.toml` & `fab_react_toolkit-0.4.7/pyproject.toml`

 * *Files identical despite different names*

