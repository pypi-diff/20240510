# Comparing `tmp/mypy-boto3-route53resolver-1.34.3.tar.gz` & `tmp/mypy_boto3_route53resolver-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53resolver-1.34.3.tar", last modified: Mon Dec 18 23:08:35 2023, max compression
+gzip compressed data, was "mypy_boto3_route53resolver-1.34.95.tar", last modified: Tue Apr 30 19:34:54 2024, max compression
```

## Comparing `mypy-boto3-route53resolver-1.34.3.tar` & `mypy_boto3_route53resolver-1.34.95.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:08:35.262668 mypy-boto3-route53resolver-1.34.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15710 2023-12-18 23:08:35.262668 mypy-boto3-route53resolver-1.34.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14145 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:08:35.262668 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59505 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    59502 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14958 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14958 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20774 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20757 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    55923 2023-12-18 23:08:20.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55923 2023-12-18 23:08:20.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:08:35.262668 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15710 2023-12-18 23:08:35.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-18 23:08:35.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 23:08:35.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 23:08:35.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-18 23:08:35.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-18 23:08:35.000000 mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 23:08:35.262668 mypy-boto3-route53resolver-1.34.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-12-18 23:08:19.000000 mypy-boto3-route53resolver-1.34.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.307060 mypy_boto3_route53resolver-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-04-30 19:34:54.307060 mypy_boto3_route53resolver-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.307060 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59799 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59796 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-30 19:34:11.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-30 19:34:11.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-04-30 19:34:11.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56604 2024-04-30 19:34:13.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56604 2024-04-30 19:34:13.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.307060 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-04-30 19:34:54.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-30 19:34:54.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:54.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:54.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:54.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 19:34:54.000000 mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:54.307060 mypy_boto3_route53resolver-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-30 19:34:10.000000 mypy_boto3_route53resolver-1.34.95/setup.py
```

### Comparing `mypy-boto3-route53resolver-1.34.3/LICENSE` & `mypy_boto3_route53resolver-1.34.95/LICENSE`

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

### Comparing `mypy-boto3-route53resolver-1.34.3/PKG-INFO` & `mypy_boto3_route53resolver-1.34.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.34.3
-Summary: Type annotations for boto3.Route53Resolver 1.34.3 service generated with mypy-boto3-builder 7.22.0
+Version: 1.34.95
+Summary: Type annotations for boto3.Route53Resolver 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
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
 
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53resolver)](https://pepy.tech/project/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.34.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.22.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53resolver-1.34.3/README.md` & `mypy_boto3_route53resolver-1.34.95/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53resolver)](https://pepy.tech/project/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.34.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.22.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/__init__.py` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/__init__.pyi` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/__main__.py` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Resolver 1.34.3\nVersion:         1.34.3\nBuilder"
-        " version: 7.22.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Route53Resolver 1.34.95\n"
+        "Version:         1.34.95\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.3")
+    print("1.34.95")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/client.py` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionType,
     AutodefinedReverseFlagType,
     BlockResponseType,
+    FirewallDomainRedirectionActionType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     MutationProtectionStatusType,
     ProtocolType,
     ResolverEndpointDirectionType,
     ResolverEndpointTypeType,
@@ -187,15 +188,15 @@
         *,
         CreatorRequestId: str,
         FirewallRuleGroupId: str,
         VpcId: str,
         Priority: int,
         Name: str,
         MutationProtection: MutationProtectionStatusType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> AssociateFirewallRuleGroupResponseTypeDef:
         """
         Associates a  FirewallRuleGroup with a VPC, to provide DNS filtering for the
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_firewall_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#associate_firewall_rule_group)
@@ -265,15 +266,17 @@
         FirewallDomainListId: str,
         Priority: int,
         Action: ActionType,
         Name: str,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
-        BlockOverrideTtl: int = ...
+        BlockOverrideTtl: int = ...,
+        FirewallDomainRedirectionAction: FirewallDomainRedirectionActionType = ...,
+        Qtype: str = ...,
     ) -> CreateFirewallRuleResponseTypeDef:
         """
         Creates a single DNS Firewall rule in the specified rule group, using the
         specified domain
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule)
@@ -295,15 +298,15 @@
         self,
         *,
         CreatorRequestId: str,
         Name: str,
         PreferredInstanceType: str,
         OutpostArn: str,
         InstanceCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOutpostResolverResponseTypeDef:
         """
         Creates a Route 53 Resolver on an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_outpost_resolver)
         """
@@ -316,30 +319,30 @@
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         OutpostArn: str = ...,
         PreferredInstanceType: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
-        Protocols: Sequence[ProtocolType] = ...
+        Protocols: Sequence[ProtocolType] = ...,
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_resolver_endpoint)
         """
 
     def create_resolver_query_log_config(
         self,
         *,
         Name: str,
         DestinationArn: str,
         CreatorRequestId: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverQueryLogConfigResponseTypeDef:
         """
         Creates a Resolver query logging configuration, which defines where you want
         Resolver to save DNS query logs that originate in your
         VPCs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_query_log_config)
@@ -351,15 +354,15 @@
         *,
         CreatorRequestId: str,
         RuleType: RuleTypeOptionType,
         Name: str = ...,
         DomainName: str = ...,
         TargetIps: Sequence[TargetAddressTypeDef] = ...,
         ResolverEndpointId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverRuleResponseTypeDef:
         """
         For DNS queries that originate in your VPCs, specifies which Resolver endpoint
         the queries pass through, one domain name that you want to forward to your
         network, and the IP addresses of the DNS resolvers in your
         network.
 
@@ -374,15 +377,15 @@
         Deletes the specified domain list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_domain_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_firewall_domain_list)
         """
 
     def delete_firewall_rule(
-        self, *, FirewallRuleGroupId: str, FirewallDomainListId: str
+        self, *, FirewallRuleGroupId: str, FirewallDomainListId: str, Qtype: str = ...
     ) -> DeleteFirewallRuleResponseTypeDef:
         """
         Deletes the specified firewall rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_firewall_rule)
         """
@@ -696,15 +699,15 @@
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRuleGroupAssociationsResponseTypeDef:
         """
         Retrieves the firewall rule group associations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rule_group_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_firewall_rule_group_associations)
         """
@@ -723,15 +726,15 @@
     def list_firewall_rules(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRulesResponseTypeDef:
         """
         Retrieves the firewall rules that you have defined for the specified firewall
         rule
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
@@ -797,15 +800,15 @@
     def list_resolver_query_log_config_associations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigAssociationsResponseTypeDef:
         """
         Lists information about associations between Amazon VPCs and query logging
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_config_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_resolver_query_log_config_associations)
@@ -814,15 +817,15 @@
     def list_resolver_query_log_configs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigsResponseTypeDef:
         """
         Lists information about the specified query logging configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_resolver_query_log_configs)
         """
@@ -928,15 +931,15 @@
         """
 
     def update_firewall_domains(
         self,
         *,
         FirewallDomainListId: str,
         Operation: FirewallDomainUpdateOperationType,
-        Domains: Sequence[str]
+        Domains: Sequence[str],
     ) -> UpdateFirewallDomainsResponseTypeDef:
         """
         Updates the firewall domain list from an array of domain specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_domains)
         """
@@ -948,45 +951,47 @@
         FirewallDomainListId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
         BlockOverrideTtl: int = ...,
-        Name: str = ...
+        Name: str = ...,
+        FirewallDomainRedirectionAction: FirewallDomainRedirectionActionType = ...,
+        Qtype: str = ...,
     ) -> UpdateFirewallRuleResponseTypeDef:
         """
         Updates the specified firewall rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_rule)
         """
 
     def update_firewall_rule_group_association(
         self,
         *,
         FirewallRuleGroupAssociationId: str,
         Priority: int = ...,
         MutationProtection: MutationProtectionStatusType = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateFirewallRuleGroupAssociationResponseTypeDef:
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_rule_group_association)
         """
 
     def update_outpost_resolver(
         self,
         *,
         Id: str,
         Name: str = ...,
         InstanceCount: int = ...,
-        PreferredInstanceType: str = ...
+        PreferredInstanceType: str = ...,
     ) -> UpdateOutpostResolverResponseTypeDef:
         """
         You can use `UpdateOutpostResolver` to update the instance count, type, or name
         of a Resolver on an
         Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
@@ -1018,15 +1023,15 @@
     def update_resolver_endpoint(
         self,
         *,
         ResolverEndpointId: str,
         Name: str = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
         UpdateIpAddresses: Sequence[UpdateIpAddressTypeDef] = ...,
-        Protocols: Sequence[ProtocolType] = ...
+        Protocols: Sequence[ProtocolType] = ...,
     ) -> UpdateResolverEndpointResponseTypeDef:
         """
         Updates the name, or endpoint type for an inbound or an outbound Resolver
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_resolver_endpoint)
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/client.pyi` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionType,
     AutodefinedReverseFlagType,
     BlockResponseType,
