# Comparing `tmp/oarepo_global_search-1.0.5.tar.gz` & `tmp/oarepo_global_search-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo_global_search-1.0.5.tar", last modified: Fri May  3 07:45:48 2024, max compression
+gzip compressed data, was "oarepo_global_search-1.0.7.tar", last modified: Fri May 10 12:28:21 2024, max compression
```

## Comparing `oarepo_global_search-1.0.5.tar` & `oarepo_global_search-1.0.7.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/format.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.375393 oarepo_global_search-1.0.5/oarepo_global_search/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.375393 oarepo_global_search-1.0.5/oarepo_global_search/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/user_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.371393 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.371393 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/semantic-ui/global_search/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:42:53.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-03 07:45:48.383393 oarepo_global_search-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.140216 oarepo_global_search-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/format.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.132216 oarepo_global_search-1.0.7/oarepo_global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/user_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.132216 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.132216 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/semantic-ui/global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:25:10.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-10 12:28:21.140216 oarepo_global_search-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/setup.py
```

### Comparing `oarepo_global_search-1.0.5/MANIFEST.in` & `oarepo_global_search-1.0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/PKG-INFO` & `oarepo_global_search-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-global-search
-Version: 1.0.5
+Version: 1.0.7
 Summary: "A model builder plugin for global search"
 Home-page: https://github.com/oarepo/oarepo-global-search
 Author: Alzbeta Pokorna
 Author-email: Alzbeta.Pokorna@cesnet.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/ext.py` & `oarepo_global_search-1.0.7/oarepo_global_search/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/resources/records/config.py` & `oarepo_global_search-1.0.7/oarepo_global_search/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/resources/records/resource.py` & `oarepo_global_search-1.0.7/oarepo_global_search/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/services/records/params.py` & `oarepo_global_search-1.0.7/oarepo_global_search/services/records/params.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/services/records/results.py` & `oarepo_global_search-1.0.7/oarepo_global_search/services/records/results.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/services/records/service.py` & `oarepo_global_search-1.0.7/oarepo_global_search/services/records/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 
-from invenio_records_resources.records.api import Record
+# from invenio_records_resources.records.api import Record
+from .api import GlobalSearchRecord
 from invenio_records_resources.records.systemfields import IndexField
 from invenio_records_resources.services import RecordService as InvenioRecordService
 from invenio_records_resources.services import (
     RecordServiceConfig as InvenioRecordServiceConfig,
 )
 from invenio_records_resources.services import pagination_links
 from oarepo_runtime.services.config.service import PermissionsPresetsConfigMixin
@@ -27,33 +28,37 @@
     def indices(self):
         indices = []
         for s in current_global_search.model_services:
             indices.append(s.record_cls.index.search_alias)
         return indices
 
     @property
+    def indexer(self):
+        return None
+
+    @property
     def service_mapping(self):
         service_mapping = []
         for s in current_global_search.model_services:
             service_mapping.append({s: s.record_cls.schema.value})
         return service_mapping
 
     @property
     def config(self):
-        Record.index = IndexField(self.indices())
+        GlobalSearchRecord.index = IndexField(self.indices())
         GlobalSearchResultList.services = self.service_mapping
 
         config_class = type(
             "GlobalSearchServiceConfig",
             (PermissionsPresetsConfigMixin, InvenioRecordServiceConfig),
             {
                 "PERMISSIONS_PRESETS": ["everyone"],
                 "base_permission_policy_cls": GlobalSearchPermissionPolicy,
                 "result_list_cls": GlobalSearchResultList,
-                "record_cls": Record,
+                "record_cls": GlobalSearchRecord,
                 "url_prefix": "/search",
                 "links_search": pagination_links("{+api}/search{?args*}"),
             },
         )
         return config_class()
 
     @config.setter
