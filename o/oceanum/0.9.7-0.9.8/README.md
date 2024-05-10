# Comparing `tmp/oceanum-0.9.7.tar.gz` & `tmp/oceanum-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.9.7.tar", last modified: Wed Aug 23 03:09:34 2023, max compression
+gzip compressed data, was "oceanum-0.9.8.tar", last modified: Tue Aug 29 03:30:56 2023, max compression
```

## Comparing `oceanum-0.9.7.tar` & `oceanum-0.9.8.tar`

### file list

```diff
@@ -1,76 +1,38 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.849189 oceanum-0.9.7/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.9.7/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.9.7/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.9.7/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.9.7/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1112 2023-08-23 03:09:34.849189 oceanum-0.9.7/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.9.7/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.837189 oceanum-0.9.7/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.829189 oceanum-0.9.7/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.829189 oceanum-0.9.7/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.837189 oceanum-0.9.7/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2022-12-01 21:44:17.000000 oceanum-0.9.7/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.9.7/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.9.7/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.829189 oceanum-0.9.7/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.837189 oceanum-0.9.7/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      741 2023-08-08 22:43:41.000000 oceanum-0.9.7/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.829189 oceanum-0.9.7/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.837189 oceanum-0.9.7/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/classes/datamesh/oceanum.datamesh.Query.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.841189 oceanum-0.9.7/docs/classes/storage/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2388 2023-08-08 22:44:06.000000 oceanum-0.9.7/docs/classes/storage/oceanum.storage.FileSystem.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5658 2023-08-23 03:05:10.000000 oceanum-0.9.7/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.9.7/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-08-23 03:05:34.000000 oceanum-0.9.7/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      384 2023-08-23 03:05:34.000000 oceanum-0.9.7/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      240 2023-08-08 22:45:14.000000 oceanum-0.9.7/docs/oceanum.storage.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.9.7/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.841189 oceanum-0.9.7/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      656 2023-08-23 03:08:37.000000 oceanum-0.9.7/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.9.7/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.841189 oceanum-0.9.7/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.9.7/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.9.7/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    21330 2023-07-30 21:15:42.000000 oceanum-0.9.7/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-30 20:00:11.000000 oceanum-0.9.7/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      186 2023-07-31 20:33:46.000000 oceanum-0.9.7/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7855 2023-08-17 02:43:31.000000 oceanum-0.9.7/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.9.7/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.841189 oceanum-0.9.7/oceanum/storage/
--rw-rw-r--   0 dave      (1000) dave      (1000)       35 2023-08-07 20:38:45.000000 oceanum-0.9.7/oceanum/storage/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11413 2023-08-23 03:07:20.000000 oceanum-0.9.7/oceanum/storage/filesystem.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.841189 oceanum-0.9.7/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1112 2023-08-23 03:09:34.000000 oceanum-0.9.7/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1529 2023-08-23 03:09:34.000000 oceanum-0.9.7/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-08-23 03:09:34.000000 oceanum-0.9.7/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       98 2023-08-23 03:09:34.000000 oceanum-0.9.7/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-08-23 03:09:34.000000 oceanum-0.9.7/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      133 2023-08-23 03:09:34.000000 oceanum-0.9.7/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-08-23 03:09:34.000000 oceanum-0.9.7/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-08-23 03:09:34.849189 oceanum-0.9.7/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1400 2023-08-17 19:56:14.000000 oceanum-0.9.7/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.845189 oceanum-0.9.7/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-23 03:09:34.849189 oceanum-0.9.7/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.9.7/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1619 2023-08-23 03:03:21.000000 oceanum-0.9.7/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2018 2023-08-23 03:08:29.000000 oceanum-0.9.7/tests/test_storage.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.9.7/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-29 03:30:56.328179 oceanum-0.9.8/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.9.8/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.9.8/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3332 2023-08-29 03:30:56.328179 oceanum-0.9.8/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.9.8/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-29 03:30:56.324180 oceanum-0.9.8/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      656 2023-08-29 03:24:56.000000 oceanum-0.9.8/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.9.8/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-29 03:30:56.328179 oceanum-0.9.8/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.9.8/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.9.8/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21330 2023-07-30 21:15:42.000000 oceanum-0.9.8/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11419 2023-08-29 03:26:00.000000 oceanum-0.9.8/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      186 2023-07-31 20:33:46.000000 oceanum-0.9.8/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7855 2023-08-17 02:43:31.000000 oceanum-0.9.8/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.9.8/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-29 03:30:56.328179 oceanum-0.9.8/oceanum/storage/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       35 2023-08-07 20:38:45.000000 oceanum-0.9.8/oceanum/storage/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11430 2023-08-23 03:28:25.000000 oceanum-0.9.8/oceanum/storage/filesystem.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-29 03:30:56.324180 oceanum-0.9.8/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3332 2023-08-29 03:30:56.000000 oceanum-0.9.8/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      760 2023-08-29 03:30:56.000000 oceanum-0.9.8/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-08-29 03:30:56.000000 oceanum-0.9.8/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       98 2023-08-29 03:30:56.000000 oceanum-0.9.8/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      232 2023-08-29 03:30:56.000000 oceanum-0.9.8/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       24 2023-08-29 03:30:56.000000 oceanum-0.9.8/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1977 2023-08-29 03:29:29.000000 oceanum-0.9.8/pyproject.toml
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-08-29 03:30:56.328179 oceanum-0.9.8/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-29 03:30:56.328179 oceanum-0.9.8/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.9.8/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.9.8/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.9.8/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.9.8/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.9.8/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.9.8/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1619 2023-08-23 03:03:21.000000 oceanum-0.9.8/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2018 2023-08-23 03:08:29.000000 oceanum-0.9.8/tests/test_storage.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      824 2023-08-29 03:26:00.000000 oceanum-0.9.8/tests/test_video_compat.py
```

### Comparing `oceanum-0.9.7/LICENSE` & `oceanum-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/PKG-INFO` & `oceanum-0.9.8/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: oceanum
-Version: 0.9.7
-Summary: Library for oceanum.io services
-Home-page: https://github.com/oceanum/oceanum-python
-Author: Oceanum Developers
-Author-email: developers@oceanum.science
-License: MIT license
-Keywords: oceanum
-Requires-Python: >=3.8
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ==============
 oceanum-python
 ==============
 
 
 .. image:: https://img.shields.io/pypi/v/oceanum.svg
         :target: https://pypi.python.org/pypi/oceanum
