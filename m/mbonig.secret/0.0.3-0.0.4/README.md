# Comparing `tmp/mbonig.secret-0.0.3.tar.gz` & `tmp/mbonig.secret-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbonig.secret-0.0.3.tar", last modified: Mon Feb 26 20:41:33 2024, max compression
+gzip compressed data, was "mbonig.secret-0.0.4.tar", last modified: Fri May 10 14:28:03 2024, max compression
```

## Comparing `mbonig.secret-0.0.3.tar` & `mbonig.secret-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:41:33.704934 mbonig.secret-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-02-26 20:41:33.704934 mbonig.secret-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 20:41:33.704934 mbonig.secret-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:41:33.700934 mbonig.secret-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:41:33.700934 mbonig.secret-0.0.3/src/mbonig.secret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-02-26 20:41:33.000000 mbonig.secret-0.0.3/src/mbonig.secret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-26 20:41:33.000000 mbonig.secret-0.0.3/src/mbonig.secret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 20:41:33.000000 mbonig.secret-0.0.3/src/mbonig.secret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-26 20:41:33.000000 mbonig.secret-0.0.3/src/mbonig.secret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-26 20:41:33.000000 mbonig.secret-0.0.3/src/mbonig.secret.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:41:33.700934 mbonig.secret-0.0.3/src/mbonig_secret/
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/src/mbonig_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:41:33.700934 mbonig.secret-0.0.3/src/mbonig_secret/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/src/mbonig_secret/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   861684 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/src/mbonig_secret/_jsii/secret@0.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 20:41:21.000000 mbonig.secret-0.0.3/src/mbonig_secret/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:28:03.791264 mbonig.secret-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-10 14:28:03.791264 mbonig.secret-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:28:03.791264 mbonig.secret-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:28:03.787264 mbonig.secret-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:28:03.787264 mbonig.secret-0.0.4/src/mbonig.secret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-10 14:28:03.000000 mbonig.secret-0.0.4/src/mbonig.secret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-10 14:28:03.000000 mbonig.secret-0.0.4/src/mbonig.secret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:28:03.000000 mbonig.secret-0.0.4/src/mbonig.secret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 14:28:03.000000 mbonig.secret-0.0.4/src/mbonig.secret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 14:28:03.000000 mbonig.secret-0.0.4/src/mbonig.secret.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:28:03.787264 mbonig.secret-0.0.4/src/mbonig_secret/
+-rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/src/mbonig_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:28:03.787264 mbonig.secret-0.0.4/src/mbonig_secret/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/src/mbonig_secret/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   861689 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/src/mbonig_secret/_jsii/secret@0.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:27:53.000000 mbonig.secret-0.0.4/src/mbonig_secret/py.typed
```

### Comparing `mbonig.secret-0.0.3/LICENSE` & `mbonig.secret-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mbonig.secret-0.0.3/PKG-INFO` & `mbonig.secret-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbonig.secret
-Version: 0.0.3
+Version: 0.0.4
 Summary: An AWS CDK construct for creating a secret in AWS Secrets Manager, without losing manually changed values.
 Home-page: https://github.com/mbonig/secret.git
 Author: Matthew Bonig<matthew.bonig@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/mbonig/secret.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,19 @@
 # @matthewbonig/secrets
 
 The AWS Secrets Manager [Secret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.Secret.html) construct has a big footgun, **if you update the `generateSecretString` property, the secret gets recreated!**
 This isn't exactly a flaw of the CDK, but of how CloudFormation handles this property.
 
 So, this library has a single construct with a single intention, to allow you to update the `generateSecretString` property without recreating the secret.
 
+> [!WARNING]
+> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
+> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
+> Make a backup of your secret before using this new construct on an existing secret.
+
 ## Design Philosophy
 
 Secrets are the AWS-preferred method for passing configuration values to runtime components. However, with the existing
 secret it's painful to manage the contents of a secret over the life of a project. You can't provide all your configuration
 values directly in your `generateSecretString` property because you'll then likely expose sensitive
 IaC. However, you also can't just leave this field completely blank because it will either make post-deployment changes
 to the secret more error-prone (as someone may manually enter in field names incorrectly) or it will make it impossible
@@ -45,19 +50,14 @@
 
 * The values stored in secrets are required to be updated manually outside of the IaC process.
 * The shape of the secret is defined in the IaC process.
 * Changes to the shape of the secret are made through the IaC process.
 * Changes to the shape and values of the secret in IaC do not affect fields and values that were not changed in IaC.
 * Changes made to the value of the secret through an outside process are retained unless explicitly changed through IaC.
 
-> [!WARNING]
-> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
-> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
-> Make a backup of your secret before using this new construct on an existing secret.
-
 ## Usage
 
 ```python
 import { Secret } from '@matthewbonig/secrets';
 // ....
 new Secret(this, 'MySecret', {
   generateSecretString: {
```

### Comparing `mbonig.secret-0.0.3/README.md` & `mbonig.secret-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # @matthewbonig/secrets
 
 The AWS Secrets Manager [Secret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.Secret.html) construct has a big footgun, **if you update the `generateSecretString` property, the secret gets recreated!**
 This isn't exactly a flaw of the CDK, but of how CloudFormation handles this property.
 
 So, this library has a single construct with a single intention, to allow you to update the `generateSecretString` property without recreating the secret.
 
+> [!WARNING]
+> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
+> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
+> Make a backup of your secret before using this new construct on an existing secret.
+
 ## Design Philosophy
 
 Secrets are the AWS-preferred method for passing configuration values to runtime components. However, with the existing
 secret it's painful to manage the contents of a secret over the life of a project. You can't provide all your configuration
 values directly in your `generateSecretString` property because you'll then likely expose sensitive
 IaC. However, you also can't just leave this field completely blank because it will either make post-deployment changes
 to the secret more error-prone (as someone may manually enter in field names incorrectly) or it will make it impossible
