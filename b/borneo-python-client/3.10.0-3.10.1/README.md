# Comparing `tmp/borneo_python_client-3.10.0.tar.gz` & `tmp/borneo_python_client-3.10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borneo_python_client-3.10.0.tar", last modified: Fri May 10 05:09:43 2024, max compression
+gzip compressed data, was "borneo_python_client-3.10.1.tar", last modified: Fri May 10 14:33:09 2024, max compression
```

## Comparing `borneo_python_client-3.10.0.tar` & `borneo_python_client-3.10.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:09:43.512065 borneo_python_client-3.10.0/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 05:02:41.000000 borneo_python_client-3.10.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-10 05:02:41.000000 borneo_python_client-3.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-10 05:09:43.512065 borneo_python_client-3.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:09:43.508065 borneo_python_client-3.10.0/borneo_python_client/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)   123987 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17027 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)   288886 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   178704 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)   136564 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/borneo_python_client/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:09:43.508065 borneo_python_client-3.10.0/borneo_python_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-10 05:09:43.000000 borneo_python_client-3.10.0/borneo_python_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 05:09:43.000000 borneo_python_client-3.10.0/borneo_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:09:43.000000 borneo_python_client-3.10.0/borneo_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 05:09:43.000000 borneo_python_client-3.10.0/borneo_python_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 05:09:43.000000 borneo_python_client-3.10.0/borneo_python_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:09:43.512065 borneo_python_client-3.10.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:09:43.508065 borneo_python_client-3.10.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-10 05:09:38.000000 borneo_python_client-3.10.0/tests/test_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:09.009816 borneo_python_client-3.10.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 14:25:29.000000 borneo_python_client-3.10.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-10 14:25:29.000000 borneo_python_client-3.10.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-10 14:33:09.009816 borneo_python_client-3.10.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:09.005816 borneo_python_client-3.10.1/borneo_python_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125040 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17124 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   310639 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   181979 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138321 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/borneo_python_client/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:09.009816 borneo_python_client-3.10.1/borneo_python_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-10 14:33:08.000000 borneo_python_client-3.10.1/borneo_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 14:33:09.000000 borneo_python_client-3.10.1/borneo_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:33:08.000000 borneo_python_client-3.10.1/borneo_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 14:33:08.000000 borneo_python_client-3.10.1/borneo_python_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 14:33:08.000000 borneo_python_client-3.10.1/borneo_python_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:33:09.009816 borneo_python_client-3.10.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:33:09.009816 borneo_python_client-3.10.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-10 14:33:03.000000 borneo_python_client-3.10.1/tests/test_protocol.py
```

### Comparing `borneo_python_client-3.10.0/LICENSE` & `borneo_python_client-3.10.1/LICENSE`

 * *Files identical despite different names*

### Comparing `borneo_python_client-3.10.0/PKG-INFO` & `borneo_python_client-3.10.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borneo_python_client
-Version: 3.10.0
+Version: 3.10.1
 Summary: borneo_python_client client
 License: Apache-2.0
 Keywords: smithy,borneo_python_client
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
@@ -46,15 +46,15 @@
 
 Requests to the Borneo API must be authenticated using an authentication token. The token is passed in the `Authorization` header of the request.
 
 ```
 Authorization: Bearer <token>
 ```
 
-**TODO**: Explain how to obtain the authentication token.
+This authorization Bearer token can generated using service accounts and Borneo SDK or directly download Borneo token from dashboard for testing.
 
 ## Pagination
 
 All list operations support pagination. The `pageSize` parameter can be
 used to control the number of results returned per API request. If there
 are more results available, the API response will contain a `nextToken`
 value that can be used to retrieve the next page of results by passing it
```

### Comparing `borneo_python_client-3.10.0/README.md` & `borneo_python_client-3.10.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Requests to the Borneo API must be authenticated using an authentication token. The token is passed in the `Authorization` header of the request.
 
 ```
 Authorization: Bearer <token>
 ```
 
-**TODO**: Explain how to obtain the authentication token.
+This authorization Bearer token can generated using service accounts and Borneo SDK or directly download Borneo token from dashboard for testing.
 
 ## Pagination
 
 All list operations support pagination. The `pageSize` parameter can be
 used to control the number of results returned per API request. If there
 are more results available, the API response will contain a `nextToken`
 value that can be used to retrieve the next page of results by passing it
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client/auth.py` & `borneo_python_client-3.10.1/borneo_python_client/auth.py`

 * *Files identical despite different names*

### Comparing `borneo_python_client-3.10.0/borneo_python_client/client.py` & `borneo_python_client-3.10.1/borneo_python_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     _deserialize_list_events,
     _deserialize_list_headquarters,
     _deserialize_list_infotype_categories,
     _deserialize_list_inspection_results,
     _deserialize_list_inventory_resources,
     _deserialize_list_inventory_resources_export,
     _deserialize_list_issues,
+    _deserialize_list_logs,
     _deserialize_list_processing_activities,
     _deserialize_list_processing_activities_export,
     _deserialize_list_processing_activities_of_recipient,
     _deserialize_list_processing_activity_filter,
     _deserialize_list_recipients,
     _deserialize_list_recipients_export,
     _deserialize_list_recipients_for_filter,
@@ -216,14 +217,16 @@
     ListInspectionResultsOutput,
     ListInventoryResourcesExportInput,
     ListInventoryResourcesExportOutput,
     ListInventoryResourcesInput,
     ListInventoryResourcesOutput,
     ListIssuesInput,
     ListIssuesOutput,
+    ListLogsInput,
+    ListLogsOutput,
     ListProcessingActivitiesExportInput,
     ListProcessingActivitiesExportOutput,
     ListProcessingActivitiesInput,
     ListProcessingActivitiesOfRecipientInput,
     ListProcessingActivitiesOfRecipientOutput,
     ListProcessingActivitiesOutput,
     ListProcessingActivityFilterInput,
@@ -349,14 +352,15 @@
     _serialize_list_events,
     _serialize_list_headquarters,
     _serialize_list_infotype_categories,
     _serialize_list_inspection_results,
     _serialize_list_inventory_resources,
     _serialize_list_inventory_resources_export,
     _serialize_list_issues,
+    _serialize_list_logs,
     _serialize_list_processing_activities,
     _serialize_list_processing_activities_export,
     _serialize_list_processing_activities_of_recipient,
     _serialize_list_processing_activity_filter,
     _serialize_list_recipients,
     _serialize_list_recipients_export,
     _serialize_list_recipients_for_filter,
@@ -421,15 +425,15 @@
 
     Requests to the Borneo API must be authenticated using an authentication token. The token is passed in the `Authorization` header of the request.
 
     ```
     Authorization: Bearer <token>
     ```
 
-    **TODO**: Explain how to obtain the authentication token.
+    This authorization Bearer token can generated using service accounts and Borneo SDK or directly download Borneo token from dashboard for testing.
 
     ## Pagination
 
     All list operations support pagination. The `pageSize` parameter can be
     used to control the number of results returned per API request. If there
     are more results available, the API response will contain a `nextToken`
     value that can be used to retrieve the next page of results by passing it
@@ -1808,14 +1812,38 @@
             plugins=operation_plugins,
             serialize=_serialize_list_issues,
             deserialize=_deserialize_list_issues,
             config=self._config,
             operation_name="ListIssues",
         )
 
