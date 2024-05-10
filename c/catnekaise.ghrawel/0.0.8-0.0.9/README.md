# Comparing `tmp/catnekaise.ghrawel-0.0.8.tar.gz` & `tmp/catnekaise.ghrawel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnekaise.ghrawel-0.0.8.tar", last modified: Tue Apr  2 06:51:31 2024, max compression
+gzip compressed data, was "catnekaise.ghrawel-0.0.9.tar", last modified: Tue Apr 30 05:38:58 2024, max compression
```

## Comparing `catnekaise.ghrawel-0.0.8.tar` & `catnekaise.ghrawel-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/
--rw-r--r--   0 runner    (1001) docker     (127)   169741 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   213785 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/_jsii/ghrawel@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:38:58.278635 catnekaise.ghrawel-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-30 05:38:58.278635 catnekaise.ghrawel-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:38:58.278635 catnekaise.ghrawel-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:38:58.274635 catnekaise.ghrawel-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:38:58.274635 catnekaise.ghrawel-0.0.9/src/catnekaise.ghrawel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-30 05:38:58.000000 catnekaise.ghrawel-0.0.9/src/catnekaise.ghrawel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 05:38:58.000000 catnekaise.ghrawel-0.0.9/src/catnekaise.ghrawel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:38:58.000000 catnekaise.ghrawel-0.0.9/src/catnekaise.ghrawel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 05:38:58.000000 catnekaise.ghrawel-0.0.9/src/catnekaise.ghrawel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 05:38:58.000000 catnekaise.ghrawel-0.0.9/src/catnekaise.ghrawel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:38:58.274635 catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/
+-rw-r--r--   0 runner    (1001) docker     (127)   169741 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:38:58.274635 catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   213784 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/_jsii/ghrawel@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:38:47.000000 catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/py.typed
```

### Comparing `catnekaise.ghrawel-0.0.8/LICENSE` & `catnekaise.ghrawel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `catnekaise.ghrawel-0.0.8/PKG-INFO` & `catnekaise.ghrawel-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.ghrawel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Use ghrawel to deploy an AWS API Gateway RestAPI capable of returning GitHub App installation access tokens and use AWS IAM to control access to this API.
 Home-page: https://github.com/catnekaise/ghrawel.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/ghrawel.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.ghrawel-0.0.8/README.md` & `catnekaise.ghrawel-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `catnekaise.ghrawel-0.0.8/setup.py` & `catnekaise.ghrawel-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "catnekaise.ghrawel",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Use ghrawel to deploy an AWS API Gateway RestAPI capable of returning GitHub App installation access tokens and use AWS IAM to control access to this API.",
     "license": "Apache-2.0",
     "url": "https://github.com/catnekaise/ghrawel.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Jonsén<djonser1@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "catnekaise_ghrawel",
         "catnekaise_ghrawel._jsii"
     ],
     "package_data": {
         "catnekaise_ghrawel._jsii": [
-            "ghrawel@0.0.8.jsii.tgz"
+            "ghrawel@0.0.9.jsii.tgz"
         ],
         "catnekaise_ghrawel": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.82.0, <3.0.0",
         "catnekaise.cdk-iam-utilities>=0.0.13, <0.0.14",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/PKG-INFO` & `catnekaise.ghrawel-0.0.9/src/catnekaise.ghrawel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.ghrawel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Use ghrawel to deploy an AWS API Gateway RestAPI capable of returning GitHub App installation access tokens and use AWS IAM to control access to this API.
 Home-page: https://github.com/catnekaise/ghrawel.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/ghrawel.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/__init__.py` & `catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/__init__.py`

 * *Files identical despite different names*

### Comparing `catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/_jsii/ghrawel@0.0.8.jsii.tgz` & `catnekaise.ghrawel-0.0.9/src/catnekaise_ghrawel/_jsii/ghrawel@0.0.9.jsii.tgz`

 * *Files 22% similar despite different names*

#### Comparing `ghrawel@0.0.8.jsii.tgz-content` & `ghrawel@0.0.9.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'fingerprint'": "'aiS91/VyZsRF7/08vAWMQ7BjQ83jtdT7WKJ7iCDgpZw='",*

 * * "'jsiiVersion'": "'5.3.34 (build f4c2317)'",*

 * * "'version'": "'0.0.9'"}*

