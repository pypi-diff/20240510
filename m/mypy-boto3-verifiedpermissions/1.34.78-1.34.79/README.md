# Comparing `tmp/mypy-boto3-verifiedpermissions-1.34.78.tar.gz` & `tmp/mypy-boto3-verifiedpermissions-1.34.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-verifiedpermissions-1.34.78.tar", last modified: Thu Apr  4 19:33:18 2024, max compression
+gzip compressed data, was "mypy-boto3-verifiedpermissions-1.34.79.tar", last modified: Fri Apr  5 19:20:35 2024, max compression
```

## Comparing `mypy-boto3-verifiedpermissions-1.34.78.tar` & `mypy-boto3-verifiedpermissions-1.34.79.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:18.124019 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22033 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22030 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27707 2024-04-04 19:33:05.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27707 2024-04-04 19:33:05.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:35.462698 mypy-boto3-verifiedpermissions-1.34.79/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-04-05 19:20:35.462698 mypy-boto3-verifiedpermissions-1.34.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:35.462698 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22919 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-05 19:20:21.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-05 19:20:21.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-05 19:20:21.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29199 2024-04-05 19:20:21.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29199 2024-04-05 19:20:21.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:35.462698 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-04-05 19:20:35.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 19:20:35.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:35.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:35.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 19:20:35.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:20:35.000000 mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:20:35.462698 mypy-boto3-verifiedpermissions-1.34.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-05 19:20:20.000000 mypy-boto3-verifiedpermissions-1.34.79/setup.py
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/LICENSE` & `mypy-boto3-verifiedpermissions-1.34.79/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.34.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.34.78
-Summary: Type annotations for boto3.VerifiedPermissions 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.79
+Summary: Type annotations for boto3.VerifiedPermissions 1.34.79 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/README.md` & `mypy-boto3-verifiedpermissions-1.34.79/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.py` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.pyi` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__main__.py` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VerifiedPermissions 1.34.78\n"
-        "Version:         1.34.78\n"
+        "Type annotations for boto3.VerifiedPermissions 1.34.79\n"
+        "Version:         1.34.79\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.78")
+    print("1.34.79")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.py` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     ListPolicyStoresPaginator,
     ListPolicyTemplatesPaginator,
 )
 from .type_defs import (
     ActionIdentifierTypeDef,
     BatchIsAuthorizedInputItemTypeDef,
     BatchIsAuthorizedOutputTypeDef,
+    BatchIsAuthorizedWithTokenInputItemTypeDef,
+    BatchIsAuthorizedWithTokenOutputTypeDef,
     ConfigurationTypeDef,
     ContextDefinitionTypeDef,
     CreateIdentitySourceOutputTypeDef,
     CreatePolicyOutputTypeDef,
     CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateOutputTypeDef,
     EntitiesDefinitionTypeDef,
@@ -118,14 +120,30 @@
         principal or
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.batch_is_authorized)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/client/#batch_is_authorized)
         """
 
+    def batch_is_authorized_with_token(
+        self,
+        *,
+        policyStoreId: str,
+        requests: Sequence[BatchIsAuthorizedWithTokenInputItemTypeDef],
+        identityToken: str = ...,
+        accessToken: str = ...,
+        entities: EntitiesDefinitionTypeDef = ...,
+    ) -> BatchIsAuthorizedWithTokenOutputTypeDef:
+        """
+        Makes a series of decisions about multiple authorization requests for one token.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.batch_is_authorized_with_token)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/client/#batch_is_authorized_with_token)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/client/#can_paginate)
         """
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.pyi` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     ListPolicyStoresPaginator,
     ListPolicyTemplatesPaginator,
 )
 from .type_defs import (
     ActionIdentifierTypeDef,
     BatchIsAuthorizedInputItemTypeDef,
     BatchIsAuthorizedOutputTypeDef,
+    BatchIsAuthorizedWithTokenInputItemTypeDef,
+    BatchIsAuthorizedWithTokenOutputTypeDef,
     ConfigurationTypeDef,
     ContextDefinitionTypeDef,
     CreateIdentitySourceOutputTypeDef,
     CreatePolicyOutputTypeDef,
     CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateOutputTypeDef,
     EntitiesDefinitionTypeDef,
@@ -115,14 +117,30 @@
         principal or
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.batch_is_authorized)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/client/#batch_is_authorized)
         """
 