+    async def list_logs(
+        self, input: ListLogsInput, plugins: list[Plugin] | None = None
+    ) -> ListLogsOutput:
+        """List all logs based on supported filters.
+
+        :param input: The operation's input.
+
+        :param plugins: A list of callables that modify the configuration dynamically.
+        Changes made by these plugins only apply for the duration of the operation
+        execution and will not affect any other operation invocations.
+        """
+        operation_plugins: list[Plugin] = []
+        if plugins:
+            operation_plugins.extend(plugins)
+
+        return await self._execute_operation(
+            input=input,
+            plugins=operation_plugins,
+            serialize=_serialize_list_logs,
+            deserialize=_deserialize_list_logs,
+            config=self._config,
+            operation_name="ListLogs",
+        )
+
     async def list_processing_activities(
         self, input: ListProcessingActivitiesInput, plugins: list[Plugin] | None = None
     ) -> ListProcessingActivitiesOutput:
         """List processing activities paginated
 
         :param input: The operation's input.
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client/config.py` & `borneo_python_client-3.10.1/borneo_python_client/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,16 @@
     ListInspectionResultsOutput,
     ListInventoryResourcesExportInput,
     ListInventoryResourcesExportOutput,
     ListInventoryResourcesInput,
     ListInventoryResourcesOutput,
     ListIssuesInput,
     ListIssuesOutput,
+    ListLogsInput,
+    ListLogsOutput,
     ListProcessingActivitiesExportInput,
     ListProcessingActivitiesExportOutput,
     ListProcessingActivitiesInput,
     ListProcessingActivitiesOfRecipientInput,
     ListProcessingActivitiesOfRecipientOutput,
     ListProcessingActivitiesOutput,
     ListProcessingActivityFilterInput,
@@ -291,14 +293,15 @@
     Interceptor[ListInfotypeCategoriesInput, ListInfotypeCategoriesOutput, Any, Any],
     Interceptor[ListInspectionResultsInput, ListInspectionResultsOutput, Any, Any],
     Interceptor[ListInventoryResourcesInput, ListInventoryResourcesOutput, Any, Any],
     Interceptor[
         ListInventoryResourcesExportInput, ListInventoryResourcesExportOutput, Any, Any
     ],
     Interceptor[ListIssuesInput, ListIssuesOutput, Any, Any],
+    Interceptor[ListLogsInput, ListLogsOutput, Any, Any],
     Interceptor[
         ListProcessingActivitiesInput, ListProcessingActivitiesOutput, Any, Any
     ],
     Interceptor[
         ListProcessingActivitiesExportInput,
         ListProcessingActivitiesExportOutput,
         Any,
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client/deserialize.py` & `borneo_python_client-3.10.1/borneo_python_client/deserialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .config import Config
 from .errors import (
     ApiError,
     NoSuchResource,
     NotAllowed,
     ServiceError,
     Unauthorized,
+    UnexpectedServerError,
     UnknownApiError,
     ValidationException,
 )
 from .models import (
     AccountListMember,
     AccountPermissions,
     AddDiscoveredRecipientAsRecipientsOutput,
@@ -115,25 +116,27 @@
     ListEventsOutput,
     ListHeadquartersOutput,
     ListInfotypeCategoriesOutput,
     ListInspectionResultsOutput,
     ListInventoryResourcesExportOutput,
     ListInventoryResourcesOutput,
     ListIssuesOutput,
+    ListLogsOutput,
     ListProcessingActivitiesExportOutput,
     ListProcessingActivitiesOfRecipientOutput,
     ListProcessingActivitiesOutput,
     ListProcessingActivityFilterMember,
     ListProcessingActivityFilterOutput,
     ListRecipientsExportOutput,
     ListRecipientsForFilterOutput,
     ListRecipientsOutput,
     ListScansOutput,
     ListTomsOutput,
     ListUserProfilesOutput,
+    LogMember,
     ManagementMethod,
     ManagerObject,
     OktaUserDiscoveryListMember,
     OwnerObject,
     PauseScanOutput,
     PollDomainOutput,
     PostalAddress,
@@ -227,14 +230,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_archive_discovered_recipient(
     http_response: HTTPResponse, config: Config
 ) -> ArchiveDiscoveredRecipientOutput:
@@ -260,14 +268,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_create_asset(
     http_response: HTTPResponse, config: Config
 ) -> CreateAssetOutput:
@@ -301,14 +314,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -347,14 +365,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_create_department(
     http_response: HTTPResponse, config: Config
 ) -> CreateDepartmentOutput:
@@ -388,14 +411,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_create_domain(
     http_response: HTTPResponse, config: Config
 ) -> CreateDomainOutput:
@@ -429,14 +457,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -475,14 +508,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -521,14 +559,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_create_headquarter(
     http_response: HTTPResponse, config: Config
 ) -> CreateHeadquarterOutput:
@@ -562,14 +605,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -608,14 +656,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -654,14 +707,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -700,14 +758,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_create_threshold(
     http_response: HTTPResponse, config: Config
 ) -> CreateThresholdOutput:
@@ -741,14 +804,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -762,55 +830,55 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
-    if (_type := output.get("type")) is not None:
-        kwargs["type"] = expect_type(str, _type)
-
     if (_data_plane_ids := output.get("dataPlaneIds")) is not None:
         kwargs["data_plane_ids"] = _deserialize_data_plane_ids(_data_plane_ids, config)
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
-
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
+    if (_deleted_at := output.get("deletedAt")) is not None:
+        kwargs["deleted_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _deleted_at)
         )
 
     if "accountId" not in output:
         raise ServiceError(
             'Expected to find "accountId" in the operation output, but it was not present.'
         )
     kwargs["account_id"] = expect_type(str, output["accountId"])
 
-    if (_deleted_at := output.get("deletedAt")) is not None:
-        kwargs["deleted_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _deleted_at)
-        )
-
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
     if (_meta := output.get("meta")) is not None:
         kwargs["meta"] = _deserialize_open_properties(_meta, config)
 
+    if (_permissions := output.get("permissions")) is not None:
+        kwargs["permissions"] = _deserialize_account_permissions(_permissions, config)
+
     if (_cloud_account_id := output.get("cloudAccountId")) is not None:
         kwargs["cloud_account_id"] = expect_type(str, _cloud_account_id)
 
-    if (_permissions := output.get("permissions")) is not None:
-        kwargs["permissions"] = _deserialize_account_permissions(_permissions, config)
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
+        )
+
+    if (_type := output.get("type")) is not None:
+        kwargs["type"] = expect_type(str, _type)
 
     return DescribeAccountOutput(**kwargs)
 
 
 async def _deserialize_error_describe_account(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -823,14 +891,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -844,40 +917,40 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_toms := output.get("toms")) is not None:
-        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
-
-    if (_location_id := output.get("locationId")) is not None:
-        kwargs["location_id"] = expect_type(str, _location_id)
+    if "assetId" not in output:
+        raise ServiceError(
+            'Expected to find "assetId" in the operation output, but it was not present.'
+        )
+    kwargs["asset_id"] = expect_type(str, output["assetId"])
 
-    if (_location_type := output.get("locationType")) is not None:
-        kwargs["location_type"] = expect_type(str, _location_type)
+    if (_type := output.get("type")) is not None:
+        kwargs["type"] = expect_type(str, _type)
 
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
-    if (_type := output.get("type")) is not None:
-        kwargs["type"] = expect_type(str, _type)
+    if (_toms := output.get("toms")) is not None:
+        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
 
     if (_tom_ids := output.get("tomIds")) is not None:
         kwargs["tom_ids"] = _deserialize_uuid_collection(_tom_ids, config)
 
     if (_location := output.get("location")) is not None:
         kwargs["location"] = _deserialize_headquarter_record(_location, config)
 
-    if "assetId" not in output:
-        raise ServiceError(
-            'Expected to find "assetId" in the operation output, but it was not present.'
-        )
-    kwargs["asset_id"] = expect_type(str, output["assetId"])
+    if (_location_type := output.get("locationType")) is not None:
+        kwargs["location_type"] = expect_type(str, _location_type)
+
+    if (_location_id := output.get("locationId")) is not None:
+        kwargs["location_id"] = expect_type(str, _location_id)
 
     return DescribeAssetOutput(**kwargs)
 
 
 async def _deserialize_error_describe_asset(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -890,14 +963,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -911,54 +989,54 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
-
     if (_source := output.get("source")) is not None:
         kwargs["source"] = expect_type(str, _source)
 
-    if (_compliance := output.get("compliance")) is not None:
-        kwargs["compliance"] = _deserialize_compliance_detail_list(_compliance, config)
-
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+    if (_snapshot := output.get("snapshot")) is not None:
+        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
 
-    if (_sample_tokens := output.get("sampleTokens")) is not None:
-        kwargs["sample_tokens"] = _deserialize_tokens(_sample_tokens, config)
+    if (_parent_id := output.get("parentId")) is not None:
+        kwargs["parent_id"] = expect_type(str, _parent_id)
 
-    if (_owner := output.get("owner")) is not None:
-        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
+    if (_compliance := output.get("compliance")) is not None:
+        kwargs["compliance"] = _deserialize_compliance_detail_list(_compliance, config)
 
     if "resourceId" not in output:
         raise ServiceError(
             'Expected to find "resourceId" in the operation output, but it was not present.'
         )
     kwargs["resource_id"] = expect_type(str, output["resourceId"])
 
-    if (_snapshot := output.get("snapshot")) is not None:
-        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
+    if (_owner := output.get("owner")) is not None:
+        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
 
-    if (_last_scanned := output.get("lastScanned")) is not None:
-        kwargs["last_scanned"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _last_scanned)
-        )
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
+
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
 
     if (_type := output.get("type")) is not None:
         kwargs["type"] = expect_type(str, _type)
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
+    if (_sample_tokens := output.get("sampleTokens")) is not None:
+        kwargs["sample_tokens"] = _deserialize_tokens(_sample_tokens, config)
 
-    if (_parent_id := output.get("parentId")) is not None:
-        kwargs["parent_id"] = expect_type(str, _parent_id)
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
+    if (_last_scanned := output.get("lastScanned")) is not None:
+        kwargs["last_scanned"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _last_scanned)
+        )
 
     return DescribeCatalogResourceOutput(**kwargs)
 
 
 async def _deserialize_error_describe_catalog_resource(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -971,14 +1049,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -997,26 +1080,26 @@
         output = json.loads(body)
 
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if "categoryLabel" not in output:
-        raise ServiceError(
-            'Expected to find "categoryLabel" in the operation output, but it was not present.'
-        )
-    kwargs["category_label"] = expect_type(str, output["categoryLabel"])
-
     if "description" not in output:
         raise ServiceError(
             'Expected to find "description" in the operation output, but it was not present.'
         )
     kwargs["description"] = expect_type(str, output["description"])
 
+    if "categoryLabel" not in output:
+        raise ServiceError(
+            'Expected to find "categoryLabel" in the operation output, but it was not present.'
+        )
+    kwargs["category_label"] = expect_type(str, output["categoryLabel"])
+
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
     return DescribeCategoryOutput(**kwargs)
 
@@ -1033,14 +1116,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1057,53 +1145,53 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
-    if (_type := output.get("type")) is not None:
-        kwargs["type"] = expect_type(str, _type)
-
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
-
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
-
-    if (_data_plane_ids := output.get("dataPlaneIds")) is not None:
-        kwargs["data_plane_ids"] = _deserialize_data_plane_ids(_data_plane_ids, config)
-
     if (_deleted_at := output.get("deletedAt")) is not None:
         kwargs["deleted_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _deleted_at)
         )
 
-    if "accountId" not in output:
-        raise ServiceError(
-            'Expected to find "accountId" in the operation output, but it was not present.'
-        )
-    kwargs["account_id"] = expect_type(str, output["accountId"])
-
     if (_cloud_account_id := output.get("cloudAccountId")) is not None:
         kwargs["cloud_account_id"] = expect_type(str, _cloud_account_id)
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
-        )
+    if (_data_plane_ids := output.get("dataPlaneIds")) is not None:
+        kwargs["data_plane_ids"] = _deserialize_data_plane_ids(_data_plane_ids, config)
+
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
 
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
     if (_permissions := output.get("permissions")) is not None:
         kwargs["permissions"] = _deserialize_account_permissions(_permissions, config)
 
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
+        )
+
+    if "accountId" not in output:
+        raise ServiceError(
+            'Expected to find "accountId" in the operation output, but it was not present.'
+        )
+    kwargs["account_id"] = expect_type(str, output["accountId"])
+
+    if (_type := output.get("type")) is not None:
+        kwargs["type"] = expect_type(str, _type)
+
     return DescribeCloudAccountOutput(**kwargs)
 
 
 async def _deserialize_error_describe_cloud_account(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1115,14 +1203,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1136,56 +1229,71 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_resource_id := output.get("resourceId")) is not None:
+        kwargs["resource_id"] = expect_type(str, _resource_id)
+
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
+        )
+
+    if (
+        _next_meta_data_sync_schedule := output.get("nextMetaDataSyncSchedule")
+    ) is not None:
+        kwargs["next_meta_data_sync_schedule"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _next_meta_data_sync_schedule)
+        )
+
+    if (_meta_data_sync_interval := output.get("metaDataSyncInterval")) is not None:
+        kwargs["meta_data_sync_interval"] = expect_type(str, _meta_data_sync_interval)
+
+    if (_params := output.get("params")) is not None:
+        kwargs["params"] = _deserialize_open_properties(_params, config)
+
     if "connectorId" not in output:
         raise ServiceError(
             'Expected to find "connectorId" in the operation output, but it was not present.'
         )
     kwargs["connector_id"] = expect_type(str, output["connectorId"])
 
-    if (_resource_account_id := output.get("resourceAccountId")) is not None:
-        kwargs["resource_account_id"] = expect_type(str, _resource_account_id)
-
-    if (_region := output.get("region")) is not None:
-        kwargs["region"] = expect_type(str, _region)
-
     if (_state := output.get("state")) is not None:
         kwargs["state"] = expect_type(str, _state)
 
-    if (_connector_type := output.get("connectorType")) is not None:
-        kwargs["connector_type"] = expect_type(str, _connector_type)
+    if (_resource_account_id := output.get("resourceAccountId")) is not None:
+        kwargs["resource_account_id"] = expect_type(str, _resource_account_id)
 
     if (_resource_type := output.get("resourceType")) is not None:
         kwargs["resource_type"] = expect_type(str, _resource_type)
 
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
+    if (_region := output.get("region")) is not None:
+        kwargs["region"] = expect_type(str, _region)
+
+    if (_is_meta_data_sync_running := output.get("isMetaDataSyncRunning")) is not None:
+        kwargs["is_meta_data_sync_running"] = expect_type(
+            bool, _is_meta_data_sync_running
+        )
+
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if (_resource_id := output.get("resourceId")) is not None:
-        kwargs["resource_id"] = expect_type(str, _resource_id)
-
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
-
     if (_data_plane_id := output.get("dataPlaneId")) is not None:
         kwargs["data_plane_id"] = expect_type(str, _data_plane_id)
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
-        )
-
-    if (_params := output.get("params")) is not None:
-        kwargs["params"] = _deserialize_open_properties(_params, config)
+    if (_connector_type := output.get("connectorType")) is not None:
+        kwargs["connector_type"] = expect_type(str, _connector_type)
 
     return DescribeConnectorOutput(**kwargs)
 
 
 async def _deserialize_error_describe_connector(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1198,14 +1306,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1219,26 +1332,26 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if "departmentId" not in output:
-        raise ServiceError(
-            'Expected to find "departmentId" in the operation output, but it was not present.'
-        )
-    kwargs["department_id"] = expect_type(str, output["departmentId"])
-
     if "name" not in output:
         raise ServiceError(
             'Expected to find "name" in the operation output, but it was not present.'
         )
     kwargs["name"] = expect_type(str, output["name"])
 
+    if "departmentId" not in output:
+        raise ServiceError(
+            'Expected to find "departmentId" in the operation output, but it was not present.'
+        )
+    kwargs["department_id"] = expect_type(str, output["departmentId"])
+
     return DescribeDepartmentOutput(**kwargs)
 
 
 async def _deserialize_error_describe_department(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1250,14 +1363,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1273,43 +1391,43 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if "recipientModelId" not in output:
+        raise ServiceError(
+            'Expected to find "recipientModelId" in the operation output, but it was not present.'
+        )
+    kwargs["recipient_model_id"] = expect_type(str, output["recipientModelId"])
+
     if "createdAt" not in output:
         raise ServiceError(
             'Expected to find "createdAt" in the operation output, but it was not present.'
         )
     kwargs["created_at"] = epoch_seconds_to_datetime(
         expect_type(int | float, output["createdAt"])
     )
 
-    if "discoverySource" not in output:
-        raise ServiceError(
-            'Expected to find "discoverySource" in the operation output, but it was not present.'
-        )
-    kwargs["discovery_source"] = _deserialize_discovery_source_list(
-        output["discoverySource"], config
-    )
-
     if "discoveredRecipientId" not in output:
         raise ServiceError(
             'Expected to find "discoveredRecipientId" in the operation output, but it was not present.'
         )
     kwargs["discovered_recipient_id"] = expect_type(
         str, output["discoveredRecipientId"]
     )
 
-    if "recipientModelId" not in output:
+    if "discoverySource" not in output:
         raise ServiceError(
-            'Expected to find "recipientModelId" in the operation output, but it was not present.'
+            'Expected to find "discoverySource" in the operation output, but it was not present.'
         )
-    kwargs["recipient_model_id"] = expect_type(str, output["recipientModelId"])
+    kwargs["discovery_source"] = _deserialize_discovery_source_list(
+        output["discoverySource"], config
+    )
 
     return DescribeDiscoveredRecipientOutput(**kwargs)
 
 
 async def _deserialize_error_describe_discovered_recipient(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1322,14 +1440,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1343,44 +1466,44 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
     if (_created_at := output.get("createdAt")) is not None:
         kwargs["created_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _created_at)
         )
 
-    if (_recipients := output.get("recipients")) is not None:
-        kwargs["recipients"] = _deserialize_recipients_discovered_of_domain_list(
-            _recipients, config
-        )
-
-    if (_frequency := output.get("frequency")) is not None:
-        kwargs["frequency"] = expect_type(str, _frequency)
-
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
-
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
-
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
+    if (_recipients := output.get("recipients")) is not None:
+        kwargs["recipients"] = _deserialize_recipients_discovered_of_domain_list(
+            _recipients, config
+        )
+
     if "domainId" not in output:
         raise ServiceError(
             'Expected to find "domainId" in the operation output, but it was not present.'
         )
     kwargs["domain_id"] = expect_type(str, output["domainId"])
 
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
+    if (_frequency := output.get("frequency")) is not None:
+        kwargs["frequency"] = expect_type(str, _frequency)
+
     return DescribeDomainOutput(**kwargs)
 
 
 async def _deserialize_error_describe_domain(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1392,14 +1515,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1413,43 +1541,43 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
-
-    if (_confidentiality := output.get("confidentiality")) is not None:
-        kwargs["confidentiality"] = _deserialize_dpia_confidentiality_risk(
-            _confidentiality, config
-        )
-
-    if (
-        _additional_information_files := output.get("additionalInformationFiles")
-    ) is not None:
-        kwargs["additional_information_files"] = _deserialize_uuid_collection(
-            _additional_information_files, config
+    if (_availability := output.get("availability")) is not None:
+        kwargs["availability"] = _deserialize_dpia_availability_risk(
+            _availability, config
         )
 
     if (_integrity := output.get("integrity")) is not None:
         kwargs["integrity"] = _deserialize_dpia_integrity_risk(_integrity, config)
 
     if (_privacy_framework := output.get("privacyFramework")) is not None:
         kwargs["privacy_framework"] = _deserialize_dpia_privacy_framework(
             _privacy_framework, config
         )
 
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
     if (_additional_information := output.get("additionalInformation")) is not None:
         kwargs["additional_information"] = expect_type(str, _additional_information)
 
-    if (_availability := output.get("availability")) is not None:
-        kwargs["availability"] = _deserialize_dpia_availability_risk(
-            _availability, config
+    if (
+        _additional_information_files := output.get("additionalInformationFiles")
+    ) is not None:
+        kwargs["additional_information_files"] = _deserialize_uuid_collection(
+            _additional_information_files, config
+        )
+
+    if (_confidentiality := output.get("confidentiality")) is not None:
+        kwargs["confidentiality"] = _deserialize_dpia_confidentiality_risk(
+            _confidentiality, config
         )
 
     return DescribeDpiaOutput(**kwargs)
 
 
 async def _deserialize_error_describe_dpia(
     http_response: HTTPResponse, config: Config
@@ -1463,14 +1591,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -1489,69 +1622,69 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_department := output.get("department")) is not None:
-        kwargs["department"] = expect_type(str, _department)
-
     if (_nif := output.get("nif")) is not None:
         kwargs["nif"] = expect_type(str, _nif)
 
-    if (_start_date := output.get("startDate")) is not None:
-        kwargs["start_date"] = expect_type(str, _start_date)
+    if (_manager_object := output.get("managerObject")) is not None:
+        kwargs["manager_object"] = _deserialize_manager_object(_manager_object, config)
 
-    if "employeeId" not in output:
+    if "surname" not in output:
         raise ServiceError(
-            'Expected to find "employeeId" in the operation output, but it was not present.'
+            'Expected to find "surname" in the operation output, but it was not present.'
         )
-    kwargs["employee_id"] = expect_type(str, output["employeeId"])
+    kwargs["surname"] = expect_type(str, output["surname"])
 
-    if (_manager := output.get("manager")) is not None:
-        kwargs["manager"] = expect_type(str, _manager)
+    if (_department := output.get("department")) is not None:
+        kwargs["department"] = expect_type(str, _department)
+
+    if (_start_date := output.get("startDate")) is not None:
+        kwargs["start_date"] = expect_type(str, _start_date)
 
     if (_end_date := output.get("endDate")) is not None:
         kwargs["end_date"] = expect_type(str, _end_date)
 
+    if (_reference_id := output.get("referenceId")) is not None:
+        kwargs["reference_id"] = expect_type(str, _reference_id)
+
     if "name" not in output:
         raise ServiceError(
             'Expected to find "name" in the operation output, but it was not present.'
         )
     kwargs["name"] = expect_type(str, output["name"])
 
+    if (_email := output.get("email")) is not None:
+        kwargs["email"] = expect_type(str, _email)
+
+    if (_department_object := output.get("departmentObject")) is not None:
+        kwargs["department_object"] = _deserialize_department_object(
+            _department_object, config
+        )
+
     if (_position := output.get("position")) is not None:
         kwargs["position"] = expect_type(str, _position)
 
     if "createdBy" not in output:
         raise ServiceError(
             'Expected to find "createdBy" in the operation output, but it was not present.'
         )
     kwargs["created_by"] = expect_type(str, output["createdBy"])
 
-    if (_email := output.get("email")) is not None:
-        kwargs["email"] = expect_type(str, _email)
-
-    if (_reference_id := output.get("referenceId")) is not None:
-        kwargs["reference_id"] = expect_type(str, _reference_id)
-
-    if "surname" not in output:
+    if "employeeId" not in output:
         raise ServiceError(
-            'Expected to find "surname" in the operation output, but it was not present.'
+            'Expected to find "employeeId" in the operation output, but it was not present.'
         )
-    kwargs["surname"] = expect_type(str, output["surname"])
-
-    if (_manager_object := output.get("managerObject")) is not None:
-        kwargs["manager_object"] = _deserialize_manager_object(_manager_object, config)
+    kwargs["employee_id"] = expect_type(str, output["employeeId"])
 
-    if (_department_object := output.get("departmentObject")) is not None:
-        kwargs["department_object"] = _deserialize_department_object(
-            _department_object, config
-        )
+    if (_manager := output.get("manager")) is not None:
+        kwargs["manager"] = expect_type(str, _manager)
 
     return DescribeEmployeeOutput(**kwargs)
 
 
 async def _deserialize_error_describe_employee(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1564,14 +1697,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1585,38 +1723,38 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if "headquarterId" not in output:
-        raise ServiceError(
-            'Expected to find "headquarterId" in the operation output, but it was not present.'
-        )
-    kwargs["headquarter_id"] = expect_type(str, output["headquarterId"])
-
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
+    if (_address := output.get("address")) is not None:
+        kwargs["address"] = expect_type(str, _address)
+
     if (_toms := output.get("toms")) is not None:
         kwargs["toms"] = _deserialize_tom_collection(_toms, config)
 
-    if (_city := output.get("city")) is not None:
-        kwargs["city"] = expect_type(str, _city)
-
-    if (_address := output.get("address")) is not None:
-        kwargs["address"] = expect_type(str, _address)
+    if "headquarterId" not in output:
+        raise ServiceError(
+            'Expected to find "headquarterId" in the operation output, but it was not present.'
+        )
+    kwargs["headquarter_id"] = expect_type(str, output["headquarterId"])
 
     if (_country := output.get("country")) is not None:
         kwargs["country"] = expect_type(str, _country)
 
     if (_zipcode := output.get("zipcode")) is not None:
         kwargs["zipcode"] = expect_type(str, _zipcode)
 
+    if (_city := output.get("city")) is not None:
+        kwargs["city"] = expect_type(str, _city)
+
     return DescribeHeadquarterOutput(**kwargs)
 
 
 async def _deserialize_error_describe_headquarter(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1628,14 +1766,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1649,85 +1792,85 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_has_finding := output.get("hasFinding")) is not None:
+        kwargs["has_finding"] = expect_type(bool, _has_finding)
+
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
     if (_sample_tokens := output.get("sampleTokens")) is not None:
         kwargs["sample_tokens"] = _deserialize_tokens(_sample_tokens, config)
 
+    if (_resource_name := output.get("resourceName")) is not None:
+        kwargs["resource_name"] = expect_type(str, _resource_name)
+
     if (_file_name := output.get("fileName")) is not None:
         kwargs["file_name"] = expect_type(str, _file_name)
 
-    if (_resource_id := output.get("resourceId")) is not None:
-        kwargs["resource_id"] = expect_type(str, _resource_id)
+    if (_user_email := output.get("userEmail")) is not None:
+        kwargs["user_email"] = expect_type(str, _user_email)
 
-    if (_scan_parameters := output.get("scanParameters")) is not None:
-        kwargs["scan_parameters"] = _deserialize_scan_parameters(
-            _scan_parameters, config
-        )
+    if (_snapshot := output.get("snapshot")) is not None:
+        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
+
+    if (_compliance := output.get("compliance")) is not None:
+        kwargs["compliance"] = _deserialize_compliance_detail_list(_compliance, config)
 
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
+        )
 
-    if (_resource_name := output.get("resourceName")) is not None:
-        kwargs["resource_name"] = expect_type(str, _resource_name)
+    if (_stats := output.get("stats")) is not None:
+        kwargs["stats"] = _deserialize_record_type(_stats, config)
 
-    if (_user_name := output.get("userName")) is not None:
-        kwargs["user_name"] = expect_type(str, _user_name)
+    if (_resource_type := output.get("resourceType")) is not None:
+        kwargs["resource_type"] = expect_type(str, _resource_type)
 
-    if (_parent_id := output.get("parentId")) is not None:
-        kwargs["parent_id"] = expect_type(str, _parent_id)
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
 
-    if (_user_email := output.get("userEmail")) is not None:
-        kwargs["user_email"] = expect_type(str, _user_email)
+    if (_tokens := output.get("tokens")) is not None:
+        kwargs["tokens"] = _deserialize_tokens(_tokens, config)
 
     if "id" not in output:
         raise ServiceError(
             'Expected to find "id" in the operation output, but it was not present.'
         )
     kwargs["id"] = expect_type(str, output["id"])
 
-    if (_tokens := output.get("tokens")) is not None:
-        kwargs["tokens"] = _deserialize_tokens(_tokens, config)
+    if (_scan_parameters := output.get("scanParameters")) is not None:
+        kwargs["scan_parameters"] = _deserialize_scan_parameters(
+            _scan_parameters, config
+        )
 
-    if (_scan_iteration_id := output.get("scanIterationId")) is not None:
-        kwargs["scan_iteration_id"] = expect_type(str, _scan_iteration_id)
+    if (_user_name := output.get("userName")) is not None:
+        kwargs["user_name"] = expect_type(str, _user_name)
 
     if (_scan_id := output.get("scanId")) is not None:
         kwargs["scan_id"] = expect_type(str, _scan_id)
 
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
-
-    if (_has_finding := output.get("hasFinding")) is not None:
-        kwargs["has_finding"] = expect_type(bool, _has_finding)
-
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
-        )
-
-    if (_resource_type := output.get("resourceType")) is not None:
-        kwargs["resource_type"] = expect_type(str, _resource_type)
-
-    if (_snapshot := output.get("snapshot")) is not None:
-        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
+    if (_scan_iteration_id := output.get("scanIterationId")) is not None:
+        kwargs["scan_iteration_id"] = expect_type(str, _scan_iteration_id)
 
-    if (_stats := output.get("stats")) is not None:
-        kwargs["stats"] = _deserialize_record_type(_stats, config)
+    if (_parent_id := output.get("parentId")) is not None:
+        kwargs["parent_id"] = expect_type(str, _parent_id)
 
-    if (_compliance := output.get("compliance")) is not None:
-        kwargs["compliance"] = _deserialize_compliance_detail_list(_compliance, config)
+    if (_resource_id := output.get("resourceId")) is not None:
+        kwargs["resource_id"] = expect_type(str, _resource_id)
 
     return DescribeInspectionResultOutput(**kwargs)
 
 
 async def _deserialize_error_describe_inspection_result(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1740,14 +1883,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1763,74 +1911,74 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_data_classification := output.get("dataClassification")) is not None:
-        kwargs["data_classification"] = _deserialize_unique_string_list(
-            _data_classification, config
-        )
+    if (_last_updated := output.get("lastUpdated")) is not None:
+        kwargs["last_updated"] = expect_type(str, _last_updated)
 
     if (_source := output.get("source")) is not None:
         kwargs["source"] = expect_type(str, _source)
 
-    if (_scan := output.get("scan")) is not None:
-        kwargs["scan"] = _deserialize_scan_information(_scan, config)
-
-    if (_properties := output.get("properties")) is not None:
-        kwargs["properties"] = _deserialize_open_properties(_properties, config)
+    if (_aka := output.get("aka")) is not None:
+        kwargs["aka"] = expect_type(str, _aka)
 
     if (_type := output.get("type")) is not None:
         kwargs["type"] = expect_type(str, _type)
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
-
-    if (_owner := output.get("owner")) is not None:
-        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
+    if (_meta := output.get("meta")) is not None:
+        kwargs["meta"] = _deserialize_open_properties(_meta, config)
 
     if (_parent_id := output.get("parentId")) is not None:
         kwargs["parent_id"] = expect_type(str, _parent_id)
 
-    if (_issue_id := output.get("issueId")) is not None:
-        kwargs["issue_id"] = expect_type(str, _issue_id)
-
-    if (_data_categories := output.get("dataCategories")) is not None:
-        kwargs["data_categories"] = _deserialize_unique_string_list(
-            _data_categories, config
+    if (_data_classification := output.get("dataClassification")) is not None:
+        kwargs["data_classification"] = _deserialize_unique_string_list(
+            _data_classification, config
         )
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
-
-    if (_severity_score := output.get("severityScore")) is not None:
-        kwargs["severity_score"] = expect_type(int, _severity_score)
-
-    if (_meta := output.get("meta")) is not None:
-        kwargs["meta"] = _deserialize_open_properties(_meta, config)
-
     if (_failed_rules := output.get("failedRules")) is not None:
         kwargs["failed_rules"] = _deserialize_unique_string_list(_failed_rules, config)
 
-    if (_last_updated := output.get("lastUpdated")) is not None:
-        kwargs["last_updated"] = expect_type(str, _last_updated)
+    if (_scan := output.get("scan")) is not None:
+        kwargs["scan"] = _deserialize_scan_information(_scan, config)
 
     if "resourceId" not in output:
         raise ServiceError(
             'Expected to find "resourceId" in the operation output, but it was not present.'
         )
     kwargs["resource_id"] = expect_type(str, output["resourceId"])
 
     if (_first_seen := output.get("firstSeen")) is not None:
         kwargs["first_seen"] = expect_type(str, _first_seen)
 
-    if (_aka := output.get("aka")) is not None:
-        kwargs["aka"] = expect_type(str, _aka)
+    if (_issue_id := output.get("issueId")) is not None:
+        kwargs["issue_id"] = expect_type(str, _issue_id)
+
+    if (_data_categories := output.get("dataCategories")) is not None:
+        kwargs["data_categories"] = _deserialize_unique_string_list(
+            _data_categories, config
+        )
+
+    if (_severity_score := output.get("severityScore")) is not None:
+        kwargs["severity_score"] = expect_type(int, _severity_score)
+
+    if (_owner := output.get("owner")) is not None:
+        kwargs["owner"] = _deserialize_owner_object_list(_owner, config)
+
+    if (_properties := output.get("properties")) is not None:
+        kwargs["properties"] = _deserialize_open_properties(_properties, config)
+
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
 
     return DescribeInventoryResourceOutput(**kwargs)
 
 
 async def _deserialize_error_describe_inventory_resource(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -1843,14 +1991,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1864,58 +2017,58 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
-        )
-
-    if (_resource_id := output.get("resourceId")) is not None:
-        kwargs["resource_id"] = expect_type(str, _resource_id)
+    if (_severity := output.get("severity")) is not None:
+        kwargs["severity"] = expect_type(str, _severity)
 
-    if "issueId" not in output:
-        raise ServiceError(
-            'Expected to find "issueId" in the operation output, but it was not present.'
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
         )
-    kwargs["issue_id"] = expect_type(str, output["issueId"])
 
     if (_events := output.get("events")) is not None:
         kwargs["events"] = _deserialize_data_security_event_list(_events, config)
 
     if (_notifications := output.get("notifications")) is not None:
         kwargs["notifications"] = _deserialize_issue_notification_list(
             _notifications, config
         )
 
-    if (_state := output.get("state")) is not None:
-        kwargs["state"] = expect_type(str, _state)
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
+        )
+
+    if (_security_risk := output.get("securityRisk")) is not None:
+        kwargs["security_risk"] = _deserialize_security_risk(_security_risk, config)
 
     if (_resource := output.get("resource")) is not None:
         kwargs["resource"] = _deserialize_issue_resource_details(_resource, config)
 
-    if (_security_risk := output.get("securityRisk")) is not None:
-        kwargs["security_risk"] = _deserialize_security_risk(_security_risk, config)
+    if "issueId" not in output:
+        raise ServiceError(
+            'Expected to find "issueId" in the operation output, but it was not present.'
+        )
+    kwargs["issue_id"] = expect_type(str, output["issueId"])
+
+    if (_state := output.get("state")) is not None:
+        kwargs["state"] = expect_type(str, _state)
+
+    if (_resource_id := output.get("resourceId")) is not None:
+        kwargs["resource_id"] = expect_type(str, _resource_id)
 
     if (_compliance_risk := output.get("complianceRisk")) is not None:
         kwargs["compliance_risk"] = _deserialize_compliance_risk(
             _compliance_risk, config
         )
 
-    if (_severity := output.get("severity")) is not None:
-        kwargs["severity"] = expect_type(str, _severity)
-
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
-        )
-
     return DescribeIssueOutput(**kwargs)
 
 
 async def _deserialize_error_describe_issue(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -1927,14 +2080,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -1950,141 +2108,141 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_data_types := output.get("dataTypes")) is not None:
+        kwargs["data_types"] = _deserialize_data_type_collection(_data_types, config)
+
+    if (_is_data_stored := output.get("isDataStored")) is not None:
+        kwargs["is_data_stored"] = expect_type(bool, _is_data_stored)
+
     if (_asset_objects := output.get("assetObjects")) is not None:
         kwargs["asset_objects"] = _deserialize_processing_activity_asset_list(
             _asset_objects, config
         )
 
-    if (_company_role := output.get("companyRole")) is not None:
-        kwargs["company_role"] = expect_type(str, _company_role)
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
 
-    if (_data_types := output.get("dataTypes")) is not None:
-        kwargs["data_types"] = _deserialize_data_type_collection(_data_types, config)
+    if (_infotype_volume := output.get("infotypeVolume")) is not None:
+        kwargs["infotype_volume"] = expect_type(str, _infotype_volume)
 
-    if (
-        _processing_frequency_comment := output.get("processingFrequencyComment")
-    ) is not None:
-        kwargs["processing_frequency_comment"] = expect_type(
-            str, _processing_frequency_comment
+    if (_additional_info_files := output.get("additionalInfoFiles")) is not None:
+        kwargs["additional_info_files"] = _deserialize_uuid_collection(
+            _additional_info_files, config
         )
 
-    if (_created_by := output.get("createdBy")) is not None:
-        kwargs["created_by"] = expect_type(str, _created_by)
+    if (_processing_frequency := output.get("processingFrequency")) is not None:
+        kwargs["processing_frequency"] = expect_type(str, _processing_frequency)
 
-    if (_contact_person_employee := output.get("contactPersonEmployee")) is not None:
-        kwargs["contact_person_employee"] = _deserialize_processing_activity_employee(
-            _contact_person_employee, config
+    if (
+        _are_access_requests_managed := output.get("areAccessRequestsManaged")
+    ) is not None:
+        kwargs["are_access_requests_managed"] = expect_type(
+            bool, _are_access_requests_managed
         )
 
-    if (_lawful_basis := output.get("lawfulBasis")) is not None:
-        kwargs["lawful_basis"] = _deserialize_lawful_basis_collection(
-            _lawful_basis, config
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
         )
 
-    if (_infotypes := output.get("infotypes")) is not None:
-        kwargs["infotypes"] = _deserialize_infotypes_list(_infotypes, config)
-
     if "processingActivityId" not in output:
         raise ServiceError(
             'Expected to find "processingActivityId" in the operation output, but it was not present.'
         )
     kwargs["processing_activity_id"] = expect_type(str, output["processingActivityId"])
 
-    if (_data_sources := output.get("dataSources")) is not None:
-        kwargs["data_sources"] = (
-            _deserialize_processing_activitiy_data_source_collection(
-                _data_sources, config
-            )
-        )
-
-    if (_management_methods := output.get("managementMethods")) is not None:
-        kwargs["management_methods"] = _deserialize_management_method_collection(
-            _management_methods, config
-        )
+    if (_infotypes := output.get("infotypes")) is not None:
+        kwargs["infotypes"] = _deserialize_infotypes_list(_infotypes, config)
 
     if (_retention_period := output.get("retentionPeriod")) is not None:
         kwargs["retention_period"] = _deserialize_retention_period(
             _retention_period, config
         )
 
-    if (_infotype_volume := output.get("infotypeVolume")) is not None:
-        kwargs["infotype_volume"] = expect_type(str, _infotype_volume)
-
-    if (
-        _are_access_requests_managed := output.get("areAccessRequestsManaged")
-    ) is not None:
-        kwargs["are_access_requests_managed"] = expect_type(
-            bool, _are_access_requests_managed
+    if (_infotype_categories := output.get("infotypeCategories")) is not None:
+        kwargs["infotype_categories"] = _deserialize_infotype_category_list(
+            _infotype_categories, config
         )
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
+    if (_data_sources := output.get("dataSources")) is not None:
+        kwargs["data_sources"] = (
+            _deserialize_processing_activitiy_data_source_collection(
+                _data_sources, config
+            )
         )
 
-    if (_additional_info_files := output.get("additionalInfoFiles")) is not None:
-        kwargs["additional_info_files"] = _deserialize_uuid_collection(
-            _additional_info_files, config
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
         )
 
-    if (_processing_frequency := output.get("processingFrequency")) is not None:
-        kwargs["processing_frequency"] = expect_type(str, _processing_frequency)
-
     if (_additional_info := output.get("additionalInfo")) is not None:
         kwargs["additional_info"] = expect_type(str, _additional_info)
 
-    if (_model_id := output.get("modelId")) is not None:
-        kwargs["model_id"] = expect_type(str, _model_id)
+    if (_department_objects := output.get("departmentObjects")) is not None:
+        kwargs["department_objects"] = _deserialize_processing_activity_department_list(
+            _department_objects, config
+        )
 
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
+    if (_retention_period_comment := output.get("retentionPeriodComment")) is not None:
+        kwargs["retention_period_comment"] = expect_type(str, _retention_period_comment)
+
+    if (_active := output.get("active")) is not None:
+        kwargs["active"] = expect_type(bool, _active)
+
+    if (_management_methods := output.get("managementMethods")) is not None:
+        kwargs["management_methods"] = _deserialize_management_method_collection(
+            _management_methods, config
         )
 
-    if (_data_subjects := output.get("dataSubjects")) is not None:
-        kwargs["data_subjects"] = _deserialize_data_subject_collection(
-            _data_subjects, config
+    if (_purpose := output.get("purpose")) is not None:
+        kwargs["purpose"] = expect_type(str, _purpose)
+
+    if (_lawful_basis := output.get("lawfulBasis")) is not None:
+        kwargs["lawful_basis"] = _deserialize_lawful_basis_collection(
+            _lawful_basis, config
         )
 
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
+    if (_contact_person_employee := output.get("contactPersonEmployee")) is not None:
+        kwargs["contact_person_employee"] = _deserialize_processing_activity_employee(
+            _contact_person_employee, config
+        )
+
     if (_recipient_objects := output.get("recipientObjects")) is not None:
         kwargs["recipient_objects"] = _deserialize_processing_activity_recipient_list(
             _recipient_objects, config
         )
 
-    if (_infotype_categories := output.get("infotypeCategories")) is not None:
-        kwargs["infotype_categories"] = _deserialize_infotype_category_list(
-            _infotype_categories, config
-        )
-
-    if (_active := output.get("active")) is not None:
-        kwargs["active"] = expect_type(bool, _active)
-
-    if (_retention_period_comment := output.get("retentionPeriodComment")) is not None:
-        kwargs["retention_period_comment"] = expect_type(str, _retention_period_comment)
+    if (_model_id := output.get("modelId")) is not None:
+        kwargs["model_id"] = expect_type(str, _model_id)
 
-    if (_is_data_stored := output.get("isDataStored")) is not None:
-        kwargs["is_data_stored"] = expect_type(bool, _is_data_stored)
+    if (_company_role := output.get("companyRole")) is not None:
+        kwargs["company_role"] = expect_type(str, _company_role)
 
-    if (_purpose := output.get("purpose")) is not None:
-        kwargs["purpose"] = expect_type(str, _purpose)
+    if (_data_subjects := output.get("dataSubjects")) is not None:
+        kwargs["data_subjects"] = _deserialize_data_subject_collection(
+            _data_subjects, config
+        )
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
+    if (_created_by := output.get("createdBy")) is not None:
+        kwargs["created_by"] = expect_type(str, _created_by)
 
-    if (_department_objects := output.get("departmentObjects")) is not None:
-        kwargs["department_objects"] = _deserialize_processing_activity_department_list(
-            _department_objects, config
+    if (
+        _processing_frequency_comment := output.get("processingFrequencyComment")
+    ) is not None:
+        kwargs["processing_frequency_comment"] = expect_type(
+            str, _processing_frequency_comment
         )
 
     return DescribeProcessingActivityOutput(**kwargs)
 
 
 async def _deserialize_error_describe_processing_activity(
     http_response: HTTPResponse, config: Config
@@ -2098,14 +2256,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -2124,60 +2287,60 @@
         output = json.loads(body)
 
     if (_recipient_warranties := output.get("recipientWarranties")) is not None:
         kwargs["recipient_warranties"] = _deserialize_warranty_list(
             _recipient_warranties, config
         )
 
-    if (_data_storage_location := output.get("dataStorageLocation")) is not None:
-        kwargs["data_storage_location"] = _deserialize_country_list(
-            _data_storage_location, config
-        )
+    if (_state := output.get("state")) is not None:
+        kwargs["state"] = expect_type(str, _state)
 
     if (_business_name := output.get("businessName")) is not None:
         kwargs["business_name"] = expect_type(str, _business_name)
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
-
-    if (_role := output.get("role")) is not None:
-        kwargs["role"] = expect_type(str, _role)
-
-    if (_dpa_files := output.get("dpaFiles")) is not None:
-        kwargs["dpa_files"] = _deserialize_uuid_collection(_dpa_files, config)
+    if (_dpa := output.get("dpa")) is not None:
+        kwargs["dpa"] = expect_type(str, _dpa)
 
     if (_dpa_status := output.get("dpaStatus")) is not None:
         kwargs["dpa_status"] = expect_type(str, _dpa_status)
 
-    if (_recipient_model_id := output.get("recipientModelId")) is not None:
-        kwargs["recipient_model_id"] = expect_type(str, _recipient_model_id)
-
-    if (_country := output.get("country")) is not None:
-        kwargs["country"] = expect_type(str, _country)
-
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
+    if (_discovery_source := output.get("discoverySource")) is not None:
+        kwargs["discovery_source"] = _deserialize_discovery_source_list(
+            _discovery_source, config
+        )
 
     if (_category := output.get("category")) is not None:
         kwargs["category"] = expect_type(str, _category)
 
     if (_discovered_date := output.get("discoveredDate")) is not None:
         kwargs["discovered_date"] = epoch_seconds_to_datetime(
             expect_type(int | float, _discovered_date)
         )
 
-    if (_dpa := output.get("dpa")) is not None:
-        kwargs["dpa"] = expect_type(str, _dpa)
+    if (_role := output.get("role")) is not None:
+        kwargs["role"] = expect_type(str, _role)
 
-    if (_state := output.get("state")) is not None:
-        kwargs["state"] = expect_type(str, _state)
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
 
-    if (_discovery_source := output.get("discoverySource")) is not None:
-        kwargs["discovery_source"] = _deserialize_discovery_source_list(
-            _discovery_source, config
+    if (_country := output.get("country")) is not None:
+        kwargs["country"] = expect_type(str, _country)
+
+    if (_recipient_model_id := output.get("recipientModelId")) is not None:
+        kwargs["recipient_model_id"] = expect_type(str, _recipient_model_id)
+
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
+    if (_dpa_files := output.get("dpaFiles")) is not None:
+        kwargs["dpa_files"] = _deserialize_uuid_collection(_dpa_files, config)
+
+    if (_data_storage_location := output.get("dataStorageLocation")) is not None:
+        kwargs["data_storage_location"] = _deserialize_country_list(
+            _data_storage_location, config
         )
 
     return DescribeRecipientOutput(**kwargs)
 
 
 async def _deserialize_error_describe_recipient(
     http_response: HTTPResponse, config: Config
@@ -2191,14 +2354,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -2217,96 +2385,96 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_connector_type := output.get("connectorType")) is not None:
-        kwargs["connector_type"] = expect_type(str, _connector_type)
-
-    if (_data_plane_name := output.get("dataPlaneName")) is not None:
-        kwargs["data_plane_name"] = expect_type(str, _data_plane_name)
-
     if (_status := output.get("status")) is not None:
         kwargs["status"] = expect_type(str, _status)
 
-    if (_data_plane_slug := output.get("dataPlaneSlug")) is not None:
-        kwargs["data_plane_slug"] = expect_type(str, _data_plane_slug)
-
     if (_data_plane_id := output.get("dataPlaneId")) is not None:
         kwargs["data_plane_id"] = expect_type(str, _data_plane_id)
 
-    if "scanId" not in output:
-        raise ServiceError(
-            'Expected to find "scanId" in the operation output, but it was not present.'
-        )
-    kwargs["scan_id"] = expect_type(str, output["scanId"])
-
-    if (_connector_id := output.get("connectorId")) is not None:
-        kwargs["connector_id"] = expect_type(str, _connector_id)
+    if (_snapshot := output.get("snapshot")) is not None:
+        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
 
     if (_scan_type := output.get("scanType")) is not None:
         kwargs["scan_type"] = expect_type(str, _scan_type)
 
-    if (_schedule_type := output.get("scheduleType")) is not None:
-        kwargs["schedule_type"] = expect_type(str, _schedule_type)
+    if (_elapsed_time_ms := output.get("elapsedTimeMs")) is not None:
+        kwargs["elapsed_time_ms"] = expect_type(int, _elapsed_time_ms)
 
-    if (_snapshot := output.get("snapshot")) is not None:
-        kwargs["snapshot"] = _deserialize_inspection_result_snapshot(_snapshot, config)
+    if (_next_execution := output.get("nextExecution")) is not None:
+        kwargs["next_execution"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _next_execution)
+        )
+
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
+        )
+
+    if (_connector_type := output.get("connectorType")) is not None:
+        kwargs["connector_type"] = expect_type(str, _connector_type)
+
+    if (_stats := output.get("stats")) is not None:
+        kwargs["stats"] = _deserialize_scan_stats(_stats, config)
+
+    if (_scan_limits := output.get("scanLimits")) is not None:
+        kwargs["scan_limits"] = _deserialize_scan_limits(_scan_limits, config)
+
+    if (_name := output.get("name")) is not None:
+        kwargs["name"] = expect_type(str, _name)
+
+    if (_scan_filter := output.get("scanFilter")) is not None:
+        kwargs["scan_filter"] = _deserialize_scan_filter_list(_scan_filter, config)
+
+    if (_resource_type := output.get("resourceType")) is not None:
+        kwargs["resource_type"] = expect_type(str, _resource_type)
+
+    if (_resources := output.get("resources")) is not None:
+        kwargs["resources"] = _deserialize_scan_resources(_resources, config)
 
     if (_updated_at := output.get("updatedAt")) is not None:
         kwargs["updated_at"] = epoch_seconds_to_datetime(
             expect_type(int | float, _updated_at)
         )
 
-    if (_name := output.get("name")) is not None:
-        kwargs["name"] = expect_type(str, _name)
+    if (_schedule_type := output.get("scheduleType")) is not None:
+        kwargs["schedule_type"] = expect_type(str, _schedule_type)
+
+    if (_cron := output.get("cron")) is not None:
+        kwargs["cron"] = expect_type(str, _cron)
 
     if (_schedule := output.get("schedule")) is not None:
         kwargs["schedule"] = _deserialize_scan_schedule(_schedule, config)
 
-    if (_cron := output.get("cron")) is not None:
-        kwargs["cron"] = expect_type(str, _cron)
+    if "scanId" not in output:
+        raise ServiceError(
+            'Expected to find "scanId" in the operation output, but it was not present.'
+        )
+    kwargs["scan_id"] = expect_type(str, output["scanId"])
+
+    if (_connector_id := output.get("connectorId")) is not None:
+        kwargs["connector_id"] = expect_type(str, _connector_id)
 
     if (_meta := output.get("meta")) is not None:
         kwargs["meta"] = _deserialize_scan_meta(_meta, config)
 
-    if (_resource_type := output.get("resourceType")) is not None:
-        kwargs["resource_type"] = expect_type(str, _resource_type)
-
-    if (_scan_filter := output.get("scanFilter")) is not None:
-        kwargs["scan_filter"] = _deserialize_scan_filter_list(_scan_filter, config)
-
-    if (_stats := output.get("stats")) is not None:
-        kwargs["stats"] = _deserialize_scan_stats(_stats, config)
+    if (_data_plane_name := output.get("dataPlaneName")) is not None:
+        kwargs["data_plane_name"] = expect_type(str, _data_plane_name)
 
     if (_inspection_policy := output.get("inspectionPolicy")) is not None:
         kwargs["inspection_policy"] = _deserialize_inspection_policy(
             _inspection_policy, config
         )
 
-    if (_scan_limits := output.get("scanLimits")) is not None:
-        kwargs["scan_limits"] = _deserialize_scan_limits(_scan_limits, config)
-
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
-        )
-
-    if (_resources := output.get("resources")) is not None:
-        kwargs["resources"] = _deserialize_scan_resources(_resources, config)
-
-    if (_elapsed_time_ms := output.get("elapsedTimeMs")) is not None:
-        kwargs["elapsed_time_ms"] = expect_type(int, _elapsed_time_ms)
-
-    if (_next_execution := output.get("nextExecution")) is not None:
-        kwargs["next_execution"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _next_execution)
-        )
+    if (_data_plane_slug := output.get("dataPlaneSlug")) is not None:
+        kwargs["data_plane_slug"] = expect_type(str, _data_plane_slug)
 
     return DescribeScanOutput(**kwargs)
 
 
 async def _deserialize_error_describe_scan(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -2319,14 +2487,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -2340,122 +2513,122 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_comment := output.get("comment")) is not None:
-        kwargs["comment"] = expect_type(str, _comment)
-
-    if (
-        _matching_merging_records_involved := output.get(
-            "matchingMergingRecordsInvolved"
-        )
-    ) is not None:
-        kwargs["matching_merging_records_involved"] = expect_type(
-            bool, _matching_merging_records_involved
-        )
-
-    if (_classifying_data_subject := output.get("classifyingDataSubject")) is not None:
-        kwargs["classifying_data_subject"] = expect_type(
-            bool, _classifying_data_subject
-        )
-
     if (
         _automated_decision_making := output.get("automatedDecisionMaking")
     ) is not None:
         kwargs["automated_decision_making"] = expect_type(
             bool, _automated_decision_making
         )
 
     if (
-        _large_scale_data_processing := output.get("largeScaleDataProcessing")
-    ) is not None:
-        kwargs["large_scale_data_processing"] = expect_type(
-            bool, _large_scale_data_processing
-        )
-
-    if (
         _processing_confidential_sensitive_data := output.get(
             "processingConfidentialSensitiveData"
         )
     ) is not None:
         kwargs["processing_confidential_sensitive_data"] = expect_type(
             bool, _processing_confidential_sensitive_data
         )
 
     if (
-        _prevent_data_subjects_exercising_their_rights := output.get(
-            "preventDataSubjectsExercisingTheirRights"
+        _matching_merging_records_involved := output.get(
+            "matchingMergingRecordsInvolved"
         )
     ) is not None:
-        kwargs["prevent_data_subjects_exercising_their_rights"] = expect_type(
-            bool, _prevent_data_subjects_exercising_their_rights
+        kwargs["matching_merging_records_involved"] = expect_type(
+            bool, _matching_merging_records_involved
         )
 
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
     if (
-        _extensive_automated_evaluation_characteristics := output.get(
-            "extensiveAutomatedEvaluationCharacteristics"
+        _monitoring_publicly_accessible_areas := output.get(
+            "monitoringPubliclyAccessibleAreas"
         )
     ) is not None:
-        kwargs["extensive_automated_evaluation_characteristics"] = expect_type(
-            bool, _extensive_automated_evaluation_characteristics
+        kwargs["monitoring_publicly_accessible_areas"] = expect_type(
+            bool, _monitoring_publicly_accessible_areas
         )
 
-    if (_blacklist := output.get("blacklist")) is not None:
-        kwargs["blacklist"] = expect_type(bool, _blacklist)
+    if (_comment := output.get("comment")) is not None:
+        kwargs["comment"] = expect_type(str, _comment)
 
     if (_dpia_status := output.get("dpiaStatus")) is not None:
         kwargs["dpia_status"] = expect_type(str, _dpia_status)
 
     if (
+        _large_scale_data_processing := output.get("largeScaleDataProcessing")
+    ) is not None:
+        kwargs["large_scale_data_processing"] = expect_type(
+            bool, _large_scale_data_processing
+        )
+
+    if (
         _processing_vulnerable_data_subject := output.get(
             "processingVulnerableDataSubject"
         )
     ) is not None:
         kwargs["processing_vulnerable_data_subject"] = expect_type(
             bool, _processing_vulnerable_data_subject
         )
 
     if (
-        _innovative_technologies_used := output.get("innovativeTechnologiesUsed")
-    ) is not None:
-        kwargs["innovative_technologies_used"] = expect_type(
-            bool, _innovative_technologies_used
-        )
-
-    if (
-        _monitoring_publicly_accessible_areas := output.get(
-            "monitoringPubliclyAccessibleAreas"
+        _systematic_monitoring_data_subject := output.get(
+            "systematicMonitoringDataSubject"
         )
     ) is not None:
-        kwargs["monitoring_publicly_accessible_areas"] = expect_type(
-            bool, _monitoring_publicly_accessible_areas
+        kwargs["systematic_monitoring_data_subject"] = expect_type(
+            bool, _systematic_monitoring_data_subject
         )
 
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
-
     if (
         _large_scale_processing_sensitive_data := output.get(
             "largeScaleProcessingSensitiveData"
         )
     ) is not None:
         kwargs["large_scale_processing_sensitive_data"] = expect_type(
             bool, _large_scale_processing_sensitive_data
         )
 
     if (
-        _systematic_monitoring_data_subject := output.get(
-            "systematicMonitoringDataSubject"
+        _prevent_data_subjects_exercising_their_rights := output.get(
+            "preventDataSubjectsExercisingTheirRights"
         )
     ) is not None:
-        kwargs["systematic_monitoring_data_subject"] = expect_type(
-            bool, _systematic_monitoring_data_subject
+        kwargs["prevent_data_subjects_exercising_their_rights"] = expect_type(
+            bool, _prevent_data_subjects_exercising_their_rights
+        )
+
+    if (_blacklist := output.get("blacklist")) is not None:
+        kwargs["blacklist"] = expect_type(bool, _blacklist)
+
+    if (_classifying_data_subject := output.get("classifyingDataSubject")) is not None:
+        kwargs["classifying_data_subject"] = expect_type(
+            bool, _classifying_data_subject
+        )
+
+    if (
+        _extensive_automated_evaluation_characteristics := output.get(
+            "extensiveAutomatedEvaluationCharacteristics"
+        )
+    ) is not None:
+        kwargs["extensive_automated_evaluation_characteristics"] = expect_type(
+            bool, _extensive_automated_evaluation_characteristics
+        )
+
+    if (
+        _innovative_technologies_used := output.get("innovativeTechnologiesUsed")
+    ) is not None:
+        kwargs["innovative_technologies_used"] = expect_type(
+            bool, _innovative_technologies_used
         )
 
     return DescribeThresholdOutput(**kwargs)
 
 
 async def _deserialize_error_describe_threshold(
     http_response: HTTPResponse, config: Config
@@ -2469,14 +2642,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -2495,43 +2673,43 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_list_ := output.get("list")) is not None:
-        kwargs["list_"] = expect_type(str, _list_)
+    if (_note := output.get("note")) is not None:
+        kwargs["note"] = expect_type(str, _note)
 
-    if (_category := output.get("category")) is not None:
-        kwargs["category"] = expect_type(str, _category)
+    if (_document_files := output.get("documentFiles")) is not None:
+        kwargs["document_files"] = _deserialize_uuid_collection(_document_files, config)
 
     if (_object_category := output.get("objectCategory")) is not None:
         kwargs["object_category"] = expect_type(str, _object_category)
 
+    if (_reference_code := output.get("referenceCode")) is not None:
+        kwargs["reference_code"] = expect_type(str, _reference_code)
+
     if (_description := output.get("description")) is not None:
         kwargs["description"] = expect_type(str, _description)
 
+    if (_status := output.get("status")) is not None:
+        kwargs["status"] = expect_type(str, _status)
+
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
-    if (_type := output.get("type")) is not None:
-        kwargs["type"] = expect_type(str, _type)
-
-    if (_reference_code := output.get("referenceCode")) is not None:
-        kwargs["reference_code"] = expect_type(str, _reference_code)
-
-    if (_status := output.get("status")) is not None:
-        kwargs["status"] = expect_type(str, _status)
+    if (_list_ := output.get("list")) is not None:
+        kwargs["list_"] = expect_type(str, _list_)
 
-    if (_document_files := output.get("documentFiles")) is not None:
-        kwargs["document_files"] = _deserialize_uuid_collection(_document_files, config)
+    if (_category := output.get("category")) is not None:
+        kwargs["category"] = expect_type(str, _category)
 
-    if (_note := output.get("note")) is not None:
-        kwargs["note"] = expect_type(str, _note)
+    if (_type := output.get("type")) is not None:
+        kwargs["type"] = expect_type(str, _type)
 
     return DescribeTomOutput(**kwargs)
 
 
 async def _deserialize_error_describe_tom(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -2544,14 +2722,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -2570,55 +2753,55 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_connector_id := output.get("connectorId")) is not None:
-        kwargs["connector_id"] = expect_type(str, _connector_id)
+    if (_connector_source_type := output.get("connectorSourceType")) is not None:
+        kwargs["connector_source_type"] = expect_type(str, _connector_source_type)
 
-    if (_email := output.get("email")) is not None:
-        kwargs["email"] = expect_type(str, _email)
+    if (_deleted_at := output.get("deletedAt")) is not None:
+        kwargs["deleted_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _deleted_at)
+        )
 
     if "userId" not in output:
         raise ServiceError(
             'Expected to find "userId" in the operation output, but it was not present.'
         )
     kwargs["user_id"] = expect_type(str, output["userId"])
 
-    if (_deleted_at := output.get("deletedAt")) is not None:
-        kwargs["deleted_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _deleted_at)
+    if (_updated_at := output.get("updatedAt")) is not None:
+        kwargs["updated_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _updated_at)
         )
 
-    if (_connector_source_type := output.get("connectorSourceType")) is not None:
-        kwargs["connector_source_type"] = expect_type(str, _connector_source_type)
+    if (_created_at := output.get("createdAt")) is not None:
+        kwargs["created_at"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _created_at)
+        )
 
-    if (_external := output.get("external")) is not None:
-        kwargs["external"] = expect_type(bool, _external)
+    if (_connector_id := output.get("connectorId")) is not None:
+        kwargs["connector_id"] = expect_type(str, _connector_id)
 
     if (_connector_user_id := output.get("connectorUserId")) is not None:
         kwargs["connector_user_id"] = expect_type(str, _connector_user_id)
 
-    if (_created_at := output.get("createdAt")) is not None:
-        kwargs["created_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _created_at)
-        )
+    if (_external := output.get("external")) is not None:
+        kwargs["external"] = expect_type(bool, _external)
 
     if (_connector_username := output.get("connectorUsername")) is not None:
         kwargs["connector_username"] = expect_type(str, _connector_username)
 
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
-    if (_updated_at := output.get("updatedAt")) is not None:
-        kwargs["updated_at"] = epoch_seconds_to_datetime(
-            expect_type(int | float, _updated_at)
-        )
+    if (_email := output.get("email")) is not None:
+        kwargs["email"] = expect_type(str, _email)
 
     return DescribeUserProfileOutput(**kwargs)
 
 
 async def _deserialize_error_describe_user_profile(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -2631,14 +2814,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -2680,14 +2868,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_assets(
     http_response: HTTPResponse, config: Config
 ) -> ListAssetsOutput:
@@ -2702,23 +2895,23 @@
 
     if "total" not in output:
         raise ServiceError(
             'Expected to find "total" in the operation output, but it was not present.'
         )
     kwargs["total"] = expect_type(int, output["total"])
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     if "assets" not in output:
         raise ServiceError(
             'Expected to find "assets" in the operation output, but it was not present.'
         )
     kwargs["assets"] = _deserialize_asset_list(output["assets"], config)
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     return ListAssetsOutput(**kwargs)
 
 
 async def _deserialize_error_list_assets(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -2730,14 +2923,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_catalog_leaf_resources(
     http_response: HTTPResponse, config: Config
 ) -> ListCatalogLeafResourcesOutput:
@@ -2751,20 +2949,20 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_resources := output.get("resources")) is not None:
         kwargs["resources"] = _deserialize_leaf_resources_data_list(_resources, config)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     if (_count := output.get("count")) is not None:
         kwargs["count"] = expect_type(int, _count)
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     return ListCatalogLeafResourcesOutput(**kwargs)
 
 
 async def _deserialize_error_list_catalog_leaf_resources(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -2776,14 +2974,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_catalog_leaf_resources_export(
     http_response: HTTPResponse, config: Config
 ) -> ListCatalogLeafResourcesExportOutput:
@@ -2816,14 +3019,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_connectors(
     http_response: HTTPResponse, config: Config
 ) -> ListConnectorsOutput:
@@ -2860,14 +3068,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_departments(
     http_response: HTTPResponse, config: Config
 ) -> ListDepartmentsOutput:
@@ -2882,23 +3095,23 @@
 
     if "departments" not in output:
         raise ServiceError(
             'Expected to find "departments" in the operation output, but it was not present.'
         )
     kwargs["departments"] = _deserialize_department_list(output["departments"], config)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     if "total" not in output:
         raise ServiceError(
             'Expected to find "total" in the operation output, but it was not present.'
         )
     kwargs["total"] = expect_type(int, output["total"])
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     return ListDepartmentsOutput(**kwargs)
 
 
 async def _deserialize_error_list_departments(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -2910,14 +3123,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_departments_for_filter(
     http_response: HTTPResponse, config: Config
 ) -> ListDepartmentsForFilterOutput:
@@ -2955,14 +3173,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_discovered_recipients(
     http_response: HTTPResponse, config: Config
 ) -> ListDiscoveredRecipientsOutput:
@@ -2971,22 +3194,22 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if (_total := output.get("total")) is not None:
+        kwargs["total"] = expect_type(int, _total)
+
     if (_discovered_recipients := output.get("discoveredRecipients")) is not None:
         kwargs["discovered_recipients"] = _deserialize_discovered_recipient_list(
             _discovered_recipients, config
         )
 
-    if (_total := output.get("total")) is not None:
-        kwargs["total"] = expect_type(int, _total)
-
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
     return ListDiscoveredRecipientsOutput(**kwargs)
 
 
 async def _deserialize_error_list_discovered_recipients(
@@ -3001,14 +3224,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_discovered_recipients_users(
     http_response: HTTPResponse, config: Config
 ) -> ListDiscoveredRecipientsUsersOutput:
@@ -3043,14 +3271,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_domains(
     http_response: HTTPResponse, config: Config
 ) -> ListDomainsOutput:
@@ -3059,20 +3292,20 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_domains := output.get("domains")) is not None:
-        kwargs["domains"] = _deserialize_domain_list(_domains, config)
-
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
+    if (_domains := output.get("domains")) is not None:
+        kwargs["domains"] = _deserialize_domain_list(_domains, config)
+
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
     return ListDomainsOutput(**kwargs)
 
 
 async def _deserialize_error_list_domains(
@@ -3087,14 +3320,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_employees(
     http_response: HTTPResponse, config: Config
 ) -> ListEmployeesOutput:
@@ -3103,29 +3341,29 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if "employees" not in output:
-        raise ServiceError(
-            'Expected to find "employees" in the operation output, but it was not present.'
-        )
-    kwargs["employees"] = _deserialize_employee_list(output["employees"], config)
-
     if "total" not in output:
         raise ServiceError(
             'Expected to find "total" in the operation output, but it was not present.'
         )
     kwargs["total"] = expect_type(int, output["total"])
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if "employees" not in output:
+        raise ServiceError(
+            'Expected to find "employees" in the operation output, but it was not present.'
+        )
+    kwargs["employees"] = _deserialize_employee_list(output["employees"], config)
+
     return ListEmployeesOutput(**kwargs)
 
 
 async def _deserialize_error_list_employees(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3137,14 +3375,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_employees_for_filter(
     http_response: HTTPResponse, config: Config
 ) -> ListEmployeesForFilterOutput:
@@ -3180,14 +3423,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_events(
     http_response: HTTPResponse, config: Config
 ) -> ListEventsOutput:
@@ -3199,20 +3447,20 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_events := output.get("events")) is not None:
         kwargs["events"] = _deserialize_events_list(_events, config)
 
-    if (_total := output.get("total")) is not None:
-        kwargs["total"] = expect_type(int, _total)
-
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if (_total := output.get("total")) is not None:
+        kwargs["total"] = expect_type(int, _total)
+
     return ListEventsOutput(**kwargs)
 
 
 async def _deserialize_error_list_events(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3224,14 +3472,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_headquarters(
     http_response: HTTPResponse, config: Config
 ) -> ListHeadquartersOutput:
@@ -3276,14 +3529,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_infotype_categories(
     http_response: HTTPResponse, config: Config
 ) -> ListInfotypeCategoriesOutput:
@@ -3314,14 +3572,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_inspection_results(
     http_response: HTTPResponse, config: Config
 ) -> ListInspectionResultsOutput:
@@ -3330,25 +3593,25 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_count := output.get("count")) is not None:
-        kwargs["count"] = expect_type(int, _count)
-
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     if (_inspection_results := output.get("inspectionResults")) is not None:
         kwargs["inspection_results"] = _deserialize_inspection_result_list(
             _inspection_results, config
         )
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
+    if (_count := output.get("count")) is not None:
+        kwargs["count"] = expect_type(int, _count)
+
     return ListInspectionResultsOutput(**kwargs)
 
 
 async def _deserialize_error_list_inspection_results(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3360,14 +3623,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_inventory_resources(
     http_response: HTTPResponse, config: Config
 ) -> ListInventoryResourcesOutput:
@@ -3376,23 +3644,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_resources := output.get("resources")) is not None:
-        kwargs["resources"] = _deserialize_resource_inventory_list(_resources, config)
-
     if (_count := output.get("count")) is not None:
         kwargs["count"] = expect_type(int, _count)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if (_resources := output.get("resources")) is not None:
+        kwargs["resources"] = _deserialize_resource_inventory_list(_resources, config)
+
     return ListInventoryResourcesOutput(**kwargs)
 
 
 async def _deserialize_error_list_inventory_resources(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3404,14 +3672,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_inventory_resources_export(
     http_response: HTTPResponse, config: Config
 ) -> ListInventoryResourcesExportOutput:
@@ -3444,14 +3717,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_issues(
     http_response: HTTPResponse, config: Config
 ) -> ListIssuesOutput:
@@ -3463,24 +3741,73 @@
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     if (_issues := output.get("issues")) is not None:
         kwargs["issues"] = _deserialize_issue_list(_issues, config)
 
+    return ListIssuesOutput(**kwargs)
+
+
+async def _deserialize_error_list_issues(
+    http_response: HTTPResponse, config: Config
+) -> ApiError:
+    code, message, parsed_body = await parse_rest_json_error_info(http_response)
+
+    match code.lower():
+        case "unauthorized":
+            return await _deserialize_error_unauthorized(
+                http_response, config, parsed_body, message
+            )
+
+        case "validationexception":
+            return await _deserialize_error_validation_exception(
+                http_response, config, parsed_body, message
+            )
+
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
+        case _:
+            return UnknownApiError(message)
+
+
+async def _deserialize_list_logs(
+    http_response: HTTPResponse, config: Config
+) -> ListLogsOutput:
+    if http_response.status != 200 and http_response.status >= 300:
+        raise await _deserialize_error_list_logs(http_response, config)
+
+    kwargs: dict[str, Any] = {}
+
+    output: dict[str, DocumentValue] = {}
+    if body := await http_response.consume_body_async():
+        output = json.loads(body)
+
+    if (_size := output.get("size")) is not None:
+        kwargs["size"] = expect_type(int, _size)
+
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
-    return ListIssuesOutput(**kwargs)
+    if (_logs := output.get("logs")) is not None:
+        kwargs["logs"] = _deserialize_logs_results(_logs, config)
 
+    return ListLogsOutput(**kwargs)
 
-async def _deserialize_error_list_issues(
+
+async def _deserialize_error_list_logs(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
 
     match code.lower():
         case "unauthorized":
             return await _deserialize_error_unauthorized(
@@ -3488,14 +3815,24 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
+        case "notallowed":
+            return await _deserialize_error_not_allowed(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_processing_activities(
     http_response: HTTPResponse, config: Config
 ) -> ListProcessingActivitiesOutput:
@@ -3504,31 +3841,31 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
+    if "total" not in output:
+        raise ServiceError(
+            'Expected to find "total" in the operation output, but it was not present.'
+        )
+    kwargs["total"] = expect_type(int, output["total"])
+
     if "processingActivities" not in output:
         raise ServiceError(
             'Expected to find "processingActivities" in the operation output, but it was not present.'
         )
     kwargs["processing_activities"] = _deserialize_processing_activity_list(
         output["processingActivities"], config
     )
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
-    if "total" not in output:
-        raise ServiceError(
-            'Expected to find "total" in the operation output, but it was not present.'
-        )
-    kwargs["total"] = expect_type(int, output["total"])
-
     return ListProcessingActivitiesOutput(**kwargs)
 
 
 async def _deserialize_error_list_processing_activities(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3540,14 +3877,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_processing_activities_export(
     http_response: HTTPResponse, config: Config
 ) -> ListProcessingActivitiesExportOutput:
@@ -3580,14 +3922,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_processing_activities_of_recipient(
     http_response: HTTPResponse, config: Config
 ) -> ListProcessingActivitiesOfRecipientOutput:
@@ -3598,28 +3945,28 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
-
     if (
         _processing_activities_of_recipient := output.get(
             "processingActivitiesOfRecipient"
         )
     ) is not None:
         kwargs["processing_activities_of_recipient"] = (
             _deserialize_processing_activity_of_recipient_list(
                 _processing_activities_of_recipient, config
             )
         )
 
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
+
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
     return ListProcessingActivitiesOfRecipientOutput(**kwargs)
 
 
 async def _deserialize_error_list_processing_activities_of_recipient(
@@ -3634,14 +3981,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_processing_activity_filter(
     http_response: HTTPResponse, config: Config
 ) -> ListProcessingActivityFilterOutput:
@@ -3676,14 +4028,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_recipients(
     http_response: HTTPResponse, config: Config
 ) -> ListRecipientsOutput:
@@ -3692,23 +4049,23 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_recipients := output.get("recipients")) is not None:
-        kwargs["recipients"] = _deserialize_recipient_list(_recipients, config)
-
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
+    if (_recipients := output.get("recipients")) is not None:
+        kwargs["recipients"] = _deserialize_recipient_list(_recipients, config)
+
     return ListRecipientsOutput(**kwargs)
 
 
 async def _deserialize_error_list_recipients(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -3720,14 +4077,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_recipients_export(
     http_response: HTTPResponse, config: Config
 ) -> ListRecipientsExportOutput:
@@ -3758,14 +4120,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_recipients_for_filter(
     http_response: HTTPResponse, config: Config
 ) -> ListRecipientsForFilterOutput:
@@ -3798,14 +4165,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_scans(
     http_response: HTTPResponse, config: Config
 ) -> ListScansOutput:
@@ -3842,14 +4214,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_toms(
     http_response: HTTPResponse, config: Config
 ) -> ListTomsOutput:
@@ -3858,22 +4235,22 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
+    if (_toms := output.get("toms")) is not None:
+        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
 
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
-    if (_toms := output.get("toms")) is not None:
-        kwargs["toms"] = _deserialize_tom_collection(_toms, config)
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
 
     return ListTomsOutput(**kwargs)
 
 
 async def _deserialize_error_list_toms(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -3886,14 +4263,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_list_user_profiles(
     http_response: HTTPResponse, config: Config
 ) -> ListUserProfilesOutput:
@@ -3902,22 +4284,22 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_next_token := output.get("nextToken")) is not None:
-        kwargs["next_token"] = expect_type(str, _next_token)
+    if (_user_profiles := output.get("userProfiles")) is not None:
+        kwargs["user_profiles"] = _deserialize_user_profile_list(_user_profiles, config)
 
     if (_total := output.get("total")) is not None:
         kwargs["total"] = expect_type(int, _total)
 
-    if (_user_profiles := output.get("userProfiles")) is not None:
-        kwargs["user_profiles"] = _deserialize_user_profile_list(_user_profiles, config)
+    if (_next_token := output.get("nextToken")) is not None:
+        kwargs["next_token"] = expect_type(str, _next_token)
 
     return ListUserProfilesOutput(**kwargs)
 
 
 async def _deserialize_error_list_user_profiles(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
@@ -3930,14 +4312,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_pause_scan(
     http_response: HTTPResponse, config: Config
 ) -> PauseScanOutput:
@@ -3971,14 +4358,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -4012,14 +4404,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_prepare_detailed_inspection_result(
     http_response: HTTPResponse, config: Config
 ) -> PrepareDetailedInspectionResultOutput:
@@ -4030,20 +4427,20 @@
 
     kwargs: dict[str, Any] = {}
 
     output: dict[str, DocumentValue] = {}
     if body := await http_response.consume_body_async():
         output = json.loads(body)
 
-    if (_url := output.get("url")) is not None:
-        kwargs["url"] = expect_type(str, _url)
-
     if (_success := output.get("success")) is not None:
         kwargs["success"] = expect_type(bool, _success)
 
+    if (_url := output.get("url")) is not None:
+        kwargs["url"] = expect_type(str, _url)
+
     return PrepareDetailedInspectionResultOutput(**kwargs)
 
 
 async def _deserialize_error_prepare_detailed_inspection_result(
     http_response: HTTPResponse, config: Config
 ) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
@@ -4055,14 +4452,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4091,14 +4493,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4137,14 +4544,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4183,14 +4595,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_remove_domain(
     http_response: HTTPResponse, config: Config
 ) -> RemoveDomainOutput:
@@ -4214,14 +4631,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_remove_dpia(
     http_response: HTTPResponse, config: Config
 ) -> RemoveDpiaOutput:
@@ -4245,14 +4667,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_remove_employee(
     http_response: HTTPResponse, config: Config
 ) -> RemoveEmployeeOutput:
@@ -4276,14 +4703,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_remove_headquarter(
     http_response: HTTPResponse, config: Config
 ) -> RemoveHeadquarterOutput:
@@ -4307,14 +4739,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_remove_processing_activity(
     http_response: HTTPResponse, config: Config
 ) -> RemoveProcessingActivityOutput:
@@ -4338,14 +4775,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_remove_recipient(
     http_response: HTTPResponse, config: Config
 ) -> RemoveRecipientOutput:
@@ -4369,14 +4811,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_remove_threshold(
     http_response: HTTPResponse, config: Config
 ) -> RemoveThresholdOutput:
@@ -4400,14 +4847,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_resume_scan(
     http_response: HTTPResponse, config: Config
 ) -> ResumeScanOutput:
@@ -4441,14 +4893,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -4489,14 +4946,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4535,14 +4997,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -4583,14 +5050,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_untag_resources(
     http_response: HTTPResponse, config: Config
 ) -> UntagResourcesOutput:
@@ -4621,14 +5093,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case _:
             return UnknownApiError(message)
 
 
 async def _deserialize_update_asset(
     http_response: HTTPResponse, config: Config
 ) -> UpdateAssetOutput:
@@ -4652,14 +5129,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4698,14 +5180,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4744,14 +5231,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4780,14 +5272,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4816,14 +5313,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -4867,14 +5369,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4903,14 +5410,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4939,14 +5451,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case _:
             return UnknownApiError(message)
@@ -4975,14 +5492,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -5016,14 +5538,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -5057,14 +5584,19 @@
             )
 
         case "validationexception":
             return await _deserialize_error_validation_exception(
                 http_response, config, parsed_body, message
             )
 
+        case "unexpectedservererror":
+            return await _deserialize_error_unexpected_server_error(
+                http_response, config, parsed_body, message
+            )
+
         case "notallowed":
             return await _deserialize_error_not_allowed(
                 http_response, config, parsed_body, message
             )
 
         case "nosuchresource":
             return await _deserialize_error_no_such_resource(
@@ -5134,14 +5666,36 @@
 
     if (_message := output.get("message")) is not None:
         kwargs["message"] = expect_type(str, _message)
 
     return Unauthorized(**kwargs)
 
 
+async def _deserialize_error_unexpected_server_error(
+    http_response: HTTPResponse,
+    config: Config,
+    parsed_body: dict[str, DocumentValue] | None,
+    default_message: str,
+) -> UnexpectedServerError:
+    kwargs: dict[str, Any] = {"message": default_message}
+
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
+        parsed_body = json.loads(body)
+
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
+
+    if "message" not in output:
+        raise ServiceError(
+            'Expected to find "message" in the operation output, but it was not present.'
+        )
+    kwargs["message"] = expect_type(str, output["message"])
+
+    return UnexpectedServerError(**kwargs)
+
+
 async def _deserialize_error_validation_exception(
     http_response: HTTPResponse,
     config: Config,
     parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> ValidationException:
     kwargs: dict[str, Any] = {"message": default_message}
@@ -5535,14 +6089,29 @@
 
     if (_params := output.get("params")) is not None:
         kwargs["params"] = _deserialize_open_properties(_params, config)
 
     if (_resource_account_id := output.get("resourceAccountId")) is not None:
         kwargs["resource_account_id"] = expect_type(str, _resource_account_id)
 
+    if (
+        _next_meta_data_sync_schedule := output.get("nextMetaDataSyncSchedule")
+    ) is not None:
+        kwargs["next_meta_data_sync_schedule"] = epoch_seconds_to_datetime(
+            expect_type(int | float, _next_meta_data_sync_schedule)
+        )
+
+    if (_is_meta_data_sync_running := output.get("isMetaDataSyncRunning")) is not None:
+        kwargs["is_meta_data_sync_running"] = expect_type(
+            bool, _is_meta_data_sync_running
+        )
+
+    if (_meta_data_sync_interval := output.get("metaDataSyncInterval")) is not None:
+        kwargs["meta_data_sync_interval"] = expect_type(str, _meta_data_sync_interval)
+
     return ConnectorListMember(**kwargs)
 
 
 def _deserialize_connectors_list(
     output: DocumentValue, config: Config
 ) -> list[ConnectorListMember]:
     if not isinstance(output, list):
@@ -7006,14 +7575,47 @@
 
     if (_name := output.get("name")) is not None:
         kwargs["name"] = expect_type(str, _name)
 
     return ListProcessingActivityFilterMember(**kwargs)
 
 
+def _deserialize_log_member(output: DocumentValue, config: Config) -> LogMember:
+    if not isinstance(output, dict):
+        raise ServiceError(f"Expected dict, found {type(output)}")
+
+    kwargs: dict[str, Any] = {}
+
+    if (_time := output.get("time")) is not None:
+        kwargs["time"] = expect_type(str, _time)
+
+    if (_email := output.get("email")) is not None:
+        kwargs["email"] = expect_type(str, _email)
+
+    if (_request_id := output.get("requestId")) is not None:
+        kwargs["request_id"] = expect_type(str, _request_id)
+
+    if (_roles := output.get("roles")) is not None:
+        kwargs["roles"] = _deserialize_unique_string_list(_roles, config)
+
+    if (_operation := output.get("operation")) is not None:
+        kwargs["operation"] = expect_type(str, _operation)
+
+    if (_msg := output.get("msg")) is not None:
+        kwargs["msg"] = expect_type(str, _msg)
+
+    return LogMember(**kwargs)
+
+
+def _deserialize_logs_results(output: DocumentValue, config: Config) -> list[LogMember]:
+    if not isinstance(output, list):
+        raise ServiceError(f"Expected list, found {type(output)}")
+    return [_deserialize_log_member(e, config) for e in output]
+
+
 def _deserialize_management_method(
     output: DocumentValue, config: Config
 ) -> ManagementMethod:
     if not isinstance(output, dict):
         raise ServiceError(f"Expected dict, found {type(output)}")
 
     kwargs: dict[str, Any] = {}
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client/errors.py` & `borneo_python_client-3.10.1/borneo_python_client/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,32 @@
     code: ClassVar[str] = "Unauthorized"
     fault: ClassVar[Literal["client", "server"]] = "client"
 
     message: str
 
 
 @dataclass(kw_only=True)
+class UnexpectedServerError(ApiError):
+    """The operation has error out due to unexpected reasons.
+
+    This could be due to the
+    current state of the resource, or one of the
+    request parameters of the operation
+    or missing permission.
+    :param message: A message associated with the specific error.
+
+    """
+
+    code: ClassVar[str] = "UnexpectedServerError"
+    fault: ClassVar[Literal["client", "server"]] = "server"
+
+    message: str
+
+
+@dataclass(kw_only=True)
 class ValidationException(ApiError):
     """A standard error for input validation failures.
     This should be thrown by
     services when a member of the input structure
     falls outside of the modeled or
     documented constraints.
     :param message: A message associated with the specific error.
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client/models.py` & `borneo_python_client-3.10.1/borneo_python_client/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -923,14 +923,33 @@
     PENDING = "pending"
     AVAILABLE = "available"
     DESTROYING = "destroying"
     DESTROYED = "destroyed"
     UNAVAILABLE = "unavailable"
 
 
