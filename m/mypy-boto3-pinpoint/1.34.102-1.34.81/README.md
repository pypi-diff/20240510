# Comparing `tmp/mypy_boto3_pinpoint-1.34.102.tar.gz` & `tmp/mypy-boto3-pinpoint-1.34.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_pinpoint-1.34.102.tar", last modified: Fri May 10 03:08:08 2024, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.34.81.tar", last modified: Tue Apr  9 19:32:46 2024, max compression
```

## Comparing `mypy_boto3_pinpoint-1.34.102.tar` & `mypy-boto3-pinpoint-1.34.81.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:08:08.792460 mypy_boto3_pinpoint-1.34.102/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-05-10 03:08:08.792460 mypy_boto3_pinpoint-1.34.102/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:08:08.792460 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80226 2024-05-10 03:07:50.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    80223 2024-05-10 03:07:50.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-05-10 03:07:50.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-05-10 03:07:50.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   150353 2024-05-10 03:07:53.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   150353 2024-05-10 03:07:52.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:08:08.792460 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-05-10 03:08:08.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-10 03:08:08.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 03:08:08.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 03:08:08.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 03:08:08.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 03:08:08.000000 mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 03:08:08.792460 mypy_boto3_pinpoint-1.34.102/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-10 03:07:49.000000 mypy_boto3_pinpoint-1.34.102/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80216 2024-04-09 19:32:21.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80213 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-09 19:32:21.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-09 19:32:21.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   139262 2024-04-09 19:32:24.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139262 2024-04-09 19:32:23.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/setup.py
```

### Comparing `mypy_boto3_pinpoint-1.34.102/LICENSE` & `mypy-boto3-pinpoint-1.34.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_pinpoint-1.34.102/PKG-INFO` & `mypy-boto3-pinpoint-1.34.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.34.102
-Summary: Type annotations for boto3.Pinpoint 1.34.102 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.81
+Summary: Type annotations for boto3.Pinpoint 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.34.102](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_pinpoint-1.34.102/README.md` & `mypy-boto3-pinpoint-1.34.81/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.34.102](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.34.102\n"
-        "Version:         1.34.102\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.Pinpoint 1.34.81\n"
+        "Version:         1.34.81\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.102")
+    print("1.34.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
-    TagsModelUnionTypeDef,
+    TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
     TimestampTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
@@ -1308,15 +1308,15 @@
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_users_messages)
         """
 
     def tag_resource(
-        self, *, ResourceArn: str, TagsModel: TagsModelUnionTypeDef
+        self, *, ResourceArn: str, TagsModel: TagsModelTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or
         segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
-    TagsModelUnionTypeDef,
+    TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
     TimestampTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
@@ -1305,15 +1305,15 @@
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_users_messages)
         """
 
     def tag_resource(
-        self, *, ResourceArn: str, TagsModel: TagsModelUnionTypeDef
+        self, *, ResourceArn: str, TagsModel: TagsModelTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or
         segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,40 +78,39 @@
     "AddressConfigurationTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
     "JourneyTimeframeCapTypeDef",
     "CampaignHookTypeDef",
     "CampaignLimitsTypeDef",
     "QuietTimeTypeDef",
-    "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
     "BlobTypeDef",
     "CampaignCustomMessageTypeDef",
-    "MessageHeaderTypeDef",
+    "CampaignEmailMessageTypeDef",
     "CampaignStateTypeDef",
-    "CustomDeliveryConfigurationOutputTypeDef",
+    "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
-    "CustomDeliveryConfigurationTypeDef",
     "JourneyCustomMessageTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
@@ -143,23 +142,22 @@
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
+    "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
-    "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
-    "SetDimensionOutputTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
@@ -217,21 +215,20 @@
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
     "InAppMessageBodyConfigTypeDef",
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
     "JourneyPushMessageTypeDef",
-    "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagsModelOutputTypeDef",
+    "TagsModelTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
@@ -242,15 +239,14 @@
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
-    "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
@@ -263,20 +259,15 @@
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
     "ApplicationSettingsJourneyLimitsTypeDef",
     "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
     "RawEmailTypeDef",
-    "CampaignEmailMessageOutputTypeDef",
-    "CampaignEmailMessageTypeDef",
-    "EmailTemplateRequestTypeDef",
-    "EmailTemplateResponseTypeDef",
     "ChannelsResponseTypeDef",
-    "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
     "DeleteApnsChannelResponseTypeDef",
     "DeleteApnsSandboxChannelResponseTypeDef",
@@ -295,14 +286,16 @@
     "RemoveAttributesResponseTypeDef",
     "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "UpdateBaiduChannelResponseTypeDef",
+    "CreateEmailTemplateRequestRequestTypeDef",
+    "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "CreateInAppTemplateResponseTypeDef",
@@ -312,15 +305,14 @@
     "GetRecommenderConfigurationResponseTypeDef",
     "ListRecommenderConfigurationsResponseTypeDef",
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
-    "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
     "PushNotificationTemplateRequestTypeDef",
     "PushNotificationTemplateResponseTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
@@ -346,21 +338,20 @@
     "GetSmsChannelResponseTypeDef",
     "UpdateSmsChannelResponseTypeDef",
     "DeleteVoiceChannelResponseTypeDef",
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
     "EmailMessageActivityTypeDef",
+    "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
+    "EndpointResponseTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
-    "EndpointResponseTypeDef",
-    "EventDimensionsOutputTypeDef",
-    "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
@@ -377,68 +368,58 @@
     "ImportJobResponseTypeDef",
     "InAppMessageButtonTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
-    "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
-    "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "TagsModelUnionTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
-    "CreateEmailTemplateRequestRequestTypeDef",
-    "UpdateEmailTemplateRequestRequestTypeDef",
-    "GetEmailTemplateResponseTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
     "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
-    "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
-    "CampaignEventFilterOutputTypeDef",
-    "EventConditionOutputTypeDef",
-    "EventFilterOutputTypeDef",
+    "SendUsersMessagesResponseTypeDef",
     "CampaignEventFilterTypeDef",
     "EventConditionTypeDef",
     "EventFilterTypeDef",
     "EventsResponseTypeDef",
     "EventsBatchTypeDef",
     "CreateExportJobResponseTypeDef",
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
-    "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
@@ -450,80 +431,66 @@
     "GetApplicationSettingsResponseTypeDef",
     "UpdateApplicationSettingsResponseTypeDef",
     "UpdateApplicationSettingsRequestRequestTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
-    "ScheduleOutputTypeDef",
-    "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
     "EventStartConditionTypeDef",
     "PutEventsResponseTypeDef",
     "EventsRequestTypeDef",
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
-    "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
-    "CampaignInAppMessageOutputTypeDef",
     "CampaignInAppMessageTypeDef",
     "InAppMessageTypeDef",
     "InAppTemplateRequestTypeDef",
     "InAppTemplateResponseTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
-    "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
-    "SegmentGroupOutputTypeDef",
-    "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
-    "MessageConfigurationOutputTypeDef",
     "MessageConfigurationTypeDef",
     "InAppMessageCampaignTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
     "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
-    "SegmentGroupListOutputTypeDef",
-    "ConditionOutputTypeDef",
-    "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
     "WriteTreatmentResourceTypeDef",
     "InAppMessagesResponseTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
-    "ConditionalSplitActivityOutputTypeDef",
-    "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
     "WriteCampaignRequestTypeDef",
     "GetInAppMessagesResponseTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
-    "ActivityOutputTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "UpdateSegmentRequestRequestTypeDef",
     "ActivityTypeDef",
     "CampaignsResponseTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignResponseTypeDef",
     "GetCampaignResponseTypeDef",
@@ -842,21 +809,14 @@
 QuietTimeTypeDef = TypedDict(
     "QuietTimeTypeDef",
     {
         "End": NotRequired[str],
         "Start": NotRequired[str],
     },
 )
-AttributeDimensionOutputTypeDef = TypedDict(
-    "AttributeDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-        "AttributeType": NotRequired[AttributeTypeType],
-    },
-)
 AttributeDimensionTypeDef = TypedDict(
     "AttributeDimensionTypeDef",
     {
         "Values": Sequence[str],
         "AttributeType": NotRequired[AttributeTypeType],
     },
 )
@@ -914,32 +874,34 @@
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": NotRequired[str],
     },
 )
-MessageHeaderTypeDef = TypedDict(
-    "MessageHeaderTypeDef",
+CampaignEmailMessageTypeDef = TypedDict(
+    "CampaignEmailMessageTypeDef",
     {
-        "Name": NotRequired[str],
-        "Value": NotRequired[str],
+        "Body": NotRequired[str],
+        "FromAddress": NotRequired[str],
+        "HtmlBody": NotRequired[str],
+        "Title": NotRequired[str],
     },
 )
 CampaignStateTypeDef = TypedDict(
     "CampaignStateTypeDef",
     {
         "CampaignStatus": NotRequired[CampaignStatusType],
     },
 )
-CustomDeliveryConfigurationOutputTypeDef = TypedDict(
-    "CustomDeliveryConfigurationOutputTypeDef",
+CustomDeliveryConfigurationTypeDef = TypedDict(
+    "CustomDeliveryConfigurationTypeDef",
     {
         "DeliveryUri": str,
-        "EndpointTypes": NotRequired[List[EndpointTypesElementType]],
+        "EndpointTypes": NotRequired[Sequence[EndpointTypesElementType]],
     },
 )
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": NotRequired[str],
         "MessageType": NotRequired[MessageTypeType],
@@ -991,14 +953,26 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
+EmailTemplateRequestTypeDef = TypedDict(
+    "EmailTemplateRequestTypeDef",
+    {
+        "DefaultSubstitutions": NotRequired[str],
+        "HtmlPart": NotRequired[str],
+        "RecommenderId": NotRequired[str],
+        "Subject": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+        "TemplateDescription": NotRequired[str],
+        "TextPart": NotRequired[str],
+    },
+)
 CreateTemplateMessageBodyTypeDef = TypedDict(
     "CreateTemplateMessageBodyTypeDef",
     {
         "Arn": NotRequired[str],
         "Message": NotRequired[str],
         "RequestID": NotRequired[str],
     },
@@ -1081,21 +1055,14 @@
         "DefaultSubstitutions": NotRequired[str],
         "LanguageCode": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
         "TemplateDescription": NotRequired[str],
         "VoiceId": NotRequired[str],
     },
 )
-CustomDeliveryConfigurationTypeDef = TypedDict(
-    "CustomDeliveryConfigurationTypeDef",
-    {
-        "DeliveryUri": str,
-        "EndpointTypes": NotRequired[Sequence[EndpointTypesElementType]],
-    },
-)
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": NotRequired[str],
     },
 )
 DefaultButtonConfigurationTypeDef = TypedDict(
@@ -1437,14 +1404,32 @@
 )
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": NotRequired[str],
     },
 )