```

### Comparing `oceanum-0.9.7/oceanum/__init__.py` & `oceanum-0.9.8/oceanum/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for oceanum."""
 
 __author__ = """Oceanum Developers"""
 __email__ = "developers@oceanum.science"
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 
 
 # Suppress tracebacks in an ipython environment
 try:
     import sys
 
     ipython = get_ipython()
```

### Comparing `oceanum-0.9.7/oceanum/datamesh/catalog.py` & `oceanum-0.9.8/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/oceanum/datamesh/connection.py` & `oceanum-0.9.8/oceanum/datamesh/connection.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/oceanum/datamesh/datasource.py` & `oceanum-0.9.8/oceanum/datamesh/datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ConfigDict,
     BaseModel,
     Field,
     AnyHttpUrl,
     PrivateAttr,
     constr,
     BeforeValidator,
+    field_validator,
 )
 from pydantic_core import core_schema
 from pydantic.json import timedelta_isoformat
 from typing_extensions import Annotated
 from typing import Optional, Dict, Union, List, NamedTuple
 from enum import Enum
 from .query import Query, Timestamp
@@ -174,16 +175,14 @@
     """Datasource"""
 
     id: str = Field(
         title="Datasource ID",
         description="Unique ID for the datasource",
         min_length=3,
         max_length=80,
-        strip_whitespace=True,
-        to_lower=True,
         pattern=r"^[a-z0-9-_]+$",
     )
     name: str = Field(
         title="Datasource name",
         description="Human readable name for the datasource",
         max_length=64,
     )
@@ -276,14 +275,19 @@
     driver: str = Field(frozen=True)
     _exists: bool = PrivateAttr(default=False)
     _detail: bool = PrivateAttr(default=False)
     # TODO[pydantic]: The following keys were removed: `json_encoders`.
     # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.
     model_config = ConfigDict(use_enum_values=True, validate_assignment=True)
 
+    @field_validator("id")
+    @classmethod
+    def validate_id(cls, v: str) -> str:
+        return v.lower().strip()
+
     def __str__(self):
         if self._detail:
             return f"""
         {self.name} [{self.id}]
             Extent: {self.bounds}
             Timerange: {self.tstart} to {self.tend}
             {len(self.attributes)} attributes
```

### Comparing `oceanum-0.9.7/oceanum/datamesh/query.py` & `oceanum-0.9.8/oceanum/datamesh/query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/oceanum/datamesh/zarr.py` & `oceanum-0.9.8/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/oceanum/storage/filesystem.py` & `oceanum-0.9.8/oceanum/storage/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def __init__(
         self,
         token=None,
         service=os.environ.get("STORAGE_SERVICE", DEFAULT_CONFIG["STORAGE_SERVICE"]),
         asynchronous=False,
         loop=None,
         timeout=3600,
-        batch_size=16,
+        batch_size=_DEFAULT_BATCH_SIZE,
     ):
         """Storage filesystem constructor
 
         Args:
             token (string): Your datamesh access token. Defaults to os.environ.get("DATAMESH_TOKEN", None).
             service (string, optional): URL of datamesh service. Defaults to os.environ.get("STORAGE_SERVICE", "https://storage.oceanum.io").
             timeout (int, optional): Timeout for requests in seconds. Defaults to 3600.
```

### Comparing `oceanum-0.9.7/tests/test_catalog.py` & `oceanum-0.9.8/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/tests/test_datamesh_connect.py` & `oceanum-0.9.8/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/tests/test_datamesh_load.py` & `oceanum-0.9.8/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/tests/test_datamesh_query.py` & `oceanum-0.9.8/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/tests/test_datamesh_write.py` & `oceanum-0.9.8/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/tests/test_datasource.py` & `oceanum-0.9.8/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/tests/test_query.py` & `oceanum-0.9.8/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.9.7/tests/test_storage.py` & `oceanum-0.9.8/tests/test_storage.py`

 * *Files identical despite different names*