+class CronValues(StrEnum):
+    """The cron schedule expression to use for a recurring scan. Only a fixed set
+    of
+    cron expressions
+    can be used to run scans at 30 minute, 1 hour, 1 day, or 1
+    week
+    intervals.
+    """
+
+    EVERY_30_MIN = "*/30 * * * *"
+    EVERY_1_HOUR = "0 */1 * * *"
+    EVERY_4_HOUR = "0 */4 * * *"
+    EVERY_6_HOUR = "0 */6 * * *"
+    EVERY_8_HOUR = "0 */8 * * *"
+    EVERY_12_HOUR = "0 */12 * * *"
+    EVERY_1_DAY = "0 0 * * *"
+    EVERY_1_WEEK = "0 0 * * 0"
+
+
 @dataclass(kw_only=True)
 class DescribeConnectorInput:
     """
     :param connector_id: The unique Borneo connector ID.
     """
 
     connector_id: str | None = None
@@ -955,14 +974,17 @@
     time.
     :param updated_at: The time at which the connector was last updated, in Unix
     epoch time.
     :param resource_account_id: For S3 and DynamoDB connectors, this is the cloud
     provider specific
     account ID of the data sources that the connector is
     configured to scan.
+    :param next_meta_data_sync_schedule: Specifies the next metasync schedule
+    :param is_meta_data_sync_running: True if the meta sync is running currently
+    :param meta_data_sync_interval: Specifies the metasync interval
     """
 
     connector_id: str
 
     name: str | None = None
     state: str | None = None
     data_plane_id: str | None = None
@@ -970,14 +992,17 @@
     connector_type: str | None = None
     resource_id: str | None = None
     region: str | None = None
     created_at: datetime | None = None
     updated_at: datetime | None = None
     params: dict[str, Document] | None = None
     resource_account_id: str | None = None
+    next_meta_data_sync_schedule: datetime | None = None
+    is_meta_data_sync_running: bool | None = None
+    meta_data_sync_interval: str | None = None
 
 
 @dataclass(kw_only=True)
 class ConnectorFilter:
     """
     :param names: Filter based on connector name.
     :param states: Filter based on connector state.