+EmailTemplateResponseTypeDef = TypedDict(
+    "EmailTemplateResponseTypeDef",
+    {
+        "CreationDate": str,
+        "LastModifiedDate": str,
+        "TemplateName": str,
+        "TemplateType": TemplateTypeType,
+        "Arn": NotRequired[str],
+        "DefaultSubstitutions": NotRequired[str],
+        "HtmlPart": NotRequired[str],
+        "RecommenderId": NotRequired[str],
+        "Subject": NotRequired[str],
+        "tags": NotRequired[Dict[str, str]],
+        "TemplateDescription": NotRequired[str],
+        "TextPart": NotRequired[str],
+        "Version": NotRequired[str],
+    },
+)
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": NotRequired[str],
         "Locale": NotRequired[str],
         "Make": NotRequired[str],
         "Model": NotRequired[str],
@@ -1464,15 +1449,15 @@
         "PostalCode": NotRequired[str],
         "Region": NotRequired[str],
     },
 )
 EndpointUserTypeDef = TypedDict(
     "EndpointUserTypeDef",
     {
-        "UserAttributes": NotRequired[Mapping[str, Sequence[str]]],
+        "UserAttributes": NotRequired[Dict[str, List[str]]],
         "UserId": NotRequired[str],
     },
 )
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
     {
         "Message": NotRequired[str],
@@ -1486,21 +1471,14 @@
         "StatusCode": int,
         "Address": NotRequired[str],
         "MessageId": NotRequired[str],
         "StatusMessage": NotRequired[str],
         "UpdatedToken": NotRequired[str],
     },
 )
-EndpointUserOutputTypeDef = TypedDict(
-    "EndpointUserOutputTypeDef",
-    {
-        "UserAttributes": NotRequired[Dict[str, List[str]]],
-        "UserId": NotRequired[str],
-    },
-)
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": NotRequired[str],
         "Context": NotRequired[Mapping[str, str]],
         "RawContent": NotRequired[str],
         "Substitutions": NotRequired[Mapping[str, Sequence[str]]],
@@ -1510,21 +1488,14 @@
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
-SetDimensionOutputTypeDef = TypedDict(
-    "SetDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-        "DimensionType": NotRequired[DimensionTypeType],
-    },
-)
 SetDimensionTypeDef = TypedDict(
     "SetDimensionTypeDef",
     {
         "Values": Sequence[str],
         "DimensionType": NotRequired[DimensionTypeType],
     },
 )
@@ -2027,22 +1998,14 @@
 )
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": NotRequired[str],
     },
 )
-JourneyScheduleOutputTypeDef = TypedDict(
-    "JourneyScheduleOutputTypeDef",
-    {
-        "EndTime": NotRequired[datetime],
-        "StartTime": NotRequired[datetime],
-        "Timezone": NotRequired[str],
-    },
-)
 JourneyRunResponseTypeDef = TypedDict(
     "JourneyRunResponseTypeDef",
     {
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
@@ -2074,16 +2037,16 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
-TagsModelOutputTypeDef = TypedDict(
-    "TagsModelOutputTypeDef",
+TagsModelTypeDef = TypedDict(
+    "TagsModelTypeDef",
     {
         "tags": Dict[str, str],
     },
 )
 ListTemplateVersionsRequestRequestTypeDef = TypedDict(
     "ListTemplateVersionsRequestRequestTypeDef",
     {
@@ -2248,20 +2211,14 @@
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": NotRequired[str],
         "Data": NotRequired[str],
     },
 )
-TagsModelTypeDef = TypedDict(
-    "TagsModelTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-)
 TemplateActiveVersionRequestTypeDef = TypedDict(
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": NotRequired[str],
     },
 )
 TemplateTypeDef = TypedDict(
@@ -2415,82 +2372,20 @@
 )
 RawEmailTypeDef = TypedDict(
     "RawEmailTypeDef",
     {
         "Data": NotRequired[BlobTypeDef],
     },
 )
-CampaignEmailMessageOutputTypeDef = TypedDict(
-    "CampaignEmailMessageOutputTypeDef",
-    {
-        "Body": NotRequired[str],
-        "FromAddress": NotRequired[str],
-        "Headers": NotRequired[List[MessageHeaderTypeDef]],
-        "HtmlBody": NotRequired[str],
-        "Title": NotRequired[str],
-    },
-)
-CampaignEmailMessageTypeDef = TypedDict(
-    "CampaignEmailMessageTypeDef",
-    {
-        "Body": NotRequired[str],
-        "FromAddress": NotRequired[str],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
-        "HtmlBody": NotRequired[str],
-        "Title": NotRequired[str],
-    },
-)
-EmailTemplateRequestTypeDef = TypedDict(
-    "EmailTemplateRequestTypeDef",
-    {
-        "DefaultSubstitutions": NotRequired[str],
-        "HtmlPart": NotRequired[str],
-        "RecommenderId": NotRequired[str],
-        "Subject": NotRequired[str],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
-        "tags": NotRequired[Mapping[str, str]],
-        "TemplateDescription": NotRequired[str],
-        "TextPart": NotRequired[str],
-    },
-)
-EmailTemplateResponseTypeDef = TypedDict(
-    "EmailTemplateResponseTypeDef",
-    {
-        "CreationDate": str,
-        "LastModifiedDate": str,
-        "TemplateName": str,
-        "TemplateType": TemplateTypeType,
-        "Arn": NotRequired[str],
-        "DefaultSubstitutions": NotRequired[str],
-        "HtmlPart": NotRequired[str],
-        "RecommenderId": NotRequired[str],
-        "Subject": NotRequired[str],
-        "Headers": NotRequired[List[MessageHeaderTypeDef]],
-        "tags": NotRequired[Dict[str, str]],
-        "TemplateDescription": NotRequired[str],
-        "TextPart": NotRequired[str],
-        "Version": NotRequired[str],
-    },
-)
 ChannelsResponseTypeDef = TypedDict(
     "ChannelsResponseTypeDef",
     {
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
-ClosedDaysOutputTypeDef = TypedDict(
-    "ClosedDaysOutputTypeDef",
-    {
-        "EMAIL": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "SMS": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "PUSH": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "VOICE": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "CUSTOM": NotRequired[List[ClosedDaysRuleTypeDef]],
-    },
-)
 ClosedDaysTypeDef = TypedDict(
     "ClosedDaysTypeDef",
     {
         "EMAIL": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
         "SMS": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
         "PUSH": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
         "VOICE": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
@@ -2666,14 +2561,30 @@
 UpdateBaiduChannelResponseTypeDef = TypedDict(
     "UpdateBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateEmailTemplateRequestRequestTypeDef = TypedDict(
+    "CreateEmailTemplateRequestRequestTypeDef",
+    {
+        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
+        "TemplateName": str,
+    },
+)
+UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateEmailTemplateRequestRequestTypeDef",
+    {
+        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
+        "TemplateName": str,
+        "CreateNewVersion": NotRequired[bool],
+        "Version": NotRequired[str],
+    },
+)
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2788,25 +2699,14 @@
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
         "CreateNewVersion": NotRequired[bool],
         "Version": NotRequired[str],
     },
 )
-CustomMessageActivityOutputTypeDef = TypedDict(
-    "CustomMessageActivityOutputTypeDef",
-    {
-        "DeliveryUri": NotRequired[str],
-        "EndpointTypes": NotRequired[List[EndpointTypesElementType]],
-        "MessageConfig": NotRequired[JourneyCustomMessageTypeDef],
-        "NextActivity": NotRequired[str],
-        "TemplateName": NotRequired[str],
-        "TemplateVersion": NotRequired[str],
-    },
-)
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": NotRequired[str],
         "EndpointTypes": NotRequired[Sequence[EndpointTypesElementType]],
         "MessageConfig": NotRequired[JourneyCustomMessageTypeDef],
         "NextActivity": NotRequired[str],
@@ -3056,14 +2956,21 @@
     {
         "MessageConfig": NotRequired[JourneyEmailMessageTypeDef],
         "NextActivity": NotRequired[str],
         "TemplateName": NotRequired[str],
         "TemplateVersion": NotRequired[str],
     },
 )
+GetEmailTemplateResponseTypeDef = TypedDict(
+    "GetEmailTemplateResponseTypeDef",
+    {
+        "EmailTemplateResponse": EmailTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": NotRequired[str],
         "Attributes": NotRequired[Mapping[str, Sequence[str]]],
         "ChannelType": NotRequired[ChannelTypeType],
         "Demographic": NotRequired[EndpointDemographicTypeDef],
@@ -3089,75 +2996,56 @@
         "Location": NotRequired[EndpointLocationTypeDef],
         "Metrics": NotRequired[Mapping[str, float]],
         "OptOut": NotRequired[str],
         "RequestId": NotRequired[str],
         "User": NotRequired[EndpointUserTypeDef],
     },
 )
-PublicEndpointTypeDef = TypedDict(
-    "PublicEndpointTypeDef",
+EndpointResponseTypeDef = TypedDict(
+    "EndpointResponseTypeDef",
     {
         "Address": NotRequired[str],
-        "Attributes": NotRequired[Mapping[str, Sequence[str]]],
+        "ApplicationId": NotRequired[str],
+        "Attributes": NotRequired[Dict[str, List[str]]],
         "ChannelType": NotRequired[ChannelTypeType],
+        "CohortId": NotRequired[str],
+        "CreationDate": NotRequired[str],
         "Demographic": NotRequired[EndpointDemographicTypeDef],
         "EffectiveDate": NotRequired[str],
         "EndpointStatus": NotRequired[str],
+        "Id": NotRequired[str],
         "Location": NotRequired[EndpointLocationTypeDef],
-        "Metrics": NotRequired[Mapping[str, float]],
+        "Metrics": NotRequired[Dict[str, float]],
         "OptOut": NotRequired[str],
         "RequestId": NotRequired[str],
         "User": NotRequired[EndpointUserTypeDef],
     },
 )
-SendUsersMessageResponseTypeDef = TypedDict(
-    "SendUsersMessageResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "RequestId": NotRequired[str],
-        "Result": NotRequired[Dict[str, Dict[str, EndpointMessageResultTypeDef]]],
-    },
-)
-EndpointResponseTypeDef = TypedDict(
-    "EndpointResponseTypeDef",
+PublicEndpointTypeDef = TypedDict(
+    "PublicEndpointTypeDef",
     {
         "Address": NotRequired[str],
-        "ApplicationId": NotRequired[str],
-        "Attributes": NotRequired[Dict[str, List[str]]],
+        "Attributes": NotRequired[Mapping[str, Sequence[str]]],
         "ChannelType": NotRequired[ChannelTypeType],
-        "CohortId": NotRequired[str],
-        "CreationDate": NotRequired[str],
         "Demographic": NotRequired[EndpointDemographicTypeDef],
         "EffectiveDate": NotRequired[str],
         "EndpointStatus": NotRequired[str],
-        "Id": NotRequired[str],
         "Location": NotRequired[EndpointLocationTypeDef],
-        "Metrics": NotRequired[Dict[str, float]],
+        "Metrics": NotRequired[Mapping[str, float]],
         "OptOut": NotRequired[str],
         "RequestId": NotRequired[str],
-        "User": NotRequired[EndpointUserOutputTypeDef],
-    },
-)
-EventDimensionsOutputTypeDef = TypedDict(
-    "EventDimensionsOutputTypeDef",
-    {
-        "Attributes": NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],
-        "EventType": NotRequired[SetDimensionOutputTypeDef],
-        "Metrics": NotRequired[Dict[str, MetricDimensionTypeDef]],
+        "User": NotRequired[EndpointUserTypeDef],
     },
 )
-SegmentDemographicsOutputTypeDef = TypedDict(
-    "SegmentDemographicsOutputTypeDef",
+SendUsersMessageResponseTypeDef = TypedDict(
+    "SendUsersMessageResponseTypeDef",
     {
-        "AppVersion": NotRequired[SetDimensionOutputTypeDef],
-        "Channel": NotRequired[SetDimensionOutputTypeDef],
-        "DeviceType": NotRequired[SetDimensionOutputTypeDef],
-        "Make": NotRequired[SetDimensionOutputTypeDef],
-        "Model": NotRequired[SetDimensionOutputTypeDef],
-        "Platform": NotRequired[SetDimensionOutputTypeDef],
+        "ApplicationId": str,
+        "RequestId": NotRequired[str],
+        "Result": NotRequired[Dict[str, Dict[str, EndpointMessageResultTypeDef]]],
     },
 )
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": NotRequired[Mapping[str, AttributeDimensionTypeDef]],
         "EventType": NotRequired[SetDimensionTypeDef],
@@ -3373,18 +3261,25 @@
         "JourneyId": str,
         "JourneyStateRequest": JourneyStateRequestTypeDef,
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagsModel": TagsModelOutputTypeDef,
+        "TagsModel": TagsModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagsModel": TagsModelTypeDef,
+    },
+)
 MessageResponseTypeDef = TypedDict(
     "MessageResponseTypeDef",
     {
         "ApplicationId": str,
         "EndpointResult": NotRequired[Dict[str, EndpointMessageResultTypeDef]],
         "RequestId": NotRequired[str],
         "Result": NotRequired[Dict[str, MessageResultTypeDef]],
@@ -3399,24 +3294,14 @@
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-OpenHoursOutputTypeDef = TypedDict(
-    "OpenHoursOutputTypeDef",
-    {
-        "EMAIL": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "SMS": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "PUSH": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "VOICE": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "CUSTOM": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-    },
-)
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
         "SMS": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
         "PUSH": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
         "VOICE": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
@@ -3426,20 +3311,14 @@
 PutEventStreamRequestRequestTypeDef = TypedDict(
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
-RandomSplitActivityOutputTypeDef = TypedDict(
-    "RandomSplitActivityOutputTypeDef",
-    {
-        "Branches": NotRequired[List[RandomSplitEntryTypeDef]],
-    },
-)
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": NotRequired[Sequence[RandomSplitEntryTypeDef]],
     },
 )
 SegmentBehaviorsTypeDef = TypedDict(
@@ -3479,25 +3358,16 @@
 )
 SimpleEmailTypeDef = TypedDict(
     "SimpleEmailTypeDef",
     {
         "HtmlPart": NotRequired[SimpleEmailPartTypeDef],
         "Subject": NotRequired[SimpleEmailPartTypeDef],
         "TextPart": NotRequired[SimpleEmailPartTypeDef],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagsModel": TagsModelTypeDef,
-    },
-)
-TagsModelUnionTypeDef = Union[TagsModelTypeDef, TagsModelOutputTypeDef]
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
@@ -3588,37 +3458,14 @@
         "CloudWatchMetricsEnabled": NotRequired[bool],
         "EventTaggingEnabled": NotRequired[bool],
         "Limits": NotRequired[CampaignLimitsTypeDef],
         "QuietTime": NotRequired[QuietTimeTypeDef],
         "JourneyLimits": NotRequired[ApplicationSettingsJourneyLimitsTypeDef],
     },
 )
-CreateEmailTemplateRequestRequestTypeDef = TypedDict(
-    "CreateEmailTemplateRequestRequestTypeDef",
-    {
-        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
-        "TemplateName": str,
-    },
-)
-UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
-    "UpdateEmailTemplateRequestRequestTypeDef",
-    {
-        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
-        "TemplateName": str,
-        "CreateNewVersion": NotRequired[bool],
-        "Version": NotRequired[str],
-    },
-)
-GetEmailTemplateResponseTypeDef = TypedDict(
-    "GetEmailTemplateResponseTypeDef",
-    {
-        "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3662,21 +3509,14 @@
     "UpdateEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
         "EndpointRequest": EndpointRequestTypeDef,
     },
 )
