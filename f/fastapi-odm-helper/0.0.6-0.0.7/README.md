# Comparing `tmp/fastapi_odm_helper-0.0.6.tar.gz` & `tmp/fastapi_odm_helper-0.0.7.tar.gz`

## Comparing `fastapi_odm_helper-0.0.6.tar` & `fastapi_odm_helper-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/build_and_publish.sh
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/build_and_test.sh
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/tox.ini
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/fastapi_odm_helper/__init__.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/fastapi_odm_helper/decorators/entity.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/fastapi_odm_helper/dependencies/pagination.py
--rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/fastapi_odm_helper/repositories/base.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/fastapi_odm_helper/responses/pagination.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/LICENSE
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/build_and_publish.sh
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/build_and_test.sh
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/tox.ini
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/fastapi_odm_helper/__init__.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/fastapi_odm_helper/decorators/entity.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/fastapi_odm_helper/dependencies/pagination.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/fastapi_odm_helper/repositories/base.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/fastapi_odm_helper/responses/pagination.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/LICENSE
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fastapi_odm_helper-0.0.7/PKG-INFO
```

### Comparing `fastapi_odm_helper-0.0.6/.github/workflows/publish.yaml` & `fastapi_odm_helper-0.0.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_odm_helper-0.0.6/fastapi_odm_helper/decorators/entity.py` & `fastapi_odm_helper-0.0.7/fastapi_odm_helper/decorators/entity.py`

 * *Files identical despite different names*

### Comparing `fastapi_odm_helper-0.0.6/fastapi_odm_helper/repositories/base.py` & `fastapi_odm_helper-0.0.7/fastapi_odm_helper/repositories/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,16 +187,16 @@
         await self.update(data, *criterion)
 
         return await self.find_one(*criterion)
 
     async def paginate(self, *criterion, pagination_params: PaginationParams) -> PaginationResponse[T]:
         page = pagination_params.page
         per_page = pagination_params.per_page
-
-        items = await self.skip(page - 1).limit(per_page).find(*criterion)
+        skip_count = (page - 1) * per_page
+        items = await self.skip(skip_count).limit(per_page).find(*criterion)
         total = await self.count(*criterion)
 
         return {'items': items, 'total': total, 'page': page, 'size': per_page}
 
     def raise_not_found(self):
         raise EntityNotFoundException(self._entity)
```

### Comparing `fastapi_odm_helper-0.0.6/.gitignore` & `fastapi_odm_helper-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_odm_helper-0.0.6/LICENSE` & `fastapi_odm_helper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_odm_helper-0.0.6/pyproject.toml` & `fastapi_odm_helper-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_odm_helper"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Dzung Nguyen", email="dung@megatron-solutions.com" },
 ]
 description = "FastAPI ODM Helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_odm_helper-0.0.6/PKG-INFO` & `fastapi_odm_helper-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi_odm_helper
-Version: 0.0.6
+Version: 0.0.7
 Summary: FastAPI ODM Helper
 Project-URL: Homepage, https://github.com/megatron-global/fastapi-odm-helper
 Project-URL: Bug Tracker, https://github.com/megatron-global/fastapi-odm-helper/issues
 Author-email: Dzung Nguyen <dung@megatron-solutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

