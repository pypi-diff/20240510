# Comparing `tmp/mypy-boto3-discovery-1.34.0.tar.gz` & `tmp/mypy_boto3_discovery-1.34.103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-discovery-1.34.0.tar", last modified: Wed Dec 13 21:22:27 2023, max compression
+gzip compressed data, was "mypy_boto3_discovery-1.34.103.tar", last modified: Fri May 10 19:47:11 2024, max compression
```

## Comparing `mypy-boto3-discovery-1.34.0.tar` & `mypy_boto3_discovery-1.34.103.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:27.751189 mypy-boto3-discovery-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2023-12-13 21:22:27.751189 mypy-boto3-discovery-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:27.751189 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25584 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25580 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-12-13 21:08:31.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26838 2023-12-13 21:08:31.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2023-12-13 21:08:31.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:27.751189 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2023-12-13 21:22:27.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-13 21:22:27.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:27.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:27.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:27.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 21:22:27.000000 mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:27.751189 mypy-boto3-discovery-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-12-13 21:08:30.000000 mypy-boto3-discovery-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:11.724248 mypy_boto3_discovery-1.34.103/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-10 19:47:11.724248 mypy_boto3_discovery-1.34.103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:11.724248 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25590 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25587 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26850 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26850 2024-05-10 19:46:37.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:11.724248 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-10 19:47:11.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-10 19:47:11.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:47:11.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:47:11.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 19:47:11.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 19:47:11.000000 mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:47:11.724248 mypy_boto3_discovery-1.34.103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-10 19:46:36.000000 mypy_boto3_discovery-1.34.103/setup.py
```

### Comparing `mypy-boto3-discovery-1.34.0/LICENSE` & `mypy_boto3_discovery-1.34.103/LICENSE`

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

### Comparing `mypy-boto3-discovery-1.34.0/PKG-INFO` & `mypy_boto3_discovery-1.34.103/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.34.0
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.103
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.34.103 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
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
 
 <a id="mypy-boto3-discovery"></a>
 
 # mypy-boto3-discovery
 
 [![PyPI - mypy-boto3-discovery](https://img.shields.io/pypi/v/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-discovery-1.34.0/README.md` & `mypy_boto3_discovery-1.34.103/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/__init__.py` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     DescribeImportTasksPaginator,
     DescribeTagsPaginator,
     ListConfigurationsPaginator,
 )
 
 Client = ApplicationDiscoveryServiceClient
 
-
 __all__ = (
     "ApplicationDiscoveryServiceClient",
     "Client",
     "DescribeAgentsPaginator",
     "DescribeContinuousExportsPaginator",
     "DescribeExportConfigurationsPaginator",
     "DescribeExportTasksPaginator",
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/__init__.pyi` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/__main__.py` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationDiscoveryService 1.34.0\nVersion:        "
-        " 1.34.0\nBuilder version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ApplicationDiscoveryService 1.34.103\n"
+        "Version:         1.34.103\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.103")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/client.py` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,40 +64,36 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApplicationDiscoveryServiceClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AuthorizationErrorException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictErrorException: Type[BotocoreClientError]
     HomeRegionNotSetException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     InvalidParameterValueException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     OperationNotPermittedException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServerInternalErrorException: Type[BotocoreClientError]
 
-
 class ApplicationDiscoveryServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/)
     """
 
     meta: ClientMeta
@@ -197,15 +193,15 @@
 
     def describe_agents(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeAgentsResponseTypeDef:
         """
         Lists agents or collectors as specified by ID or other filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/#describe_agents)
         """
@@ -254,29 +250,29 @@
 
     def describe_export_tasks(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Retrieve status of one or more export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_export_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/#describe_export_tasks)
         """
 
     def describe_import_tasks(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeImportTasksResponseTypeDef:
         """
         Returns an array of import tasks for your account, including status
         information, times, IDs, the Amazon S3 Object URL for the import file, and
         more.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_import_tasks)
@@ -284,15 +280,15 @@
         """
 
     def describe_tags(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeTagsResponseTypeDef:
         """
         Retrieves a list of configuration items that have tags as specified by the
         key-value pairs, name and value, passed to the optional parameter
         `filters`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_tags)
@@ -342,15 +338,15 @@
     def list_configurations(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: Sequence[OrderByElementTypeDef] = ...
+        orderBy: Sequence[OrderByElementTypeDef] = ...,
     ) -> ListConfigurationsResponseTypeDef:
         """
         Retrieves a list of configuration items as specified by the value passed to the
         required parameter
         `configurationType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_configurations)
