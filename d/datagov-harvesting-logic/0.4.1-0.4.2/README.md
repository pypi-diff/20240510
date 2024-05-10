# Comparing `tmp/datagov_harvesting_logic-0.4.1.tar.gz` & `tmp/datagov_harvesting_logic-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.4.1.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.4.2.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.4.1.tar` & `datagov_harvesting_logic-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1878 2024-05-07 22:36:52.669434 datagov_harvesting_logic-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     5935 2024-05-07 22:36:52.669434 datagov_harvesting_logic-0.4.1/README.md
--rw-r--r--   0        0        0      164 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/__init__.py
--rw-r--r--   0        0        0     8369 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/ckan_utils.py
--rw-r--r--   0        0        0     2158 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/exceptions.py
--rw-r--r--   0        0        0    14138 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/logger_config.py
--rw-r--r--   0        0        0     4058 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/utils.py
--rw-r--r--   0        0        0     2275 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-05-10 20:27:44.878631 datagov_harvesting_logic-0.4.2/LICENSE.md
+-rw-r--r--   0        0        0     5935 2024-05-10 20:27:44.878631 datagov_harvesting_logic-0.4.2/README.md
+-rw-r--r--   0        0        0      164 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/__init__.py
+-rw-r--r--   0        0        0     8369 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     2158 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/exceptions.py
+-rw-r--r--   0        0        0    14138 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/logger_config.py
+-rw-r--r--   0        0        0     4058 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/utils.py
+-rw-r--r--   0        0        0     2275 2024-05-10 20:27:44.886631 datagov_harvesting_logic-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.2/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.4.1/LICENSE.md` & `datagov_harvesting_logic-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.1/README.md` & `datagov_harvesting_logic-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.1/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.4.2/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.1/harvester/exceptions.py` & `datagov_harvesting_logic-0.4.2/harvester/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.1/harvester/harvest.py` & `datagov_harvesting_logic-0.4.2/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.1/harvester/logger_config.py` & `datagov_harvesting_logic-0.4.2/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.1/harvester/utils.py` & `datagov_harvesting_logic-0.4.2/harvester/utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.1/pyproject.toml` & `datagov_harvesting_logic-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
```

### Comparing `datagov_harvesting_logic-0.4.1/PKG-INFO` & `datagov_harvesting_logic-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
```