@@ -1035,14 +1060,17 @@
     time.
     :param updated_at: The time at which the connector was last updated, in Unix
     epoch time.
     :param resource_account_id: For S3 and DynamoDB connectors, this is the cloud
     provider specific
     account ID of the data sources that the connector is
     configured to scan.
+    :param next_meta_data_sync_schedule: Specifies the next metasync schedule
+    :param is_meta_data_sync_running: True if the meta sync is running currently
+    :param meta_data_sync_interval: Specifies the metasync interval
     """
 
     connector_id: str
 
     name: str | None = None
     state: str | None = None
     data_plane_id: str | None = None
@@ -1050,14 +1078,17 @@
     connector_type: str | None = None
     resource_id: str | None = None
     region: str | None = None
     created_at: datetime | None = None
     updated_at: datetime | None = None
     params: dict[str, Document] | None = None
     resource_account_id: str | None = None
+    next_meta_data_sync_schedule: datetime | None = None
+    is_meta_data_sync_running: bool | None = None
+    meta_data_sync_interval: str | None = None
 
 
 @dataclass(kw_only=True)
 class ListConnectorsOutput:
     """
     :param connectors: The list of connectors matching the filter conditions, up to
     the specified page size.
@@ -3264,14 +3295,92 @@
     """
 
     issues: list[IssueRecord] | None = None
     total: int | None = None
     next_token: str | None = None
 
 
+class LogType(StrEnum):
+    API = "API"
+
+
+@dataclass(kw_only=True)
+class ListLogsFilter:
+    """Filters resources based on the specified filter criteria.
+
+    :param search: Free-text search on the logs.
+    :param log_type: Filter logs based on type of service logs eg. "API".
+    :param email: Filters all logs with user email eg. "user@example.com".
+    :param operation_name: List logs based on operation type eg. "ListConnectors",
+    "CreateOktaConnection".
+    :param request_id: List logs from a specific requestId eg.
+    "clvuywyoq009407rj61sxcrpc"
+    :param start: List logs starting in between a specific timestamps with
+    nonoseconds eg. 1715076388657800827.
+    :param end: List logs ending in between a specific timestamps with nonoseconds
+    eg. 1715076399359944184.
+    """
+
+    search: str | None = None
+    log_type: str = "API"
+    email: str | None = None
+    operation_name: str | None = None
+    request_id: str | None = None
+    start: str | None = None
+    end: str | None = None
+
+
+@dataclass(kw_only=True)
+class ListLogsInput:
+    """
+    :param filter: Filters resources based on the specified filter criteria.
+    :param page_size: The maximum number of logs to return per API call.
+    :param next_token: The `nextToken` from the last page of results to retrieve the
+    next page of results.
+    """
+
+    filter: ListLogsFilter | None = None
+    page_size: int | None = None
+    next_token: str | None = None
+
+
+@dataclass(kw_only=True)
+class LogMember:
+    """
+    :param time: This time will be a 13 digit timestamp.
+    :param email: Email of the user.
+    :param request_id: A unique request ID.
+    :param roles: List of role the user has while logging the request.
+    :param operation: Smithy operation name for thr request.
+    :param msg: Message logged.
+    """
+
+    time: str | None = None
+    email: str | None = None
+    request_id: str | None = None
+    roles: list[str] | None = None
+    operation: str | None = None
+    msg: str | None = None
+
+
+@dataclass(kw_only=True)
+class ListLogsOutput:
+    """
+    :param logs: The list of all logs matching the filters.
+    :param size: Size of logs fetched.
+    :param next_token: A token that can used in a subsequent API request to retrieve
+    the next
+    set of records.
+    """
+
+    logs: list[LogMember] | None = None
+    size: int | None = None
+    next_token: str | None = None
+
+
 class CompanyRole(StrEnum):
     """Role of the company for a processing activity"""
 
     CONTROLLER = "controller"
     PROCESSOR = "processor"
     JOINT_CONTROLLER = "joint_controller"
     SUB_PROCESSOR = "sub_processor"
@@ -4699,29 +4808,14 @@
 
 @dataclass(kw_only=True)
 class UntagResourcesOutput:
 
     results: list[TaggingResult] | None = None
 
 
-class CronValues(StrEnum):
-    """The cron schedule expression to use for a recurring scan. Only a fixed set
-    of
-    cron expressions
-    can be used to run scans at 30 minute, 1 hour, 1 day, or 1
-    week
-    intervals.
-    """
-
-    EVERY_30_MIN = "*/30 * * * *"
-    EVERY_1_HOUR = "0 */1 * * *"
-    EVERY_1_DAY = "0 0 * * *"
-    EVERY_1_WEEK = "0 0 * * 0"
-
-
 @dataclass(kw_only=True)
 class ScanLimits:
     """Scan limits specify the maximum amount of data to scan per resource.
 
     :param sample_percentage: Percentage of data to scan per resource. Supported for
     full scans on the following resource
     types: S3, BigQuery.
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client/serialize.py` & `borneo_python_client-3.10.1/borneo_python_client/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,16 @@
     ListEventsInput,
     ListHeadquartersInput,
     ListInfotypeCategoriesInput,
     ListInspectionResultsInput,
     ListInventoryResourcesExportInput,
     ListInventoryResourcesInput,
     ListIssuesInput,
