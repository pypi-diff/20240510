# Comparing `tmp/opengate_data-1.0.5.tar.gz` & `tmp/opengate_data-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengate_data-1.0.5.tar", last modified: Fri Apr 19 11:36:56 2024, max compression
+gzip compressed data, was "opengate_data-1.0.6.tar", last modified: Fri May 10 10:56:44 2024, max compression
```

## Comparing `opengate_data-1.0.5.tar` & `opengate_data-1.0.6.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/
--rw-r--r--   0 manuel    (1000) manuel    (1000)      974 2024-04-19 11:36:56.820613 opengate_data-1.0.5/PKG-INFO
--rw-r--r--   0 manuel    (1000) manuel    (1000)      549 2024-04-15 07:45:27.000000 opengate_data-1.0.5/README.md
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.812613 opengate_data-1.0.5/opengate_data/
--rw-r--r--   0 manuel    (1000) manuel    (1000)      249 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/__init__.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/ai_models/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/ai_models/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    15395 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/ai_models/ai_models.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/ai_pipelines/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/ai_pipelines/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    14795 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/ai_pipelines/ai_pipelines.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/ai_transformers/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/ai_transformers/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    16353 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/ai_transformers/ai_transformers.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/datapoints/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/datapoints/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     4492 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/datapoints/datapoints.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/datasets/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/datasets/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     3393 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/datasets/datasets.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/entities/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/entities/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     6978 2024-04-19 10:51:35.000000 opengate_data-1.0.5/opengate_data/entities/entities.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     4027 2024-04-19 10:57:54.000000 opengate_data-1.0.5/opengate_data/opengate_client.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/operations/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/operations/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     3085 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/operations/operations.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/provision_processor/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 13:58:53.000000 opengate_data-1.0.5/opengate_data/provision_processor/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     6205 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/provision_processor/provision_processor.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/rules/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/rules/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    18199 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/rules/rules.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/test/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/test/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)      525 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/test/ownworld.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    12881 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/test/test_steps_cucumber.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/timeseries/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/timeseries/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     3342 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/timeseries/timeseries.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data.egg-info/
--rw-r--r--   0 manuel    (1000) manuel    (1000)      974 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/PKG-INFO
--rw-r--r--   0 manuel    (1000) manuel    (1000)     1143 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/SOURCES.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)        1 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/dependency_links.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)       88 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/requires.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)       14 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/top_level.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)       38 2024-04-19 11:36:56.820613 opengate_data-1.0.5/setup.cfg
--rw-r--r--   0 manuel    (1000) manuel    (1000)      793 2024-04-19 10:28:57.000000 opengate_data-1.0.5/setup.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.152010 opengate_data-1.0.6/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     1022 2024-05-10 10:56:44.152010 opengate_data-1.0.6/PKG-INFO
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      549 2024-04-15 07:45:27.000000 opengate_data-1.0.6/README.md
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.140009 opengate_data-1.0.6/opengate_data/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      296 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.144009 opengate_data-1.0.6/opengate_data/ai_models/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/ai_models/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    15395 2024-05-10 10:43:50.000000 opengate_data-1.0.6/opengate_data/ai_models/ai_models.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.144009 opengate_data-1.0.6/opengate_data/ai_pipelines/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/ai_pipelines/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    14795 2024-05-10 10:43:53.000000 opengate_data-1.0.6/opengate_data/ai_pipelines/ai_pipelines.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.144009 opengate_data-1.0.6/opengate_data/ai_transformers/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/ai_transformers/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    16353 2024-05-10 10:43:56.000000 opengate_data-1.0.6/opengate_data/ai_transformers/ai_transformers.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.144009 opengate_data-1.0.6/opengate_data/collection/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      108 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/collection/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    16179 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/collection/iot_bulk_collection.py
+-rwxr-xr-x   0 manuel    (1000) manuel    (1000)    18179 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/collection/iot_collection.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.144009 opengate_data-1.0.6/opengate_data/datapoints/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/datapoints/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     4492 2024-05-10 10:44:49.000000 opengate_data-1.0.6/opengate_data/datapoints/datapoints.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.148009 opengate_data-1.0.6/opengate_data/datasets/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/datasets/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     3393 2024-04-19 12:03:56.000000 opengate_data-1.0.6/opengate_data/datasets/datasets.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.148009 opengate_data-1.0.6/opengate_data/entities/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/entities/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     8342 2024-05-10 10:53:11.000000 opengate_data-1.0.6/opengate_data/entities/entities.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     4585 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/opengate_client.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.148009 opengate_data-1.0.6/opengate_data/operations/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/operations/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     3085 2024-04-19 12:05:31.000000 opengate_data-1.0.6/opengate_data/operations/operations.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.148009 opengate_data-1.0.6/opengate_data/provision_processor/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 13:58:53.000000 opengate_data-1.0.6/opengate_data/provision_processor/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     6025 2024-05-10 10:53:11.000000 opengate_data-1.0.6/opengate_data/provision_processor/provision_processor.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.148009 opengate_data-1.0.6/opengate_data/rules/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/rules/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    18199 2024-04-19 12:03:56.000000 opengate_data-1.0.6/opengate_data/rules/rules.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.148009 opengate_data-1.0.6/opengate_data/test/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/test/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      661 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/test/ownworld.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    19457 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/test/test_steps_cucumber.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.152010 opengate_data-1.0.6/opengate_data/timeseries/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.6/opengate_data/timeseries/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     3342 2024-05-10 10:47:51.000000 opengate_data-1.0.6/opengate_data/timeseries/timeseries.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.152010 opengate_data-1.0.6/opengate_data/utils/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       62 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/utils/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     2619 2024-05-10 10:53:14.000000 opengate_data-1.0.6/opengate_data/utils/utils.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-05-10 10:56:44.152010 opengate_data-1.0.6/opengate_data.egg-info/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     1022 2024-05-10 10:56:44.000000 opengate_data-1.0.6/opengate_data.egg-info/PKG-INFO
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     1332 2024-05-10 10:56:44.000000 opengate_data-1.0.6/opengate_data.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        1 2024-05-10 10:56:44.000000 opengate_data-1.0.6/opengate_data.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       97 2024-05-10 10:56:44.000000 opengate_data-1.0.6/opengate_data.egg-info/requires.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       14 2024-05-10 10:56:44.000000 opengate_data-1.0.6/opengate_data.egg-info/top_level.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       38 2024-05-10 10:56:44.152010 opengate_data-1.0.6/setup.cfg
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      838 2024-05-10 10:53:14.000000 opengate_data-1.0.6/setup.py
```

### Comparing `opengate_data-1.0.5/PKG-INFO` & `opengate_data-1.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: opengate-data
-Version: 1.0.5
+Version: 1.0.6
 Summary: description
 Author: amplia soluciones
 Author-email: pipy@amplia.es
 License: Apache License 2.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: jsonpath_ng
 Requires-Dist: numpy
 Requires-Dist: urllib3
 Requires-Dist: configparser
 Requires-Dist: parse
 Requires-Dist: python-dotenv
