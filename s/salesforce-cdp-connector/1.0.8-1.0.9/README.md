# Comparing `tmp/salesforce-cdp-connector-1.0.8.tar.gz` & `tmp/salesforce-cdp-connector-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-cdp-connector-1.0.8.tar", last modified: Tue Sep 20 10:50:25 2022, max compression
+gzip compressed data, was "salesforce-cdp-connector-1.0.9.tar", last modified: Tue Jan 31 09:11:20 2023, max compression
```

## Comparing `salesforce-cdp-connector-1.0.8.tar` & `salesforce-cdp-connector-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 10:50:25.225064 salesforce-cdp-connector-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-09-20 10:50:25.225064 salesforce-cdp-connector-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 10:50:25.225064 salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-09-20 10:50:24.000000 salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-09-20 10:50:25.000000 salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 10:50:24.000000 salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-20 10:50:25.000000 salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-20 10:50:25.000000 salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 10:50:25.225064 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7987 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/authentication_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     7668 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/parsed_query_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/query_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/salesforcecdpconnector/query_submitter.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-09-20 10:50:25.225064 salesforce-cdp-connector-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-20 10:50:08.000000 salesforce-cdp-connector-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:11:20.637371 salesforce-cdp-connector-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-31 09:11:20.637371 salesforce-cdp-connector-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:11:20.633371 salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-31 09:11:20.000000 salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-31 09:11:20.000000 salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 09:11:20.000000 salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-31 09:11:20.000000 salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-31 09:11:20.000000 salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:11:20.637371 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/authentication_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/genie_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/metadata_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/parsed_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/query_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/salesforcecdpconnector/query_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-31 09:11:20.637371 salesforce-cdp-connector-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-31 09:10:51.000000 salesforce-cdp-connector-1.0.9/setup.py
```

### Comparing `salesforce-cdp-connector-1.0.8/LICENSE.txt` & `salesforce-cdp-connector-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `salesforce-cdp-connector-1.0.8/PKG-INFO` & `salesforce-cdp-connector-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: salesforce-cdp-connector
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Connector for Salesforce CDP
 Home-page: https://github.com/forcedotcom/salesforce-cdp-connector
-Author: Vishnu Prasad
+Author: Query Service
 License: BSD-3-Clause
 Keywords: cdp,salesforce,dbapi
 Platform: UNKNOWN
 Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `salesforce-cdp-connector-1.0.8/README.md` & `salesforce-cdp-connector-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/PKG-INFO` & `salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: salesforce-cdp-connector
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Connector for Salesforce CDP
 Home-page: https://github.com/forcedotcom/salesforce-cdp-connector
-Author: Vishnu Prasad
+Author: Query Service
 License: BSD-3-Clause
 Keywords: cdp,salesforce,dbapi
 Platform: UNKNOWN
 Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `salesforce-cdp-connector-1.0.8/salesforce_cdp_connector.egg-info/SOURCES.txt` & `salesforce-cdp-connector-1.0.9/salesforce_cdp_connector.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 salesforce_cdp_connector.egg-info/top_level.txt
 salesforcecdpconnector/__init__.py
 salesforcecdpconnector/authentication_helper.py
 salesforcecdpconnector/connection.py
 salesforcecdpconnector/constants.py
 salesforcecdpconnector/cursor.py
 salesforcecdpconnector/exceptions.py
+salesforcecdpconnector/genie_table.py
+salesforcecdpconnector/metadata_processor.py
 salesforcecdpconnector/pandas_utils.py
 salesforcecdpconnector/parsed_query_result.py
 salesforcecdpconnector/query_result_parser.py
 salesforcecdpconnector/query_submitter.py
```

### Comparing `salesforce-cdp-connector-1.0.8/salesforcecdpconnector/authentication_helper.py` & `salesforce-cdp-connector-1.0.9/salesforcecdpconnector/authentication_helper.py`

 * *Files identical despite different names*

### Comparing `salesforce-cdp-connector-1.0.8/salesforcecdpconnector/connection.py` & `salesforce-cdp-connector-1.0.9/salesforcecdpconnector/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 from .authentication_helper import AuthenticationHelper
 from .constants import API_VERSION_V2
 from .constants import MAX_RETRY_COUNT
 from .cursor import SalesforceCDPCursor
 from .exceptions import Error
 from .pandas_utils import PandasUtils
+from .metadata_processor import MetadataProcessor
 
 apilevel = "2.0"
 threadsafety = 2
 paramstyle = "qmark"
 
 
 class SalesforceCDPConnection:
@@ -49,14 +50,23 @@
         :param query: The input query
         :return: Query Results as Pandas dataframe
         """
         if self.closed:
             raise Error('Cannot create dataframe. Connection is closed')
         return PandasUtils.get_dataframe(self, query)
 
+    def list_tables(self, table_name=None, table_category=None, table_type=None):
+        """
+        Returns the genie table list
+        :return: Query Results as Table list
+        """
+        if self.closed:
+            raise Error('Cannot create table list. Connection is closed')
+        return MetadataProcessor.list_tables(self, table_name, table_category, table_type)
+
     def close(self):
         """
         Clearing credentials
         Marking connection as closed
         :return: None
         """
         self.login_url = None
```

### Comparing `salesforce-cdp-connector-1.0.8/salesforcecdpconnector/cursor.py` & `salesforce-cdp-connector-1.0.9/salesforcecdpconnector/cursor.py`

 * *Files identical despite different names*

### Comparing `salesforce-cdp-connector-1.0.8/salesforcecdpconnector/pandas_utils.py` & `salesforce-cdp-connector-1.0.9/salesforcecdpconnector/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-cdp-connector-1.0.8/salesforcecdpconnector/query_result_parser.py` & `salesforce-cdp-connector-1.0.9/salesforcecdpconnector/query_result_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-cdp-connector-1.0.8/salesforcecdpconnector/query_submitter.py` & `salesforce-cdp-connector-1.0.9/salesforcecdpconnector/query_submitter.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import json
 import logging
 import requests
 import socket
 from timeit import default_timer as timer
 
 from .constants import API_VERSION_V2
+from .constants import API_VERSION_V1
 from .constants import QUERY_HEADER_KEY_AUTHORIZATION
 from .constants import QUERY_HEADER_KEY_CONTENT_TYPE
 from .constants import QUERY_HEADER_VALUE_APPLICATION_JSON
 from .constants import QUERY_HEADER_KEY_ACCEPT_ENCODING
 from .constants import QUERY_HEADER_VALUE_GZIP
 from .exceptions import Error
 
@@ -58,14 +59,24 @@
         :param enable_arrow_stream: Set as True to fetch the results as ArrowStream
         :return:
         """
         token, instance_url = connection.authentication_helper.get_token()
         return QuerySubmitter._get_next_batch_results(next_batch_id, instance_url, token, enable_arrow_stream)
 
     @staticmethod
+    def get_metadata(connection, request_params={}):
+        """
+        This method fetches the metadata for a given tenant.
+        :param connection:  SalesforceCDPConnection
+        :return: Metadata for a given tenant
+        """
+        token, instance_url = connection.authentication_helper.get_token()
+        return QuerySubmitter.__get_metadata_results(instance_url, token, request_params)
+
+    @staticmethod
     def _get_query_results(query, instance_url, token, api_version='V2', enable_arrow_stream=False):
         url = f'https://{instance_url}/api/{api_version}/query'
         json_payload = QuerySubmitter._get_payload(query)
         headers = QuerySubmitter._get_headers(token, enable_arrow_stream)
         QuerySubmitter.logger.debug("Submitting query for execution")
         start_time = timer()
         sql_response = QuerySubmitter.session.post(url=url, data=json_payload, headers=headers, verify=False)
@@ -105,13 +116,32 @@
                    QUERY_HEADER_KEY_CONTENT_TYPE: QUERY_HEADER_VALUE_APPLICATION_JSON,
                    QUERY_HEADER_KEY_ACCEPT_ENCODING: QUERY_HEADER_VALUE_GZIP}
         if enable_arrow_stream:
             headers['enable-arrow-stream'] = 'true'
         return headers
 
     @staticmethod
+    def __get_metadata_results(instance_url, token, parameters={}):
+        url = f'https://{instance_url}/api/v1/metadata'
+        headers = QuerySubmitter._get_headers(token, enable_arrow_stream=False)
+        QuerySubmitter.logger.debug("Submitting metadata query for execution")
+        start_time = timer()
+        sql_response = QuerySubmitter.session.get(url=url, headers=headers, verify=False, params=parameters)
+        QuerySubmitter.logger.debug("Metadata Query Submitted in %s", str(timedelta(seconds=timer() - start_time)))
+        if sql_response.status_code != 200:
+            try:
+                error_json = sql_response.json()
+                error_message = error_json['message']
+            finally:
+                if error_message is not None:
+                    raise Error('Failed executing metadata query in server : %s' % error_message)
+                raise Error('Failed executing query in server')
+        response_json = sql_response.json()
+        return response_json
+
+    @staticmethod
     def _get_payload(query):
         payload = {
             'sql': query
         }
         json_payload = json.dumps(payload)
         return json_payload
```

### Comparing `salesforce-cdp-connector-1.0.8/setup.cfg` & `salesforce-cdp-connector-1.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = salesforce-cdp-connector
-version = 1.0.8
-author = Vishnu Prasad
+version = 1.0.9
+author = Query Service
 description = Python Connector for Salesforce CDP
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/forcedotcom/salesforce-cdp-connector
 keywords = cdp, salesforce, dbapi
 license = BSD-3-Clause
```

