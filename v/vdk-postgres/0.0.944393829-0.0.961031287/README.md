# Comparing `tmp/vdk-postgres-0.0.944393829.tar.gz` & `tmp/vdk-postgres-0.0.961031287.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-postgres-0.0.944393829.tar", last modified: Tue Jul 25 09:00:58 2023, max compression
+gzip compressed data, was "vdk-postgres-0.0.961031287.tar", last modified: Wed Aug  9 16:25:59 2023, max compression
```

## Comparing `vdk-postgres-0.0.944393829.tar` & `vdk-postgres-0.0.961031287.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:58.910925 vdk-postgres-0.0.944393829/
--rw-r--r--   0 root         (0) root         (0)     1564 2023-07-25 09:00:58.906925 vdk-postgres-0.0.944393829/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      926 2023-07-25 09:00:43.000000 vdk-postgres-0.0.944393829/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:00:58.910925 vdk-postgres-0.0.944393829/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-07-25 09:00:47.000000 vdk-postgres-0.0.944393829/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:58.902925 vdk-postgres-0.0.944393829/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:58.902925 vdk-postgres-0.0.944393829/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:58.902925 vdk-postgres-0.0.944393829/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:58.906925 vdk-postgres-0.0.944393829/src/vdk/plugin/postgres/
--rw-rw-rw-   0 root         (0) root         (0)     3354 2023-07-25 09:00:43.000000 vdk-postgres-0.0.944393829/src/vdk/plugin/postgres/ingest_to_postgres.py
--rw-rw-rw-   0 root         (0) root         (0)     3862 2023-07-25 09:00:43.000000 vdk-postgres-0.0.944393829/src/vdk/plugin/postgres/postgres_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-07-25 09:00:43.000000 vdk-postgres-0.0.944393829/src/vdk/plugin/postgres/postgres_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:58.906925 vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1564 2023-07-25 09:00:58.000000 vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-25 09:00:58.000000 vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:00:58.000000 vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-25 09:00:58.000000 vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-25 09:00:58.000000 vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:00:58.000000 vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:58.906925 vdk-postgres-0.0.944393829/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3108 2023-07-25 09:00:43.000000 vdk-postgres-0.0.944393829/tests/test_ingest.py
--rw-rw-rw-   0 root         (0) root         (0)     1568 2023-07-25 09:00:43.000000 vdk-postgres-0.0.944393829/tests/test_vdk_postgres_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:25:59.855979 vdk-postgres-0.0.961031287/
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-08-09 16:25:59.855979 vdk-postgres-0.0.961031287/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      926 2023-08-09 16:25:42.000000 vdk-postgres-0.0.961031287/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-09 16:25:59.855979 vdk-postgres-0.0.961031287/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-08-09 16:25:47.000000 vdk-postgres-0.0.961031287/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:25:59.851979 vdk-postgres-0.0.961031287/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:25:59.851979 vdk-postgres-0.0.961031287/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:25:59.851979 vdk-postgres-0.0.961031287/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:25:59.851979 vdk-postgres-0.0.961031287/src/vdk/plugin/postgres/
+-rw-rw-rw-   0 root         (0) root         (0)     3354 2023-08-09 16:25:42.000000 vdk-postgres-0.0.961031287/src/vdk/plugin/postgres/ingest_to_postgres.py
+-rw-rw-rw-   0 root         (0) root         (0)     3862 2023-08-09 16:25:42.000000 vdk-postgres-0.0.961031287/src/vdk/plugin/postgres/postgres_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-08-09 16:25:42.000000 vdk-postgres-0.0.961031287/src/vdk/plugin/postgres/postgres_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:25:59.855979 vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-08-09 16:25:59.000000 vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      450 2023-08-09 16:25:59.000000 vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 16:25:59.000000 vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-08-09 16:25:59.000000 vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-08-09 16:25:59.000000 vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-09 16:25:59.000000 vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:25:59.855979 vdk-postgres-0.0.961031287/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2023-08-09 16:25:42.000000 vdk-postgres-0.0.961031287/tests/test_ingest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2023-08-09 16:25:42.000000 vdk-postgres-0.0.961031287/tests/test_vdk_postgres_utils.py
```

### Comparing `vdk-postgres-0.0.944393829/PKG-INFO` & `vdk-postgres-0.0.961031287/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-postgres
-Version: 0.0.944393829
+Version: 0.0.961031287
 Summary: Versatile Data Kit SDK plugin provides support for PostgreSQL database and postgres transformation templates.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-postgres-0.0.944393829/README.md` & `vdk-postgres-0.0.961031287/README.md`

 * *Files identical despite different names*

### Comparing `vdk-postgres-0.0.944393829/setup.py` & `vdk-postgres-0.0.961031287/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.0.944393829"
+__version__ = "0.0.961031287"
 
 setuptools.setup(
     name="vdk-postgres",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for PostgreSQL database and postgres transformation templates.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-postgres-0.0.944393829/src/vdk/plugin/postgres/ingest_to_postgres.py` & `vdk-postgres-0.0.961031287/src/vdk/plugin/postgres/ingest_to_postgres.py`

 * *Files identical despite different names*

### Comparing `vdk-postgres-0.0.944393829/src/vdk/plugin/postgres/postgres_connection.py` & `vdk-postgres-0.0.961031287/src/vdk/plugin/postgres/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-postgres-0.0.944393829/src/vdk/plugin/postgres/postgres_plugin.py` & `vdk-postgres-0.0.961031287/src/vdk/plugin/postgres/postgres_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-postgres-0.0.944393829/src/vdk_postgres.egg-info/PKG-INFO` & `vdk-postgres-0.0.961031287/src/vdk_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-postgres
-Version: 0.0.944393829
+Version: 0.0.961031287
 Summary: Versatile Data Kit SDK plugin provides support for PostgreSQL database and postgres transformation templates.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-postgres-0.0.944393829/tests/test_ingest.py` & `vdk-postgres-0.0.961031287/tests/test_ingest.py`

 * *Files identical despite different names*

### Comparing `vdk-postgres-0.0.944393829/tests/test_vdk_postgres_utils.py` & `vdk-postgres-0.0.961031287/tests/test_vdk_postgres_utils.py`

 * *Files identical despite different names*

