# Comparing `tmp/alibabacloud_elasticsearch20170613_py2-1.4.0.tar.gz` & `tmp/alibabacloud_elasticsearch20170613_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_elasticsearch20170613_py2-1.4.0.tar", last modified: Thu Mar  7 17:10:47 2024, max compression
+gzip compressed data, was "dist/alibabacloud_elasticsearch20170613_py2-2.0.0.tar", last modified: Tue Apr 23 03:16:52 2024, max compression
```

## Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0.tar` & `alibabacloud_elasticsearch20170613_py2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     1739 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2532 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1146 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293525 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613/client.py
--rw-r--r--   0 root         (0) root         (0)  1265452 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2532 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      520 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-07 17:10:47.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2953 2024-03-07 17:10:46.000000 alibabacloud_elasticsearch20170613_py2-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   290910 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613/client.py
+-rw-r--r--   0 root         (0) root         (0)  1245805 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      520 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2953 2024-04-23 03:16:52.000000 alibabacloud_elasticsearch20170613_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/ChangeLog.md` & `alibabacloud_elasticsearch20170613_py2-2.0.0/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2024-03-07 Version: 1.4.0
+- Support API DisableKibanaPvlNetwork.
+- Support API EnableKibanaPvlNetwork.
+- Support API GetRegionalInstanceConfig.
+- Support API ListKibanaPvlNetwork.
+- Support API UpdateKibanaPvlNetwork.
+
+
 2024-02-21 Version: 1.3.0
 - Support API GetRegionalInstanceConfig.
 
 
 2023-11-28 Version: 1.2.0
 - Generated python2 2017-06-13 for elasticsearch.
```

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/LICENSE` & `alibabacloud_elasticsearch20170613_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/PKG-INFO` & `alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_elasticsearch20170613_py2
-Version: 1.4.0
+Name: alibabacloud-elasticsearch20170613-py2
+Version: 2.0.0
 Summary: Alibaba Cloud Elasticsearch (20170613) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/README-CN.md` & `alibabacloud_elasticsearch20170613_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/README.md` & `alibabacloud_elasticsearch20170613_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613/client.py` & `alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,74 +448,14 @@
         )
 
     def create_data_stream(self, instance_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_data_stream_with_options(instance_id, request, headers, runtime)
 
-    def create_data_tasks_with_options(self, instance_id, request, headers, runtime):
-        """
-        @deprecated
-        Before you call this operation, note that:
-        *   Currently, the one-click index migration feature only supports the China (Beijing) region.
-        *   The source and destination Elasticsearch clusters must meet the following requirements: a user-created or Alibaba Cloud Elasticsearch Elasticsearch cluster with a source of version 6.7.0 and a Alibaba Cloud Elasticsearch Elasticsearch cluster with a destination of version 6.3.2 or 6.7.0.
-        
-
-        @param request: CreateDataTasksRequest
-
-        @type headers: dict
-        @param headers: map
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: CreateDataTasksResponse
-        Deprecated
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.client_token):
-            query['ClientToken'] = request.client_token
-        req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_array(request.body)
-        )
-        params = open_api_models.Params(
-            action='CreateDataTasks',
-            version='2017-06-13',
-            protocol='HTTPS',
-            pathname='/openapi/instances/%s/data-task' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(instance_id)),
-            method='POST',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            elasticsearch_20170613_models.CreateDataTasksResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def create_data_tasks(self, instance_id, request):
-        """
-        @deprecated
-        Before you call this operation, note that:
-        *   Currently, the one-click index migration feature only supports the China (Beijing) region.
-        *   The source and destination Elasticsearch clusters must meet the following requirements: a user-created or Alibaba Cloud Elasticsearch Elasticsearch cluster with a source of version 6.7.0 and a Alibaba Cloud Elasticsearch Elasticsearch cluster with a destination of version 6.3.2 or 6.7.0.
-        
-
-        @param request: CreateDataTasksRequest
-
-        @return: CreateDataTasksResponse
-        Deprecated
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.create_data_tasks_with_options(instance_id, request, headers, runtime)
-
     def create_ilmpolicy_with_options(self, instance_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         req = open_api_models.OpenApiRequest(
             headers=headers,
```

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613/models.py` & `alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3408,513 +3408,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDataStreamResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateDataTasksRequestBodyMigrateConfig(TeaModel):
-    def __init__(self, source_filter_params=None):
-        self.source_filter_params = source_filter_params  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDataTasksRequestBodyMigrateConfig, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.source_filter_params is not None:
-            result['sourceFilterParams'] = self.source_filter_params
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('sourceFilterParams') is not None:
-            self.source_filter_params = m.get('sourceFilterParams')
-        return self
-
-
-class CreateDataTasksRequestBodySinkCluster(TeaModel):
-    def __init__(self, data_source_type=None, index=None, mapping=None, password=None, routing=None, settings=None,
-                 type=None, username=None):
-        self.data_source_type = data_source_type  # type: str
-        self.index = index  # type: str
-        self.mapping = mapping  # type: str
-        self.password = password  # type: str
-        self.routing = routing  # type: str
-        self.settings = settings  # type: str
-        self.type = type  # type: str
-        self.username = username  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDataTasksRequestBodySinkCluster, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data_source_type is not None:
-            result['dataSourceType'] = self.data_source_type
-        if self.index is not None:
-            result['index'] = self.index
-        if self.mapping is not None:
-            result['mapping'] = self.mapping
-        if self.password is not None:
-            result['password'] = self.password
-        if self.routing is not None:
-            result['routing'] = self.routing
-        if self.settings is not None:
-            result['settings'] = self.settings
-        if self.type is not None:
-            result['type'] = self.type
-        if self.username is not None:
-            result['username'] = self.username
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('dataSourceType') is not None:
-            self.data_source_type = m.get('dataSourceType')
-        if m.get('index') is not None:
-            self.index = m.get('index')
-        if m.get('mapping') is not None:
-            self.mapping = m.get('mapping')
-        if m.get('password') is not None:
-            self.password = m.get('password')
-        if m.get('routing') is not None:
-            self.routing = m.get('routing')
-        if m.get('settings') is not None:
-            self.settings = m.get('settings')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('username') is not None:
-            self.username = m.get('username')
-        return self
-
-
-class CreateDataTasksRequestBodySourceCluster(TeaModel):
-    def __init__(self, data_source_type=None, endpoint=None, index=None, password=None, type=None, username=None,
-                 vpc_id=None, vpc_instance_id=None, vpc_instance_port=None):
-        self.data_source_type = data_source_type  # type: str
-        self.endpoint = endpoint  # type: str
-        self.index = index  # type: str
-        self.password = password  # type: str
-        self.type = type  # type: str
-        self.username = username  # type: str
-        self.vpc_id = vpc_id  # type: str
-        self.vpc_instance_id = vpc_instance_id  # type: str
-        self.vpc_instance_port = vpc_instance_port  # type: int
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDataTasksRequestBodySourceCluster, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data_source_type is not None:
-            result['dataSourceType'] = self.data_source_type
-        if self.endpoint is not None:
-            result['endpoint'] = self.endpoint
-        if self.index is not None:
-            result['index'] = self.index
-        if self.password is not None:
-            result['password'] = self.password
-        if self.type is not None:
-            result['type'] = self.type
-        if self.username is not None:
-            result['username'] = self.username
-        if self.vpc_id is not None:
-            result['vpcId'] = self.vpc_id
-        if self.vpc_instance_id is not None:
-            result['vpcInstanceId'] = self.vpc_instance_id
-        if self.vpc_instance_port is not None:
-            result['vpcInstancePort'] = self.vpc_instance_port
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('dataSourceType') is not None:
-            self.data_source_type = m.get('dataSourceType')
-        if m.get('endpoint') is not None:
-            self.endpoint = m.get('endpoint')
-        if m.get('index') is not None:
-            self.index = m.get('index')
-        if m.get('password') is not None:
-            self.password = m.get('password')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('username') is not None:
-            self.username = m.get('username')
-        if m.get('vpcId') is not None:
-            self.vpc_id = m.get('vpcId')
-        if m.get('vpcInstanceId') is not None:
-            self.vpc_instance_id = m.get('vpcInstanceId')
-        if m.get('vpcInstancePort') is not None:
-            self.vpc_instance_port = m.get('vpcInstancePort')
-        return self
-
-
-class CreateDataTasksRequestBody(TeaModel):
-    def __init__(self, migrate_config=None, sink_cluster=None, source_cluster=None):
-        self.migrate_config = migrate_config  # type: CreateDataTasksRequestBodyMigrateConfig
-        self.sink_cluster = sink_cluster  # type: CreateDataTasksRequestBodySinkCluster
-        self.source_cluster = source_cluster  # type: CreateDataTasksRequestBodySourceCluster
-
-    def validate(self):
-        if self.migrate_config:
-            self.migrate_config.validate()
-        if self.sink_cluster:
-            self.sink_cluster.validate()
-        if self.source_cluster:
-            self.source_cluster.validate()
-
-    def to_map(self):
-        _map = super(CreateDataTasksRequestBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.migrate_config is not None:
-            result['migrateConfig'] = self.migrate_config.to_map()
-        if self.sink_cluster is not None:
-            result['sinkCluster'] = self.sink_cluster.to_map()
-        if self.source_cluster is not None:
-            result['sourceCluster'] = self.source_cluster.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('migrateConfig') is not None:
-            temp_model = CreateDataTasksRequestBodyMigrateConfig()
-            self.migrate_config = temp_model.from_map(m['migrateConfig'])
-        if m.get('sinkCluster') is not None:
-            temp_model = CreateDataTasksRequestBodySinkCluster()
-            self.sink_cluster = temp_model.from_map(m['sinkCluster'])
-        if m.get('sourceCluster') is not None:
-            temp_model = CreateDataTasksRequestBodySourceCluster()
-            self.source_cluster = temp_model.from_map(m['sourceCluster'])
-        return self
-
-
-class CreateDataTasksRequest(TeaModel):
-    def __init__(self, client_token=None, body=None):
-        # es-cn-n6w1o1x0w001c\*\*\*\*\
-        self.client_token = client_token  # type: str
-        self.body = body  # type: list[CreateDataTasksRequestBody]
-
-    def validate(self):
-        if self.body:
-            for k in self.body:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(CreateDataTasksRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
-        result['body'] = []
-        if self.body is not None:
-            for k in self.body:
-                result['body'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
-        self.body = []
-        if m.get('body') is not None:
-            for k in m.get('body'):
-                temp_model = CreateDataTasksRequestBody()
-                self.body.append(temp_model.from_map(k))
-        return self
-
-
-class CreateDataTasksResponseBodyResultSinkCluster(TeaModel):
-    def __init__(self, data_source_type=None, index=None, mapping=None, password=None, routing=None, settings=None,
-                 type=None, username=None, vpc_id=None, vpc_instance_id=None, vpc_instance_port=None):
-        self.data_source_type = data_source_type  # type: str
-        # The settings configuration.
-        self.index = index  # type: str
-        # The type of the target index.
-        self.mapping = mapping  # type: str
-        # The name of the target index.
-        self.password = password  # type: str
-        # The username of the destination cluster.
-        self.routing = routing  # type: str
-        # Mapping configuration.
-        self.settings = settings  # type: str
-        # The routing field. The primary key field is used by default.
-        self.type = type  # type: str
-        # The ID of the Virtual Private Cloud to which the cluster belongs. If the cluster access address is a public domain name, you can not specify the private endpoint.
-        self.username = username  # type: str
-        # The access port number of the cluster.
-        self.vpc_id = vpc_id  # type: str
-        # The type of the target cluster.
-        self.vpc_instance_id = vpc_instance_id  # type: str
-        # The instance ID of the cluster under the Virtual Private Cloud, or the ID of the SLB instance.
-        self.vpc_instance_port = vpc_instance_port  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDataTasksResponseBodyResultSinkCluster, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data_source_type is not None:
-            result['dataSourceType'] = self.data_source_type
-        if self.index is not None:
-            result['index'] = self.index
-        if self.mapping is not None:
-            result['mapping'] = self.mapping
-        if self.password is not None:
-            result['password'] = self.password
-        if self.routing is not None:
-            result['routing'] = self.routing
-        if self.settings is not None:
-            result['settings'] = self.settings
-        if self.type is not None:
-            result['type'] = self.type
-        if self.username is not None:
-            result['username'] = self.username
-        if self.vpc_id is not None:
-            result['vpcId'] = self.vpc_id
-        if self.vpc_instance_id is not None:
-            result['vpcInstanceId'] = self.vpc_instance_id
-        if self.vpc_instance_port is not None:
-            result['vpcInstancePort'] = self.vpc_instance_port
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('dataSourceType') is not None:
-            self.data_source_type = m.get('dataSourceType')
-        if m.get('index') is not None:
-            self.index = m.get('index')
-        if m.get('mapping') is not None:
-            self.mapping = m.get('mapping')
-        if m.get('password') is not None:
-            self.password = m.get('password')
-        if m.get('routing') is not None:
-            self.routing = m.get('routing')
-        if m.get('settings') is not None:
-            self.settings = m.get('settings')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('username') is not None:
-            self.username = m.get('username')
-        if m.get('vpcId') is not None:
-            self.vpc_id = m.get('vpcId')
-        if m.get('vpcInstanceId') is not None:
-            self.vpc_instance_id = m.get('vpcInstanceId')
-        if m.get('vpcInstancePort') is not None:
-            self.vpc_instance_port = m.get('vpcInstancePort')
-        return self
-
-
-class CreateDataTasksResponseBodyResultSourceCluster(TeaModel):
-    def __init__(self, data_source_type=None, endpoint=None, index=None, password=None, type=None, username=None,
-                 vpc_id=None, vpc_instance_id=None, vpc_instance_port=None):
-        # The information about the target cluster.
-        self.data_source_type = data_source_type  # type: str
-        # The username of the source cluster.
-        self.endpoint = endpoint  # type: str
-        # The type of the specified index.
-        self.index = index  # type: str
-        # Specifies the indexes to be migrated.
-        self.password = password  # type: str
-        # The public domain name of the cluster.
-        self.type = type  # type: str
-        # The ID of the Virtual Private Cloud where the source cluster resides. If the cluster access address is a public domain name, you can not specify the private endpoint.
-        self.username = username  # type: str
-        # The instance ID of the cluster under the Virtual Private Cloud, or the ID of the SLB instance.
-        self.vpc_id = vpc_id  # type: str
-        # The access port number of the source cluster.
-        self.vpc_instance_id = vpc_instance_id  # type: str
-        # The type of the source cluster. Default value: Elasticsearch.
-        self.vpc_instance_port = vpc_instance_port  # type: int
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDataTasksResponseBodyResultSourceCluster, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data_source_type is not None:
-            result['dataSourceType'] = self.data_source_type
-        if self.endpoint is not None:
-            result['endpoint'] = self.endpoint
-        if self.index is not None:
-            result['index'] = self.index
-        if self.password is not None:
-            result['password'] = self.password
-        if self.type is not None:
-            result['type'] = self.type
-        if self.username is not None:
-            result['username'] = self.username
-        if self.vpc_id is not None:
-            result['vpcId'] = self.vpc_id
-        if self.vpc_instance_id is not None:
-            result['vpcInstanceId'] = self.vpc_instance_id
-        if self.vpc_instance_port is not None:
-            result['vpcInstancePort'] = self.vpc_instance_port
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('dataSourceType') is not None:
-            self.data_source_type = m.get('dataSourceType')
-        if m.get('endpoint') is not None:
-            self.endpoint = m.get('endpoint')
-        if m.get('index') is not None:
-            self.index = m.get('index')
-        if m.get('password') is not None:
-            self.password = m.get('password')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('username') is not None:
-            self.username = m.get('username')
-        if m.get('vpcId') is not None:
-            self.vpc_id = m.get('vpcId')
-        if m.get('vpcInstanceId') is not None:
-            self.vpc_instance_id = m.get('vpcInstanceId')
-        if m.get('vpcInstancePort') is not None:
-            self.vpc_instance_port = m.get('vpcInstancePort')
-        return self
-
-
-class CreateDataTasksResponseBodyResult(TeaModel):
-    def __init__(self, sink_cluster=None, source_cluster=None):
-        # The access password of the target cluster.
-        self.sink_cluster = sink_cluster  # type: CreateDataTasksResponseBodyResultSinkCluster
-        # The access password of the source cluster.
-        self.source_cluster = source_cluster  # type: CreateDataTasksResponseBodyResultSourceCluster
-
-    def validate(self):
-        if self.sink_cluster:
-            self.sink_cluster.validate()
-        if self.source_cluster:
-            self.source_cluster.validate()
-
-    def to_map(self):
-        _map = super(CreateDataTasksResponseBodyResult, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.sink_cluster is not None:
-            result['sinkCluster'] = self.sink_cluster.to_map()
-        if self.source_cluster is not None:
-            result['sourceCluster'] = self.source_cluster.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('sinkCluster') is not None:
-            temp_model = CreateDataTasksResponseBodyResultSinkCluster()
-            self.sink_cluster = temp_model.from_map(m['sinkCluster'])
-        if m.get('sourceCluster') is not None:
-            temp_model = CreateDataTasksResponseBodyResultSourceCluster()
-            self.source_cluster = temp_model.from_map(m['sourceCluster'])
-        return self
-
-
-class CreateDataTasksResponseBody(TeaModel):
-    def __init__(self, request_id=None, result=None):
-        # The result of the request.
-        self.request_id = request_id  # type: str
-        # The information about the source cluster.
-        self.result = result  # type: list[CreateDataTasksResponseBodyResult]
-
-    def validate(self):
-        if self.result:
-            for k in self.result:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(CreateDataTasksResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        result['Result'] = []
-        if self.result is not None:
-            for k in self.result:
-                result['Result'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        self.result = []
-        if m.get('Result') is not None:
-            for k in m.get('Result'):
-                temp_model = CreateDataTasksResponseBodyResult()
-                self.result.append(temp_model.from_map(k))
-        return self
-
-
-class CreateDataTasksResponse(TeaModel):
-    def __init__(self, headers=None, status_code=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.status_code = status_code  # type: int
-        self.body = body  # type: CreateDataTasksResponseBody
-
-    def validate(self):
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(CreateDataTasksResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = CreateDataTasksResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class CreateILMPolicyRequest(TeaModel):
     def __init__(self, client_token=None, body=None):
         self.client_token = client_token  # type: str
         self.body = body  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/PKG-INFO` & `alibabacloud_elasticsearch20170613_py2-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-elasticsearch20170613-py2
-Version: 1.4.0
+Name: alibabacloud_elasticsearch20170613_py2
+Version: 2.0.0
 Summary: Alibaba Cloud Elasticsearch (20170613) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/alibabacloud_elasticsearch20170613_py2.egg-info/SOURCES.txt` & `alibabacloud_elasticsearch20170613_py2-2.0.0/alibabacloud_elasticsearch20170613_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_elasticsearch20170613_py2-1.4.0/setup.py` & `alibabacloud_elasticsearch20170613_py2-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_elasticsearch20170613_py2.
 
-Created on 07/03/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_elasticsearch20170613"
 NAME = "alibabacloud_elasticsearch20170613_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Elasticsearch (20170613) SDK Library for Python2"
```

