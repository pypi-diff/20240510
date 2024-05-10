# Comparing `tmp/alibabacloud_elasticsearch20170613-1.4.0.tar.gz` & `tmp/alibabacloud_elasticsearch20170613-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_elasticsearch20170613-1.4.0.tar", last modified: Thu Mar  7 17:11:05 2024, max compression
+gzip compressed data, was "dist/alibabacloud_elasticsearch20170613-2.0.0.tar", last modified: Tue Apr 23 03:17:25 2024, max compression
```

## Comparing `alibabacloud_elasticsearch20170613-1.4.0.tar` & `alibabacloud_elasticsearch20170613-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     1786 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2471 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1135 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1220 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613/__init__.py
--rw-r--r--   0 root         (0) root         (0)   717810 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613/client.py
--rw-r--r--   0 root         (0) root         (0)  1256290 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2471 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-07 17:11:05.000000 alibabacloud_elasticsearch20170613-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2661 2024-03-07 17:11:04.000000 alibabacloud_elasticsearch20170613-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   711946 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613/client.py
+-rw-r--r--   0 root         (0) root         (0)  1236777 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2661 2024-04-23 03:17:25.000000 alibabacloud_elasticsearch20170613-2.0.0/setup.py
```

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/ChangeLog.md` & `alibabacloud_elasticsearch20170613-2.0.0/ChangeLog.md`

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
 - Generated python 2017-06-13 for elasticsearch.
