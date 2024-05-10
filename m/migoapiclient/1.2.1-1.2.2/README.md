# Comparing `tmp/migoapiclient-1.2.1.tar.gz` & `tmp/migoapiclient-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.2.1.tar", last modified: Wed May  8 09:33:53 2024, max compression
+gzip compressed data, was "migoapiclient-1.2.2.tar", last modified: Fri May 10 01:46:48 2024, max compression
```

## Comparing `migoapiclient-1.2.1.tar` & `migoapiclient-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.996908 migoapiclient-1.2.1/
--rw-rw-rw-   0        0        0     3900 2024-05-08 09:33:53.996908 migoapiclient-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.992907 migoapiclient-1.2.1/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.2.1/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    14171 2024-05-08 03:25:26.000000 migoapiclient-1.2.1/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.2.1/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.995906 migoapiclient-1.2.1/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 09:33:53.996908 migoapiclient-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-05-08 09:26:40.000000 migoapiclient-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.995906 migoapiclient-1.2.1/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:46:48.523442 migoapiclient-1.2.2/
+-rw-rw-rw-   0        0        0     3900 2024-05-10 01:46:48.523442 migoapiclient-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 01:46:48.511442 migoapiclient-1.2.2/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.2.2/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    15245 2024-05-10 01:26:03.000000 migoapiclient-1.2.2/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.2.2/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:46:48.522442 migoapiclient-1.2.2/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-05-10 01:46:48.000000 migoapiclient-1.2.2/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-10 01:46:48.000000 migoapiclient-1.2.2/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 01:46:48.000000 migoapiclient-1.2.2/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 01:46:48.000000 migoapiclient-1.2.2/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 01:46:48.523442 migoapiclient-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-05-10 01:26:03.000000 migoapiclient-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:46:48.522442 migoapiclient-1.2.2/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.2.2/src/__init__.py
```

### Comparing `migoapiclient-1.2.1/PKG-INFO` & `migoapiclient-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.2.1
+Version: 1.2.2
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.2.1/README.md` & `migoapiclient-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.2.1/migoapiclient/api_client.py` & `migoapiclient-1.2.2/migoapiclient/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from datetime import datetime
 
 from dateutil.tz import tz
 from requests import Response
 
-from file_manager import LogFileManager
+from .file_manager import LogFileManager
 import time
 import requests
 
 TZ_NAME = 'Asia/Shanghai'
 ERROR_MSG = """
 ---------------------------------- {0} begin ----------------------------------
 请求URL是：{1}
@@ -222,25 +222,32 @@
 
     def get_third_party_crawl_data(self, auth_type: str, auth_id: str):
         """
         获取第三方平台采集数据
         :param auth_type 授权类型
         :param auth_id 授权ID
         """
+        node_data = self.get_node_context(auth_id)
+        for auth_data in node_data[auth_type]:
+            if int(auth_data['auth_id']) == int(auth_id):
+                return json.loads(auth_data['crawl_data'])
+        raise Exception(f'找不到该授权信息，授权ID是：{auth_id}')
+
+    def get_node_context(self, auth_id: int):
+        """
+        获取节点信息
+        :param auth_id 认证ID
+        """
         uri = '/data-collection-service/node/detail'
         operate_name = f'获取第三方平台授权信息，授权ID为：{auth_id}'
         post_data = {
             'nodeConfigId': self.node_id
         }
         response = self.migo_try_post(self.host + uri, auth_id, operate_name, json=post_data)
-        node_data = json.loads(response['data']['nodeContext'])
-        for auth_data in node_data[auth_type]:
-            if auth_data['auth_id'] == auth_id:
-                return json.loads(auth_data['crawl_data'])
-        raise Exception(f'找不到该授权信息，授权ID是：{auth_id}')
+        return json.loads(response['data']['nodeContext'])
 
     def get_heartbeat(self):
         """
         发送心跳
         """
         uri = f'/data-collection-service/node/heartbeat/{self.node_id}'
         return self.try_get(self.host + uri, error_count=0)
@@ -341,14 +348,37 @@
         """
         获取第三方平台授权信息
         :param auth_id
         """
         uri = f'/data-collection-service/node/thirdpartyauths/{auth_id}'
         return self.migo_try_get(self.host + uri, auth_id, '获取第三方平台授权信息')
 
+    def post_node_style_id_data(self, style: str, data_id: int, crawl_data: dict):
+        """
+        保存某个类型的某个ID数据
+        :param style 类型
+        :param data_id 数据ID
+        :param crawl_data 采集数据
+        """
+        node_data = self.get_node_context(data_id)
+        for auth_data in node_data[style]:
+            if int(auth_data['auth_id']) == int(data_id):
+                auth_data['crawl_data'] = json.dumps(crawl_data)
+                break
+        return self.post_node_context(node_data)
+
+    def post_node_context(self, node_context: dict):
+        """
+        上传节点信息
+        :param node_context 节点信息
+        """
+        uri = '/data-collection-service/node/nodeContext'
+        url = self.host + uri
+        return self.migo_try_post(url, -1, '上传节点信息', json=node_context)
+
     def post_schedule_log(self, msg: str, shop_id: str, definition_info: dict, log_params: dict = None):
         """
         上传日志
         :param msg 信息
         :param shop_id 店铺ID
         :param definition_info 策略信息
         :param log_params 其他信息
```

### Comparing `migoapiclient-1.2.1/migoapiclient/file_manager.py` & `migoapiclient-1.2.2/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.2.1/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.2.2/migoapiclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.2.1
+Version: 1.2.2
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.2.1/setup.py` & `migoapiclient-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

