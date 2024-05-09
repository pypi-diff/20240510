# Comparing `tmp/peco-0.0.8.tar.gz` & `tmp/peco-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/peco_outage_api/dist/tmpzwxby4c3/peco-0.0.8.tar", last modified: Tue Feb  1 00:30:52 2022, max compression
+gzip compressed data, was "/home/pi/peco_outage_api/dist/tmp647jwaws/peco-0.0.9.tar", last modified: Tue Feb  1 00:36:59 2022, max compression
```

## Comparing `peco-0.0.8.tar` & `peco-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:30:52.000000 peco-0.0.8/
--rw-r--r--   0 pi        (1000) pi        (1000)     1064 2022-01-31 00:25:51.000000 peco-0.0.8/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1516 2022-02-01 00:30:52.000000 peco-0.0.8/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      978 2022-01-31 00:25:14.000000 peco-0.0.8/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      103 2022-01-31 00:11:02.000000 peco-0.0.8/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)      655 2022-02-01 00:30:52.000000 peco-0.0.8/setup.cfg
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:30:52.000000 peco-0.0.8/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:30:52.000000 peco-0.0.8/src/peco/
--rw-r--r--   0 pi        (1000) pi        (1000)     2621 2022-02-01 00:29:12.000000 peco-0.0.8/src/peco/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      246 2022-01-31 00:21:28.000000 peco-0.0.8/src/peco/const.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:30:52.000000 peco-0.0.8/src/peco.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1516 2022-02-01 00:30:52.000000 peco-0.0.8/src/peco.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      240 2022-02-01 00:30:52.000000 peco-0.0.8/src/peco.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-02-01 00:30:52.000000 peco-0.0.8/src/peco.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2022-02-01 00:30:52.000000 peco-0.0.8/src/peco.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        5 2022-02-01 00:30:52.000000 peco-0.0.8/src/peco.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:36:59.000000 peco-0.0.9/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1064 2022-01-31 00:25:51.000000 peco-0.0.9/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1516 2022-02-01 00:36:59.000000 peco-0.0.9/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      978 2022-01-31 00:25:14.000000 peco-0.0.9/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      103 2022-01-31 00:11:02.000000 peco-0.0.9/pyproject.toml
+-rw-r--r--   0 pi        (1000) pi        (1000)      655 2022-02-01 00:36:59.000000 peco-0.0.9/setup.cfg
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:36:59.000000 peco-0.0.9/src/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:36:59.000000 peco-0.0.9/src/peco/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2626 2022-02-01 00:35:35.000000 peco-0.0.9/src/peco/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      246 2022-01-31 00:21:28.000000 peco-0.0.9/src/peco/const.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-01 00:36:59.000000 peco-0.0.9/src/peco.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1516 2022-02-01 00:36:59.000000 peco-0.0.9/src/peco.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      240 2022-02-01 00:36:59.000000 peco-0.0.9/src/peco.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-02-01 00:36:59.000000 peco-0.0.9/src/peco.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2022-02-01 00:36:59.000000 peco-0.0.9/src/peco.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        5 2022-02-01 00:36:59.000000 peco-0.0.9/src/peco.egg-info/top_level.txt
```

### Comparing `peco-0.0.8/LICENSE` & `peco-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `peco-0.0.8/PKG-INFO` & `peco-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peco
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper for PECO Outage API
 Home-page: https://github.com/IceBotYT/peco-outage-api
 Author: IceBotYT
 Author-email: icebotyt@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/IceBotYT/peco-outage-api/issues
 Platform: UNKNOWN
```

### Comparing `peco-0.0.8/README.md` & `peco-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `peco-0.0.8/setup.cfg` & `peco-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = peco
-version = 0.0.8
+version = 0.0.9
 author = IceBotYT
 author_email = icebotyt@outlook.com
 description = Wrapper for PECO Outage API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IceBotYT/peco-outage-api
 project_urls =
```

### Comparing `peco-0.0.8/src/peco/__init__.py` & `peco-0.0.9/src/peco/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main object for getting the PECO outage counter data."""
 import aiohttp
 
 from .const import API_URL, COUNTY_LIST
 
-async def get_outage_count(county, websession):
+async def get_outage_count(county, websession=None):
     """Get the outage count for the given county."""
     if not isinstance(county, str):
         raise ValueError("County must be specified")
 
     if county not in COUNTY_LIST:
         raise InvalidCountyError(f"{county} is not a valid county")
```

### Comparing `peco-0.0.8/src/peco.egg-info/PKG-INFO` & `peco-0.0.9/src/peco.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peco
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper for PECO Outage API
 Home-page: https://github.com/IceBotYT/peco-outage-api
 Author: IceBotYT
 Author-email: icebotyt@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/IceBotYT/peco-outage-api/issues
 Platform: UNKNOWN
```