+Requires-Dist: datetime
 Requires-Dist: flatten-dict
 
 # Opengate-data
 
 Opengate-data is a python library that helps you easily integrate OpenGate into your python projects.
 
 ## Installation
```

### Comparing `opengate_data-1.0.5/README.md` & `opengate_data-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/ai_models/ai_models.py` & `opengate_data-1.0.6/opengate_data/ai_models/ai_models.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/ai_pipelines/ai_pipelines.py` & `opengate_data-1.0.6/opengate_data/ai_pipelines/ai_pipelines.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/ai_transformers/ai_transformers.py` & `opengate_data-1.0.6/opengate_data/ai_transformers/ai_transformers.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/datapoints/datapoints.py` & `opengate_data-1.0.6/opengate_data/datapoints/datapoints.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/datasets/datasets.py` & `opengate_data-1.0.6/opengate_data/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/entities/entities.py` & `opengate_data-1.0.6/opengate_data/entities/entities.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,19 @@
         self.requires: Dict[str, Any] = {}
         self.headers: Dict[str, Any] = self.client.headers
 
     def with_filter(self, filter_data: Dict[str, Any]) -> 'EntitiesBuilder':
         ''' Body '''
         self.filter = filter_data
         return self
+      
+    def with_select(self, select_data: Dict[str, Any]) -> 'EntitiesBuilder':
+        ''' Select '''
+        self.select_data = select_data
+        return self
 
     def with_body(self, filter_data: Dict[str, Any]) -> 'EntitiesBuilder':
         ''' Body '''
         self.filter = filter_data
         return self
 
     def with_format(self, format_data: str) -> 'EntitiesBuilder':
@@ -64,25 +69,55 @@
 
     def with_case_sensitive(self) -> 'EntitiesBuilder':
         ''' case sensitive'''
         self.case_sensitive = True
         return self
 
     def search(self) -> 'EntitiesBuilder':
