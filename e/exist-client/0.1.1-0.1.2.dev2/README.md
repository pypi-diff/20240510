# Comparing `tmp/exist_client-0.1.1.tar.gz` & `tmp/exist_client-0.1.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exist_client-0.1.1.tar", max compression
+gzip compressed data, was "exist_client-0.1.2.dev2.tar", max compression
```

## Comparing `exist_client-0.1.1.tar` & `exist_client-0.1.2.dev2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      105 2024-01-20 19:08:04.727727 exist_client-0.1.1/README.md
--rw-r--r--   0        0        0     1675 2024-01-20 19:08:23.767664 exist_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       59 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/__init__.py
--rw-r--r--   0        0        0      152 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/__init__.py
--rw-r--r--   0        0        0       47 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/__init__.py
--rw-r--r--   0        0        0     3450 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/access_token.py
--rw-r--r--   0        0        0     3075 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/accounts_profile.py
--rw-r--r--   0        0        0     4364 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attribute_values_get.py
--rw-r--r--   0        0        0     4732 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attributes_acquire.py
--rw-r--r--   0        0        0     8044 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attributes_get.py
--rw-r--r--   0        0        0     4188 2024-01-20 19:08:04.727727 exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attributes_update.py
--rw-r--r--   0        0        0    12209 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/client.py
--rw-r--r--   0        0        0      492 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/errors.py
--rw-r--r--   0        0        0     1501 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/__init__.py
--rw-r--r--   0        0        0     2066 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/access_token_data.py
--rw-r--r--   0        0        0     2455 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute.py
--rw-r--r--   0        0        0     1440 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_by_name.py
--rw-r--r--   0        0        0     1500 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_by_template.py
--rw-r--r--   0        0        0     1584 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_group.py
--rw-r--r--   0        0        0     1952 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_value.py
--rw-r--r--   0        0        0     2520 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_values_get_result.py
--rw-r--r--   0        0        0     3028 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_acquire_result.py
--rw-r--r--   0        0        0     1890 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_acquire_result_failed_item.py
--rw-r--r--   0        0        0     1541 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_acquire_result_success_item.py
--rw-r--r--   0        0        0     2490 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_get_result.py
--rw-r--r--   0        0        0     2798 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_update_result.py
--rw-r--r--   0        0        0     2405 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_update_result_failed_item.py
--rw-r--r--   0        0        0     1784 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/date_value.py
--rw-r--r--   0        0        0     1624 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/error_mixin.py
--rw-r--r--   0        0        0     1839 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/paginated_response.py
--rw-r--r--   0        0        0     2257 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/tokens.py
--rw-r--r--   0        0        0     1457 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/models/user_profile.py
--rw-r--r--   0        0        0      968 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/_exist_io_client/types.py
--rw-r--r--   0        0        0     2678 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/client.py
--rw-r--r--   0        0        0      106 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/models.py
--rw-r--r--   0        0        0        0 2024-01-20 19:08:04.731727 exist_client-0.1.1/src/exist_client/py.typed
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 exist_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      105 2024-05-10 12:08:06.210901 exist_client-0.1.2.dev2/README.md
+-rw-r--r--   0        0        0     1680 2024-05-10 12:08:46.034785 exist_client-0.1.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/__init__.py
+-rw-r--r--   0        0        0     3450 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/access_token.py
+-rw-r--r--   0        0        0     3075 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/accounts_profile.py
+-rw-r--r--   0        0        0     4364 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attribute_values_get.py
+-rw-r--r--   0        0        0     4732 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attributes_acquire.py
+-rw-r--r--   0        0        0     8044 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attributes_get.py
+-rw-r--r--   0        0        0     4188 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attributes_update.py
+-rw-r--r--   0        0        0    12209 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/client.py
+-rw-r--r--   0        0        0      492 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/errors.py
+-rw-r--r--   0        0        0     1501 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/access_token_data.py
+-rw-r--r--   0        0        0     2455 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute.py
+-rw-r--r--   0        0        0     1440 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_by_name.py
+-rw-r--r--   0        0        0     1500 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_by_template.py
+-rw-r--r--   0        0        0     1584 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_group.py
+-rw-r--r--   0        0        0     1952 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_value.py
+-rw-r--r--   0        0        0     2520 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_values_get_result.py
+-rw-r--r--   0        0        0     3028 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_acquire_result.py
+-rw-r--r--   0        0        0     1890 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_acquire_result_failed_item.py
+-rw-r--r--   0        0        0     1541 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_acquire_result_success_item.py
+-rw-r--r--   0        0        0     2490 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_get_result.py
+-rw-r--r--   0        0        0     2798 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_update_result.py
+-rw-r--r--   0        0        0     2405 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_update_result_failed_item.py
+-rw-r--r--   0        0        0     1784 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/date_value.py
+-rw-r--r--   0        0        0     1624 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/error_mixin.py
+-rw-r--r--   0        0        0     1839 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/paginated_response.py
+-rw-r--r--   0        0        0     2257 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/tokens.py
+-rw-r--r--   0        0        0     1457 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/user_profile.py
+-rw-r--r--   0        0        0      968 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/types.py
+-rw-r--r--   0        0        0     2704 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/client.py
+-rw-r--r--   0        0        0      106 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/models.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:08:06.214901 exist_client-0.1.2.dev2/src/exist_client/py.typed
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 exist_client-0.1.2.dev2/PKG-INFO
```

### Comparing `exist_client-0.1.1/pyproject.toml` & `exist_client-0.1.2.dev2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exist-client"
-version = "0.1.1"
+version = "0.1.2.dev2"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "exist_client", from = "src"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/access_token.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/access_token.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/accounts_profile.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/accounts_profile.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attribute_values_get.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attribute_values_get.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attributes_acquire.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attributes_acquire.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attributes_get.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attributes_get.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/api/default/attributes_update.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/api/default/attributes_update.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/client.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/client.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/__init__.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/access_token_data.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/access_token_data.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_by_name.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_by_name.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_by_template.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_by_template.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_group.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_group.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_value.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_value.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attribute_values_get_result.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attribute_values_get_result.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_acquire_result.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_acquire_result.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_acquire_result_failed_item.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_acquire_result_failed_item.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_acquire_result_success_item.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_acquire_result_success_item.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_get_result.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_get_result.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_update_result.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_update_result.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/attributes_update_result_failed_item.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/attributes_update_result_failed_item.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/date_value.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/date_value.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/error_mixin.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/error_mixin.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/paginated_response.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/paginated_response.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/tokens.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/tokens.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/models/user_profile.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/_exist_io_client/types.py` & `exist_client-0.1.2.dev2/src/exist_client/_exist_io_client/types.py`

 * *Files identical despite different names*

### Comparing `exist_client-0.1.1/src/exist_client/client.py` & `exist_client-0.1.2.dev2/src/exist_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     next_: Optional[str]
 
 
 PaginatedApi = Callable[..., Optional[PaginatedResponse[T]]]
 
 
 class ExistClient:
-    def __init__(self, *, token: str):
+    def __init__(self, *, token: str, base_url: str = EXIST_IO_BASE_URL):
         self.client = AuthenticatedClient(
-            EXIST_IO_BASE_URL,
+            base_url,
             token,
             raise_on_unexpected_status=True,
             follow_redirects=True,
         )
 
     def get_profile(self) -> Optional[UserProfile]:
         return accounts_profile.sync(client=self.client)
```

### Comparing `exist_client-0.1.1/PKG-INFO` & `exist_client-0.1.2.dev2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exist-client
-Version: 0.1.1
+Version: 0.1.2.dev2
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

