# Comparing `tmp/mypy-boto3-sso-oidc-1.34.0.tar.gz` & `tmp/mypy_boto3_sso_oidc-1.34.103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-oidc-1.34.0.tar", last modified: Wed Dec 13 21:23:57 2023, max compression
+gzip compressed data, was "mypy_boto3_sso_oidc-1.34.103.tar", last modified: Fri May 10 19:47:12 2024, max compression
```

## Comparing `mypy-boto3-sso-oidc-1.34.0.tar` & `mypy_boto3_sso_oidc-1.34.103.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:57.819395 mypy-boto3-sso-oidc-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2023-12-13 21:23:57.819395 mypy-boto3-sso-oidc-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:57.819395 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2023-12-13 21:20:28.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2023-12-13 21:20:28.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2023-12-13 21:20:28.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2023-12-13 21:20:28.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-13 21:20:28.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-12-13 21:20:28.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:57.819395 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2023-12-13 21:23:57.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-13 21:23:57.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:57.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:57.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:57.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-13 21:23:57.000000 mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:57.819395 mypy-boto3-sso-oidc-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2023-12-13 21:20:27.000000 mypy-boto3-sso-oidc-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:12.860256 mypy_boto3_sso_oidc-1.34.103/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-10 19:47:12.860256 mypy_boto3_sso_oidc-1.34.103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:12.860256 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:47:12.860256 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-10 19:47:12.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-10 19:47:12.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:47:12.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:47:12.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 19:47:12.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 19:47:12.000000 mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:47:12.860256 mypy_boto3_sso_oidc-1.34.103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-10 19:47:01.000000 mypy_boto3_sso_oidc-1.34.103/setup.py
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/LICENSE` & `mypy_boto3_sso_oidc-1.34.103/LICENSE`

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

### Comparing `mypy-boto3-sso-oidc-1.34.0/PKG-INFO` & `mypy_boto3_sso_oidc-1.34.103/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-oidc
-Version: 1.34.0
-Summary: Type annotations for boto3.SSOOIDC 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.103
+Summary: Type annotations for boto3.SSOOIDC 1.34.103 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/
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
 
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-oidc)](https://pepy.tech/project/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/README.md` & `mypy_boto3_sso_oidc-1.34.103/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-oidc)](https://pepy.tech/project/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/__main__.py` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSOOIDC 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.SSOOIDC 1.34.103\n"
+        "Version:         1.34.103\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC\n"
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

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/client.py` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -23,40 +23,38 @@
     CreateTokenWithIAMResponseTypeDef,
     RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 __all__ = ("SSOOIDCClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AuthorizationPendingException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ExpiredTokenException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidClientException: Type[BotocoreClientError]
     InvalidClientMetadataException: Type[BotocoreClientError]
     InvalidGrantException: Type[BotocoreClientError]
+    InvalidRedirectUriException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidRequestRegionException: Type[BotocoreClientError]
     InvalidScopeException: Type[BotocoreClientError]
     SlowDownException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
     UnsupportedGrantTypeException: Type[BotocoreClientError]
 
-
 class SSOOIDCClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/client/)
     """
 
     meta: ClientMeta
@@ -92,15 +90,16 @@
         clientId: str,
         clientSecret: str,
         grantType: str,
         deviceCode: str = ...,
         code: str = ...,
         refreshToken: str = ...,
         scope: Sequence[str] = ...,
-        redirectUri: str = ...
+        redirectUri: str = ...,
+        codeVerifier: str = ...,
     ) -> CreateTokenResponseTypeDef:
         """
         Creates and returns access and refresh tokens for clients that are
         authenticated using client
         secrets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.create_token)
@@ -115,15 +114,16 @@
         code: str = ...,
         refreshToken: str = ...,
         assertion: str = ...,
         scope: Sequence[str] = ...,
         redirectUri: str = ...,
         subjectToken: str = ...,
         subjectTokenType: str = ...,
-        requestedTokenType: str = ...
+        requestedTokenType: str = ...,
+        codeVerifier: str = ...,
     ) -> CreateTokenWithIAMResponseTypeDef:
         """
         Creates and returns access and refresh tokens for clients and applications that
         are authenticated using IAM
         entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.create_token_with_iam)
@@ -141,15 +141,23 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/client/#generate_presigned_url)
         """
 
     def register_client(
-        self, *, clientName: str, clientType: str, scopes: Sequence[str] = ...
+        self,
+        *,
+        clientName: str,
+        clientType: str,
+        scopes: Sequence[str] = ...,
+        redirectUris: Sequence[str] = ...,
+        grantTypes: Sequence[str] = ...,
+        issuerUrl: str = ...,
+        entitledApplicationArn: str = ...,
     ) -> RegisterClientResponseTypeDef:
         """
         Registers a client with IAM Identity Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.register_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/client/#register_client)
         """
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/client.pyi` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,37 +23,41 @@
     CreateTokenWithIAMResponseTypeDef,
     RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 __all__ = ("SSOOIDCClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AuthorizationPendingException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ExpiredTokenException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidClientException: Type[BotocoreClientError]
     InvalidClientMetadataException: Type[BotocoreClientError]
     InvalidGrantException: Type[BotocoreClientError]
+    InvalidRedirectUriException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidRequestRegionException: Type[BotocoreClientError]
     InvalidScopeException: Type[BotocoreClientError]
     SlowDownException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
     UnsupportedGrantTypeException: Type[BotocoreClientError]
 
+
 class SSOOIDCClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/client/)
     """
 
     meta: ClientMeta
@@ -89,15 +93,16 @@
         clientId: str,
         clientSecret: str,
         grantType: str,
         deviceCode: str = ...,
         code: str = ...,
         refreshToken: str = ...,
         scope: Sequence[str] = ...,
-        redirectUri: str = ...
+        redirectUri: str = ...,
+        codeVerifier: str = ...,
     ) -> CreateTokenResponseTypeDef:
         """
         Creates and returns access and refresh tokens for clients that are
         authenticated using client
         secrets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.create_token)
