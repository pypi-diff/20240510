# Comparing `tmp/mypy-boto3-ssm-sap-1.34.0.tar.gz` & `tmp/mypy_boto3_ssm_sap-1.34.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-sap-1.34.0.tar", last modified: Wed Dec 13 21:23:57 2023, max compression
+gzip compressed data, was "mypy_boto3_ssm_sap-1.34.102.tar", last modified: Fri May 10 03:08:09 2024, max compression
```

## Comparing `mypy-boto3-ssm-sap-1.34.0.tar` & `mypy_boto3_ssm_sap-1.34.102.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:57.071393 mypy-boto3-ssm-sap-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2023-12-13 21:23:57.071393 mypy-boto3-ssm-sap-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11494 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:57.071393 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15891 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15887 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2023-12-13 21:20:22.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2023-12-13 21:20:22.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2023-12-13 21:20:22.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2023-12-13 21:20:22.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17377 2023-12-13 21:20:22.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2023-12-13 21:20:22.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:57.071393 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2023-12-13 21:23:57.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-13 21:23:57.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:57.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:57.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:57.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 21:23:57.000000 mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:57.071393 mypy-boto3-ssm-sap-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2023-12-13 21:20:21.000000 mypy-boto3-ssm-sap-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:08:09.488466 mypy_boto3_ssm_sap-1.34.102/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13202 2024-05-10 03:08:09.488466 mypy_boto3_ssm_sap-1.34.102/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:08:09.488466 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18124 2024-05-10 03:07:56.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18121 2024-05-10 03:07:56.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-10 03:07:56.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-10 03:07:56.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-10 03:07:56.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-10 03:07:56.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19866 2024-05-10 03:07:57.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19866 2024-05-10 03:07:57.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:08:09.488466 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13202 2024-05-10 03:08:09.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-10 03:08:09.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 03:08:09.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 03:08:09.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 03:08:09.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 03:08:09.000000 mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 03:08:09.488466 mypy_boto3_ssm_sap-1.34.102/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-10 03:07:55.000000 mypy_boto3_ssm_sap-1.34.102/setup.py
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/LICENSE` & `mypy_boto3_ssm_sap-1.34.102/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/PKG-INFO` & `mypy_boto3_ssm_sap-1.34.102/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.34.0
-Summary: Type annotations for boto3.SsmSap 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.102
+Summary: Type annotations for boto3.SsmSap 1.34.102 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.34.102](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,24 +283,28 @@
 from boto3.session import Session
 
 from mypy_boto3_ssm_sap import SsmSapClient
 from mypy_boto3_ssm_sap.paginator import (
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
+    ListOperationEventsPaginator,
     ListOperationsPaginator,
 )
 
 client: SsmSapClient = Session().client("ssm-sap")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
 list_databases_paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
+list_operation_events_paginator: ListOperationEventsPaginator = client.get_paginator(
+    "list_operation_events"
+)
 list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/README.md` & `mypy_boto3_ssm_sap-1.34.102/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.34.102](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -250,24 +250,28 @@
 from boto3.session import Session
 
 from mypy_boto3_ssm_sap import SsmSapClient
 from mypy_boto3_ssm_sap.paginator import (
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
+    ListOperationEventsPaginator,
     ListOperationsPaginator,
 )
 
 client: SsmSapClient = Session().client("ssm-sap")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
 list_databases_paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
+list_operation_events_paginator: ListOperationEventsPaginator = client.get_paginator(
+    "list_operation_events"
+)
 list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/__init__.py` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,40 +6,43 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_ssm_sap import (
         Client,
         ListApplicationsPaginator,
         ListComponentsPaginator,
         ListDatabasesPaginator,
+        ListOperationEventsPaginator,
         ListOperationsPaginator,
         SsmSapClient,
     )
 
     session = Session()
     client: SsmSapClient = session.client("ssm-sap")
 
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_databases_paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
+    list_operation_events_paginator: ListOperationEventsPaginator = client.get_paginator("list_operation_events")
     list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
     ```
 """
 
 from .client import SsmSapClient
 from .paginator import (
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
+    ListOperationEventsPaginator,
     ListOperationsPaginator,
 )
 
 Client = SsmSapClient
 
-
 __all__ = (
     "Client",
     "ListApplicationsPaginator",
     "ListComponentsPaginator",
     "ListDatabasesPaginator",
+    "ListOperationEventsPaginator",
     "ListOperationsPaginator",
     "SsmSapClient",
 )
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/__init__.pyi` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -6,39 +6,43 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_ssm_sap import (
         Client,
         ListApplicationsPaginator,
         ListComponentsPaginator,
         ListDatabasesPaginator,
+        ListOperationEventsPaginator,
         ListOperationsPaginator,
         SsmSapClient,
     )
 
     session = Session()
     client: SsmSapClient = session.client("ssm-sap")
 
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_databases_paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
+    list_operation_events_paginator: ListOperationEventsPaginator = client.get_paginator("list_operation_events")
     list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
     ```
 """
 
 from .client import SsmSapClient
 from .paginator import (
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
+    ListOperationEventsPaginator,
     ListOperationsPaginator,
 )
 
 Client = SsmSapClient
 
 __all__ = (
     "Client",
     "ListApplicationsPaginator",
     "ListComponentsPaginator",
     "ListDatabasesPaginator",
+    "ListOperationEventsPaginator",
     "ListOperationsPaginator",
     "SsmSapClient",
 )
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/__main__.py` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SsmSap 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.SsmSap 1.34.102\n"
+        "Version:         1.34.102\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.102")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/client.py` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationTypeType
 from .paginator import (
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
+    ListOperationEventsPaginator,
     ListOperationsPaginator,
 )
 from .type_defs import (
     ApplicationCredentialTypeDef,
     BackintConfigTypeDef,
     DeleteResourcePermissionOutputTypeDef,
     FilterTypeDef,
@@ -35,28 +36,30 @@
     GetComponentOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetOperationOutputTypeDef,
     GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
+    ListOperationEventsOutputTypeDef,
     ListOperationsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePermissionOutputTypeDef,
     RegisterApplicationOutputTypeDef,
+    StartApplicationOutputTypeDef,
     StartApplicationRefreshOutputTypeDef,
+    StopApplicationOutputTypeDef,
     UpdateApplicationSettingsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SsmSapClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -107,15 +110,15 @@
         """
 
     def delete_resource_permission(
         self,
         *,
         ResourceArn: str,
         ActionType: Literal["RESTORE"] = ...,
-        SourceResourceArn: str = ...
+        SourceResourceArn: str = ...,
     ) -> DeleteResourcePermissionOutputTypeDef:
         """
         Removes permissions associated with the target database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.delete_resource_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#delete_resource_permission)
         """
@@ -163,15 +166,15 @@
 
     def get_database(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         DatabaseId: str = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> GetDatabaseOutputTypeDef:
         """
         Gets the SAP HANA database of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_database)
@@ -218,32 +221,47 @@
 
     def list_databases(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatabasesOutputTypeDef:
         """
         Lists the SAP HANA databases of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#list_databases)
         """
 
+    def list_operation_events(
+        self,
+        *,
+        OperationId: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        Filters: Sequence[FilterTypeDef] = ...,
+    ) -> ListOperationEventsOutputTypeDef:
+        """
+        Returns a list of operations events.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_operation_events)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#list_operation_events)
+        """
+
     def list_operations(
         self,
         *,
         ApplicationId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListOperationsOutputTypeDef:
         """
         Lists the operations performed by AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#list_operations)
         """
@@ -274,33 +292,55 @@
         ApplicationId: str,
         ApplicationType: ApplicationTypeType,
         Instances: Sequence[str],
         SapInstanceNumber: str = ...,
         Sid: str = ...,
         Tags: Mapping[str, str] = ...,
         Credentials: Sequence[ApplicationCredentialTypeDef] = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> RegisterApplicationOutputTypeDef:
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#register_application)
         """
 
+    def start_application(self, *, ApplicationId: str) -> StartApplicationOutputTypeDef:
+        """
+        Request is an operation which starts an application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#start_application)
+        """
+
     def start_application_refresh(
         self, *, ApplicationId: str
     ) -> StartApplicationRefreshOutputTypeDef:
         """
         Refreshes a registered application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#start_application_refresh)
         """
 
+    def stop_application(
+        self,
+        *,
+        ApplicationId: str,
+        StopConnectedEntity: Literal["DBMS"] = ...,
+        IncludeEc2InstanceShutdown: bool = ...,
+    ) -> StopApplicationOutputTypeDef:
+        """
+        Request is an operation to stop an application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.stop_application)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#stop_application)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Creates tag for a resource by specifying the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#tag_resource)
         """
@@ -316,15 +356,15 @@
     def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
         CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
         Backint: BackintConfigTypeDef = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#update_application_settings)
@@ -350,12 +390,21 @@
     def get_paginator(self, operation_name: Literal["list_databases"]) -> ListDatabasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_operation_events"]
+    ) -> ListOperationEventsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_operations"]) -> ListOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/client.pyi` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationTypeType
 from .paginator import (
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
+    ListOperationEventsPaginator,
     ListOperationsPaginator,
 )
 from .type_defs import (
     ApplicationCredentialTypeDef,
     BackintConfigTypeDef,
     DeleteResourcePermissionOutputTypeDef,
     FilterTypeDef,
@@ -35,19 +36,22 @@
     GetComponentOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetOperationOutputTypeDef,
     GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
+    ListOperationEventsOutputTypeDef,
     ListOperationsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePermissionOutputTypeDef,
     RegisterApplicationOutputTypeDef,
+    StartApplicationOutputTypeDef,
     StartApplicationRefreshOutputTypeDef,
+    StopApplicationOutputTypeDef,
     UpdateApplicationSettingsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -103,15 +107,15 @@
         """
 
     def delete_resource_permission(
         self,
         *,
         ResourceArn: str,
         ActionType: Literal["RESTORE"] = ...,
-        SourceResourceArn: str = ...
+        SourceResourceArn: str = ...,
     ) -> DeleteResourcePermissionOutputTypeDef:
         """
         Removes permissions associated with the target database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.delete_resource_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#delete_resource_permission)
         """
@@ -159,15 +163,15 @@
 
     def get_database(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         DatabaseId: str = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> GetDatabaseOutputTypeDef:
         """
         Gets the SAP HANA database of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_database)
@@ -214,32 +218,47 @@
 
     def list_databases(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatabasesOutputTypeDef:
         """
         Lists the SAP HANA databases of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#list_databases)
         """
 
+    def list_operation_events(
+        self,
+        *,
+        OperationId: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        Filters: Sequence[FilterTypeDef] = ...,
+    ) -> ListOperationEventsOutputTypeDef:
+        """
+        Returns a list of operations events.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_operation_events)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#list_operation_events)
+        """
+
     def list_operations(
         self,
         *,
         ApplicationId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListOperationsOutputTypeDef:
         """
         Lists the operations performed by AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#list_operations)
         """
@@ -270,33 +289,55 @@
         ApplicationId: str,
         ApplicationType: ApplicationTypeType,
         Instances: Sequence[str],
         SapInstanceNumber: str = ...,
         Sid: str = ...,
         Tags: Mapping[str, str] = ...,
         Credentials: Sequence[ApplicationCredentialTypeDef] = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> RegisterApplicationOutputTypeDef:
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#register_application)
         """
 
+    def start_application(self, *, ApplicationId: str) -> StartApplicationOutputTypeDef:
+        """
+        Request is an operation which starts an application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#start_application)
+        """
+
     def start_application_refresh(
         self, *, ApplicationId: str
     ) -> StartApplicationRefreshOutputTypeDef:
         """
         Refreshes a registered application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#start_application_refresh)
         """
 
+    def stop_application(
+        self,
+        *,
+        ApplicationId: str,
+        StopConnectedEntity: Literal["DBMS"] = ...,
+        IncludeEc2InstanceShutdown: bool = ...,
+    ) -> StopApplicationOutputTypeDef:
+        """
+        Request is an operation to stop an application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.stop_application)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#stop_application)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Creates tag for a resource by specifying the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#tag_resource)
         """
@@ -312,15 +353,15 @@
     def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
         CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
         Backint: BackintConfigTypeDef = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#update_application_settings)
@@ -346,12 +387,21 @@
     def get_paginator(self, operation_name: Literal["list_databases"]) -> ListDatabasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_operation_events"]
+    ) -> ListOperationEventsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_operations"]) -> ListOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/literals.py` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,70 +15,74 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AllocationTypeType",
     "ApplicationDiscoveryStatusType",
     "ApplicationStatusType",
     "ApplicationTypeType",
     "BackintModeType",
     "ClusterStatusType",
     "ComponentStatusType",
     "ComponentTypeType",
+    "ConnectedEntityTypeType",
     "CredentialTypeType",
     "DatabaseConnectionMethodType",
     "DatabaseStatusType",
     "DatabaseTypeType",
     "FilterOperatorType",
     "HostRoleType",
     "ListApplicationsPaginatorName",
     "ListComponentsPaginatorName",
     "ListDatabasesPaginatorName",
+    "ListOperationEventsPaginatorName",
     "ListOperationsPaginatorName",
+    "OperationEventStatusType",
     "OperationModeType",
     "OperationStatusType",
     "PermissionActionTypeType",
     "ReplicationModeType",
     "SsmSapServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AllocationTypeType = Literal["ELASTIC_IP", "OVERLAY", "UNKNOWN", "VPC_SUBNET"]
 ApplicationDiscoveryStatusType = Literal[
     "DELETING", "REFRESH_FAILED", "REGISTERING", "REGISTRATION_FAILED", "SUCCESS"
 ]
 ApplicationStatusType = Literal[
     "ACTIVATED", "DELETING", "FAILED", "REGISTERING", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
 ApplicationTypeType = Literal["HANA", "SAP_ABAP"]
 BackintModeType = Literal["AWSBackup"]
 ClusterStatusType = Literal["MAINTENANCE", "NONE", "OFFLINE", "ONLINE", "STANDBY"]
 ComponentStatusType = Literal[
     "ACTIVATED", "RUNNING", "RUNNING_WITH_ERROR", "STARTING", "STOPPED", "STOPPING", "UNDEFINED"
 ]
 ComponentTypeType = Literal["ABAP", "ASCS", "DIALOG", "ERS", "HANA", "HANA_NODE", "WD", "WEBDISP"]
+ConnectedEntityTypeType = Literal["DBMS"]
 CredentialTypeType = Literal["ADMIN"]
 DatabaseConnectionMethodType = Literal["DIRECT", "OVERLAY"]
 DatabaseStatusType = Literal["ERROR", "RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
 DatabaseTypeType = Literal["SYSTEM", "TENANT"]
 FilterOperatorType = Literal["Equals", "GreaterThanOrEquals", "LessThanOrEquals"]
 HostRoleType = Literal["LEADER", "STANDBY", "UNKNOWN", "WORKER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListDatabasesPaginatorName = Literal["list_databases"]
+ListOperationEventsPaginatorName = Literal["list_operation_events"]
 ListOperationsPaginatorName = Literal["list_operations"]
+OperationEventStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS"]
 OperationModeType = Literal[
     "DELTA_DATASHIPPING", "LOGREPLAY", "LOGREPLAY_READACCESS", "NONE", "PRIMARY"
 ]
 OperationStatusType = Literal["ERROR", "INPROGRESS", "SUCCESS"]
 PermissionActionTypeType = Literal["RESTORE"]
 ReplicationModeType = Literal["ASYNC", "NONE", "PRIMARY", "SYNC", "SYNCMEM"]
 SsmSapServiceName = Literal["ssm-sap"]
@@ -104,14 +108,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -122,14 +127,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -147,14 +153,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -167,24 +174,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -245,15 +254,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -325,17 +333,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -380,14 +390,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -425,19 +436,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -466,15 +479,21 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_applications", "list_components", "list_databases", "list_operations"]
+PaginatorName = Literal[
+    "list_applications",
+    "list_components",
+    "list_databases",
+    "list_operation_events",
+    "list_operations",
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/literals.pyi` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,27 @@
     "ApplicationDiscoveryStatusType",
     "ApplicationStatusType",
     "ApplicationTypeType",
     "BackintModeType",
     "ClusterStatusType",
     "ComponentStatusType",
     "ComponentTypeType",
+    "ConnectedEntityTypeType",
     "CredentialTypeType",
     "DatabaseConnectionMethodType",
     "DatabaseStatusType",
     "DatabaseTypeType",
     "FilterOperatorType",
     "HostRoleType",
     "ListApplicationsPaginatorName",
     "ListComponentsPaginatorName",
     "ListDatabasesPaginatorName",
+    "ListOperationEventsPaginatorName",
     "ListOperationsPaginatorName",
+    "OperationEventStatusType",
     "OperationModeType",
     "OperationStatusType",
     "PermissionActionTypeType",
     "ReplicationModeType",
     "SsmSapServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -59,24 +62,27 @@
 ApplicationTypeType = Literal["HANA", "SAP_ABAP"]
 BackintModeType = Literal["AWSBackup"]
 ClusterStatusType = Literal["MAINTENANCE", "NONE", "OFFLINE", "ONLINE", "STANDBY"]
 ComponentStatusType = Literal[
     "ACTIVATED", "RUNNING", "RUNNING_WITH_ERROR", "STARTING", "STOPPED", "STOPPING", "UNDEFINED"
 ]
 ComponentTypeType = Literal["ABAP", "ASCS", "DIALOG", "ERS", "HANA", "HANA_NODE", "WD", "WEBDISP"]
+ConnectedEntityTypeType = Literal["DBMS"]
 CredentialTypeType = Literal["ADMIN"]
 DatabaseConnectionMethodType = Literal["DIRECT", "OVERLAY"]
 DatabaseStatusType = Literal["ERROR", "RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
 DatabaseTypeType = Literal["SYSTEM", "TENANT"]
 FilterOperatorType = Literal["Equals", "GreaterThanOrEquals", "LessThanOrEquals"]
 HostRoleType = Literal["LEADER", "STANDBY", "UNKNOWN", "WORKER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListDatabasesPaginatorName = Literal["list_databases"]
+ListOperationEventsPaginatorName = Literal["list_operation_events"]
 ListOperationsPaginatorName = Literal["list_operations"]
+OperationEventStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS"]
 OperationModeType = Literal[
     "DELTA_DATASHIPPING", "LOGREPLAY", "LOGREPLAY_READACCESS", "NONE", "PRIMARY"
 ]
 OperationStatusType = Literal["ERROR", "INPROGRESS", "SUCCESS"]
 PermissionActionTypeType = Literal["RESTORE"]
 ReplicationModeType = Literal["ASYNC", "NONE", "PRIMARY", "SYNC", "SYNCMEM"]
 SsmSapServiceName = Literal["ssm-sap"]
@@ -102,14 +108,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -120,14 +127,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -145,14 +153,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -165,24 +174,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -243,15 +254,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -323,17 +333,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -378,14 +390,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -423,19 +436,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -464,15 +479,21 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_applications", "list_components", "list_databases", "list_operations"]
+PaginatorName = Literal[
+    "list_applications",
+    "list_components",
+    "list_databases",
+    "list_operation_events",
+    "list_operations",
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/paginator.py` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,48 +9,51 @@
     from boto3.session import Session
 
     from mypy_boto3_ssm_sap.client import SsmSapClient
     from mypy_boto3_ssm_sap.paginator import (
         ListApplicationsPaginator,
         ListComponentsPaginator,
         ListDatabasesPaginator,
+        ListOperationEventsPaginator,
         ListOperationsPaginator,
     )
 
     session = Session()
     client: SsmSapClient = session.client("ssm-sap")
 
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_databases_paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
+    list_operation_events_paginator: ListOperationEventsPaginator = client.get_paginator("list_operation_events")
     list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
     ```
 """
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     FilterTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
+    ListOperationEventsOutputTypeDef,
     ListOperationsOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListApplicationsPaginator",
     "ListComponentsPaginator",
     "ListDatabasesPaginator",
+    "ListOperationEventsPaginator",
     "ListOperationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -63,15 +66,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 
@@ -97,32 +100,51 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listdatabasespaginator)
         """
 
 
+class ListOperationEventsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperationEvents)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationeventspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        OperationId: str,
+        Filters: Sequence[FilterTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListOperationEventsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperationEvents.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationeventspaginator)
+        """
+
+
 class ListOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/paginator.pyi` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,44 +9,48 @@
     from boto3.session import Session
 
     from mypy_boto3_ssm_sap.client import SsmSapClient
     from mypy_boto3_ssm_sap.paginator import (
         ListApplicationsPaginator,
         ListComponentsPaginator,
         ListDatabasesPaginator,
+        ListOperationEventsPaginator,
         ListOperationsPaginator,
     )
 
     session = Session()
     client: SsmSapClient = session.client("ssm-sap")
 
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_databases_paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
+    list_operation_events_paginator: ListOperationEventsPaginator = client.get_paginator("list_operation_events")
     list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
     ```
 """
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     FilterTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
+    ListOperationEventsOutputTypeDef,
     ListOperationsOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListApplicationsPaginator",
     "ListComponentsPaginator",
     "ListDatabasesPaginator",
+    "ListOperationEventsPaginator",
     "ListOperationsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -60,15 +64,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 class ListComponentsPaginator(Paginator):
@@ -92,31 +96,49 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listdatabasespaginator)
         """
 
+class ListOperationEventsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperationEvents)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationeventspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        OperationId: str,
+        Filters: Sequence[FilterTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListOperationEventsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperationEvents.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationeventspaginator)
+        """
+
 class ListOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/type_defs.py` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ComponentStatusType,
     ComponentTypeType,
     DatabaseConnectionMethodType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
+    OperationEventStatusType,
     OperationModeType,
     OperationStatusType,
     ReplicationModeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -43,15 +44,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "IpAddressMemberTypeDef",
     "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
@@ -69,16 +69,19 @@
     "GetOperationInputRequestTypeDef",
     "OperationTypeDef",
     "GetResourcePermissionInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResourceTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
+    "StartApplicationInputRequestTypeDef",
     "StartApplicationRefreshInputRequestTypeDef",
+    "StopApplicationInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "AssociatedHostTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
     "DeleteResourcePermissionOutputTypeDef",
@@ -86,26 +89,32 @@
     "GetResourcePermissionOutputTypeDef",
     "ListApplicationsOutputTypeDef",
     "ListComponentsOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePermissionOutputTypeDef",
     "RegisterApplicationOutputTypeDef",
+    "StartApplicationOutputTypeDef",
     "StartApplicationRefreshOutputTypeDef",
+    "StopApplicationOutputTypeDef",
     "UpdateApplicationSettingsOutputTypeDef",
     "ListApplicationsInputRequestTypeDef",
+    "ListOperationEventsInputRequestTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListOperationEventsInputListOperationEventsPaginateTypeDef",
     "ListOperationsInputListOperationsPaginateTypeDef",
+    "OperationEventTypeDef",
     "GetDatabaseOutputTypeDef",
     "ComponentTypeDef",
+    "ListOperationEventsOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
         "DatabaseName": str,
@@ -210,18 +219,18 @@
         "SourceResourceArn": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeregisterApplicationInputRequestTypeDef = TypedDict(
     "DeregisterApplicationInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
@@ -314,28 +323,49 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
+    {
+        "ResourceArn": NotRequired[str],
+        "ResourceType": NotRequired[str],
+    },
+)
 PutResourcePermissionInputRequestTypeDef = TypedDict(
     "PutResourcePermissionInputRequestTypeDef",
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
+StartApplicationInputRequestTypeDef = TypedDict(
+    "StartApplicationInputRequestTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
 StartApplicationRefreshInputRequestTypeDef = TypedDict(
     "StartApplicationRefreshInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
+StopApplicationInputRequestTypeDef = TypedDict(
+    "StopApplicationInputRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "StopConnectedEntity": NotRequired[Literal["DBMS"]],
+        "IncludeEc2InstanceShutdown": NotRequired[bool],
+    },
+)
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -416,32 +446,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApplicationsOutputTypeDef = TypedDict(
     "ListApplicationsOutputTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListComponentsOutputTypeDef = TypedDict(
     "ListComponentsOutputTypeDef",
     {
         "Components": List[ComponentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "Databases": List[DatabaseSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -458,21 +488,35 @@
     "RegisterApplicationOutputTypeDef",
     {
         "Application": ApplicationTypeDef,
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartApplicationOutputTypeDef = TypedDict(
+    "StartApplicationOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StartApplicationRefreshOutputTypeDef = TypedDict(
     "StartApplicationRefreshOutputTypeDef",
     {
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StopApplicationOutputTypeDef = TypedDict(
+    "StopApplicationOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateApplicationSettingsOutputTypeDef = TypedDict(
     "UpdateApplicationSettingsOutputTypeDef",
     {
         "Message": str,
         "OperationIds": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -481,14 +525,23 @@
     "ListApplicationsInputRequestTypeDef",
     {
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
         "Filters": NotRequired[Sequence[FilterTypeDef]],
     },
 )
+ListOperationEventsInputRequestTypeDef = TypedDict(
+    "ListOperationEventsInputRequestTypeDef",
+    {
+        "OperationId": str,
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "Filters": NotRequired[Sequence[FilterTypeDef]],
+    },
+)
 ListOperationsInputRequestTypeDef = TypedDict(
     "ListOperationsInputRequestTypeDef",
     {
         "ApplicationId": str,
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
         "Filters": NotRequired[Sequence[FilterTypeDef]],
@@ -501,16 +554,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListOperationsOutputTypeDef = TypedDict(
     "ListOperationsOutputTypeDef",
     {
         "Operations": List[OperationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     {
         "Filters": NotRequired[Sequence[FilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -527,22 +580,40 @@
     "ListDatabasesInputListDatabasesPaginateTypeDef",
     {
         "ApplicationId": NotRequired[str],
         "ComponentId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListOperationEventsInputListOperationEventsPaginateTypeDef = TypedDict(
+    "ListOperationEventsInputListOperationEventsPaginateTypeDef",
+    {
+        "OperationId": str,
+        "Filters": NotRequired[Sequence[FilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListOperationsInputListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsInputListOperationsPaginateTypeDef",
     {
         "ApplicationId": str,
         "Filters": NotRequired[Sequence[FilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+OperationEventTypeDef = TypedDict(
+    "OperationEventTypeDef",
+    {
+        "Description": NotRequired[str],
+        "Resource": NotRequired[ResourceTypeDef],
+        "Status": NotRequired[OperationEventStatusType],
+        "StatusMessage": NotRequired[str],
+        "Timestamp": NotRequired[datetime],
+    },
+)
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -568,14 +639,22 @@
         "Hosts": NotRequired[List[HostTypeDef]],
         "PrimaryHost": NotRequired[str],
         "DatabaseConnection": NotRequired[DatabaseConnectionTypeDef],
         "LastUpdated": NotRequired[datetime],
         "Arn": NotRequired[str],
     },
 )
+ListOperationEventsOutputTypeDef = TypedDict(
+    "ListOperationEventsOutputTypeDef",
+    {
+        "OperationEvents": List[OperationEventTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap/type_defs.pyi` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ComponentStatusType,
     ComponentTypeType,
     DatabaseConnectionMethodType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
+    OperationEventStatusType,
     OperationModeType,
     OperationStatusType,
     ReplicationModeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -68,16 +69,19 @@
     "GetOperationInputRequestTypeDef",
     "OperationTypeDef",
     "GetResourcePermissionInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResourceTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
+    "StartApplicationInputRequestTypeDef",
     "StartApplicationRefreshInputRequestTypeDef",
+    "StopApplicationInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "AssociatedHostTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
     "DeleteResourcePermissionOutputTypeDef",
@@ -85,26 +89,32 @@
     "GetResourcePermissionOutputTypeDef",
     "ListApplicationsOutputTypeDef",
     "ListComponentsOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePermissionOutputTypeDef",
     "RegisterApplicationOutputTypeDef",
+    "StartApplicationOutputTypeDef",
     "StartApplicationRefreshOutputTypeDef",
+    "StopApplicationOutputTypeDef",
     "UpdateApplicationSettingsOutputTypeDef",
     "ListApplicationsInputRequestTypeDef",
+    "ListOperationEventsInputRequestTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListOperationEventsInputListOperationEventsPaginateTypeDef",
     "ListOperationsInputListOperationsPaginateTypeDef",
+    "OperationEventTypeDef",
     "GetDatabaseOutputTypeDef",
     "ComponentTypeDef",
+    "ListOperationEventsOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
         "DatabaseName": str,
@@ -209,18 +219,18 @@
         "SourceResourceArn": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeregisterApplicationInputRequestTypeDef = TypedDict(
     "DeregisterApplicationInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
@@ -313,28 +323,49 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
+    {
+        "ResourceArn": NotRequired[str],
+        "ResourceType": NotRequired[str],
+    },
+)
 PutResourcePermissionInputRequestTypeDef = TypedDict(
     "PutResourcePermissionInputRequestTypeDef",
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
+StartApplicationInputRequestTypeDef = TypedDict(
+    "StartApplicationInputRequestTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
 StartApplicationRefreshInputRequestTypeDef = TypedDict(
     "StartApplicationRefreshInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
+StopApplicationInputRequestTypeDef = TypedDict(
+    "StopApplicationInputRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "StopConnectedEntity": NotRequired[Literal["DBMS"]],
+        "IncludeEc2InstanceShutdown": NotRequired[bool],
+    },
+)
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -415,32 +446,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApplicationsOutputTypeDef = TypedDict(
     "ListApplicationsOutputTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListComponentsOutputTypeDef = TypedDict(
     "ListComponentsOutputTypeDef",
     {
         "Components": List[ComponentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "Databases": List[DatabaseSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -457,21 +488,35 @@
     "RegisterApplicationOutputTypeDef",
     {
         "Application": ApplicationTypeDef,
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartApplicationOutputTypeDef = TypedDict(
+    "StartApplicationOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StartApplicationRefreshOutputTypeDef = TypedDict(
     "StartApplicationRefreshOutputTypeDef",
     {
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StopApplicationOutputTypeDef = TypedDict(
+    "StopApplicationOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateApplicationSettingsOutputTypeDef = TypedDict(
     "UpdateApplicationSettingsOutputTypeDef",
     {
         "Message": str,
         "OperationIds": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -480,14 +525,23 @@
     "ListApplicationsInputRequestTypeDef",
     {
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
         "Filters": NotRequired[Sequence[FilterTypeDef]],
     },
 )
+ListOperationEventsInputRequestTypeDef = TypedDict(
+    "ListOperationEventsInputRequestTypeDef",
+    {
+        "OperationId": str,
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "Filters": NotRequired[Sequence[FilterTypeDef]],
+    },
+)
 ListOperationsInputRequestTypeDef = TypedDict(
     "ListOperationsInputRequestTypeDef",
     {
         "ApplicationId": str,
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
         "Filters": NotRequired[Sequence[FilterTypeDef]],
@@ -500,16 +554,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListOperationsOutputTypeDef = TypedDict(
     "ListOperationsOutputTypeDef",
     {
         "Operations": List[OperationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     {
         "Filters": NotRequired[Sequence[FilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -526,22 +580,40 @@
     "ListDatabasesInputListDatabasesPaginateTypeDef",
     {
         "ApplicationId": NotRequired[str],
         "ComponentId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListOperationEventsInputListOperationEventsPaginateTypeDef = TypedDict(
+    "ListOperationEventsInputListOperationEventsPaginateTypeDef",
+    {
+        "OperationId": str,
+        "Filters": NotRequired[Sequence[FilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListOperationsInputListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsInputListOperationsPaginateTypeDef",
     {
         "ApplicationId": str,
         "Filters": NotRequired[Sequence[FilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+OperationEventTypeDef = TypedDict(
+    "OperationEventTypeDef",
+    {
+        "Description": NotRequired[str],
+        "Resource": NotRequired[ResourceTypeDef],
+        "Status": NotRequired[OperationEventStatusType],
+        "StatusMessage": NotRequired[str],
+        "Timestamp": NotRequired[datetime],
+    },
+)
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -567,14 +639,22 @@
         "Hosts": NotRequired[List[HostTypeDef]],
         "PrimaryHost": NotRequired[str],
         "DatabaseConnection": NotRequired[DatabaseConnectionTypeDef],
         "LastUpdated": NotRequired[datetime],
         "Arn": NotRequired[str],
     },
 )
+ListOperationEventsOutputTypeDef = TypedDict(
+    "ListOperationEventsOutputTypeDef",
+    {
+        "OperationEvents": List[OperationEventTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/PKG-INFO` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.34.0
-Summary: Type annotations for boto3.SsmSap 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.102
+Summary: Type annotations for boto3.SsmSap 1.34.102 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.34.102](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,24 +283,28 @@
 from boto3.session import Session
 
 from mypy_boto3_ssm_sap import SsmSapClient
 from mypy_boto3_ssm_sap.paginator import (
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
+    ListOperationEventsPaginator,
     ListOperationsPaginator,
 )
 
 client: SsmSapClient = Session().client("ssm-sap")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
 list_databases_paginator: ListDatabasesPaginator = client.get_paginator("list_databases")
+list_operation_events_paginator: ListOperationEventsPaginator = client.get_paginator(
+    "list_operation_events"
+)
 list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `mypy-boto3-ssm-sap-1.34.0/mypy_boto3_ssm_sap.egg-info/SOURCES.txt` & `mypy_boto3_ssm_sap-1.34.102/mypy_boto3_ssm_sap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.34.0/setup.py` & `mypy_boto3_ssm_sap-1.34.102/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-sap",
-    version="1.34.0",
+    version="1.34.102",
     packages=["mypy_boto3_ssm_sap"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.SsmSap 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.SsmSap 1.34.102 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 ssm-sap type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ssm_sap": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

