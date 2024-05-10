# Comparing `tmp/stac_fastapi_pgstac-2.5.0.tar.gz` & `tmp/stac_fastapi_pgstac-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_pgstac-2.5.0.tar", last modified: Thu Apr 25 15:42:48 2024, max compression
+gzip compressed data, was "stac_fastapi_pgstac-3.0.0a0.tar", last modified: Fri May 10 14:19:33 2024, max compression
```

## Comparing `stac_fastapi_pgstac-2.5.0.tar` & `stac_fastapi_pgstac-3.0.0a0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.858034 stac_fastapi_pgstac-2.5.0/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/base_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:42:48.000000 stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.858034 stac_fastapi_pgstac-2.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24752 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.862034 stac_fastapi_pgstac-2.5.0/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/clients/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:48.866034 stac_fastapi_pgstac-2.5.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)    50351 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 15:42:40.000000 stac_fastapi_pgstac-2.5.0/tests/resources/test_mgmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.665520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/base_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.665520 stac_fastapi_pgstac-3.0.0a0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24803 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/clients/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51039 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_mgmt.py
```

### Comparing `stac_fastapi_pgstac-2.5.0/LICENSE` & `stac_fastapi_pgstac-3.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-2.5.0/PKG-INFO` & `stac_fastapi_pgstac-3.0.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.5.0
+Version: 3.0.0a0
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -13,27 +13,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: orjson
-Requires-Dist: pydantic[dotenv]>=1.10.8
-Requires-Dist: stac_pydantic==2.0.*
-Requires-Dist: stac-fastapi.types~=2.5.5.post1
-Requires-Dist: stac-fastapi.api~=2.5.5.post1
-Requires-Dist: stac-fastapi.extensions~=2.5.5.post1
+Requires-Dist: pydantic
+Requires-Dist: stac_pydantic==3.0.*
+Requires-Dist: stac-fastapi.api~=3.0.0a0
+Requires-Dist: stac-fastapi.extensions~=3.0.0a0
+Requires-Dist: stac-fastapi.types~=3.0.0a0
 Requires-Dist: asyncpg
 Requires-Dist: buildpg
 Requires-Dist: brotli_asgi
 Requires-Dist: pygeofilter>=0.2
-Requires-Dist: pypgstac==0.7.*
+Requires-Dist: pypgstac==0.8.*
 Provides-Extra: dev
 Requires-Dist: pystac[validation]; extra == "dev"
-Requires-Dist: pypgstac[psycopg]==0.7.*; extra == "dev"
+Requires-Dist: pypgstac[psycopg]==0.8.*; extra == "dev"
 Requires-Dist: pytest-postgresql; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio<0.23.0,>=0.17; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: shapely; extra == "dev"
```

### Comparing `stac_fastapi_pgstac-2.5.0/README.md` & `stac_fastapi_pgstac-3.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-2.5.0/pyproject.toml` & `stac_fastapi_pgstac-3.0.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-2.5.0/setup.py` & `stac_fastapi_pgstac-3.0.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
     "attrs",
     "orjson",
-    "pydantic[dotenv]>=1.10.8",  # https://github.com/pydantic/pydantic/issues/5821
-    "stac_pydantic==2.0.*",
-    "stac-fastapi.types~=2.5.5.post1",
-    "stac-fastapi.api~=2.5.5.post1",
-    "stac-fastapi.extensions~=2.5.5.post1",
+    "pydantic",
+    "stac_pydantic==3.0.*",
+    "stac-fastapi.api~=3.0.0a0",
+    "stac-fastapi.extensions~=3.0.0a0",
+    "stac-fastapi.types~=3.0.0a0",
     "asyncpg",
     "buildpg",
     "brotli_asgi",
     "pygeofilter>=0.2",
-    "pypgstac==0.7.*",
+    "pypgstac==0.8.*",
 ]
 
 extra_reqs = {
     "dev": [
         "pystac[validation]",
-        "pypgstac[psycopg]==0.7.*",
+        "pypgstac[psycopg]==0.8.*",
         "pytest-postgresql",
         "pytest",
         "pytest-cov",
         "pytest-asyncio>=0.17,<0.23.0",
         "pre-commit",
         "requests",
         "shapely",
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/app.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import os
 
 from fastapi.responses import ORJSONResponse
 from stac_fastapi.api.app import StacApi
 from stac_fastapi.api.models import create_get_request_model, create_post_request_model
 from stac_fastapi.extensions.core import (
-    ContextExtension,
     FieldsExtension,
     FilterExtension,
     SortExtension,
     TokenPaginationExtension,
     TransactionExtension,
 )
 from stac_fastapi.extensions.third_party import BulkTransactionExtension
@@ -35,15 +34,14 @@
         settings=settings,
         response_class=ORJSONResponse,
     ),
     "query": QueryExtension(),
     "sort": SortExtension(),
     "fields": FieldsExtension(),
     "pagination": TokenPaginationExtension(),
-    "context": ContextExtension(),
     "filter": FilterExtension(client=FiltersClient()),
     "bulk_transactions": BulkTransactionExtension(client=BulkTransactionsClient()),
 }
 
 if enabled_extensions := os.getenv("ENABLED_EXTENSIONS"):
     extensions = [
         extensions_map[extension_name] for extension_name in enabled_extensions.split(",")
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/config.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Postgres API configuration."""
 
 from typing import List, Type
 from urllib.parse import quote
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+from pydantic_settings import SettingsConfigDict
 from stac_fastapi.types.config import ApiSettings
 
 from stac_fastapi.pgstac.types.base_item_cache import (
     BaseItemCache,
     DefaultBaseItemCache,
 )
 
@@ -29,20 +30,22 @@
     "+",
     ",",
     ";",
     "=",
 ]
 
 
-class ServerSettings(BaseModel, extra=Extra.allow):
+class ServerSettings(BaseModel):
     """Server runtime parameters."""
 
     search_path: str = "pgstac,public"
     application_name: str = "pgstac"
 
+    model_config = SettingsConfigDict(extra="allow")
+
 
 class Settings(ApiSettings):
     """Postgres-specific API settings.
 
     Attributes:
         postgres_user: postgres username.
         postgres_pass: postgres password.
@@ -54,15 +57,15 @@
         invalid_id_chars: list of characters that are not allowed in item or collection ids.
     """
 
     postgres_user: str
     postgres_pass: str
     postgres_host_reader: str
     postgres_host_writer: str
-    postgres_port: str
+    postgres_port: int
     postgres_dbname: str
 
     db_min_conn_size: int = 10
     db_max_conn_size: int = 10
     db_max_queries: int = 50000
     db_max_inactive_conn_lifetime: float = 300
 
@@ -85,11 +88,10 @@
         return f"postgresql://{self.postgres_user}:{quote(self.postgres_pass)}@{self.postgres_host_writer}:{self.postgres_port}/{self.postgres_dbname}"
 
     @property
     def testing_connection_string(self):
         """Create testing psql connection string."""
         return f"postgresql://{self.postgres_user}:{quote(self.postgres_pass)}@{self.postgres_host_writer}:{self.postgres_port}/pgstactestdb"
 
-    class Config(ApiSettings.Config):
-        """Model config."""
-
-        env_nested_delimiter = "__"
+    model_config = SettingsConfigDict(
+        **{**ApiSettings.model_config, **{"env_nested_delimiter": "__"}}
+    )
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/core.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,17 @@
 
         if search_request.datetime:
             search_request.datetime = format_datetime_range(search_request.datetime)
 
         search_request.conf = search_request.conf or {}
         search_request.conf["nohydrate"] = settings.use_api_hydrate
 
-        search_request_json = search_request.json(exclude_none=True, by_alias=True)
+        search_request_json = search_request.model_dump_json(
+            exclude_none=True, by_alias=True
+        )
 
         try:
             async with request.app.state.get_connection(request, "r") as conn:
                 q, p = render(
                     """
                     SELECT * FROM search(:req::text::jsonb);
                     """,
@@ -222,14 +224,17 @@
 
             base_item_cache = settings.base_item_cache(
                 fetch_base_item=_get_base_item, request=request
             )
 
             for feature in collection.get("features") or []:
                 base_item = await base_item_cache.get(feature.get("collection"))
+                # Exclude None values
+                base_item = {k: v for k, v in base_item.items() if v is not None}
+
                 feature = hydrate(base_item, feature)
 
                 # Grab ids needed for links that may be removed by the fields extension.
                 collection_id = feature.get("collection")
                 item_id = feature.get("id")
 
                 feature = filter_fields(feature, include, exclude)
@@ -270,14 +275,17 @@
 
         Returns:
             An ItemCollection.
         """
         # If collection does not exist, NotFoundError wil be raised
         await self.get_collection(collection_id, request=request)
 
+        if datetime:
+            datetime = format_datetime_range(datetime)
+
         base_args = {
             "collections": [collection_id],
             "bbox": bbox,
             "datetime": datetime,
             "limit": limit,
             "token": token,
         }
@@ -386,15 +394,15 @@
         if filter:
             if filter_lang == "cql2-text":
                 ast = parse_cql2_text(filter)
                 base_args["filter"] = orjson.loads(to_cql2(ast))
                 base_args["filter-lang"] = "cql2-json"
 
         if datetime:
-            base_args["datetime"] = datetime
+            base_args["datetime"] = format_datetime_range(datetime)
 
         if intersects:
             base_args["intersects"] = orjson.loads(unquote_plus(intersects))
 
         if sortby:
             # https://github.com/radiantearth/stac-spec/tree/master/api-spec/extensions/sort#http-get-or-post-form
             sort_param = []
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/db.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,10 +138,10 @@
         pool = await asyncpg.create_pool(
             connection_string,
             min_size=settings.db_min_conn_size,
             max_size=settings.db_max_conn_size,
             max_queries=settings.db_max_queries,
             max_inactive_connection_lifetime=settings.db_max_inactive_conn_lifetime,
             init=con_init,
-            server_settings=settings.server_settings.dict(),
+            server_settings=settings.server_settings.model_dump(),
         )
         return pool
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/filter.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Get Queryables."""
 
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 
 from buildpg import render
 from fastapi import Request
-from fastapi.responses import JSONResponse
 from stac_fastapi.types.core import AsyncBaseFiltersClient
 from stac_fastapi.types.errors import NotFoundError
 
 
 class FiltersClient(AsyncBaseFiltersClient):
     """Defines a pattern for implementing the STAC filter extension."""
 
     async def get_queryables(
-        self, request: Request, collection_id: Optional[str] = None, **kwargs: Any
-    ) -> JSONResponse:
+        self,
+        request: Request,
+        collection_id: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Dict[str, Any]:
         """Get the queryables available for the given collection_id.
 
         If collection_id is None, returns the intersection of all
         queryables over all collections.
         This base implementation returns a blank queryable schema. This is not allowed
         under OGC CQL but it is allowed by the STAC API Filter Extension
         https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
@@ -33,9 +35,8 @@
                 collection=collection_id,
             )
             queryables = await conn.fetchval(q, *p)
             if not queryables:
                 raise NotFoundError(f"Collection {collection_id} not found")
 
             queryables["$id"] = str(request.url)
