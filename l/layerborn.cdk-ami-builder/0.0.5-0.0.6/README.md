# Comparing `tmp/layerborn.cdk-ami-builder-0.0.5.tar.gz` & `tmp/layerborn.cdk-ami-builder-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layerborn.cdk-ami-builder-0.0.5.tar", last modified: Wed Feb  7 03:23:07 2024, max compression
+gzip compressed data, was "layerborn.cdk-ami-builder-0.0.6.tar", last modified: Fri May 10 15:08:29 2024, max compression
```

## Comparing `layerborn.cdk-ami-builder-0.0.5.tar` & `layerborn.cdk-ami-builder-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 03:23:07.585938 layerborn.cdk-ami-builder-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-02-07 03:23:07.585938 layerborn.cdk-ami-builder-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 03:23:07.585938 layerborn.cdk-ami-builder-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 03:23:07.577937 layerborn.cdk-ami-builder-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 03:23:07.577937 layerborn.cdk-ami-builder-0.0.5/src/layerborn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 03:23:07.581937 layerborn.cdk-ami-builder-0.0.5/src/layerborn/cdk_ami_builder/
--rw-r--r--   0 runner    (1001) docker     (127)   218456 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn/cdk_ami_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 03:23:07.581937 layerborn.cdk-ami-builder-0.0.5/src/layerborn/cdk_ami_builder/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn/cdk_ami_builder/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  4249270 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn/cdk_ami_builder/_jsii/cdk-ami-builder@0.0.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 03:22:53.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn/cdk_ami_builder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 03:23:07.577937 layerborn.cdk-ami-builder-0.0.5/src/layerborn.cdk_ami_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-02-07 03:23:07.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn.cdk_ami_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-07 03:23:07.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn.cdk_ami_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 03:23:07.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn.cdk_ami_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-07 03:23:07.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn.cdk_ami_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-07 03:23:07.000000 layerborn.cdk-ami-builder-0.0.5/src/layerborn.cdk_ami_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:29.172499 layerborn.cdk-ami-builder-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-10 15:08:29.172499 layerborn.cdk-ami-builder-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:08:29.172499 layerborn.cdk-ami-builder-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:29.164499 layerborn.cdk-ami-builder-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:29.164499 layerborn.cdk-ami-builder-0.0.6/src/layerborn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:29.168499 layerborn.cdk-ami-builder-0.0.6/src/layerborn/cdk_ami_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)   224034 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn/cdk_ami_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:29.168499 layerborn.cdk-ami-builder-0.0.6/src/layerborn/cdk_ami_builder/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn/cdk_ami_builder/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4277579 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn/cdk_ami_builder/_jsii/cdk-ami-builder@0.0.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:08:16.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn/cdk_ami_builder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:29.168499 layerborn.cdk-ami-builder-0.0.6/src/layerborn.cdk_ami_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-10 15:08:29.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn.cdk_ami_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-10 15:08:29.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn.cdk_ami_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:08:29.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn.cdk_ami_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 15:08:29.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn.cdk_ami_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 15:08:29.000000 layerborn.cdk-ami-builder-0.0.6/src/layerborn.cdk_ami_builder.egg-info/top_level.txt
```

### Comparing `layerborn.cdk-ami-builder-0.0.5/LICENSE` & `layerborn.cdk-ami-builder-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `layerborn.cdk-ami-builder-0.0.5/PKG-INFO` & `layerborn.cdk-ami-builder-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerborn.cdk-ami-builder
-Version: 0.0.5
+Version: 0.0.6
 Summary: Creates an EC2 AMI using an Image Builder Pipeline and returns the AMI ID.
 Home-page: https://github.com/layerborn/cdk-ami-builder-construct.git
 Author: Jayson Rawlins<jayson.rawlins@layerborn.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/layerborn/cdk-ami-builder-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `layerborn.cdk-ami-builder-0.0.5/README.md` & `layerborn.cdk-ami-builder-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `layerborn.cdk-ami-builder-0.0.5/setup.py` & `layerborn.cdk-ami-builder-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "layerborn.cdk-ami-builder",
-    "version": "0.0.5",
+    "version": "0.0.6",
     "description": "Creates an EC2 AMI using an Image Builder Pipeline and returns the AMI ID.",
     "license": "Apache-2.0",
     "url": "https://github.com/layerborn/cdk-ami-builder-construct.git",
     "long_description_content_type": "text/markdown",
     "author": "Jayson Rawlins<jayson.rawlins@layerborn.io>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "layerborn.cdk_ami_builder",
         "layerborn.cdk_ami_builder._jsii"
     ],
     "package_data": {
         "layerborn.cdk_ami_builder._jsii": [
-            "cdk-ami-builder@0.0.5.jsii.tgz"
+            "cdk-ami-builder@0.0.6.jsii.tgz"
         ],
         "layerborn.cdk_ami_builder": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.100.0, <3.0.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.94.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "layerborn.cdk-iam-policy-builder-helper>=0.0.4, <0.0.5",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `layerborn.cdk-ami-builder-0.0.5/src/layerborn/cdk_ami_builder/__init__.py` & `layerborn.cdk-ami-builder-0.0.6/src/layerborn/cdk_ami_builder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,17 @@
 
 
 This README provides a basic guide to getting started with the `ImagePipeline` construct. For more advanced usage and
 customization, refer to the detailed documentation in the package.
 
 ![User](https://lh3.googleusercontent.com/a/AEdFTp6yNsN1-EC5-OZ2vss91NDDYmHKgEHn8xwdd6eS=s96-c)
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -215,16 +218,18 @@
         environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
         events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
         filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
         function_name: typing.Optional[builtins.str] = None,
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+        ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_format: typing.Optional[builtins.str] = None,
+        logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
         log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
         params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
@@ -262,16 +267,18 @@
         :param environment_encryption: The AWS KMS key that's used to encrypt your function's environment variables. Default: - AWS Lambda creates and uses an AWS managed customer master key (CMK).
         :param ephemeral_storage_size: The size of the function’s /tmp directory in MiB. Default: 512 MiB
         :param events: Event sources for this function. You can also add event sources using ``addEventSource``. Default: - No event sources.
         :param filesystem: The filesystem configuration for the lambda function. Default: - will not mount any filesystem
         :param function_name: A name for the function. Default: - AWS CloudFormation generates a unique physical ID and uses that ID for the function's name. For more information, see Name Type.
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
+        :param ipv6_allowed_for_dual_stack: Allows outbound IPv6 traffic on VPC functions that are connected to dual-stack subnets. Only used if 'vpc' is supplied. Default: false
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_format: Sets the logFormat for the function. Default: "Text"
+        :param logging_format: Sets the loggingFormat for the function. Default: LoggingFormat.TEXT
         :param log_group: The log group the function sends logs to. By default, Lambda functions send logs to an automatically created default log group named /aws/lambda/<function name>. However you cannot change the properties of this auto-created log group using the AWS CDK, e.g. you cannot set a different log retention. Use the ``logGroup`` property to create a fully customizable LogGroup ahead of time, and instruct the Lambda function to send logs to it. Providing a user-controlled log group was rolled out to commercial regions on 2023-11-16. If you are deploying to another type of region, please check regional availability first. Default: ``/aws/lambda/${this.functionName}`` - default log group created by Lambda
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. This is a legacy API and we strongly recommend you move away from it if you can. Instead create a fully customizable log group with ``logs.LogGroup`` and use the ``logGroup`` property to instruct the Lambda function to send logs to it. Migrating from ``logRetention`` to ``logGroup`` will cause the name of the log group to change. Users and code and referencing the name verbatim will have to adjust. In AWS CDK code, you can access the log group name directly from the LogGroup construct:: import * as logs from 'aws-cdk-lib/aws-logs'; declare const myLogGroup: logs.LogGroup; myLogGroup.logGroupName; Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
         :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
@@ -311,16 +318,18 @@
             environment_encryption=environment_encryption,
             ephemeral_storage_size=ephemeral_storage_size,
             events=events,
             filesystem=filesystem,
             function_name=function_name,
             initial_policy=initial_policy,
             insights_version=insights_version,
+            ipv6_allowed_for_dual_stack=ipv6_allowed_for_dual_stack,
             layers=layers,
             log_format=log_format,
+            logging_format=logging_format,
             log_group=log_group,
             log_retention=log_retention,
             log_retention_retry_options=log_retention_retry_options,
             log_retention_role=log_retention_role,
             memory_size=memory_size,
             params_and_secrets=params_and_secrets,
             profiling=profiling,
@@ -367,16 +376,18 @@
         "environment_encryption": "environmentEncryption",
         "ephemeral_storage_size": "ephemeralStorageSize",
         "events": "events",
         "filesystem": "filesystem",
         "function_name": "functionName",
         "initial_policy": "initialPolicy",
         "insights_version": "insightsVersion",
+        "ipv6_allowed_for_dual_stack": "ipv6AllowedForDualStack",
         "layers": "layers",
         "log_format": "logFormat",
+        "logging_format": "loggingFormat",
         "log_group": "logGroup",
         "log_retention": "logRetention",
         "log_retention_retry_options": "logRetentionRetryOptions",
         "log_retention_role": "logRetentionRole",
         "memory_size": "memorySize",
         "params_and_secrets": "paramsAndSecrets",
         "profiling": "profiling",
@@ -418,16 +429,18 @@
         environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
         events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
         filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
         function_name: typing.Optional[builtins.str] = None,
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+        ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_format: typing.Optional[builtins.str] = None,
+        logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
         log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
         params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
@@ -464,16 +477,18 @@
         :param environment_encryption: The AWS KMS key that's used to encrypt your function's environment variables. Default: - AWS Lambda creates and uses an AWS managed customer master key (CMK).
         :param ephemeral_storage_size: The size of the function’s /tmp directory in MiB. Default: 512 MiB
         :param events: Event sources for this function. You can also add event sources using ``addEventSource``. Default: - No event sources.
         :param filesystem: The filesystem configuration for the lambda function. Default: - will not mount any filesystem
         :param function_name: A name for the function. Default: - AWS CloudFormation generates a unique physical ID and uses that ID for the function's name. For more information, see Name Type.
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
+        :param ipv6_allowed_for_dual_stack: Allows outbound IPv6 traffic on VPC functions that are connected to dual-stack subnets. Only used if 'vpc' is supplied. Default: false
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_format: Sets the logFormat for the function. Default: "Text"
+        :param logging_format: Sets the loggingFormat for the function. Default: LoggingFormat.TEXT
         :param log_group: The log group the function sends logs to. By default, Lambda functions send logs to an automatically created default log group named /aws/lambda/<function name>. However you cannot change the properties of this auto-created log group using the AWS CDK, e.g. you cannot set a different log retention. Use the ``logGroup`` property to create a fully customizable LogGroup ahead of time, and instruct the Lambda function to send logs to it. Providing a user-controlled log group was rolled out to commercial regions on 2023-11-16. If you are deploying to another type of region, please check regional availability first. Default: ``/aws/lambda/${this.functionName}`` - default log group created by Lambda
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. This is a legacy API and we strongly recommend you move away from it if you can. Instead create a fully customizable log group with ``logs.LogGroup`` and use the ``logGroup`` property to instruct the Lambda function to send logs to it. Migrating from ``logRetention`` to ``logGroup`` will cause the name of the log group to change. Users and code and referencing the name verbatim will have to adjust. In AWS CDK code, you can access the log group name directly from the LogGroup construct:: import * as logs from 'aws-cdk-lib/aws-logs'; declare const myLogGroup: logs.LogGroup; myLogGroup.logGroupName; Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
         :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
@@ -518,16 +533,18 @@
             check_type(argname="argument environment_encryption", value=environment_encryption, expected_type=type_hints["environment_encryption"])
             check_type(argname="argument ephemeral_storage_size", value=ephemeral_storage_size, expected_type=type_hints["ephemeral_storage_size"])
             check_type(argname="argument events", value=events, expected_type=type_hints["events"])
             check_type(argname="argument filesystem", value=filesystem, expected_type=type_hints["filesystem"])
             check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
             check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
             check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
+            check_type(argname="argument ipv6_allowed_for_dual_stack", value=ipv6_allowed_for_dual_stack, expected_type=type_hints["ipv6_allowed_for_dual_stack"])
             check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
             check_type(argname="argument log_format", value=log_format, expected_type=type_hints["log_format"])
+            check_type(argname="argument logging_format", value=logging_format, expected_type=type_hints["logging_format"])
             check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
             check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
             check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
             check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
             check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
             check_type(argname="argument params_and_secrets", value=params_and_secrets, expected_type=type_hints["params_and_secrets"])
             check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
@@ -585,18 +602,22 @@
             self._values["filesystem"] = filesystem
         if function_name is not None:
             self._values["function_name"] = function_name
         if initial_policy is not None:
             self._values["initial_policy"] = initial_policy
         if insights_version is not None:
             self._values["insights_version"] = insights_version
+        if ipv6_allowed_for_dual_stack is not None:
+            self._values["ipv6_allowed_for_dual_stack"] = ipv6_allowed_for_dual_stack
         if layers is not None:
             self._values["layers"] = layers
         if log_format is not None:
             self._values["log_format"] = log_format
+        if logging_format is not None:
+            self._values["logging_format"] = logging_format
         if log_group is not None:
             self._values["log_group"] = log_group
         if log_retention is not None:
             self._values["log_retention"] = log_retention
         if log_retention_retry_options is not None:
             self._values["log_retention_retry_options"] = log_retention_retry_options
         if log_retention_role is not None:
@@ -889,14 +910,25 @@
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Lambda-Insights-Getting-Started-docker.html
         '''
         result = self._values.get("insights_version")
         return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion], result)
 
     @builtins.property
+    def ipv6_allowed_for_dual_stack(self) -> typing.Optional[builtins.bool]:
+        '''Allows outbound IPv6 traffic on VPC functions that are connected to dual-stack subnets.
+
+        Only used if 'vpc' is supplied.
+
+        :default: false
+        '''
+        result = self._values.get("ipv6_allowed_for_dual_stack")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def layers(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]]:
         '''A list of layers to add to the function's execution environment.
 
         You can configure your Lambda function to pull in
         additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies
@@ -913,14 +945,25 @@
 
         :default: "Text"
         '''
         result = self._values.get("log_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def logging_format(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat]:
+        '''Sets the loggingFormat for the function.
+
+        :default: LoggingFormat.TEXT
+        '''
+        result = self._values.get("logging_format")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat], result)
+
+    @builtins.property
     def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
         '''The log group the function sends logs to.
 
         By default, Lambda functions send logs to an automatically created default log group named /aws/lambda/.
         However you cannot change the properties of this auto-created log group using the AWS CDK, e.g. you cannot set a different log retention.
 
         Use the ``logGroup`` property to create a fully customizable LogGroup ahead of time, and instruct the Lambda function to send logs to it.
@@ -2303,16 +2346,18 @@
         environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
         events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
         filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
         function_name: typing.Optional[builtins.str] = None,
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+        ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_format: typing.Optional[builtins.str] = None,
+        logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
         log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
         params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
@@ -2350,16 +2395,18 @@
         :param environment_encryption: The AWS KMS key that's used to encrypt your function's environment variables. Default: - AWS Lambda creates and uses an AWS managed customer master key (CMK).
         :param ephemeral_storage_size: The size of the function’s /tmp directory in MiB. Default: 512 MiB
         :param events: Event sources for this function. You can also add event sources using ``addEventSource``. Default: - No event sources.
         :param filesystem: The filesystem configuration for the lambda function. Default: - will not mount any filesystem
         :param function_name: A name for the function. Default: - AWS CloudFormation generates a unique physical ID and uses that ID for the function's name. For more information, see Name Type.
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
+        :param ipv6_allowed_for_dual_stack: Allows outbound IPv6 traffic on VPC functions that are connected to dual-stack subnets. Only used if 'vpc' is supplied. Default: false
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_format: Sets the logFormat for the function. Default: "Text"
+        :param logging_format: Sets the loggingFormat for the function. Default: LoggingFormat.TEXT
         :param log_group: The log group the function sends logs to. By default, Lambda functions send logs to an automatically created default log group named /aws/lambda/<function name>. However you cannot change the properties of this auto-created log group using the AWS CDK, e.g. you cannot set a different log retention. Use the ``logGroup`` property to create a fully customizable LogGroup ahead of time, and instruct the Lambda function to send logs to it. Providing a user-controlled log group was rolled out to commercial regions on 2023-11-16. If you are deploying to another type of region, please check regional availability first. Default: ``/aws/lambda/${this.functionName}`` - default log group created by Lambda
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. This is a legacy API and we strongly recommend you move away from it if you can. Instead create a fully customizable log group with ``logs.LogGroup`` and use the ``logGroup`` property to instruct the Lambda function to send logs to it. Migrating from ``logRetention`` to ``logGroup`` will cause the name of the log group to change. Users and code and referencing the name verbatim will have to adjust. In AWS CDK code, you can access the log group name directly from the LogGroup construct:: import * as logs from 'aws-cdk-lib/aws-logs'; declare const myLogGroup: logs.LogGroup; myLogGroup.logGroupName; Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
         :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
@@ -2399,16 +2446,18 @@
             environment_encryption=environment_encryption,
             ephemeral_storage_size=ephemeral_storage_size,
             events=events,
             filesystem=filesystem,
             function_name=function_name,
             initial_policy=initial_policy,
             insights_version=insights_version,
+            ipv6_allowed_for_dual_stack=ipv6_allowed_for_dual_stack,
             layers=layers,
             log_format=log_format,
+            logging_format=logging_format,
             log_group=log_group,
             log_retention=log_retention,
             log_retention_retry_options=log_retention_retry_options,
             log_retention_role=log_retention_role,
             memory_size=memory_size,
             params_and_secrets=params_and_secrets,
             profiling=profiling,
@@ -2455,16 +2504,18 @@
         "environment_encryption": "environmentEncryption",
         "ephemeral_storage_size": "ephemeralStorageSize",
         "events": "events",
         "filesystem": "filesystem",
         "function_name": "functionName",
         "initial_policy": "initialPolicy",
         "insights_version": "insightsVersion",
+        "ipv6_allowed_for_dual_stack": "ipv6AllowedForDualStack",
         "layers": "layers",
         "log_format": "logFormat",
+        "logging_format": "loggingFormat",
         "log_group": "logGroup",
         "log_retention": "logRetention",
         "log_retention_retry_options": "logRetentionRetryOptions",
         "log_retention_role": "logRetentionRole",
         "memory_size": "memorySize",
         "params_and_secrets": "paramsAndSecrets",
         "profiling": "profiling",
@@ -2504,16 +2555,18 @@
         environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
         events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
         filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
         function_name: typing.Optional[builtins.str] = None,
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+        ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_format: typing.Optional[builtins.str] = None,
+        logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
         log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
         params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
@@ -2550,16 +2603,18 @@
         :param environment_encryption: The AWS KMS key that's used to encrypt your function's environment variables. Default: - AWS Lambda creates and uses an AWS managed customer master key (CMK).
         :param ephemeral_storage_size: The size of the function’s /tmp directory in MiB. Default: 512 MiB
         :param events: Event sources for this function. You can also add event sources using ``addEventSource``. Default: - No event sources.
         :param filesystem: The filesystem configuration for the lambda function. Default: - will not mount any filesystem
         :param function_name: A name for the function. Default: - AWS CloudFormation generates a unique physical ID and uses that ID for the function's name. For more information, see Name Type.
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
+        :param ipv6_allowed_for_dual_stack: Allows outbound IPv6 traffic on VPC functions that are connected to dual-stack subnets. Only used if 'vpc' is supplied. Default: false
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_format: Sets the logFormat for the function. Default: "Text"
+        :param logging_format: Sets the loggingFormat for the function. Default: LoggingFormat.TEXT
         :param log_group: The log group the function sends logs to. By default, Lambda functions send logs to an automatically created default log group named /aws/lambda/<function name>. However you cannot change the properties of this auto-created log group using the AWS CDK, e.g. you cannot set a different log retention. Use the ``logGroup`` property to create a fully customizable LogGroup ahead of time, and instruct the Lambda function to send logs to it. Providing a user-controlled log group was rolled out to commercial regions on 2023-11-16. If you are deploying to another type of region, please check regional availability first. Default: ``/aws/lambda/${this.functionName}`` - default log group created by Lambda
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. This is a legacy API and we strongly recommend you move away from it if you can. Instead create a fully customizable log group with ``logs.LogGroup`` and use the ``logGroup`` property to instruct the Lambda function to send logs to it. Migrating from ``logRetention`` to ``logGroup`` will cause the name of the log group to change. Users and code and referencing the name verbatim will have to adjust. In AWS CDK code, you can access the log group name directly from the LogGroup construct:: import * as logs from 'aws-cdk-lib/aws-logs'; declare const myLogGroup: logs.LogGroup; myLogGroup.logGroupName; Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. This is a legacy API and we strongly recommend you migrate to ``logGroup`` if you can. ``logGroup`` allows you to create a fully customizable log group and instruct the Lambda function to send logs to it. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
         :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
@@ -2604,16 +2659,18 @@
             check_type(argname="argument environment_encryption", value=environment_encryption, expected_type=type_hints["environment_encryption"])
             check_type(argname="argument ephemeral_storage_size", value=ephemeral_storage_size, expected_type=type_hints["ephemeral_storage_size"])
             check_type(argname="argument events", value=events, expected_type=type_hints["events"])
             check_type(argname="argument filesystem", value=filesystem, expected_type=type_hints["filesystem"])
             check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
             check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
             check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
+            check_type(argname="argument ipv6_allowed_for_dual_stack", value=ipv6_allowed_for_dual_stack, expected_type=type_hints["ipv6_allowed_for_dual_stack"])
             check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
             check_type(argname="argument log_format", value=log_format, expected_type=type_hints["log_format"])
+            check_type(argname="argument logging_format", value=logging_format, expected_type=type_hints["logging_format"])
             check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
             check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
             check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
             check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
             check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
             check_type(argname="argument params_and_secrets", value=params_and_secrets, expected_type=type_hints["params_and_secrets"])
             check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
@@ -2671,18 +2728,22 @@
             self._values["filesystem"] = filesystem
         if function_name is not None:
             self._values["function_name"] = function_name
         if initial_policy is not None:
             self._values["initial_policy"] = initial_policy
         if insights_version is not None:
             self._values["insights_version"] = insights_version
+        if ipv6_allowed_for_dual_stack is not None:
+            self._values["ipv6_allowed_for_dual_stack"] = ipv6_allowed_for_dual_stack
         if layers is not None:
             self._values["layers"] = layers
         if log_format is not None:
             self._values["log_format"] = log_format
+        if logging_format is not None:
+            self._values["logging_format"] = logging_format
         if log_group is not None:
             self._values["log_group"] = log_group
         if log_retention is not None:
             self._values["log_retention"] = log_retention
         if log_retention_retry_options is not None:
             self._values["log_retention_retry_options"] = log_retention_retry_options
         if log_retention_role is not None:
@@ -2975,14 +3036,25 @@
 
         :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Lambda-Insights-Getting-Started-docker.html
         '''
         result = self._values.get("insights_version")
         return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion], result)
 
     @builtins.property
+    def ipv6_allowed_for_dual_stack(self) -> typing.Optional[builtins.bool]:
+        '''Allows outbound IPv6 traffic on VPC functions that are connected to dual-stack subnets.
+
+        Only used if 'vpc' is supplied.
+
+        :default: false
+        '''
+        result = self._values.get("ipv6_allowed_for_dual_stack")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def layers(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]]:
         '''A list of layers to add to the function's execution environment.
 
         You can configure your Lambda function to pull in
         additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies
@@ -2999,14 +3071,25 @@
 
         :default: "Text"
         '''
         result = self._values.get("log_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def logging_format(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat]:
+        '''Sets the loggingFormat for the function.
+
+        :default: LoggingFormat.TEXT
+        '''
+        result = self._values.get("logging_format")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat], result)
+
+    @builtins.property
     def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
         '''The log group the function sends logs to.
 
         By default, Lambda functions send logs to an automatically created default log group named /aws/lambda/.
         However you cannot change the properties of this auto-created log group using the AWS CDK, e.g. you cannot set a different log retention.
 
         Use the ``logGroup`` property to create a fully customizable LogGroup ahead of time, and instruct the Lambda function to send logs to it.
@@ -3356,16 +3439,18 @@
     environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
     events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
     filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
     function_name: typing.Optional[builtins.str] = None,
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+    ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_format: typing.Optional[builtins.str] = None,
+    logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
     log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
     params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
@@ -3409,16 +3494,18 @@
     environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
     events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
     filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
     function_name: typing.Optional[builtins.str] = None,
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+    ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_format: typing.Optional[builtins.str] = None,
+    logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
     log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
     params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
@@ -3680,16 +3767,18 @@
     environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
     events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
     filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
     function_name: typing.Optional[builtins.str] = None,
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+    ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_format: typing.Optional[builtins.str] = None,
+    logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
     log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
     params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
@@ -3733,16 +3822,18 @@
     environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
     events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
     filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
     function_name: typing.Optional[builtins.str] = None,
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+    ipv6_allowed_for_dual_stack: typing.Optional[builtins.bool] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_format: typing.Optional[builtins.str] = None,
+    logging_format: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LoggingFormat] = None,
     log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
     params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
```

### Comparing `layerborn.cdk-ami-builder-0.0.5/src/layerborn.cdk_ami_builder.egg-info/PKG-INFO` & `layerborn.cdk-ami-builder-0.0.6/src/layerborn.cdk_ami_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerborn.cdk-ami-builder
-Version: 0.0.5
+Version: 0.0.6
 Summary: Creates an EC2 AMI using an Image Builder Pipeline and returns the AMI ID.
 Home-page: https://github.com/layerborn/cdk-ami-builder-construct.git
 Author: Jayson Rawlins<jayson.rawlins@layerborn.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/layerborn/cdk-ami-builder-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