```

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/LICENSE` & `alibabacloud_elasticsearch20170613-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/PKG-INFO` & `alibabacloud_elasticsearch20170613-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_elasticsearch20170613
-Version: 1.4.0
+Version: 2.0.0
 Summary: Alibaba Cloud Elasticsearch (20170613) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/README-CN.md` & `alibabacloud_elasticsearch20170613-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/README.md` & `alibabacloud_elasticsearch20170613-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613/client.py` & `alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1138,140 +1138,14 @@
         instance_id: str,
         request: elasticsearch_20170613_models.CreateDataStreamRequest,
     ) -> elasticsearch_20170613_models.CreateDataStreamResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_data_stream_with_options_async(instance_id, request, headers, runtime)
 
-    def create_data_tasks_with_options(
-        self,
-        instance_id: str,
-        request: elasticsearch_20170613_models.CreateDataTasksRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> elasticsearch_20170613_models.CreateDataTasksResponse:
-        """
-        @deprecated
-        Before you call this operation, note that:
-        *   Currently, the one-click index migration feature only supports the China (Beijing) region.
-        *   The source and destination Elasticsearch clusters must meet the following requirements: a user-created or Alibaba Cloud Elasticsearch Elasticsearch cluster with a source of version 6.7.0 and a Alibaba Cloud Elasticsearch Elasticsearch cluster with a destination of version 6.3.2 or 6.7.0.
-        
-        @param request: CreateDataTasksRequest
-        @param headers: map
-        @param runtime: runtime options for this request RuntimeOptions
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
-            pathname=f'/openapi/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/data-task',
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
-    async def create_data_tasks_with_options_async(
-        self,
-        instance_id: str,
-        request: elasticsearch_20170613_models.CreateDataTasksRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> elasticsearch_20170613_models.CreateDataTasksResponse:
-        """
-        @deprecated
-        Before you call this operation, note that:
-        *   Currently, the one-click index migration feature only supports the China (Beijing) region.
-        *   The source and destination Elasticsearch clusters must meet the following requirements: a user-created or Alibaba Cloud Elasticsearch Elasticsearch cluster with a source of version 6.7.0 and a Alibaba Cloud Elasticsearch Elasticsearch cluster with a destination of version 6.3.2 or 6.7.0.
-        
-        @param request: CreateDataTasksRequest
-        @param headers: map
-        @param runtime: runtime options for this request RuntimeOptions
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
-            pathname=f'/openapi/instances/{OpenApiUtilClient.get_encode_param(instance_id)}/data-task',
-            method='POST',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            elasticsearch_20170613_models.CreateDataTasksResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_data_tasks(
-        self,
-        instance_id: str,
-        request: elasticsearch_20170613_models.CreateDataTasksRequest,
-    ) -> elasticsearch_20170613_models.CreateDataTasksResponse:
-        """
-        @deprecated
-        Before you call this operation, note that:
-        *   Currently, the one-click index migration feature only supports the China (Beijing) region.
-        *   The source and destination Elasticsearch clusters must meet the following requirements: a user-created or Alibaba Cloud Elasticsearch Elasticsearch cluster with a source of version 6.7.0 and a Alibaba Cloud Elasticsearch Elasticsearch cluster with a destination of version 6.3.2 or 6.7.0.
-        
-        @param request: CreateDataTasksRequest
-        @return: CreateDataTasksResponse
-        Deprecated
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.create_data_tasks_with_options(instance_id, request, headers, runtime)
-
-    async def create_data_tasks_async(
-        self,
-        instance_id: str,
-        request: elasticsearch_20170613_models.CreateDataTasksRequest,
-    ) -> elasticsearch_20170613_models.CreateDataTasksResponse:
-        """
-        @deprecated
-        Before you call this operation, note that:
-        *   Currently, the one-click index migration feature only supports the China (Beijing) region.
-        *   The source and destination Elasticsearch clusters must meet the following requirements: a user-created or Alibaba Cloud Elasticsearch Elasticsearch cluster with a source of version 6.7.0 and a Alibaba Cloud Elasticsearch Elasticsearch cluster with a destination of version 6.3.2 or 6.7.0.
-        
-        @param request: CreateDataTasksRequest
-        @return: CreateDataTasksResponse
-        Deprecated
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.create_data_tasks_with_options_async(instance_id, request, headers, runtime)
-
     def create_ilmpolicy_with_options(
         self,
         instance_id: str,
         request: elasticsearch_20170613_models.CreateILMPolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> elasticsearch_20170613_models.CreateILMPolicyResponse:
```

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613/models.py` & `alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3861,579 +3861,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDataStreamResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateDataTasksRequestBodyMigrateConfig(TeaModel):
-    def __init__(
-        self,
-        source_filter_params: str = None,
-    ):
-        self.source_filter_params = source_filter_params
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.source_filter_params is not None:
-            result['sourceFilterParams'] = self.source_filter_params
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('sourceFilterParams') is not None:
-            self.source_filter_params = m.get('sourceFilterParams')
-        return self
-
-
-class CreateDataTasksRequestBodySinkCluster(TeaModel):
-    def __init__(
-        self,
-        data_source_type: str = None,
-        index: str = None,
-        mapping: str = None,
-        password: str = None,
-        routing: str = None,
-        settings: str = None,
-        type: str = None,
-        username: str = None,
-    ):
-        self.data_source_type = data_source_type
-        self.index = index
-        self.mapping = mapping
-        self.password = password
-        self.routing = routing
-        self.settings = settings
-        self.type = type
-        self.username = username
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        data_source_type: str = None,
-        endpoint: str = None,
-        index: str = None,
-        password: str = None,
-        type: str = None,
-        username: str = None,
-        vpc_id: str = None,
-        vpc_instance_id: str = None,
-        vpc_instance_port: int = None,
-    ):
-        self.data_source_type = data_source_type
-        self.endpoint = endpoint
-        self.index = index
-        self.password = password
-        self.type = type
-        self.username = username
-        self.vpc_id = vpc_id
-        self.vpc_instance_id = vpc_instance_id
-        self.vpc_instance_port = vpc_instance_port
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        migrate_config: CreateDataTasksRequestBodyMigrateConfig = None,
-        sink_cluster: CreateDataTasksRequestBodySinkCluster = None,
-        source_cluster: CreateDataTasksRequestBodySourceCluster = None,
-    ):
-        self.migrate_config = migrate_config
-        self.sink_cluster = sink_cluster
-        self.source_cluster = source_cluster
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
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        client_token: str = None,
-        body: List[CreateDataTasksRequestBody] = None,
-    ):
-        # es-cn-n6w1o1x0w001c\*\*\*\*\
-        self.client_token = client_token
-        self.body = body
-
-    def validate(self):
-        if self.body:
-            for k in self.body:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        data_source_type: str = None,
-        index: str = None,
-        mapping: str = None,
-        password: str = None,
-        routing: str = None,
-        settings: str = None,
-        type: str = None,
-        username: str = None,
-        vpc_id: str = None,
-        vpc_instance_id: str = None,
-        vpc_instance_port: str = None,
-    ):
-        self.data_source_type = data_source_type
-        # The settings configuration.
-        self.index = index
-        # The type of the target index.
-        self.mapping = mapping
-        # The name of the target index.
-        self.password = password
-        # The username of the destination cluster.
-        self.routing = routing
-        # Mapping configuration.
-        self.settings = settings
-        # The routing field. The primary key field is used by default.
-        self.type = type
-        # The ID of the Virtual Private Cloud to which the cluster belongs. If the cluster access address is a public domain name, you can not specify the private endpoint.
-        self.username = username
-        # The access port number of the cluster.
-        self.vpc_id = vpc_id
-        # The type of the target cluster.
-        self.vpc_instance_id = vpc_instance_id
-        # The instance ID of the cluster under the Virtual Private Cloud, or the ID of the SLB instance.
-        self.vpc_instance_port = vpc_instance_port
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        data_source_type: str = None,
-        endpoint: str = None,
-        index: str = None,
-        password: str = None,
-        type: str = None,
-        username: str = None,
-        vpc_id: str = None,
-        vpc_instance_id: str = None,
-        vpc_instance_port: int = None,
-    ):
-        # The information about the target cluster.
-        self.data_source_type = data_source_type
-        # The username of the source cluster.
-        self.endpoint = endpoint
-        # The type of the specified index.
-        self.index = index
-        # Specifies the indexes to be migrated.
-        self.password = password
-        # The public domain name of the cluster.
-        self.type = type
-        # The ID of the Virtual Private Cloud where the source cluster resides. If the cluster access address is a public domain name, you can not specify the private endpoint.
-        self.username = username
-        # The instance ID of the cluster under the Virtual Private Cloud, or the ID of the SLB instance.
-        self.vpc_id = vpc_id
-        # The access port number of the source cluster.
-        self.vpc_instance_id = vpc_instance_id
-        # The type of the source cluster. Default value: Elasticsearch.
-        self.vpc_instance_port = vpc_instance_port
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        sink_cluster: CreateDataTasksResponseBodyResultSinkCluster = None,
-        source_cluster: CreateDataTasksResponseBodyResultSourceCluster = None,
-    ):
-        # The access password of the target cluster.
-        self.sink_cluster = sink_cluster
-        # The access password of the source cluster.
-        self.source_cluster = source_cluster
-
-    def validate(self):
-        if self.sink_cluster:
-            self.sink_cluster.validate()
-        if self.source_cluster:
-            self.source_cluster.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        request_id: str = None,
-        result: List[CreateDataTasksResponseBodyResult] = None,
-    ):
-        # The result of the request.
-        self.request_id = request_id
-        # The information about the source cluster.
-        self.result = result
-
-    def validate(self):
-        if self.result:
-            for k in self.result:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: CreateDataTasksResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         client_token: str = None,
         body: str = None,
     ):
         self.client_token = client_token
```

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/alibabacloud_elasticsearch20170613.egg-info/PKG-INFO` & `alibabacloud_elasticsearch20170613-2.0.0/alibabacloud_elasticsearch20170613.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-elasticsearch20170613
-Version: 1.4.0
+Version: 2.0.0
 Summary: Alibaba Cloud Elasticsearch (20170613) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_elasticsearch20170613-1.4.0/setup.py` & `alibabacloud_elasticsearch20170613-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_elasticsearch20170613.
 
-Created on 07/03/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_elasticsearch20170613"
 NAME = "alibabacloud_elasticsearch20170613" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Elasticsearch (20170613) SDK Library for Python"
```