-            headers = {"Content-Type": "application/schema+json"}
-            return JSONResponse(queryables, headers=headers)
+            return queryables
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/extensions/query.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """Return python operator."""
         return getattr(operator, self._value_)
 
 
 class QueryExtensionPostRequest(BaseModel):
     """Query Extension POST request model."""
 
-    query: Optional[Dict[str, Dict[Operator, Any]]]
+    query: Optional[Dict[str, Dict[Operator, Any]]] = None
 
 
 class QueryExtension(QueryExtensionBase):
     """Query Extension.
 
     Override the POST request model to add validation against
     supported fields
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/models/links.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/transactions.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from stac_fastapi.extensions.third_party.bulk_transactions import (
     AsyncBaseBulkTransactionsClient,
     BulkTransactionMethod,
     Items,
 )
 from stac_fastapi.types import stac as stac_types
 from stac_fastapi.types.core import AsyncBaseTransactionsClient
+from stac_pydantic import Collection, Item, ItemCollection
 from starlette.responses import JSONResponse, Response
 
 from stac_fastapi.pgstac.config import Settings
 from stac_fastapi.pgstac.db import dbfunc
 from stac_fastapi.pgstac.models.links import CollectionLinks, ItemLinks
 
 logger = logging.getLogger("uvicorn")
@@ -65,19 +66,21 @@
                 status_code=400,
                 detail=f"Item ID from path parameter ({expected_item_id}) does not match Item ID from Item ({body_item_id})",
             )
 
     async def create_item(
         self,
         collection_id: str,
-        item: Union[stac_types.Item, stac_types.ItemCollection],
+        item: Union[Item, ItemCollection],
         request: Request,
         **kwargs,
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Create item."""
+        item = item.model_dump(mode="json")
+
         if item["type"] == "FeatureCollection":
             valid_items = []
             for item in item["features"]:  # noqa: B020
                 self._validate_item(request, item, collection_id)
                 item["collection"] = collection_id
                 valid_items.append(item)
 
@@ -96,29 +99,32 @@
             item["links"] = await ItemLinks(
                 collection_id=collection_id,
                 item_id=item["id"],
                 request=request,
             ).get_links(extra_links=item.get("links"))
 
             return stac_types.Item(**item)
