# Comparing `tmp/iam_actions-1.2.20240508.tar.gz` & `tmp/iam_actions-1.2.20240509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240508.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240509.tar", max compression
```

## Comparing `iam_actions-1.2.20240508.tar` & `iam_actions-1.2.20240509.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-08 02:09:35.737366 iam_actions-1.2.20240508/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-08 02:09:35.737366 iam_actions-1.2.20240508/README.md
--rw-r--r--   0        0        0      228 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/__init__.py
--rw-r--r--   0        0        0  4827367 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/services.py
--rw-r--r--   0        0        0   628076 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/policies.json
--rw-r--r--   0        0        0   209418 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   609432 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-08 02:11:22.033173 iam_actions-1.2.20240508/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240508/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240508/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/README.md
+-rw-r--r--   0        0        0      228 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4828689 2024-05-09 02:24:59.204566 iam_actions-1.2.20240509/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-09 02:23:18.696477 iam_actions-1.2.20240509/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   628163 2024-05-09 02:24:59.204566 iam_actions-1.2.20240509/iam_actions/policies.json
+-rw-r--r--   0        0        0   209462 2024-05-09 02:24:59.204566 iam_actions-1.2.20240509/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   609516 2024-05-09 02:24:59.204566 iam_actions-1.2.20240509/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-09 02:24:59.904566 iam_actions-1.2.20240509/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240509/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240509/PKG-INFO
```

### Comparing `iam_actions-1.2.20240508/LICENSE` & `iam_actions-1.2.20240509/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/README.md` & `iam_actions-1.2.20240509/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/iam_actions/actions.json` & `iam_actions-1.2.20240509/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992441883691323%*

 * *Differences: {"'budgets'": "{'CreateBudgetAction': {'condition_keys': ['aws:RequestTag/${TagKey}', "*

 * *              '\'aws:ResourceTag/${TagKey}\', \'aws:TagKeys\'], \'description\': "Grants '*

 * *              'permission to configure a response that executes once your budget exceeds a '*

 * *              'specific budget threshold. Creating a budget action with tags also requires the '*

 * *              '\'budgets:TagResource\' permission"}, \'ModifyBudget\': {\'description\': "Grants '*

 * *              'permission to create and modi […]*

```diff
@@ -15275,16 +15275,20 @@
             ]
         }
     },
     "budgets": {
         "CreateBudgetAction": {
             "access_level": "Write",
             "action": "CreateBudgetAction",
-            "condition_keys": [],
-            "description": "Grants permission to create and define a response that you can configure to execute once your budget has exceeded a specific budget threshold",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to configure a response that executes once your budget exceeds a specific budget threshold. Creating a budget action with tags also requires the 'budgets:TagResource' permission",
             "orphan": false,
             "resources": [
                 "budgetAction"
             ]
         },
         "DeleteBudgetAction": {
             "access_level": "Write",
@@ -15341,46 +15345,60 @@
             "description": "Grants permission to initiate a pending budget action as well as reverse a previously executed budget action",
             "orphan": false,
             "resources": [
                 "budgetAction"
             ]
         },
         "ListTagsForResource": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view resource tags for a budget or budget action",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "budget",
+                "budgetAction"
+            ]
         },
         "ModifyBudget": {
             "access_level": "Write",
             "action": "ModifyBudget",
             "condition_keys": [],
-            "description": "Grants permission to modify budgets and budget details",
+            "description": "Grants permission to create and modify budgets, and edit budget details. Creating a budget with tags also requires the 'budgets:TagResource' permission",
             "orphan": false,
             "resources": [
                 "budget"
             ]
         },
         "TagResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "TagResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to apply resource tags to a budget or budget action. Also needed to create a budget or budget action with tags",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "budget",
+                "budgetAction"
+            ]
         },
         "UntagResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "UntagResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to remove resource tags from a budget or budget action",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "budget",
+                "budgetAction"
+            ]
         },
         "UpdateBudgetAction": {
             "access_level": "Write",
             "action": "UpdateBudgetAction",
             "condition_keys": [],
             "description": "Grants permission to update the details of a specific budget action associated with a budget",
             "orphan": false,
@@ -104032,14 +104050,22 @@
             "condition_keys": [],
             "description": "Grants permission to list executions for a batch job",
             "orphan": false,
             "resources": [
                 "Application"
             ]
         },
+        "ListBatchJobRestartPoints": {
+            "access_level": "Undocumented",
+            "action": "ListBatchJobRestartPoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListDataSetImportHistory": {
             "access_level": "Read",
             "action": "ListDataSetImportHistory",
             "condition_keys": [],
             "description": "Grants permission to list data set import history",
             "orphan": false,
             "resources": [
@@ -132551,14 +132577,22 @@
             "access_level": "Undocumented",
             "action": "ListAppAssessmentComplianceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListAppAssessmentResourceDrifts": {
+            "access_level": "Undocumented",
+            "action": "ListAppAssessmentResourceDrifts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAppAssessments": {
             "access_level": "Undocumented",
             "action": "ListAppAssessments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -164073,18 +164107,18 @@
             "resources": [
                 "parallel-data"
             ]
         }
     },
     "trustedadvisor": {
         "BatchUpdateRecommendationResourceExclusion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "BatchUpdateRecommendationResourceExclusion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update one or more exclusion status for a list of recommendation resources",
             "orphan": false,
             "resources": []
         },
         "CreateEngagement": {
             "access_level": "Write",
             "action": "CreateEngagement",
             "condition_keys": [],
@@ -165995,14 +166029,22 @@
             "orphan": false,
             "resources": [
                 "TargetGroup"
             ]
         }
     },
     "vpc-lattice-svcs": {
+        "Connect": {
+            "access_level": "Undocumented",
+            "action": "Connect",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Invoke": {
             "access_level": "Write",
             "action": "Invoke",
             "condition_keys": [
                 "vpc-lattice-svcs:Port",
                 "vpc-lattice-svcs:RequestHeader/${HeaderName}",
                 "vpc-lattice-svcs:RequestQueryString/${QueryStringKey}",
```

### Comparing `iam_actions-1.2.20240508/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240509/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240509/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/iam_actions/generate/generate.py` & `iam_actions-1.2.20240509/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240509/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240509/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/iam_actions/generate/services.py` & `iam_actions-1.2.20240509/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240508/iam_actions/policies.json` & `iam_actions-1.2.20240509/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999944485646504%*

 * *Differences: {"'serviceMap'": "{'AWS Resilience Hub': {'Actions': {insert: [(26, "*

 * *                 "'ListAppAssessmentResourceDrifts')]}}, 'Amazon VPC Lattice Services': "*

 * *                 "{'Actions': {insert: [(0, 'Connect')]}}, 'AWS Mainframe Modernization Service': "*

 * *                 "{'Actions': {insert: [(20, 'ListBatchJobRestartPoints')]}}}"}*

```diff
@@ -7451,14 +7451,15 @@
                 "GetDeployment",
                 "GetEnvironment",
                 "GetSignedBluinsightsUrl",
                 "ListApplicationVersions",
                 "ListApplications",
                 "ListBatchJobDefinitions",
                 "ListBatchJobExecutions",
+                "ListBatchJobRestartPoints",
                 "ListDataSetImportHistory",
                 "ListDataSets",
                 "ListDeployments",
                 "ListEngineVersions",
                 "ListEnvironments",
                 "ListTagsForResource",
                 "StartApplication",
@@ -8693,14 +8694,15 @@
                 "DescribeAppVersionResourcesResolutionStatus",
                 "DescribeAppVersionTemplate",
                 "DescribeDraftAppVersionResourcesImportStatus",
                 "DescribeResiliencyPolicy",
                 "ImportResourcesToDraftAppVersion",
                 "ListAlarmRecommendations",
                 "ListAppAssessmentComplianceDrifts",
+                "ListAppAssessmentResourceDrifts",
                 "ListAppAssessments",
                 "ListAppComponentCompliances",
                 "ListAppComponentRecommendations",
                 "ListAppInputSources",
                 "ListAppVersionAppComponents",
                 "ListAppVersionResourceMappings",
                 "ListAppVersionResources",
@@ -21836,14 +21838,15 @@
                 "vpc-lattice:VpcId"
             ]
         },
         "Amazon VPC Lattice Services": {
             "ARNFormat": "arn:aws:vpc-lattice:${Region}:${Account}:${ResourceType}/${RelativeId}",
             "ARNRegex": "^arn:aws:vpc-lattice:.+",
             "Actions": [
+                "Connect",
                 "Invoke"
             ],
             "HasResource": true,
             "StringPrefix": "vpc-lattice-svcs",
             "conditionKeys": [
                 "vpc-lattice-svcs:Port",
                 "vpc-lattice-svcs:RequestHeader/${HeaderName}",
```

### Comparing `iam_actions-1.2.20240508/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240509/iam_actions/resourcetypes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998409669211196%*

 * *Differences: {"'budgets'": "{'budget': {'condition_keys': 'aws:RequestTag/${TagKey}'}, 'budgetAction': "*

 * *              "{'condition_keys': 'aws:RequestTag/${TagKey}'}}"}*

```diff
@@ -870,19 +870,19 @@
             "arn_pattern": "arn:*:braket:*:*:quantum-task/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "budgets": {
         "budget": {
             "arn_pattern": "arn:*:budgets::*:budget/*",
-            "condition_keys": null
+            "condition_keys": "aws:RequestTag/${TagKey}"
         },
         "budgetAction": {
             "arn_pattern": "arn:*:budgets::*:budget/*/action/*",
-            "condition_keys": null
+            "condition_keys": "aws:RequestTag/${TagKey}"
         }
     },
     "bugbust": {
         "Event": {
             "arn_pattern": "arn:*:bugbust:*:*:events/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
```

### Comparing `iam_actions-1.2.20240508/iam_actions/services.json` & `iam_actions-1.2.20240509/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999419430043589%*

 * *Differences: {"'m2'": "{'Actions': {insert: [(20, 'ListBatchJobRestartPoints')]}}",*

 * * "'resiliencehub'": "{'Actions': {insert: [(26, 'ListAppAssessmentResourceDrifts')]}}",*

 * * "'vpc-lattice-svcs'": "{'Actions': {insert: [(0, 'Connect')]}}"}*

```diff
@@ -14363,14 +14363,15 @@
             "GetDeployment",
             "GetEnvironment",
             "GetSignedBluinsightsUrl",
             "ListApplicationVersions",
             "ListApplications",
             "ListBatchJobDefinitions",
             "ListBatchJobExecutions",
+            "ListBatchJobRestartPoints",
             "ListDataSetImportHistory",
             "ListDataSets",
             "ListDeployments",
             "ListEngineVersions",
             "ListEnvironments",
             "ListTagsForResource",
             "StartApplication",
@@ -18616,14 +18617,15 @@
             "DescribeAppVersionResourcesResolutionStatus",
             "DescribeAppVersionTemplate",
             "DescribeDraftAppVersionResourcesImportStatus",
             "DescribeResiliencyPolicy",
             "ImportResourcesToDraftAppVersion",
             "ListAlarmRecommendations",
             "ListAppAssessmentComplianceDrifts",
+            "ListAppAssessmentResourceDrifts",
             "ListAppAssessments",
             "ListAppComponentCompliances",
             "ListAppComponentRecommendations",
             "ListAppInputSources",
             "ListAppVersionAppComponents",
             "ListAppVersionResourceMappings",
             "ListAppVersionResources",
@@ -23425,14 +23427,15 @@
         "ARNFormats": [
             "arn:aws:vpc-lattice:${Region}:${Account}:${ResourceType}/${RelativeId}"
         ],
         "ARNRegexes": [
             "^arn:aws:vpc-lattice:.+"
         ],
         "Actions": [
+            "Connect",
             "Invoke"
         ],
         "ConditionKeys": [
             "vpc-lattice-svcs:Port",
             "vpc-lattice-svcs:RequestHeader/${HeaderName}",
             "vpc-lattice-svcs:RequestMethod",
             "vpc-lattice-svcs:RequestQueryString/${QueryStringKey}",
```

### Comparing `iam_actions-1.2.20240508/pyproject.toml` & `iam_actions-1.2.20240509/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240508"
+version = "1.2.20240509"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240508/setup.py` & `iam_actions-1.2.20240509/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240508',
+    'version': '1.2.20240509',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240508/PKG-INFO` & `iam_actions-1.2.20240509/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240508
+Version: 1.2.20240509
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