-SendUsersMessagesResponseTypeDef = TypedDict(
-    "SendUsersMessagesResponseTypeDef",
-    {
-        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3689,33 +3529,19 @@
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CampaignEventFilterOutputTypeDef = TypedDict(
-    "CampaignEventFilterOutputTypeDef",
-    {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
-    },
-)
-EventConditionOutputTypeDef = TypedDict(
-    "EventConditionOutputTypeDef",
-    {
-        "Dimensions": NotRequired[EventDimensionsOutputTypeDef],
-        "MessageActivity": NotRequired[str],
-    },
-)
-EventFilterOutputTypeDef = TypedDict(
-    "EventFilterOutputTypeDef",
+SendUsersMessagesResponseTypeDef = TypedDict(
+    "SendUsersMessagesResponseTypeDef",
     {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
+        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
         "FilterType": FilterTypeType,
@@ -3765,21 +3591,14 @@
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SegmentLocationOutputTypeDef = TypedDict(
-    "SegmentLocationOutputTypeDef",
-    {
-        "Country": NotRequired[SetDimensionOutputTypeDef],
-        "GPSPoint": NotRequired[GPSPointDimensionTypeDef],
-    },
-)
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": NotRequired[SetDimensionTypeDef],
         "GPSPoint": NotRequired[GPSPointDimensionTypeDef],
     },
 )
@@ -3910,35 +3729,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": NotRequired[str],
-        "EventFilter": NotRequired[CampaignEventFilterOutputTypeDef],
-        "QuietTime": NotRequired[QuietTimeTypeDef],
-    },
-)
-ScheduleOutputTypeDef = TypedDict(
-    "ScheduleOutputTypeDef",
-    {
-        "StartTime": str,
-        "EndTime": NotRequired[str],
-        "EventFilter": NotRequired[CampaignEventFilterOutputTypeDef],
-        "Frequency": NotRequired[FrequencyType],
-        "IsLocalTime": NotRequired[bool],
+        "EventFilter": NotRequired[CampaignEventFilterTypeDef],
         "QuietTime": NotRequired[QuietTimeTypeDef],
-        "Timezone": NotRequired[str],
-    },
-)
-EventStartConditionOutputTypeDef = TypedDict(
-    "EventStartConditionOutputTypeDef",
-    {
-        "EventFilter": NotRequired[EventFilterOutputTypeDef],
-        "SegmentId": NotRequired[str],
     },
 )
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "StartTime": str,
         "EndTime": NotRequired[str],
@@ -3979,25 +3779,14 @@
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SegmentDimensionsOutputTypeDef = TypedDict(
-    "SegmentDimensionsOutputTypeDef",
-    {
-        "Attributes": NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],
-        "Behavior": NotRequired[SegmentBehaviorsTypeDef],
-        "Demographic": NotRequired[SegmentDemographicsOutputTypeDef],
-        "Location": NotRequired[SegmentLocationOutputTypeDef],
-        "Metrics": NotRequired[Dict[str, MetricDimensionTypeDef]],
-        "UserAttributes": NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],
-    },
-)
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": NotRequired[Mapping[str, AttributeDimensionTypeDef]],
         "Behavior": NotRequired[SegmentBehaviorsTypeDef],
         "Demographic": NotRequired[SegmentDemographicsTypeDef],
         "Location": NotRequired[SegmentLocationTypeDef],
@@ -4015,23 +3804,14 @@
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CampaignInAppMessageOutputTypeDef = TypedDict(
-    "CampaignInAppMessageOutputTypeDef",
-    {
-        "Body": NotRequired[str],
-        "Content": NotRequired[List[InAppMessageContentTypeDef]],
-        "CustomConfig": NotRequired[Dict[str, str]],
-        "Layout": NotRequired[LayoutType],
-    },
-)
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": NotRequired[str],
         "Content": NotRequired[Sequence[InAppMessageContentTypeDef]],
         "CustomConfig": NotRequired[Mapping[str, str]],
         "Layout": NotRequired[LayoutType],
@@ -4116,22 +3896,14 @@
         "DefaultPushNotificationMessage": NotRequired[DefaultPushNotificationMessageTypeDef],
         "EmailMessage": NotRequired[EmailMessageTypeDef],
         "GCMMessage": NotRequired[GCMMessageTypeDef],
         "SMSMessage": NotRequired[SMSMessageTypeDef],
         "VoiceMessage": NotRequired[VoiceMessageTypeDef],
     },
 )