-        ''' searching '''
-        self.requires = {
-            'default sorted': self.default_sorted
-        }
+        """ searching """
+
         self.method = 'search'
         if self.format_data == "pandas":
             self.flatten = False
 
         self.url = f'{self.client.url}/north/v80/search/entities?flattened={self.flatten}&utc={self.utc}&summary={self.summary}&defaultSorted={self.default_sorted}&caseSensitive={self.case_sensitive}'
         print("url", self.url)
         return self
+    
+    def with_organization_name(self, organization_name: str) -> 'EntitiesBuilder':
+        ''' organization_name '''
+        self.organization_name = organization_name
+        return self
+    
+    def with_bulk_action(self, bulk_action: str) -> 'EntitiesBuilder':
+        ''' bulk_action '''
+        self.bulk_action = bulk_action
+        return self
+    
+    def with_bulk_type(self, bulk_type: str) -> 'EntitiesBuilder':
+        ''' bulk_type '''
+        self.bulk_type = bulk_type
+        return self
+    
+    def with_csv_data(self, csv_data: str) -> 'EntitiesBuilder':
+        ''' csv_data '''
+        self.csv_data = csv_data
+        return self
+    
+    def bulk_provisioning(self) -> 'EntitiesBuilder':
+        ''' bulk provisioning '''
+        self.requires = {
+            'organization_name': self.organization_name,
+            'action': self.bulk_action,
+            'type': self.bulk_type,
+            'data': self.csv_data
+        }
+        self.method = 'bulk_provisioning'
+        self.url = f'{self.client.url}/north/v80/provision/organizations/{self.organization_name}/bulk/async?action={self.bulk_action}&type={self.bulk_type}'
+        return self
 
     def with_organization_name(self, organization_name: str) -> 'EntitiesBuilder':
         ''' organization_name '''
         self.organization_name = organization_name
         return self
 
     def with_bulk_action(self, bulk_action: str) -> 'EntitiesBuilder':
@@ -125,14 +160,17 @@
             'search': self._execute_searching,
             'bulk_provisioning': self._execute_bulk_provisioning
         }
         function = methods.get(self.method)
         if function is None:
             raise ValueError(f'Unsupported method: {self.method}')
         return function()
+      
+    def add_header(self, key: str, value: str) -> 'EntitiesBuilder':
+        self.headers[key] = value
 
     def _execute_searching(self) -> Union[int, List[Dict[str, Any]]]:
         response = self._send_request()
         if response.status_code == 200:
             if self.format_data == 'csv':
                 return response.text
             else:
```

### Comparing `opengate_data-1.0.5/opengate_data/opengate_client.py` & `opengate_data-1.0.6/opengate_data/opengate_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-''' Class representing the OpenGateClient '''
+""" Class representing the OpenGateClient """
 
-from typing import Dict, Optional
+import openpyxl
 import requests
+from datetime import datetime
+from urllib3.exceptions import InsecureRequestWarning
+from urllib3 import disable_warnings
 from .datapoints.datapoints import DataPointsBuilder
 from .datasets.datasets import DataSetsBuilder
 from .timeseries.timeseries import TimeSeriesBuilder
 from .entities.entities import EntitiesBuilder
 from .provision_processor.provision_processor import ProvisionProcessorBuilder
 from .operations.operations import OperationsBuilder
 from .ai_models.ai_models import AIModelsBuilder
 from .ai_pipelines.ai_pipelines import AIPipelinesBuilder
 from .ai_transformers.ai_transformers import AITransformersBuilder
 from .rules.rules import RulesBuilder
+from .collection.iot_collection import IotCollectionBuilder
+from .collection.iot_bulk_collection import IotBulkCollectionBuilder
+
 
 class OpenGateClient:
-    ''' Class representing the OpenGateClient '''
-    def __init__(self, url: str = None, user: Optional[str] = None, password: Optional[str] = None, api_key: Optional[str] = None) -> None:
+    """ Class representing the OpenGateClient """
+
+    def __init__(self, url: str | None = None, user: str | None = None, password: str | None = None,
+                 api_key: str | None = None) -> None:
         self.url: str = url
-        self.user: Optional[str] = user
-        self.password: Optional[str] = password
-        self.api_key: Optional[str] = api_key
-        self.headers: Dict[str, str] = {}
+        self.user: str = user
+        self.password: str | None = password
+        self.api_key: str | None = api_key
+        self.headers: dict[str, str] = {}
         self.client: OpenGateClient = self