```diff
@@ -3476,17 +3476,17 @@
             }
         }
     },
     "description": "Use ghrawel to deploy an AWS API Gateway RestAPI capable of returning GitHub App installation access tokens and use AWS IAM to control access to this API.",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "j+lpKKwYCYWnGHGsy8SaIwYnKgc/g3Zf80JVFOi9V08=",
+    "fingerprint": "aiS91/VyZsRF7/08vAWMQ7BjQ83jtdT7WKJ7iCDgpZw=",
     "homepage": "https://github.com/catnekaise/ghrawel.git",
-    "jsiiVersion": "5.3.33 (build 023495c)",
+    "jsiiVersion": "5.3.34 (build f4c2317)",
     "keywords": [
         "api-gateway",
         "aws-iam",
         "cdk",
         "github",
         "github-actions",
         "github-app"
@@ -7154,9 +7154,9 @@
                         "fqn": "@catnekaise/ghrawel.RepositorySelectionMode"
                     }
                 }
             ],
             "symbolId": "src/token-provider/target:TokenProviderTargetRule"
         }
     },
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

##### package/lib/token-provider/api.js

###### js-beautify {}

```diff
@@ -114,10 +114,10 @@
         });
     }
 }
 exports.TokenProviderApi = TokenProviderApi;
 _a = JSII_RTTI_SYMBOL_1;
 TokenProviderApi[_a] = {
     fqn: "@catnekaise/ghrawel.TokenProviderApi",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiYXBpLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vLi4vc3JjL3Rva2VuLXByb3ZpZGVyL2FwaS50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLDZDQUFvRDtBQUNwRCx5REFBeUQ7QUFDekQsaURBQWlEO0FBQ2pELDJDQUF1QztBQUN2QyxpREFBMkQ7QUFDM0QscUNBQW1EO0FBQ25ELHFEQUF3RjtBQUN4RiwyQkFBb0U7QUFnRHBFLE1BQWEsZ0JBQWlCLFNBQVEsc0JBQVM7SUFXN0MsSUFBSSxjQUFjO1FBQ2hCLE9BQU8sSUFBSSxDQUFDLE9BQU8sQ0FBQztJQUN0QixDQUFDO0lBRUQsSUFBSSxPQUFPO1FBQ1QsT0FBTyxJQUFJLENBQUMsSUFBSSxDQUFDO0lBQ25CLENBQUM7SUFFRCxZQUFZLEtBQWdCLEVBQUUsRUFBVSxFQUFFLEtBQTRCO1FBQ3BFLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxDQUFDLENBQUM7UUFsQkYsMkJBQXNCLEdBQWEsRUFBRSxDQUFDO1FBb0JyRCxJQUFJLENBQUMsS0FBSyxHQUFHLEtBQUssQ0FBQztRQUVuQixJQUFJLEtBQUssQ0FBQyxHQUFHLEVBQUUsQ0FBQztZQUNkLElBQUksQ0FBQyxJQUFJLEdBQUcsS0FBSyxDQUFDLEdBQUcsQ0FBQztRQUN4QixDQUFDO2FBQU0sQ0FBQztZQUNOLElBQUksQ0FBQyxJQUFJLEdBQUcsSUFBSSxVQUFVLENBQUMsT0FBTyxDQUFDLElBQUksRUFBRSxrQkFBa0IsRUFBRTtnQkFDM0QsYUFBYSxFQUFFO29CQUNiLG9CQUFvQixFQUFFLEVBQUU7b0JBQ3hCLG1CQUFtQixFQUFFLEVBQUU7b0JBQ3ZCLFNBQVMsRUFBRSxLQUFLO2lCQUNqQjthQUNGLENBQUMsQ0FBQztZQUNILHlCQUFXLENBQUMsRUFBRSxDQUFDLElBQUksQ0FBQyxDQUFDLFVBQVUsQ0FBQyxzSkFBc0osQ0FBQyxDQUFDO1FBQzFMLENBQUM7UUFFRCxJQUFJLENBQUMsa0JBQWtCLEdBQUcsSUFB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LEVBQUUsQ0FBQztRQUM5RSxNQUFNLFVBQVUsR0FBRyxhQUFhLENBQUMsVUFBVSxJQUFJLGdDQUF1QixDQUFDLFVBQVUsRUFBRSxDQUFDO1FBQ3BGLE1BQU0sT0FBTyxHQUFHLGFBQWEsQ0FBQyxHQUFHLElBQUksU0FBUyxDQUFDO1FBRS9DLE9BQU8sOEJBQWEsQ0FBQyxNQUFNLENBQUMsSUFBSSxFQUFFLElBQUksRUFBRTtZQUN0QyxHQUFHLEVBQUUsSUFBSSxDQUFDLElBQUk7WUFDZCxHQUFHLEVBQUUsT0FBTztZQUNaLEtBQUssRUFBRSxJQUFJLENBQUMsS0FBSyxDQUFDLElBQUksQ0FBQyxrQkFBa0IsQ0FBQyxPQUFPLENBQUM7WUFDbEQsWUFBWSxFQUFFLHdDQUF5QixDQUFDLE1BQU0sRUFBRTtZQUNoRCxRQUFRO1lBQ1IsTUFBTSxFQUFFLElBQUksQ0FBQyxPQUFPO1lBQ3BCLGFBQWEsRUFBRTtnQkFDYixnQkFBZ0IsRUFBRSxJQUFJLENBQUMsZ0JBQWdCO2dCQUN2QyxZQUFZLEVBQUUsUUFBUSxDQUFDLElBQUk7Z0JBQzNCLGtCQUFrQixFQUFFLElBQUksQ0FBQyxrQkFBa0I7Z0JBQzNDLGtCQUFrQixFQUFFLElBQUksQ0FBQyxrQkFBa0I7Z0JBQzNDLGFBQWEsRUFBRSxZQUFZLElBQUksRUFBRTthQUNsQztZQUNELElBQUk7WUFDSixXQUFXLEVBQUUsYUFBYSxDQUFDLFdBQVc7WUFDdEMsVUFBVTtTQUNYLENBQUMsQ0FBQztJQUNMLENBQUM7O0FBekhILDRDQTJIQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IEFubm90YXRpb25zLCBEdXJhdGlvbiB9IGZyb20gJ2F3cy1jZGstbGliJztcbmltcG9ydCAqIGFzIGFwaWdhdGV3YXkgZnJvbSAnYXdzLWNkay1saWIvYXdzLWFwaWdhdGV3YXknO1xuaW1wb3J0ICogYXMgbGFtYmRhIGZyb20gJ2F3cy1jZGstbGliL2F3cy1sYW1iZGEnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQgeyBUb2tlblByb3ZpZGVyQ29uZmlndXJhdG9yIH0gZnJvbSAnLi9jb25maWd1cmF0b3InO1xuaW1wb3J0IHsgVG9rZW5Qcm92aWRlclRhcmdldFJ1bGUgfSBmcm9tICcuL3RhcmdldCc7XG5pbXBvcnQgeyBJVG9rZW5Qcm92aWRlciwgVG9rZW5Qcm92aWRlciwgVG9rZW5Qcm92aWRlckVuZHBvaW50IH0gZnJvbSAnLi90b2tlbi1wcm92aWRlcic7XG5pbXBvcnQgeyBHaXRIdWJBcHBQZXJtaXNzaW9ucywgVG9rZW5Qcm92aWRlckxhbWJkYUNvZGUgfSBmcm9tICcuLi8nO1xuaW1wb3J0IHsgSUdpdEh1YkFwcHMgfSBmcm9tICcuLi9hcHBzJztcblxuZXhwb3J0IGludGVyZmFjZSBUb2tlblByb3ZpZGVyQXBpUHJvcHMge1xuXG4gIC8qKlxuICAgKiBHaXRIdWIgQXBwcyBjb25maWd1cmF0aW9uXG4gICAqL1xuICByZWFkb25seSBhcHBzOiBJR2l0SHViQXBwcztcblxuICAvKipcbiAgICogVXNlIHRoaXMgdG8gcHJvdmlkZSB0aGUgQVBJIEdhdGV3YXkgUmVzdEFwaSBjb25maWd1cmVkIHRvIHlvdXIgcmVxdWlyZW1lbnRzXG4gICAqL1xuICByZWFkb25seSBhcGk/OiBhcGlnYXRld2F5LlJlc3RBcGk7XG5cbiAgLyoqXG4gICAqIFVzZSB0aGlzIHRvIHByb3ZpZGUgdGhlIExhbWJkYSBGdW5jdGlvbiBjb25maWd1cmVkIHRvIHlvdXIgcmVxdWlyZW1lbnRzXG4gICAqL1xuICByZWFkb25seSBsYW1iZGE/OiBsYW1iZGEuRnVuY3Rpb247XG59XG5cbmV4cG9ydCBpbnRlcmZhY2UgTmV3VG9rZW5Qcm92aWRlckNvbmZpZ3VyYXRpb24ge1xuXG4gIC8qKlxuICAgKiBQZXJtaXNzaW9uc1xuICAgKi9cbiAgcmVhZG9ubHkgcGVybWlzc2lvbnM6IEdpdEh1YkFwcFBlcm1pc3Npb25zO1xuXG4gIC8qKlxuICAgKiBAZGVmYXVsdCBERUZBVUxUXG4gICAqL1xuICByZWFkb25seSBlbmRwb2ludD86IFRva2VuUHJvdmlkZXJFbmRwb2ludDtcblxuICAvKipcbiAgICogQGRlZmF1bHQgQVRfTEVBU1RfT05FXG4gICAqL1xuICByZWFkb25seSB0YXJnZXRSdWxlPzogVG9rZW5Qcm92aWRlclRhcmdldFJ1bGU7XG5cbiAgLyoqXG4gICAqIEBkZWZhdWx0IGRlZmF1bHRcbiAgICovXG4gIHJlYWRvbmx5IGFwcD86IHN0cmluZztcbn1cblxuZXhwb3J0IGludGVyZmFjZSBJVG9rZW5Qcm92aWRlckFwaSB7XG4gIG5ld1Rva2VuUHJvdmlkZXIobmFtZTogc3RyaW5nLCBjb25maWd1cmF0aW9uOiBOZXdUb2tlblByb3ZpZGVyQ29uZmlndXJhdGlvbik6IElUb2tlblByb3ZpZGVyO1xufVxuXG5leHBvcnQgY2xhc3MgVG9rZW5Qcm92aWRlckFwaSBleHRlbmRzIENvbnN0cnVjdCBpbXBsZW1lbnRzIElUb2tlblByb3ZpZGVyQXBpIHtcblxuICBwcml2YXRlIHJlYWRvbmx5IHVzZWRUb2tlblByb3ZpZGVyTmFtZXM6IHN0cmluZ1tdID0gW107XG5cbiAgcHJpdmF0ZSByZWFkb25seSB0b2tlblJlc3BvbnNlTW9kZWw6IGFwaWdhdGV3YXkuTW9kZWw7XG4gIHByaXZhdGUgcmVhZG9ubHkgZXJyb3JSZXNwb25zZU1vZGVsOiBhcGlnYXRld2F5Lk1vZGVsO1xuICBwcml2YXRlIHJlYWRvbmx5IF9sYW1iZGE6IGxhbWJkYS5GdW5jdGlvbjtcbiAgcHJpdmF0ZSByZWFkb25seSBfYXBpOiBhcGlnYXRld2F5LlJlc3RBcGk7XG4gIHByaXZhdGUgcmVhZG9ubHkgcHJvcHM6IFRva2VuUHJvdmlkZXJBcGlQcm9wcztcbiAgcHJpdmF0ZSByZWFkb25seSByZXF1ZXN0VmFsaWRhdG9yOiBhcGlnYXRld2F5LlJlcXVlc3RWYWxpZGF0b3I7XG5cbiAgZ2V0IGxhbWJkYUZ1bmN0aW9uKCk6IGxhbWJkYS5GdW5jdGlvbiB7XG4gICAgcmV0dXJuIHRoaXMuX2xhbWJkYTtcbiAgfVxuXG4gIGdldCByZXN0QXBpKCk6IGFwaWdhdGV3YXkuUmVzdEFwaSB7XG4gICAgcmV0dXJuIHRoaXMuX2FwaTtcbiAgfVxuXG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBUb2tlblByb3ZpZGVyQXBpUHJvcHMpIHtcbiAgICBzdXBlcihzY29wZSwgaWQpO1xuXG4gICAgdGhpcy5wcm9wcyA9IHByb3BzO1xuXG4gICAgaWYgKHByb3BzLmFwaSkge1xuICAgICAgdGhpcy5fYXBpID0gcHJvcHMuYXBpO1xuICAgIH0gZWxzZSB7XG4gICAgICB0aGlzLl9hcGkgPSBuZXcgYXBpZ2F0ZXdheS5SZXN0QXBpKHRoaXMsICdUb2tlblByb3ZpZGVyQXBpJywge1xuICAgICAgICBkZXBsb3lPcHRpb25zOiB7XG4gICAgICAgICAgdGhyb3R0bGluZ0J1cnN0TGltaXQ6IDEwLFxuICAgICAgICAgIHRocm90dGxpbmdSYXRlTGltaXQ6IDEwLFxuICAgICAgICAgIHN0YWdlTmFtZTogJ2RldicsXG4gICAgICAgIH0sXG4gICAgICB9KTtcbiAgICAgIEFubm90YXRpb25zLm9mKHRoaXMpLmFkZFdhcm5pbmcoJ1RoZSBSZXN0QXBpIGNyZWF0ZWQgYnkgdGhlIGBUb2tlblByb3ZpZGVyQXBpYCBjb25zdHJ1Y3QgaXMgb25seSBpbnRlbmRlZCBmb3IgdGVzdGluZyBwdXJwb3Nlcy4gUHJvdmlkZSB5b3VyIG93biBSZXN0QXBpIHZpYSBwcm9wcyB0byB0aGlzIGNvbnN0cnVjdC4nKTtcbiAgICB9XG5cbiAgICB0aGlzLnRva2VuUmVzcG9uc2VNb2RlbCA9IHRoaXMuX2FwaS5hZGRNb2RlbCgnVG9rZW5SZXNwb25zZU1vZGVsJywge1xuICAgICAgY29udGVudFR5cGU6ICdhcHBsaWNhdGlvbi9qc29uJyxcbiAgICAgIG1vZGVsTmFtZTogJ1Rva2VuUmVzcG9uc2UnLFxuICAgICAgc2NoZW1hOiB7XG4gICAgICAgIHNjaGVtYTogYXBpZ2F0ZXdheS5Kc29uU2NoZW1hVmVyc2lvbi5EUkFGVDcsXG4gICAgICAgIHRpdGxlOiAndG9rZW5SZXNwb25zZScsXG4gICAgICAgIHR5cGU6IGFwaWdhdGV3YXkuSnNvblNjaGVtYVR5cGUuT0JKRUNULFxuICAgICAgICBwcm9wZXJ0aWVzOiB7XG4gICAgICAgICAgdG9rZW46IHsgdHlwZTogYXBpZ2F0ZXdheS5Kc29uU2NoZW1hVHlwZS5TVFJJTkcgfSxcbiAgICAgICAgfSxcbiAgICAgIH0sXG4gICAgfSk7XG5cbiAgICB0aGlzLmVycm9yUmVzcG9uc2VNb2RlbCA9IHRoaXMuX2FwaS5hZGRNb2RlbCgnRXJyb3JSZXNwb25zZU1vZGVsJywge1xuICAgICAgY29udGVudFR5cGU6ICdhcHBsaWNhdGlvbi9qc29uJyxcbiAgICAgIG1vZGVsTmFtZTogJ0Vycm9yUmVzcG9uc2VNb2RlbCcsXG4gICAgICBzY2hlbWE6IHtcbiAgICAgICAgc2NoZW1hOiBhcGlnYXRld2F5Lkpzb25TY2hlbWFWZXJzaW9uLkRSQUZUNyxcbiAgICAgICAgdGl0bGU6ICdlcnJvclJlc3BvbnNlJyxcbiAgICAgICAgdHlwZTogYXBpZ2F0ZXdheS5Kc29uU2NoZW1hVHlwZS5PQkpFQ1QsXG4gICAgICAgIHByb3BlcnRpZXM6IHtcbiAgICAgICAgICBlcnJvck1lc3NhZ2U6IHsgdHlwZTogYXBpZ2F0ZXdheS5Kc29uU2NoZW1hVHlwZS5TVFJJTkcgfSxcbiAgICAgICAgfSxcbiAgICAgIH0sXG4gICAgfSk7XG5cbiAgICB0aGlzLnJlcXVlc3RWYWxpZGF0b3IgPSBuZXcgYXBpZ2F0ZXdheS5SZXF1ZXN0VmFsaWRhdG9yKHRoaXMsICdSZXF1ZXN0VmFsaWRhdG9yJywge1xuICAgICAgcmVxdWVzdFZhbGlkYXRvck5hbWU6ICdQYXJhbWV0ZXJWYWxpZGF0b3InLFxuICAgICAgcmVzdEFwaTogdGhpcy5fYXBpLFxuICAgICAgdmFsaWRhdGVSZXF1ZXN0Qm9keTogZmFsc2UsXG4gICAgICB2YWxpZGF0ZVJlcXVlc3RQYXJhbWV0ZXJzOiB0cnVlLFxuXG4gICAgfSk7XG5cbiAgICBpZiAocHJvcHMubGFtYmRhKSB7XG4gICAgICB0aGlzLl9sYW1iZGEgPSBwcm9wcy5sYW1iZGE7XG4gICAgfSBlbHNlIHtcbiAgICAgIHRoaXMuX2xhbWJkYSA9IG5ldyBsYW1iZGEuRnVuY3Rpb24odGhpcywgJ0Z1bmN0aW9uJywge1xuICAgICAgICBjb2RlOiBUb2tlblByb3ZpZGVyTGFtYmRhQ29kZS5kZWZhdWx0R28oKSxcbiAgICAgICAgaGFuZGxlcjogJ2Jvb3RzdHJhcCcsXG4gICAgICAgIHJ1bnRpbWU6IG5ldyBsYW1iZGEuUnVudGltZSgncHJvdmlkZWQuYWwyMDIzJywgbGFtYmRhLlJ1bnRpbWVGYW1pbHkuT1RIRVIpLFxuICAgICAgICBtZW1vcnlTaXplOiA1MTIsXG4gICAgICAgIHJldHJ5QXR0ZW1wdHM6IDAsXG4gICAgICAgIHRpbWVvdXQ6IER1cmF0aW9uLnNlY29uZHMoMTApLFxuICAgICAgfSk7XG4gICAgfVxuXG4gICAgdGhpcy5fbGFtYmRhLmFkZEVudmlyb25tZW50KCdTRUNSRVRTX1BSRUZJWCcsIHByb3BzLmFwcHMuc2VjcmV0c1ByZWZpeCk7XG4gICAgdGhpcy5fbGFtYmRhLmFkZEVudmlyb25tZW50KCdTRUNSRVRTX1NUT1JBR0UnLCBwcm9wcy5hcHBzLnNlY3JldHNTdG9yYWdlKTtcblxuICAgIHByb3BzLmFwcHMuZ3JhbnRBY2Nlc3ModGhpcy5fbGFtYmRhLmdyYW50UHJpbmNpcGFsKTtcblxuICB9XG5cbiAgbmV3VG9rZW5Qcm92aWRlcihuYW1lOiBzdHJpbmcsIGNvbmZpZ3VyYXRpb246IE5ld1Rva2VuUHJvdmlkZXJDb25maWd1cmF0aW9uKTogSVRva2VuUHJvdmlkZXIge1xuXG4gICAgaWYgKHRoaXMudXNlZFRva2VuUHJvdmlkZXJOYW1lcy5pbmNsdWRlcyhuYW1lKSkge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKGBBIHRva2VuIHByb3ZpZGVyIHdpdGggdGhlIG5hbWUgJHtuYW1lfSBoYXMgYWxyZWFkeSBiZWVuIGNyZWF0ZWRgKTtcbiAgICB9XG5cbiAgICB0aGlzLnVzZWRUb2tlblByb3ZpZGVyTmFtZXMucHVzaChuYW1lKTtcblxuICAgIGNvbnN0IGVuZHBvaW50ID0gY29uZmlndXJhdGlvbi5lbmRwb2ludCA/PyBUb2tlblByb3ZpZGVyRW5kcG9pbnQudXNlRGVmYXVsdCgpO1xuICAgIGNvbnN0IHRhcmdldFJ1bGUgPSBjb25maWd1cmF0aW9uLnRhcmdldFJ1bGUgPz8gVG9rZW5Qcm92aWRlclRhcmdldFJ1bGUuYXRMZWFzdE9uZSgpO1xuICAgIGNvbnN0IGFwcE5hbWUgPSBjb25maWd1cmF0aW9uLmFwcCA/PyAnZGVmYXVsdCc7XG5cbiAgICByZXR1cm4gVG9rZW5Qcm92aWRlci5jcmVhdGUodGhpcywgbmFtZSwge1xuICAgICAgYXBpOiB0aGlzLl9hcGksXG4gICAgICBhcHA6IGFwcE5hbWUsXG4gICAgICBhcHBJZDogdGhpcy5wcm9wcy5hcHBzLmdldEFwcElkRm9yQXBwTmFtZShhcHBOYW1lKSxcbiAgICAgIGNvbmZpZ3VyYXRvcjogVG9rZW5Qcm92aWRlckNvbmZpZ3VyYXRvci5jcmVhdGUoKSxcbiAgICAgIGVuZHBvaW50LFxuICAgICAgbGFtYmRhOiB0aGlzLl9sYW1iZGEsXG4gICAgICBtZXRob2RPcHRpb25zOiB7XG4gICAgICAgIHJlcXVlc3RWYWxpZGF0b3I6IHRoaXMucmVxdWVzdFZhbGlkYXRvcixcbiAgICAgICAgZW5kcG9pbnRUeXBlOiBlbmRwb2ludC50eXBlLFxuICAgICAgICB0b2tlblJlc3BvbnNlTW9kZWw6IHRoaXMudG9rZW5SZXNwb25zZU1vZGVsLFxuICAgICAgICBlcnJvclJlc3BvbnNlTW9kZWw6IHRoaXMuZXJyb3JSZXNwb25zZU1vZGVsLFxuICAgICAgICBvcGVyYXRpb25OYW1lOiBgcHJvdmlkZXItJHtuYW1lfWAsXG4gICAgICB9LFxuICAgICAgbmFtZSxcbiAgICAgIHBlcm1pc3Npb25zOiBjb25maWd1cmF0aW9uLnBlcm1pc3Npb25zLFxuICAgICAgdGFyZ2V0UnVsZSxcbiAgICB9KTtcbiAgfVxuXG59XG4iXX0=
```

##### package/lib/apps.js

###### js-beautify {}

```diff
@@ -24,15 +24,15 @@
         this.appId = appId;
     }
 }
 exports.GitHubApp = GitHubApp;
 _a = JSII_RTTI_SYMBOL_1;
 GitHubApp[_a] = {
     fqn: "@catnekaise/ghrawel.GitHubApp",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 const DEFAULT_SECRETS_PREFIX = '/catnekaise/github-apps';
 class BaseGitHubApps extends constructs_1.Construct {
     constructor(scope, id, baseProps) {
         super(scope, id);
         this.baseProps = baseProps;
     }
@@ -53,15 +53,15 @@
         return app.appId;
     }
 }
 exports.BaseGitHubApps = BaseGitHubApps;
 _b = JSII_RTTI_SYMBOL_1;
 BaseGitHubApps[_b] = {
     fqn: "@catnekaise/ghrawel.BaseGitHubApps",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 class ManagedGitHubApps extends BaseGitHubApps {
     constructor(scope, id, props) {
         super(scope, id, props);
         this.props = props;
         const appNames = ['default', ...(props.additionalApps ?? []).map(x => x.name)];
         const secretPrefixId = this.secretsPrefix.substring(1).split('/')
@@ -114,30 +114,30 @@
         return grant;
     }
 }
 exports.ManagedGitHubApps = ManagedGitHubApps;
 _c = JSII_RTTI_SYMBOL_1;
 ManagedGitHubApps[_c] = {
     fqn: "@catnekaise/ghrawel.ManagedGitHubApps",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 class SelfManagedGitHubApps extends BaseGitHubApps {
     constructor(scope, id, props) {
         super(scope, id, props);
     }
     // @ts-ignore
     grantAccess(principal) {
         return undefined;
     }
 }
 exports.SelfManagedGitHubApps = SelfManagedGitHubApps;
 _d = JSII_RTTI_SYMBOL_1;
 SelfManagedGitHubApps[_d] = {
     fqn: "@catnekaise/ghrawel.SelfManagedGitHubApps",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 class InitializedParameter extends custom_resources_1.AwsCustomResource {
     constructor(scope, name, parameterName, kmsKey, removalPolicy) {
         const region = aws_cdk_lib_1.Stack.of(scope).region;
         const account = aws_cdk_lib_1.Stack.of(scope).account;
         const policies = [
             new iam.PolicyStatement({
```

##### package/lib/token-provider/configurator.js

###### js-beautify {}

```diff
@@ -219,15 +219,15 @@
         });
     }
 }
 exports.TokenProviderConfigurator = TokenProviderConfigurator;
 _a = JSII_RTTI_SYMBOL_1;
 TokenProviderConfigurator[_a] = {
     fqn: "@catnekaise/ghrawel.TokenProviderConfigurator",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 const PermissionObjectKeyRemaps = {
     actions: 'actions',
     administration: 'administration',
     checks: 'checks',
     codespaces: 'codespaces',
     contents: 'contents',
```

##### package/lib/token-provider/gha-abac.js

###### js-beautify {}

```diff
@@ -100,10 +100,10 @@
         }
     }
 }
 exports.TokenProviderPathStrategy = TokenProviderPathStrategy;
 _a = JSII_RTTI_SYMBOL_1;
 TokenProviderPathStrategy[_a] = {
     fqn: "@catnekaise/ghrawel.TokenProviderPathStrategy",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZ2hhLWFiYWMuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi8uLi9zcmMvdG9rZW4tcHJvdmlkZXIvZ2hhLWFiYWMudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSxJQUFZLCtCQUdYO0FBSEQsV0FBWSwrQkFBK0I7SUFDekMsNERBQXlCLENBQUE7SUFDekIsd0VBQXFDLENBQUE7QUFDdkMsQ0FBQyxFQUhXLCtCQUErQiwrQ0FBL0IsK0JBQStCLFFBRzFDO0FBRUQsSUFBWSw2QkFLWDtBQUxELFdBQVksNkJBQTZCO0lBQ3ZDLDBEQUF5QixDQUFBO0lBQ3pCLGtFQUFpQyxDQUFBO0lBQ2pDLGdEQUFlLENBQUE7SUFDZiw4REFBNkIsQ0FBQTtBQUMvQixDQUFDLEVBTFcsNkJBQTZCLDZDQUE3Qiw2QkFBNkIsUUFLeEM7QUFTRCxNQUFhLHlCQUF5QjtJQUVwQzs7T0FFRztJQUNILE1BQU0sQ0FBQyxtQkFBbUI7UUFDeEIsT0FBTyxJQUFJLHlCQUF5QixDQUFDO1lBQ25DLElBQUksRUFBRSw2QkFBNkIsQ0FBQyxVQUFVO1lBQzlDLFNBQVMsRUFBRSwrQkFBK0IsQ0FBQyxVQUFVO1NBQ3RELENBQUMsQ0FBQztJQUNMLENBQUM7SUFFRDs7T0FFRztJQUNILE1BQU0sQ0FBQyx3QkFBd0IsQ0FBQyxHQUFHLFlBQXNCO1FBQ3ZELE9BQU8sSUFBSSx5QkFBeUIsQ0FBQztZQUNuQyxJQUFJLEVBQUUsNkJBQTZCLENBQUMsVUFBVTtZQUM5QyxTQUFTLEVBQUUsK0JBQStCLENBQUMsZ0JBQWdCO1lBQzNELFlBQVk7U0FDYixDQUFDLENBQUM7SUFDTCxDQUFDO0lBRUQ7O09BRUc7SUFDSCxNQUFNLENBQUMsYUFBYTtRQUNsQixPQUFPLElBQUkseUJBQXlCLENBQUMsRUFBRSxJQUFJLEVBQUUsNkJBQTZCLENBQUMsY0FBYyxFQUFFLENBQUMsQ0FBQztJQUMvRixDQUFDO0lBRUQ7O09BRUc7SUFDSCxNQUFNLENBQUMsa0JBQWtCLENBQUMsS0FBYSxFQUFFLEdBQUcsWUFBc0I7UUFFaEUsSUFBSSxZQUFZLENBQUMsTUFBTSxLQUFLLENBQUMsRUFBRSxDQUFDO1lBQzlCLE1BQU0sSUFBSSxLQUFLLENBQUMsNkNBQTZDLENBQUMsQ0FBQztRQUNqRSxDQUFDO1FBRUQsT0FBTyxJQUFJLHlCQUF5QixDQUFDO1lBQ25DLElBQUksRUFBRSw2QkFBNkIsQ0FBQyxZQUFZO1lBQ2hELEtBQUs7WUFDTCxZQUFZO1NBQ2IsQ0FBQyxDQUFDO0lBQ0wsQ0FBQztJQUVEOztPQUVHO0lBQ0gsTUFBTSxDQUFDLFdBQVcsQ0FBQyxLQUFhO1FBQzlCLE9BQU8sSUFBSSx5QkFBeUIsQ0FBQztZQUNuQyxJQUFJLEVBQUUsNkJBQTZCLENBQUMsS0FBSztZQUN6QyxLQUFLO1NBQ04sQ0FBQyxDQUFDO0lBQ0wsQ0FBQztJQUVELFlBQXFDLFFBQThCO1FBQTlCLGFBQVEsR0FBUixRQUFRLENBQXNCO0lBQ25FLENBQUM7SUFFRCxJQUFJLElBQUk7UUFDTixPQUFPLElBQUksQ0FBQyxRQUFRLENBQUMsSUFBSSxDQUFDO0lBQzVCLENBQUM7SUFFRCxJQUFJLEtBQUs7UUFDUCxPQUFPLElBQUksQ0FBQyxRQUFRLENBQUMsS0FBSyxDQUFDO0lBQzdCLENBQUM7SUFFRCxJQUFJLFlBQVk7UUFDZCxPQUFPLElBQUksQ0FBQyxRQUFRLENBQUMsWUFBWSxJQUFJLEVBQUUsQ0FBQztJQUMxQyxDQUFDO0lBRUQsSUFBSSxTQUFTO1FBQ1gsT0FBTyxJQUFJLENBQUMsUUFBUSxDQUFDLFNBQVMsQ0FBQztJQUNqQyxDQUFDO0lBRUQsSUFBSSx1QkFBdUI7UUFFekIsUUFBUSxJQUFJLENBQUMsSUFBSSxFQUFFLENBQUM7WUFDbEIsS0FBSyw2QkFBNkIsQ0FBQyxVQUFVO2dCQUMzQyxJQUFJLElBQUksQ0FBQyxRQUFRLENBQUMsU0FBUyxLQUFLLCtCQUErQixDQUFDLFVBQVUsRUFBRSxDQUFDO29CQUMzRSxPQUFPLElBQUksQ0FBQztnQkFDZCxDQUFDO3FCQUFNLElBQUksSUFBSSxDQUFDLFFBQVEsQ0FBQyxTQUFTLEtBQUssK0JBQStCLENBQUMsZ0JBQWdCLEVBQUUsQ0FBQztvQkFDeEYsT0FBTyxJQUFJLENBQUMsWUFBWSxDQUFDLE1BQU0sR0FBRyxDQUFDLENBQUM7Z0JBQ3RDLENBQUM7Z0JBRUQsTUFBTSxJQUFJLEtBQUssQ0FBQyw4QkFBOEIsQ0FBQyxDQUFDO1lBQ2xELEtBQUssNkJBQTZCLENBQUMsY0FBYztnQkFDL0MsT0FBTyxLQUFLLENBQUM7WUFDZixLQUFLLDZCQUE2QixDQUFDLEtBQUs7Z0JBQ3RDLE9BQU8sS0FBSyxDQUFDO1lBRWYsS0FBSyw2QkFBNkIsQ0FBQyxZQUFZO2dCQUM3QyxPQUFPLElBQUksQ0FBQztRQUNoQixDQUFDO0lBQ0gsQ0FBQzs7QUE5RkgsOERBK0ZDIiwic291cmNlc0NvbnRlbnQiOlsiZXhwb3J0IGVudW0gVG9rZW5Qcm92aWRlclBhdGhQb2xpY3lWYXJpYWJsZSB7XG4gIFJFUE9TSVRPUlkgPSAnUkVQT1NJVE9SWScsXG4gIFJFUE9TSVRPUllfT1dORVIgPSAnUkVQT1NJVE9SWV9PV05FUicsXG59XG5cbmV4cG9ydCBlbnVtIFRva2VuUHJvdmlkZXJQYXRoU3RyYXRlZ3lUeXBlIHtcbiAgUE9MSUNZX1ZBUiA9ICdQT0xJQ1lfVkFSJyxcbiAgQU5ZX1JFUE9TSVRPUlkgPSAnQU5ZX1JFUE9TSVRPUlknLFxuICBPV05FUiA9ICdPV05FUicsXG4gIFJFUE9TSVRPUklFUyA9ICdSRVBPU0lUT1JJRVMnLFxufVxuXG5pbnRlcmZhY2UgUGF0aFN0cmF0ZWd5U2V0dGluZ3Mge1xuICByZWFkb25seSB0eXBlOiBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5VHlwZTtcbiAgcmVhZG9ubHkgcmVwb3NpdG9yaWVzPzogc3RyaW5nW107XG4gIHJlYWRvbmx5IG93bmVyPzogc3RyaW5nO1xuICByZWFkb25seSBwb2xpY3lWYXI/OiBUb2tlblByb3ZpZGVyUGF0aFBvbGljeVZhcmlhYmxlO1xufVxuXG5leHBvcnQgY2xhc3MgVG9rZW5Qcm92aWRlclBhdGhTdHJhdGVneSB7XG5cbiAgLyoqXG4gICAqIEdyYW50cyBwZXJtaXNzaW9uIHRvIGAveC88cHJvdmlkZXItbmFtZT4vJHthd3M6UHJpbmNpcGFsVGFnL3JlcG9zaXRvcnl9YFxuICAgKi9cbiAgc3RhdGljIHBvbGljeVZhclJlcG9zaXRvcnkoKTogVG9rZW5Qcm92aWRlclBhdGhTdHJhdGVneSB7XG4gICAgcmV0dXJuIG5ldyBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5KHtcbiAgICAgIHR5cGU6IFRva2VuUHJvdmlkZXJQYXRoU3RyYXRlZ3lUeXBlLlBPTElDWV9WQVIsXG4gICAgICBwb2xpY3lWYXI6IFRva2VuUHJvdmlkZXJQYXRoUG9saWN5VmFyaWFibGUuUkVQT1NJVE9SWSxcbiAgICB9KTtcbiAgfVxuXG4gIC8qKlxuICAgKiBHcmFudHMgcGVybWlzc2lvbiB0byBgL3gvPHByb3ZpZGVyLW5hbWU+LyR7YXdzOlByaW5jaXBhbFRhZy9yZXBvc2l0b3J5X293bmVyfWAgb3IgYC94Lzxwcm92aWRlci1uYW1lPi8ke2F3czpQcmluY2lwYWxUYWcvcmVwb3NpdG9yeV9vd25lcn0vPHJlcG8+YFxuICAgKi9cbiAgc3RhdGljIHBvbGljeVZhclJlcG9zaXRvcnlPd25lciguLi5yZXBvc2l0b3JpZXM6IHN0cmluZ1tdKTogVG9rZW5Qcm92aWRlclBhdGhTdHJhdGVneSB7XG4gICAgcmV0dXJuIG5ldyBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5KHtcbiAgICAgIHR5cGU6IFRva2VuUHJvdmlkZXJQYXRoU3RyYXRlZ3lUeXBlLlBPTElDWV9WQVIsXG4gICAgICBwb2xpY3lWYXI6IFRva2VuUHJvdmlkZXJQYXRoUG9saWN5VmFyaWFibGUuUkVQT1NJVE9SWV9PV05FUixcbiAgICAgIHJlcG9zaXRvcmllcyxcbiAgICB9KTtcbiAgfVxuXG4gIC8qKlxuICAgKiBHcmFudHMgcGVybWlzc2lvbiB0byBgL3gvPHByb3ZpZGVyLW5hbWU+LypgXG4gICAqL1xuICBzdGF0aWMgYW55UmVwb3NpdG9yeSgpOiBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5IHtcbiAgICByZXR1cm4gbmV3IFRva2VuUHJvdmlkZXJQYXRoU3RyYXRlZ3koeyB0eXBlOiBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5VHlwZS5BTllfUkVQT1NJVE9SWSB9KTtcbiAgfVxuXG4gIC8qKlxuICAgKiBHcmFudHMgcGVybWlzc2lvbiBmb3IgZWFjaCBzcGVjaWZpZWQgcmVwbyBgL3gvPHByb3ZpZGVyLW5hbWU+Lzxvd25lcj4vPHJlcG8+YFxuICAgKi9cbiAgc3RhdGljIHNlbGVjdFJlcG9zaXRvcmllcyhvd25lcjogc3RyaW5nLCAuLi5yZXBvc2l0b3JpZXM6IHN0cmluZ1tdKTogVG9rZW5Qcm92aWRlclBhdGhTdHJhdGVneSB7XG5cbiAgICBpZiAocmVwb3NpdG9yaWVzLmxlbmd0aCA9PT0gMCkge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKCdBdCBsZWFzdCBvbmUgcmVwb3NpdG9yeSBoYXMgdG8gYmUgc3BlY2lmaWVkJyk7XG4gICAgfVxuXG4gICAgcmV0dXJuIG5ldyBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5KHtcbiAgICAgIHR5cGU6IFRva2VuUHJvdmlkZXJQYXRoU3RyYXRlZ3lUeXBlLlJFUE9TSVRPUklFUyxcbiAgICAgIG93bmVyLFxuICAgICAgcmVwb3NpdG9yaWVzLFxuICAgIH0pO1xuICB9XG5cbiAgLyoqXG4gICAqIEdyYW50cyBwZXJtaXNzaW9uIHRvIGAveC88cHJvdmlkZXItbmFtZT4vPG93bmVyPmBcbiAgICovXG4gIHN0YXRpYyBzZWxlY3RPd25lcihvd25lcjogc3RyaW5nKTogVG9rZW5Qcm92aWRlclBhdGhTdHJhdGVneSB7XG4gICAgcmV0dXJuIG5ldyBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5KHtcbiAgICAgIHR5cGU6IFRva2VuUHJvdmlkZXJQYXRoU3RyYXRlZ3lUeXBlLk9XTkVSLFxuICAgICAgb3duZXIsXG4gICAgfSk7XG4gIH1cblxuICBwcml2YXRlIGNvbnN0cnVjdG9yKHByaXZhdGUgcmVhZG9ubHkgc2V0dGluZ3M6IFBhdGhTdHJhdGVneVNldHRpbmdzKSB7XG4gIH1cblxuICBnZXQgdHlwZSgpOiBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5VHlwZSB7XG4gICAgcmV0dXJuIHRoaXMuc2V0dGluZ3MudHlwZTtcbiAgfVxuXG4gIGdldCBvd25lcigpOiBzdHJpbmcgfCB1bmRlZmluZWQge1xuICAgIHJldHVybiB0aGlzLnNldHRpbmdzLm93bmVyO1xuICB9XG5cbiAgZ2V0IHJlcG9zaXRvcmllcygpOiBzdHJpbmdbXSB7XG4gICAgcmV0dXJuIHRoaXMuc2V0dGluZ3MucmVwb3NpdG9yaWVzID8/IFtdO1xuICB9XG5cbiAgZ2V0IHBvbGljeVZhcigpOiBUb2tlblByb3ZpZGVyUGF0aFBvbGljeVZhcmlhYmxlIHwgdW5kZWZpbmVkIHtcbiAgICByZXR1cm4gdGhpcy5zZXR0aW5ncy5wb2xpY3lWYXI7XG4gIH1cblxuICBnZXQgcGF0aFRhcmdldHNSZXBvc2l0b3JpZXMoKTogYm9vbGVhbiB7XG5cbiAgICBzd2l0Y2ggKHRoaXMudHlwZSkge1xuICAgICAgY2FzZSBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5VHlwZS5QT0xJQ1lfVkFSOlxuICAgICAgICBpZiAodGhpcy5zZXR0aW5ncy5wb2xpY3lWYXIgPT09IFRva2VuUHJvdmlkZXJQYXRoUG9saWN5VmFyaWFibGUuUkVQT1NJVE9SWSkge1xuICAgICAgICAgIHJldHVybiB0cnVlO1xuICAgICAgICB9IGVsc2UgaWYgKHRoaXMuc2V0dGluZ3MucG9saWN5VmFyID09PSBUb2tlblByb3ZpZGVyUGF0aFBvbGljeVZhcmlhYmxlLlJFUE9TSVRPUllfT1dORVIpIHtcbiAgICAgICAgICByZXR1cm4gdGhpcy5yZXBvc2l0b3JpZXMubGVuZ3RoID4gMDtcbiAgICAgICAgfVxuXG4gICAgICAgIHRocm93IG5ldyBFcnJvcignQ29uZmlndXJlIGEgdmFsaWQgcG9saWN5IHZhcicpO1xuICAgICAgY2FzZSBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5VHlwZS5BTllfUkVQT1NJVE9SWTpcbiAgICAgICAgcmV0dXJuIGZhbHNlO1xuICAgICAgY2FzZSBUb2tlblByb3ZpZGVyUGF0aFN0cmF0ZWd5VHlwZS5PV05FUjpcbiAgICAgICAgcmV0dXJuIGZhbHNlO1xuXG4gICAgICBjYXNlIFRva2VuUHJvdmlkZXJQYXRoU3RyYXRlZ3lUeXBlLlJFUE9TSVRPUklFUzpcbiAgICAgICAgcmV0dXJuIHRydWU7XG4gICAgfVxuICB9XG59XG4iXX0=
```

##### package/lib/token-provider/lambda-code.js

###### js-beautify {}

```diff
@@ -16,15 +16,15 @@
         this.name = name;
     }
 }
 exports.ApplicationArchitecture = ApplicationArchitecture;
 _a = JSII_RTTI_SYMBOL_1;
 ApplicationArchitecture[_a] = {
     fqn: "@catnekaise/ghrawel.ApplicationArchitecture",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 ApplicationArchitecture.X86_64 = new ApplicationArchitecture('x86_64');
 ApplicationArchitecture.ARM_64 = new ApplicationArchitecture('arm64');
 class TokenProviderLambdaCode {
     static defaultGo(options) {
         const architecture = options?.architecture ?? lambda.Architecture.X86_64;
         return lambda.Code.fromDockerBuild(path.join(__dirname, '../../lambda/default'), {
@@ -57,10 +57,10 @@
         return args;
     }
 }
 exports.TokenProviderLambdaCode = TokenProviderLambdaCode;
 _b = JSII_RTTI_SYMBOL_1;
 TokenProviderLambdaCode[_b] = {
     fqn: "@catnekaise/ghrawel.TokenProviderLambdaCode",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoibGFtYmRhLWNvZGUuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi8uLi9zcmMvdG9rZW4tcHJvdmlkZXIvbGFtYmRhLWNvZGUudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSxrQ0FBa0M7QUFDbEMsaURBQWlEO0FBRWpEOzs7R0FHRztBQUNILE1BQWEsdUJBQXVCO0lBS2xDLFlBQW9DLElBQVk7UUFBWixTQUFJLEdBQUosSUFBSSxDQUFRO0lBQ2hELENBQUM7O0FBTkgsMERBT0M7OztBQUxpQiw4QkFBTSxHQUFHLElBQUksdUJBQXVCLENBQUMsUUFBUSxDQUFDLENBQUM7QUFDL0MsOEJBQU0sR0FBRyxJQUFJLHVCQUF1QixDQUFDLE9BQU8sQ0FBQyxDQUFDO0FBbUNoRSxNQUFzQix1QkFBdUI7SUFFM0MsTUFBTSxDQUFDLFNBQVMsQ0FBQyxPQUF3QztRQUV2RCxNQUFNLFlBQVksR0FBRyxPQUFPLEVBQUUsWUFBWSxJQUFJLE1BQU0sQ0FBQyxZQUFZLENBQUMsTUFBTSxDQUFDO1FBRXpFLE9BQU8sTUFBTSxDQUFDLElBQUksQ0FBQyxlQUFlLENBQUMsSUFBSSxDQUFDLElBQUksQ0FBQyxTQUFTLEVBQUUsc0JBQXNCLENBQUMsRUFBRTtZQUMvRSxRQUFRLEVBQUUsT0FBTyxFQUFFLFFBQVE7WUFDM0IsU0FBUyxFQUFFO2dCQUNULElBQUksRUFBRSxZQUFZLENBQUMsSUFBSSxLQUFLLE9BQU8sQ0FBQyxDQUFDLENBQUMsT0FBTyxDQUFDLENBQUMsQ0FBQyxPQUFPO2dCQUN2RCxHQUFHLElBQUksQ0FBQyxhQUFhLENBQUMsT0FBTyxFQUFFLFVBQVUsRUFBRSxPQUFPLEVBQUUsUUFBUSxDQUFDO2FBQzlEO1NBQ0YsQ0FBQyxDQUFDO0lBQ0wsQ0FBQztJQUVELE1BQU0sQ0FBQyxNQUFNLENBQUMsT0FBd0M7UUFFcEQsTUFBTSxZQUFZLEdBQUcsT0FBTyxFQUFFLFlBQVksSUFBSSxNQUFNLENBQUMsWUFBWSxDQUFDLE1BQU0sQ0FBQztRQUV6RSxPQUFPLE1BQU0sQ0FBQyxJQUFJLENBQUMsZUFBZSxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsU0FBUyxFQUFFLHFCQUFxQixDQUFDLEVBQUU7WUFDOUUsUUFBUSxFQUFFLE9BQU8sRUFBRSxRQUFRO1lBQzNCLFNBQVMsRUFBRTtnQkFDVCxTQUFTLEVBQUUsVUFBVSxZQUFZLENBQUMsSUFBSSxFQUFFO2dCQUN4QyxJQUFJLEVBQUUsWUFBWSxDQUFDLElBQUksS0FBSyxPQUFPLENBQUMsQ0FBQyxDQUFDLGFBQWEsQ0FBQyxDQUFDLENBQUMsV0FBVztnQkFDakUsR0FBRyxJQUFJLENBQUMsYUFBYSxDQUFDLE9BQU8sRUFBRSxVQUFVLEVBQUUsT0FBTyxFQUFFLFFBQVEsQ0FBQzthQUM5RDtTQUNGLENBQUMsQ0FBQztJQUNMLENBQUM7SUFFTyxNQUFNLENBQUMsYUFBYSxDQUFDLElBQWEsRUFBRSxRQUFpQjtRQUUzRCxNQUFNLElBQUksR0FBOEIsRUFBRSxDQUFDO1FBRTNDLElBQUksSUFBSSxFQUFFLENBQUM7WUFDVCxJQUFJLENBQUMsUUFBUSxHQUFHLElBQUksQ0FBQztRQUN2QixDQUFDO1FBRUQsSUFBSSxRQUFRLEVBQUUsQ0FBQztZQUNiLElBQUksQ0FBQyxZQUFZLEdBQUcsUUFBUSxDQUFDO1FBQy9CLENBQUM7UUFFRCxPQUFPLElBQUksQ0FBQztJQUNkLENBQUM7O0FBMUNILDBEQTJDQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCAqIGFzIHBhdGggZnJvbSAnbm9kZTpwYXRoJztcbmltcG9ydCAqIGFzIGxhbWJkYSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtbGFtYmRhJztcblxuLyoqXG4gKiBPbmx5IGFwcGxpY2FibGUgdG8gVG9rZW5Qcm92aWRlckxhbWJkYUNvZGVPcHRpb25zLlxuICogRW5zdXJlIHRoYXQgdGhlIGxhbWJkYSBmdW5jdGlvbiBhcmNoaXRlY3R1cmUgbWF0Y2hlcy5cbiAqL1xuZXhwb3J0IGNsYXNzIEFwcGxpY2F0aW9uQXJjaGl0ZWN0dXJlIHtcblxuICBzdGF0aWMgcmVhZG9ubHkgWDg2XzY0ID0gbmV3IEFwcGxpY2F0aW9uQXJjaGl0ZWN0dXJlKCd4ODZfNjQnKTtcbiAgc3RhdGljIHJlYWRvbmx5IEFSTV82NCA9IG5ldyBBcHBsaWNhdGlvbkFyY2hpdGVjdHVyZSgnYXJtNjQnKTtcblxuICBwcml2YXRlIGNvbnN0cnVjdG9yKHB1YmxpYyByZWFkb25seSBuYW1lOiBzdHJpbmcpIHtcbiAgfVxufVxuXG4vKipcbiAqIFVzZSB0aGlzIHRvIGJ1aWxkIGEgc3VwcG9ydGVkIHRoZSBUb2tlblByb3ZpZGVyIGxhbWJkYSBhcHBsaWNhdGlvbiB3aGVuIHRoZSBzb3VyY2UgaXMgbG9jYXRlZCBpbiBhIHB1YmxpYyByZXBvc2l0b3J5LlxuICovXG5leHBvcnQgaW50ZXJmYWNlIFRva2VuUHJvdmlkZXJMYW1iZGFDb2RlT3B0aW9ucyB7XG5cbiAgLyoqXG4gICAqIFJlcG9zaXRvcnkgVXJsXG4gICAqIEV4YW1wbGU6IGh0dHBzOi8vZ2l0aHViLmNvbS9jYXRuZWthaXNlL2V4YW1wbGUtZm9yay5naXRcbiAgICovXG4gIHJlYWRvbmx5IHJlcG9zaXRvcnk/OiBzdHJpbmc7XG5cbiAgLyoqXG4gICAqIFZhbHVlIGZvciBgZ2l0IGNoZWNrb3V0YCBhZnRlciBjbG9uaW5nIHRoZSByZXBvc2l0b3J5XG4gICAqIEV4YW1wbGU6IG1haW4sIG9yaWdpbi9mZWF0dXJlMSwgU0hBXG4gICAqL1xuICByZWFkb25seSBjaGVja291dD86IHN0cmluZztcblxuICAvKipcbiAgICogU2hvdWxkIGJlIGVxdWFsIHRvIHRoZSBhcmNoaXRlY3R1cmUgY29uZmlndXJlZCBmb3IgdGhlIGxhbWJkYSBmdW5jdGlvbi4gVGhpcyB2YWx1ZSBpcyB1c2VkIHRvIGJ1aWxkIHRoZSBhcHBsaWNhdGlvbiBpbiB0aGUgc3BlY2lmaWVkIGFyY2hpdGVjdHVyZS5cbiAgICovXG4gIHJlYWRvbmx5IGFyY2hpdGVjdHVyZT86IEFwcGxpY2F0aW9uQXJjaGl0ZWN0dXJlO1xuXG4gIC8qKlxuICAgKiBWYWx1ZSBmb3IgZG9ja2VyIHBsYXRmb3JtXG4gICAqIEV4YW1wbGU6IGxpbnV4L2FtZDY0XG4gICAqL1xuICByZWFkb25seSBwbGF0Zm9ybT86IHN0cmluZztcbn1cblxuZXhwb3J0IGFic3RyYWN0IGNsYXNzIFRva2VuUHJvdmlkZXJMYW1iZGFDb2RlIHtcblxuICBzdGF0aWMgZGVmYXVsdEdvKG9wdGlvbnM/OiBUb2tlblByb3ZpZGVyTGFtYmRhQ29kZU9wdGlvbnMpOiBsYW1iZGEuQ29kZSB7XG5cbiAgICBjb25zdCBhcmNoaXRlY3R1cmUgPSBvcHRpb25zPy5hcmNoaXRlY3R1cmUgPz8gbGFtYmRhLkFyY2hpdGVjdHVyZS5YODZfNjQ7XG5cbiAgICByZXR1cm4gbGFtYmRhLkNvZGUuZnJvbURvY2tlckJ1aWxkKHBhdGguam9pbihfX2Rpcm5hbWUsICcuLi8uLi9sYW1iZGEvZGVmYXVsdCcpLCB7XG4gICAgICBwbGF0Zm9ybTogb3B0aW9ucz8ucGxhdGZvcm0sXG4gICAgICBidWlsZEFyZ3M6IHtcbiAgICAgICAgQVJDSDogYXJjaGl0ZWN0dXJlLm5hbWUgPT09ICdhcm02NCcgPyAnYXJtNjQnIDogJ2FtZDY0JyxcbiAgICAgICAgLi4udGhpcy5yZXBvQnVpbGRBcmdzKG9wdGlvbnM/LnJlcG9zaXRvcnksIG9wdGlvbnM/LmNoZWNrb3V0KSxcbiAgICAgIH0sXG4gICAgfSk7XG4gIH1cblxuICBzdGF0aWMgZG90bmV0KG9wdGlvbnM/OiBUb2tlblByb3ZpZGVyTGFtYmRhQ29kZU9wdGlvbnMpOiBsYW1iZGEuQ29kZSB7XG5cbiAgICBjb25zdCBhcmNoaXRlY3R1cmUgPSBvcHRpb25zPy5hcmNoaXRlY3R1cmUgPz8gbGFtYmRhLkFyY2hpdGVjdHVyZS5YODZfNjQ7XG5cbiAgICByZXR1cm4gbGFtYmRhLkNvZGUuZnJvbURvY2tlckJ1aWxkKHBhdGguam9pbihfX2Rpcm5hbWUsICcuLi8uLi9sYW1iZGEvZG90bmV0JyksIHtcbiAgICAgIHBsYXRmb3JtOiBvcHRpb25zPy5wbGF0Zm9ybSxcbiAgICAgIGJ1aWxkQXJnczoge1xuICAgICAgICBJTUFHRV9UQUc6IGBsYXRlc3QtJHthcmNoaXRlY3R1cmUubmFtZX1gLFxuICAgICAgICBBUkNIOiBhcmNoaXRlY3R1cmUubmFtZSA9PT0gJ2FybTY0JyA/ICdsaW51eC1hcm02NCcgOiAnbGludXgteDY0JyxcbiAgICAgICAgLi4udGhpcy5yZXBvQnVpbGRBcmdzKG9wdGlvbnM/LnJlcG9zaXRvcnksIG9wdGlvbnM/LmNoZWNrb3V0KSxcbiAgICAgIH0sXG4gICAgfSk7XG4gIH1cblxuICBwcml2YXRlIHN0YXRpYyByZXBvQnVpbGRBcmdzKHJlcG8/OiBzdHJpbmcsIGNoZWNrb3V0Pzogc3RyaW5nKTogeyBba2V5OiBzdHJpbmddOiBzdHJpbmcgfSB7XG5cbiAgICBjb25zdCBhcmdzOiB7IFtrZXk6IHN0cmluZ106IHN0cmluZyB9ID0ge307XG5cbiAgICBpZiAocmVwbykge1xuICAgICAgYXJncy5HSVRfUkVQTyA9IHJlcG87XG4gICAgfVxuXG4gICAgaWYgKGNoZWNrb3V0KSB7XG4gICAgICBhcmdzLkdJVF9DSEVDS09VVCA9IGNoZWNrb3V0O1xuICAgIH1cblxuICAgIHJldHVybiBhcmdzO1xuICB9XG59XG4iXX0=
```

##### package/lib/token-provider/target.js

###### js-beautify {}

```diff
@@ -34,10 +34,10 @@
         this.settings = settings;
     }
 }
 exports.TokenProviderTargetRule = TokenProviderTargetRule;
 _a = JSII_RTTI_SYMBOL_1;
 TokenProviderTargetRule[_a] = {
     fqn: "@catnekaise/ghrawel.TokenProviderTargetRule",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoidGFyZ2V0LmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vLi4vc3JjL3Rva2VuLXByb3ZpZGVyL3RhcmdldC50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLElBQVksdUJBVVg7QUFWRCxXQUFZLHVCQUF1QjtJQUNqQzs7T0FFRztJQUNILHdEQUE2QixDQUFBO0lBRTdCOztPQUVHO0lBQ0gsc0RBQTJCLENBQUE7QUFDN0IsQ0FBQyxFQVZXLHVCQUF1Qix1Q0FBdkIsdUJBQXVCLFFBVWxDO0FBTUQsTUFBYSx1QkFBdUI7SUFFbEMsTUFBTSxDQUFDLFVBQVU7UUFDZixPQUFPLElBQUksdUJBQXVCLENBQUM7WUFDakMsSUFBSSxFQUFFLHVCQUF1QixDQUFDLFlBQVk7U0FDM0MsQ0FBQyxDQUFDO0lBQ0wsQ0FBQztJQUVELE1BQU0sQ0FBQyxVQUFVO1FBQ2YsT0FBTyxJQUFJLHVCQUF1QixDQUFDO1lBQ2pDLElBQUksRUFBRSx1QkFBdUIsQ0FBQyxXQUFXO1NBQzFDLENBQUMsQ0FBQztJQUNMLENBQUM7SUFFRCxJQUFJLHVCQUF1QjtRQUN6QixPQUFPLElBQUksQ0FBQyxRQUFRLENBQUMsSUFBSSxDQUFDO0lBQzVCLENBQUM7SUFFRCxZQUFxQyxRQUE0QjtRQUE1QixhQUFRLEdBQVIsUUFBUSxDQUFvQjtJQUNqRSxDQUFDOztBQW5CSCwwREFvQkMiLCJzb3VyY2VzQ29udGVudCI6WyJleHBvcnQgZW51bSBSZXBvc2l0b3J5U2VsZWN0aW9uTW9kZSB7XG4gIC8qKlxuICAgKiBBbGxvd3MgdGFyZ2V0aW5nIG9mIGFueSBpbmRpdmlkdWFsIG9yIG11bHRpcGxlIHJlcG9zLCBidXQgTk9UIHRoZSBvcmdhbml6YXRpb25cbiAgICovXG4gIEFUX0xFQVNUX09ORSA9ICdBVF9MRUFTVF9PTkUnLFxuXG4gIC8qKlxuICAgKiBBbGxvd3MgdGFyZ2V0aW5nIG9mIGFueSBpbmRpdmlkdWFsIG9yIG11bHRpcGxlIHJlcG9zIGFuZCB0aGUgb3JnYW5pemF0aW9uL3VzZXJcbiAgICovXG4gIEFMTE9XX09XTkVSID0gJ0FMTE9XX09XTkVSJyxcbn1cblxuZXhwb3J0IGludGVyZmFjZSBUYXJnZXRSdWxlU2V0dGluZ3Mge1xuICByZWFkb25seSBtb2RlOiBSZXBvc2l0b3J5U2VsZWN0aW9uTW9kZTtcbn1cblxuZXhwb3J0IGNsYXNzIFRva2VuUHJvdmlkZXJUYXJnZXRSdWxlIHtcblxuICBzdGF0aWMgYXRMZWFzdE9uZSgpOiBUb2tlblByb3ZpZGVyVGFyZ2V0UnVsZSB7XG4gICAgcmV0dXJuIG5ldyBUb2tlblByb3ZpZGVyVGFyZ2V0UnVsZSh7XG4gICAgICBtb2RlOiBSZXBvc2l0b3J5U2VsZWN0aW9uTW9kZS5BVF9MRUFTVF9PTkUsXG4gICAgfSk7XG4gIH1cblxuICBzdGF0aWMgYWxsb3dPd25lcigpOiBUb2tlblByb3ZpZGVyVGFyZ2V0UnVsZSB7XG4gICAgcmV0dXJuIG5ldyBUb2tlblByb3ZpZGVyVGFyZ2V0UnVsZSh7XG4gICAgICBtb2RlOiBSZXBvc2l0b3J5U2VsZWN0aW9uTW9kZS5BTExPV19PV05FUixcbiAgICB9KTtcbiAgfVxuXG4gIGdldCByZXBvc2l0b3J5U2VsZWN0aW9uTW9kZSgpOiBSZXBvc2l0b3J5U2VsZWN0aW9uTW9kZSB7XG4gICAgcmV0dXJuIHRoaXMuc2V0dGluZ3MubW9kZTtcbiAgfVxuXG4gIHByaXZhdGUgY29uc3RydWN0b3IocHJpdmF0ZSByZWFkb25seSBzZXR0aW5nczogVGFyZ2V0UnVsZVNldHRpbmdzKSB7XG4gIH1cbn1cblxuIl19
```

##### package/lib/token-provider/token-provider.js

###### js-beautify {}

```diff
@@ -41,15 +41,15 @@
         return [TokenProviderEndpointType.DYNAMIC_OWNER, TokenProviderEndpointType.STATIC_OWNER].includes(this.type);
     }
 }
 exports.TokenProviderEndpoint = TokenProviderEndpoint;
 _a = JSII_RTTI_SYMBOL_1;
 TokenProviderEndpoint[_a] = {
     fqn: "@catnekaise/ghrawel.TokenProviderEndpoint",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 /**
  * This construct may receive some changes before constructor is made public. Until then use static create method.
  */
 class TokenProvider extends constructs_1.Construct {
     static create(scope, id, settings) {
         return new TokenProvider(scope, id, settings);
@@ -219,15 +219,15 @@
         return this.method.httpMethod;
     }
 }
 exports.TokenProvider = TokenProvider;
 _b = JSII_RTTI_SYMBOL_1;
 TokenProvider[_b] = {
     fqn: "@catnekaise/ghrawel.TokenProvider",
-    version: "0.0.8"
+    version: "0.0.9"
 };
 class ProviderPermissions {
     static createExecuteArn(scope, input) {
         const {
             baseResourcePath,
             endpoint,
             owner: owner,
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -134,9 +134,9 @@
         "test": "npx projen test",
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