-StartConditionOutputTypeDef = TypedDict(
-    "StartConditionOutputTypeDef",
-    {
-        "Description": NotRequired[str],
-        "EventStartCondition": NotRequired[EventStartConditionOutputTypeDef],
-        "SegmentStartCondition": NotRequired[SegmentConditionTypeDef],
-    },
-)
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
         "Description": NotRequired[str],
         "EventStartCondition": NotRequired[EventStartConditionTypeDef],
         "SegmentStartCondition": NotRequired[SegmentConditionTypeDef],
     },
@@ -4139,31 +3911,14 @@
 PutEventsRequestRequestTypeDef = TypedDict(
     "PutEventsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EventsRequest": EventsRequestTypeDef,
     },
 )
-SegmentGroupOutputTypeDef = TypedDict(
-    "SegmentGroupOutputTypeDef",
-    {
-        "Dimensions": NotRequired[List[SegmentDimensionsOutputTypeDef]],
-        "SourceSegments": NotRequired[List[SegmentReferenceTypeDef]],
-        "SourceType": NotRequired[SourceTypeType],
-        "Type": NotRequired[TypeType],
-    },
-)
-SimpleConditionOutputTypeDef = TypedDict(
-    "SimpleConditionOutputTypeDef",
-    {
-        "EventCondition": NotRequired[EventConditionOutputTypeDef],
-        "SegmentCondition": NotRequired[SegmentConditionTypeDef],
-        "SegmentDimensions": NotRequired[SegmentDimensionsOutputTypeDef],
-    },
-)
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
     {
         "Dimensions": NotRequired[Sequence[SegmentDimensionsTypeDef]],
         "SourceSegments": NotRequired[Sequence[SegmentReferenceTypeDef]],
         "SourceType": NotRequired[SourceTypeType],
         "Type": NotRequired[TypeType],
@@ -4173,28 +3928,14 @@
     "SimpleConditionTypeDef",
     {
         "EventCondition": NotRequired[EventConditionTypeDef],
         "SegmentCondition": NotRequired[SegmentConditionTypeDef],
         "SegmentDimensions": NotRequired[SegmentDimensionsTypeDef],
     },
 )
-MessageConfigurationOutputTypeDef = TypedDict(
-    "MessageConfigurationOutputTypeDef",
-    {
-        "ADMMessage": NotRequired[MessageTypeDef],
-        "APNSMessage": NotRequired[MessageTypeDef],
-        "BaiduMessage": NotRequired[MessageTypeDef],
-        "CustomMessage": NotRequired[CampaignCustomMessageTypeDef],
-        "DefaultMessage": NotRequired[MessageTypeDef],
-        "EmailMessage": NotRequired[CampaignEmailMessageOutputTypeDef],
-        "GCMMessage": NotRequired[MessageTypeDef],
-        "SMSMessage": NotRequired[CampaignSmsMessageTypeDef],
-        "InAppMessage": NotRequired[CampaignInAppMessageOutputTypeDef],
-    },
-)
 MessageConfigurationTypeDef = TypedDict(
     "MessageConfigurationTypeDef",
     {
         "ADMMessage": NotRequired[MessageTypeDef],
         "APNSMessage": NotRequired[MessageTypeDef],
         "BaiduMessage": NotRequired[MessageTypeDef],
         "CustomMessage": NotRequired[CampaignCustomMessageTypeDef],
@@ -4279,35 +4020,14 @@
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
         "Context": NotRequired[Mapping[str, str]],
         "TemplateConfiguration": NotRequired[TemplateConfigurationTypeDef],
         "TraceId": NotRequired[str],
     },
 )
-SegmentGroupListOutputTypeDef = TypedDict(
-    "SegmentGroupListOutputTypeDef",
-    {
-        "Groups": NotRequired[List[SegmentGroupOutputTypeDef]],
-        "Include": NotRequired[IncludeType],
-    },
-)
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "Conditions": NotRequired[List[SimpleConditionOutputTypeDef]],
-        "Operator": NotRequired[OperatorType],
-    },
-)
-MultiConditionalBranchOutputTypeDef = TypedDict(
-    "MultiConditionalBranchOutputTypeDef",
-    {
-        "Condition": NotRequired[SimpleConditionOutputTypeDef],
-        "NextActivity": NotRequired[str],
-    },
-)
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": NotRequired[Sequence[SegmentGroupTypeDef]],
         "Include": NotRequired[IncludeType],
     },
 )
@@ -4326,17 +4046,17 @@
     },
 )
 TreatmentResourceTypeDef = TypedDict(
     "TreatmentResourceTypeDef",
     {
         "Id": str,
         "SizePercent": int,
-        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationOutputTypeDef],
-        "MessageConfiguration": NotRequired[MessageConfigurationOutputTypeDef],
-        "Schedule": NotRequired[ScheduleOutputTypeDef],
+        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationTypeDef],
+        "MessageConfiguration": NotRequired[MessageConfigurationTypeDef],
+        "Schedule": NotRequired[ScheduleTypeDef],
         "State": NotRequired[CampaignStateTypeDef],
         "TemplateConfiguration": NotRequired[TemplateConfigurationTypeDef],
         "TreatmentDescription": NotRequired[str],
         "TreatmentName": NotRequired[str],
     },
 )
 WriteTreatmentResourceTypeDef = TypedDict(
@@ -4375,40 +4095,23 @@
     "SegmentResponseTypeDef",
     {
         "ApplicationId": str,
         "Arn": str,
         "CreationDate": str,
         "Id": str,
         "SegmentType": SegmentTypeType,
-        "Dimensions": NotRequired[SegmentDimensionsOutputTypeDef],
+        "Dimensions": NotRequired[SegmentDimensionsTypeDef],
         "ImportDefinition": NotRequired[SegmentImportResourceTypeDef],
         "LastModifiedDate": NotRequired[str],
         "Name": NotRequired[str],
-        "SegmentGroups": NotRequired[SegmentGroupListOutputTypeDef],
+        "SegmentGroups": NotRequired[SegmentGroupListTypeDef],
         "tags": NotRequired[Dict[str, str]],
         "Version": NotRequired[int],
     },
 )
-ConditionalSplitActivityOutputTypeDef = TypedDict(
-    "ConditionalSplitActivityOutputTypeDef",
-    {
-        "Condition": NotRequired[ConditionOutputTypeDef],
-        "EvaluationWaitTime": NotRequired[WaitTimeTypeDef],
-        "FalseActivity": NotRequired[str],
-        "TrueActivity": NotRequired[str],
-    },
-)
-MultiConditionalSplitActivityOutputTypeDef = TypedDict(
-    "MultiConditionalSplitActivityOutputTypeDef",
-    {
-        "Branches": NotRequired[List[MultiConditionalBranchOutputTypeDef]],
-        "DefaultActivity": NotRequired[str],
-        "EvaluationWaitTime": NotRequired[WaitTimeTypeDef],
-    },
-)
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": NotRequired[SegmentDimensionsTypeDef],
         "Name": NotRequired[str],
         "SegmentGroups": NotRequired[SegmentGroupListTypeDef],
         "tags": NotRequired[Mapping[str, str]],
@@ -4438,24 +4141,24 @@
         "Arn": str,
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "SegmentId": str,
         "SegmentVersion": int,
         "AdditionalTreatments": NotRequired[List[TreatmentResourceTypeDef]],
-        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationOutputTypeDef],
+        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationTypeDef],
         "DefaultState": NotRequired[CampaignStateTypeDef],
         "Description": NotRequired[str],
         "HoldoutPercent": NotRequired[int],
         "Hook": NotRequired[CampaignHookTypeDef],
         "IsPaused": NotRequired[bool],
         "Limits": NotRequired[CampaignLimitsTypeDef],
-        "MessageConfiguration": NotRequired[MessageConfigurationOutputTypeDef],
+        "MessageConfiguration": NotRequired[MessageConfigurationTypeDef],
         "Name": NotRequired[str],
-        "Schedule": NotRequired[ScheduleOutputTypeDef],
+        "Schedule": NotRequired[ScheduleTypeDef],
         "State": NotRequired[CampaignStateTypeDef],
         "tags": NotRequired[Dict[str, str]],
         "TemplateConfiguration": NotRequired[TemplateConfigurationTypeDef],
         "TreatmentDescription": NotRequired[str],
         "TreatmentName": NotRequired[str],
         "Version": NotRequired[int],
         "Priority": NotRequired[int],
@@ -4528,30 +4231,14 @@
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ActivityOutputTypeDef = TypedDict(
-    "ActivityOutputTypeDef",
-    {
-        "CUSTOM": NotRequired[CustomMessageActivityOutputTypeDef],
-        "ConditionalSplit": NotRequired[ConditionalSplitActivityOutputTypeDef],
-        "Description": NotRequired[str],
-        "EMAIL": NotRequired[EmailMessageActivityTypeDef],
-        "Holdout": NotRequired[HoldoutActivityTypeDef],
-        "MultiCondition": NotRequired[MultiConditionalSplitActivityOutputTypeDef],
-        "PUSH": NotRequired[PushMessageActivityTypeDef],
-        "RandomSplit": NotRequired[RandomSplitActivityOutputTypeDef],
-        "SMS": NotRequired[SMSMessageActivityTypeDef],
-        "Wait": NotRequired[WaitActivityTypeDef],
-        "ContactCenter": NotRequired[ContactCenterActivityTypeDef],
-    },
-)
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteSegmentRequest": WriteSegmentRequestTypeDef,
     },
 )