@@ -112,15 +117,16 @@
         code: str = ...,
         refreshToken: str = ...,
         assertion: str = ...,
         scope: Sequence[str] = ...,
         redirectUri: str = ...,
         subjectToken: str = ...,
         subjectTokenType: str = ...,
-        requestedTokenType: str = ...
+        requestedTokenType: str = ...,
+        codeVerifier: str = ...,
     ) -> CreateTokenWithIAMResponseTypeDef:
         """
         Creates and returns access and refresh tokens for clients and applications that
         are authenticated using IAM
         entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.create_token_with_iam)
@@ -138,15 +144,23 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/client/#generate_presigned_url)
         """
 
     def register_client(
-        self, *, clientName: str, clientType: str, scopes: Sequence[str] = ...
+        self,
+        *,
+        clientName: str,
+        clientType: str,
+        scopes: Sequence[str] = ...,
+        redirectUris: Sequence[str] = ...,
+        grantTypes: Sequence[str] = ...,
+        issuerUrl: str = ...,
+        entitledApplicationArn: str = ...,
     ) -> RegisterClientResponseTypeDef:
         """
         Registers a client with IAM Identity Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client.register_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/client/#register_client)
         """
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/literals.py` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSOOIDCServiceName", "ServiceName", "ResourceServiceName", "RegionName")
 
-
 SSOOIDCServiceName = Literal["sso-oidc"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -46,14 +44,15 @@
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
@@ -64,14 +63,15 @@
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
@@ -89,14 +89,15 @@
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
@@ -109,24 +110,26 @@
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
@@ -187,15 +190,14 @@
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
@@ -267,17 +269,19 @@
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
@@ -322,14 +326,15 @@
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
@@ -367,19 +372,21 @@
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
@@ -415,26 +422,30 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "il-central-1",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/literals.pyi` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
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
@@ -62,14 +63,15 @@
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
@@ -87,14 +89,15 @@
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
@@ -107,24 +110,26 @@
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
@@ -185,15 +190,14 @@
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
@@ -265,17 +269,19 @@
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
@@ -320,14 +326,15 @@
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
@@ -365,19 +372,21 @@
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
@@ -413,26 +422,30 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "il-central-1",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/type_defs.py` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateTokenWithIAMRequestRequestTypeDef",
     "RegisterClientRequestRequestTypeDef",
     "StartDeviceAuthorizationRequestRequestTypeDef",
     "CreateTokenResponseTypeDef",
@@ -44,24 +43,25 @@
         "clientSecret": str,
         "grantType": str,
         "deviceCode": NotRequired[str],
         "code": NotRequired[str],
         "refreshToken": NotRequired[str],
         "scope": NotRequired[Sequence[str]],
         "redirectUri": NotRequired[str],
+        "codeVerifier": NotRequired[str],
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
 CreateTokenWithIAMRequestRequestTypeDef = TypedDict(
     "CreateTokenWithIAMRequestRequestTypeDef",
     {
         "clientId": str,
         "grantType": str,
@@ -69,22 +69,27 @@
         "refreshToken": NotRequired[str],
         "assertion": NotRequired[str],
         "scope": NotRequired[Sequence[str]],
         "redirectUri": NotRequired[str],
         "subjectToken": NotRequired[str],
         "subjectTokenType": NotRequired[str],
         "requestedTokenType": NotRequired[str],
+        "codeVerifier": NotRequired[str],
     },
 )
 RegisterClientRequestRequestTypeDef = TypedDict(
     "RegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
         "clientType": str,
         "scopes": NotRequired[Sequence[str]],
+        "redirectUris": NotRequired[Sequence[str]],
+        "grantTypes": NotRequired[Sequence[str]],
+        "issuerUrl": NotRequired[str],
+        "entitledApplicationArn": NotRequired[str],
     },
 )
 StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
     "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc/type_defs.pyi` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -43,24 +43,25 @@
         "clientSecret": str,
         "grantType": str,
         "deviceCode": NotRequired[str],
         "code": NotRequired[str],
         "refreshToken": NotRequired[str],
         "scope": NotRequired[Sequence[str]],
         "redirectUri": NotRequired[str],
