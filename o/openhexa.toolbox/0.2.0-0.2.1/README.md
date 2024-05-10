# Comparing `tmp/openhexa.toolbox-0.2.0.tar.gz` & `tmp/openhexa_toolbox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.toolbox-0.2.0.tar", last modified: Thu Apr  4 12:35:19 2024, max compression
+gzip compressed data, was "openhexa_toolbox-0.2.1.tar", last modified: Fri May 10 15:23:56 2024, max compression
```

## Comparing `openhexa.toolbox-0.2.0.tar` & `openhexa_toolbox-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.647705 openhexa.toolbox-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.639705 openhexa.toolbox-0.2.0/openhexa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35411 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/periods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:35:19.647705 openhexa.toolbox-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/tests/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.427989 openhexa_toolbox-0.2.1/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.427989 openhexa_toolbox-0.2.1/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.427989 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/tests/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/test_lib.py
```

### Comparing `openhexa.toolbox-0.2.0/LICENSE` & `openhexa_toolbox-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/PKG-INFO` & `openhexa_toolbox-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.0 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.1 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `openhexa.toolbox-0.2.0/README.md` & `openhexa_toolbox-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/api.py` & `openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/dhis2.py` & `openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/dhis2.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 from typing import Callable, List, Tuple, Union
 from urllib.parse import urlparse
 
 import pandas as pd
 import polars as pl
 from diskcache import Cache
 
-
-from .api import Api, DHIS2Error, DHIS2Connection
+from .api import Api, DHIS2Connection, DHIS2Error
 
 logger = logging.getLogger(__name__)
 
 
-def use_cache(key: str):
+def use_cache(key: str, expire_time=86400):
     """Use sqlite-based diskcache.
 
     Return json response as a dict if cache is hit. If not, store the response in cache.
     """
 
     def decorator(func: Callable):
         @wraps(func)
@@ -29,15 +28,15 @@
                 return func(*args, **kwargs)
             else:
                 with Cache(args[0].client.cache_dir) as cache:
                     if key in cache:
                         return json.loads(cache.get(key))
                     else:
                         value = func(*args, **kwargs)
-                        cache.set(key, json.dumps(value))
+                        cache.set(key, json.dumps(value), expire=expire_time)
                         return value
 
         return wrapper
 
     return decorator
 
 
@@ -115,26 +114,34 @@
                     "level": level.get("level"),
                     "name": level.get("name"),
                 }
             )
         return levels
 
     @use_cache("organisation_units")
-    def organisation_units(self) -> List[dict]:
+    def organisation_units(self, filter: str = None) -> List[dict]:
         """Get organisation units metadata.
 
+        Parameters
+        ----------
+        filter: str, optional
+            DHIS2 query filter
+
         Return
         ------
         list of dict
             Id, name, level, path and geometry of all org units.
         """
+        params = {"fields": "id,name,level,path,geometry"}
+        if filter:
+            params["filter"] = filter
         org_units = []
         for page in self.client.api.get_paged(
             "organisationUnits",
-            params={"fields": "id,name,level,path,geometry"},
+            params=filter,
             page_size=1000,
         ):
             page = page.json()
             for ou in page["organisationUnits"]:
                 org_units.append(
                     {
                         "id": ou.get("id"),
@@ -195,26 +202,34 @@
                 row["data_elements"] = [dx["dataElement"]["id"] for dx in ds["dataSetElements"]]
                 row["indicators"] = [indicator["id"] for indicator in ds["indicators"]]
                 row["organisation_units"] = [ou["id"] for ou in ds["organisationUnits"]]
                 datasets.append(row)
         return datasets
 
     @use_cache("data_elements")
-    def data_elements(self) -> List[dict]:
+    def data_elements(self, filter: str = None) -> List[dict]:
         """Get data elements metadata.
 
+        Parameters
+        ----------
+        filter: str, optional
+            DHIS2 query filter
+
         Return
         ------
         list of dict
             Id, name, and aggregation type of all data elements.
         """
+        params = {"fields": "id,name,aggregationType,zeroIsSignificant"}
+        if filter:
+            params["filter"] = filter
         elements = []
         for page in self.client.api.get_paged(
             "dataElements",
-            params={"fields": "id,name,aggregationType,zeroIsSignificant"},
+            params=params,
             page_size=1000,
         ):
             elements += page.json()["dataElements"]
         return elements
 
     @use_cache("data_element_groups")
     def data_element_groups(self) -> List[dict]:
@@ -254,26 +269,34 @@
         """
         combos = []
         for page in self.client.api.get_paged("categoryOptionCombos", params={"fields": "id,name"}, page_size=1000):
             combos += page.json().get("categoryOptionCombos")
         return combos
 
     @use_cache("indicators")
-    def indicators(self) -> List[dict]:
+    def indicators(self, filter: str = None) -> List[dict]:
         """Get indicators metadata.
 
+        Parameters
+        ----------
+        filter: str, optional
+            DHIS2 query filter
+
         Return
         ------
         list of dict
             Id, name, numerator and denominator of all indicators.
         """
+        params = {"fields": "id,name,numerator,denominator"}
+        if filter:
+            params["filter"] = filter
         indicators = []
         for page in self.client.api.get_paged(
             "indicators",
-            params={"fields": "id,name,numerator,denominator"},
+            params=params,
             page_size=1000,
         ):
             indicators += page.json()["indicators"]
         return indicators
 
     @use_cache("indicatorGroups")
     def indicator_groups(self) -> List[dict]:
@@ -635,15 +658,22 @@
             # keep a cache with value type for each data element
             if de_uid in value_types:
                 value_type = value_types[de_uid]
             else:
                 value_type = self.client.meta.identifiable_objects(de_uid).get("valueType")
                 value_types[de_uid] = value_type
 
-            for key in ["dataElement", "orgUnit", "period", "value", "categoryOptionCombo", "attributeOptionCombo"]:
+            for key in [
+                "dataElement",
+                "orgUnit",
+                "period",
+                "value",
+                "categoryOptionCombo",
+                "attributeOptionCombo",
+            ]:
                 if not dv.get(key):
                     raise ValueError(f"Missing {key} key in data value")
 
             if value_type == "INTEGER":
                 if not isinstance(value, int):
                     raise ValueError(f"Data value {value} is not a valid {value_type}")
```

### Comparing `openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/periods.py` & `openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/periods.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/api.py` & `openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/parse.py` & `openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/parse.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/utils.py` & `openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/utils.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.0 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.1 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/SOURCES.txt` & `openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/pyproject.toml` & `openhexa_toolbox-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openhexa.toolbox"
-version = "0.2.0"
+version = "0.2.1"
 description = "A set of tools to acquire & process data from various sources"
 authors = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
 maintainers = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2.py` & `openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2_periods.py` & `openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2_periods.py`

 * *Files identical despite different names*