@@ -4652,32 +4339,32 @@
 )
 JourneyResponseTypeDef = TypedDict(
     "JourneyResponseTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
-        "Activities": NotRequired[Dict[str, ActivityOutputTypeDef]],
+        "Activities": NotRequired[Dict[str, ActivityTypeDef]],
         "CreationDate": NotRequired[str],
         "LastModifiedDate": NotRequired[str],
         "Limits": NotRequired[JourneyLimitsTypeDef],
         "LocalTime": NotRequired[bool],
         "QuietTime": NotRequired[QuietTimeTypeDef],
         "RefreshFrequency": NotRequired[str],
-        "Schedule": NotRequired[JourneyScheduleOutputTypeDef],
+        "Schedule": NotRequired[JourneyScheduleTypeDef],
         "StartActivity": NotRequired[str],
-        "StartCondition": NotRequired[StartConditionOutputTypeDef],
+        "StartCondition": NotRequired[StartConditionTypeDef],
         "State": NotRequired[StateType],
         "tags": NotRequired[Dict[str, str]],
         "WaitForQuietTime": NotRequired[bool],
         "RefreshOnSegmentUpdate": NotRequired[bool],
         "JourneyChannelSettings": NotRequired[JourneyChannelSettingsTypeDef],
         "SendingSchedule": NotRequired[bool],
-        "OpenHours": NotRequired[OpenHoursOutputTypeDef],
-        "ClosedDays": NotRequired[ClosedDaysOutputTypeDef],
+        "OpenHours": NotRequired[OpenHoursTypeDef],
+        "ClosedDays": NotRequired[ClosedDaysTypeDef],
         "TimezoneEstimationMethods": NotRequired[List[TimezoneEstimationMethodsElementType]],
     },
 )
 WriteJourneyRequestTypeDef = TypedDict(
     "WriteJourneyRequestTypeDef",
     {
         "Name": str,
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -78,40 +78,39 @@
     "AddressConfigurationTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
     "JourneyTimeframeCapTypeDef",
     "CampaignHookTypeDef",
     "CampaignLimitsTypeDef",
     "QuietTimeTypeDef",
-    "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
     "BlobTypeDef",
     "CampaignCustomMessageTypeDef",
-    "MessageHeaderTypeDef",
+    "CampaignEmailMessageTypeDef",
     "CampaignStateTypeDef",
-    "CustomDeliveryConfigurationOutputTypeDef",
+    "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
-    "CustomDeliveryConfigurationTypeDef",
     "JourneyCustomMessageTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
@@ -143,23 +142,22 @@
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
+    "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
-    "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
-    "SetDimensionOutputTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
@@ -217,21 +215,20 @@
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
     "InAppMessageBodyConfigTypeDef",
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
     "JourneyPushMessageTypeDef",
-    "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagsModelOutputTypeDef",
+    "TagsModelTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
@@ -242,15 +239,14 @@
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
-    "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
@@ -263,20 +259,15 @@
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
     "ApplicationSettingsJourneyLimitsTypeDef",
     "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
     "RawEmailTypeDef",
-    "CampaignEmailMessageOutputTypeDef",
-    "CampaignEmailMessageTypeDef",
-    "EmailTemplateRequestTypeDef",
-    "EmailTemplateResponseTypeDef",
     "ChannelsResponseTypeDef",
-    "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
     "DeleteApnsChannelResponseTypeDef",
     "DeleteApnsSandboxChannelResponseTypeDef",
@@ -295,14 +286,16 @@
     "RemoveAttributesResponseTypeDef",
     "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "UpdateBaiduChannelResponseTypeDef",
+    "CreateEmailTemplateRequestRequestTypeDef",
+    "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "CreateInAppTemplateResponseTypeDef",
@@ -312,15 +305,14 @@
     "GetRecommenderConfigurationResponseTypeDef",
     "ListRecommenderConfigurationsResponseTypeDef",
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
-    "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
     "PushNotificationTemplateRequestTypeDef",
     "PushNotificationTemplateResponseTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
@@ -346,21 +338,20 @@
     "GetSmsChannelResponseTypeDef",
     "UpdateSmsChannelResponseTypeDef",
     "DeleteVoiceChannelResponseTypeDef",
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
     "EmailMessageActivityTypeDef",
+    "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
+    "EndpointResponseTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
-    "EndpointResponseTypeDef",
-    "EventDimensionsOutputTypeDef",
-    "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
@@ -377,68 +368,58 @@
     "ImportJobResponseTypeDef",
     "InAppMessageButtonTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
-    "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
-    "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "TagsModelUnionTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
-    "CreateEmailTemplateRequestRequestTypeDef",
-    "UpdateEmailTemplateRequestRequestTypeDef",
-    "GetEmailTemplateResponseTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
     "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
-    "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
-    "CampaignEventFilterOutputTypeDef",
-    "EventConditionOutputTypeDef",
-    "EventFilterOutputTypeDef",
+    "SendUsersMessagesResponseTypeDef",
     "CampaignEventFilterTypeDef",
     "EventConditionTypeDef",
     "EventFilterTypeDef",
     "EventsResponseTypeDef",
     "EventsBatchTypeDef",
     "CreateExportJobResponseTypeDef",
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
-    "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
@@ -450,80 +431,66 @@
     "GetApplicationSettingsResponseTypeDef",
     "UpdateApplicationSettingsResponseTypeDef",
     "UpdateApplicationSettingsRequestRequestTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
-    "ScheduleOutputTypeDef",
-    "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
     "EventStartConditionTypeDef",
     "PutEventsResponseTypeDef",
     "EventsRequestTypeDef",
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
-    "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
-    "CampaignInAppMessageOutputTypeDef",
     "CampaignInAppMessageTypeDef",
     "InAppMessageTypeDef",
     "InAppTemplateRequestTypeDef",
     "InAppTemplateResponseTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
-    "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
-    "SegmentGroupOutputTypeDef",
-    "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
-    "MessageConfigurationOutputTypeDef",
     "MessageConfigurationTypeDef",
     "InAppMessageCampaignTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
     "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
-    "SegmentGroupListOutputTypeDef",
-    "ConditionOutputTypeDef",
-    "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
     "WriteTreatmentResourceTypeDef",
     "InAppMessagesResponseTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
-    "ConditionalSplitActivityOutputTypeDef",
-    "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
     "WriteCampaignRequestTypeDef",
     "GetInAppMessagesResponseTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
-    "ActivityOutputTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "UpdateSegmentRequestRequestTypeDef",
     "ActivityTypeDef",
     "CampaignsResponseTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignResponseTypeDef",
     "GetCampaignResponseTypeDef",
@@ -842,21 +809,14 @@
 QuietTimeTypeDef = TypedDict(
     "QuietTimeTypeDef",
     {
         "End": NotRequired[str],
         "Start": NotRequired[str],
     },
 )
-AttributeDimensionOutputTypeDef = TypedDict(
-    "AttributeDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-        "AttributeType": NotRequired[AttributeTypeType],
-    },
-)
 AttributeDimensionTypeDef = TypedDict(
     "AttributeDimensionTypeDef",
     {
         "Values": Sequence[str],
         "AttributeType": NotRequired[AttributeTypeType],
     },
 )
@@ -914,32 +874,34 @@
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": NotRequired[str],
     },
 )
-MessageHeaderTypeDef = TypedDict(
-    "MessageHeaderTypeDef",
+CampaignEmailMessageTypeDef = TypedDict(
+    "CampaignEmailMessageTypeDef",
     {
-        "Name": NotRequired[str],
-        "Value": NotRequired[str],
+        "Body": NotRequired[str],
+        "FromAddress": NotRequired[str],
+        "HtmlBody": NotRequired[str],
+        "Title": NotRequired[str],
     },
 )
 CampaignStateTypeDef = TypedDict(
     "CampaignStateTypeDef",
     {
         "CampaignStatus": NotRequired[CampaignStatusType],
     },
 )
-CustomDeliveryConfigurationOutputTypeDef = TypedDict(
-    "CustomDeliveryConfigurationOutputTypeDef",
+CustomDeliveryConfigurationTypeDef = TypedDict(
+    "CustomDeliveryConfigurationTypeDef",
     {
         "DeliveryUri": str,
-        "EndpointTypes": NotRequired[List[EndpointTypesElementType]],
+        "EndpointTypes": NotRequired[Sequence[EndpointTypesElementType]],
     },
 )
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": NotRequired[str],
         "MessageType": NotRequired[MessageTypeType],
@@ -991,14 +953,26 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
+EmailTemplateRequestTypeDef = TypedDict(
+    "EmailTemplateRequestTypeDef",
+    {
+        "DefaultSubstitutions": NotRequired[str],
+        "HtmlPart": NotRequired[str],
+        "RecommenderId": NotRequired[str],
+        "Subject": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+        "TemplateDescription": NotRequired[str],
+        "TextPart": NotRequired[str],
+    },
+)
 CreateTemplateMessageBodyTypeDef = TypedDict(
     "CreateTemplateMessageBodyTypeDef",
     {
         "Arn": NotRequired[str],
         "Message": NotRequired[str],
         "RequestID": NotRequired[str],
     },
@@ -1081,21 +1055,14 @@
         "DefaultSubstitutions": NotRequired[str],
         "LanguageCode": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
         "TemplateDescription": NotRequired[str],
         "VoiceId": NotRequired[str],
     },
 )
-CustomDeliveryConfigurationTypeDef = TypedDict(
-    "CustomDeliveryConfigurationTypeDef",
-    {
-        "DeliveryUri": str,
-        "EndpointTypes": NotRequired[Sequence[EndpointTypesElementType]],
-    },
-)
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": NotRequired[str],
     },
 )
 DefaultButtonConfigurationTypeDef = TypedDict(
@@ -1437,14 +1404,32 @@
 )
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": NotRequired[str],
     },
 )
+EmailTemplateResponseTypeDef = TypedDict(
+    "EmailTemplateResponseTypeDef",
+    {
+        "CreationDate": str,
+        "LastModifiedDate": str,
+        "TemplateName": str,
+        "TemplateType": TemplateTypeType,
+        "Arn": NotRequired[str],
+        "DefaultSubstitutions": NotRequired[str],
+        "HtmlPart": NotRequired[str],
+        "RecommenderId": NotRequired[str],
+        "Subject": NotRequired[str],
+        "tags": NotRequired[Dict[str, str]],
+        "TemplateDescription": NotRequired[str],
+        "TextPart": NotRequired[str],
+        "Version": NotRequired[str],
+    },
+)
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": NotRequired[str],
         "Locale": NotRequired[str],
         "Make": NotRequired[str],
         "Model": NotRequired[str],
@@ -1464,15 +1449,15 @@
         "PostalCode": NotRequired[str],
         "Region": NotRequired[str],
     },
 )
 EndpointUserTypeDef = TypedDict(
     "EndpointUserTypeDef",
     {
-        "UserAttributes": NotRequired[Mapping[str, Sequence[str]]],
+        "UserAttributes": NotRequired[Dict[str, List[str]]],
         "UserId": NotRequired[str],
     },
 )
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
     {
         "Message": NotRequired[str],
@@ -1486,21 +1471,14 @@
         "StatusCode": int,
         "Address": NotRequired[str],
         "MessageId": NotRequired[str],
         "StatusMessage": NotRequired[str],
         "UpdatedToken": NotRequired[str],
     },
 )