+    ListLogsFilter,
+    ListLogsInput,
     ListProcessingActivitiesExportInput,
     ListProcessingActivitiesInput,
     ListProcessingActivitiesOfRecipientInput,
     ListProcessingActivityFilterInput,
     ListRecipientsExportInput,
     ListRecipientsForFilterInput,
     ListRecipientsInput,
@@ -235,26 +237,26 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.type is not None:
         result["type"] = input.type
 
-    if input.name is not None:
-        result["name"] = input.name
-
     if input.tom_ids is not None:
         result["tomIds"] = input.tom_ids
 
-    if input.location_id is not None:
-        result["locationId"] = input.location_id
-
     if input.location_type is not None:
         result["locationType"] = input.location_type
 
+    if input.name is not None:
+        result["name"] = input.name
+
+    if input.location_id is not None:
+        result["locationId"] = input.location_id
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -280,23 +282,23 @@
 ) -> HTTPRequest:
     path = "/categories"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.category_label is not None:
+        result["categoryLabel"] = input.category_label
+
     if input.infotypes is not None:
         result["infotypes"] = input.infotypes
 
     if input.description is not None:
         result["description"] = input.description
 
-    if input.category_label is not None:
-        result["categoryLabel"] = input.category_label
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -395,44 +397,44 @@
 async def _serialize_create_dpia(input: CreateDpiaInput, config: Config) -> HTTPRequest:
     path = "/dpias"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.processing_activity_id is not None:
+        result["processingActivityId"] = input.processing_activity_id
+
     if input.privacy_framework is not None:
         result["privacyFramework"] = _serialize_dpia_privacy_framework(
             input.privacy_framework, config
         )
 
-    if input.status is not None:
-        result["status"] = input.status
-
-    if input.processing_activity_id is not None:
-        result["processingActivityId"] = input.processing_activity_id
-
     if input.integrity is not None:
         result["integrity"] = _serialize_dpia_integrity_risk(input.integrity, config)
 
-    if input.additional_information_files is not None:
-        result["additionalInformationFiles"] = input.additional_information_files
-
     if input.availability is not None:
         result["availability"] = _serialize_dpia_availability_risk(
             input.availability, config
         )
 
     if input.additional_information is not None:
         result["additionalInformation"] = input.additional_information
 
+    if input.status is not None:
+        result["status"] = input.status
+
     if input.confidentiality is not None:
         result["confidentiality"] = _serialize_dpia_confidentiality_risk(
             input.confidentiality, config
         )
 
+    if input.additional_information_files is not None:
+        result["additionalInformationFiles"] = input.additional_information_files
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -458,47 +460,47 @@
 ) -> HTTPRequest:
     path = "/employees"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.nif is not None:
-        result["nif"] = input.nif
-
-    if input.email is not None:
-        result["email"] = input.email
-
-    if input.position is not None:
-        result["position"] = input.position
+    if input.end_date is not None:
+        result["endDate"] = input.end_date
 
     if input.reference_id is not None:
         result["referenceId"] = input.reference_id
 
+    if input.surname is not None:
+        result["surname"] = input.surname
+
     if input.name is not None:
         result["name"] = input.name
 
-    if input.department is not None:
-        result["department"] = input.department
-
     if input.start_date is not None:
         result["startDate"] = input.start_date
 
-    if input.surname is not None:
-        result["surname"] = input.surname
+    if input.email is not None:
+        result["email"] = input.email
 
-    if input.end_date is not None:
-        result["endDate"] = input.end_date
+    if input.position is not None:
+        result["position"] = input.position
+
+    if input.nif is not None:
+        result["nif"] = input.nif
 
     if input.created_by is not None:
         result["createdBy"] = input.created_by
 
     if input.manager is not None:
         result["manager"] = input.manager
 
+    if input.department is not None:
+        result["department"] = input.department
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -524,32 +526,32 @@
 ) -> HTTPRequest:
     path = "/headquarters"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.zipcode is not None:
-        result["zipcode"] = input.zipcode
-
     if input.tom_ids is not None:
         result["tomIds"] = input.tom_ids
 
     if input.name is not None:
         result["name"] = input.name
 
-    if input.city is not None:
-        result["city"] = input.city
-
     if input.address is not None:
         result["address"] = input.address
 
     if input.country is not None:
         result["country"] = input.country
 
+    if input.zipcode is not None:
+        result["zipcode"] = input.zipcode
+
+    if input.city is not None:
+        result["city"] = input.city
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -575,96 +577,96 @@
 ) -> HTTPRequest:
     path = "/processing-activities"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.assets is not None:
-        result["assets"] = input.assets
-
     if input.processing_frequency is not None:
         result["processingFrequency"] = input.processing_frequency
 
-    if input.data_types is not None:
-        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
-
     if input.lawful_basis is not None:
         result["lawfulBasis"] = _serialize_lawful_basis_collection(
             input.lawful_basis, config
         )
 
