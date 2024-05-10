# Comparing `tmp/vdk_oracle-0.1.1284357447.tar.gz` & `tmp/vdk-oracle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk_oracle-0.1.1284357447.tar", last modified: Thu May  9 09:30:59 2024, max compression
+gzip compressed data, was "vdk-oracle-0.1.2.tar", last modified: Tue Jan 16 23:54:31 2024, max compression
```

## Comparing `vdk_oracle-0.1.1284357447.tar` & `vdk-oracle-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 09:30:58.990404 vdk_oracle-0.1.1284357447/
--rw-r--r--   0 root         (0) root         (0)    13809 2024-05-09 09:30:58.990404 vdk_oracle-0.1.1284357447/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12800 2024-05-09 09:30:38.000000 vdk_oracle-0.1.1284357447/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 09:30:58.994404 vdk_oracle-0.1.1284357447/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-05-09 09:30:45.000000 vdk_oracle-0.1.1284357447/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 09:30:58.974404 vdk_oracle-0.1.1284357447/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 09:30:58.970404 vdk_oracle-0.1.1284357447/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 09:30:58.970404 vdk_oracle-0.1.1284357447/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 09:30:58.978404 vdk_oracle-0.1.1284357447/src/vdk/plugin/oracle/
--rw-rw-rw-   0 root         (0) root         (0)    10778 2024-05-09 09:30:38.000000 vdk_oracle-0.1.1284357447/src/vdk/plugin/oracle/ingest_to_oracle.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2024-05-09 09:30:38.000000 vdk_oracle-0.1.1284357447/src/vdk/plugin/oracle/oracle_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2024-05-09 09:30:38.000000 vdk_oracle-0.1.1284357447/src/vdk/plugin/oracle/oracle_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     6114 2024-05-09 09:30:38.000000 vdk_oracle-0.1.1284357447/src/vdk/plugin/oracle/oracle_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 09:30:58.990404 vdk_oracle-0.1.1284357447/src/vdk_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13809 2024-05-09 09:30:58.000000 vdk_oracle-0.1.1284357447/src/vdk_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-05-09 09:30:58.000000 vdk_oracle-0.1.1284357447/src/vdk_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 09:30:58.000000 vdk_oracle-0.1.1284357447/src/vdk_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-09 09:30:58.000000 vdk_oracle-0.1.1284357447/src/vdk_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-09 09:30:58.000000 vdk_oracle-0.1.1284357447/src/vdk_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-09 09:30:58.000000 vdk_oracle-0.1.1284357447/src/vdk_oracle.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 09:30:58.990404 vdk_oracle-0.1.1284357447/tests/
--rw-rw-rw-   0 root         (0) root         (0)    17836 2024-05-09 09:30:38.000000 vdk_oracle-0.1.1284357447/tests/test_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-09 09:30:38.000000 vdk_oracle-0.1.1284357447/tests/test_secrets_config.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.982146 vdk-oracle-0.1.2/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7363 2024-01-16 23:54:31.979875 vdk-oracle-0.1.2/PKG-INFO
+-rw-r--r--   0 aivanov    (502) staff       (20)     6414 2024-01-16 16:15:12.000000 vdk-oracle-0.1.2/README.md
+-rw-r--r--   0 aivanov    (502) staff       (20)       38 2024-01-16 23:54:31.982451 vdk-oracle-0.1.2/setup.cfg
+-rw-r--r--   0 aivanov    (502) staff       (20)     1646 2024-01-16 23:54:23.000000 vdk-oracle-0.1.2/setup.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.957032 vdk-oracle-0.1.2/src/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.955869 vdk-oracle-0.1.2/src/vdk/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.956330 vdk-oracle-0.1.2/src/vdk/plugin/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.965605 vdk-oracle-0.1.2/src/vdk/plugin/oracle/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7702 2024-01-09 13:57:58.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/ingest_to_oracle.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     4340 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_configuration.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     3168 2024-01-16 17:02:10.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_connection.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     4029 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_plugin.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.976413 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7363 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 aivanov    (502) staff       (20)      468 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)        1 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)       62 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)       27 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/requires.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)        4 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.974616 vdk-oracle-0.1.2/tests/
+-rw-r--r--   0 aivanov    (502) staff       (20)     8319 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/tests/test_plugin.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     5232 2024-01-09 13:57:58.000000 vdk-oracle-0.1.2/tests/test_secrets_config.py
```

### Comparing `vdk_oracle-0.1.1284357447/setup.py` & `vdk-oracle-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.1284357447"
+__version__ = "0.1.2"
 
 setuptools.setup(
     name="vdk-oracle",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Support for VDK Managed Oracle connection",
     long_description=pathlib.Path("README.md").read_text(),
@@ -27,15 +27,14 @@
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
     ],
     project_urls={
         "Documentation": "https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle",
         "Source Code": "https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle",
         "Bug Tracker": "https://github.com/vmware/versatile-data-kit/issues/new/choose",
     },
 )
```

### Comparing `vdk_oracle-0.1.1284357447/src/vdk/plugin/oracle/oracle_connection.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 from typing import List
 from typing import Optional
 
 from oracledb import Connection
@@ -18,26 +18,24 @@
     def __init__(
         self,
         user: str,
         password: str,
         connection_string: str = None,
         host=None,
         port=1521,
-        sid: str = None,
-        service_name: str = None,
+        sid=None,
         thick_mode: bool = True,
         thick_mode_lib_dir: Optional[str] = None,
     ):
         super().__init__(log)
         self._oracle_user = user
         self._oracle_password = password
         self._host = host
         self._port = port
         self._sid = sid
-        self._service_name = service_name
         self._oracle_connection_string = connection_string
         self._thick_mode = thick_mode
         self._thick_mode_lib_dir = thick_mode_lib_dir
 
     def _connect(self) -> Connection:
         import oracledb
 
@@ -58,15 +56,14 @@
             log.debug("Connecting to Oracle using host,port,sid")
             params = oracledb.ConnectParams(
                 user=self._oracle_user,
                 password=self._oracle_password,
                 host=self._host,
                 port=self._port,
                 sid=self._sid,
-                service_name=self._service_name,
             )
             conn = oracledb.connect(params=params)
         return conn
 
     def _is_connected(self) -> bool:
         if None is self._is_db_con_open:
             return False
```

### Comparing `vdk_oracle-0.1.1284357447/tests/test_secrets_config.py` & `vdk-oracle-0.1.2/tests/test_secrets_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import os
 from unittest import mock
 
 import pytest
 from click.testing import Result
```