-        requests.packages.urllib3.disable_warnings()
+        self.entity_type: str | None = None
+        disable_warnings(InsecureRequestWarning)
 
         if not url:
             raise ValueError('You have not provided a URL')
 
         if user and password:
             data_user = {
                 'email': self.user,
@@ -50,47 +59,55 @@
                 raise requests.exceptions.RequestException(f'Connection failed: {error}')
         elif api_key:
             self.headers.update({
                 'X-ApiKey': self.api_key
             })
         else:
             raise ValueError('You have not provided an API key or user and password')
-               
+
     def data_sets(self) -> DataSetsBuilder:
-        ''' Represents the builder of datasets '''
+        """ Represents the builder of datasets """
         return DataSetsBuilder(self)
-    
+
     def timeseries(self) -> TimeSeriesBuilder:
-        ''' Represents the builder of timeseries '''
+        """ Represents the builder of timeseries """
         return TimeSeriesBuilder(self)
-    
+
     def entities(self) -> EntitiesBuilder:
-        ''' Represents the builder of entities '''
+        """ Represents the builder of entities """
         return EntitiesBuilder(self)
-    
+
     def provision_processor(self) -> ProvisionProcessorBuilder:
-        ''' Represents the builder of provision processors '''
+        """ Represents the builder of provision processors """
         return ProvisionProcessorBuilder(self)
-    
+
     def operations(self) -> OperationsBuilder:
-        ''' Represents the builder of operations '''
+        """ Represents the builder of operations """
         return OperationsBuilder(self)
-    
+
     def data_points_builder(self) -> DataPointsBuilder:
-        ''' Represents the builder of datapoints '''
+        """ Represents the builder of datapoints """
         return DataPointsBuilder(self)
-    
+
     def ai_models_builder(self) -> AIModelsBuilder:
-        ''' Represents the builder of artificial intelligence models '''
+        """ Represents the builder of artificial intelligence models """
         return AIModelsBuilder(self)
 
     def ai_pipelines_builder(self) -> AIPipelinesBuilder:
-        ''' Represents the builder of artificial intelligence models '''
+        """ Represents the builder of artificial intelligence models """
         return AIPipelinesBuilder(self)
-    
+
     def ai_transformers_builder(self) -> AITransformersBuilder:
-        ''' Represents the builder of artificial intelligence models '''
+        """ Represents the builder of artificial intelligence models """
         return AITransformersBuilder(self)
-    
+
     def rules_builder(self) -> RulesBuilder:
-        ''' Represents the builder of artificial intelligence models '''
+        """ Represents the builder rules """
         return RulesBuilder(self)
+
+    def new_iot_collection_builder(self) -> IotCollectionBuilder:
+        """ Represents the builder iot collection builder """
+        return IotCollectionBuilder(self)
+
+    def new_iot_bulk_collection_builder(self) -> IotBulkCollectionBuilder:
+        """ Represents the builder iot bulk collection builder """
+        return IotBulkCollectionBuilder(self)
```

### Comparing `opengate_data-1.0.5/opengate_data/operations/operations.py` & `opengate_data-1.0.6/opengate_data/operations/operations.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/provision_processor/provision_processor.py` & `opengate_data-1.0.6/opengate_data/provision_processor/provision_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,54 +54,50 @@
         ''' bulk_provision_processor '''
         self.requires = {
             'organization_name': self.organization_name,
             'provision_processor_id': self.provision_processor_id,
             'bulk_file': self.bulk_file
         }
         self.method = 'bulk_provision_processor'
-        self.headers['Accept'] = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}/{self.provision_processor_id}/bulk'
         return self
     
         
     def search_by_name(self) -> 'ProvisionProcessorBuilder':
         ''' search_provision_processor '''
         self.requires = {
             'organization_name': self.organization_name,
             'provision_processor_name': self.provision_processor_name,
             
         }
         self.method = 'search_provision_processor'
-        self.headers['Accept'] = 'application/json'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}'
         return self
     
         
     def bulk_status(self) -> 'ProvisionProcessorBuilder':
         ''' bulk_status '''
         self.requires = {
             'organization_name': self.organization_name,
             'bulk_process_id': self.bulk_process_id,
             
         }
         self.method = 'bulk_status'