-EndpointUserOutputTypeDef = TypedDict(
-    "EndpointUserOutputTypeDef",
-    {
-        "UserAttributes": NotRequired[Dict[str, List[str]]],
-        "UserId": NotRequired[str],
-    },
-)
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": NotRequired[str],
         "Context": NotRequired[Mapping[str, str]],
         "RawContent": NotRequired[str],
         "Substitutions": NotRequired[Mapping[str, Sequence[str]]],
@@ -1510,21 +1488,14 @@
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
-SetDimensionOutputTypeDef = TypedDict(
-    "SetDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-        "DimensionType": NotRequired[DimensionTypeType],
-    },
-)
 SetDimensionTypeDef = TypedDict(
     "SetDimensionTypeDef",
     {
         "Values": Sequence[str],
         "DimensionType": NotRequired[DimensionTypeType],
     },
 )
@@ -2027,22 +1998,14 @@
 )
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": NotRequired[str],
     },
 )
-JourneyScheduleOutputTypeDef = TypedDict(
-    "JourneyScheduleOutputTypeDef",
-    {
-        "EndTime": NotRequired[datetime],
-        "StartTime": NotRequired[datetime],
-        "Timezone": NotRequired[str],
-    },
-)
 JourneyRunResponseTypeDef = TypedDict(
     "JourneyRunResponseTypeDef",
     {
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
@@ -2074,16 +2037,16 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
-TagsModelOutputTypeDef = TypedDict(
-    "TagsModelOutputTypeDef",
+TagsModelTypeDef = TypedDict(
+    "TagsModelTypeDef",
     {
         "tags": Dict[str, str],
     },
 )
 ListTemplateVersionsRequestRequestTypeDef = TypedDict(
     "ListTemplateVersionsRequestRequestTypeDef",
     {
@@ -2248,20 +2211,14 @@
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": NotRequired[str],
         "Data": NotRequired[str],
     },
 )
-TagsModelTypeDef = TypedDict(
-    "TagsModelTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-)
 TemplateActiveVersionRequestTypeDef = TypedDict(
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": NotRequired[str],
     },
 )
 TemplateTypeDef = TypedDict(
@@ -2415,82 +2372,20 @@
 )
 RawEmailTypeDef = TypedDict(
     "RawEmailTypeDef",
     {
         "Data": NotRequired[BlobTypeDef],
     },
 )
-CampaignEmailMessageOutputTypeDef = TypedDict(
-    "CampaignEmailMessageOutputTypeDef",
-    {
-        "Body": NotRequired[str],
-        "FromAddress": NotRequired[str],
-        "Headers": NotRequired[List[MessageHeaderTypeDef]],
-        "HtmlBody": NotRequired[str],
-        "Title": NotRequired[str],
-    },
-)
-CampaignEmailMessageTypeDef = TypedDict(
-    "CampaignEmailMessageTypeDef",
-    {
-        "Body": NotRequired[str],
-        "FromAddress": NotRequired[str],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
-        "HtmlBody": NotRequired[str],
-        "Title": NotRequired[str],
-    },
-)
-EmailTemplateRequestTypeDef = TypedDict(
-    "EmailTemplateRequestTypeDef",
-    {
-        "DefaultSubstitutions": NotRequired[str],
-        "HtmlPart": NotRequired[str],
-        "RecommenderId": NotRequired[str],
-        "Subject": NotRequired[str],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
-        "tags": NotRequired[Mapping[str, str]],
-        "TemplateDescription": NotRequired[str],
-        "TextPart": NotRequired[str],
-    },
-)
-EmailTemplateResponseTypeDef = TypedDict(
-    "EmailTemplateResponseTypeDef",
-    {
-        "CreationDate": str,
-        "LastModifiedDate": str,
-        "TemplateName": str,
-        "TemplateType": TemplateTypeType,
-        "Arn": NotRequired[str],
-        "DefaultSubstitutions": NotRequired[str],
-        "HtmlPart": NotRequired[str],
-        "RecommenderId": NotRequired[str],
-        "Subject": NotRequired[str],
-        "Headers": NotRequired[List[MessageHeaderTypeDef]],
-        "tags": NotRequired[Dict[str, str]],
-        "TemplateDescription": NotRequired[str],
-        "TextPart": NotRequired[str],
-        "Version": NotRequired[str],
-    },
-)
 ChannelsResponseTypeDef = TypedDict(
     "ChannelsResponseTypeDef",
     {
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
-ClosedDaysOutputTypeDef = TypedDict(
-    "ClosedDaysOutputTypeDef",
-    {
-        "EMAIL": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "SMS": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "PUSH": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "VOICE": NotRequired[List[ClosedDaysRuleTypeDef]],
-        "CUSTOM": NotRequired[List[ClosedDaysRuleTypeDef]],
-    },
-)
 ClosedDaysTypeDef = TypedDict(
     "ClosedDaysTypeDef",
     {
         "EMAIL": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
         "SMS": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
         "PUSH": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
         "VOICE": NotRequired[Sequence[ClosedDaysRuleTypeDef]],
@@ -2666,14 +2561,30 @@
 UpdateBaiduChannelResponseTypeDef = TypedDict(
     "UpdateBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateEmailTemplateRequestRequestTypeDef = TypedDict(
+    "CreateEmailTemplateRequestRequestTypeDef",
+    {
+        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
+        "TemplateName": str,
+    },
+)
+UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateEmailTemplateRequestRequestTypeDef",
+    {
+        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
+        "TemplateName": str,
+        "CreateNewVersion": NotRequired[bool],
+        "Version": NotRequired[str],
+    },
+)
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2788,25 +2699,14 @@
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
         "CreateNewVersion": NotRequired[bool],
         "Version": NotRequired[str],
     },
 )
-CustomMessageActivityOutputTypeDef = TypedDict(
-    "CustomMessageActivityOutputTypeDef",
-    {
-        "DeliveryUri": NotRequired[str],
-        "EndpointTypes": NotRequired[List[EndpointTypesElementType]],
-        "MessageConfig": NotRequired[JourneyCustomMessageTypeDef],
-        "NextActivity": NotRequired[str],
-        "TemplateName": NotRequired[str],
-        "TemplateVersion": NotRequired[str],
-    },
-)
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": NotRequired[str],
         "EndpointTypes": NotRequired[Sequence[EndpointTypesElementType]],
         "MessageConfig": NotRequired[JourneyCustomMessageTypeDef],
         "NextActivity": NotRequired[str],
@@ -3056,14 +2956,21 @@
     {
         "MessageConfig": NotRequired[JourneyEmailMessageTypeDef],
         "NextActivity": NotRequired[str],
         "TemplateName": NotRequired[str],
         "TemplateVersion": NotRequired[str],
     },
 )
+GetEmailTemplateResponseTypeDef = TypedDict(
+    "GetEmailTemplateResponseTypeDef",
+    {
+        "EmailTemplateResponse": EmailTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": NotRequired[str],
         "Attributes": NotRequired[Mapping[str, Sequence[str]]],
         "ChannelType": NotRequired[ChannelTypeType],
         "Demographic": NotRequired[EndpointDemographicTypeDef],
@@ -3089,75 +2996,56 @@
         "Location": NotRequired[EndpointLocationTypeDef],
         "Metrics": NotRequired[Mapping[str, float]],
         "OptOut": NotRequired[str],
         "RequestId": NotRequired[str],
         "User": NotRequired[EndpointUserTypeDef],
     },
 )
-PublicEndpointTypeDef = TypedDict(
-    "PublicEndpointTypeDef",
+EndpointResponseTypeDef = TypedDict(
+    "EndpointResponseTypeDef",
     {
         "Address": NotRequired[str],
-        "Attributes": NotRequired[Mapping[str, Sequence[str]]],
+        "ApplicationId": NotRequired[str],
+        "Attributes": NotRequired[Dict[str, List[str]]],
         "ChannelType": NotRequired[ChannelTypeType],
+        "CohortId": NotRequired[str],
+        "CreationDate": NotRequired[str],
         "Demographic": NotRequired[EndpointDemographicTypeDef],
         "EffectiveDate": NotRequired[str],
         "EndpointStatus": NotRequired[str],
+        "Id": NotRequired[str],
         "Location": NotRequired[EndpointLocationTypeDef],
-        "Metrics": NotRequired[Mapping[str, float]],
+        "Metrics": NotRequired[Dict[str, float]],
         "OptOut": NotRequired[str],
         "RequestId": NotRequired[str],
         "User": NotRequired[EndpointUserTypeDef],
     },
 )
-SendUsersMessageResponseTypeDef = TypedDict(
-    "SendUsersMessageResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "RequestId": NotRequired[str],
-        "Result": NotRequired[Dict[str, Dict[str, EndpointMessageResultTypeDef]]],
-    },
-)
-EndpointResponseTypeDef = TypedDict(
-    "EndpointResponseTypeDef",
+PublicEndpointTypeDef = TypedDict(
+    "PublicEndpointTypeDef",
     {
         "Address": NotRequired[str],
-        "ApplicationId": NotRequired[str],
-        "Attributes": NotRequired[Dict[str, List[str]]],
+        "Attributes": NotRequired[Mapping[str, Sequence[str]]],
         "ChannelType": NotRequired[ChannelTypeType],
-        "CohortId": NotRequired[str],
-        "CreationDate": NotRequired[str],
         "Demographic": NotRequired[EndpointDemographicTypeDef],
         "EffectiveDate": NotRequired[str],
         "EndpointStatus": NotRequired[str],
-        "Id": NotRequired[str],
         "Location": NotRequired[EndpointLocationTypeDef],
-        "Metrics": NotRequired[Dict[str, float]],
+        "Metrics": NotRequired[Mapping[str, float]],
         "OptOut": NotRequired[str],
         "RequestId": NotRequired[str],
-        "User": NotRequired[EndpointUserOutputTypeDef],
-    },
-)
-EventDimensionsOutputTypeDef = TypedDict(
-    "EventDimensionsOutputTypeDef",
-    {
-        "Attributes": NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],
-        "EventType": NotRequired[SetDimensionOutputTypeDef],
-        "Metrics": NotRequired[Dict[str, MetricDimensionTypeDef]],
+        "User": NotRequired[EndpointUserTypeDef],
     },
 )
-SegmentDemographicsOutputTypeDef = TypedDict(
-    "SegmentDemographicsOutputTypeDef",
+SendUsersMessageResponseTypeDef = TypedDict(
+    "SendUsersMessageResponseTypeDef",
     {
-        "AppVersion": NotRequired[SetDimensionOutputTypeDef],
-        "Channel": NotRequired[SetDimensionOutputTypeDef],
-        "DeviceType": NotRequired[SetDimensionOutputTypeDef],
-        "Make": NotRequired[SetDimensionOutputTypeDef],
-        "Model": NotRequired[SetDimensionOutputTypeDef],
-        "Platform": NotRequired[SetDimensionOutputTypeDef],
+        "ApplicationId": str,
+        "RequestId": NotRequired[str],
+        "Result": NotRequired[Dict[str, Dict[str, EndpointMessageResultTypeDef]]],
     },
 )
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": NotRequired[Mapping[str, AttributeDimensionTypeDef]],
         "EventType": NotRequired[SetDimensionTypeDef],
@@ -3373,18 +3261,25 @@
         "JourneyId": str,
         "JourneyStateRequest": JourneyStateRequestTypeDef,
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagsModel": TagsModelOutputTypeDef,
+        "TagsModel": TagsModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagsModel": TagsModelTypeDef,
+    },
+)
 MessageResponseTypeDef = TypedDict(
     "MessageResponseTypeDef",
     {
         "ApplicationId": str,
         "EndpointResult": NotRequired[Dict[str, EndpointMessageResultTypeDef]],
         "RequestId": NotRequired[str],
         "Result": NotRequired[Dict[str, MessageResultTypeDef]],
@@ -3399,24 +3294,14 @@
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-OpenHoursOutputTypeDef = TypedDict(
-    "OpenHoursOutputTypeDef",
-    {
-        "EMAIL": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "SMS": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "PUSH": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "VOICE": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-        "CUSTOM": NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],
-    },
-)
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
         "SMS": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
         "PUSH": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
         "VOICE": NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],
@@ -3426,20 +3311,14 @@
 PutEventStreamRequestRequestTypeDef = TypedDict(
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
-RandomSplitActivityOutputTypeDef = TypedDict(
-    "RandomSplitActivityOutputTypeDef",
-    {
-        "Branches": NotRequired[List[RandomSplitEntryTypeDef]],
-    },
-)
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": NotRequired[Sequence[RandomSplitEntryTypeDef]],
     },
 )
 SegmentBehaviorsTypeDef = TypedDict(
@@ -3479,25 +3358,16 @@
 )
 SimpleEmailTypeDef = TypedDict(
     "SimpleEmailTypeDef",
     {
         "HtmlPart": NotRequired[SimpleEmailPartTypeDef],
         "Subject": NotRequired[SimpleEmailPartTypeDef],
         "TextPart": NotRequired[SimpleEmailPartTypeDef],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagsModel": TagsModelTypeDef,
-    },
-)
-TagsModelUnionTypeDef = Union[TagsModelTypeDef, TagsModelOutputTypeDef]
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
@@ -3588,37 +3458,14 @@
         "CloudWatchMetricsEnabled": NotRequired[bool],
         "EventTaggingEnabled": NotRequired[bool],
         "Limits": NotRequired[CampaignLimitsTypeDef],
         "QuietTime": NotRequired[QuietTimeTypeDef],
         "JourneyLimits": NotRequired[ApplicationSettingsJourneyLimitsTypeDef],
     },
 )