+    FirewallDomainRedirectionActionType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     MutationProtectionStatusType,
     ProtocolType,
     ResolverEndpointDirectionType,
     ResolverEndpointTypeType,
@@ -184,15 +185,15 @@
         *,
         CreatorRequestId: str,
         FirewallRuleGroupId: str,
         VpcId: str,
         Priority: int,
         Name: str,
         MutationProtection: MutationProtectionStatusType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> AssociateFirewallRuleGroupResponseTypeDef:
         """
         Associates a  FirewallRuleGroup with a VPC, to provide DNS filtering for the
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.associate_firewall_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#associate_firewall_rule_group)
@@ -262,15 +263,17 @@
         FirewallDomainListId: str,
         Priority: int,
         Action: ActionType,
         Name: str,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
-        BlockOverrideTtl: int = ...
+        BlockOverrideTtl: int = ...,
+        FirewallDomainRedirectionAction: FirewallDomainRedirectionActionType = ...,
+        Qtype: str = ...,
     ) -> CreateFirewallRuleResponseTypeDef:
         """
         Creates a single DNS Firewall rule in the specified rule group, using the
         specified domain
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule)
@@ -292,15 +295,15 @@
         self,
         *,
         CreatorRequestId: str,
         Name: str,
         PreferredInstanceType: str,
         OutpostArn: str,
         InstanceCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOutpostResolverResponseTypeDef:
         """
         Creates a Route 53 Resolver on an Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_outpost_resolver)
         """