@@ -360,15 +356,15 @@
     def list_server_neighbors(
         self,
         *,
         configurationId: str,
         portInformationNeeded: bool = ...,
         neighborConfigurationIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServerNeighborsResponseTypeDef:
         """
         Retrieves a list of servers that are one network hop away from a specified
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_server_neighbors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/#list_server_neighbors)
@@ -407,15 +403,15 @@
     def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        preferences: ExportPreferencesTypeDef = ...
+        preferences: ExportPreferencesTypeDef = ...,
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/client.pyi` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,34 +66,37 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("ApplicationDiscoveryServiceClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AuthorizationErrorException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictErrorException: Type[BotocoreClientError]
     HomeRegionNotSetException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     InvalidParameterValueException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     OperationNotPermittedException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServerInternalErrorException: Type[BotocoreClientError]
 
+
 class ApplicationDiscoveryServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/)
     """
 
     meta: ClientMeta
@@ -193,15 +196,15 @@
 
     def describe_agents(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeAgentsResponseTypeDef:
         """
         Lists agents or collectors as specified by ID or other filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/#describe_agents)
         """
@@ -250,29 +253,29 @@
 
     def describe_export_tasks(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Retrieve status of one or more export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_export_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/#describe_export_tasks)
         """
 
     def describe_import_tasks(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeImportTasksResponseTypeDef:
         """
         Returns an array of import tasks for your account, including status
         information, times, IDs, the Amazon S3 Object URL for the import file, and
         more.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_import_tasks)
@@ -280,15 +283,15 @@
         """
 
     def describe_tags(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeTagsResponseTypeDef:
         """
         Retrieves a list of configuration items that have tags as specified by the
         key-value pairs, name and value, passed to the optional parameter
         `filters`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_tags)
@@ -338,15 +341,15 @@
     def list_configurations(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: Sequence[OrderByElementTypeDef] = ...
+        orderBy: Sequence[OrderByElementTypeDef] = ...,
     ) -> ListConfigurationsResponseTypeDef:
         """
         Retrieves a list of configuration items as specified by the value passed to the
         required parameter
         `configurationType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_configurations)
@@ -356,15 +359,15 @@
     def list_server_neighbors(
         self,
         *,
         configurationId: str,
         portInformationNeeded: bool = ...,
         neighborConfigurationIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServerNeighborsResponseTypeDef:
         """
         Retrieves a list of servers that are one network hop away from a specified
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_server_neighbors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/#list_server_neighbors)
@@ -403,15 +406,15 @@
     def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        preferences: ExportPreferencesTypeDef = ...
+        preferences: ExportPreferencesTypeDef = ...,
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/literals.py` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AgentStatusType",
     "BatchDeleteConfigurationTaskStatusType",
     "BatchDeleteImportDataErrorCodeType",
     "ConfigurationItemTypeType",
     "ContinuousExportStatusType",
     "DataSourceType",
@@ -37,26 +36,25 @@
     "DescribeTagsPaginatorName",
     "ExportDataFormatType",
     "ExportStatusType",
     "ImportStatusType",
     "ImportTaskFilterNameType",
     "ListConfigurationsPaginatorName",
     "OfferingClassType",
+    "OrderStringType",
     "PurchasingOptionType",
     "TenancyType",
     "TermLengthType",
-    "orderStringType",
     "ApplicationDiscoveryServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AgentStatusType = Literal["BLACKLISTED", "HEALTHY", "RUNNING", "SHUTDOWN", "UNHEALTHY", "UNKNOWN"]
 BatchDeleteConfigurationTaskStatusType = Literal[
     "COMPLETED", "DELETING", "FAILED", "INITIALIZING", "VALIDATING"
 ]
 BatchDeleteImportDataErrorCodeType = Literal["INTERNAL_SERVER_ERROR", "NOT_FOUND", "OVER_LIMIT"]
 ConfigurationItemTypeType = Literal["APPLICATION", "CONNECTION", "PROCESS", "SERVER"]
 ContinuousExportStatusType = Literal[
@@ -91,18 +89,18 @@
     "IMPORT_FAILED_SERVER_LIMIT_EXCEEDED",
     "IMPORT_IN_PROGRESS",
     "INTERNAL_ERROR",
 ]
 ImportTaskFilterNameType = Literal["IMPORT_TASK_ID", "NAME", "STATUS"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 OfferingClassType = Literal["CONVERTIBLE", "STANDARD"]
+OrderStringType = Literal["ASC", "DESC"]
 PurchasingOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 TenancyType = Literal["DEDICATED", "SHARED"]
 TermLengthType = Literal["ONE_YEAR", "THREE_YEAR"]
-orderStringType = Literal["ASC", "DESC"]
 ApplicationDiscoveryServiceServiceName = Literal["discovery"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -122,14 +120,15 @@
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
@@ -140,14 +139,15 @@
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
@@ -165,14 +165,15 @@
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
@@ -185,24 +186,26 @@
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
@@ -263,15 +266,14 @@
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
@@ -343,17 +345,19 @@
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
@@ -398,14 +402,15 @@
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
@@ -443,19 +448,21 @@
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
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/literals.pyi` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
     "DescribeTagsPaginatorName",
     "ExportDataFormatType",
     "ExportStatusType",
     "ImportStatusType",
     "ImportTaskFilterNameType",
     "ListConfigurationsPaginatorName",
     "OfferingClassType",
+    "OrderStringType",
     "PurchasingOptionType",
     "TenancyType",
     "TermLengthType",
-    "orderStringType",
     "ApplicationDiscoveryServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -89,18 +89,18 @@
     "IMPORT_FAILED_SERVER_LIMIT_EXCEEDED",
     "IMPORT_IN_PROGRESS",
     "INTERNAL_ERROR",
 ]
 ImportTaskFilterNameType = Literal["IMPORT_TASK_ID", "NAME", "STATUS"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 OfferingClassType = Literal["CONVERTIBLE", "STANDARD"]
+OrderStringType = Literal["ASC", "DESC"]
 PurchasingOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 TenancyType = Literal["DEDICATED", "SHARED"]
 TermLengthType = Literal["ONE_YEAR", "THREE_YEAR"]
-orderStringType = Literal["ASC", "DESC"]
 ApplicationDiscoveryServiceServiceName = Literal["discovery"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -120,14 +120,15 @@
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
@@ -138,14 +139,15 @@
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
@@ -163,14 +165,15 @@
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
@@ -183,24 +186,26 @@
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
@@ -261,15 +266,14 @@
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
@@ -341,17 +345,19 @@
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
@@ -396,14 +402,15 @@
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
@@ -441,19 +448,21 @@
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
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/paginator.py` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "DescribeExportConfigurationsPaginator",
     "DescribeExportTasksPaginator",
     "DescribeImportTasksPaginator",
     "DescribeTagsPaginator",
     "ListConfigurationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -81,15 +80,15 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeagentspaginator)
         """
 
 
@@ -130,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexporttaskspaginator)
         """
 
 
@@ -148,15 +147,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeimporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeImportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeImportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeimporttaskspaginator)
         """
 
 
@@ -166,15 +165,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
         """
 
 
@@ -186,13 +185,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/paginator.pyi` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeagentspaginator)
         """
 
 class DescribeContinuousExportsPaginator(Paginator):
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexporttaskspaginator)
         """
 
 class DescribeImportTasksPaginator(Paginator):
@@ -141,15 +141,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeimporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeImportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeImportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeimporttaskspaginator)
         """
 
 class DescribeTagsPaginator(Paginator):
@@ -158,15 +158,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
         """
 
 class ListConfigurationsPaginator(Paginator):