-CreateEmailTemplateRequestRequestTypeDef = TypedDict(
-    "CreateEmailTemplateRequestRequestTypeDef",
-    {
-        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
-        "TemplateName": str,
-    },
-)
-UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
-    "UpdateEmailTemplateRequestRequestTypeDef",
-    {
-        "EmailTemplateRequest": EmailTemplateRequestTypeDef,
-        "TemplateName": str,
-        "CreateNewVersion": NotRequired[bool],
-        "Version": NotRequired[str],
-    },
-)
-GetEmailTemplateResponseTypeDef = TypedDict(
-    "GetEmailTemplateResponseTypeDef",
-    {
-        "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3662,21 +3509,14 @@
     "UpdateEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
         "EndpointRequest": EndpointRequestTypeDef,
     },
 )
-SendUsersMessagesResponseTypeDef = TypedDict(
-    "SendUsersMessagesResponseTypeDef",
-    {
-        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3689,33 +3529,19 @@
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CampaignEventFilterOutputTypeDef = TypedDict(
-    "CampaignEventFilterOutputTypeDef",
-    {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
-    },
-)
-EventConditionOutputTypeDef = TypedDict(
-    "EventConditionOutputTypeDef",
-    {
-        "Dimensions": NotRequired[EventDimensionsOutputTypeDef],
-        "MessageActivity": NotRequired[str],
-    },
-)
-EventFilterOutputTypeDef = TypedDict(
-    "EventFilterOutputTypeDef",
+SendUsersMessagesResponseTypeDef = TypedDict(
+    "SendUsersMessagesResponseTypeDef",
     {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
+        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
         "FilterType": FilterTypeType,
@@ -3765,21 +3591,14 @@
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SegmentLocationOutputTypeDef = TypedDict(
-    "SegmentLocationOutputTypeDef",
-    {
-        "Country": NotRequired[SetDimensionOutputTypeDef],
-        "GPSPoint": NotRequired[GPSPointDimensionTypeDef],
-    },
-)
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": NotRequired[SetDimensionTypeDef],
         "GPSPoint": NotRequired[GPSPointDimensionTypeDef],
     },
 )
@@ -3910,35 +3729,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": NotRequired[str],
-        "EventFilter": NotRequired[CampaignEventFilterOutputTypeDef],
-        "QuietTime": NotRequired[QuietTimeTypeDef],
-    },
-)
-ScheduleOutputTypeDef = TypedDict(
-    "ScheduleOutputTypeDef",
-    {
-        "StartTime": str,
-        "EndTime": NotRequired[str],
-        "EventFilter": NotRequired[CampaignEventFilterOutputTypeDef],
-        "Frequency": NotRequired[FrequencyType],
-        "IsLocalTime": NotRequired[bool],
+        "EventFilter": NotRequired[CampaignEventFilterTypeDef],
         "QuietTime": NotRequired[QuietTimeTypeDef],
-        "Timezone": NotRequired[str],
-    },
-)
-EventStartConditionOutputTypeDef = TypedDict(
-    "EventStartConditionOutputTypeDef",
-    {
-        "EventFilter": NotRequired[EventFilterOutputTypeDef],
-        "SegmentId": NotRequired[str],
     },
 )
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "StartTime": str,
         "EndTime": NotRequired[str],
@@ -3979,25 +3779,14 @@
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SegmentDimensionsOutputTypeDef = TypedDict(
-    "SegmentDimensionsOutputTypeDef",
-    {
-        "Attributes": NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],
-        "Behavior": NotRequired[SegmentBehaviorsTypeDef],
-        "Demographic": NotRequired[SegmentDemographicsOutputTypeDef],
-        "Location": NotRequired[SegmentLocationOutputTypeDef],
-        "Metrics": NotRequired[Dict[str, MetricDimensionTypeDef]],
-        "UserAttributes": NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],
-    },
-)
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": NotRequired[Mapping[str, AttributeDimensionTypeDef]],
         "Behavior": NotRequired[SegmentBehaviorsTypeDef],
         "Demographic": NotRequired[SegmentDemographicsTypeDef],
         "Location": NotRequired[SegmentLocationTypeDef],
@@ -4015,23 +3804,14 @@
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CampaignInAppMessageOutputTypeDef = TypedDict(
-    "CampaignInAppMessageOutputTypeDef",
-    {
-        "Body": NotRequired[str],
-        "Content": NotRequired[List[InAppMessageContentTypeDef]],
-        "CustomConfig": NotRequired[Dict[str, str]],
-        "Layout": NotRequired[LayoutType],
-    },
-)
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": NotRequired[str],
         "Content": NotRequired[Sequence[InAppMessageContentTypeDef]],
         "CustomConfig": NotRequired[Mapping[str, str]],
         "Layout": NotRequired[LayoutType],
@@ -4116,22 +3896,14 @@
         "DefaultPushNotificationMessage": NotRequired[DefaultPushNotificationMessageTypeDef],
         "EmailMessage": NotRequired[EmailMessageTypeDef],
         "GCMMessage": NotRequired[GCMMessageTypeDef],
         "SMSMessage": NotRequired[SMSMessageTypeDef],
         "VoiceMessage": NotRequired[VoiceMessageTypeDef],
     },
 )
-StartConditionOutputTypeDef = TypedDict(
-    "StartConditionOutputTypeDef",
-    {
-        "Description": NotRequired[str],
-        "EventStartCondition": NotRequired[EventStartConditionOutputTypeDef],
-        "SegmentStartCondition": NotRequired[SegmentConditionTypeDef],
-    },
-)
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
         "Description": NotRequired[str],
         "EventStartCondition": NotRequired[EventStartConditionTypeDef],
         "SegmentStartCondition": NotRequired[SegmentConditionTypeDef],
     },
@@ -4139,31 +3911,14 @@
 PutEventsRequestRequestTypeDef = TypedDict(
     "PutEventsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EventsRequest": EventsRequestTypeDef,
     },
 )
-SegmentGroupOutputTypeDef = TypedDict(
-    "SegmentGroupOutputTypeDef",
-    {
-        "Dimensions": NotRequired[List[SegmentDimensionsOutputTypeDef]],
-        "SourceSegments": NotRequired[List[SegmentReferenceTypeDef]],
-        "SourceType": NotRequired[SourceTypeType],
-        "Type": NotRequired[TypeType],
-    },
-)
-SimpleConditionOutputTypeDef = TypedDict(
-    "SimpleConditionOutputTypeDef",
-    {
-        "EventCondition": NotRequired[EventConditionOutputTypeDef],
-        "SegmentCondition": NotRequired[SegmentConditionTypeDef],
-        "SegmentDimensions": NotRequired[SegmentDimensionsOutputTypeDef],
-    },
-)
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
     {
         "Dimensions": NotRequired[Sequence[SegmentDimensionsTypeDef]],
         "SourceSegments": NotRequired[Sequence[SegmentReferenceTypeDef]],
         "SourceType": NotRequired[SourceTypeType],
         "Type": NotRequired[TypeType],
@@ -4173,28 +3928,14 @@
     "SimpleConditionTypeDef",
     {
         "EventCondition": NotRequired[EventConditionTypeDef],
         "SegmentCondition": NotRequired[SegmentConditionTypeDef],
         "SegmentDimensions": NotRequired[SegmentDimensionsTypeDef],
     },
 )