@@ -313,30 +316,30 @@
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         OutpostArn: str = ...,
         PreferredInstanceType: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
-        Protocols: Sequence[ProtocolType] = ...
+        Protocols: Sequence[ProtocolType] = ...,
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_resolver_endpoint)
         """
 
     def create_resolver_query_log_config(
         self,
         *,
         Name: str,
         DestinationArn: str,
         CreatorRequestId: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverQueryLogConfigResponseTypeDef:
         """
         Creates a Resolver query logging configuration, which defines where you want
         Resolver to save DNS query logs that originate in your
         VPCs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_query_log_config)
@@ -348,15 +351,15 @@
         *,
         CreatorRequestId: str,
         RuleType: RuleTypeOptionType,
         Name: str = ...,
         DomainName: str = ...,
         TargetIps: Sequence[TargetAddressTypeDef] = ...,
         ResolverEndpointId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateResolverRuleResponseTypeDef:
         """
         For DNS queries that originate in your VPCs, specifies which Resolver endpoint
         the queries pass through, one domain name that you want to forward to your
         network, and the IP addresses of the DNS resolvers in your
         network.
 
@@ -371,15 +374,15 @@
         Deletes the specified domain list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_domain_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_firewall_domain_list)
         """
 
     def delete_firewall_rule(
-        self, *, FirewallRuleGroupId: str, FirewallDomainListId: str
+        self, *, FirewallRuleGroupId: str, FirewallDomainListId: str, Qtype: str = ...
     ) -> DeleteFirewallRuleResponseTypeDef:
         """
         Deletes the specified firewall rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_firewall_rule)
         """
@@ -693,15 +696,15 @@
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRuleGroupAssociationsResponseTypeDef:
         """
         Retrieves the firewall rule group associations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rule_group_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_firewall_rule_group_associations)
         """