+        "codeVerifier": NotRequired[str],
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
 CreateTokenWithIAMRequestRequestTypeDef = TypedDict(
     "CreateTokenWithIAMRequestRequestTypeDef",
     {
         "clientId": str,
         "grantType": str,
@@ -68,22 +69,27 @@
         "refreshToken": NotRequired[str],
         "assertion": NotRequired[str],
         "scope": NotRequired[Sequence[str]],
         "redirectUri": NotRequired[str],
         "subjectToken": NotRequired[str],
         "subjectTokenType": NotRequired[str],
         "requestedTokenType": NotRequired[str],
+        "codeVerifier": NotRequired[str],
     },
 )
 RegisterClientRequestRequestTypeDef = TypedDict(
     "RegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
         "clientType": str,
         "scopes": NotRequired[Sequence[str]],
+        "redirectUris": NotRequired[Sequence[str]],
+        "grantTypes": NotRequired[Sequence[str]],
+        "issuerUrl": NotRequired[str],
+        "entitledApplicationArn": NotRequired[str],
     },
 )
 StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
     "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/PKG-INFO` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-oidc
-Version: 1.34.0
-Summary: Type annotations for boto3.SSOOIDC 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.103
+Summary: Type annotations for boto3.SSOOIDC 1.34.103 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/
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
 
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-oidc)](https://pepy.tech/project/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.34.103](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-oidc-1.34.0/mypy_boto3_sso_oidc.egg-info/SOURCES.txt` & `mypy_boto3_sso_oidc-1.34.103/mypy_boto3_sso_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.34.0/setup.py` & `mypy_boto3_sso_oidc-1.34.103/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso-oidc",
-    version="1.34.0",
+    version="1.34.103",
     packages=["mypy_boto3_sso_oidc"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.SSOOIDC 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.SSOOIDC 1.34.103 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 sso-oidc type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sso_oidc": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