@@ -22,19 +27,14 @@
 
 * The values stored in secrets are required to be updated manually outside of the IaC process.
 * The shape of the secret is defined in the IaC process.
 * Changes to the shape of the secret are made through the IaC process.
 * Changes to the shape and values of the secret in IaC do not affect fields and values that were not changed in IaC.
 * Changes made to the value of the secret through an outside process are retained unless explicitly changed through IaC.
 
-> [!WARNING]
-> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
-> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
-> Make a backup of your secret before using this new construct on an existing secret.
-
 ## Usage
 
 ```python
 import { Secret } from '@matthewbonig/secrets';
 // ....
 new Secret(this, 'MySecret', {
   generateSecretString: {
```

### Comparing `mbonig.secret-0.0.3/setup.py` & `mbonig.secret-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mbonig.secret",
-    "version": "0.0.3",
+    "version": "0.0.4",
     "description": "An AWS CDK construct for creating a secret in AWS Secrets Manager, without losing manually changed values.",
     "license": "MIT",
     "url": "https://github.com/mbonig/secret.git",
     "long_description_content_type": "text/markdown",
     "author": "Matthew Bonig<matthew.bonig@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "mbonig_secret",
         "mbonig_secret._jsii"
     ],
     "package_data": {
         "mbonig_secret._jsii": [
-            "secret@0.0.3.jsii.tgz"
+            "secret@0.0.4.jsii.tgz"
         ],
         "mbonig_secret": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `mbonig.secret-0.0.3/src/mbonig.secret.egg-info/PKG-INFO` & `mbonig.secret-0.0.4/src/mbonig.secret.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbonig.secret
-Version: 0.0.3
+Version: 0.0.4
 Summary: An AWS CDK construct for creating a secret in AWS Secrets Manager, without losing manually changed values.
 Home-page: https://github.com/mbonig/secret.git
 Author: Matthew Bonig<matthew.bonig@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/mbonig/secret.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,19 @@
 # @matthewbonig/secrets
 
 The AWS Secrets Manager [Secret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.Secret.html) construct has a big footgun, **if you update the `generateSecretString` property, the secret gets recreated!**
 This isn't exactly a flaw of the CDK, but of how CloudFormation handles this property.
 
 So, this library has a single construct with a single intention, to allow you to update the `generateSecretString` property without recreating the secret.
 
+> [!WARNING]
+> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
+> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
+> Make a backup of your secret before using this new construct on an existing secret.
+
 ## Design Philosophy
 
 Secrets are the AWS-preferred method for passing configuration values to runtime components. However, with the existing
 secret it's painful to manage the contents of a secret over the life of a project. You can't provide all your configuration
 values directly in your `generateSecretString` property because you'll then likely expose sensitive
 IaC. However, you also can't just leave this field completely blank because it will either make post-deployment changes
 to the secret more error-prone (as someone may manually enter in field names incorrectly) or it will make it impossible
@@ -45,19 +50,14 @@
 
 * The values stored in secrets are required to be updated manually outside of the IaC process.
 * The shape of the secret is defined in the IaC process.
 * Changes to the shape of the secret are made through the IaC process.
 * Changes to the shape and values of the secret in IaC do not affect fields and values that were not changed in IaC.
 * Changes made to the value of the secret through an outside process are retained unless explicitly changed through IaC.
 
-> [!WARNING]
-> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
-> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
-> Make a backup of your secret before using this new construct on an existing secret.
-
 ## Usage
 
 ```python
 import { Secret } from '@matthewbonig/secrets';
 // ....
 new Secret(this, 'MySecret', {
   generateSecretString: {
```

### Comparing `mbonig.secret-0.0.3/src/mbonig_secret/__init__.py` & `mbonig.secret-0.0.4/src/mbonig_secret/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 # @matthewbonig/secrets
 
 The AWS Secrets Manager [Secret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.Secret.html) construct has a big footgun, **if you update the `generateSecretString` property, the secret gets recreated!**
 This isn't exactly a flaw of the CDK, but of how CloudFormation handles this property.
 
 So, this library has a single construct with a single intention, to allow you to update the `generateSecretString` property without recreating the secret.
 
+> [!WARNING]
+> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
+> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
+> Make a backup of your secret before using this new construct on an existing secret.
+
 ## Design Philosophy
 
 Secrets are the AWS-preferred method for passing configuration values to runtime components. However, with the existing
 secret it's painful to manage the contents of a secret over the life of a project. You can't provide all your configuration
 values directly in your `generateSecretString` property because you'll then likely expose sensitive
 IaC. However, you also can't just leave this field completely blank because it will either make post-deployment changes
 to the secret more error-prone (as someone may manually enter in field names incorrectly) or it will make it impossible
@@ -23,19 +28,14 @@
 
 * The values stored in secrets are required to be updated manually outside of the IaC process.
 * The shape of the secret is defined in the IaC process.
 * Changes to the shape of the secret are made through the IaC process.
 * Changes to the shape and values of the secret in IaC do not affect fields and values that were not changed in IaC.
 * Changes made to the value of the secret through an outside process are retained unless explicitly changed through IaC.
 
-> [!WARNING]
-> If you have an existing aws-cdk-lib/aws_secretsmanager.Secret, you can replace it with this new construct. However,
-> when you update your stack the existing value will be completely wiped out and re-created using the new construct.
-> Make a backup of your secret before using this new construct on an existing secret.
-
 ## Usage
 
 ```python
 import { Secret } from '@matthewbonig/secrets';
 // ....
 new Secret(this, 'MySecret', {
   generateSecretString: {
```