@@ -720,15 +723,15 @@
     def list_firewall_rules(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFirewallRulesResponseTypeDef:
         """
         Retrieves the firewall rules that you have defined for the specified firewall
         rule
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
@@ -794,15 +797,15 @@
     def list_resolver_query_log_config_associations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigAssociationsResponseTypeDef:
         """
         Lists information about associations between Amazon VPCs and query logging
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_config_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_resolver_query_log_config_associations)
@@ -811,15 +814,15 @@
     def list_resolver_query_log_configs(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListResolverQueryLogConfigsResponseTypeDef:
         """
         Lists information about the specified query logging configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_query_log_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_resolver_query_log_configs)
         """
@@ -925,15 +928,15 @@
         """
 
     def update_firewall_domains(
         self,
         *,
         FirewallDomainListId: str,
         Operation: FirewallDomainUpdateOperationType,
-        Domains: Sequence[str]
+        Domains: Sequence[str],
     ) -> UpdateFirewallDomainsResponseTypeDef:
         """
         Updates the firewall domain list from an array of domain specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_domains)
         """
@@ -945,45 +948,47 @@
         FirewallDomainListId: str,
         Priority: int = ...,
         Action: ActionType = ...,
         BlockResponse: BlockResponseType = ...,
         BlockOverrideDomain: str = ...,
         BlockOverrideDnsType: Literal["CNAME"] = ...,
         BlockOverrideTtl: int = ...,
-        Name: str = ...
+        Name: str = ...,
+        FirewallDomainRedirectionAction: FirewallDomainRedirectionActionType = ...,
+        Qtype: str = ...,
     ) -> UpdateFirewallRuleResponseTypeDef:
         """
         Updates the specified firewall rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_rule)
         """
 
     def update_firewall_rule_group_association(
         self,
         *,
         FirewallRuleGroupAssociationId: str,
         Priority: int = ...,
         MutationProtection: MutationProtectionStatusType = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateFirewallRuleGroupAssociationResponseTypeDef:
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_rule_group_association)
         """
 
     def update_outpost_resolver(
         self,
         *,
         Id: str,
         Name: str = ...,
         InstanceCount: int = ...,
-        PreferredInstanceType: str = ...
+        PreferredInstanceType: str = ...,
     ) -> UpdateOutpostResolverResponseTypeDef:
         """
         You can use `UpdateOutpostResolver` to update the instance count, type, or name
         of a Resolver on an
         Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
@@ -1015,15 +1020,15 @@
     def update_resolver_endpoint(
         self,
         *,
         ResolverEndpointId: str,
         Name: str = ...,
         ResolverEndpointType: ResolverEndpointTypeType = ...,
         UpdateIpAddresses: Sequence[UpdateIpAddressTypeDef] = ...,
-        Protocols: Sequence[ProtocolType] = ...
+        Protocols: Sequence[ProtocolType] = ...,
     ) -> UpdateResolverEndpointResponseTypeDef:
         """
         Updates the name, or endpoint type for an inbound or an outbound Resolver
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_resolver_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_resolver_endpoint)
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/literals.py` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = (
     "ActionType",
     "AutodefinedReverseFlagType",
     "BlockOverrideDnsTypeType",
     "BlockResponseType",
     "FirewallDomainImportOperationType",
     "FirewallDomainListStatusType",
+    "FirewallDomainRedirectionActionType",
     "FirewallDomainUpdateOperationType",
     "FirewallFailOpenStatusType",
     "FirewallRuleGroupAssociationStatusType",
     "FirewallRuleGroupStatusType",
     "IpAddressStatusType",
     "ListFirewallConfigsPaginatorName",
     "ListFirewallDomainListsPaginatorName",
@@ -75,14 +76,17 @@
 AutodefinedReverseFlagType = Literal["DISABLE", "ENABLE", "USE_LOCAL_RESOURCE_SETTING"]
 BlockOverrideDnsTypeType = Literal["CNAME"]
 BlockResponseType = Literal["NODATA", "NXDOMAIN", "OVERRIDE"]
 FirewallDomainImportOperationType = Literal["REPLACE"]
 FirewallDomainListStatusType = Literal[
     "COMPLETE", "COMPLETE_IMPORT_FAILED", "DELETING", "IMPORTING", "UPDATING"
 ]
+FirewallDomainRedirectionActionType = Literal[
+    "INSPECT_REDIRECTION_DOMAIN", "TRUST_REDIRECTION_DOMAIN"
+]
 FirewallDomainUpdateOperationType = Literal["ADD", "REMOVE", "REPLACE"]
 FirewallFailOpenStatusType = Literal["DISABLED", "ENABLED", "USE_LOCAL_RESOURCE_SETTING"]
 FirewallRuleGroupAssociationStatusType = Literal["COMPLETE", "DELETING", "UPDATING"]
 FirewallRuleGroupStatusType = Literal["COMPLETE", "DELETING", "UPDATING"]
 IpAddressStatusType = Literal[
     "ATTACHED",
     "ATTACHING",
@@ -185,14 +189,15 @@
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
@@ -203,14 +208,15 @@
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
@@ -228,14 +234,15 @@
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
@@ -248,24 +255,26 @@
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
@@ -326,15 +335,14 @@
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
@@ -410,14 +418,15 @@
     "mturk",
     "mwaa",
     "neptune",
     "neptune-graph",
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
@@ -462,14 +471,15 @@
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
@@ -507,19 +517,21 @@
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
@@ -579,14 +591,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/literals.pyi` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = (
     "ActionType",
     "AutodefinedReverseFlagType",
     "BlockOverrideDnsTypeType",
     "BlockResponseType",
     "FirewallDomainImportOperationType",
     "FirewallDomainListStatusType",
+    "FirewallDomainRedirectionActionType",
     "FirewallDomainUpdateOperationType",
     "FirewallFailOpenStatusType",
     "FirewallRuleGroupAssociationStatusType",
     "FirewallRuleGroupStatusType",
     "IpAddressStatusType",
     "ListFirewallConfigsPaginatorName",
     "ListFirewallDomainListsPaginatorName",
@@ -75,14 +76,17 @@
 AutodefinedReverseFlagType = Literal["DISABLE", "ENABLE", "USE_LOCAL_RESOURCE_SETTING"]
 BlockOverrideDnsTypeType = Literal["CNAME"]
 BlockResponseType = Literal["NODATA", "NXDOMAIN", "OVERRIDE"]
 FirewallDomainImportOperationType = Literal["REPLACE"]
 FirewallDomainListStatusType = Literal[
     "COMPLETE", "COMPLETE_IMPORT_FAILED", "DELETING", "IMPORTING", "UPDATING"
 ]
+FirewallDomainRedirectionActionType = Literal[
+    "INSPECT_REDIRECTION_DOMAIN", "TRUST_REDIRECTION_DOMAIN"
+]
 FirewallDomainUpdateOperationType = Literal["ADD", "REMOVE", "REPLACE"]
 FirewallFailOpenStatusType = Literal["DISABLED", "ENABLED", "USE_LOCAL_RESOURCE_SETTING"]
 FirewallRuleGroupAssociationStatusType = Literal["COMPLETE", "DELETING", "UPDATING"]
 FirewallRuleGroupStatusType = Literal["COMPLETE", "DELETING", "UPDATING"]
 IpAddressStatusType = Literal[
     "ATTACHED",
     "ATTACHING",
@@ -185,14 +189,15 @@
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
@@ -203,14 +208,15 @@
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
@@ -228,14 +234,15 @@
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
@@ -248,24 +255,26 @@
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
@@ -326,15 +335,14 @@
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
@@ -410,14 +418,15 @@
     "mturk",
     "mwaa",
     "neptune",
     "neptune-graph",
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
@@ -462,14 +471,15 @@
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
@@ -507,19 +517,21 @@
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
@@ -579,14 +591,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/paginator.py` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 
@@ -194,15 +194,15 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 
@@ -242,15 +242,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 
@@ -275,15 +275,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 
@@ -295,15 +295,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 
@@ -315,15 +315,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 
@@ -333,15 +333,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 
@@ -351,15 +351,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
         """
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/paginator.pyi` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 class ListFirewallRuleGroupsPaginator(Paginator):
@@ -187,15 +187,15 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 class ListOutpostResolversPaginator(Paginator):
@@ -232,15 +232,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 class ListResolverEndpointIpAddressesPaginator(Paginator):
@@ -263,15 +263,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 class ListResolverQueryLogConfigAssociationsPaginator(Paginator):
@@ -282,15 +282,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 class ListResolverQueryLogConfigsPaginator(Paginator):
@@ -301,15 +301,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 class ListResolverRuleAssociationsPaginator(Paginator):
@@ -318,15 +318,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 class ListResolverRulesPaginator(Paginator):
@@ -335,15 +335,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/type_defs.py` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Dict, List, Sequence
 
 from .literals import (
     ActionType,
     AutodefinedReverseFlagType,
     BlockResponseType,
     FirewallDomainListStatusType,
+    FirewallDomainRedirectionActionType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     FirewallRuleGroupStatusType,
     IpAddressStatusType,
     MutationProtectionStatusType,
     OutpostResolverStatusType,
@@ -260,18 +261,18 @@
         "ModificationTime": NotRequired[str],
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
 IpAddressUpdateTypeDef = TypedDict(
     "IpAddressUpdateTypeDef",
     {
         "IpId": NotRequired[str],
         "SubnetId": NotRequired[str],
@@ -378,14 +379,16 @@
         "Priority": int,
         "Action": ActionType,
         "Name": str,
         "BlockResponse": NotRequired[BlockResponseType],
         "BlockOverrideDomain": NotRequired[str],
         "BlockOverrideDnsType": NotRequired[Literal["CNAME"]],
         "BlockOverrideTtl": NotRequired[int],
+        "FirewallDomainRedirectionAction": NotRequired[FirewallDomainRedirectionActionType],
+        "Qtype": NotRequired[str],
     },
 )
 FirewallRuleTypeDef = TypedDict(
     "FirewallRuleTypeDef",
     {
         "FirewallRuleGroupId": NotRequired[str],
         "FirewallDomainListId": NotRequired[str],
@@ -395,14 +398,16 @@
         "BlockResponse": NotRequired[BlockResponseType],
         "BlockOverrideDomain": NotRequired[str],
         "BlockOverrideDnsType": NotRequired[Literal["CNAME"]],
         "BlockOverrideTtl": NotRequired[int],
         "CreatorRequestId": NotRequired[str],
         "CreationTime": NotRequired[str],
         "ModificationTime": NotRequired[str],
+        "FirewallDomainRedirectionAction": NotRequired[FirewallDomainRedirectionActionType],
+        "Qtype": NotRequired[str],
     },
 )
 OutpostResolverTypeDef = TypedDict(
     "OutpostResolverTypeDef",
     {
         "Arn": NotRequired[str],
         "CreationTime": NotRequired[str],
@@ -462,14 +467,15 @@
     },
 )
 DeleteFirewallRuleRequestRequestTypeDef = TypedDict(
     "DeleteFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
+        "Qtype": NotRequired[str],
     },
 )
 DeleteOutpostResolverRequestRequestTypeDef = TypedDict(
     "DeleteOutpostResolverRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -827,14 +833,16 @@
         "Priority": NotRequired[int],
         "Action": NotRequired[ActionType],
         "BlockResponse": NotRequired[BlockResponseType],
         "BlockOverrideDomain": NotRequired[str],
         "BlockOverrideDnsType": NotRequired[Literal["CNAME"]],
         "BlockOverrideTtl": NotRequired[int],
         "Name": NotRequired[str],
+        "FirewallDomainRedirectionAction": NotRequired[FirewallDomainRedirectionActionType],
+        "Qtype": NotRequired[str],
     },
 )
 UpdateIpAddressTypeDef = TypedDict(
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
@@ -969,33 +977,33 @@
         "StatusMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallDomainsResponseTypeDef = TypedDict(
     "ListFirewallDomainsResponseTypeDef",
     {
-        "NextToken": str,
         "Domains": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFirewallRuleGroupAssociationsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallRuleGroupAssociations": List[FirewallRuleGroupAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
     "PutFirewallRuleGroupPolicyResponseTypeDef",
     {
         "ReturnValue": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1080,18 +1088,18 @@
         "ResolverEndpoint": ResolverEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverEndpointsResponseTypeDef = TypedDict(
     "ListResolverEndpointsResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "ResolverEndpoints": List[ResolverEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverEndpointResponseTypeDef = TypedDict(
     "UpdateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1117,19 +1125,19 @@
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverQueryLogConfigAssociationsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsResponseTypeDef",
     {
-        "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigAssociations": List[ResolverQueryLogConfigAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateResolverRuleResponseTypeDef = TypedDict(
     "AssociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1148,18 +1156,18 @@
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverRuleAssociationsResponseTypeDef = TypedDict(
     "ListResolverRuleAssociationsResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "ResolverRuleAssociations": List[ResolverRuleAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateFirewallDomainListResponseTypeDef = TypedDict(
     "CreateFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1213,17 +1221,17 @@
         "FirewallRule": FirewallRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallRulesResponseTypeDef = TypedDict(
     "ListFirewallRulesResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallRules": List[FirewallRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateFirewallRuleResponseTypeDef = TypedDict(
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1250,16 +1258,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListOutpostResolversResponseTypeDef = TypedDict(
     "ListOutpostResolversResponseTypeDef",
     {
         "OutpostResolvers": List[OutpostResolverTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateOutpostResolverResponseTypeDef = TypedDict(
     "UpdateOutpostResolverResponseTypeDef",
     {
         "OutpostResolver": OutpostResolverTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1300,19 +1308,19 @@
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverQueryLogConfigsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigs": List[ResolverQueryLogConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateResolverRuleRequestRequestTypeDef = TypedDict(
     "CreateResolverRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "RuleType": RuleTypeOptionType,
@@ -1408,55 +1416,55 @@
         "FirewallConfig": FirewallConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallConfigsResponseTypeDef = TypedDict(
     "ListFirewallConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallConfigs": List[FirewallConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateFirewallConfigResponseTypeDef = TypedDict(
     "UpdateFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallDomainListsResponseTypeDef = TypedDict(
     "ListFirewallDomainListsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallDomainLists": List[FirewallDomainListMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFirewallRuleGroupsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallRuleGroups": List[FirewallRuleGroupMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetResolverConfigResponseTypeDef = TypedDict(
     "GetResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverConfigsResponseTypeDef = TypedDict(
     "ListResolverConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "ResolverConfigs": List[ResolverConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverConfigResponseTypeDef = TypedDict(
     "UpdateResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1468,33 +1476,33 @@
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverDnssecConfigsResponseTypeDef = TypedDict(
     "ListResolverDnssecConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "ResolverDnssecConfigs": List[ResolverDnssecConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverDnssecConfigResponseTypeDef = TypedDict(
     "UpdateResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverEndpointIpAddressesResponseTypeDef = TypedDict(
     "ListResolverEndpointIpAddressesResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "IpAddresses": List[IpAddressResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
     "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
@@ -1649,18 +1657,18 @@
         "ResolverRule": ResolverRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverRulesResponseTypeDef = TypedDict(
     "ListResolverRulesResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "ResolverRules": List[ResolverRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverRuleResponseTypeDef = TypedDict(
     "UpdateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver/type_defs.pyi` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Dict, List, Sequence
 
 from .literals import (
     ActionType,
     AutodefinedReverseFlagType,
     BlockResponseType,
     FirewallDomainListStatusType,
+    FirewallDomainRedirectionActionType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     FirewallRuleGroupStatusType,
     IpAddressStatusType,
     MutationProtectionStatusType,
     OutpostResolverStatusType,
@@ -260,18 +261,18 @@
         "ModificationTime": NotRequired[str],
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
 IpAddressUpdateTypeDef = TypedDict(
     "IpAddressUpdateTypeDef",
     {
         "IpId": NotRequired[str],
         "SubnetId": NotRequired[str],
@@ -378,14 +379,16 @@
         "Priority": int,
         "Action": ActionType,
         "Name": str,
         "BlockResponse": NotRequired[BlockResponseType],
         "BlockOverrideDomain": NotRequired[str],
         "BlockOverrideDnsType": NotRequired[Literal["CNAME"]],
         "BlockOverrideTtl": NotRequired[int],
+        "FirewallDomainRedirectionAction": NotRequired[FirewallDomainRedirectionActionType],
+        "Qtype": NotRequired[str],
     },
 )
 FirewallRuleTypeDef = TypedDict(
     "FirewallRuleTypeDef",
     {
         "FirewallRuleGroupId": NotRequired[str],
         "FirewallDomainListId": NotRequired[str],
@@ -395,14 +398,16 @@
         "BlockResponse": NotRequired[BlockResponseType],
         "BlockOverrideDomain": NotRequired[str],
         "BlockOverrideDnsType": NotRequired[Literal["CNAME"]],
         "BlockOverrideTtl": NotRequired[int],
         "CreatorRequestId": NotRequired[str],
         "CreationTime": NotRequired[str],
         "ModificationTime": NotRequired[str],
+        "FirewallDomainRedirectionAction": NotRequired[FirewallDomainRedirectionActionType],
+        "Qtype": NotRequired[str],
     },
 )
 OutpostResolverTypeDef = TypedDict(
     "OutpostResolverTypeDef",
     {
         "Arn": NotRequired[str],
         "CreationTime": NotRequired[str],
@@ -462,14 +467,15 @@
     },
 )
 DeleteFirewallRuleRequestRequestTypeDef = TypedDict(
     "DeleteFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
+        "Qtype": NotRequired[str],
     },
 )
 DeleteOutpostResolverRequestRequestTypeDef = TypedDict(
     "DeleteOutpostResolverRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -827,14 +833,16 @@
         "Priority": NotRequired[int],
         "Action": NotRequired[ActionType],
         "BlockResponse": NotRequired[BlockResponseType],
         "BlockOverrideDomain": NotRequired[str],
         "BlockOverrideDnsType": NotRequired[Literal["CNAME"]],
         "BlockOverrideTtl": NotRequired[int],
         "Name": NotRequired[str],
+        "FirewallDomainRedirectionAction": NotRequired[FirewallDomainRedirectionActionType],
+        "Qtype": NotRequired[str],
     },
 )
 UpdateIpAddressTypeDef = TypedDict(
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
@@ -969,33 +977,33 @@
         "StatusMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallDomainsResponseTypeDef = TypedDict(
     "ListFirewallDomainsResponseTypeDef",
     {
-        "NextToken": str,
         "Domains": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFirewallRuleGroupAssociationsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallRuleGroupAssociations": List[FirewallRuleGroupAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
     "PutFirewallRuleGroupPolicyResponseTypeDef",
     {
         "ReturnValue": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1080,18 +1088,18 @@
         "ResolverEndpoint": ResolverEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverEndpointsResponseTypeDef = TypedDict(
     "ListResolverEndpointsResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "ResolverEndpoints": List[ResolverEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverEndpointResponseTypeDef = TypedDict(
     "UpdateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1117,19 +1125,19 @@
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverQueryLogConfigAssociationsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsResponseTypeDef",
     {
-        "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigAssociations": List[ResolverQueryLogConfigAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateResolverRuleResponseTypeDef = TypedDict(
     "AssociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1148,18 +1156,18 @@
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverRuleAssociationsResponseTypeDef = TypedDict(
     "ListResolverRuleAssociationsResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "ResolverRuleAssociations": List[ResolverRuleAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateFirewallDomainListResponseTypeDef = TypedDict(
     "CreateFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1213,17 +1221,17 @@
         "FirewallRule": FirewallRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallRulesResponseTypeDef = TypedDict(
     "ListFirewallRulesResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallRules": List[FirewallRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateFirewallRuleResponseTypeDef = TypedDict(
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1250,16 +1258,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListOutpostResolversResponseTypeDef = TypedDict(
     "ListOutpostResolversResponseTypeDef",
     {
         "OutpostResolvers": List[OutpostResolverTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateOutpostResolverResponseTypeDef = TypedDict(
     "UpdateOutpostResolverResponseTypeDef",
     {
         "OutpostResolver": OutpostResolverTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1300,19 +1308,19 @@
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverQueryLogConfigsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigs": List[ResolverQueryLogConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateResolverRuleRequestRequestTypeDef = TypedDict(
     "CreateResolverRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "RuleType": RuleTypeOptionType,
@@ -1408,55 +1416,55 @@
         "FirewallConfig": FirewallConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallConfigsResponseTypeDef = TypedDict(
     "ListFirewallConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallConfigs": List[FirewallConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateFirewallConfigResponseTypeDef = TypedDict(
     "UpdateFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListFirewallDomainListsResponseTypeDef = TypedDict(
     "ListFirewallDomainListsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallDomainLists": List[FirewallDomainListMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFirewallRuleGroupsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupsResponseTypeDef",
     {
-        "NextToken": str,
         "FirewallRuleGroups": List[FirewallRuleGroupMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetResolverConfigResponseTypeDef = TypedDict(
     "GetResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverConfigsResponseTypeDef = TypedDict(
     "ListResolverConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "ResolverConfigs": List[ResolverConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverConfigResponseTypeDef = TypedDict(
     "UpdateResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1468,33 +1476,33 @@
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverDnssecConfigsResponseTypeDef = TypedDict(
     "ListResolverDnssecConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "ResolverDnssecConfigs": List[ResolverDnssecConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverDnssecConfigResponseTypeDef = TypedDict(
     "UpdateResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverEndpointIpAddressesResponseTypeDef = TypedDict(
     "ListResolverEndpointIpAddressesResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "IpAddresses": List[IpAddressResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
     "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
@@ -1649,18 +1657,18 @@
         "ResolverRule": ResolverRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListResolverRulesResponseTypeDef = TypedDict(
     "ListResolverRulesResponseTypeDef",
     {
-        "NextToken": str,
         "MaxResults": int,
         "ResolverRules": List[ResolverRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateResolverRuleResponseTypeDef = TypedDict(
     "UpdateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/PKG-INFO` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.34.3
-Summary: Type annotations for boto3.Route53Resolver 1.34.3 service generated with mypy-boto3-builder 7.22.0
+Version: 1.34.95
+Summary: Type annotations for boto3.Route53Resolver 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
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
 
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53resolver)](https://pepy.tech/project/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.34.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.22.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53resolver-1.34.3/mypy_boto3_route53resolver.egg-info/SOURCES.txt` & `mypy_boto3_route53resolver-1.34.95/mypy_boto3_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.34.3/setup.py` & `mypy_boto3_route53resolver-1.34.95/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53resolver",
-    version="1.34.3",
+    version="1.34.95",
     packages=["mypy_boto3_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Route53Resolver 1.34.3 service generated with"
-        " mypy-boto3-builder 7.22.0"
-    ),
+    description="Type annotations for boto3.Route53Resolver 1.34.95 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 route53resolver type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_route53resolver": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

