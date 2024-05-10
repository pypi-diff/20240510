# Comparing `tmp/mypy-boto3-greengrassv2-1.34.0.tar.gz` & `tmp/mypy_boto3_greengrassv2-1.34.103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrassv2-1.34.0.tar", last modified: Wed Dec 13 21:22:45 2023, max compression
+gzip compressed data, was "mypy_boto3_greengrassv2-1.34.103.tar", last modified: Fri May 10 19:47:12 2024, max compression
```

## Comparing `mypy-boto3-greengrassv2-1.34.0.tar` & `mypy_boto3_greengrassv2-1.34.103.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:45.839227 mypy-boto3-greengrassv2-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14014 2023-12-13 21:22:45.839227 mypy-boto3-greengrassv2-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12461 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:45.839227 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25644 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25640 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9495 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33797 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33796 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:45.839227 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14014 2023-12-13 21:22:45.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 21:22:45.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:45.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:45.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:45.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 21:22:45.000000 mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:45.839227 mypy-boto3-greengrassv2-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-13 21:11:10.000000 mypy-boto3-greengrassv2-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:12.056250 mypy_boto3_greengrassv2-1.34.103/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-05-10 19:47:12.056250 mypy_boto3_greengrassv2-1.34.103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:12.056250 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25855 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    34920 2024-05-10 19:46:39.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34920 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:12.056250 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-05-10 19:47:12.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-10 19:47:12.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:47:12.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:47:12.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 19:47:12.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 19:47:12.000000 mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:47:12.056250 mypy_boto3_greengrassv2-1.34.103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 19:46:38.000000 mypy_boto3_greengrassv2-1.34.103/setup.py
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/LICENSE` & `mypy_boto3_greengrassv2-1.34.103/LICENSE`

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

### Comparing `mypy-boto3-greengrassv2-1.34.0/PKG-INFO` & `mypy_boto3_greengrassv2-1.34.103/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.34.0
-Summary: Type annotations for boto3.GreengrassV2 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.103
+Summary: Type annotations for boto3.GreengrassV2 1.34.103 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
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
 
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/README.md` & `mypy_boto3_greengrassv2-1.34.103/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/__init__.py` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListDeploymentsPaginator,
     ListEffectiveDeploymentsPaginator,
     ListInstalledComponentsPaginator,
 )
 
 Client = GreengrassV2Client
 
-
 __all__ = (
     "Client",
     "GreengrassV2Client",
     "ListClientDevicesAssociatedWithCoreDevicePaginator",
     "ListComponentVersionsPaginator",
     "ListComponentsPaginator",
     "ListCoreDevicesPaginator",
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/__init__.pyi` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/__main__.py` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GreengrassV2 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.GreengrassV2 1.34.103\n"
+        "Version:         1.34.103\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\n"
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

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/client.py` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ComponentVisibilityScopeType,
     CoreDeviceStatusType,
     DeploymentHistoryFilterType,
     InstalledComponentTopologyFilterType,
+    IotEndpointTypeType,
     RecipeOutputFormatType,