-    if input.is_data_stored is not None:
-        result["isDataStored"] = input.is_data_stored
-
     if input.infotypes is not None:
         result["infotypes"] = input.infotypes
 
-    if input.data_sources is not None:
-        result["dataSources"] = input.data_sources
+    if input.data_types is not None:
+        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
 
-    if input.recipients is not None:
-        result["recipients"] = _serialize_recipient_collection(input.recipients, config)
+    if input.are_access_requests_managed is not None:
+        result["areAccessRequestsManaged"] = input.are_access_requests_managed
 
-    if input.processing_frequency_comment is not None:
-        result["processingFrequencyComment"] = input.processing_frequency_comment
+    if input.contact_person is not None:
+        result["contactPerson"] = input.contact_person
+
+    if input.assets is not None:
+        result["assets"] = input.assets
+
+    if input.additional_info_files is not None:
+        result["additionalInfoFiles"] = input.additional_info_files
 
     if input.infotype_volume is not None:
         result["infotypeVolume"] = input.infotype_volume
 
     if input.management_methods is not None:
         result["managementMethods"] = _serialize_management_method_collection(
             input.management_methods, config
         )
 
+    if input.departments is not None:
+        result["departments"] = input.departments
+
     if input.retention_period is not None:
         result["retentionPeriod"] = _serialize_retention_period(
             input.retention_period, config
         )
 
-    if input.additional_info_files is not None:
-        result["additionalInfoFiles"] = input.additional_info_files
-
-    if input.departments is not None:
-        result["departments"] = input.departments
+    if input.data_sources is not None:
+        result["dataSources"] = input.data_sources
 
-    if input.are_access_requests_managed is not None:
-        result["areAccessRequestsManaged"] = input.are_access_requests_managed
+    if input.additional_info is not None:
+        result["additionalInfo"] = input.additional_info
 
     if input.infotype_categories is not None:
         result["infotypeCategories"] = input.infotype_categories
 
+    if input.active is not None:
+        result["active"] = input.active
+
     if input.data_subjects is not None:
         result["dataSubjects"] = _serialize_data_subject_collection(
             input.data_subjects, config
         )
 
     if input.name is not None:
         result["name"] = input.name
 
-    if input.additional_info is not None:
-        result["additionalInfo"] = input.additional_info
-
-    if input.model_id is not None:
-        result["modelId"] = input.model_id
-
     if input.purpose is not None:
         result["purpose"] = input.purpose
 
-    if input.company_role is not None:
-        result["companyRole"] = input.company_role
-
     if input.retention_period_comment is not None:
         result["retentionPeriodComment"] = input.retention_period_comment
 
-    if input.contact_person is not None:
-        result["contactPerson"] = input.contact_person
+    if input.processing_frequency_comment is not None:
+        result["processingFrequencyComment"] = input.processing_frequency_comment
 
-    if input.active is not None:
-        result["active"] = input.active
+    if input.recipients is not None:
+        result["recipients"] = _serialize_recipient_collection(input.recipients, config)
+
+    if input.is_data_stored is not None:
+        result["isDataStored"] = input.is_data_stored
+
+    if input.company_role is not None:
+        result["companyRole"] = input.company_role
+
+    if input.model_id is not None:
+        result["modelId"] = input.model_id
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -691,56 +693,56 @@
 ) -> HTTPRequest:
     path = "/recipients"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.category is not None:
-        result["category"] = input.category
-
-    if input.dpa is not None:
-        result["dpa"] = input.dpa
+    if input.country is not None:
+        result["country"] = input.country
 
     if input.dpa_status is not None:
         result["dpaStatus"] = input.dpa_status
 
     if input.dpa_files is not None:
         result["dpaFiles"] = input.dpa_files
 
+    if input.category is not None:
+        result["category"] = input.category
+
+    if input.business_name is not None:
+        result["businessName"] = input.business_name
+
+    if input.data_storage_location is not None:
+        result["dataStorageLocation"] = input.data_storage_location
+
+    if input.role is not None:
+        result["role"] = input.role
+
     if input.status is not None:
         result["status"] = input.status
 
-    if input.from_discovered_recipient_id is not None:
-        result["fromDiscoveredRecipientId"] = input.from_discovered_recipient_id
-
     if input.state is not None:
         result["state"] = input.state
 
+    if input.from_discovered_recipient_id is not None:
+        result["fromDiscoveredRecipientId"] = input.from_discovered_recipient_id
+
     if input.name is not None:
         result["name"] = input.name
 
+    if input.dpa is not None:
+        result["dpa"] = input.dpa
+
     if input.recipient_warranties is not None:
         result["recipientWarranties"] = input.recipient_warranties
 
     if input.recipient_model_id is not None:
         result["recipientModelId"] = input.recipient_model_id
 
-    if input.data_storage_location is not None:
-        result["dataStorageLocation"] = input.data_storage_location
-
-    if input.role is not None:
-        result["role"] = input.role
-
-    if input.business_name is not None:
-        result["businessName"] = input.business_name
-
-    if input.country is not None:
-        result["country"] = input.country
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -764,49 +766,49 @@
 async def _serialize_create_scan(input: CreateScanInput, config: Config) -> HTTPRequest:
     path = "/scan"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.scan_limits is not None:
-        result["scanLimits"] = _serialize_scan_limits(input.scan_limits, config)
+    if input.resources is not None:
+        result["resources"] = _serialize_scan_resources(input.resources, config)
+
+    if input.scan_type is not None:
+        result["scanType"] = input.scan_type
 
     if input.name is not None:
         result["name"] = input.name
 
-    if input.scan_filter is not None:
-        result["scanFilter"] = _serialize_scan_filter_list(input.scan_filter, config)
-
     if input.resource_type is not None:
         result["resourceType"] = input.resource_type
 
-    if input.scan_type is not None:
-        result["scanType"] = input.scan_type
-
-    if input.resources is not None:
-        result["resources"] = _serialize_scan_resources(input.resources, config)
-
-    if input.schedule_type is not None:
-        result["scheduleType"] = input.schedule_type
+    if input.schedule is not None:
+        result["schedule"] = _serialize_scan_schedule(input.schedule, config)
 
     if input.cron is not None:
         result["cron"] = input.cron
 
-    if input.connector_id is not None:
-        result["connectorId"] = input.connector_id
-
-    if input.schedule is not None:
-        result["schedule"] = _serialize_scan_schedule(input.schedule, config)
-
     if input.inspection_policy is not None:
         result["inspectionPolicy"] = _serialize_inspection_policy(
             input.inspection_policy, config
         )
 
+    if input.scan_limits is not None:
+        result["scanLimits"] = _serialize_scan_limits(input.scan_limits, config)
+
+    if input.scan_filter is not None:
+        result["scanFilter"] = _serialize_scan_filter_list(input.scan_filter, config)
+
+    if input.connector_id is not None:
+        result["connectorId"] = input.connector_id
+
+    if input.schedule_type is not None:
+        result["scheduleType"] = input.schedule_type
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -832,52 +834,50 @@
 ) -> HTTPRequest:
     path = "/thresholds"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.large_scale_processing_sensitive_data is not None:
-        result["largeScaleProcessingSensitiveData"] = (
-            input.large_scale_processing_sensitive_data
-        )
-
-    if input.systematic_monitoring_data_subject is not None:
-        result["systematicMonitoringDataSubject"] = (
-            input.systematic_monitoring_data_subject
-        )
+    if input.large_scale_data_processing is not None:
+        result["largeScaleDataProcessing"] = input.large_scale_data_processing
 
     if input.prevent_data_subjects_exercising_their_rights is not None:
         result["preventDataSubjectsExercisingTheirRights"] = (
             input.prevent_data_subjects_exercising_their_rights
         )
 
-    if input.large_scale_data_processing is not None:
-        result["largeScaleDataProcessing"] = input.large_scale_data_processing
-
     if input.classifying_data_subject is not None:
         result["classifyingDataSubject"] = input.classifying_data_subject
 
-    if input.processing_vulnerable_data_subject is not None:
-        result["processingVulnerableDataSubject"] = (
-            input.processing_vulnerable_data_subject
+    if input.matching_merging_records_involved is not None:
+        result["matchingMergingRecordsInvolved"] = (
+            input.matching_merging_records_involved
         )
 
-    if input.comment is not None:
-        result["comment"] = input.comment
+    if input.processing_activity_id is not None:
+        result["processingActivityId"] = input.processing_activity_id
+
+    if input.large_scale_processing_sensitive_data is not None:
+        result["largeScaleProcessingSensitiveData"] = (
+            input.large_scale_processing_sensitive_data
+        )
+
+    if input.systematic_monitoring_data_subject is not None:
+        result["systematicMonitoringDataSubject"] = (
+            input.systematic_monitoring_data_subject
+        )
 
     if input.processing_confidential_sensitive_data is not None:
         result["processingConfidentialSensitiveData"] = (
             input.processing_confidential_sensitive_data
         )
 
-    if input.matching_merging_records_involved is not None:
-        result["matchingMergingRecordsInvolved"] = (
-            input.matching_merging_records_involved
-        )
+    if input.automated_decision_making is not None:
+        result["automatedDecisionMaking"] = input.automated_decision_making
 
     if input.extensive_automated_evaluation_characteristics is not None:
         result["extensiveAutomatedEvaluationCharacteristics"] = (
             input.extensive_automated_evaluation_characteristics
         )
 
     if input.innovative_technologies_used is not None:
@@ -890,19 +890,21 @@
 
     if input.blacklist is not None:
         result["blacklist"] = input.blacklist
 
     if input.status is not None:
         result["status"] = input.status
 
-    if input.processing_activity_id is not None:
-        result["processingActivityId"] = input.processing_activity_id
+    if input.processing_vulnerable_data_subject is not None:
+        result["processingVulnerableDataSubject"] = (
+            input.processing_vulnerable_data_subject
+        )
 
-    if input.automated_decision_making is not None:
-        result["automatedDecisionMaking"] = input.automated_decision_making
+    if input.comment is not None:
+        result["comment"] = input.comment
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -1500,26 +1502,26 @@
 ) -> HTTPRequest:
     path = "/accounts"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.filter is not None:
-        result["filter"] = _serialize_account_filter(input.filter, config)
-
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
+    if input.filter is not None:
+        result["filter"] = _serialize_account_filter(input.filter, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -1590,26 +1592,26 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.filter is not None:
         result["filter"] = _serialize_leaf_resource_filter(input.filter, config)
 
-    if input.source_type is not None:
-        result["sourceType"] = input.source_type
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.source_type is not None:
+        result["sourceType"] = input.source_type
+
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -1635,23 +1637,23 @@
 ) -> HTTPRequest:
     path = "/resource/catalog/listLeafResources/export"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.source_type is not None:
-        result["sourceType"] = input.source_type
-
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.filter is not None:
         result["filter"] = _serialize_leaf_resource_filter(input.filter, config)
 
+    if input.source_type is not None:
+        result["sourceType"] = input.source_type
+
     if input.detailed is not None:
         result["detailed"] = input.detailed
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -1683,22 +1685,22 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.filter is not None:
         result["filter"] = _serialize_connector_filter(input.filter, config)
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
+    if input.page_size is not None:
+        result["pageSize"] = input.page_size
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.page_size is not None:
-        result["pageSize"] = input.page_size
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -1725,23 +1727,23 @@
 ) -> HTTPRequest:
     path = "/departments/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.filter is not None:
-        result["filter"] = _serialize_department_select_filter(input.filter, config)
-
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.filter is not None:
+        result["filter"] = _serialize_department_select_filter(input.filter, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -1789,25 +1791,25 @@
 ) -> HTTPRequest:
     path = "/discovered-recipients/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.filter is not None:
         result["filter"] = _serialize_discovered_recipient_filters(input.filter, config)
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -1864,20 +1866,20 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -1967,28 +1969,28 @@
 async def _serialize_list_events(input: ListEventsInput, config: Config) -> HTTPRequest:
     path = "/events/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.select is not None:
-        result["select"] = input.select
+    if input.filter is not None:
+        result["filter"] = _serialize_events_filter(input.filter, config)
 
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.filter is not None:
-        result["filter"] = _serialize_events_filter(input.filter, config)
+    if input.select is not None:
+        result["select"] = input.select
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -2090,26 +2092,26 @@
 ) -> HTTPRequest:
     path = "/insight/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.type is not None:
         result["type"] = input.type
 
     if input.filter is not None:
         result["filter"] = _serialize_inspection_result_filter(input.filter, config)
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -2138,29 +2140,29 @@
 ) -> HTTPRequest:
     path = "/resource/inventory/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.page_size is not None:
+        result["pageSize"] = input.page_size
+
     if input.filter is not None:
         result["filter"] = _serialize_inventory_list_filter(input.filter, config)
 
+    if input.select is not None:
+        result["select"] = input.select
+
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.select is not None:
-        result["select"] = input.select
-
-    if input.page_size is not None:
-        result["pageSize"] = input.page_size
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2186,28 +2188,28 @@
 ) -> HTTPRequest:
     path = "/resource/inventory/list/export"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.filter is not None:
-        result["filter"] = _serialize_inventory_list_filter(input.filter, config)
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.select is not None:
         result["select"] = input.select
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
+    if input.filter is not None:
+        result["filter"] = _serialize_inventory_list_filter(input.filter, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -2232,26 +2234,26 @@
 async def _serialize_list_issues(input: ListIssuesInput, config: Config) -> HTTPRequest:
     path = "/issue/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.filter is not None:
-        result["filter"] = _serialize_issue_filter(input.filter, config)
-
-    if input.include is not None:
-        result["include"] = input.include
-
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
+    if input.include is not None:
+        result["include"] = input.include
+
+    if input.filter is not None:
+        result["filter"] = _serialize_issue_filter(input.filter, config)
+
     if input.select is not None:
         result["select"] = input.select
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
     content = json.dumps(result).encode("utf-8")
@@ -2274,37 +2276,77 @@
         ),
         method="POST",
         fields=headers,
         body=body,
     )
 
 
+async def _serialize_list_logs(input: ListLogsInput, config: Config) -> HTTPRequest:
+    path = "/logs"
+    query: str = f""
+
+    body: AsyncIterable[bytes] = AsyncBytesReader(b"")
+    result: dict[str, DocumentValue] = {}
+
+    if input.filter is not None:
+        result["filter"] = _serialize_list_logs_filter(input.filter, config)
+
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
+    if input.page_size is not None:
+        result["pageSize"] = input.page_size
+
+    content = json.dumps(result).encode("utf-8")
+    content_length = len(content)
+    body = AsyncBytesReader(content)
+
+    headers = Fields(
+        [
+            Field(name="Content-Type", values=["application/json"]),
+            Field(name="Content-Length", values=[str(content_length)]),
+        ]
+    )
+
+    return _HTTPRequest(
+        destination=_URI(
+            host="",
+            path=path,
+            scheme="https",
+            query=query,
+        ),
+        method="POST",
+        fields=headers,
+        body=body,
+    )
+
+
 async def _serialize_list_processing_activities(
     input: ListProcessingActivitiesInput, config: Config
 ) -> HTTPRequest:
     path = "/processing-activities/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
     if input.filter is not None:
         result["filter"] = _serialize_processing_activity_select_filter(
             input.filter, config
         )
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2330,22 +2372,22 @@
 ) -> HTTPRequest:
     path = "/processing-activities/list/export"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.export_types is not None:
+        result["exportTypes"] = input.export_types
+
     if input.filter is not None:
         result["filter"] = _serialize_processing_activity_export_filters(
             input.filter, config
         )
 
-    if input.export_types is not None:
-        result["exportTypes"] = input.export_types
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2376,20 +2418,20 @@
         recipient_id=urlquote(input.recipient_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.page_size is not None:
-        result["pageSize"] = input.page_size
-
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
+    if input.page_size is not None:
+        result["pageSize"] = input.page_size
+
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
@@ -2454,22 +2496,22 @@
 ) -> HTTPRequest:
     path = "/recipients/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.page_size is not None:
-        result["pageSize"] = input.page_size
+    if input.filter is not None:
+        result["filter"] = _serialize_recipient_filters(input.filter, config)
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.filter is not None:
-        result["filter"] = _serialize_recipient_filters(input.filter, config)
+    if input.page_size is not None:
+        result["pageSize"] = input.page_size
 
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
@@ -2555,32 +2597,32 @@
 async def _serialize_list_scans(input: ListScansInput, config: Config) -> HTTPRequest:
     path = "/scan/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.get_next_execution is not None:
-        result["getNextExecution"] = input.get_next_execution
-
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
-    if input.filter is not None:
-        result["filter"] = _serialize_scan_select_filter(input.filter, config)
+    if input.get_next_execution is not None:
+        result["getNextExecution"] = input.get_next_execution
 
     if input.select is not None:
         result["select"] = input.select
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
+    if input.filter is not None:
+        result["filter"] = _serialize_scan_select_filter(input.filter, config)
+
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2604,26 +2646,26 @@
 async def _serialize_list_toms(input: ListTomsInput, config: Config) -> HTTPRequest:
     path = "/toms/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.page_size is not None:
+        result["pageSize"] = input.page_size
+
     if input.filter is not None:
         result["filter"] = _serialize_tom_select_filter(input.filter, config)
 
     if input.sort is not None:
         result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.next_token is not None:
         result["nextToken"] = input.next_token
 
