# Comparing `tmp/cdklabs.cdk-verified-permissions-0.0.1a7.tar.gz` & `tmp/cdklabs.cdk-verified-permissions-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-verified-permissions-0.0.1a7.tar", last modified: Mon Apr 29 10:42:59 2024, max compression
+gzip compressed data, was "cdklabs.cdk-verified-permissions-0.0.1a8.tar", last modified: Fri May 10 09:02:26 2024, max compression
```

## Comparing `cdklabs.cdk-verified-permissions-0.0.1a7.tar` & `cdklabs.cdk-verified-permissions-0.0.1a8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:42:59.782721 cdklabs.cdk-verified-permissions-0.0.1a7/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-29 10:42:59.782721 cdklabs.cdk-verified-permissions-0.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:42:59.782721 cdklabs.cdk-verified-permissions-0.0.1a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:42:59.778721 cdklabs.cdk-verified-permissions-0.0.1a7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:42:59.778721 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:42:59.782721 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/
--rw-r--r--   0 runner    (1001) docker     (127)   107624 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:42:59.782721 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55598 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:42:47.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:42:59.782721 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-29 10:42:59.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-29 10:42:59.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:42:59.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 10:42:59.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 10:42:59.000000 cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:02:26.519083 cdklabs.cdk-verified-permissions-0.0.1a8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-10 09:02:26.519083 cdklabs.cdk-verified-permissions-0.0.1a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:02:26.519083 cdklabs.cdk-verified-permissions-0.0.1a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:02:26.515083 cdklabs.cdk-verified-permissions-0.0.1a8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:02:26.515083 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:02:26.519083 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)   111252 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:02:26.519083 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56531 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:02:13.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:02:26.515083 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-10 09:02:26.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-10 09:02:26.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:02:26.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-10 09:02:26.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:02:26.000000 cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/LICENSE` & `cdklabs.cdk-verified-permissions-0.0.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/PKG-INFO` & `cdklabs.cdk-verified-permissions-0.0.1a8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-verified-permissions
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: L2 AWS CDK Constructs for Amazon Verified Permissions
 Home-page: https://github.com/cdklabs/cdk-verified-permissions.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-verified-permissions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -165,20 +165,24 @@
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
     validation_settings=validation_settings_strict
 )
+cognito_group_entity_type = "test"
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             client_ids=["&ExampleCogClientId;"],
-            user_pool=user_pool
+            user_pool=user_pool,
+            group_configuration=CognitoGroupConfiguration(
+                group_entity_type=cognito_group_entity_type
+            )
         )
     ),
     policy_store=policy_store,
     principal_entity_type="PETEXAMPLEabcdefg111111"
 )
 ```
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/README.md` & `cdklabs.cdk-verified-permissions-0.0.1a8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,20 +141,24 @@
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
     validation_settings=validation_settings_strict
 )
+cognito_group_entity_type = "test"
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             client_ids=["&ExampleCogClientId;"],
-            user_pool=user_pool
+            user_pool=user_pool,
+            group_configuration=CognitoGroupConfiguration(
+                group_entity_type=cognito_group_entity_type
+            )
         )
     ),
     policy_store=policy_store,
     principal_entity_type="PETEXAMPLEabcdefg111111"
 )
 ```
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/setup.py` & `cdklabs.cdk-verified-permissions-0.0.1a8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-verified-permissions",
-    "version": "0.0.1.a7",
+    "version": "0.0.1.a8",
     "description": "L2 AWS CDK Constructs for Amazon Verified Permissions",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-verified-permissions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdklabs.cdk_verified_permissions",
         "cdklabs.cdk_verified_permissions._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_verified_permissions._jsii": [
-            "cdk-verified-permissions@0.0.1-alpha.7.jsii.tgz"
+            "cdk-verified-permissions@0.0.1-alpha.8.jsii.tgz"
         ],
         "cdklabs.cdk_verified_permissions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.139.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/__init__.py` & `cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,20 +142,24 @@
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
     validation_settings=validation_settings_strict
 )