-        self.headers['Accept'] = 'application/json'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}/bulk/{self.bulk_process_id}'
         return self
     
         
     def bulk_details(self) -> 'ProvisionProcessorBuilder':
         ''' bulk_details '''
         self.requires = {
             'organization_name': self.organization_name,
             'bulk_process_id': self.bulk_process_id,
             
         }
         self.method = 'bulk_details'
-        self.headers['Accept'] = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}/bulk/{self.bulk_process_id}/details'
         return self
     
     def build(self) -> 'ProvisionProcessorBuilder':
         ''' Check if any parameter is missing. '''
         if self.requires is not None:
             for key, value in self.requires.items():
@@ -117,14 +113,19 @@
             'bulk_status': self._execute_bulk_status,
             'bulk_details': self._execute_bulk_details,
         }
         function = methods.get(self.method)
         if function is None:
             raise ValueError(f'Unsupported method: {self.method}')
         return function()
+    
+      
+    def add_header(self, key: str, value: str) -> 'ProvisionProcessorBuilder':
+        self.headers[key] = value
+
 
     def _execute_bulk(self) -> Union[int, List[Dict[str, Any]]]:
         return requests.post(self.url, headers=self.headers, files=self.bulk_file, verify=False, timeout=3000)
 
 
     def _execute_searching(self) -> Union[int, List[Dict[str, Any]]]:
         request_response = requests.get(self.url, headers=self.headers, verify=False, timeout=3000)
```

### Comparing `opengate_data-1.0.5/opengate_data/rules/rules.py` & `opengate_data-1.0.6/opengate_data/rules/rules.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data/timeseries/timeseries.py` & `opengate_data-1.0.6/opengate_data/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `opengate_data-1.0.5/opengate_data.egg-info/PKG-INFO` & `opengate_data-1.0.6/opengate_data.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: opengate-data
-Version: 1.0.5
+Version: 1.0.6
 Summary: description
 Author: amplia soluciones
 Author-email: pipy@amplia.es
 License: Apache License 2.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: jsonpath_ng
 Requires-Dist: numpy
 Requires-Dist: urllib3
 Requires-Dist: configparser
 Requires-Dist: parse
 Requires-Dist: python-dotenv
+Requires-Dist: datetime
 Requires-Dist: flatten-dict
 
 # Opengate-data
 
 Opengate-data is a python library that helps you easily integrate OpenGate into your python projects.
 
 ## Installation
```

### Comparing `opengate_data-1.0.5/opengate_data.egg-info/SOURCES.txt` & `opengate_data-1.0.6/opengate_data.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 opengate_data.egg-info/top_level.txt
 opengate_data/ai_models/__init__.py
 opengate_data/ai_models/ai_models.py
 opengate_data/ai_pipelines/__init__.py
 opengate_data/ai_pipelines/ai_pipelines.py
 opengate_data/ai_transformers/__init__.py
 opengate_data/ai_transformers/ai_transformers.py
+opengate_data/collection/__init__.py
+opengate_data/collection/iot_bulk_collection.py
+opengate_data/collection/iot_collection.py
 opengate_data/datapoints/__init__.py
 opengate_data/datapoints/datapoints.py
 opengate_data/datasets/__init__.py
 opengate_data/datasets/datasets.py
 opengate_data/entities/__init__.py
 opengate_data/entities/entities.py
 opengate_data/operations/__init__.py
@@ -25,8 +28,10 @@
 opengate_data/provision_processor/provision_processor.py
 opengate_data/rules/__init__.py
 opengate_data/rules/rules.py
 opengate_data/test/__init__.py
 opengate_data/test/ownworld.py
 opengate_data/test/test_steps_cucumber.py
 opengate_data/timeseries/__init__.py
-opengate_data/timeseries/timeseries.py
+opengate_data/timeseries/timeseries.py
+opengate_data/utils/__init__.py
+opengate_data/utils/utils.py
```

### Comparing `opengate_data-1.0.5/setup.py` & `opengate_data-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
-
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 PACKAGE_NAME = 'opengate-data'
 AUTHOR = 'amplia soluciones'
 AUTHOR_EMAIL = 'pipy@amplia.es'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'description'
 
@@ -16,23 +15,25 @@
     'requests',
     'jsonpath_ng',
     'numpy',
     'urllib3',
     'configparser',
     'parse',
     'python-dotenv',
+    'datetime',
     'flatten-dict'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     install_requires=INSTALL_REQUIRES,
     license=LICENSE,
     packages=find_packages(),
+    python_requires='>=3.10',
     include_package_data=True,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
 )
```