@@ -177,13 +177,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/type_defs.py` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     ConfigurationItemTypeType,
     ContinuousExportStatusType,
     DeleteAgentErrorCodeType,
     ExportStatusType,
     ImportStatusType,
     ImportTaskFilterNameType,
     OfferingClassType,
+    OrderStringType,
     PurchasingOptionType,
     TenancyType,
     TermLengthType,
-    orderStringType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AgentConfigurationStatusTypeDef",
     "AgentNetworkInfoTypeDef",
     "AssociateConfigurationItemsToApplicationRequestRequestTypeDef",
     "BatchDeleteAgentErrorTypeDef",
     "DeleteAgentTypeDef",
     "ResponseMetadataTypeDef",
@@ -172,18 +171,18 @@
         "force": NotRequired[bool],
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
 DeletionWarningTypeDef = TypedDict(
     "DeletionWarningTypeDef",
     {
         "configurationId": NotRequired[str],
         "warningCode": NotRequired[int],
@@ -423,15 +422,15 @@
         "percentageAdjust": NotRequired[float],
     },
 )
 OrderByElementTypeDef = TypedDict(
     "OrderByElementTypeDef",
     {
         "fieldName": str,
-        "sortOrder": NotRequired[orderStringType],
+        "sortOrder": NotRequired[OrderStringType],
     },
 )
 ListServerNeighborsRequestRequestTypeDef = TypedDict(
     "ListServerNeighborsRequestRequestTypeDef",
     {
         "configurationId": str,
         "portInformationNeeded": NotRequired[bool],
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery/type_defs.pyi` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     ConfigurationItemTypeType,
     ContinuousExportStatusType,
     DeleteAgentErrorCodeType,
     ExportStatusType,
     ImportStatusType,
     ImportTaskFilterNameType,
     OfferingClassType,
