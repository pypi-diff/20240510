# Comparing `tmp/pulumi_ec-0.9.0a1715233208.tar.gz` & `tmp/pulumi_ec-0.9.0a1715303612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ec-0.9.0a1715233208.tar", last modified: Thu May  9 05:45:25 2024, max compression
+gzip compressed data, was "pulumi_ec-0.9.0a1715303612.tar", last modified: Fri May 10 01:29:47 2024, max compression
```

## Comparing `pulumi_ec-0.9.0a1715233208.tar` & `pulumi_ec-0.9.0a1715303612.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/pulumi_ec/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   222209 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    56946 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_elasticsearch_keystore.py
--rw-r--r--   0 runner    (1001) docker     (127)    23082 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_aws_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_azure_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15714 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_gcp_private_service_connect_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/get_traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)   296632 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec/snapshot_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 05:45:25.000000 pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 05:45:18.000000 pulumi_ec-0.9.0a1715233208/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:45:25.297719 pulumi_ec-0.9.0a1715233208/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:29:47.566381 pulumi_ec-0.9.0a1715303612/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-10 01:29:47.566381 pulumi_ec-0.9.0a1715303612/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:29:47.566381 pulumi_ec-0.9.0a1715303612/pulumi_ec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   222209 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:29:47.566381 pulumi_ec-0.9.0a1715303612/pulumi_ec/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54407 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_elasticsearch_keystore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23082 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_traffic_filter_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_aws_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_azure_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_deployment_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15714 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_gcp_private_service_connect_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/get_traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)   296632 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14217 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec/snapshot_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:29:47.566381 pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-10 01:29:47.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-10 01:29:47.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:29:47.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:29:47.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 01:29:47.000000 pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-10 01:29:41.000000 pulumi_ec-0.9.0a1715303612/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:29:47.566381 pulumi_ec-0.9.0a1715303612/setup.cfg
```

### Comparing `pulumi_ec-0.9.0a1715233208/PKG-INFO` & `pulumi_ec-0.9.0a1715303612/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ec
-Version: 0.9.0a1715233208
+Version: 0.9.0a1715303612
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi,ec,elasticsearch,es,elastic,elasticcloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.9.0a1715233208/README.md` & `pulumi_ec-0.9.0a1715303612/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/__init__.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/_inputs.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/_utilities.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/config/__init__.pyi` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/config/vars.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         :param pulumi.Input['DeploymentElasticsearchArgs'] elasticsearch: Elasticsearch cluster definition
         :param pulumi.Input[str] region: Elasticsearch Service (ESS) region where the deployment should be hosted. For Elastic Cloud Enterprise (ECE) installations, set to `"ece-region".
         :param pulumi.Input[str] version: Elastic Stack version to use for all of the deployment resources.
         :param pulumi.Input[str] alias: Deployment alias, affects the format of the resource URLs.
         :param pulumi.Input['DeploymentApmArgs'] apm: **DEPRECATED** APM cluster definition. This should only be used for deployments running a version lower than 8.0
         :param pulumi.Input['DeploymentEnterpriseSearchArgs'] enterprise_search: Enterprise Search cluster definition.
         :param pulumi.Input['DeploymentIntegrationsServerArgs'] integrations_server: Integrations Server cluster definition. Integrations Server replaces `apm` in Stack versions > 8.0
-        :param pulumi.Input['DeploymentKibanaArgs'] kibana: Kibana cluster definition. -> **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
+        :param pulumi.Input['DeploymentKibanaArgs'] kibana: Kibana cluster definition. > **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
                block, since not doing so might cause issues when modifying or upgrading the deployment.
-        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. ~> **Note** If the
+        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. > **Note** If the
                <code>instance_configuration_id</code> or <code>instance_configuration_version</code> fields are set for a specific