-MessageConfigurationOutputTypeDef = TypedDict(
-    "MessageConfigurationOutputTypeDef",
-    {
-        "ADMMessage": NotRequired[MessageTypeDef],
-        "APNSMessage": NotRequired[MessageTypeDef],
-        "BaiduMessage": NotRequired[MessageTypeDef],
-        "CustomMessage": NotRequired[CampaignCustomMessageTypeDef],
-        "DefaultMessage": NotRequired[MessageTypeDef],
-        "EmailMessage": NotRequired[CampaignEmailMessageOutputTypeDef],
-        "GCMMessage": NotRequired[MessageTypeDef],
-        "SMSMessage": NotRequired[CampaignSmsMessageTypeDef],
-        "InAppMessage": NotRequired[CampaignInAppMessageOutputTypeDef],
-    },
-)
 MessageConfigurationTypeDef = TypedDict(
     "MessageConfigurationTypeDef",
     {
         "ADMMessage": NotRequired[MessageTypeDef],
         "APNSMessage": NotRequired[MessageTypeDef],
         "BaiduMessage": NotRequired[MessageTypeDef],
         "CustomMessage": NotRequired[CampaignCustomMessageTypeDef],
@@ -4279,35 +4020,14 @@
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
         "Context": NotRequired[Mapping[str, str]],
         "TemplateConfiguration": NotRequired[TemplateConfigurationTypeDef],
         "TraceId": NotRequired[str],
     },
 )
-SegmentGroupListOutputTypeDef = TypedDict(
-    "SegmentGroupListOutputTypeDef",
-    {
-        "Groups": NotRequired[List[SegmentGroupOutputTypeDef]],
-        "Include": NotRequired[IncludeType],
-    },
-)
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "Conditions": NotRequired[List[SimpleConditionOutputTypeDef]],
-        "Operator": NotRequired[OperatorType],
-    },
-)
-MultiConditionalBranchOutputTypeDef = TypedDict(
-    "MultiConditionalBranchOutputTypeDef",
-    {
-        "Condition": NotRequired[SimpleConditionOutputTypeDef],
-        "NextActivity": NotRequired[str],
-    },
-)
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": NotRequired[Sequence[SegmentGroupTypeDef]],
         "Include": NotRequired[IncludeType],
     },
 )
@@ -4326,17 +4046,17 @@
     },
 )
 TreatmentResourceTypeDef = TypedDict(
     "TreatmentResourceTypeDef",
     {
         "Id": str,
         "SizePercent": int,
-        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationOutputTypeDef],
-        "MessageConfiguration": NotRequired[MessageConfigurationOutputTypeDef],
-        "Schedule": NotRequired[ScheduleOutputTypeDef],
+        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationTypeDef],
+        "MessageConfiguration": NotRequired[MessageConfigurationTypeDef],
+        "Schedule": NotRequired[ScheduleTypeDef],
         "State": NotRequired[CampaignStateTypeDef],
         "TemplateConfiguration": NotRequired[TemplateConfigurationTypeDef],
         "TreatmentDescription": NotRequired[str],
         "TreatmentName": NotRequired[str],
     },
 )
 WriteTreatmentResourceTypeDef = TypedDict(
@@ -4375,40 +4095,23 @@
     "SegmentResponseTypeDef",
     {
         "ApplicationId": str,
         "Arn": str,
         "CreationDate": str,
         "Id": str,
         "SegmentType": SegmentTypeType,
-        "Dimensions": NotRequired[SegmentDimensionsOutputTypeDef],
+        "Dimensions": NotRequired[SegmentDimensionsTypeDef],
         "ImportDefinition": NotRequired[SegmentImportResourceTypeDef],
         "LastModifiedDate": NotRequired[str],
         "Name": NotRequired[str],
-        "SegmentGroups": NotRequired[SegmentGroupListOutputTypeDef],
+        "SegmentGroups": NotRequired[SegmentGroupListTypeDef],
         "tags": NotRequired[Dict[str, str]],
         "Version": NotRequired[int],
     },
 )
-ConditionalSplitActivityOutputTypeDef = TypedDict(
-    "ConditionalSplitActivityOutputTypeDef",
-    {
-        "Condition": NotRequired[ConditionOutputTypeDef],
-        "EvaluationWaitTime": NotRequired[WaitTimeTypeDef],
-        "FalseActivity": NotRequired[str],
-        "TrueActivity": NotRequired[str],
-    },
-)
-MultiConditionalSplitActivityOutputTypeDef = TypedDict(
-    "MultiConditionalSplitActivityOutputTypeDef",
-    {
-        "Branches": NotRequired[List[MultiConditionalBranchOutputTypeDef]],
-        "DefaultActivity": NotRequired[str],
-        "EvaluationWaitTime": NotRequired[WaitTimeTypeDef],
-    },
-)
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": NotRequired[SegmentDimensionsTypeDef],
         "Name": NotRequired[str],
         "SegmentGroups": NotRequired[SegmentGroupListTypeDef],
         "tags": NotRequired[Mapping[str, str]],
@@ -4438,24 +4141,24 @@
         "Arn": str,
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "SegmentId": str,
         "SegmentVersion": int,
         "AdditionalTreatments": NotRequired[List[TreatmentResourceTypeDef]],
-        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationOutputTypeDef],
+        "CustomDeliveryConfiguration": NotRequired[CustomDeliveryConfigurationTypeDef],
         "DefaultState": NotRequired[CampaignStateTypeDef],
         "Description": NotRequired[str],
         "HoldoutPercent": NotRequired[int],
         "Hook": NotRequired[CampaignHookTypeDef],
         "IsPaused": NotRequired[bool],
         "Limits": NotRequired[CampaignLimitsTypeDef],
-        "MessageConfiguration": NotRequired[MessageConfigurationOutputTypeDef],
+        "MessageConfiguration": NotRequired[MessageConfigurationTypeDef],
         "Name": NotRequired[str],
-        "Schedule": NotRequired[ScheduleOutputTypeDef],
+        "Schedule": NotRequired[ScheduleTypeDef],
         "State": NotRequired[CampaignStateTypeDef],
         "tags": NotRequired[Dict[str, str]],
         "TemplateConfiguration": NotRequired[TemplateConfigurationTypeDef],
         "TreatmentDescription": NotRequired[str],
         "TreatmentName": NotRequired[str],
         "Version": NotRequired[int],
         "Priority": NotRequired[int],
@@ -4528,30 +4231,14 @@
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ActivityOutputTypeDef = TypedDict(
-    "ActivityOutputTypeDef",
-    {
-        "CUSTOM": NotRequired[CustomMessageActivityOutputTypeDef],
-        "ConditionalSplit": NotRequired[ConditionalSplitActivityOutputTypeDef],
-        "Description": NotRequired[str],
-        "EMAIL": NotRequired[EmailMessageActivityTypeDef],
-        "Holdout": NotRequired[HoldoutActivityTypeDef],
-        "MultiCondition": NotRequired[MultiConditionalSplitActivityOutputTypeDef],
-        "PUSH": NotRequired[PushMessageActivityTypeDef],
-        "RandomSplit": NotRequired[RandomSplitActivityOutputTypeDef],
-        "SMS": NotRequired[SMSMessageActivityTypeDef],
-        "Wait": NotRequired[WaitActivityTypeDef],
-        "ContactCenter": NotRequired[ContactCenterActivityTypeDef],
-    },
-)
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteSegmentRequest": WriteSegmentRequestTypeDef,
     },
 )
@@ -4652,32 +4339,32 @@
 )
 JourneyResponseTypeDef = TypedDict(
     "JourneyResponseTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
-        "Activities": NotRequired[Dict[str, ActivityOutputTypeDef]],
+        "Activities": NotRequired[Dict[str, ActivityTypeDef]],
         "CreationDate": NotRequired[str],
         "LastModifiedDate": NotRequired[str],
         "Limits": NotRequired[JourneyLimitsTypeDef],
         "LocalTime": NotRequired[bool],
         "QuietTime": NotRequired[QuietTimeTypeDef],
         "RefreshFrequency": NotRequired[str],
-        "Schedule": NotRequired[JourneyScheduleOutputTypeDef],
+        "Schedule": NotRequired[JourneyScheduleTypeDef],
         "StartActivity": NotRequired[str],
-        "StartCondition": NotRequired[StartConditionOutputTypeDef],
+        "StartCondition": NotRequired[StartConditionTypeDef],
         "State": NotRequired[StateType],
         "tags": NotRequired[Dict[str, str]],
         "WaitForQuietTime": NotRequired[bool],
         "RefreshOnSegmentUpdate": NotRequired[bool],
         "JourneyChannelSettings": NotRequired[JourneyChannelSettingsTypeDef],
         "SendingSchedule": NotRequired[bool],
-        "OpenHours": NotRequired[OpenHoursOutputTypeDef],
-        "ClosedDays": NotRequired[ClosedDaysOutputTypeDef],
+        "OpenHours": NotRequired[OpenHoursTypeDef],
+        "ClosedDays": NotRequired[ClosedDaysTypeDef],
         "TimezoneEstimationMethods": NotRequired[List[TimezoneEstimationMethodsElementType]],
     },
 )
 WriteJourneyRequestTypeDef = TypedDict(
     "WriteJourneyRequestTypeDef",
     {
         "Name": str,
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.34.102
-Summary: Type annotations for boto3.Pinpoint 1.34.102 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.81
+Summary: Type annotations for boto3.Pinpoint 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.34.102](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_pinpoint-1.34.102/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_pinpoint-1.34.102/setup.py` & `mypy-boto3-pinpoint-1.34.81/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.34.102",
+    version="1.34.81",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Pinpoint 1.34.102 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.Pinpoint 1.34.81 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