+    OrderStringType,
     PurchasingOptionType,
     TenancyType,
     TermLengthType,
-    orderStringType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -171,18 +171,18 @@
         "force": NotRequired[bool],
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
 DeletionWarningTypeDef = TypedDict(
     "DeletionWarningTypeDef",
     {
         "configurationId": NotRequired[str],
         "warningCode": NotRequired[int],
@@ -422,15 +422,15 @@
         "percentageAdjust": NotRequired[float],
     },
 )
 OrderByElementTypeDef = TypedDict(
     "OrderByElementTypeDef",
     {
         "fieldName": str,
-        "sortOrder": NotRequired[orderStringType],
+        "sortOrder": NotRequired[OrderStringType],
     },
 )
 ListServerNeighborsRequestRequestTypeDef = TypedDict(
     "ListServerNeighborsRequestRequestTypeDef",
     {
         "configurationId": str,
         "portInformationNeeded": NotRequired[bool],
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/PKG-INFO` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.34.0
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.103
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.34.103 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
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
 
 <a id="mypy-boto3-discovery"></a>
 
 # mypy-boto3-discovery
 
 [![PyPI - mypy-boto3-discovery](https://img.shields.io/pypi/v/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-discovery-1.34.0/mypy_boto3_discovery.egg-info/SOURCES.txt` & `mypy_boto3_discovery-1.34.103/mypy_boto3_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.34.0/setup.py` & `mypy_boto3_discovery-1.34.103/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-discovery",
-    version="1.34.0",
+    version="1.34.103",
     packages=["mypy_boto3_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ApplicationDiscoveryService 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.ApplicationDiscoveryService 1.34.103 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 discovery type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_discovery": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