-               topology element, that element will not be updated. ~> **Note** Hardware migrations are not supported for deployments
+               topology element, that element will not be updated. > **Note** Hardware migrations are not supported for deployments
                with node types. To use this field, the deployment needs to be migrated to node roles first.
         :param pulumi.Input[str] name: Name for the deployment
         :param pulumi.Input['DeploymentObservabilityArgs'] observability: Observability settings that you can set to ship logs and metrics to a deployment. The target deployment can also be the
                current deployment itself by setting observability.deployment_id to `self`.
         :param pulumi.Input[str] request_id: Request ID to set when you create the deployment. Use it only when previous attempts return an error and `request_id` is
                returned as part of the error.
         :param pulumi.Input[bool] reset_elasticsearch_password: Explicitly resets the elasticsearch_password when true
@@ -182,30 +182,30 @@
     def integrations_server(self, value: Optional[pulumi.Input['DeploymentIntegrationsServerArgs']]):
         pulumi.set(self, "integrations_server", value)
 
     @property
     @pulumi.getter
     def kibana(self) -> Optional[pulumi.Input['DeploymentKibanaArgs']]:
         """
-        Kibana cluster definition. -> **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
+        Kibana cluster definition. > **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
         block, since not doing so might cause issues when modifying or upgrading the deployment.
         """
         return pulumi.get(self, "kibana")
 
     @kibana.setter
     def kibana(self, value: Optional[pulumi.Input['DeploymentKibanaArgs']]):
         pulumi.set(self, "kibana", value)
 
     @property
     @pulumi.getter(name="migrateToLatestHardware")
     def migrate_to_latest_hardware(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set to true, the deployment will be updated according to the latest deployment template values. ~> **Note** If the
+        When set to true, the deployment will be updated according to the latest deployment template values. > **Note** If the
         <code>instance_configuration_id</code> or <code>instance_configuration_version</code> fields are set for a specific
-        topology element, that element will not be updated. ~> **Note** Hardware migrations are not supported for deployments
+        topology element, that element will not be updated. > **Note** Hardware migrations are not supported for deployments
         with node types. To use this field, the deployment needs to be migrated to node roles first.
         """
         return pulumi.get(self, "migrate_to_latest_hardware")
 
     @migrate_to_latest_hardware.setter
     def migrate_to_latest_hardware(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "migrate_to_latest_hardware", value)
@@ -309,27 +309,22 @@
                  version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Deployment resources.
         :param pulumi.Input[str] alias: Deployment alias, affects the format of the resource URLs.
         :param pulumi.Input['DeploymentApmArgs'] apm: **DEPRECATED** APM cluster definition. This should only be used for deployments running a version lower than 8.0
         :param pulumi.Input[str] deployment_template_id: Deployment template identifier to create the deployment from. See the [full list](https://www.elastic.co/guide/en/cloud/current/ec-regions-templates-instances.html) of regions and deployment templates available in ESS.
         :param pulumi.Input['DeploymentElasticsearchArgs'] elasticsearch: Elasticsearch cluster definition
-        :param pulumi.Input[str] elasticsearch_password: Password for authenticating to the Elasticsearch resource. ~> **Note on deployment credentials** The
-               <code>elastic</code> user credentials are only available whilst creating a deployment. Importing a deployment will not
-               import the <code>elasticsearch_username</code> or <code>elasticsearch_password</code> attributes. ~> **Note on
-               deployment credentials in state** The <code>elastic</code> user credentials are stored in the state file as plain text.
-               Please follow the official Terraform recommendations regarding senstaive data in state.
         :param pulumi.Input[str] elasticsearch_username: Username for authenticating to the Elasticsearch resource.
         :param pulumi.Input['DeploymentEnterpriseSearchArgs'] enterprise_search: Enterprise Search cluster definition.
         :param pulumi.Input['DeploymentIntegrationsServerArgs'] integrations_server: Integrations Server cluster definition. Integrations Server replaces `apm` in Stack versions > 8.0
-        :param pulumi.Input['DeploymentKibanaArgs'] kibana: Kibana cluster definition. -> **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
+        :param pulumi.Input['DeploymentKibanaArgs'] kibana: Kibana cluster definition. > **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
                block, since not doing so might cause issues when modifying or upgrading the deployment.
-        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. ~> **Note** If the
+        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. > **Note** If the
                <code>instance_configuration_id</code> or <code>instance_configuration_version</code> fields are set for a specific
-               topology element, that element will not be updated. ~> **Note** Hardware migrations are not supported for deployments
+               topology element, that element will not be updated. > **Note** Hardware migrations are not supported for deployments
                with node types. To use this field, the deployment needs to be migrated to node roles first.
         :param pulumi.Input[str] name: Name for the deployment
         :param pulumi.Input['DeploymentObservabilityArgs'] observability: Observability settings that you can set to ship logs and metrics to a deployment. The target deployment can also be the
                current deployment itself by setting observability.deployment_id to `self`.
         :param pulumi.Input[str] region: Elasticsearch Service (ESS) region where the deployment should be hosted. For Elastic Cloud Enterprise (ECE) installations, set to `"ece-region".
         :param pulumi.Input[str] request_id: Request ID to set when you create the deployment. Use it only when previous attempts return an error and `request_id` is
                returned as part of the error.
@@ -433,21 +428,14 @@
     @elasticsearch.setter
     def elasticsearch(self, value: Optional[pulumi.Input['DeploymentElasticsearchArgs']]):
         pulumi.set(self, "elasticsearch", value)
 
     @property
     @pulumi.getter(name="elasticsearchPassword")
     def elasticsearch_password(self) -> Optional[pulumi.Input[str]]:
-        """
-        Password for authenticating to the Elasticsearch resource. ~> **Note on deployment credentials** The
-        <code>elastic</code> user credentials are only available whilst creating a deployment. Importing a deployment will not
-        import the <code>elasticsearch_username</code> or <code>elasticsearch_password</code> attributes. ~> **Note on
-        deployment credentials in state** The <code>elastic</code> user credentials are stored in the state file as plain text.
-        Please follow the official Terraform recommendations regarding senstaive data in state.
-        """
         return pulumi.get(self, "elasticsearch_password")
 
     @elasticsearch_password.setter
     def elasticsearch_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "elasticsearch_password", value)
 
     @property
@@ -486,30 +474,30 @@
     def integrations_server(self, value: Optional[pulumi.Input['DeploymentIntegrationsServerArgs']]):
         pulumi.set(self, "integrations_server", value)
 
     @property
     @pulumi.getter
     def kibana(self) -> Optional[pulumi.Input['DeploymentKibanaArgs']]:
         """
-        Kibana cluster definition. -> **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
+        Kibana cluster definition. > **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
         block, since not doing so might cause issues when modifying or upgrading the deployment.
         """
         return pulumi.get(self, "kibana")
 
     @kibana.setter
     def kibana(self, value: Optional[pulumi.Input['DeploymentKibanaArgs']]):
         pulumi.set(self, "kibana", value)
 
     @property
     @pulumi.getter(name="migrateToLatestHardware")
     def migrate_to_latest_hardware(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set to true, the deployment will be updated according to the latest deployment template values. ~> **Note** If the
+        When set to true, the deployment will be updated according to the latest deployment template values. > **Note** If the
         <code>instance_configuration_id</code> or <code>instance_configuration_version</code> fields are set for a specific
-        topology element, that element will not be updated. ~> **Note** Hardware migrations are not supported for deployments
+        topology element, that element will not be updated. > **Note** Hardware migrations are not supported for deployments
         with node types. To use this field, the deployment needs to be migrated to node roles first.
         """
         return pulumi.get(self, "migrate_to_latest_hardware")
 
     @migrate_to_latest_hardware.setter
     def migrate_to_latest_hardware(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "migrate_to_latest_hardware", value)
@@ -676,19 +664,19 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] alias: Deployment alias, affects the format of the resource URLs.
         :param pulumi.Input[pulumi.InputType['DeploymentApmArgs']] apm: **DEPRECATED** APM cluster definition. This should only be used for deployments running a version lower than 8.0
         :param pulumi.Input[str] deployment_template_id: Deployment template identifier to create the deployment from. See the [full list](https://www.elastic.co/guide/en/cloud/current/ec-regions-templates-instances.html) of regions and deployment templates available in ESS.
         :param pulumi.Input[pulumi.InputType['DeploymentElasticsearchArgs']] elasticsearch: Elasticsearch cluster definition
         :param pulumi.Input[pulumi.InputType['DeploymentEnterpriseSearchArgs']] enterprise_search: Enterprise Search cluster definition.
         :param pulumi.Input[pulumi.InputType['DeploymentIntegrationsServerArgs']] integrations_server: Integrations Server cluster definition. Integrations Server replaces `apm` in Stack versions > 8.0
-        :param pulumi.Input[pulumi.InputType['DeploymentKibanaArgs']] kibana: Kibana cluster definition. -> **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
+        :param pulumi.Input[pulumi.InputType['DeploymentKibanaArgs']] kibana: Kibana cluster definition. > **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
                block, since not doing so might cause issues when modifying or upgrading the deployment.
-        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. ~> **Note** If the
+        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. > **Note** If the
                <code>instance_configuration_id</code> or <code>instance_configuration_version</code> fields are set for a specific
-               topology element, that element will not be updated. ~> **Note** Hardware migrations are not supported for deployments
+               topology element, that element will not be updated. > **Note** Hardware migrations are not supported for deployments
                with node types. To use this field, the deployment needs to be migrated to node roles first.
         :param pulumi.Input[str] name: Name for the deployment
         :param pulumi.Input[pulumi.InputType['DeploymentObservabilityArgs']] observability: Observability settings that you can set to ship logs and metrics to a deployment. The target deployment can also be the
                current deployment itself by setting observability.deployment_id to `self`.
         :param pulumi.Input[str] region: Elasticsearch Service (ESS) region where the deployment should be hosted. For Elastic Cloud Enterprise (ECE) installations, set to `"ece-region".
         :param pulumi.Input[str] request_id: Request ID to set when you create the deployment. Use it only when previous attempts return an error and `request_id` is
                returned as part of the error.
@@ -845,27 +833,22 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] alias: Deployment alias, affects the format of the resource URLs.
         :param pulumi.Input[pulumi.InputType['DeploymentApmArgs']] apm: **DEPRECATED** APM cluster definition. This should only be used for deployments running a version lower than 8.0
         :param pulumi.Input[str] deployment_template_id: Deployment template identifier to create the deployment from. See the [full list](https://www.elastic.co/guide/en/cloud/current/ec-regions-templates-instances.html) of regions and deployment templates available in ESS.
         :param pulumi.Input[pulumi.InputType['DeploymentElasticsearchArgs']] elasticsearch: Elasticsearch cluster definition
-        :param pulumi.Input[str] elasticsearch_password: Password for authenticating to the Elasticsearch resource. ~> **Note on deployment credentials** The
-               <code>elastic</code> user credentials are only available whilst creating a deployment. Importing a deployment will not
-               import the <code>elasticsearch_username</code> or <code>elasticsearch_password</code> attributes. ~> **Note on
-               deployment credentials in state** The <code>elastic</code> user credentials are stored in the state file as plain text.
-               Please follow the official Terraform recommendations regarding senstaive data in state.
         :param pulumi.Input[str] elasticsearch_username: Username for authenticating to the Elasticsearch resource.
         :param pulumi.Input[pulumi.InputType['DeploymentEnterpriseSearchArgs']] enterprise_search: Enterprise Search cluster definition.
         :param pulumi.Input[pulumi.InputType['DeploymentIntegrationsServerArgs']] integrations_server: Integrations Server cluster definition. Integrations Server replaces `apm` in Stack versions > 8.0
-        :param pulumi.Input[pulumi.InputType['DeploymentKibanaArgs']] kibana: Kibana cluster definition. -> **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
+        :param pulumi.Input[pulumi.InputType['DeploymentKibanaArgs']] kibana: Kibana cluster definition. > **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
                block, since not doing so might cause issues when modifying or upgrading the deployment.
-        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. ~> **Note** If the
+        :param pulumi.Input[bool] migrate_to_latest_hardware: When set to true, the deployment will be updated according to the latest deployment template values. > **Note** If the
                <code>instance_configuration_id</code> or <code>instance_configuration_version</code> fields are set for a specific
-               topology element, that element will not be updated. ~> **Note** Hardware migrations are not supported for deployments
+               topology element, that element will not be updated. > **Note** Hardware migrations are not supported for deployments
                with node types. To use this field, the deployment needs to be migrated to node roles first.
         :param pulumi.Input[str] name: Name for the deployment
         :param pulumi.Input[pulumi.InputType['DeploymentObservabilityArgs']] observability: Observability settings that you can set to ship logs and metrics to a deployment. The target deployment can also be the
                current deployment itself by setting observability.deployment_id to `self`.
         :param pulumi.Input[str] region: Elasticsearch Service (ESS) region where the deployment should be hosted. For Elastic Cloud Enterprise (ECE) installations, set to `"ece-region".
         :param pulumi.Input[str] request_id: Request ID to set when you create the deployment. Use it only when previous attempts return an error and `request_id` is
                returned as part of the error.
@@ -935,21 +918,14 @@
         Elasticsearch cluster definition
         """
         return pulumi.get(self, "elasticsearch")
 
     @property
     @pulumi.getter(name="elasticsearchPassword")
     def elasticsearch_password(self) -> pulumi.Output[str]:
-        """
-        Password for authenticating to the Elasticsearch resource. ~> **Note on deployment credentials** The
-        <code>elastic</code> user credentials are only available whilst creating a deployment. Importing a deployment will not
-        import the <code>elasticsearch_username</code> or <code>elasticsearch_password</code> attributes. ~> **Note on
-        deployment credentials in state** The <code>elastic</code> user credentials are stored in the state file as plain text.
-        Please follow the official Terraform recommendations regarding senstaive data in state.
-        """
         return pulumi.get(self, "elasticsearch_password")
 
     @property
     @pulumi.getter(name="elasticsearchUsername")
     def elasticsearch_username(self) -> pulumi.Output[str]:
         """
         Username for authenticating to the Elasticsearch resource.
@@ -972,26 +948,26 @@
         """
         return pulumi.get(self, "integrations_server")
 
     @property
     @pulumi.getter
     def kibana(self) -> pulumi.Output[Optional['outputs.DeploymentKibana']]:
         """
-        Kibana cluster definition. -> **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
+        Kibana cluster definition. > **Note on disabling Kibana** While optional it is recommended deployments specify a Kibana
         block, since not doing so might cause issues when modifying or upgrading the deployment.
         """
         return pulumi.get(self, "kibana")
 
     @property
     @pulumi.getter(name="migrateToLatestHardware")
     def migrate_to_latest_hardware(self) -> pulumi.Output[Optional[bool]]:
         """
-        When set to true, the deployment will be updated according to the latest deployment template values. ~> **Note** If the
+        When set to true, the deployment will be updated according to the latest deployment template values. > **Note** If the
         <code>instance_configuration_id</code> or <code>instance_configuration_version</code> fields are set for a specific
-        topology element, that element will not be updated. ~> **Note** Hardware migrations are not supported for deployments
+        topology element, that element will not be updated. > **Note** Hardware migrations are not supported for deployments
         with node types. To use this field, the deployment needs to be migrated to node roles first.
         """
         return pulumi.get(self, "migrate_to_latest_hardware")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
```

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_elasticsearch_keystore.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_elasticsearch_keystore.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_extension.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_traffic_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/deployment_traffic_filter_association.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/deployment_traffic_filter_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_aws_privatelink_endpoint.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_aws_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_azure_privatelink_endpoint.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_azure_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployment_templates.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_deployment_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_deployments.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_gcp_private_service_connect_endpoint.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_gcp_private_service_connect_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_stack.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_stack.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/get_traffic_filter.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/get_traffic_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/outputs.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/provider.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  verbose: Optional[pulumi.Input[bool]] = None,
                  verbose_credentials: Optional[pulumi.Input[bool]] = None,
                  verbose_file: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] apikey: API Key to use for API authentication. The only valid authentication mechanism for the Elasticsearch Service.
-        :param pulumi.Input[str] endpoint: Endpoint where the terraform provider will point to. Defaults to "https://api.elastic-cloud.com".
         :param pulumi.Input[bool] insecure: Allow the provider to skip TLS validation on its outgoing HTTP calls.
         :param pulumi.Input[str] password: Password to use for API authentication. Available only when targeting ECE Installations or Elasticsearch Service
                Private.
         :param pulumi.Input[str] timeout: Timeout used for individual HTTP calls. Defaults to "1m".
         :param pulumi.Input[str] username: Username to use for API authentication. Available only when targeting ECE Installations or Elasticsearch Service
                Private.
         :param pulumi.Input[bool] verbose: When set, a "request.log" file will be written with all outgoing HTTP requests. Defaults to "false".
@@ -67,17 +66,14 @@
     @apikey.setter
     def apikey(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "apikey", value)
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[pulumi.Input[str]]:
-        """
-        Endpoint where the terraform provider will point to. Defaults to "https://api.elastic-cloud.com".
-        """
         return pulumi.get(self, "endpoint")
 
     @endpoint.setter
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
 
     @property
@@ -187,15 +183,14 @@
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] apikey: API Key to use for API authentication. The only valid authentication mechanism for the Elasticsearch Service.
-        :param pulumi.Input[str] endpoint: Endpoint where the terraform provider will point to. Defaults to "https://api.elastic-cloud.com".
         :param pulumi.Input[bool] insecure: Allow the provider to skip TLS validation on its outgoing HTTP calls.
         :param pulumi.Input[str] password: Password to use for API authentication. Available only when targeting ECE Installations or Elasticsearch Service
                Private.
         :param pulumi.Input[str] timeout: Timeout used for individual HTTP calls. Defaults to "1m".
         :param pulumi.Input[str] username: Username to use for API authentication. Available only when targeting ECE Installations or Elasticsearch Service
                Private.
         :param pulumi.Input[bool] verbose: When set, a "request.log" file will be written with all outgoing HTTP requests. Defaults to "false".
@@ -271,17 +266,14 @@
         API Key to use for API authentication. The only valid authentication mechanism for the Elasticsearch Service.
         """
         return pulumi.get(self, "apikey")
 
     @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Output[Optional[str]]:
-        """
-        Endpoint where the terraform provider will point to. Defaults to "https://api.elastic-cloud.com".
-        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[Optional[str]]:
         """
         Password to use for API authentication. Available only when targeting ECE Installations or Elasticsearch Service
```

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec/snapshot_repository.py` & `pulumi_ec-0.9.0a1715303612/pulumi_ec/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/PKG-INFO` & `pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ec
-Version: 0.9.0a1715233208
+Version: 0.9.0a1715303612
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi,ec,elasticsearch,es,elastic,elasticcloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.9.0a1715233208/pulumi_ec.egg-info/SOURCES.txt` & `pulumi_ec-0.9.0a1715303612/pulumi_ec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.9.0a1715233208/pyproject.toml` & `pulumi_ec-0.9.0a1715303612/pyproject.toml`

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
-  version = "0.9.0a1715233208"
+  version = "0.9.0a1715303612"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-ec"
 
 [build-system]
```