+    S3EndpointTypeType,
 )
 from .paginator import (
     ListClientDevicesAssociatedWithCoreDevicePaginator,
     ListComponentsPaginator,
     ListComponentVersionsPaginator,
     ListCoreDevicesPaginator,
     ListDeploymentsPaginator,
@@ -39,20 +41,20 @@
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     BlobTypeDef,
     CancelDeploymentResponseTypeDef,
     ComponentCandidateTypeDef,
-    ComponentDeploymentSpecificationTypeDef,
-    ComponentPlatformTypeDef,
+    ComponentDeploymentSpecificationUnionTypeDef,
+    ComponentPlatformUnionTypeDef,
     ConnectivityInfoTypeDef,
     CreateComponentVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
-    DeploymentIoTJobConfigurationTypeDef,
+    DeploymentIoTJobConfigurationUnionTypeDef,
     DeploymentPoliciesTypeDef,
     DescribeComponentResponseTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentResponseTypeDef,
     GetComponentVersionArtifactResponseTypeDef,
@@ -74,15 +76,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GreengrassV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -131,28 +132,28 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#associate_service_role_to_account)
         """
 
     def batch_associate_client_device_with_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...,
     ) -> BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef:
         """
         Associates a list of client devices with a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_associate_client_device_with_core_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#batch_associate_client_device_with_core_device)
         """
 
     def batch_disassociate_client_device_from_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...,
     ) -> BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef:
         """
         Disassociates a list of client devices from a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_disassociate_client_device_from_core_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#batch_disassociate_client_device_from_core_device)
         """
@@ -183,34 +184,34 @@
 
     def create_component_version(
         self,
         *,
         inlineRecipe: BlobTypeDef = ...,
         lambdaFunction: LambdaFunctionRecipeSourceTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateComponentVersionResponseTypeDef:
         """
         Creates a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_component_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#create_component_version)
         """
 
     def create_deployment(
         self,
         *,
         targetArn: str,
         deploymentName: str = ...,
-        components: Mapping[str, ComponentDeploymentSpecificationTypeDef] = ...,
-        iotJobConfiguration: DeploymentIoTJobConfigurationTypeDef = ...,
+        components: Mapping[str, ComponentDeploymentSpecificationUnionTypeDef] = ...,
+        iotJobConfiguration: DeploymentIoTJobConfigurationUnionTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
         or group of core
         devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_deployment)
@@ -282,15 +283,20 @@
         Gets the recipe for a version of a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#get_component)
         """
 
     def get_component_version_artifact(
-        self, *, arn: str, artifactName: str
+        self,
+        *,
+        arn: str,
+        artifactName: str,
+        s3EndpointType: S3EndpointTypeType = ...,
+        iotEndpointType: IotEndpointTypeType = ...,
     ) -> GetComponentVersionArtifactResponseTypeDef:
         """
         Gets the pre-signed URL to download a public or a Lambda component artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.get_component_version_artifact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#get_component_version_artifact)
         """
@@ -351,30 +357,30 @@
         """
 
     def list_components(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Retrieves a paginated list of component summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_components)
         """
 
     def list_core_devices(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoreDevicesResponseTypeDef:
         """
         Retrieves a paginated list of Greengrass core devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_core_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_core_devices)
         """
@@ -382,15 +388,15 @@
     def list_deployments(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsResponseTypeDef:
         """
         Retrieves a paginated list of deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_deployments)
         """
@@ -409,15 +415,15 @@
 
     def list_installed_components(
         self,
         *,
         coreDeviceThingName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        topologyFilter: InstalledComponentTopologyFilterType = ...
+        topologyFilter: InstalledComponentTopologyFilterType = ...,
     ) -> ListInstalledComponentsResponseTypeDef:
         """
         Retrieves a paginated list of the components that a Greengrass core device runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_installed_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_installed_components)
         """
@@ -429,16 +435,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_tags_for_resource)
         """
 
     def resolve_component_candidates(
         self,
         *,
-        platform: ComponentPlatformTypeDef = ...,
-        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
+        platform: ComponentPlatformUnionTypeDef = ...,
+        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...,
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a
         deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/client.pyi` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ComponentVisibilityScopeType,
     CoreDeviceStatusType,
     DeploymentHistoryFilterType,
     InstalledComponentTopologyFilterType,
+    IotEndpointTypeType,
     RecipeOutputFormatType,
+    S3EndpointTypeType,
 )
 from .paginator import (
     ListClientDevicesAssociatedWithCoreDevicePaginator,
     ListComponentsPaginator,
     ListComponentVersionsPaginator,
     ListCoreDevicesPaginator,
     ListDeploymentsPaginator,
@@ -39,20 +41,20 @@
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     BlobTypeDef,
     CancelDeploymentResponseTypeDef,
     ComponentCandidateTypeDef,
-    ComponentDeploymentSpecificationTypeDef,
-    ComponentPlatformTypeDef,
+    ComponentDeploymentSpecificationUnionTypeDef,
+    ComponentPlatformUnionTypeDef,
     ConnectivityInfoTypeDef,
     CreateComponentVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
-    DeploymentIoTJobConfigurationTypeDef,
+    DeploymentIoTJobConfigurationUnionTypeDef,
     DeploymentPoliciesTypeDef,
     DescribeComponentResponseTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentResponseTypeDef,
     GetComponentVersionArtifactResponseTypeDef,
@@ -127,28 +129,28 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#associate_service_role_to_account)
         """
 
     def batch_associate_client_device_with_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...,
     ) -> BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef:
         """
         Associates a list of client devices with a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_associate_client_device_with_core_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#batch_associate_client_device_with_core_device)
         """
 
     def batch_disassociate_client_device_from_core_device(
         self,
         *,
         coreDeviceThingName: str,
-        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...
+        entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...,
     ) -> BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef:
         """
         Disassociates a list of client devices from a core device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.batch_disassociate_client_device_from_core_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#batch_disassociate_client_device_from_core_device)
         """
@@ -179,34 +181,34 @@
 
     def create_component_version(
         self,
         *,
         inlineRecipe: BlobTypeDef = ...,
         lambdaFunction: LambdaFunctionRecipeSourceTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateComponentVersionResponseTypeDef:
         """
         Creates a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_component_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#create_component_version)
         """
 
     def create_deployment(
         self,
         *,
         targetArn: str,
         deploymentName: str = ...,
-        components: Mapping[str, ComponentDeploymentSpecificationTypeDef] = ...,
-        iotJobConfiguration: DeploymentIoTJobConfigurationTypeDef = ...,
+        components: Mapping[str, ComponentDeploymentSpecificationUnionTypeDef] = ...,
+        iotJobConfiguration: DeploymentIoTJobConfigurationUnionTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
         or group of core
         devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.create_deployment)
@@ -278,15 +280,20 @@
         Gets the recipe for a version of a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#get_component)
         """
 
     def get_component_version_artifact(
-        self, *, arn: str, artifactName: str
+        self,
+        *,
+        arn: str,
+        artifactName: str,
+        s3EndpointType: S3EndpointTypeType = ...,
+        iotEndpointType: IotEndpointTypeType = ...,
     ) -> GetComponentVersionArtifactResponseTypeDef:
         """
         Gets the pre-signed URL to download a public or a Lambda component artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.get_component_version_artifact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#get_component_version_artifact)
         """
@@ -347,30 +354,30 @@
         """
 
     def list_components(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListComponentsResponseTypeDef:
         """
         Retrieves a paginated list of component summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_components)
         """
 
     def list_core_devices(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCoreDevicesResponseTypeDef:
         """
         Retrieves a paginated list of Greengrass core devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_core_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_core_devices)
         """
@@ -378,15 +385,15 @@
     def list_deployments(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListDeploymentsResponseTypeDef:
         """
         Retrieves a paginated list of deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_deployments)
         """
@@ -405,15 +412,15 @@
 
     def list_installed_components(
         self,
         *,
         coreDeviceThingName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        topologyFilter: InstalledComponentTopologyFilterType = ...
+        topologyFilter: InstalledComponentTopologyFilterType = ...,
     ) -> ListInstalledComponentsResponseTypeDef:
         """
         Retrieves a paginated list of the components that a Greengrass core device runs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_installed_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_installed_components)
         """
@@ -425,16 +432,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_tags_for_resource)
         """
 
     def resolve_component_candidates(
         self,
         *,
-        platform: ComponentPlatformTypeDef = ...,
-        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
+        platform: ComponentPlatformUnionTypeDef = ...,
+        componentCandidates: Sequence[ComponentCandidateTypeDef] = ...,
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a
         deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/literals.py` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,50 +15,50 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CloudComponentStateType",
     "ComponentDependencyTypeType",
     "ComponentVisibilityScopeType",
     "CoreDeviceStatusType",
     "DeploymentComponentUpdatePolicyActionType",
     "DeploymentFailureHandlingPolicyType",
     "DeploymentHistoryFilterType",
     "DeploymentStatusType",
     "EffectiveDeploymentExecutionStatusType",
     "InstalledComponentLifecycleStateType",
     "InstalledComponentTopologyFilterType",
     "IoTJobAbortActionType",
     "IoTJobExecutionFailureTypeType",
+    "IotEndpointTypeType",
     "LambdaEventSourceTypeType",
     "LambdaFilesystemPermissionType",
     "LambdaInputPayloadEncodingTypeType",
     "LambdaIsolationModeType",
     "ListClientDevicesAssociatedWithCoreDevicePaginatorName",
     "ListComponentVersionsPaginatorName",
     "ListComponentsPaginatorName",
     "ListCoreDevicesPaginatorName",
     "ListDeploymentsPaginatorName",
     "ListEffectiveDeploymentsPaginatorName",
     "ListInstalledComponentsPaginatorName",
     "RecipeOutputFormatType",
+    "S3EndpointTypeType",
     "VendorGuidanceType",
     "GreengrassV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CloudComponentStateType = Literal["DEPLOYABLE", "DEPRECATED", "FAILED", "INITIATED", "REQUESTED"]
 ComponentDependencyTypeType = Literal["HARD", "SOFT"]
 ComponentVisibilityScopeType = Literal["PRIVATE", "PUBLIC"]
 CoreDeviceStatusType = Literal["HEALTHY", "UNHEALTHY"]
 DeploymentComponentUpdatePolicyActionType = Literal["NOTIFY_COMPONENTS", "SKIP_NOTIFY_COMPONENTS"]
 DeploymentFailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK"]
 DeploymentHistoryFilterType = Literal["ALL", "LATEST_ONLY"]
@@ -68,28 +68,30 @@
 ]
 InstalledComponentLifecycleStateType = Literal[
     "BROKEN", "ERRORED", "FINISHED", "INSTALLED", "NEW", "RUNNING", "STARTING", "STOPPING"
 ]
 InstalledComponentTopologyFilterType = Literal["ALL", "ROOT"]
 IoTJobAbortActionType = Literal["CANCEL"]
 IoTJobExecutionFailureTypeType = Literal["ALL", "FAILED", "REJECTED", "TIMED_OUT"]
+IotEndpointTypeType = Literal["fips", "standard"]
 LambdaEventSourceTypeType = Literal["IOT_CORE", "PUB_SUB"]
 LambdaFilesystemPermissionType = Literal["ro", "rw"]
 LambdaInputPayloadEncodingTypeType = Literal["binary", "json"]
 LambdaIsolationModeType = Literal["GreengrassContainer", "NoContainer"]
 ListClientDevicesAssociatedWithCoreDevicePaginatorName = Literal[
     "list_client_devices_associated_with_core_device"
 ]
 ListComponentVersionsPaginatorName = Literal["list_component_versions"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListCoreDevicesPaginatorName = Literal["list_core_devices"]
 ListDeploymentsPaginatorName = Literal["list_deployments"]
 ListEffectiveDeploymentsPaginatorName = Literal["list_effective_deployments"]
 ListInstalledComponentsPaginatorName = Literal["list_installed_components"]
 RecipeOutputFormatType = Literal["JSON", "YAML"]
+S3EndpointTypeType = Literal["GLOBAL", "REGIONAL"]
 VendorGuidanceType = Literal["ACTIVE", "DELETED", "DISCONTINUED"]
 GreengrassV2ServiceName = Literal["greengrassv2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -110,14 +112,15 @@
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
@@ -128,14 +131,15 @@
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
@@ -153,14 +157,15 @@
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
@@ -173,24 +178,26 @@
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
@@ -251,15 +258,14 @@
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
@@ -331,17 +337,19 @@
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
@@ -386,14 +394,15 @@
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
@@ -431,19 +440,21 @@
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

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/literals.pyi` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,28 @@
     "DeploymentHistoryFilterType",
     "DeploymentStatusType",
     "EffectiveDeploymentExecutionStatusType",
     "InstalledComponentLifecycleStateType",
     "InstalledComponentTopologyFilterType",
     "IoTJobAbortActionType",
     "IoTJobExecutionFailureTypeType",
+    "IotEndpointTypeType",
     "LambdaEventSourceTypeType",
     "LambdaFilesystemPermissionType",
     "LambdaInputPayloadEncodingTypeType",
     "LambdaIsolationModeType",
     "ListClientDevicesAssociatedWithCoreDevicePaginatorName",
     "ListComponentVersionsPaginatorName",
     "ListComponentsPaginatorName",
     "ListCoreDevicesPaginatorName",
     "ListDeploymentsPaginatorName",
     "ListEffectiveDeploymentsPaginatorName",
     "ListInstalledComponentsPaginatorName",
     "RecipeOutputFormatType",
+    "S3EndpointTypeType",
     "VendorGuidanceType",
     "GreengrassV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -66,28 +68,30 @@
 ]
 InstalledComponentLifecycleStateType = Literal[
     "BROKEN", "ERRORED", "FINISHED", "INSTALLED", "NEW", "RUNNING", "STARTING", "STOPPING"
 ]
 InstalledComponentTopologyFilterType = Literal["ALL", "ROOT"]
 IoTJobAbortActionType = Literal["CANCEL"]
 IoTJobExecutionFailureTypeType = Literal["ALL", "FAILED", "REJECTED", "TIMED_OUT"]
+IotEndpointTypeType = Literal["fips", "standard"]
 LambdaEventSourceTypeType = Literal["IOT_CORE", "PUB_SUB"]
 LambdaFilesystemPermissionType = Literal["ro", "rw"]
 LambdaInputPayloadEncodingTypeType = Literal["binary", "json"]
 LambdaIsolationModeType = Literal["GreengrassContainer", "NoContainer"]
 ListClientDevicesAssociatedWithCoreDevicePaginatorName = Literal[
     "list_client_devices_associated_with_core_device"
 ]
 ListComponentVersionsPaginatorName = Literal["list_component_versions"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListCoreDevicesPaginatorName = Literal["list_core_devices"]
 ListDeploymentsPaginatorName = Literal["list_deployments"]
 ListEffectiveDeploymentsPaginatorName = Literal["list_effective_deployments"]
 ListInstalledComponentsPaginatorName = Literal["list_installed_components"]
 RecipeOutputFormatType = Literal["JSON", "YAML"]
+S3EndpointTypeType = Literal["GLOBAL", "REGIONAL"]
 VendorGuidanceType = Literal["ACTIVE", "DELETED", "DISCONTINUED"]
 GreengrassV2ServiceName = Literal["greengrassv2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -108,14 +112,15 @@
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
@@ -126,14 +131,15 @@
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
@@ -151,14 +157,15 @@
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
@@ -171,24 +178,26 @@
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
@@ -249,15 +258,14 @@
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
@@ -329,17 +337,19 @@
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
@@ -384,14 +394,15 @@
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
@@ -429,19 +440,21 @@
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

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/paginator.py` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ComponentVisibilityScopeType,
     CoreDeviceStatusType,
     DeploymentHistoryFilterType,
     InstalledComponentTopologyFilterType,
 )
 from .type_defs import (
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
-    ListComponentsResponsePaginatorTypeDef,
+    ListComponentsResponseTypeDef,
     ListComponentVersionsResponseTypeDef,
     ListCoreDevicesResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     ListInstalledComponentsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
@@ -59,137 +59,128 @@
     "ListComponentsPaginator",
     "ListCoreDevicesPaginator",
     "ListDeploymentsPaginator",
     "ListEffectiveDeploymentsPaginator",
     "ListInstalledComponentsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListClientDevicesAssociatedWithCoreDevicePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
     """
 
     def paginate(
         self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
         """
 
-
 class ListComponentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
     """
 
     def paginate(
         self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
         """
 
-
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListComponentsResponsePaginatorTypeDef]:
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
         """
 
-
 class ListCoreDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
-
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
-
 class ListEffectiveDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
     """
 
     def paginate(
         self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEffectiveDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
         """
 
-
 class ListInstalledComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/paginator.pyi` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ComponentVisibilityScopeType,
     CoreDeviceStatusType,
     DeploymentHistoryFilterType,
     InstalledComponentTopologyFilterType,
 )
 from .type_defs import (
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
-    ListComponentsResponsePaginatorTypeDef,
+    ListComponentsResponseTypeDef,
     ListComponentVersionsResponseTypeDef,
     ListCoreDevicesResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     ListInstalledComponentsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
@@ -61,126 +61,134 @@
     "ListDeploymentsPaginator",
     "ListEffectiveDeploymentsPaginator",
     "ListInstalledComponentsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListClientDevicesAssociatedWithCoreDevicePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
     """
 
     def paginate(
         self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
         """
 
+
 class ListComponentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
     """
 
     def paginate(
         self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
         """
 
+
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListComponentsResponsePaginatorTypeDef]:
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
         """
 
+
 class ListCoreDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
+
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
+
 class ListEffectiveDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
     """
 
     def paginate(
         self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEffectiveDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
         """
 
+
 class ListInstalledComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/type_defs.py` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,22 @@
     DeploymentComponentUpdatePolicyActionType,
     DeploymentFailureHandlingPolicyType,
     DeploymentHistoryFilterType,
     DeploymentStatusType,
     EffectiveDeploymentExecutionStatusType,
     InstalledComponentLifecycleStateType,
     InstalledComponentTopologyFilterType,
+    IotEndpointTypeType,
     IoTJobExecutionFailureTypeType,
     LambdaEventSourceTypeType,
     LambdaFilesystemPermissionType,
     LambdaInputPayloadEncodingTypeType,
     LambdaIsolationModeType,
     RecipeOutputFormatType,
+    S3EndpointTypeType,
     VendorGuidanceType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -48,30 +50,31 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
+    "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
-    "ComponentPlatformPaginatorTypeDef",
+    "ComponentPlatformOutputTypeDef",
+    "ComponentPlatformExtraOutputTypeDef",
     "ComponentPlatformTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
@@ -118,50 +121,53 @@
     "GetServiceRoleForAccountResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
-    "ComponentLatestVersionPaginatorTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
+    "ComponentPlatformUnionTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
+    "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
-    "ComponentPaginatorTypeDef",
     "ComponentTypeDef",
+    "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
-    "ListComponentsResponsePaginatorTypeDef",
     "ListComponentsResponseTypeDef",
+    "ComponentDeploymentSpecificationUnionTypeDef",
+    "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
-    "CreateDeploymentRequestRequestTypeDef",
     "GetDeploymentResponseTypeDef",
+    "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentIoTJobConfigurationUnionTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -182,18 +188,18 @@
         "roleArn": str,
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
 AssociatedClientDeviceTypeDef = TypedDict(
     "AssociatedClientDeviceTypeDef",
     {
         "thingName": NotRequired[str],
         "associationTimestamp": NotRequired[datetime],
@@ -234,30 +240,44 @@
     "ComponentCandidateTypeDef",
     {
         "componentName": NotRequired[str],
         "componentVersion": NotRequired[str],
         "versionRequirements": NotRequired[Mapping[str, str]],
     },
 )
+ComponentConfigurationUpdateOutputTypeDef = TypedDict(
+    "ComponentConfigurationUpdateOutputTypeDef",
+    {
+        "merge": NotRequired[str],
+        "reset": NotRequired[List[str]],
+    },
+)
 ComponentConfigurationUpdateTypeDef = TypedDict(
     "ComponentConfigurationUpdateTypeDef",
     {
         "merge": NotRequired[str],
         "reset": NotRequired[Sequence[str]],
     },
 )
 ComponentDependencyRequirementTypeDef = TypedDict(
     "ComponentDependencyRequirementTypeDef",
     {
         "versionRequirement": NotRequired[str],
         "dependencyType": NotRequired[ComponentDependencyTypeType],
     },
 )
-ComponentPlatformPaginatorTypeDef = TypedDict(
-    "ComponentPlatformPaginatorTypeDef",
+ComponentPlatformOutputTypeDef = TypedDict(
+    "ComponentPlatformOutputTypeDef",
+    {
+        "name": NotRequired[str],
+        "attributes": NotRequired[Dict[str, str]],
+    },
+)
+ComponentPlatformExtraOutputTypeDef = TypedDict(
+    "ComponentPlatformExtraOutputTypeDef",
     {
         "name": NotRequired[str],
         "attributes": NotRequired[Dict[str, str]],
     },
 )
 ComponentPlatformTypeDef = TypedDict(
     "ComponentPlatformTypeDef",
@@ -369,14 +389,16 @@
     },
 )
 GetComponentVersionArtifactRequestRequestTypeDef = TypedDict(
     "GetComponentVersionArtifactRequestRequestTypeDef",
     {
         "arn": str,
         "artifactName": str,
+        "s3EndpointType": NotRequired[S3EndpointTypeType],
+        "iotEndpointType": NotRequired[IotEndpointTypeType],
     },
 )
 GetConnectivityInfoRequestRequestTypeDef = TypedDict(
     "GetConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
     },
@@ -677,51 +699,41 @@
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "status": CloudComponentStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ComponentLatestVersionPaginatorTypeDef = TypedDict(
-    "ComponentLatestVersionPaginatorTypeDef",
-    {
-        "arn": NotRequired[str],
-        "componentVersion": NotRequired[str],
-        "creationTimestamp": NotRequired[datetime],
-        "description": NotRequired[str],
-        "publisher": NotRequired[str],
-        "platforms": NotRequired[List[ComponentPlatformPaginatorTypeDef]],
-    },
-)
 ComponentLatestVersionTypeDef = TypedDict(
     "ComponentLatestVersionTypeDef",
     {
         "arn": NotRequired[str],
         "componentVersion": NotRequired[str],
         "creationTimestamp": NotRequired[datetime],
         "description": NotRequired[str],
         "publisher": NotRequired[str],
-        "platforms": NotRequired[List[ComponentPlatformTypeDef]],
+        "platforms": NotRequired[List[ComponentPlatformOutputTypeDef]],
     },
 )
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
-        "platforms": List[ComponentPlatformTypeDef],
+        "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ComponentPlatformUnionTypeDef = Union[ComponentPlatformTypeDef, ComponentPlatformExtraOutputTypeDef]
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": NotRequired[ComponentPlatformTypeDef],
         "componentCandidates": NotRequired[Sequence[ComponentCandidateTypeDef]],
     },
 )
@@ -802,14 +814,20 @@
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IoTJobAbortConfigOutputTypeDef = TypedDict(
+    "IoTJobAbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[IoTJobAbortCriteriaTypeDef],
+    },
+)
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 IoTJobExponentialRolloutRateTypeDef = TypedDict(
@@ -885,34 +903,34 @@
 ResolveComponentCandidatesResponseTypeDef = TypedDict(
     "ResolveComponentCandidatesResponseTypeDef",
     {
         "resolvedComponentVersions": List[ResolvedComponentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ComponentPaginatorTypeDef = TypedDict(
-    "ComponentPaginatorTypeDef",
-    {
-        "arn": NotRequired[str],
-        "componentName": NotRequired[str],
-        "latestVersion": NotRequired[ComponentLatestVersionPaginatorTypeDef],
-    },
-)
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "arn": NotRequired[str],
         "componentName": NotRequired[str],
         "latestVersion": NotRequired[ComponentLatestVersionTypeDef],
     },
 )
+ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
+    "ComponentDeploymentSpecificationOutputTypeDef",
+    {
+        "componentVersion": str,
+        "configurationUpdate": NotRequired[ComponentConfigurationUpdateOutputTypeDef],
+        "runWith": NotRequired[ComponentRunWithTypeDef],
+    },
+)
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
-        "componentVersion": NotRequired[str],
+        "componentVersion": str,
         "configurationUpdate": NotRequired[ComponentConfigurationUpdateTypeDef],
         "runWith": NotRequired[ComponentRunWithTypeDef],
     },
 )
 ListEffectiveDeploymentsResponseTypeDef = TypedDict(
     "ListEffectiveDeploymentsResponseTypeDef",
     {
@@ -931,30 +949,33 @@
 LambdaLinuxProcessParamsTypeDef = TypedDict(
     "LambdaLinuxProcessParamsTypeDef",
     {
         "isolationMode": NotRequired[LambdaIsolationModeType],
         "containerParams": NotRequired[LambdaContainerParamsTypeDef],
     },
 )
-ListComponentsResponsePaginatorTypeDef = TypedDict(
-    "ListComponentsResponsePaginatorTypeDef",
-    {
-        "components": List[ComponentPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ComponentDeploymentSpecificationUnionTypeDef = Union[
+    ComponentDeploymentSpecificationTypeDef, ComponentDeploymentSpecificationOutputTypeDef
+]
+DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
+    "DeploymentIoTJobConfigurationOutputTypeDef",
+    {
+        "jobExecutionsRolloutConfig": NotRequired[IoTJobExecutionsRolloutConfigTypeDef],
+        "abortConfig": NotRequired[IoTJobAbortConfigOutputTypeDef],
+        "timeoutConfig": NotRequired[IoTJobTimeoutConfigTypeDef],
+    },
+)
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": NotRequired[IoTJobExecutionsRolloutConfigTypeDef],
         "abortConfig": NotRequired[IoTJobAbortConfigTypeDef],
         "timeoutConfig": NotRequired[IoTJobTimeoutConfigTypeDef],
     },
@@ -971,47 +992,50 @@
         "pinned": NotRequired[bool],
         "inputPayloadEncodingType": NotRequired[LambdaInputPayloadEncodingTypeType],
         "execArgs": NotRequired[Sequence[str]],
         "environmentVariables": NotRequired[Mapping[str, str]],
         "linuxProcessParams": NotRequired[LambdaLinuxProcessParamsTypeDef],
     },
 )
-CreateDeploymentRequestRequestTypeDef = TypedDict(
-    "CreateDeploymentRequestRequestTypeDef",
-    {
-        "targetArn": str,
-        "deploymentName": NotRequired[str],
-        "components": NotRequired[Mapping[str, ComponentDeploymentSpecificationTypeDef]],
-        "iotJobConfiguration": NotRequired[DeploymentIoTJobConfigurationTypeDef],
-        "deploymentPolicies": NotRequired[DeploymentPoliciesTypeDef],
-        "parentTargetArn": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
-        "clientToken": NotRequired[str],
-    },
-)
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
     {
         "targetArn": str,
         "revisionId": str,
         "deploymentId": str,
         "deploymentName": str,
         "deploymentStatus": DeploymentStatusType,
         "iotJobId": str,
         "iotJobArn": str,
-        "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
+        "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
         "deploymentPolicies": DeploymentPoliciesTypeDef,
-        "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
+        "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
         "creationTimestamp": datetime,
         "isLatestForTarget": bool,
         "parentTargetArn": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDeploymentRequestRequestTypeDef = TypedDict(
+    "CreateDeploymentRequestRequestTypeDef",
+    {
+        "targetArn": str,
+        "deploymentName": NotRequired[str],
+        "components": NotRequired[Mapping[str, ComponentDeploymentSpecificationUnionTypeDef]],
+        "iotJobConfiguration": NotRequired[DeploymentIoTJobConfigurationTypeDef],
+        "deploymentPolicies": NotRequired[DeploymentPoliciesTypeDef],
+        "parentTargetArn": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+        "clientToken": NotRequired[str],
+    },
+)
+DeploymentIoTJobConfigurationUnionTypeDef = Union[
+    DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
+]
 LambdaFunctionRecipeSourceTypeDef = TypedDict(
     "LambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
         "componentName": NotRequired[str],
         "componentVersion": NotRequired[str],
         "componentPlatforms": NotRequired[Sequence[ComponentPlatformTypeDef]],
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2/type_defs.pyi` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,22 @@
     DeploymentComponentUpdatePolicyActionType,
     DeploymentFailureHandlingPolicyType,
     DeploymentHistoryFilterType,
     DeploymentStatusType,
     EffectiveDeploymentExecutionStatusType,
     InstalledComponentLifecycleStateType,
     InstalledComponentTopologyFilterType,
+    IotEndpointTypeType,
     IoTJobExecutionFailureTypeType,
     LambdaEventSourceTypeType,
     LambdaFilesystemPermissionType,
     LambdaInputPayloadEncodingTypeType,
     LambdaIsolationModeType,
     RecipeOutputFormatType,
+    S3EndpointTypeType,
     VendorGuidanceType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -60,17 +62,19 @@
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
+    "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
-    "ComponentPlatformPaginatorTypeDef",
+    "ComponentPlatformOutputTypeDef",
+    "ComponentPlatformExtraOutputTypeDef",
     "ComponentPlatformTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
@@ -117,50 +121,53 @@
     "GetServiceRoleForAccountResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
-    "ComponentLatestVersionPaginatorTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
+    "ComponentPlatformUnionTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
+    "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
-    "ComponentPaginatorTypeDef",
     "ComponentTypeDef",
+    "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
-    "ListComponentsResponsePaginatorTypeDef",
     "ListComponentsResponseTypeDef",
+    "ComponentDeploymentSpecificationUnionTypeDef",
+    "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
-    "CreateDeploymentRequestRequestTypeDef",
     "GetDeploymentResponseTypeDef",
+    "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentIoTJobConfigurationUnionTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -181,18 +188,18 @@
         "roleArn": str,
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
 AssociatedClientDeviceTypeDef = TypedDict(
     "AssociatedClientDeviceTypeDef",
     {
         "thingName": NotRequired[str],
         "associationTimestamp": NotRequired[datetime],
@@ -233,30 +240,44 @@
     "ComponentCandidateTypeDef",
     {
         "componentName": NotRequired[str],
         "componentVersion": NotRequired[str],
         "versionRequirements": NotRequired[Mapping[str, str]],
     },
 )
+ComponentConfigurationUpdateOutputTypeDef = TypedDict(
+    "ComponentConfigurationUpdateOutputTypeDef",
+    {
+        "merge": NotRequired[str],
+        "reset": NotRequired[List[str]],
+    },
+)
 ComponentConfigurationUpdateTypeDef = TypedDict(
     "ComponentConfigurationUpdateTypeDef",
     {
         "merge": NotRequired[str],
         "reset": NotRequired[Sequence[str]],
     },
 )
 ComponentDependencyRequirementTypeDef = TypedDict(
     "ComponentDependencyRequirementTypeDef",
     {
         "versionRequirement": NotRequired[str],
         "dependencyType": NotRequired[ComponentDependencyTypeType],
     },
 )
-ComponentPlatformPaginatorTypeDef = TypedDict(
-    "ComponentPlatformPaginatorTypeDef",
+ComponentPlatformOutputTypeDef = TypedDict(
+    "ComponentPlatformOutputTypeDef",
+    {
+        "name": NotRequired[str],
+        "attributes": NotRequired[Dict[str, str]],
+    },
+)
+ComponentPlatformExtraOutputTypeDef = TypedDict(
+    "ComponentPlatformExtraOutputTypeDef",
     {
         "name": NotRequired[str],
         "attributes": NotRequired[Dict[str, str]],
     },
 )
 ComponentPlatformTypeDef = TypedDict(
     "ComponentPlatformTypeDef",
@@ -368,14 +389,16 @@
     },
 )
 GetComponentVersionArtifactRequestRequestTypeDef = TypedDict(
     "GetComponentVersionArtifactRequestRequestTypeDef",
     {
         "arn": str,
         "artifactName": str,
+        "s3EndpointType": NotRequired[S3EndpointTypeType],
+        "iotEndpointType": NotRequired[IotEndpointTypeType],
     },
 )
 GetConnectivityInfoRequestRequestTypeDef = TypedDict(
     "GetConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
     },
@@ -676,51 +699,41 @@
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "status": CloudComponentStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ComponentLatestVersionPaginatorTypeDef = TypedDict(
-    "ComponentLatestVersionPaginatorTypeDef",
-    {
-        "arn": NotRequired[str],
-        "componentVersion": NotRequired[str],
-        "creationTimestamp": NotRequired[datetime],
-        "description": NotRequired[str],
-        "publisher": NotRequired[str],
-        "platforms": NotRequired[List[ComponentPlatformPaginatorTypeDef]],
-    },
-)
 ComponentLatestVersionTypeDef = TypedDict(
     "ComponentLatestVersionTypeDef",
     {
         "arn": NotRequired[str],
         "componentVersion": NotRequired[str],
         "creationTimestamp": NotRequired[datetime],
         "description": NotRequired[str],
         "publisher": NotRequired[str],
-        "platforms": NotRequired[List[ComponentPlatformTypeDef]],
+        "platforms": NotRequired[List[ComponentPlatformOutputTypeDef]],
     },
 )
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
-        "platforms": List[ComponentPlatformTypeDef],
+        "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ComponentPlatformUnionTypeDef = Union[ComponentPlatformTypeDef, ComponentPlatformExtraOutputTypeDef]
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": NotRequired[ComponentPlatformTypeDef],
         "componentCandidates": NotRequired[Sequence[ComponentCandidateTypeDef]],
     },
 )
@@ -801,14 +814,20 @@
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IoTJobAbortConfigOutputTypeDef = TypedDict(
+    "IoTJobAbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[IoTJobAbortCriteriaTypeDef],
+    },
+)
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 IoTJobExponentialRolloutRateTypeDef = TypedDict(
@@ -884,34 +903,34 @@
 ResolveComponentCandidatesResponseTypeDef = TypedDict(
     "ResolveComponentCandidatesResponseTypeDef",
     {
         "resolvedComponentVersions": List[ResolvedComponentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ComponentPaginatorTypeDef = TypedDict(
-    "ComponentPaginatorTypeDef",
-    {
-        "arn": NotRequired[str],
-        "componentName": NotRequired[str],
-        "latestVersion": NotRequired[ComponentLatestVersionPaginatorTypeDef],
-    },
-)
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "arn": NotRequired[str],
         "componentName": NotRequired[str],
         "latestVersion": NotRequired[ComponentLatestVersionTypeDef],
     },
 )
+ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
+    "ComponentDeploymentSpecificationOutputTypeDef",
+    {
+        "componentVersion": str,
+        "configurationUpdate": NotRequired[ComponentConfigurationUpdateOutputTypeDef],
+        "runWith": NotRequired[ComponentRunWithTypeDef],
+    },
+)
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
-        "componentVersion": NotRequired[str],
+        "componentVersion": str,
         "configurationUpdate": NotRequired[ComponentConfigurationUpdateTypeDef],
         "runWith": NotRequired[ComponentRunWithTypeDef],
     },
 )
 ListEffectiveDeploymentsResponseTypeDef = TypedDict(
     "ListEffectiveDeploymentsResponseTypeDef",
     {
@@ -930,30 +949,33 @@
 LambdaLinuxProcessParamsTypeDef = TypedDict(
     "LambdaLinuxProcessParamsTypeDef",
     {
         "isolationMode": NotRequired[LambdaIsolationModeType],
         "containerParams": NotRequired[LambdaContainerParamsTypeDef],
     },
 )
-ListComponentsResponsePaginatorTypeDef = TypedDict(
-    "ListComponentsResponsePaginatorTypeDef",
-    {
-        "components": List[ComponentPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ComponentDeploymentSpecificationUnionTypeDef = Union[
+    ComponentDeploymentSpecificationTypeDef, ComponentDeploymentSpecificationOutputTypeDef
+]
+DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
+    "DeploymentIoTJobConfigurationOutputTypeDef",
+    {
+        "jobExecutionsRolloutConfig": NotRequired[IoTJobExecutionsRolloutConfigTypeDef],
+        "abortConfig": NotRequired[IoTJobAbortConfigOutputTypeDef],
+        "timeoutConfig": NotRequired[IoTJobTimeoutConfigTypeDef],
+    },
+)
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": NotRequired[IoTJobExecutionsRolloutConfigTypeDef],
         "abortConfig": NotRequired[IoTJobAbortConfigTypeDef],
         "timeoutConfig": NotRequired[IoTJobTimeoutConfigTypeDef],
     },
@@ -970,47 +992,50 @@
         "pinned": NotRequired[bool],
         "inputPayloadEncodingType": NotRequired[LambdaInputPayloadEncodingTypeType],
         "execArgs": NotRequired[Sequence[str]],
         "environmentVariables": NotRequired[Mapping[str, str]],
         "linuxProcessParams": NotRequired[LambdaLinuxProcessParamsTypeDef],
     },
 )
-CreateDeploymentRequestRequestTypeDef = TypedDict(
-    "CreateDeploymentRequestRequestTypeDef",
-    {
-        "targetArn": str,
-        "deploymentName": NotRequired[str],
-        "components": NotRequired[Mapping[str, ComponentDeploymentSpecificationTypeDef]],
-        "iotJobConfiguration": NotRequired[DeploymentIoTJobConfigurationTypeDef],
-        "deploymentPolicies": NotRequired[DeploymentPoliciesTypeDef],
-        "parentTargetArn": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
-        "clientToken": NotRequired[str],
-    },
-)
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
     {
         "targetArn": str,
         "revisionId": str,
         "deploymentId": str,
         "deploymentName": str,
         "deploymentStatus": DeploymentStatusType,
         "iotJobId": str,
         "iotJobArn": str,
-        "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
+        "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
         "deploymentPolicies": DeploymentPoliciesTypeDef,
-        "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
+        "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
         "creationTimestamp": datetime,
         "isLatestForTarget": bool,
         "parentTargetArn": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDeploymentRequestRequestTypeDef = TypedDict(
+    "CreateDeploymentRequestRequestTypeDef",
+    {
+        "targetArn": str,
+        "deploymentName": NotRequired[str],
+        "components": NotRequired[Mapping[str, ComponentDeploymentSpecificationUnionTypeDef]],
+        "iotJobConfiguration": NotRequired[DeploymentIoTJobConfigurationTypeDef],
+        "deploymentPolicies": NotRequired[DeploymentPoliciesTypeDef],
+        "parentTargetArn": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+        "clientToken": NotRequired[str],
+    },
+)
+DeploymentIoTJobConfigurationUnionTypeDef = Union[
+    DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
+]
 LambdaFunctionRecipeSourceTypeDef = TypedDict(
     "LambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
         "componentName": NotRequired[str],
         "componentVersion": NotRequired[str],
         "componentPlatforms": NotRequired[Sequence[ComponentPlatformTypeDef]],
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/PKG-INFO` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.34.0
-Summary: Type annotations for boto3.GreengrassV2 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.103
+Summary: Type annotations for boto3.GreengrassV2 1.34.103 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
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
 
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-greengrassv2-1.34.0/mypy_boto3_greengrassv2.egg-info/SOURCES.txt` & `mypy_boto3_greengrassv2-1.34.103/mypy_boto3_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.34.0/setup.py` & `mypy_boto3_greengrassv2-1.34.103/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrassv2",
-    version="1.34.0",
+    version="1.34.103",
     packages=["mypy_boto3_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.GreengrassV2 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.GreengrassV2 1.34.103 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 greengrassv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_greengrassv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

