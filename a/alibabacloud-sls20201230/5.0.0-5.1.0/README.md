# Comparing `tmp/alibabacloud_sls20201230-5.0.0.tar.gz` & `tmp/alibabacloud_sls20201230-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sls20201230-5.0.0.tar", last modified: Tue Feb  6 09:03:00 2024, max compression
+gzip compressed data, was "dist/alibabacloud_sls20201230-5.1.0.tar", last modified: Tue Apr  9 08:43:22 2024, max compression
```

## Comparing `alibabacloud_sls20201230-5.0.0.tar` & `alibabacloud_sls20201230-5.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/
--rw-r--r--   0 root         (0) root         (0)     3135 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2409 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230/__init__.py
--rw-r--r--   0 root         (0) root         (0)   646175 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230/client.py
--rw-r--r--   0 root         (0) root         (0)   568570 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2409 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2664 2024-02-06 09:03:00.000000 alibabacloud_sls20201230-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2409 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   663828 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230/client.py
+-rw-r--r--   0 root         (0) root         (0)   582683 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2409 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 08:43:22.000000 alibabacloud_sls20201230-5.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2664 2024-04-09 08:43:21.000000 alibabacloud_sls20201230-5.1.0/setup.py
```

### Comparing `alibabacloud_sls20201230-5.0.0/ChangeLog.md` & `alibabacloud_sls20201230-5.1.0/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-02-06 Version: 5.0.0
+- Generated python 2020-12-30 for Sls.
+
 2024-01-19 Version: 4.4.1
 - Generated python 2020-12-30 for Sls.
 
 2024-01-15 Version: 4.4.0
 - Generated python 2020-12-30 for Sls.
 
 2024-01-10 Version: 4.3.0
```

### Comparing `alibabacloud_sls20201230-5.0.0/LICENSE` & `alibabacloud_sls20201230-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-5.0.0/PKG-INFO` & `alibabacloud_sls20201230-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sls20201230
-Version: 5.0.0
+Version: 5.1.0
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230-5.0.0/README-CN.md` & `alibabacloud_sls20201230-5.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-5.0.0/README.md` & `alibabacloud_sls20201230-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230/client.py` & `alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
+        self._signature_algorithm = 'v2'
         self._endpoint_rule = 'central'
 
     def apply_config_to_machine_group_with_options(
         self,
         project: str,
         machine_group: str,
         config_name: str,
@@ -2774,21 +2775,119 @@
         project: str,
         request: sls_20201230_models.CreateScheduledSQLRequest,
     ) -> sls_20201230_models.CreateScheduledSQLResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_scheduled_sqlwith_options_async(project, request, headers, runtime)
 
+    def create_sql_instance_with_options(
+        self,
+        project: str,
+        request: sls_20201230_models.CreateSqlInstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.CreateSqlInstanceResponse:
+        UtilClient.validate_model(request)
+        host_map = {}
+        host_map['project'] = project
+        body = {}
+        if not UtilClient.is_unset(request.cu):
+            body['cu'] = request.cu
+        if not UtilClient.is_unset(request.use_as_default):
+            body['useAsDefault'] = request.use_as_default
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/sqlinstance',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.CreateSqlInstanceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def create_sql_instance_with_options_async(
+        self,
+        project: str,
+        request: sls_20201230_models.CreateSqlInstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.CreateSqlInstanceResponse:
+        UtilClient.validate_model(request)
+        host_map = {}
+        host_map['project'] = project
+        body = {}
+        if not UtilClient.is_unset(request.cu):
+            body['cu'] = request.cu
+        if not UtilClient.is_unset(request.use_as_default):
+            body['useAsDefault'] = request.use_as_default
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/sqlinstance',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.CreateSqlInstanceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def create_sql_instance(
+        self,
+        project: str,
+        request: sls_20201230_models.CreateSqlInstanceRequest,
+    ) -> sls_20201230_models.CreateSqlInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_sql_instance_with_options(project, request, headers, runtime)
+
+    async def create_sql_instance_async(
+        self,
+        project: str,
+        request: sls_20201230_models.CreateSqlInstanceRequest,
+    ) -> sls_20201230_models.CreateSqlInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_sql_instance_with_options_async(project, request, headers, runtime)
+
     def create_ticket_with_options(
         self,
+        request: sls_20201230_models.CreateTicketRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.CreateTicketResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.access_token_expiration_time):
+            query['accessTokenExpirationTime'] = request.access_token_expiration_time
+        if not UtilClient.is_unset(request.expiration_time):
+            query['expirationTime'] = request.expiration_time
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateTicket',
             version='2020-12-30',
             protocol='HTTPS',
             pathname=f'/tickets',
             method='POST',