+    def batch_is_authorized_with_token(
+        self,
+        *,
+        policyStoreId: str,
+        requests: Sequence[BatchIsAuthorizedWithTokenInputItemTypeDef],
+        identityToken: str = ...,
+        accessToken: str = ...,
+        entities: EntitiesDefinitionTypeDef = ...,
+    ) -> BatchIsAuthorizedWithTokenOutputTypeDef:
+        """
+        Makes a series of decisions about multiple authorization requests for one token.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.batch_is_authorized_with_token)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/client/#batch_is_authorized_with_token)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/client/#can_paginate)
         """
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.py` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.pyi` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.py` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.pyi` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.py` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     "AttributeValueTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
     "BatchIsAuthorizedInputItemTypeDef",
+    "BatchIsAuthorizedWithTokenInputItemTypeDef",
     "CreateIdentitySourceOutputTypeDef",
     "CreatePolicyOutputTypeDef",
     "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateOutputTypeDef",
     "GetPolicyTemplateOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "IsAuthorizedOutputTypeDef",
@@ -104,28 +105,31 @@
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
     "PolicyDefinitionDetailTypeDef",
     "PolicyDefinitionItemTypeDef",
     "PolicyDefinitionTypeDef",
     "BatchIsAuthorizedOutputItemTypeDef",
+    "BatchIsAuthorizedWithTokenOutputItemTypeDef",
     "ConfigurationDetailTypeDef",
     "ConfigurationItemTypeDef",
     "ConfigurationTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedInputRequestTypeDef",
+    "BatchIsAuthorizedWithTokenInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
     "CreatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedOutputTypeDef",
+    "BatchIsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
     "IdentitySourceItemTypeDef",
     "CreateIdentitySourceInputRequestTypeDef",
     "UpdateIdentitySourceInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
     "ListIdentitySourcesOutputTypeDef",
 )
@@ -435,14 +439,22 @@
     {
         "principal": NotRequired[EntityIdentifierTypeDef],
         "action": NotRequired[ActionIdentifierTypeDef],
         "resource": NotRequired[EntityIdentifierTypeDef],
         "context": NotRequired[ContextDefinitionTypeDef],
     },
 )
+BatchIsAuthorizedWithTokenInputItemTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenInputItemTypeDef",
+    {
+        "action": NotRequired[ActionIdentifierTypeDef],
+        "resource": NotRequired[EntityIdentifierTypeDef],
+        "context": NotRequired[ContextDefinitionTypeDef],
+    },
+)
 CreateIdentitySourceOutputTypeDef = TypedDict(
     "CreateIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
@@ -739,14 +751,23 @@
     {
         "request": BatchIsAuthorizedInputItemTypeDef,
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
     },
 )
+BatchIsAuthorizedWithTokenOutputItemTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenOutputItemTypeDef",
+    {
+        "request": BatchIsAuthorizedWithTokenInputItemTypeDef,
+        "decision": DecisionType,
+        "determiningPolicies": List[DeterminingPolicyItemTypeDef],
+        "errors": List[EvaluationErrorItemTypeDef],
+    },
+)
 ConfigurationDetailTypeDef = TypedDict(
     "ConfigurationDetailTypeDef",
     {
         "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationDetailTypeDef],
     },
 )
 ConfigurationItemTypeDef = TypedDict(
@@ -779,14 +800,24 @@
     "BatchIsAuthorizedInputRequestTypeDef",
     {
         "policyStoreId": str,
         "requests": Sequence[BatchIsAuthorizedInputItemTypeDef],
         "entities": NotRequired[EntitiesDefinitionTypeDef],
     },
 )
+BatchIsAuthorizedWithTokenInputRequestTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "requests": Sequence[BatchIsAuthorizedWithTokenInputItemTypeDef],
+        "identityToken": NotRequired[str],
+        "accessToken": NotRequired[str],
+        "entities": NotRequired[EntitiesDefinitionTypeDef],
+    },
+)
 IsAuthorizedInputRequestTypeDef = TypedDict(
     "IsAuthorizedInputRequestTypeDef",
     {
         "policyStoreId": str,
         "principal": NotRequired[EntityIdentifierTypeDef],
         "action": NotRequired[ActionIdentifierTypeDef],
         "resource": NotRequired[EntityIdentifierTypeDef],
@@ -861,14 +892,22 @@
 BatchIsAuthorizedOutputTypeDef = TypedDict(
     "BatchIsAuthorizedOutputTypeDef",
     {
         "results": List[BatchIsAuthorizedOutputItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchIsAuthorizedWithTokenOutputTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenOutputTypeDef",
+    {
+        "principal": EntityIdentifierTypeDef,
+        "results": List[BatchIsAuthorizedWithTokenOutputItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.pyi` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     "AttributeValueTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
     "BatchIsAuthorizedInputItemTypeDef",