-    if input.page_size is not None:
-        result["pageSize"] = input.page_size
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -2649,28 +2691,28 @@
 ) -> HTTPRequest:
     path = "/user/profile/list"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.filter is not None:
-        result["filter"] = _serialize_user_profile_filter(input.filter, config)
+    if input.sort is not None:
+        result["sort"] = _serialize_sort_records(input.sort, config)
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     if input.select is not None:
         result["select"] = input.select
 
-    if input.sort is not None:
-        result["sort"] = _serialize_sort_records(input.sort, config)
-
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
+    if input.filter is not None:
+        result["filter"] = _serialize_user_profile_filter(input.filter, config)
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3158,25 +3200,25 @@
 ) -> HTTPRequest:
     path = "/resource/tags"
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.tag_value is not None:
-        result["tagValue"] = input.tag_value
-
     if input.tag_resources is not None:
         result["tagResources"] = _serialize_tag_resource_union(
             input.tag_resources, config
         )
 
     if input.tag_key is not None:
         result["tagKey"] = input.tag_key
 
+    if input.tag_value is not None:
+        result["tagValue"] = input.tag_value
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3207,29 +3249,29 @@
         asset_id=urlquote(input.asset_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.location_id is not None:
-        result["locationId"] = input.location_id
-
     if input.name is not None:
         result["name"] = input.name
 
+    if input.type is not None:
+        result["type"] = input.type
+
+    if input.location_id is not None:
+        result["locationId"] = input.location_id
+
     if input.location_type is not None:
         result["locationType"] = input.location_type
 
     if input.tom_ids is not None:
         result["tomIds"] = input.tom_ids
 
-    if input.type is not None:
-        result["type"] = input.type
-
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3260,20 +3302,20 @@
         category_label=urlquote(input.category_label, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.description is not None:
-        result["description"] = input.description
-
     if input.infotypes is not None:
         result["infotypes"] = input.infotypes
 
+    if input.description is not None:
+        result["description"] = input.description
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3345,20 +3387,20 @@
         domain_id=urlquote(input.domain_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.frequency is not None:
-        result["frequency"] = input.frequency
-
     if input.name is not None:
         result["name"] = input.name
 
+    if input.frequency is not None:
+        result["frequency"] = input.frequency
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3387,41 +3429,41 @@
         dpia_id=urlquote(input.dpia_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
+    if input.confidentiality is not None:
+        result["confidentiality"] = _serialize_dpia_confidentiality_risk(
+            input.confidentiality, config
+        )
+
     if input.additional_information is not None:
         result["additionalInformation"] = input.additional_information
 
-    if input.additional_information_files is not None:
-        result["additionalInformationFiles"] = input.additional_information_files
-
-    if input.privacy_framework is not None:
-        result["privacyFramework"] = _serialize_dpia_privacy_framework(
-            input.privacy_framework, config
-        )
-
     if input.status is not None:
         result["status"] = input.status
 
     if input.integrity is not None:
         result["integrity"] = _serialize_dpia_integrity_risk(input.integrity, config)
 
     if input.availability is not None:
         result["availability"] = _serialize_dpia_availability_risk(
             input.availability, config
         )
 
-    if input.confidentiality is not None:
-        result["confidentiality"] = _serialize_dpia_confidentiality_risk(
-            input.confidentiality, config
+    if input.privacy_framework is not None:
+        result["privacyFramework"] = _serialize_dpia_privacy_framework(
+            input.privacy_framework, config
         )
 
+    if input.additional_information_files is not None:
+        result["additionalInformationFiles"] = input.additional_information_files
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3452,40 +3494,40 @@
         employee_id=urlquote(input.employee_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.name is not None:
-        result["name"] = input.name
-
     if input.email is not None:
         result["email"] = input.email
 
-    if input.department is not None:
-        result["department"] = input.department
-
-    if input.start_date is not None:
-        result["startDate"] = input.start_date
+    if input.end_date is not None:
+        result["endDate"] = input.end_date
 
     if input.nif is not None:
         result["nif"] = input.nif
 
     if input.position is not None:
         result["position"] = input.position
 
     if input.surname is not None:
         result["surname"] = input.surname
 
+    if input.start_date is not None:
+        result["startDate"] = input.start_date
+
     if input.manager is not None:
         result["manager"] = input.manager
 
-    if input.end_date is not None:
-        result["endDate"] = input.end_date
+    if input.name is not None:
+        result["name"] = input.name
+
+    if input.department is not None:
+        result["department"] = input.department
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3517,26 +3559,26 @@
         headquarter_id=urlquote(input.headquarter_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.city is not None:
-        result["city"] = input.city
-
-    if input.address is not None:
-        result["address"] = input.address
-
     if input.zipcode is not None:
         result["zipcode"] = input.zipcode
 
     if input.country is not None:
         result["country"] = input.country
 
+    if input.city is not None:
+        result["city"] = input.city
+
+    if input.address is not None:
+        result["address"] = input.address
+
     if input.name is not None:
         result["name"] = input.name
 
     if input.tom_ids is not None:
         result["tomIds"] = input.tom_ids
 
     content = json.dumps(result).encode("utf-8")
@@ -3573,96 +3615,96 @@
         processing_activity_id=urlquote(input.processing_activity_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.additional_info is not None:
-        result["additionalInfo"] = input.additional_info
+    if input.purpose is not None:
+        result["purpose"] = input.purpose
 
-    if input.data_subjects is not None:
-        result["dataSubjects"] = _serialize_data_subject_collection(
-            input.data_subjects, config
-        )
+    if input.infotype_categories is not None:
+        result["infotypeCategories"] = input.infotype_categories
 
-    if input.model_id is not None:
-        result["modelId"] = input.model_id
+    if input.active is not None:
+        result["active"] = input.active
 
-    if input.contact_person is not None:
-        result["contactPerson"] = input.contact_person
+    if input.lawful_basis is not None:
+        result["lawfulBasis"] = _serialize_lawful_basis_collection(
+            input.lawful_basis, config
+        )
 
     if input.name is not None:
         result["name"] = input.name
 
-    if input.active is not None:
-        result["active"] = input.active
-
-    if input.infotype_categories is not None:
-        result["infotypeCategories"] = input.infotype_categories
-
     if input.retention_period_comment is not None:
         result["retentionPeriodComment"] = input.retention_period_comment
 
-    if input.is_data_stored is not None:
-        result["isDataStored"] = input.is_data_stored
-
-    if input.purpose is not None:
-        result["purpose"] = input.purpose
-
-    if input.additional_info_files is not None:
-        result["additionalInfoFiles"] = input.additional_info_files
+    if input.data_subjects is not None:
+        result["dataSubjects"] = _serialize_data_subject_collection(
+            input.data_subjects, config
+        )
 
-    if input.infotype_volume is not None:
-        result["infotypeVolume"] = input.infotype_volume
+    if input.processing_frequency_comment is not None:
+        result["processingFrequencyComment"] = input.processing_frequency_comment
 
     if input.company_role is not None:
         result["companyRole"] = input.company_role
 
-    if input.data_types is not None:
-        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
+    if input.model_id is not None:
+        result["modelId"] = input.model_id
 
     if input.recipients is not None:
         result["recipients"] = _serialize_recipient_collection(input.recipients, config)
 
-    if input.processing_frequency_comment is not None:
-        result["processingFrequencyComment"] = input.processing_frequency_comment
+    if input.are_access_requests_managed is not None:
+        result["areAccessRequestsManaged"] = input.are_access_requests_managed
 
-    if input.infotypes is not None:
-        result["infotypes"] = input.infotypes
+    if input.data_types is not None:
+        result["dataTypes"] = _serialize_data_type_collection(input.data_types, config)
 
-    if input.lawful_basis is not None:
-        result["lawfulBasis"] = _serialize_lawful_basis_collection(
-            input.lawful_basis, config
-        )
+    if input.additional_info_files is not None:
+        result["additionalInfoFiles"] = input.additional_info_files
+
+    if input.is_data_stored is not None:
+        result["isDataStored"] = input.is_data_stored
+
+    if input.processing_frequency is not None:
+        result["processingFrequency"] = input.processing_frequency
+
+    if input.assets is not None:
+        result["assets"] = input.assets
+
+    if input.departments is not None:
+        result["departments"] = input.departments
 
     if input.retention_period is not None:
         result["retentionPeriod"] = _serialize_retention_period(
             input.retention_period, config
         )
 
     if input.data_sources is not None:
         result["dataSources"] = input.data_sources
 
+    if input.contact_person is not None:
+        result["contactPerson"] = input.contact_person
+
     if input.management_methods is not None:
         result["managementMethods"] = _serialize_management_method_collection(
             input.management_methods, config
         )
 
-    if input.assets is not None:
-        result["assets"] = input.assets
-
-    if input.processing_frequency is not None:
-        result["processingFrequency"] = input.processing_frequency
+    if input.infotypes is not None:
+        result["infotypes"] = input.infotypes
 
-    if input.are_access_requests_managed is not None:
-        result["areAccessRequestsManaged"] = input.are_access_requests_managed
+    if input.infotype_volume is not None:
+        result["infotypeVolume"] = input.infotype_volume
 
-    if input.departments is not None:
-        result["departments"] = input.departments
+    if input.additional_info is not None:
+        result["additionalInfo"] = input.additional_info
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3694,50 +3736,50 @@
         recipient_id=urlquote(input.recipient_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.country is not None:
-        result["country"] = input.country
-
-    if input.role is not None:
-        result["role"] = input.role
-
-    if input.dpa_files is not None:
-        result["dpaFiles"] = input.dpa_files
-
-    if input.dpa_status is not None:
-        result["dpaStatus"] = input.dpa_status
-
     if input.dpa is not None:
         result["dpa"] = input.dpa
 
-    if input.state is not None:
-        result["state"] = input.state
+    if input.status is not None:
+        result["status"] = input.status
 
     if input.data_storage_location is not None:
         result["dataStorageLocation"] = input.data_storage_location
 
-    if input.category is not None:
-        result["category"] = input.category
+    if input.dpa_files is not None:
+        result["dpaFiles"] = input.dpa_files
 
-    if input.status is not None:
-        result["status"] = input.status
+    if input.dpa_status is not None:
+        result["dpaStatus"] = input.dpa_status
 
     if input.recipient_warranties is not None:
         result["recipientWarranties"] = input.recipient_warranties
 
     if input.name is not None:
         result["name"] = input.name
 
     if input.business_name is not None:
         result["businessName"] = input.business_name
 
+    if input.category is not None:
+        result["category"] = input.category
+
+    if input.country is not None:
+        result["country"] = input.country
+
+    if input.role is not None:
+        result["role"] = input.role
+
+    if input.state is not None:
+        result["state"] = input.state
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -3768,74 +3810,74 @@
         threshold_id=urlquote(input.threshold_id, safe=""),
     )
     query: str = f""
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
-    if input.prevent_data_subjects_exercising_their_rights is not None:
-        result["preventDataSubjectsExercisingTheirRights"] = (
-            input.prevent_data_subjects_exercising_their_rights
+    if input.matching_merging_records_involved is not None:
+        result["matchingMergingRecordsInvolved"] = (
+            input.matching_merging_records_involved
         )
 
-    if input.classifying_data_subject is not None:
-        result["classifyingDataSubject"] = input.classifying_data_subject
-
-    if input.comment is not None:
-        result["comment"] = input.comment
-
-    if input.large_scale_data_processing is not None:
-        result["largeScaleDataProcessing"] = input.large_scale_data_processing
-
     if input.automated_decision_making is not None:
         result["automatedDecisionMaking"] = input.automated_decision_making
 
-    if input.systematic_monitoring_data_subject is not None:
-        result["systematicMonitoringDataSubject"] = (
-            input.systematic_monitoring_data_subject
-        )
+    if input.classifying_data_subject is not None:
+        result["classifyingDataSubject"] = input.classifying_data_subject
 
     if input.processing_confidential_sensitive_data is not None:
         result["processingConfidentialSensitiveData"] = (
             input.processing_confidential_sensitive_data
         )
 
-    if input.large_scale_processing_sensitive_data is not None:
-        result["largeScaleProcessingSensitiveData"] = (
-            input.large_scale_processing_sensitive_data
+    if input.prevent_data_subjects_exercising_their_rights is not None:
+        result["preventDataSubjectsExercisingTheirRights"] = (
+            input.prevent_data_subjects_exercising_their_rights
         )
 
-    if input.matching_merging_records_involved is not None:
-        result["matchingMergingRecordsInvolved"] = (
-            input.matching_merging_records_involved
+    if input.extensive_automated_evaluation_characteristics is not None:
+        result["extensiveAutomatedEvaluationCharacteristics"] = (
+            input.extensive_automated_evaluation_characteristics
         )
 
-    if input.monitoring_publicly_accessible_areas is not None:
-        result["monitoringPubliclyAccessibleAreas"] = (
-            input.monitoring_publicly_accessible_areas
-        )
+    if input.blacklist is not None:
+        result["blacklist"] = input.blacklist
 
     if input.processing_vulnerable_data_subject is not None:
         result["processingVulnerableDataSubject"] = (
             input.processing_vulnerable_data_subject
         )
 
+    if input.innovative_technologies_used is not None:
+        result["innovativeTechnologiesUsed"] = input.innovative_technologies_used
+
+    if input.systematic_monitoring_data_subject is not None:
+        result["systematicMonitoringDataSubject"] = (
+            input.systematic_monitoring_data_subject
+        )
+
+    if input.monitoring_publicly_accessible_areas is not None:
+        result["monitoringPubliclyAccessibleAreas"] = (
+            input.monitoring_publicly_accessible_areas
+        )
+
     if input.status is not None:
         result["status"] = input.status
 
-    if input.blacklist is not None:
-        result["blacklist"] = input.blacklist
+    if input.large_scale_processing_sensitive_data is not None:
+        result["largeScaleProcessingSensitiveData"] = (
+            input.large_scale_processing_sensitive_data
+        )
 
-    if input.innovative_technologies_used is not None:
-        result["innovativeTechnologiesUsed"] = input.innovative_technologies_used
+    if input.large_scale_data_processing is not None:
+        result["largeScaleDataProcessing"] = input.large_scale_data_processing
 
-    if input.extensive_automated_evaluation_characteristics is not None:
-        result["extensiveAutomatedEvaluationCharacteristics"] = (
-            input.extensive_automated_evaluation_characteristics
-        )
+    if input.comment is not None:
+        result["comment"] = input.comment
 
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -3868,20 +3910,20 @@
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b"")
     result: dict[str, DocumentValue] = {}
 
     if input.document_files is not None:
         result["documentFiles"] = input.document_files
 
-    if input.status is not None:
-        result["status"] = input.status
-
     if input.note is not None:
         result["note"] = input.note
 
+    if input.status is not None:
+        result["status"] = input.status
+
     content = json.dumps(result).encode("utf-8")
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -4670,14 +4712,42 @@
         result["infoTypes"] = _serialize_info_types_combination_filter(
             input.info_types, config
         )
 
     return result
 
 
+def _serialize_list_logs_filter(
+    input: ListLogsFilter, config: Config
+) -> dict[str, DocumentValue]:
+    result: dict[str, DocumentValue] = {}
+
+    if input.search is not None:
+        result["search"] = input.search
+
+    result["logType"] = input.log_type
+
+    if input.email is not None:
+        result["email"] = input.email
+
+    if input.operation_name is not None:
+        result["operationName"] = input.operation_name
+
+    if input.request_id is not None:
+        result["requestId"] = input.request_id
+
+    if input.start is not None:
+        result["start"] = input.start
+
+    if input.end is not None:
+        result["end"] = input.end
+
+    return result
+
+
 def _serialize_management_method(
     input: ManagementMethod, config: Config
 ) -> dict[str, DocumentValue]:
     result: dict[str, DocumentValue] = {}
 
     result["methodType"] = input.method_type
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client.egg-info/PKG-INFO` & `borneo_python_client-3.10.1/borneo_python_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borneo_python_client
-Version: 3.10.0
+Version: 3.10.1
 Summary: borneo_python_client client
 License: Apache-2.0
 Keywords: smithy,borneo_python_client
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
@@ -46,15 +46,15 @@
 
 Requests to the Borneo API must be authenticated using an authentication token. The token is passed in the `Authorization` header of the request.
 
 ```
 Authorization: Bearer <token>
 ```
 
-**TODO**: Explain how to obtain the authentication token.
+This authorization Bearer token can generated using service accounts and Borneo SDK or directly download Borneo token from dashboard for testing.
 
 ## Pagination
 
 All list operations support pagination. The `pageSize` parameter can be
 used to control the number of results returned per API request. If there
 are more results available, the API response will contain a `nextToken`
 value that can be used to retrieve the next page of results by passing it
```

### Comparing `borneo_python_client-3.10.0/borneo_python_client.egg-info/SOURCES.txt` & `borneo_python_client-3.10.1/borneo_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `borneo_python_client-3.10.0/pyproject.toml` & `borneo_python_client-3.10.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "borneo_python_client"
-version = "3.10.0"
+version = "3.10.1"
 description = "borneo_python_client client"
 readme = "README.md"
 requires-python = ">=3.12"
 keywords = ["smithy", "borneo_python_client"]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `borneo_python_client-3.10.0/tests/test_protocol.py` & `borneo_python_client-3.10.1/tests/test_protocol.py`

 * *Files identical despite different names*