+cognito_group_entity_type = "test"
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             client_ids=["&ExampleCogClientId;"],
-            user_pool=user_pool
+            user_pool=user_pool,
+            group_configuration=CognitoGroupConfiguration(
+                group_entity_type=cognito_group_entity_type
+            )
         )
     ),
     policy_store=policy_store,
     principal_entity_type="PETEXAMPLEabcdefg111111"
 )
 ```
 
@@ -360,40 +364,92 @@
     def __repr__(self) -> str:
         return "AddPolicyOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="@cdklabs/cdk-verified-permissions.CognitoGroupConfiguration",
+    jsii_struct_bases=[],
+    name_mapping={"group_entity_type": "groupEntityType"},
+)
+class CognitoGroupConfiguration:
+    def __init__(self, *, group_entity_type: builtins.str) -> None:
+        '''
+        :param group_entity_type: (experimental) The name of the schema entity type that's mapped to the user pool group.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f2f9c1387675a8fdb59b6473754c70d80fdbd3a887cc2234938f0a70f1aa560e)
+            check_type(argname="argument group_entity_type", value=group_entity_type, expected_type=type_hints["group_entity_type"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "group_entity_type": group_entity_type,
+        }
+
+    @builtins.property
+    def group_entity_type(self) -> builtins.str:
+        '''(experimental) The name of the schema entity type that's mapped to the user pool group.
+
+        :stability: experimental
+        '''
+        result = self._values.get("group_entity_type")
+        assert result is not None, "Required property 'group_entity_type' is missing"
+        return typing.cast(builtins.str, result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "CognitoGroupConfiguration(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="@cdklabs/cdk-verified-permissions.CognitoUserPoolConfiguration",
     jsii_struct_bases=[],
-    name_mapping={"user_pool": "userPool", "client_ids": "clientIds"},
+    name_mapping={
+        "user_pool": "userPool",
+        "client_ids": "clientIds",
+        "group_configuration": "groupConfiguration",
+    },
 )
 class CognitoUserPoolConfiguration:
     def __init__(
         self,
         *,
         user_pool: _aws_cdk_aws_cognito_ceddda9d.IUserPool,
         client_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
+        group_configuration: typing.Optional[typing.Union[CognitoGroupConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param user_pool: (experimental) Cognito User Pool. Default: - no Cognito User Pool
         :param client_ids: (experimental) Client identifiers. Default: - empty list.
+        :param group_configuration: (experimental) Cognito Group Configuration. Default: - no Cognito Group configuration provided
 
         :stability: experimental
         '''
+        if isinstance(group_configuration, dict):
+            group_configuration = CognitoGroupConfiguration(**group_configuration)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ca5911da207441ba7e1b4d34d96a47a7c703f02f20a0f129103da2d7d3c147bc)
             check_type(argname="argument user_pool", value=user_pool, expected_type=type_hints["user_pool"])
             check_type(argname="argument client_ids", value=client_ids, expected_type=type_hints["client_ids"])
+            check_type(argname="argument group_configuration", value=group_configuration, expected_type=type_hints["group_configuration"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "user_pool": user_pool,
         }
         if client_ids is not None:
             self._values["client_ids"] = client_ids
+        if group_configuration is not None:
+            self._values["group_configuration"] = group_configuration
 
     @builtins.property
     def user_pool(self) -> _aws_cdk_aws_cognito_ceddda9d.IUserPool:
         '''(experimental) Cognito User Pool.
 
         :default: - no Cognito User Pool
 
@@ -410,14 +466,25 @@
         :default: - empty list.
 
         :stability: experimental
         '''
         result = self._values.get("client_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
+    @builtins.property
+    def group_configuration(self) -> typing.Optional[CognitoGroupConfiguration]:
+        '''(experimental) Cognito Group Configuration.
+
+        :default: - no Cognito Group configuration provided
+
+        :stability: experimental
+        '''
+        result = self._values.get("group_configuration")
+        return typing.cast(typing.Optional[CognitoGroupConfiguration], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1101,14 +1168,22 @@
     @jsii.member(jsii_name="userPoolArn")
     def user_pool_arn(self) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "userPoolArn"))
 
+    @builtins.property
+    @jsii.member(jsii_name="cognitoGroupEntityType")
+    def cognito_group_entity_type(self) -> typing.Optional[builtins.str]:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "cognitoGroupEntityType"))
+
 
 @jsii.data_type(
     jsii_type="@cdklabs/cdk-verified-permissions.IdentitySourceAttributes",
     jsii_struct_bases=[],
     name_mapping={
         "identity_source_arn": "identitySourceArn",
         "identity_source_id": "identitySourceId",
@@ -2497,14 +2572,15 @@
     '''
     :stability: experimental
     '''
 
 
 __all__ = [
     "AddPolicyOptions",
+    "CognitoGroupConfiguration",
     "CognitoUserPoolConfiguration",
     "EntityIdentifierProperty",
     "IIdentitySource",
     "IPolicy",
     "IPolicyStore",
     "IPolicyTemplate",
     "ISchema",
@@ -2536,18 +2612,26 @@
     *,
     policy_configuration: typing.Union[PolicyDefinitionProperty, typing.Dict[builtins.str, typing.Any]],
     policy_id: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__f2f9c1387675a8fdb59b6473754c70d80fdbd3a887cc2234938f0a70f1aa560e(
+    *,
+    group_entity_type: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__ca5911da207441ba7e1b4d34d96a47a7c703f02f20a0f129103da2d7d3c147bc(
     *,
     user_pool: _aws_cdk_aws_cognito_ceddda9d.IUserPool,
     client_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
+    group_configuration: typing.Optional[typing.Union[CognitoGroupConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__aaa2b8143bc6c28b8f73dd964f712a25298be8ecd5d95a23ca2ef7f66953d41d(
     *,
     entity_id: builtins.str,
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py` & `cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/cdk-verified-permissions",
-    "0.0.1-alpha.7",
+    "0.0.1-alpha.8",
     __name__[0:-6],
-    "cdk-verified-permissions@0.0.1-alpha.7.jsii.tgz",
+    "cdk-verified-permissions@0.0.1-alpha.8.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO` & `cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-verified-permissions
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: L2 AWS CDK Constructs for Amazon Verified Permissions
 Home-page: https://github.com/cdklabs/cdk-verified-permissions.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-verified-permissions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -165,20 +165,24 @@
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
     validation_settings=validation_settings_strict
 )
+cognito_group_entity_type = "test"
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             client_ids=["&ExampleCogClientId;"],
-            user_pool=user_pool
+            user_pool=user_pool,
+            group_configuration=CognitoGroupConfiguration(
+                group_entity_type=cognito_group_entity_type
+            )
         )
     ),
     policy_store=policy_store,
     principal_entity_type="PETEXAMPLEabcdefg111111"
 )
 ```
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a7/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt` & `cdklabs.cdk-verified-permissions-0.0.1a8/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
 src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
 src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
 src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
 src/cdklabs/cdk_verified_permissions/__init__.py
 src/cdklabs/cdk_verified_permissions/py.typed
 src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
-src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.7.jsii.tgz
+src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.8.jsii.tgz
```