+    "BatchIsAuthorizedWithTokenInputItemTypeDef",
     "CreateIdentitySourceOutputTypeDef",
     "CreatePolicyOutputTypeDef",
     "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateOutputTypeDef",
     "GetPolicyTemplateOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "IsAuthorizedOutputTypeDef",
@@ -104,28 +105,31 @@
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
     "PolicyDefinitionDetailTypeDef",
     "PolicyDefinitionItemTypeDef",
     "PolicyDefinitionTypeDef",
     "BatchIsAuthorizedOutputItemTypeDef",
+    "BatchIsAuthorizedWithTokenOutputItemTypeDef",
     "ConfigurationDetailTypeDef",
     "ConfigurationItemTypeDef",
     "ConfigurationTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedInputRequestTypeDef",
+    "BatchIsAuthorizedWithTokenInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
     "CreatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedOutputTypeDef",
+    "BatchIsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
     "IdentitySourceItemTypeDef",
     "CreateIdentitySourceInputRequestTypeDef",
     "UpdateIdentitySourceInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
     "ListIdentitySourcesOutputTypeDef",
 )
@@ -435,14 +439,22 @@
     {
         "principal": NotRequired[EntityIdentifierTypeDef],
         "action": NotRequired[ActionIdentifierTypeDef],
         "resource": NotRequired[EntityIdentifierTypeDef],
         "context": NotRequired[ContextDefinitionTypeDef],
     },
 )
+BatchIsAuthorizedWithTokenInputItemTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenInputItemTypeDef",
+    {
+        "action": NotRequired[ActionIdentifierTypeDef],
+        "resource": NotRequired[EntityIdentifierTypeDef],
+        "context": NotRequired[ContextDefinitionTypeDef],
+    },
+)
 CreateIdentitySourceOutputTypeDef = TypedDict(
     "CreateIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
@@ -739,14 +751,23 @@
     {
         "request": BatchIsAuthorizedInputItemTypeDef,
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
     },
 )
+BatchIsAuthorizedWithTokenOutputItemTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenOutputItemTypeDef",
+    {
+        "request": BatchIsAuthorizedWithTokenInputItemTypeDef,
+        "decision": DecisionType,
+        "determiningPolicies": List[DeterminingPolicyItemTypeDef],
+        "errors": List[EvaluationErrorItemTypeDef],
+    },
+)
 ConfigurationDetailTypeDef = TypedDict(
     "ConfigurationDetailTypeDef",
     {
         "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationDetailTypeDef],
     },
 )
 ConfigurationItemTypeDef = TypedDict(
@@ -779,14 +800,24 @@
     "BatchIsAuthorizedInputRequestTypeDef",
     {
         "policyStoreId": str,
         "requests": Sequence[BatchIsAuthorizedInputItemTypeDef],
         "entities": NotRequired[EntitiesDefinitionTypeDef],
     },
 )
+BatchIsAuthorizedWithTokenInputRequestTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "requests": Sequence[BatchIsAuthorizedWithTokenInputItemTypeDef],
+        "identityToken": NotRequired[str],
+        "accessToken": NotRequired[str],
+        "entities": NotRequired[EntitiesDefinitionTypeDef],
+    },
+)
 IsAuthorizedInputRequestTypeDef = TypedDict(
     "IsAuthorizedInputRequestTypeDef",
     {
         "policyStoreId": str,
         "principal": NotRequired[EntityIdentifierTypeDef],
         "action": NotRequired[ActionIdentifierTypeDef],
         "resource": NotRequired[EntityIdentifierTypeDef],
@@ -861,14 +892,22 @@
 BatchIsAuthorizedOutputTypeDef = TypedDict(
     "BatchIsAuthorizedOutputTypeDef",
     {
         "results": List[BatchIsAuthorizedOutputItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchIsAuthorizedWithTokenOutputTypeDef = TypedDict(
+    "BatchIsAuthorizedWithTokenOutputTypeDef",
+    {
+        "principal": EntityIdentifierTypeDef,
+        "results": List[BatchIsAuthorizedWithTokenOutputItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.34.78
-Summary: Type annotations for boto3.VerifiedPermissions 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.79
+Summary: Type annotations for boto3.VerifiedPermissions 1.34.79 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt` & `mypy-boto3-verifiedpermissions-1.34.79/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.78/setup.py` & `mypy-boto3-verifiedpermissions-1.34.79/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-verifiedpermissions",
-    version="1.34.78",
+    version="1.34.79",
     packages=["mypy_boto3_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.VerifiedPermissions 1.34.78 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.VerifiedPermissions 1.34.79 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