@@ -2800,19 +2899,27 @@
         return TeaCore.from_map(
             sls_20201230_models.CreateTicketResponse(),
             self.execute(params, req, runtime)
         )
 
     async def create_ticket_with_options_async(
         self,
+        request: sls_20201230_models.CreateTicketRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.CreateTicketResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.access_token_expiration_time):
+            query['accessTokenExpirationTime'] = request.access_token_expiration_time
+        if not UtilClient.is_unset(request.expiration_time):
+            query['expirationTime'] = request.expiration_time
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateTicket',
             version='2020-12-30',
             protocol='HTTPS',
             pathname=f'/tickets',
             method='POST',
@@ -2822,23 +2929,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             sls_20201230_models.CreateTicketResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def create_ticket(self) -> sls_20201230_models.CreateTicketResponse:
+    def create_ticket(
+        self,
+        request: sls_20201230_models.CreateTicketRequest,
+    ) -> sls_20201230_models.CreateTicketResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_ticket_with_options(headers, runtime)
+        return self.create_ticket_with_options(request, headers, runtime)
 
-    async def create_ticket_async(self) -> sls_20201230_models.CreateTicketResponse:
+    async def create_ticket_async(
+        self,
+        request: sls_20201230_models.CreateTicketRequest,
+    ) -> sls_20201230_models.CreateTicketResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_ticket_with_options_async(headers, runtime)
+        return await self.create_ticket_with_options_async(request, headers, runtime)
 
     def delete_alert_with_options(
         self,
         project: str,
         alert_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -7434,16 +7547,14 @@
             body['powerSql'] = request.power_sql
         if not UtilClient.is_unset(request.query):
             body['query'] = request.query
         if not UtilClient.is_unset(request.reverse):
             body['reverse'] = request.reverse
         if not UtilClient.is_unset(request.session):
             body['session'] = request.session
-        if not UtilClient.is_unset(request.shard):
-            body['shard'] = request.shard
         if not UtilClient.is_unset(request.to):
             body['to'] = request.to
         if not UtilClient.is_unset(request.topic):
             body['topic'] = request.topic
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -7508,16 +7619,14 @@
             body['powerSql'] = request.power_sql
         if not UtilClient.is_unset(request.query):
             body['query'] = request.query
         if not UtilClient.is_unset(request.reverse):
             body['reverse'] = request.reverse
         if not UtilClient.is_unset(request.session):
             body['session'] = request.session
-        if not UtilClient.is_unset(request.shard):
-            body['shard'] = request.shard
         if not UtilClient.is_unset(request.to):
             body['to'] = request.to
         if not UtilClient.is_unset(request.topic):
             body['topic'] = request.topic
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -8754,14 +8863,144 @@
         @return: GetShipperStatusResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_shipper_status_with_options_async(project, logstore, shipper_name, request, headers, runtime)
 
+    def get_sls_service_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.GetSlsServiceResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetSlsService',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/slsservice',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.GetSlsServiceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_sls_service_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.GetSlsServiceResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetSlsService',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/slsservice',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.GetSlsServiceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_sls_service(self) -> sls_20201230_models.GetSlsServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_sls_service_with_options(headers, runtime)
+
+    async def get_sls_service_async(self) -> sls_20201230_models.GetSlsServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_sls_service_with_options_async(headers, runtime)
+
+    def get_sql_instance_with_options(
+        self,
+        project: str,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.GetSqlInstanceResponse:
+        host_map = {}
+        host_map['project'] = project
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/sqlinstance',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='array'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.GetSqlInstanceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_sql_instance_with_options_async(
+        self,
+        project: str,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.GetSqlInstanceResponse:
+        host_map = {}
+        host_map['project'] = project
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/sqlinstance',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='array'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.GetSqlInstanceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_sql_instance(
+        self,
+        project: str,
+    ) -> sls_20201230_models.GetSqlInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_sql_instance_with_options(project, headers, runtime)
+
+    async def get_sql_instance_async(
+        self,
+        project: str,
+    ) -> sls_20201230_models.GetSqlInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_sql_instance_with_options_async(project, headers, runtime)
+
     def list_alerts_with_options(
         self,
         project: str,
         request: sls_20201230_models.ListAlertsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListAlertsResponse:
@@ -9717,14 +9956,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListETLsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -9753,14 +9994,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListETLsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -10465,14 +10708,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListOSSExportsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -10501,14 +10746,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListOSSExportsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -10555,14 +10802,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListOSSHDFSExportsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -10591,14 +10840,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListOSSHDFSExportsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -10645,14 +10896,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListOSSIngestionsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -10681,14 +10934,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListOSSIngestionsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -10977,14 +11232,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListScheduledSQLsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -11013,14 +11270,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.ListScheduledSQLsResponse:
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -11448,14 +11707,72 @@
         logstore: str,
         shard: str,
     ) -> sls_20201230_models.MergeShardResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.merge_shard_with_options_async(project, logstore, shard, headers, runtime)
 
+    def open_sls_service_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.OpenSlsServiceResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='OpenSlsService',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/slsservice',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.OpenSlsServiceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def open_sls_service_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.OpenSlsServiceResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='OpenSlsService',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/slsservice',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.OpenSlsServiceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def open_sls_service(self) -> sls_20201230_models.OpenSlsServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.open_sls_service_with_options(headers, runtime)
+
+    async def open_sls_service_async(self) -> sls_20201230_models.OpenSlsServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.open_sls_service_with_options_async(headers, runtime)
+
     def put_annotation_data_with_options(
         self,
         dataset_id: str,
         request: sls_20201230_models.PutAnnotationDataRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.PutAnnotationDataResponse:
@@ -11800,15 +12117,15 @@
         )
         params = open_api_models.Params(
             action='PutWebtracking',
             version='2020-12-30',
             protocol='HTTPS',
             pathname=f'/logstores/{logstore_name}/track',
             method='POST',
-            auth_type='AK',
+            auth_type='Anonymous',
             style='ROA',
             req_body_type='json',
             body_type='none'
         )
         return TeaCore.from_map(
             sls_20201230_models.PutWebtrackingResponse(),
             self.execute(params, req, runtime)
@@ -11856,15 +12173,15 @@
         )
         params = open_api_models.Params(
             action='PutWebtracking',
             version='2020-12-30',
             protocol='HTTPS',
             pathname=f'/logstores/{logstore_name}/track',
             method='POST',
-            auth_type='AK',
+            auth_type='Anonymous',
             style='ROA',
             req_body_type='json',
             body_type='none'
         )
         return TeaCore.from_map(
             sls_20201230_models.PutWebtrackingResponse(),
             await self.execute_async(params, req, runtime)
@@ -12026,14 +12343,94 @@
         @return: QueryMLServiceResultsResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.query_mlservice_results_with_options_async(service_name, request, headers, runtime)
 
+    def refresh_token_with_options(
+        self,
+        request: sls_20201230_models.RefreshTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.RefreshTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.access_token_expiration_time):
+            query['accessTokenExpirationTime'] = request.access_token_expiration_time
+        if not UtilClient.is_unset(request.ticket):
+            query['ticket'] = request.ticket
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RefreshToken',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/token/refresh',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.RefreshTokenResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def refresh_token_with_options_async(
+        self,
+        request: sls_20201230_models.RefreshTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.RefreshTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.access_token_expiration_time):
+            query['accessTokenExpirationTime'] = request.access_token_expiration_time
+        if not UtilClient.is_unset(request.ticket):
+            query['ticket'] = request.ticket
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RefreshToken',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/token/refresh',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.RefreshTokenResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def refresh_token(
+        self,
+        request: sls_20201230_models.RefreshTokenRequest,
+    ) -> sls_20201230_models.RefreshTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.refresh_token_with_options(request, headers, runtime)
+
+    async def refresh_token_async(
+        self,
+        request: sls_20201230_models.RefreshTokenRequest,
+    ) -> sls_20201230_models.RefreshTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.refresh_token_with_options_async(request, headers, runtime)
+
     def remove_config_from_machine_group_with_options(
         self,
         project: str,
         machine_group: str,
         config_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -15684,14 +16081,104 @@
         scheduled_sqlname: str,
         request: sls_20201230_models.UpdateScheduledSQLRequest,
     ) -> sls_20201230_models.UpdateScheduledSQLResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_scheduled_sqlwith_options_async(project, scheduled_sqlname, request, headers, runtime)
 
+    def update_sql_instance_with_options(
+        self,
+        project: str,
+        request: sls_20201230_models.UpdateSqlInstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.UpdateSqlInstanceResponse:
+        UtilClient.validate_model(request)
+        host_map = {}
+        host_map['project'] = project
+        body = {}
+        if not UtilClient.is_unset(request.cu):
+            body['cu'] = request.cu
+        if not UtilClient.is_unset(request.use_as_default):
+            body['useAsDefault'] = request.use_as_default
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/sqlinstance',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.UpdateSqlInstanceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def update_sql_instance_with_options_async(
+        self,
+        project: str,
+        request: sls_20201230_models.UpdateSqlInstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> sls_20201230_models.UpdateSqlInstanceResponse:
+        UtilClient.validate_model(request)
+        host_map = {}
+        host_map['project'] = project
+        body = {}
+        if not UtilClient.is_unset(request.cu):
+            body['cu'] = request.cu
+        if not UtilClient.is_unset(request.use_as_default):
+            body['useAsDefault'] = request.use_as_default
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname=f'/sqlinstance',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.UpdateSqlInstanceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def update_sql_instance(
+        self,
+        project: str,
+        request: sls_20201230_models.UpdateSqlInstanceRequest,
+    ) -> sls_20201230_models.UpdateSqlInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_sql_instance_with_options(project, request, headers, runtime)
+
+    async def update_sql_instance_async(
+        self,
+        project: str,
+        request: sls_20201230_models.UpdateSqlInstanceRequest,
+    ) -> sls_20201230_models.UpdateSqlInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_sql_instance_with_options_async(project, request, headers, runtime)
+
     def upsert_collection_policy_with_options(
         self,
         request: sls_20201230_models.UpsertCollectionPolicyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> sls_20201230_models.UpsertCollectionPolicyResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230/models.py` & `alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,39 +69,39 @@
             self.count_condition = m.get('countCondition')
         return self
 
 
 class GroupConfiguration(TeaModel):
     def __init__(
         self,
-        fileds: List[str] = None,
+        fields: List[str] = None,
         type: str = None,
     ):
-        self.fileds = fileds
+        self.fields = fields
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fileds is not None:
-            result['fileds'] = self.fileds
+        if self.fields is not None:
+            result['fields'] = self.fields
         if self.type is not None:
             result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('fileds') is not None:
-            self.fileds = m.get('fileds')
+        if m.get('fields') is not None:
+            self.fields = m.get('fields')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
 class JoinConfiguration(TeaModel):
     def __init__(
@@ -918,15 +918,15 @@
 class OSSExportConfigurationSink(TeaModel):
     def __init__(
         self,
         bucket: str = None,
         buffer_interval: int = None,
         buffer_size: int = None,
         compression_type: str = None,
-        content_detail: str = None,
+        content_detail: Dict[str, Any] = None,
         content_type: str = None,
         delay_sec: int = None,
         endpoint: str = None,
         path_format: str = None,
         path_format_type: str = None,
         prefix: str = None,
         role_arn: str = None,
@@ -3164,36 +3164,77 @@
             temp_model = Schedule()
             self.schedule = temp_model.from_map(m['schedule'])
         if m.get('scheduleId') is not None:
             self.schedule_id = m.get('scheduleId')
         return self
 
 
+class StoreViewStore(TeaModel):
+    def __init__(
+        self,
+        project: str = None,
+        query: str = None,
+        store_name: str = None,
+    ):
+        self.project = project
+        self.query = query
+        self.store_name = store_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.project is not None:
+            result['project'] = self.project
+        if self.query is not None:
+            result['query'] = self.query
+        if self.store_name is not None:
+            result['storeName'] = self.store_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('project') is not None:
+            self.project = m.get('project')
+        if m.get('query') is not None:
+            self.query = m.get('query')
+        if m.get('storeName') is not None:
+            self.store_name = m.get('storeName')
+        return self
+
+
 class Ticket(TeaModel):
     def __init__(
         self,
         caller_uid: int = None,
         create_date: str = None,
         expiration_time: int = None,
         expire_date: str = None,
         extra: str = None,
         name: str = None,
         number: int = None,
+        sharing_to: str = None,
         ticket: str = None,
         ticket_id: str = None,
         used_number: int = None,
         valid: bool = None,
     ):
         self.caller_uid = caller_uid
         self.create_date = create_date
         self.expiration_time = expiration_time
         self.expire_date = expire_date
         self.extra = extra
         self.name = name
         self.number = number
+        self.sharing_to = sharing_to
         self.ticket = ticket
         self.ticket_id = ticket_id
         self.used_number = used_number
         self.valid = valid
 
     def validate(self):
         pass
@@ -3214,14 +3255,16 @@
             result['expireDate'] = self.expire_date
         if self.extra is not None:
             result['extra'] = self.extra
         if self.name is not None:
             result['name'] = self.name
         if self.number is not None:
             result['number'] = self.number
+        if self.sharing_to is not None:
+            result['sharingTo'] = self.sharing_to
         if self.ticket is not None:
             result['ticket'] = self.ticket
         if self.ticket_id is not None:
             result['ticketId'] = self.ticket_id
         if self.used_number is not None:
             result['usedNumber'] = self.used_number
         if self.valid is not None:
@@ -3240,14 +3283,16 @@
             self.expire_date = m.get('expireDate')
         if m.get('extra') is not None:
             self.extra = m.get('extra')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('number') is not None:
             self.number = m.get('number')
+        if m.get('sharingTo') is not None:
+            self.sharing_to = m.get('sharingTo')
         if m.get('ticket') is not None:
             self.ticket = m.get('ticket')
         if m.get('ticketId') is not None:
             self.ticket_id = m.get('ticketId')
         if m.get('usedNumber') is not None:
             self.used_number = m.get('usedNumber')
         if m.get('valid') is not None:
@@ -6887,14 +6932,113 @@
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         return self
 
 
+class CreateSqlInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        cu: int = None,
+        use_as_default: bool = None,
+    ):
+        self.cu = cu
+        self.use_as_default = use_as_default
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cu is not None:
+            result['cu'] = self.cu
+        if self.use_as_default is not None:
+            result['useAsDefault'] = self.use_as_default
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cu') is not None:
+            self.cu = m.get('cu')
+        if m.get('useAsDefault') is not None:
+            self.use_as_default = m.get('useAsDefault')
+        return self
+
+
+class CreateSqlInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class CreateTicketRequest(TeaModel):
+    def __init__(
+        self,
+        access_token_expiration_time: int = None,
+        expiration_time: int = None,
+    ):
+        self.access_token_expiration_time = access_token_expiration_time
+        self.expiration_time = expiration_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token_expiration_time is not None:
+            result['accessTokenExpirationTime'] = self.access_token_expiration_time
+        if self.expiration_time is not None:
+            result['expirationTime'] = self.expiration_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('accessTokenExpirationTime') is not None:
+            self.access_token_expiration_time = m.get('accessTokenExpirationTime')
+        if m.get('expirationTime') is not None:
+            self.expiration_time = m.get('expirationTime')
+        return self
+
+
 class CreateTicketResponseBody(TeaModel):
     def __init__(
         self,
         ticket: str = None,
     ):
         self.ticket = ticket
 
@@ -9846,15 +9990,14 @@
         highlight: bool = None,
         line: int = None,
         offset: int = None,
         power_sql: bool = None,
         query: str = None,
         reverse: bool = None,
         session: str = None,
-        shard: int = None,
         to: int = None,
         topic: str = None,
     ):
         # Specifies whether to page forward or backward for the scan-based query or the phrase search.
         self.forward = forward
         # The beginning of the time range to query. The value is the log time that is specified when log data is written.
         # 
@@ -9875,16 +10018,14 @@
         self.query = query
         # Specifies whether to return logs in reverse chronological order of log timestamps. The log timestamps are accurate to the minute. Valid values:
         # 
         # true: Logs are returned in reverse chronological order of log timestamps. false (default): Logs are returned in chronological order of log timestamps. Note: The reverse parameter takes effect only when the query parameter is set to a search statement. The reverse parameter specifies the method used to sort returned logs. If the query parameter is set to a query statement, the reverse parameter does not take effect. The method used to sort returned logs is specified by the ORDER BY clause in the analytic statement. If you use the keyword asc in the ORDER BY clause, the logs are sorted in chronological order. If you use the keyword desc in the ORDER BY clause, the logs are sorted in reverse chronological order. By default, asc is used in the ORDER BY clause.
         self.reverse = reverse
         # The parameter that is used to query data.
         self.session = session
-        # The ID of the shard.
-        self.shard = shard
         # The end of the time range to query. The value is the log time that is specified when log data is written.
         # 
         # The time range that is specified in this operation is a left-closed, right-open interval. The interval includes the start time specified by the from parameter, but does not include the end time specified by the to parameter. If you specify the same value for the from and to parameters, the interval is invalid, and an error message is returned. The value is a UNIX timestamp representing the number of seconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.to = to
         # The topic of the logs. Default value: double quotation marks ("").
         self.topic = topic
 
@@ -9911,16 +10052,14 @@
             result['powerSql'] = self.power_sql
         if self.query is not None:
             result['query'] = self.query
         if self.reverse is not None:
             result['reverse'] = self.reverse
         if self.session is not None:
             result['session'] = self.session
-        if self.shard is not None:
-            result['shard'] = self.shard
         if self.to is not None:
             result['to'] = self.to
         if self.topic is not None:
             result['topic'] = self.topic
         return result
 
     def from_map(self, m: dict = None):
@@ -9939,16 +10078,14 @@
             self.power_sql = m.get('powerSql')
         if m.get('query') is not None:
             self.query = m.get('query')
         if m.get('reverse') is not None:
             self.reverse = m.get('reverse')
         if m.get('session') is not None:
             self.session = m.get('session')
-        if m.get('shard') is not None:
-            self.shard = m.get('shard')
         if m.get('to') is not None:
             self.to = m.get('to')
         if m.get('topic') is not None:
             self.topic = m.get('topic')
         return self
 
 
@@ -11070,14 +11207,153 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetShipperStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetSlsServiceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ServiceStatus = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ServiceStatus()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetSqlInstanceResponseBody(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        cu: int = None,
+        create_time: int = None,
+        update_time: int = None,
+        use_as_default: bool = None,
+    ):
+        self.name = name
+        self.cu = cu
+        self.create_time = create_time
+        self.update_time = update_time
+        self.use_as_default = use_as_default
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.cu is not None:
+            result['cu'] = self.cu
+        if self.create_time is not None:
+            result['createTime'] = self.create_time
+        if self.update_time is not None:
+            result['updateTime'] = self.update_time
+        if self.use_as_default is not None:
+            result['useAsDefault'] = self.use_as_default
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('cu') is not None:
+            self.cu = m.get('cu')
+        if m.get('createTime') is not None:
+            self.create_time = m.get('createTime')
+        if m.get('updateTime') is not None:
+            self.update_time = m.get('updateTime')
+        if m.get('useAsDefault') is not None:
+            self.use_as_default = m.get('useAsDefault')
+        return self
+
+
+class GetSqlInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: List[GetSqlInstanceResponseBody] = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            for k in self.body:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        result['body'] = []
+        if self.body is not None:
+            for k in self.body:
+                result['body'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        self.body = []
+        if m.get('body') is not None:
+            for k in m.get('body'):
+                temp_model = GetSqlInstanceResponseBody()
+                self.body.append(temp_model.from_map(k))
+        return self
+
+
 class ListAlertsRequest(TeaModel):
     def __init__(
         self,
         logstore: str = None,
         offset: int = None,
         size: int = None,
     ):
@@ -12464,37 +12740,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListETLsRequest(TeaModel):
     def __init__(
         self,
+        logstore: str = None,
         offset: int = None,
         size: int = None,
     ):
+        self.logstore = logstore
         self.offset = offset
         self.size = size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -12628,55 +12910,47 @@
         return self
 
 
 class ListExternalStoreResponseBody(TeaModel):
     def __init__(
         self,
         count: int = None,
-        externalstores: List[ExternalStore] = None,
+        externalstores: List[str] = None,
         total: int = None,
     ):
         # The number of external stores returned on the current page.
         self.count = count
         # The names of the external stores.
         self.externalstores = externalstores
         # The number of external stores that meet the query conditions.
         self.total = total
 
     def validate(self):
-        if self.externalstores:
-            for k in self.externalstores:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.count is not None:
             result['count'] = self.count
-        result['externalstores'] = []
         if self.externalstores is not None:
-            for k in self.externalstores:
-                result['externalstores'].append(k.to_map() if k else None)
+            result['externalstores'] = self.externalstores
         if self.total is not None:
             result['total'] = self.total
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('count') is not None:
             self.count = m.get('count')
-        self.externalstores = []
         if m.get('externalstores') is not None:
-            for k in m.get('externalstores'):
-                temp_model = ExternalStore()
-                self.externalstores.append(temp_model.from_map(k))
+            self.externalstores = m.get('externalstores')
         if m.get('total') is not None:
             self.total = m.get('total')
         return self
 
 
 class ListExternalStoreResponse(TeaModel):
     def __init__(
@@ -13246,37 +13520,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOSSExportsRequest(TeaModel):
     def __init__(
         self,
+        logstore: str = None,
         offset: int = None,
         size: int = None,
     ):
+        self.logstore = logstore
         self.offset = offset
         self.size = size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -13367,37 +13647,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOSSHDFSExportsRequest(TeaModel):
     def __init__(
         self,
+        logstore: str = None,
         offset: int = None,
         size: int = None,
     ):
+        self.logstore = logstore
         self.offset = offset
         self.size = size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -13488,37 +13774,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOSSIngestionsRequest(TeaModel):
     def __init__(
         self,
+        logstore: str = None,
         offset: int = None,
         size: int = None,
     ):
+        self.logstore = logstore
         self.offset = offset
         self.size = size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -13874,37 +14166,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListScheduledSQLsRequest(TeaModel):
     def __init__(
         self,
+        logstore: str = None,
         offset: int = None,
         size: int = None,
     ):
+        self.logstore = logstore
         self.offset = offset
         self.size = size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -14433,14 +14731,47 @@
         if m.get('body') is not None:
             for k in m.get('body'):
                 temp_model = Shard()
                 self.body.append(temp_model.from_map(k))
         return self
 
 
+class OpenSlsServiceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
 class PutAnnotationDataRequest(TeaModel):
     def __init__(
         self,
         annotationdata_id: str = None,
         ml_data_param: MLDataParam = None,
         raw_log: List[Dict[str, str]] = None,
     ):
@@ -14824,14 +15155,115 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryMLServiceResultsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RefreshTokenRequest(TeaModel):
+    def __init__(
+        self,
+        access_token_expiration_time: int = None,
+        ticket: str = None,
+    ):
+        self.access_token_expiration_time = access_token_expiration_time
+        self.ticket = ticket
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token_expiration_time is not None:
+            result['accessTokenExpirationTime'] = self.access_token_expiration_time
+        if self.ticket is not None:
+            result['ticket'] = self.ticket
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('accessTokenExpirationTime') is not None:
+            self.access_token_expiration_time = m.get('accessTokenExpirationTime')
+        if m.get('ticket') is not None:
+            self.ticket = m.get('ticket')
+        return self
+
+
+class RefreshTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        access_token: str = None,
+    ):
+        self.access_token = access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token is not None:
+            result['accessToken'] = self.access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('accessToken') is not None:
+            self.access_token = m.get('accessToken')
+        return self
+
+
+class RefreshTokenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RefreshTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RefreshTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RemoveConfigFromMachineGroupResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
     ):
         self.headers = headers
@@ -17522,14 +17954,80 @@
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
     ):
         self.headers = headers
         self.status_code = status_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class UpdateSqlInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        cu: int = None,
+        use_as_default: bool = None,
+    ):
+        self.cu = cu
+        self.use_as_default = use_as_default
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cu is not None:
+            result['cu'] = self.cu
+        if self.use_as_default is not None:
+            result['useAsDefault'] = self.use_as_default
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cu') is not None:
+            self.cu = m.get('cu')
+        if m.get('useAsDefault') is not None:
+            self.use_as_default = m.get('useAsDefault')
+        return self
+
+
+class UpdateSqlInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
```

### Comparing `alibabacloud_sls20201230-5.0.0/alibabacloud_sls20201230.egg-info/PKG-INFO` & `alibabacloud_sls20201230-5.1.0/alibabacloud_sls20201230.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sls20201230
-Version: 5.0.0
+Version: 5.1.0
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230-5.0.0/setup.py` & `alibabacloud_sls20201230-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sls20201230.
 
-Created on 06/02/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sls20201230"
 NAME = "alibabacloud_sls20201230" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Log Service (20201230) SDK Library for Python"
```

