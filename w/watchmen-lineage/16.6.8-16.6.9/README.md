# Comparing `tmp/watchmen_lineage-16.6.8.tar.gz` & `tmp/watchmen_lineage-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_lineage-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_lineage-16.6.9.tar", max compression
```

## Comparing `watchmen_lineage-16.6.8.tar` & `watchmen_lineage-16.6.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/LICENSE
--rw-r--r--   0        0        0       46 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/README.md
--rw-r--r--   0        0        0      633 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/__init__.py
--rw-r--r--   0        0        0     1371 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/index.py
--rw-r--r--   0        0        0      550 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/lineage_setting.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/ml/__init__.py
--rw-r--r--   0        0        0      911 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/ml/mapping_similar.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/model/__init__.py
--rw-r--r--   0        0        0      676 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/model/ast.py
--rw-r--r--   0        0        0     5521 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/model/lineage.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/router/__init__.py
--rw-r--r--   0        0        0     1564 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/router/lineage_router.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/__init__.py
--rw-r--r--   0        0        0     4777 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/graphic_builder.py
--rw-r--r--   0        0        0     1179 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/index.py
--rw-r--r--   0        0        0     5696 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/indicator_lineage.py
--rw-r--r--   0        0        0      581 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/loader.py
--rw-r--r--   0        0        0    10390 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/objective_lineage.py
--rw-r--r--   0        0        0     7469 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/pipeline_lineage.py
--rw-r--r--   0        0        0     6522 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/subject_lineage.py
--rw-r--r--   0        0        0     2896 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/topic_lineage.py
--rw-r--r--   0        0        0      291 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/compute_service.py
--rw-r--r--   0        0        0     1028 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/lineage_cache.py
--rw-r--r--   0        0        0    12852 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/lineage_service.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/memory/__init__.py
--rw-r--r--   0        0        0      141 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/memory/memory_compute_service.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/table/__init__.py
--rw-r--r--   0        0        0      140 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/service/table/table_compute_service.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/storage/__init__.py
--rw-r--r--   0        0        0      247 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/storage/lineage_storage.py
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/utils/__init__.py
--rw-r--r--   0        0        0     7971 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/utils/constant_utils.py
--rw-r--r--   0        0        0     1991 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/utils/id_utils.py
--rw-r--r--   0        0        0     1453 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/utils/size_utils.py
--rw-r--r--   0        0        0    11880 2024-01-08 07:58:02.512594 watchmen_lineage-16.6.8/src/watchmen_lineage/utils/utils.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 watchmen_lineage-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/LICENSE
+-rw-r--r--   0        0        0       46 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/README.md
+-rw-r--r--   0        0        0      633 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/__init__.py
+-rw-r--r--   0        0        0     1371 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/index.py
+-rw-r--r--   0        0        0      550 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/lineage_setting.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/ml/__init__.py
+-rw-r--r--   0        0        0      911 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/ml/mapping_similar.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/model/__init__.py
+-rw-r--r--   0        0        0      676 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/model/ast.py
+-rw-r--r--   0        0        0     5521 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/model/lineage.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/router/__init__.py
+-rw-r--r--   0        0        0     1564 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/router/lineage_router.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/__init__.py
+-rw-r--r--   0        0        0     4777 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/graphic_builder.py
+-rw-r--r--   0        0        0     1179 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/index.py
+-rw-r--r--   0        0        0     5696 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/indicator_lineage.py
+-rw-r--r--   0        0        0      581 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/loader.py
+-rw-r--r--   0        0        0    10390 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/objective_lineage.py
+-rw-r--r--   0        0        0     7469 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/pipeline_lineage.py
+-rw-r--r--   0        0        0     6522 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/subject_lineage.py
+-rw-r--r--   0        0        0     2896 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/topic_lineage.py
+-rw-r--r--   0        0        0      291 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/compute_service.py
+-rw-r--r--   0        0        0     1028 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/lineage_cache.py
+-rw-r--r--   0        0        0    12852 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/lineage_service.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/memory/__init__.py
+-rw-r--r--   0        0        0      141 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/memory/memory_compute_service.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/table/__init__.py
+-rw-r--r--   0        0        0      140 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/service/table/table_compute_service.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/storage/__init__.py
+-rw-r--r--   0        0        0      247 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/storage/lineage_storage.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/utils/__init__.py
+-rw-r--r--   0        0        0     7971 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/utils/constant_utils.py
+-rw-r--r--   0        0        0     1991 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/utils/id_utils.py
+-rw-r--r--   0        0        0     1453 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/utils/size_utils.py
+-rw-r--r--   0        0        0    11880 2024-02-01 01:32:37.247323 watchmen_lineage-16.6.9/src/watchmen_lineage/utils/utils.py
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 watchmen_lineage-16.6.9/PKG-INFO
```

### Comparing `watchmen_lineage-16.6.8/LICENSE` & `watchmen_lineage-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/pyproject.toml` & `watchmen_lineage-16.6.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "watchmen-lineage"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["luke0623 <luke0623@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "watchmen_lineage", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-surface = "16.6.8"
-watchmen-pipeline-surface = "16.6.8"
-watchmen-inquiry-surface = "16.6.8"
-watchmen-inquiry-trino = { version = "16.6.8", optional = true }
-watchmen-indicator-surface = "16.6.8"
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
+watchmen-data-surface = "16.6.9"
+watchmen-pipeline-surface = "16.6.9"
+watchmen-inquiry-surface = "16.6.9"
+watchmen-inquiry-trino = { version = "16.6.9", optional = true }
+watchmen-indicator-surface = "16.6.9"
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
 networkx = "^2.8.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/index.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/index.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/lineage_setting.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/lineage_setting.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/ml/mapping_similar.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/ml/mapping_similar.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/model/ast.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/model/ast.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/model/lineage.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/model/lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/router/lineage_router.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/router/lineage_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/graphic_builder.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/graphic_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/index.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/index.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/indicator_lineage.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/indicator_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/loader.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/loader.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/objective_lineage.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/objective_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/pipeline_lineage.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/pipeline_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/subject_lineage.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/subject_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/builder/topic_lineage.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/builder/topic_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/lineage_cache.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/lineage_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/service/lineage_service.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/service/lineage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/utils/constant_utils.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/utils/constant_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/utils/id_utils.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/utils/id_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/utils/size_utils.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/utils/size_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/src/watchmen_lineage/utils/utils.py` & `watchmen_lineage-16.6.9/src/watchmen_lineage/utils/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.6.8/PKG-INFO` & `watchmen_lineage-16.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: watchmen-lineage
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 Author: luke0623
 Author-email: luke0623@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: networkx (>=2.8.8,<3.0.0)
-Requires-Dist: watchmen-data-surface (==16.6.8)
-Requires-Dist: watchmen-indicator-surface (==16.6.8)
-Requires-Dist: watchmen-inquiry-surface (==16.6.8)
-Requires-Dist: watchmen-inquiry-trino (==16.6.8)
-Requires-Dist: watchmen-pipeline-surface (==16.6.8)
-Requires-Dist: watchmen-storage-mysql (==16.6.8)
+Requires-Dist: watchmen-data-surface (==16.6.9)
+Requires-Dist: watchmen-indicator-surface (==16.6.9)
+Requires-Dist: watchmen-inquiry-surface (==16.6.9)
+Requires-Dist: watchmen-inquiry-trino (==16.6.9)
+Requires-Dist: watchmen-pipeline-surface (==16.6.9)
+Requires-Dist: watchmen-storage-mysql (==16.6.9)
 Description-Content-Type: text/markdown
 
 # Watchmen Lineage
 
 Lineage of _**Watchmen**_.
```