```

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/services/records/user_service.py` & `oarepo_global_search-1.0.7/oarepo_global_search/services/records/user_service.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/ui/config.py` & `oarepo_global_search-1.0.7/oarepo_global_search/ui/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/views/api.py` & `oarepo_global_search-1.0.7/oarepo_global_search/views/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,14 @@
     with app.app_context():
         # register service
         sregistry = app.extensions["invenio-records-resources"].registry
         sregistry.register(
             ext.service_records, service_id=ext.service_records.config.service_id
         )
 
-        # # Register indexer
-        # if hasattr(ext.service_records, "indexer"):
-        #     iregistry = app.extensions["invenio-indexer"].registry
-        #     iregistry.register(
-        #         ext.service_records.indexer,
-        #         indexer_id=ext.service_records.config.service_id,
-        #     )
+        # Register indexer
+        if hasattr(ext.service_records, "indexer"):
+            iregistry = app.extensions["invenio-indexer"].registry
+            iregistry.register(
+                ext.service_records.indexer,
+                indexer_id=ext.service_records.config.service_id,
+            )
```

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search/views/app.py` & `oarepo_global_search-1.0.7/oarepo_global_search/views/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     with app.app_context():
         # register service
         sregistry = app.extensions["invenio-records-resources"].registry
         sregistry.register(
             ext.service_records, service_id=ext.service_records.config.service_id
         )
 
-        # # Register indexer
-        # if hasattr(ext.service_records, "indexer"):
-        #     iregistry = app.extensions["invenio-indexer"].registry
-        #     iregistry.register(
-        #         ext.service_records.indexer,
-        #         indexer_id=ext.service_records.config.service_id,
-        #     )
+        # Register indexer
+        if hasattr(ext.service_records, "indexer"):
+            iregistry = app.extensions["invenio-indexer"].registry
+            iregistry.register(
+                ext.service_records.indexer,
+                indexer_id=ext.service_records.config.service_id,
+            )
```

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search.egg-info/PKG-INFO` & `oarepo_global_search-1.0.7/oarepo_global_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-global-search
-Version: 1.0.5
+Version: 1.0.7
 Summary: "A model builder plugin for global search"
 Home-page: https://github.com/oarepo/oarepo-global-search
 Author: Alzbeta Pokorna
 Author-email: Alzbeta.Pokorna@cesnet.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search.egg-info/SOURCES.txt` & `oarepo_global_search-1.0.7/oarepo_global_search.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 oarepo_global_search.egg-info/top_level.txt
 oarepo_global_search/resources/__init__.py
 oarepo_global_search/resources/records/__init__.py
 oarepo_global_search/resources/records/config.py
 oarepo_global_search/resources/records/resource.py
 oarepo_global_search/services/__init__.py
 oarepo_global_search/services/records/__init__.py
+oarepo_global_search/services/records/api.py
 oarepo_global_search/services/records/params.py
 oarepo_global_search/services/records/permissions.py
 oarepo_global_search/services/records/results.py
 oarepo_global_search/services/records/service.py
 oarepo_global_search/services/records/user_service.py
 oarepo_global_search/ui/__init__.py
 oarepo_global_search/ui/config.py
```

### Comparing `oarepo_global_search-1.0.5/oarepo_global_search.egg-info/entry_points.txt` & `oarepo_global_search-1.0.7/oarepo_global_search.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/run-tests.sh` & `oarepo_global_search-1.0.7/run-tests.sh`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.5/setup.cfg` & `oarepo_global_search-1.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = oarepo-global-search
-version = 1.0.5
+version = 1.0.7
 description = "A model builder plugin for global search"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio relations model builder
 license = MIT
 author = Alzbeta Pokorna
 author_email = Alzbeta.Pokorna@cesnet.cz
 platforms = any
 url = https://github.com/oarepo/oarepo-global-search
 classifiers = 
 	Development Status :: 3 - Alpha
 
 [options]
 packages = find:
+include_package_data = True
 python_requires = >=3.10
 zip_safe = False
 install_requires = 
 	oarepo-model-builder>=4.0.0
 	invenio_records_resources>=0.21.4
 	oarepo-ui
```