+
         else:
             raise HTTPException(
                 status_code=400,
                 detail=f"Item body type must be 'Feature' or 'FeatureCollection', not {item['type']}",
             )
 
     async def update_item(
         self,
         request: Request,
         collection_id: str,
         item_id: str,
-        item: stac_types.Item,
+        item: Item,
         **kwargs,
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Update item."""
+        item = item.model_dump(mode="json")
+
         self._validate_item(request, item, collection_id, item_id)
         item["collection"] = collection_id
 
         async with request.app.state.get_connection(request, "w") as conn:
             await dbfunc(conn, "update_item", item)
 
         item["links"] = await ItemLinks(
@@ -126,56 +132,77 @@
             item_id=item["id"],
             request=request,
         ).get_links(extra_links=item.get("links"))
 
         return stac_types.Item(**item)
 
     async def create_collection(
-        self, collection: stac_types.Collection, request: Request, **kwargs
+        self,
+        collection: Collection,
+        request: Request,
+        **kwargs,
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Create collection."""
+        collection = collection.model_dump(mode="json")
+
         self._validate_collection(request, collection)
+
         async with request.app.state.get_connection(request, "w") as conn:
             await dbfunc(conn, "create_collection", collection)
+
         collection["links"] = await CollectionLinks(
             collection_id=collection["id"], request=request
-        ).get_links(extra_links=collection.get("links"))
+        ).get_links(extra_links=collection["links"])
 
         return stac_types.Collection(**collection)
 
     async def update_collection(
-        self, collection: stac_types.Collection, request: Request, **kwargs
+        self,
+        collection: Collection,
+        request: Request,
+        **kwargs,
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Update collection."""
+
+        col = collection.model_dump(mode="json")
+
         async with request.app.state.get_connection(request, "w") as conn:
-            await dbfunc(conn, "update_collection", collection)
-        collection["links"] = await CollectionLinks(
-            collection_id=collection["id"], request=request
-        ).get_links(extra_links=collection.get("links"))
-        return stac_types.Collection(**collection)
+            await dbfunc(conn, "update_collection", col)
+
+        col["links"] = await CollectionLinks(
+            collection_id=col["id"], request=request
+        ).get_links(extra_links=col.get("links"))
+
+        return stac_types.Collection(**col)
 
     async def delete_item(
-        self, item_id: str, collection_id: str, request: Request, **kwargs
+        self,
+        item_id: str,
+        collection_id: str,
+        request: Request,
+        **kwargs,
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Delete item."""
         q, p = render(
             "SELECT * FROM delete_item(:item::text, :collection::text);",
             item=item_id,
             collection=collection_id,
         )
         async with request.app.state.get_connection(request, "w") as conn:
             await conn.fetchval(q, *p)
+
         return JSONResponse({"deleted item": item_id})
 
     async def delete_collection(
         self, collection_id: str, request: Request, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Delete collection."""
         async with request.app.state.get_connection(request, "w") as conn:
             await dbfunc(conn, "delete_collection", collection_id)
+
         return JSONResponse({"deleted collection": collection_id})
 
 
 @attr.s
 class BulkTransactionsClient(AsyncBaseBulkTransactionsClient):
     """Postgres bulk transactions."""
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/base_item_cache.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/base_item_cache.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/types/search.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """stac_fastapi.types.search module."""
 
 from typing import Dict, Optional
 
-from pydantic import validator
+from pydantic import ValidationInfo, field_validator
 from stac_fastapi.types.search import BaseSearchPostRequest
 
 
 class PgstacSearch(BaseSearchPostRequest):
     """Search model.
 
     Overrides the validation for datetime from the base request model.
     """
 
     conf: Optional[Dict] = None
 
-    @validator("filter_lang", pre=False, check_fields=False, always=True)
-    def validate_query_uses_cql(cls, v, values):
+    @field_validator("filter_lang", check_fields=False)
+    @classmethod
+    def validate_query_uses_cql(cls, v: str, info: ValidationInfo):
         """Use of Query Extension is not allowed with cql2."""
-        if values.get("query", None) is not None and v != "cql-json":
+        if info.data.get("query", None) is not None and v != "cql-json":
             raise ValueError(
                 "Query extension is not available when using pgstac with cql2"
             )
 
         return v
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi/pgstac/utils.py` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             and isinstance(merge_from[k], dict)
         ):
             dict_deep_update(merge_to[k], merge_from[k])
         else:
             merge_to[k] = v
 
 
-def format_datetime_range(dt_range: DateTimeType) -> Union[str, Any]:
+def format_datetime_range(dt_range: Union[DateTimeType, str]) -> str:
     """
     Convert a datetime object or a tuple of datetime objects to a formatted string for datetime ranges.
 
     Args:
         dt_range (DateTimeType): The date interval,
             which might be a single datetime or a tuple with one or two datetimes.
 
@@ -128,15 +128,15 @@
         str: A formatted string like 'YYYY-MM-DDTHH:MM:SSZ/..', 'YYYY-MM-DDTHH:MM:SSZ', or the original string input.
     """
     # Handle a single datetime object
     if isinstance(dt_range, datetime):
         return dt_range.isoformat().replace("+00:00", "Z")
 
     # Handle a tuple containing datetime objects or None
-    if isinstance(dt_range, tuple):
+    elif isinstance(dt_range, tuple):
         start, end = dt_range
 
         # Convert start datetime to string if not None, otherwise use ".."
         start_str = start.isoformat().replace("+00:00", "Z") if start else ".."
 
         # Convert end datetime to string if not None, otherwise use ".."
         end_str = end.isoformat().replace("+00:00", "Z") if end else ".."
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/PKG-INFO` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.5.0
+Version: 3.0.0a0
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -13,27 +13,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: orjson
-Requires-Dist: pydantic[dotenv]>=1.10.8
-Requires-Dist: stac_pydantic==2.0.*
-Requires-Dist: stac-fastapi.types~=2.5.5.post1
-Requires-Dist: stac-fastapi.api~=2.5.5.post1
-Requires-Dist: stac-fastapi.extensions~=2.5.5.post1
+Requires-Dist: pydantic
+Requires-Dist: stac_pydantic==3.0.*
+Requires-Dist: stac-fastapi.api~=3.0.0a0
+Requires-Dist: stac-fastapi.extensions~=3.0.0a0
+Requires-Dist: stac-fastapi.types~=3.0.0a0
 Requires-Dist: asyncpg
 Requires-Dist: buildpg
 Requires-Dist: brotli_asgi
 Requires-Dist: pygeofilter>=0.2
-Requires-Dist: pypgstac==0.7.*
+Requires-Dist: pypgstac==0.8.*
 Provides-Extra: dev
 Requires-Dist: pystac[validation]; extra == "dev"
-Requires-Dist: pypgstac[psycopg]==0.7.*; extra == "dev"
+Requires-Dist: pypgstac[psycopg]==0.8.*; extra == "dev"
 Requires-Dist: pytest-postgresql; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio<0.23.0,>=0.17; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: shapely; extra == "dev"
```

### Comparing `stac_fastapi_pgstac-2.5.0/stac_fastapi.pgstac.egg-info/SOURCES.txt` & `stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-2.5.0/tests/api/test_api.py` & `stac_fastapi_pgstac-3.0.0a0/tests/api/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime, timedelta
 from typing import Any, Callable, Coroutine, Dict, List, Optional, TypeVar
 from urllib.parse import quote_plus
 
 import orjson
 import pytest
 from fastapi import Request
-from httpx import AsyncClient
+from httpx import ASGITransport, AsyncClient
 from pystac import Collection, Extent, Item, SpatialExtent, TemporalExtent
 from stac_fastapi.api.app import StacApi
 from stac_fastapi.api.models import create_post_request_model
 from stac_fastapi.extensions.core import FieldsExtension, TransactionExtension
 from stac_fastapi.types import stac as stac_types
 
 from stac_fastapi.pgstac.core import CoreCrudClient, Settings
@@ -68,37 +68,37 @@
 
 
 async def test_get_queryables_content_type(app_client, load_test_collection):
     resp = await app_client.get("queryables")
     assert resp.headers["content-type"] == "application/schema+json"
 
     coll = load_test_collection
-    resp = await app_client.get(f"collections/{coll.id}/queryables")
+    resp = await app_client.get(f"collections/{coll['id']}/queryables")
     assert resp.headers["content-type"] == "application/schema+json"
 
 
 async def test_get_features_content_type(app_client, load_test_collection):
     coll = load_test_collection
-    resp = await app_client.get(f"collections/{coll.id}/items")
+    resp = await app_client.get(f"collections/{coll['id']}/items")
     assert resp.headers["content-type"] == "application/geo+json"
 
 
 async def test_get_features_self_link(app_client, load_test_collection):
     # https://github.com/stac-utils/stac-fastapi/issues/483
-    resp = await app_client.get(f"collections/{load_test_collection.id}/items")
+    resp = await app_client.get(f"collections/{load_test_collection['id']}/items")
     assert resp.status_code == 200
     resp_json = resp.json()
     self_link = next((link for link in resp_json["links"] if link["rel"] == "self"), None)
     assert self_link is not None
     assert self_link["href"].endswith("/items")
 
 
 async def test_get_feature_content_type(app_client, load_test_collection, load_test_item):
     resp = await app_client.get(
-        f"collections/{load_test_collection.id}/items/{load_test_item.id}"
+        f"collections/{load_test_collection['id']}/items/{load_test_item['id']}"
     )
     assert resp.headers["content-type"] == "application/geo+json"
 
 
 async def test_api_headers(app_client):
     resp = await app_client.get("/api")
     assert resp.headers["content-type"] == "application/vnd.oai.openapi+json;version=3.0"
@@ -137,23 +137,23 @@
 
 
 async def test_app_transaction_extension(
     app_client, load_test_data, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
 
 async def test_app_query_extension(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     params = {"query": {"proj:epsg": {"eq": item["properties"]["proj:epsg"]}}}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
@@ -165,16 +165,16 @@
 
 
 async def test_app_query_extension_limit_1(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     params = {"limit": 1}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
@@ -186,163 +186,163 @@
 
 
 async def test_app_query_extension_limit_lt0(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     params = {"limit": -1}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 400
 
 
 async def test_app_query_extension_limit_gt10000(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     params = {"limit": 10001}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
 
 
 async def test_app_query_extension_gt(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     params = {"query": {"proj:epsg": {"gt": item["properties"]["proj:epsg"]}}}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 0
 
 
 async def test_app_query_extension_gte(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     params = {"query": {"proj:epsg": {"gte": item["properties"]["proj:epsg"]}}}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
 
 async def test_app_sort_extension(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     first_item = load_test_data("test_item.json")
     item_date = datetime.strptime(
         first_item["properties"]["datetime"], "%Y-%m-%dT%H:%M:%SZ"
     )
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=first_item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=first_item)
+    assert resp.status_code == 201
 
     second_item = load_test_data("test_item.json")
     second_item["id"] = "another-item"
     another_item_date = item_date - timedelta(days=1)
     second_item["properties"]["datetime"] = another_item_date.strftime(
         "%Y-%m-%dT%H:%M:%SZ"
     )
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=second_item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=second_item)
+    assert resp.status_code == 201
 
     params = {
-        "collections": [coll.id],
+        "collections": [coll["id"]],
         "sortby": [{"field": "datetime", "direction": "desc"}],
     }
 
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert resp_json["features"][0]["id"] == first_item["id"]
     assert resp_json["features"][1]["id"] == second_item["id"]
 
     params = {
-        "collections": [coll.id],
+        "collections": [coll["id"]],
         "sortby": [{"field": "datetime", "direction": "asc"}],
     }
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert resp_json["features"][1]["id"] == first_item["id"]
     assert resp_json["features"][0]["id"] == second_item["id"]
 
 
 async def test_search_invalid_date(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     first_item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=first_item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=first_item)
+    assert resp.status_code == 201
 
     params = {
         "datetime": "2020-XX-01/2020-10-30",
-        "collections": [coll.id],
+        "collections": [coll["id"]],
     }
 
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 400
 
 
 async def test_bbox_3d(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     first_item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=first_item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=first_item)
+    assert resp.status_code == 201
 
     australia_bbox = [106.343365, -47.199523, 0.1, 168.218365, -19.437288, 0.1]
     params = {
         "bbox": australia_bbox,
-        "collections": [coll.id],
+        "collections": [coll["id"]],
     }
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
 
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
 
 async def test_app_search_response(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     params = {
-        "collections": [coll.id],
+        "collections": [coll["id"]],
     }
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
 
     assert resp_json.get("type") == "FeatureCollection"
     # stac_version and stac_extensions were removed in v1.0.0-beta.3
     assert resp_json.get("stac_version") is None
     assert resp_json.get("stac_extensions") is None
 
 
 async def test_search_point_intersects(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     new_coordinates = []
     for coordinate in item["geometry"]["coordinates"][0]:
         new_coordinates.append([coordinate[0] * -1, coordinate[1] * -1])
     item["id"] = "test-item-other-hemispheres"
     item["geometry"]["coordinates"] = [new_coordinates]
     item["bbox"] = [value * -1 for value in item["bbox"]]
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     point = [150.04, -33.14]
     intersects = {"type": "Point", "coordinates": point}
 
     params = {
         "intersects": intersects,
         "collections": [item["collection"]],
@@ -360,16 +360,16 @@
 
 
 async def test_search_line_string_intersects(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     line = [[150.04, -33.14], [150.22, -33.89]]
     intersects = {"type": "LineString", "coordinates": line}
 
     params = {
         "intersects": intersects,
         "collections": [item["collection"]],
@@ -380,15 +380,15 @@
     assert len(resp_json["features"]) == 1
 
 
 @pytest.mark.asyncio
 async def test_landing_forwarded_header(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    await app_client.post(f"/collections/{coll.id}/items", json=item)
+    await app_client.post(f"/collections/{coll['id']}/items", json=item)
     response = (
         await app_client.get(
             "/",
             headers={
                 "Forwarded": "proto=https;host=test:1234",
                 "X-Forwarded-Proto": "http",
                 "X-Forwarded-Port": "4321",
@@ -399,15 +399,15 @@
         assert link["href"].startswith("https://test:1234/")
 
 
 @pytest.mark.asyncio
 async def test_search_forwarded_header(load_test_data, app_client, load_test_collection):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    await app_client.post(f"/collections/{coll.id}/items", json=item)
+    await app_client.post(f"/collections/{coll['id']}/items", json=item)
     resp = await app_client.post(
         "/search",
         json={
             "collections": [item["collection"]],
         },
         headers={"Forwarded": "proto=https;host=test:1234"},
     )
@@ -420,15 +420,15 @@
 
 @pytest.mark.asyncio
 async def test_search_x_forwarded_headers(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    await app_client.post(f"/collections/{coll.id}/items", json=item)
+    await app_client.post(f"/collections/{coll['id']}/items", json=item)
     resp = await app_client.post(
         "/search",
         json={
             "collections": [item["collection"]],
         },
         headers={
             "X-Forwarded-Proto": "https",
@@ -444,15 +444,15 @@
 
 @pytest.mark.asyncio
 async def test_search_duplicate_forward_headers(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
-    await app_client.post(f"/collections/{coll.id}/items", json=item)
+    await app_client.post(f"/collections/{coll['id']}/items", json=item)
     resp = await app_client.post(
         "/search",
         json={
             "collections": [item["collection"]],
         },
         headers={
             "Forwarded": "proto=https;host=test:1234",
@@ -472,71 +472,69 @@
     resp = await app_client.get("/queryables")
     assert resp.headers["Content-Type"] == "application/schema+json"
     q = resp.json()
     assert q["$id"].endswith("/queryables")
     assert q["type"] == "object"
     assert "properties" in q
     assert "id" in q["properties"]
-    assert "eo:cloud_cover" in q["properties"]
 
 
 @pytest.mark.asyncio
 async def test_collection_queryables(load_test_data, app_client, load_test_collection):
     resp = await app_client.get("/collections/test-collection/queryables")
     assert resp.headers["Content-Type"] == "application/schema+json"
     q = resp.json()
     assert q["$id"].endswith("/collections/test-collection/queryables")
     assert q["type"] == "object"
     assert "properties" in q
     assert "id" in q["properties"]
-    assert "eo:cloud_cover" in q["properties"]
 
 
 @pytest.mark.asyncio
 async def test_item_collection_filter_bbox(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     first_item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=first_item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=first_item)
+    assert resp.status_code == 201
 
     bbox = "100,-50,170,-20"
-    resp = await app_client.get(f"/collections/{coll.id}/items", params={"bbox": bbox})
+    resp = await app_client.get(f"/collections/{coll['id']}/items", params={"bbox": bbox})
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
     bbox = "1,2,3,4"
-    resp = await app_client.get(f"/collections/{coll.id}/items", params={"bbox": bbox})
+    resp = await app_client.get(f"/collections/{coll['id']}/items", params={"bbox": bbox})
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 0
 
 
 @pytest.mark.asyncio
 async def test_item_collection_filter_datetime(
     load_test_data, app_client, load_test_collection
 ):
     coll = load_test_collection
     first_item = load_test_data("test_item.json")
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=first_item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=first_item)
+    assert resp.status_code == 201
 
     datetime_range = "2020-01-01T00:00:00.00Z/.."
     resp = await app_client.get(
-        f"/collections/{coll.id}/items", params={"datetime": datetime_range}
+        f"/collections/{coll['id']}/items", params={"datetime": datetime_range}
     )
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
     datetime_range = "2018-01-01T00:00:00.00Z/2019-01-01T00:00:00.00Z"
     resp = await app_client.get(
-        f"/collections/{coll.id}/items", params={"datetime": datetime_range}
+        f"/collections/{coll['id']}/items", params={"datetime": datetime_range}
     )
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 0
 
 
 @pytest.mark.asyncio
@@ -552,21 +550,21 @@
     collection_b = Collection("collection-b", "The second collection", DEFAULT_EXTENT)
     item = Item("the-item", GLOBAL_GEOMETRY, GLOBAL_BBOX, datetime.now(), {})
 
     for collection in (collection_a, collection_b):
         response = await app_client.post(
             "/collections", json=collection.to_dict(include_self_link=False)
         )
-        assert response.status_code == 200
+        assert response.status_code == 201
         item_as_dict = item.to_dict(include_self_link=False)
         item_as_dict["collection"] = collection.id
         response = await app_client.post(
             f"/collections/{collection.id}/items", json=item_as_dict
         )
-        assert response.status_code == 200
+        assert response.status_code == 201
         response = await app_client.get(f"/collections/{collection.id}/items")
         assert response.status_code == 200, response.json()
         assert len(response.json()["features"]) == 1
 
     for collection in (collection_a, collection_b):
         response = await app_client.delete(
             f"/collections/{collection.id}/items/{item.id}"
@@ -575,15 +573,15 @@
         response = await app_client.get(f"/collections/{collection.id}/items")
         assert response.status_code == 200, response.json()
         assert not response.json()["features"]
 
 
 @pytest.mark.parametrize("direction", ("asc", "desc"))
 async def test_sorting_and_paging(app_client, load_test_collection, direction: str):
-    collection_id = load_test_collection.id
+    collection_id = load_test_collection["id"]
     for i in range(10):
         item = Item(
             id=f"item-{i}",
             geometry={"type": "Point", "coordinates": [-105.1019, 40.1672]},
             bbox=[-105.1019, 40.1672, -105.1019, 40.1672],
             datetime=datetime.now(),
             properties={
@@ -591,15 +589,15 @@
             },
         )
         item.collection_id = collection_id
         response = await app_client.post(
             f"/collections/{collection_id}/items",
             json=item.to_dict(include_self_link=False, transform_hrefs=False),
         )
-        assert response.status_code == 200
+        assert response.status_code == 201
 
     async def search(query: Dict[str, Any]) -> List[Item]:
         items: List[Item] = []
         while True:
             response = await app_client.post("/search", json=query)
             json = response.json()
             assert response.status_code == 200, json
@@ -676,24 +674,24 @@
         settings=settings,
         extensions=extensions,
         search_post_request_model=post_request_model,
     )
     app = api.app
     await connect_to_db(app)
     try:
-        async with AsyncClient(app=app) as client:
+        async with AsyncClient(transport=ASGITransport(app=app)) as client:
             response = await client.post(
                 "http://test/collections",
                 json=load_test_data("test_collection.json"),
             )
-            assert response.status_code == 200
+            assert response.status_code == 201
             response = await client.post(
                 "http://test/collections/test-collection/items",
                 json=load_test_data("test_item.json"),
             )
-            assert response.status_code == 200
+            assert response.status_code == 201
             response = await client.get(
                 "http://test/collections/test-collection/items/test-item"
             )
             assert response.status_code == 200
     finally:
         await close_db_connection(app)
```

### Comparing `stac_fastapi_pgstac-2.5.0/tests/clients/test_postgres.py` & `stac_fastapi_pgstac-3.0.0a0/tests/clients/test_postgres.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,182 +12,193 @@
 
 # from tests.conftest import MockStarletteRequest
 logger = logging.getLogger(__name__)
 
 
 async def test_create_collection(app_client, load_test_data: Callable):
     in_json = load_test_data("test_collection.json")
-    in_coll = Collection.parse_obj(in_json)
+    in_coll = Collection.model_validate(in_json)
     resp = await app_client.post(
         "/collections",
         json=in_json,
     )
-    assert resp.status_code == 200
-    post_coll = Collection.parse_obj(resp.json())
-    assert in_coll.dict(exclude={"links"}) == post_coll.dict(exclude={"links"})
+    assert resp.status_code == 201
+    post_coll = Collection.model_validate(resp.json())
+    assert in_coll.model_dump(exclude={"links"}) == post_coll.model_dump(
+        exclude={"links"}
+    )
+
     resp = await app_client.get(f"/collections/{post_coll.id}")
     assert resp.status_code == 200
-    get_coll = Collection.parse_obj(resp.json())
-    assert post_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
+    get_coll = Collection.model_validate(resp.json())
+    assert post_coll.model_dump(exclude={"links"}) == get_coll.model_dump(
+        exclude={"links"}
+    )
 
 
-async def test_update_collection(app_client, load_test_collection):
+async def test_update_collection(app_client, load_test_collection, load_test_data):
     in_coll = load_test_collection
-    in_coll.keywords.append("newkeyword")
+    in_coll["keywords"].append("newkeyword")
 
-    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll['id']}", json=in_coll)
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{in_coll.id}")
+    resp = await app_client.get(f"/collections/{in_coll['id']}")
     assert resp.status_code == 200
 
-    get_coll = Collection.parse_obj(resp.json())
-    assert in_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
+    get_coll = Collection.model_validate(resp.json())
+    in_coll = Collection(**in_coll)
+    assert in_coll.model_dump(exclude={"links"}) == get_coll.model_dump(exclude={"links"})
     assert "newkeyword" in get_coll.keywords
 
 
 async def test_delete_collection(app_client, load_test_collection):
     in_coll = load_test_collection
 
-    resp = await app_client.delete(f"/collections/{in_coll.id}")
+    resp = await app_client.delete(f"/collections/{in_coll['id']}")
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{in_coll.id}")
+    resp = await app_client.get(f"/collections/{in_coll['id']}")
     assert resp.status_code == 404
 
 
 async def test_create_item(app_client, load_test_data: Callable, load_test_collection):
     coll = load_test_collection
     in_json = load_test_data("test_item.json")
-    in_item = Item.parse_obj(in_json)
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=in_json,
     )
+    assert resp.status_code == 201
+    in_item = Item.model_validate(in_json)
+    post_item = Item.model_validate(resp.json())
+    assert in_item.model_dump(exclude={"links"}) == post_item.model_dump(
+        exclude={"links"}
+    )
+
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{post_item.id}")
     assert resp.status_code == 200
-    post_item = Item.parse_obj(resp.json())
-    assert in_item.dict(exclude={"links"}) == post_item.dict(exclude={"links"})
-    resp = await app_client.get(f"/collections/{coll.id}/items/{post_item.id}")
-    assert resp.status_code == 200
-    get_item = Item.parse_obj(resp.json())
-    assert in_item.dict(exclude={"links"}) == get_item.dict(exclude={"links"})
+    get_item = Item.model_validate(resp.json())
+    assert in_item.model_dump(exclude={"links"}) == get_item.model_dump(exclude={"links"})
 
 
 async def test_create_item_no_collection_id(
     app_client, load_test_data: Callable, load_test_collection
 ):
     """Items with no collection id should be set with the collection id from the path"""
     coll = load_test_collection
 
     item = load_test_data("test_item.json")
     item["collection"] = None
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item,
     )
 
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{item['id']}")
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{item['id']}")
 
     assert resp.status_code == 200
 
-    get_item = Item.parse_obj(resp.json())
-    assert get_item.collection == coll.id
+    get_item = Item.model_validate(resp.json())
+    assert get_item.collection == coll["id"]
 
 
 async def test_create_item_invalid_ids(
     app_client, load_test_data: Callable, load_test_collection
 ):
     """Items with invalid ids should return an error"""
     coll = load_test_collection
 
     item = load_test_data("test_item.json")
     item["id"] = "invalid/id"
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item,
     )
     assert resp.status_code == 400
 
 
 async def test_create_item_invalid_collection_id(
     app_client, load_test_data: Callable, load_test_collection
 ):
     """Items with invalid collection ids should return an error"""
     coll = load_test_collection
 
     item = load_test_data("test_item.json")
     item["collection"] = "wrong-collection-id"
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item,
     )
     assert resp.status_code == 400
 
 
 async def test_create_item_bad_body(
     app_client, load_test_data: Callable, load_test_collection
 ):
     """Items with invalid type should return an error"""
     coll = load_test_collection
 
     item = load_test_data("test_item.json")
     item["type"] = "not-a-type"
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item,
     )
     assert resp.status_code == 400
 
 
 async def test_update_item(app_client, load_test_collection, load_test_item):
     coll = load_test_collection
     item = load_test_item
 
-    item.properties.description = "Update Test"
+    item["properties"]["description"] = "Update Test"
 
     resp = await app_client.put(
-        f"/collections/{coll.id}/items/{item.id}", content=item.json()
+        f"/collections/{coll['id']}/items/{item['id']}", json=item
     )
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 200
-    get_item = Item.parse_obj(resp.json())
-    assert item.dict(exclude={"links"}) == get_item.dict(exclude={"links"})
+    get_item = Item.model_validate(resp.json())
+
+    item = Item(**item)
+    assert item.model_dump(exclude={"links"}) == get_item.model_dump(exclude={"links"})
     assert get_item.properties.description == "Update Test"
 
 
 async def test_delete_item(app_client, load_test_collection, load_test_item):
     coll = load_test_collection
     item = load_test_item
 
-    resp = await app_client.delete(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.delete(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 404
 
 
 async def test_get_collection_items(app_client, load_test_collection, load_test_item):
     coll = load_test_collection
     item = load_test_item
 
     for _ in range(4):
-        item.id = str(uuid.uuid4())
+        item["id"] = str(uuid.uuid4())
         resp = await app_client.post(
-            f"/collections/{coll.id}/items",
-            content=item.json(),
+            f"/collections/{coll['id']}/items",
+            json=item,
         )
-        assert resp.status_code == 200
+        assert resp.status_code == 201
 
     resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
     )
     assert resp.status_code == 200
     fc = resp.json()
     assert "features" in fc
     assert len(fc["features"]) == 5
 
 
@@ -203,25 +214,25 @@
         item = deepcopy(base_item)
         item["id"] = str(uuid.uuid4())
         items.append(item)
 
     item_collection = {"type": "FeatureCollection", "features": items, "links": []}
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item_collection,
     )
 
     assert resp.status_code == 201
 
     resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
     )
     for item in items:
-        resp = await app_client.get(f"/collections/{coll.id}/items/{item['id']}")
+        resp = await app_client.get(f"/collections/{coll['id']}/items/{item['id']}")
         assert resp.status_code == 200
 
 
 async def test_create_item_collection_no_collection_ids(
     app_client, load_test_data: Callable, load_test_collection
 ):
     """Items in ItemCollection with no collection ids should be set with the collection id from the path"""
@@ -234,27 +245,27 @@
         item["id"] = str(uuid.uuid4())
         item["collection"] = None
         items.append(item)
 
     item_collection = {"type": "FeatureCollection", "features": items, "links": []}
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item_collection,
     )
 
     assert resp.status_code == 201
 
     resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
     )
     for item in items:
-        resp = await app_client.get(f"/collections/{coll.id}/items/{item['id']}")
+        resp = await app_client.get(f"/collections/{coll['id']}/items/{item['id']}")
         assert resp.status_code == 200
-        assert resp.json()["collection"] == coll.id
+        assert resp.json()["collection"] == coll["id"]
 
 
 async def test_create_item_collection_invalid_collection_ids(
     app_client, load_test_data: Callable, load_test_collection
 ):
     """Feature collection containing items with invalid collection ids should return an error"""
     coll = load_test_collection
@@ -266,15 +277,15 @@
         item["id"] = str(uuid.uuid4())
         item["collection"] = "wrong-collection-id"
         items.append(item)
 
     item_collection = {"type": "FeatureCollection", "features": items, "links": []}
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item_collection,
     )
 
     assert resp.status_code == 400
 
 
 async def test_create_item_collection_invalid_item_ids(
@@ -289,15 +300,15 @@
         item = deepcopy(base_item)
         item["id"] = str(uuid.uuid4()) + "/bad/id"
         items.append(item)
 
     item_collection = {"type": "FeatureCollection", "features": items, "links": []}
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=item_collection,
     )
 
     assert resp.status_code == 400
 
 
 async def test_create_bulk_items(
@@ -311,22 +322,22 @@
         _item = deepcopy(item)
         _item["id"] = str(uuid.uuid4())
         items[_item["id"]] = _item
 
     payload = {"items": items}
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/bulk_items",
+        f"/collections/{coll['id']}/bulk_items",
         json=payload,
     )
     assert resp.status_code == 200
     assert resp.text == '"Successfully added 2 items."'
 
     for item_id in items.keys():
-        resp = await app_client.get(f"/collections/{coll.id}/items/{item_id}")
+        resp = await app_client.get(f"/collections/{coll['id']}/items/{item_id}")
         assert resp.status_code == 200
 
 
 async def test_create_bulk_items_already_exist_insert(
     app_client, load_test_data: Callable, load_test_collection
 ):
     coll = load_test_collection
@@ -337,28 +348,28 @@
         _item = deepcopy(item)
         _item["id"] = str(uuid.uuid4())
         items[_item["id"]] = _item
 
     payload = {"items": items, "method": "insert"}
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/bulk_items",
+        f"/collections/{coll['id']}/bulk_items",
         json=payload,
     )
     assert resp.status_code == 200
     assert resp.text == '"Successfully added 2 items."'
 
     for item_id in items.keys():
-        resp = await app_client.get(f"/collections/{coll.id}/items/{item_id}")
+        resp = await app_client.get(f"/collections/{coll['id']}/items/{item_id}")
         assert resp.status_code == 200
 
     # Try creating the same items again.
     # This should fail with the default insert behavior.
     resp = await app_client.post(
-        f"/collections/{coll.id}/bulk_items",
+        f"/collections/{coll['id']}/bulk_items",
         json=payload,
     )
     assert resp.status_code == 409
 
 
 async def test_create_bulk_items_already_exist_upsert(
     app_client, load_test_data: Callable, load_test_collection
@@ -371,29 +382,29 @@
         _item = deepcopy(item)
         _item["id"] = str(uuid.uuid4())
         items[_item["id"]] = _item
 
     payload = {"items": items, "method": "insert"}
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/bulk_items",
+        f"/collections/{coll['id']}/bulk_items",
         json=payload,
     )
     assert resp.status_code == 200
     assert resp.text == '"Successfully added 2 items."'
 
     for item_id in items.keys():
-        resp = await app_client.get(f"/collections/{coll.id}/items/{item_id}")
+        resp = await app_client.get(f"/collections/{coll['id']}/items/{item_id}")
         assert resp.status_code == 200
 
     # Try creating the same items again, but using upsert.
     # This should succeed.
     payload["method"] = "upsert"
     resp = await app_client.post(
-        f"/collections/{coll.id}/bulk_items",
+        f"/collections/{coll['id']}/bulk_items",
         json=payload,
     )
     assert resp.status_code == 200
     assert resp.text == '"Successfully upserted 2 items."'
 
 
 # TODO since right now puts implement upsert
@@ -402,18 +413,18 @@
 
 
 # def test_get_collection_items(
 #     postgres_core: CoreCrudClient,
 #     postgres_transactions: TransactionsClient,
 #     load_test_data: Callable,
 # ):
-#     coll = Collection.parse_obj(load_test_data("test_collection.json"))
+#     coll = Collection.model_validate(load_test_data("test_collection.json"))
 #     postgres_transactions.create_collection(coll, request=MockStarletteRequest)
 
-#     item = Item.parse_obj(load_test_data("test_item.json"))
+#     item = Item.model_validate(load_test_data("test_item.json"))
 
 #     for _ in range(5):
 #         item.id = str(uuid.uuid4())
 #         postgres_transactions.create_item(item, request=MockStarletteRequest)
 
 #     fc = postgres_core.item_collection(coll.id, request=MockStarletteRequest)
 #     assert len(fc.features) == 5
```

### Comparing `stac_fastapi_pgstac-2.5.0/tests/resources/test_collection.py` & `stac_fastapi_pgstac-3.0.0a0/tests/resources/test_collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,75 +3,94 @@
 import pystac
 import pytest
 from stac_pydantic import Collection
 
 
 async def test_create_collection(app_client, load_test_data: Callable):
     in_json = load_test_data("test_collection.json")
-    in_coll = Collection.parse_obj(in_json)
+    in_coll = Collection.model_validate(in_json)
     resp = await app_client.post(
         "/collections",
         json=in_json,
     )
-    assert resp.status_code == 200
-    post_coll = Collection.parse_obj(resp.json())
-    assert in_coll.dict(exclude={"links"}) == post_coll.dict(exclude={"links"})
+    assert resp.status_code == 201
+
+    post_coll = Collection.model_validate(resp.json())
+    assert in_coll.model_dump(exclude={"links"}) == post_coll.model_dump(
+        exclude={"links"}
+    )
     resp = await app_client.get(f"/collections/{post_coll.id}")
     assert resp.status_code == 200
-    get_coll = Collection.parse_obj(resp.json())
-    assert post_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
+    get_coll = Collection.model_validate(resp.json())
+    assert post_coll.model_dump(exclude={"links"}) == get_coll.model_dump(
+        exclude={"links"}
+    )
 
-    post_self_link = next((link for link in post_coll.links if link.rel == "self"), None)
-    get_self_link = next((link for link in get_coll.links if link.rel == "self"), None)
+    post_coll = post_coll.model_dump(mode="json")
+    get_coll = get_coll.model_dump(mode="json")
+    post_self_link = next(
+        (link for link in post_coll["links"] if link["rel"] == "self"), None
+    )
+    get_self_link = next(
+        (link for link in get_coll["links"] if link["rel"] == "self"), None
+    )
     assert post_self_link is not None and get_self_link is not None
-    assert post_self_link.href == get_self_link.href
+    assert post_self_link["href"] == get_self_link["href"]
 
 
 async def test_update_collection(app_client, load_test_data, load_test_collection):
     in_coll = load_test_collection
-    in_coll.keywords.append("newkeyword")
+    in_coll["keywords"].append("newkeyword")
 
-    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll['id']}", json=in_coll)
     assert resp.status_code == 200
-    put_coll = Collection.parse_obj(resp.json())
+    put_coll = Collection.model_validate(resp.json())
 
-    resp = await app_client.get(f"/collections/{in_coll.id}")
+    resp = await app_client.get(f"/collections/{in_coll['id']}")
     assert resp.status_code == 200
 
-    get_coll = Collection.parse_obj(resp.json())
-    assert in_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
+    get_coll = Collection.model_validate(resp.json())
+
+    in_coll = Collection(**in_coll)
+    assert in_coll.model_dump(exclude={"links"}) == get_coll.model_dump(exclude={"links"})
     assert "newkeyword" in get_coll.keywords
 
-    put_self_link = next((link for link in put_coll.links if link.rel == "self"), None)
-    get_self_link = next((link for link in get_coll.links if link.rel == "self"), None)
+    get_coll = get_coll.model_dump(mode="json")
+    put_coll = put_coll.model_dump(mode="json")
+    put_self_link = next(
+        (link for link in put_coll["links"] if link["rel"] == "self"), None
+    )
+    get_self_link = next(
+        (link for link in get_coll["links"] if link["rel"] == "self"), None
+    )
     assert put_self_link is not None and get_self_link is not None
-    assert put_self_link.href == get_self_link.href
+    assert put_self_link["href"] == get_self_link["href"]
 
 
 async def test_delete_collection(
     app_client, load_test_data: Callable, load_test_collection
 ):
     in_coll = load_test_collection
 
-    resp = await app_client.delete(f"/collections/{in_coll.id}")
+    resp = await app_client.delete(f"/collections/{in_coll['id']}")
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{in_coll.id}")
+    resp = await app_client.get(f"/collections/{in_coll['id']}")
     assert resp.status_code == 404
 
 
 async def test_create_collection_conflict(app_client, load_test_data: Callable):
     in_json = load_test_data("test_collection.json")
-    Collection.parse_obj(in_json)
+    Collection.model_validate(in_json)
     resp = await app_client.post(
         "/collections",
         json=in_json,
     )
-    assert resp.status_code == 200
-    Collection.parse_obj(resp.json())
+    assert resp.status_code == 201
+    Collection.model_validate(resp.json())
     resp = await app_client.post(
         "/collections",
         json=in_json,
     )
     assert resp.status_code == 409
 
 
@@ -80,17 +99,17 @@
 ):
     resp = await app_client.delete("/collections")
     assert resp.status_code == 405
 
 
 async def test_update_new_collection(app_client, load_test_collection):
     in_coll = load_test_collection
-    in_coll.id = "test-updatenew"
+    in_coll["id"] = "test-updatenew"
 
-    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll['id']}", json=in_coll)
     assert resp.status_code == 404
 
 
 async def test_nocollections(
     app_client,
 ):
     resp = await app_client.get("/collections")
@@ -100,15 +119,15 @@
 async def test_returns_valid_collection(app_client, load_test_data):
     """Test updating a collection which already exists"""
     in_json = load_test_data("test_collection.json")
     resp = await app_client.post(
         "/collections",
         json=in_json,
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     resp = await app_client.get(f"/collections/{in_json['id']}")
     assert resp.status_code == 200
     resp_json = resp.json()
 
     # Mock root to allow validation
     mock_root = pystac.Catalog(
@@ -123,15 +142,15 @@
 async def test_returns_valid_links_in_collections(app_client, load_test_data):
     """Test links from listing collections"""
     in_json = load_test_data("test_collection.json")
     resp = await app_client.post(
         "/collections",
         json=in_json,
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # Get collection by ID
     resp = await app_client.get(f"/collections/{in_json['id']}")
     assert resp.status_code == 200
     resp_json = resp.json()
 
     # Mock root to allow validation
@@ -168,41 +187,41 @@
         if i not in single_coll_mocked_link.to_dict()["links"]
     ] == []
 
 
 async def test_returns_license_link(app_client, load_test_collection):
     coll = load_test_collection
 
-    resp = await app_client.get(f"/collections/{coll.id}")
+    resp = await app_client.get(f"/collections/{coll['id']}")
     assert resp.status_code == 200
     resp_json = resp.json()
     link_rel_types = [link["rel"] for link in resp_json["links"]]
     assert "license" in link_rel_types
 
 
 @pytest.mark.asyncio
 async def test_get_collection_forwarded_header(app_client, load_test_collection):
     coll = load_test_collection
     resp = await app_client.get(
-        f"/collections/{coll.id}",
+        f"/collections/{coll['id']}",
         headers={"Forwarded": "proto=https;host=test:1234"},
     )
     for link in [
         link
         for link in resp.json()["links"]
         if link["rel"] in ["items", "parent", "root", "self"]
     ]:
         assert link["href"].startswith("https://test:1234/")
 
 
 @pytest.mark.asyncio
 async def test_get_collection_x_forwarded_headers(app_client, load_test_collection):
     coll = load_test_collection
     resp = await app_client.get(
-        f"/collections/{coll.id}",
+        f"/collections/{coll['id']}",
         headers={
             "X-Forwarded-Port": "1234",
             "X-Forwarded-Proto": "https",
         },
     )
     for link in [
         link
@@ -214,15 +233,15 @@
 
 @pytest.mark.asyncio
 async def test_get_collection_duplicate_forwarded_headers(
     app_client, load_test_collection
 ):
     coll = load_test_collection
     resp = await app_client.get(
-        f"/collections/{coll.id}",
+        f"/collections/{coll['id']}",
         headers={
             "Forwarded": "proto=https;host=test:1234",
             "X-Forwarded-Port": "4321",
             "X-Forwarded-Proto": "http",
         },
     )
     for link in [
```

### Comparing `stac_fastapi_pgstac-2.5.0/tests/resources/test_conformance.py` & `stac_fastapi_pgstac-3.0.0a0/tests/resources/test_conformance.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-2.5.0/tests/resources/test_item.py` & `stac_fastapi_pgstac-3.0.0a0/tests/resources/test_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,116 +17,134 @@
 from starlette.requests import Request
 
 from stac_fastapi.pgstac.models.links import CollectionLinks
 
 
 async def test_create_collection(app_client, load_test_data: Callable):
     in_json = load_test_data("test_collection.json")
-    in_coll = Collection.parse_obj(in_json)
+    in_coll = Collection.model_validate(in_json)
     resp = await app_client.post(
         "/collections",
         json=in_json,
     )
-    assert resp.status_code == 200
-    post_coll = Collection.parse_obj(resp.json())
-    assert in_coll.dict(exclude={"links"}) == post_coll.dict(exclude={"links"})
+    assert resp.status_code == 201
+    post_coll = Collection.model_validate(resp.json())
+    assert in_coll.model_dump(exclude={"links"}) == post_coll.model_dump(
+        exclude={"links"}
+    )
     resp = await app_client.get(f"/collections/{post_coll.id}")
     assert resp.status_code == 200
-    get_coll = Collection.parse_obj(resp.json())
-    assert post_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
+    get_coll = Collection.model_validate(resp.json())
+    assert post_coll.model_dump(exclude={"links"}) == get_coll.model_dump(
+        exclude={"links"}
+    )
 
 
 async def test_update_collection(app_client, load_test_data, load_test_collection):
     in_coll = load_test_collection
-    in_coll.keywords.append("newkeyword")
+    in_coll = load_test_data("test_collection.json")
+    in_coll["keywords"].append("newkeyword")
 
-    resp = await app_client.put(f"/collections/{in_coll.id}", json=in_coll.dict())
+    resp = await app_client.put(f"/collections/{in_coll['id']}", json=in_coll)
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{in_coll.id}")
+    resp = await app_client.get(f"/collections/{in_coll['id']}")
     assert resp.status_code == 200
 
-    get_coll = Collection.parse_obj(resp.json())
-    assert in_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
+    get_coll = Collection.model_validate(resp.json())
+
+    in_coll = Collection(**in_coll)
+    assert in_coll.model_dump(exclude={"links"}) == get_coll.model_dump(exclude={"links"})
     assert "newkeyword" in get_coll.keywords
 
 
 async def test_delete_collection(
     app_client, load_test_data: Callable, load_test_collection
 ):
     in_coll = load_test_collection
 
-    resp = await app_client.delete(f"/collections/{in_coll.id}")
+    resp = await app_client.delete(f"/collections/{in_coll['id']}")
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{in_coll.id}")
+    resp = await app_client.get(f"/collections/{in_coll['id']}")
     assert resp.status_code == 404
 
 
 async def test_create_item(app_client, load_test_data: Callable, load_test_collection):
     coll = load_test_collection
 
     in_json = load_test_data("test_item.json")
-    in_item = Item.parse_obj(in_json)
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=in_json,
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
-    post_item = Item.parse_obj(resp.json())
-    assert in_item.dict(exclude={"links"}) == post_item.dict(exclude={"links"})
+    in_item = Item.model_validate(in_json)
+    post_item = Item.model_validate(resp.json())
+    assert in_item.model_dump(exclude={"links"}) == post_item.model_dump(
+        exclude={"links"}
+    )
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{post_item.id}")
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{post_item.id}")
 
     assert resp.status_code == 200
-    get_item = Item.parse_obj(resp.json())
-    assert in_item.dict(exclude={"links"}) == get_item.dict(exclude={"links"})
+    get_item = Item.model_validate(resp.json())
+    assert in_item.model_dump(exclude={"links"}) == get_item.model_dump(exclude={"links"})
 
-    post_self_link = next((link for link in post_item.links if link.rel == "self"), None)
-    get_self_link = next((link for link in get_item.links if link.rel == "self"), None)
+    get_item = get_item.model_dump(mode="json")
+    post_item = post_item.model_dump(mode="json")
+    post_self_link = next(
+        (link for link in post_item["links"] if link["rel"] == "self"), None
+    )
+    get_self_link = next(
+        (link for link in get_item["links"] if link["rel"] == "self"), None
+    )
     assert post_self_link is not None and get_self_link is not None
-    assert post_self_link.href == get_self_link.href
+    assert post_self_link["href"] == get_self_link["href"]
 
 
 async def test_create_item_mismatched_collection_id(
     app_client, load_test_data: Callable, load_test_collection
 ):
     # If the collection_id path parameter and the Item's "collection" property do not match, a 400 response should
     # be returned.
     coll = load_test_collection
 
     in_json = load_test_data("test_item.json")
     in_json["collection"] = random.choice(ascii_letters)
-    assert in_json["collection"] != coll.id
+    assert in_json["collection"] != coll["id"]
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=in_json,
     )
     assert resp.status_code == 400
 
 
 async def test_fetches_valid_item(
     app_client, load_test_data: Callable, load_test_collection
 ):
     coll = load_test_collection
 
     in_json = load_test_data("test_item.json")
-    in_item = Item.parse_obj(in_json)
+
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=in_json,
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
-    post_item = Item.parse_obj(resp.json())
-    assert in_item.dict(exclude={"links"}) == post_item.dict(exclude={"links"})
+    in_item = Item.model_validate(in_json)
+    post_item = Item.model_validate(resp.json())
+    assert in_item.model_dump(exclude={"links"}) == post_item.model_dump(
+        exclude={"links"}
+    )
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{post_item.id}")
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{post_item.id}")
 
     assert resp.status_code == 200
     item_dict = resp.json()
     # Mock root to allow validation
     mock_root = pystac.Catalog(
         id="test", description="test desc", href="https://example.com"
     )
@@ -136,177 +154,185 @@
 
 async def test_update_item(
     app_client, load_test_data: Callable, load_test_collection, load_test_item
 ):
     coll = load_test_collection
     item = load_test_item
 
-    item.properties.description = "Update Test"
+    item["properties"]["description"] = "Update Test"
 
     resp = await app_client.put(
-        f"/collections/{coll.id}/items/{item.id}", content=item.json()
+        f"/collections/{coll['id']}/items/{item['id']}", json=item
     )
     assert resp.status_code == 200
-    put_item = Item.parse_obj(resp.json())
+    put_item = Item.model_validate(resp.json())
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 200
 
-    get_item = Item.parse_obj(resp.json())
-    assert item.dict(exclude={"links"}) == get_item.dict(exclude={"links"})
+    get_item = Item.model_validate(resp.json())
+    item = Item(**item)
+    assert item.model_dump(exclude={"links"}) == get_item.model_dump(exclude={"links"})
     assert get_item.properties.description == "Update Test"
 
-    post_self_link = next((link for link in put_item.links if link.rel == "self"), None)
-    get_self_link = next((link for link in get_item.links if link.rel == "self"), None)
+    put_item = put_item.model_dump(mode="json")
+    get_item = get_item.model_dump(mode="json")
+    post_self_link = next(
+        (link for link in put_item["links"] if link["rel"] == "self"), None
+    )
+    get_self_link = next(
+        (link for link in get_item["links"] if link["rel"] == "self"), None
+    )
     assert post_self_link is not None and get_self_link is not None
-    assert post_self_link.href == get_self_link.href
+    assert post_self_link["href"] == get_self_link["href"]
 
 
 async def test_update_item_mismatched_collection_id(
     app_client, load_test_data: Callable, load_test_collection, load_test_item
 ) -> None:
     coll = load_test_collection
 
     in_json = load_test_data("test_item.json")
 
     in_json["collection"] = random.choice(ascii_letters)
-    assert in_json["collection"] != coll.id
+    assert in_json["collection"] != coll["id"]
 
     item_id = in_json["id"]
 
     resp = await app_client.put(
-        f"/collections/{coll.id}/items/{item_id}",
+        f"/collections/{coll['id']}/items/{item_id}",
         json=in_json,
     )
     assert resp.status_code == 400
 
 
 async def test_delete_item(
     app_client, load_test_data: Callable, load_test_collection, load_test_item
 ):
     coll = load_test_collection
     item = load_test_item
 
-    resp = await app_client.delete(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.delete(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.get(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 404
 
 
-async def test_get_collection_items(app_client, load_test_collection, load_test_item):
+async def test_get_collection_items(
+    app_client, load_test_collection, load_test_item, load_test_data
+):
     coll = load_test_collection
-    item = load_test_item
+    item = load_test_data("test_item.json")
 
     for _ in range(4):
-        item.id = str(uuid.uuid4())
+        item["id"] = str(uuid.uuid4())
         resp = await app_client.post(
-            f"/collections/{coll.id}/items",
-            content=item.json(),
+            f"/collections/{coll['id']}/items",
+            json=item,
         )
-        assert resp.status_code == 200
+        assert resp.status_code == 201
 
     resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
     )
     assert resp.status_code == 200
     fc = resp.json()
     assert "features" in fc
     assert len(fc["features"]) == 5
 
 
 async def test_create_item_conflict(
     app_client, load_test_data: Callable, load_test_collection
 ):
     coll = load_test_collection
     in_json = load_test_data("test_item.json")
-    Item.parse_obj(in_json)
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=in_json,
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         json=in_json,
     )
     assert resp.status_code == 409
 
 
 async def test_delete_missing_item(
     app_client, load_test_data: Callable, load_test_collection, load_test_item
 ):
     coll = load_test_collection
     item = load_test_item
 
-    resp = await app_client.delete(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.delete(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 200
 
-    resp = await app_client.delete(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.delete(f"/collections/{coll['id']}/items/{item['id']}")
     assert resp.status_code == 404
 
 
 async def test_create_item_missing_collection(
     app_client, load_test_data: Callable, load_test_collection
 ):
     coll = load_test_collection
     item = load_test_data("test_item.json")
     item["collection"] = None
 
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+    assert resp.status_code == 201
 
     post_item = resp.json()
-    assert post_item["collection"] == coll.id
+    assert post_item["collection"] == coll["id"]
 
 
 async def test_update_new_item(
-    app_client, load_test_data: Callable, load_test_collection, load_test_item
+    app_client, load_test_data: Callable, load_test_collection
 ):
     coll = load_test_collection
-    item = load_test_item
-    item.id = "test-updatenewitem"
+
+    new_item = load_test_data("test_item.json")
+    new_item["id"] = "test-updatenewitem"
 
     resp = await app_client.put(
-        f"/collections/{coll.id}/items/{item.id}", content=item.json()
+        f"/collections/{coll['id']}/items/{new_item['id']}", json=new_item
     )
     assert resp.status_code == 404
 
 
 async def test_update_item_missing_collection(
     app_client, load_test_data: Callable, load_test_collection, load_test_item
 ):
     coll = load_test_collection
     item = load_test_item
-    item.collection = None
+    item["collection"] = None
 
     resp = await app_client.put(
-        f"/collections/{coll.id}/items/{item.id}", content=item.json()
+        f"/collections/{coll['id']}/items/{item['id']}", json=item
     )
     assert resp.status_code == 200
 
     put_item = resp.json()
-    assert put_item["collection"] == coll.id
+    assert put_item["collection"] == coll["id"]
 
 
 async def test_pagination(app_client, load_test_data, load_test_collection):
     """Test item collection pagination (paging extension)"""
     coll = load_test_collection
     item_count = 21
-    test_item = load_test_data("test_item.json")
 
     for idx in range(1, item_count):
-        item = Item.parse_obj(test_item)
-        item.id = item.id + str(idx)
-        item.properties.datetime = f"2020-01-{idx:02d}T00:00:00"
-        resp = await app_client.post(f"/collections/{coll.id}/items", json=item.dict())
-        assert resp.status_code == 200
+        item = load_test_data("test_item.json")
+        item["id"] = item["id"] + str(idx)
+        item["properties"]["datetime"] = f"2020-01-{idx:02d}T00:00:00Z"
+        resp = await app_client.post(f"/collections/{coll['id']}/items", json=item)
+        assert resp.status_code == 201
 
-    resp = await app_client.get(f"/collections/{coll.id}/items", params={"limit": 3})
+    resp = await app_client.get(f"/collections/{coll['id']}/items", params={"limit": 3})
     assert resp.status_code == 200
     first_page = resp.json()
     assert len(first_page["features"]) == 3
 
     nextlink = [
         link["href"] for link in first_page["links"] if link["rel"] == "next"
     ].pop()
@@ -358,15 +384,15 @@
     ids = ["test1", "test2", "test3"]
     for id in ids:
         test_item = load_test_data("test_item.json")
         test_item["id"] = id
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
-        assert resp.status_code == 200
+        assert resp.status_code == 201
 
     params = {"collections": [test_item["collection"]], "ids": ids}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == len(ids)
     assert {feat["id"] for feat in resp_json["features"]} == set(ids)
@@ -391,22 +417,22 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with spatial query (core)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # Add second item with a different datetime.
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     params = {
         "collections": [test_item["collection"]],
         "intersects": test_item["geometry"],
     }
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
@@ -419,22 +445,22 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with single-tailed spatio-temporal query (core)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # Add second item with a different datetime.
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     item_date = rfc3339_str_to_datetime(test_item["properties"]["datetime"])
 
     params = {
         "collections": [test_item["collection"]],
         "intersects": test_item["geometry"],
         "datetime": datetime_to_str(item_date),
@@ -450,22 +476,22 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with two-tailed spatio-temporal query (core)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # Add second item with a different datetime.
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     item_date = rfc3339_str_to_datetime(test_item["properties"]["datetime"])
     item_date_before = item_date - timedelta(seconds=1)
     item_date_after = item_date + timedelta(seconds=1)
 
     params = {
         "collections": [test_item["collection"]],
@@ -489,24 +515,24 @@
 async def test_item_search_sort_post(app_client, load_test_data, load_test_collection):
     """Test POST search with sorting (sort extension)"""
     first_item = load_test_data("test_item.json")
     item_date = rfc3339_str_to_datetime(first_item["properties"]["datetime"])
     resp = await app_client.post(
         f"/collections/{first_item['collection']}/items", json=first_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_item = load_test_data("test_item.json")
     second_item["id"] = "another-item"
     another_item_date = item_date - timedelta(days=1)
     second_item["properties"]["datetime"] = datetime_to_str(another_item_date)
     resp = await app_client.post(
         f"/collections/{second_item['collection']}/items", json=second_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     params = {
         "collections": [first_item["collection"]],
         "sortby": [{"field": "datetime", "direction": "desc"}],
     }
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
@@ -520,15 +546,15 @@
     ids = ["test1", "test2", "test3"]
     for id in ids:
         test_item = load_test_data("test_item.json")
         test_item["id"] = id
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
-        assert resp.status_code == 200
+        assert resp.status_code == 201
 
     params = {"collections": test_item["collection"], "ids": ",".join(ids)}
     resp = await app_client.get("/search", params=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == len(ids)
     assert {feat["id"] for feat in resp_json["features"]} == set(ids)
@@ -536,22 +562,22 @@
 
 async def test_item_search_bbox_get(app_client, load_test_data, load_test_collection):
     """Test GET search with spatial query (core)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # Add second item with a different datetime.
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     params = {
         "collections": test_item["collection"],
         "bbox": ",".join([str(coord) for coord in test_item["bbox"]]),
     }
     resp = await app_client.get("/search", params=params)
     assert resp.status_code == 200
@@ -564,22 +590,22 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test GET search without specifying collections"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # Add second item with a different datetime.
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     params = {
         "bbox": ",".join([str(coord) for coord in test_item["bbox"]]),
     }
     resp = await app_client.get("/search", params=params)
     assert resp.status_code == 200
     resp_json = resp.json()
@@ -591,22 +617,22 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test GET search with spatio-temporal query (core)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # Add second item with a different datetime.
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     item_date = rfc3339_str_to_datetime(test_item["properties"]["datetime"])
     item_date_before = item_date - timedelta(seconds=1)
     item_date_after = item_date + timedelta(seconds=1)
 
     params = {
         "collections": test_item["collection"],
@@ -621,24 +647,24 @@
 async def test_item_search_sort_get(app_client, load_test_data, load_test_collection):
     """Test GET search with sorting (sort extension)"""
     first_item = load_test_data("test_item.json")
     item_date = rfc3339_str_to_datetime(first_item["properties"]["datetime"])
     resp = await app_client.post(
         f"/collections/{first_item['collection']}/items", json=first_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_item = load_test_data("test_item.json")
     second_item["id"] = "another-item"
     another_item_date = item_date - timedelta(days=1)
     second_item["properties"]["datetime"] = datetime_to_str(another_item_date)
     resp = await app_client.post(
         f"/collections/{second_item['collection']}/items", json=second_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
     params = {"collections": [first_item["collection"]], "sortby": "-datetime"}
     resp = await app_client.get("/search", params=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert resp_json["features"][0]["id"] == first_item["id"]
     assert resp_json["features"][1]["id"] == second_item["id"]
 
@@ -647,21 +673,21 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search without specifying a collection"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     params = {
         "bbox": test_item["bbox"],
     }
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
@@ -672,21 +698,21 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with JSONB query (query extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # EPSG is a JSONB key
     params = {"query": {"proj:epsg": {"gt": test_item["properties"]["proj:epsg"] - 1}}}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
@@ -696,22 +722,22 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search indexed field with query (query extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_test_item = load_test_data("test_item2.json")
     second_test_item["properties"]["eo:cloud_cover"] = 5
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     params = {"query": {"eo:cloud_cover": {"eq": 0}}}
     resp = await app_client.post("/search", json=params)
     assert resp.status_code == 200
     resp_json = resp.json()
     assert len(resp_json["features"]) == 1
 
@@ -720,21 +746,21 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test GET search with JSONB query (query extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # EPSG is a JSONB key
     params = {
         "collections": [test_item["collection"]],
         "query": json.dumps(
             {"proj:epsg": {"gt": test_item["properties"]["proj:epsg"] + 1}}
         ),
@@ -760,21 +786,21 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with JSONB query (cql json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # EPSG is a JSONB key
     params = {
         "collections": [test_item["collection"]],
         "filter": {
             "gt": [
                 {"property": "proj:epsg"},
@@ -810,21 +836,21 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with JSONB query (cql2 json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # EPSG is a JSONB key
     params = {
         "collections": [test_item["collection"]],
         "filter-lang": "cql2-json",
         "filter": {
             "op": "gt",
@@ -864,21 +890,21 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with JSONB query (cql2 json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     second_test_item = load_test_data("test_item2.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=second_test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # EPSG is a JSONB key
     params = {
         "collections": [test_item["collection"]],
         "filter-lang": "cql2-json",
         "filter": {
             "op": "gt",
@@ -915,15 +941,15 @@
     # Ingest 5 items
     for _ in range(5):
         uid = str(uuid.uuid4())
         test_item["id"] = uid
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
-        assert resp.status_code == 200
+        assert resp.status_code == 201
         ids.append(uid)
 
     # Paginate through all 5 items with a limit of 1 (expecting 5 requests)
     page = await app_client.get(
         f"/collections/{test_item['collection']}/items", params={"limit": 1}
     )
     idx = 0
@@ -955,15 +981,15 @@
     # Ingest 5 items
     for _ in range(5):
         uid = str(uuid.uuid4())
         test_item["id"] = uid
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
-        assert resp.status_code == 200
+        assert resp.status_code == 201
         ids.append(uid)
 
     # Paginate through all 5 items with a limit of 1 (expecting 5 requests)
     request_body = {
         "filter-lang": "cql2-json",
         "filter": {"op": "in", "args": [{"property": "id"}, ids]},
         "limit": 1,
@@ -1002,15 +1028,15 @@
     # Ingest 5 items
     for _ in range(5):
         uid = str(uuid.uuid4())
         test_item["id"] = uid
         resp = await app_client.post(
             f"/collections/{test_item['collection']}/items", json=test_item
         )
-        assert resp.status_code == 200
+        assert resp.status_code == 201
         ids.append(uid)
 
     page = await app_client.post(
         "/search",
         json={
             "filter-lang": "cql2-json",
             "filter": {"op": "in", "args": [{"property": "id"}, ids]},
@@ -1038,29 +1064,29 @@
 
 async def test_field_extension_get(app_client, load_test_data, load_test_collection):
     """Test GET search with included fields (fields extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     params = {"fields": "+properties.proj:epsg,+properties.gsd,+collection"}
     resp = await app_client.get("/search", params=params)
     feat_properties = resp.json()["features"][0]["properties"]
     assert not set(feat_properties) - {"proj:epsg", "gsd", "datetime"}
 
 
 async def test_field_extension_post(app_client, load_test_data, load_test_collection):
     """Test POST search with included and excluded fields (fields extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     body = {
         "fields": {
             "exclude": ["assets.B1"],
             "include": [
                 "properties.eo:cloud_cover",
                 "properties.orientation",
@@ -1084,15 +1110,15 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search including/excluding same field (fields extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     body = {
         "fields": {
             "exclude": ["properties.eo:cloud_cover"],
             "include": ["properties.eo:cloud_cover", "collection"],
         }
     }
@@ -1106,15 +1132,15 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search excluding a forbidden field (fields extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     body = {"fields": {"exclude": ["geometry"]}}
 
     resp = await app_client.post("/search", json=body)
     resp_json = resp.json()
     assert "geometry" not in resp_json["features"][0]
 
@@ -1264,19 +1290,19 @@
 async def test_preserves_extra_link(
     app_client: AsyncClient, load_test_data, load_test_collection
 ):
     coll = load_test_collection
     test_item = load_test_data("test_item.json")
     expected_href = urljoin(str(app_client.base_url), "preview.html")
 
-    resp = await app_client.post(f"/collections/{coll.id}/items", json=test_item)
-    assert resp.status_code == 200
+    resp = await app_client.post(f"/collections/{coll['id']}/items", json=test_item)
+    assert resp.status_code == 201
 
     response_item = await app_client.get(
-        f"/collections/{coll.id}/items/{test_item['id']}",
+        f"/collections/{coll['id']}/items/{test_item['id']}",
         params={"limit": 1},
     )
     assert response_item.status_code == 200
     item = response_item.json()
     extra_link = [link for link in item["links"] if link["rel"] == "preview"]
     assert extra_link
     assert extra_link[0]["href"] == expected_href
@@ -1286,15 +1312,15 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with JSONB query (cql json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # EPSG is a JSONB key
     params = {
         "collections": [test_item["collection"]],
         "filter-lang": "cql-json",
         "filter": {
             "gt": [
@@ -1332,15 +1358,15 @@
     app_client, load_test_data, load_test_collection
 ):
     """Test POST search with JSONB query (cql json filter extension)"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     # EPSG is a JSONB key
     params = {
         "filter-lang": "cql2-json",
         "filter": {
             "op": "and",
             "args": [
@@ -1420,15 +1446,15 @@
 
 async def test_get_filter_cql2text(app_client, load_test_data, load_test_collection):
     """Test GET search with cql2-text"""
     test_item = load_test_data("test_item.json")
     resp = await app_client.post(
         f"/collections/{test_item['collection']}/items", json=test_item
     )
-    assert resp.status_code == 200
+    assert resp.status_code == 201
 
     epsg = test_item["properties"]["proj:epsg"]
     collection = test_item["collection"]
 
     filter = f"proj:epsg={epsg} AND collection = '{collection}'"
     params = {"filter": filter, "filter-lang": "cql2-text"}
     resp = await app_client.get("/search", params=params)
@@ -1464,28 +1490,28 @@
 
 @pytest.mark.asyncio
 async def test_get_collection_items_forwarded_header(
     app_client, load_test_collection, load_test_item
 ):
     coll = load_test_collection
     resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         headers={"Forwarded": "proto=https;host=test:1234"},
     )
     for link in resp.json()["features"][0]["links"]:
         assert link["href"].startswith("https://test:1234/")
 
 
 @pytest.mark.asyncio
 async def test_get_collection_items_x_forwarded_headers(
     app_client, load_test_collection, load_test_item
 ):
     coll = load_test_collection
     resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         headers={
             "X-Forwarded-Port": "1234",
             "X-Forwarded-Proto": "https",
         },
     )
     for link in resp.json()["features"][0]["links"]:
         assert link["href"].startswith("https://test:1234/")
@@ -1493,15 +1519,15 @@
 
 @pytest.mark.asyncio
 async def test_get_collection_items_duplicate_forwarded_headers(
     app_client, load_test_collection, load_test_item
 ):
     coll = load_test_collection
     resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+        f"/collections/{coll['id']}/items",
         headers={
             "Forwarded": "proto=https;host=test:1234",
             "X-Forwarded-Port": "4321",
             "X-Forwarded-Proto": "http",
         },
     )
     for link in resp.json()["features"][0]["links"]:
```

