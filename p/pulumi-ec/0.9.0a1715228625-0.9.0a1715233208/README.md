# Comparing `tmp/pulumi_ec-0.9.0a1715228625.tar.gz` & `tmp/pulumi_ec-0.9.0a1715233208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ec-0.9.0a1715228625.tar", last modified: Thu May  9 04:31:33 2024, max compression
+gzip compressed data, was "pulumi_ec-0.9.0a1715233208.tar", last modified: Thu May  9 05:45:25 2024, max compression
```

## Comparing `pulumi_ec-0.9.0a1715228625.tar` & `pulumi_ec-0.9.0a1715233208.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:31:33.621639 pulumi_ec-0.9.0a1715228625/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-09 04:31:33.621639 pulumi_ec-0.9.0a1715228625/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:31:33.617639 pulumi_ec-0.9.0a1715228625/pulumi_ec/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   222209 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:31:33.621639 pulumi_ec-0.9.0a1715228625/pulumi_ec/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    56946 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_elasticsearch_keystore.py
--rw-r--r--   0 runner    (1001) docker     (127)    23082 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_traffic_filter_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_aws_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_azure_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_deployment_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15714 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_gcp_private_service_connect_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/get_traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)   296632 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec/snapshot_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:31:33.621639 pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-09 04:31:33.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-09 04:31:33.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:31:33.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:31:33.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 04:31:33.000000 pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 04:31:27.000000 pulumi_ec-0.9.0a1715228625/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:31:33.621639 pulumi_ec-0.9.0a1715228625/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/pulumi_ec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   222209 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56946 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_elasticsearch_keystore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23082 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_aws_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_azure_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15714 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_gcp_private_service_connect_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)   296632 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/snapshot_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/setup.cfg
```

### Comparing `pulumi_ec-0.9.0a1715228625/PKG-INFO` & `pulumi_ec-0.9.0a1715233208/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ec
-Version: 0.9.0a1715228625
+Version: 0.9.0a1715233208
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi,ec,elasticsearch,es,elastic,elasticcloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.9.0a1715228625/README.md` & `pulumi_ec-0.9.0a1715233208/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/__init__.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/_inputs.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/_utilities.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/config/__init__.pyi` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/config/vars.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_elasticsearch_keystore.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_elasticsearch_keystore.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_extension.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_traffic_filter.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/deployment_traffic_filter_association.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_aws_privatelink_endpoint.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_aws_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_azure_privatelink_endpoint.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_azure_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_deployment.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_deployment_templates.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_deployments.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_gcp_private_service_connect_endpoint.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_gcp_private_service_connect_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_stack.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_stack.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/get_traffic_filter.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_traffic_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/outputs.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/provider.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec/snapshot_repository.py` & `pulumi_ec-0.9.0a1715233208/pulumi_ec/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/PKG-INFO` & `pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ec
-Version: 0.9.0a1715228625
+Version: 0.9.0a1715233208
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi,ec,elasticsearch,es,elastic,elasticcloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.9.0a1715228625/pulumi_ec.egg-info/SOURCES.txt` & `pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715228625/pyproject.toml` & `pulumi_ec-0.9.0a1715233208/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_ec"
   description = "A Pulumi package for creating and managing ElasticCloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "ec", "elasticsearch", "es", "elastic", "elasticcloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.9.0a1715228625"
+  version = "0.9.0a1715233208"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-ec"
 
 [build-system]
```

