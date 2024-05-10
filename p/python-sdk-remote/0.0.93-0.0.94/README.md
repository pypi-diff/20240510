# Comparing `tmp/python_sdk_remote-0.0.93.tar.gz` & `tmp/python_sdk_remote-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sdk_remote-0.0.93.tar", last modified: Tue May  7 04:52:27 2024, max compression
+gzip compressed data, was "python_sdk_remote-0.0.94.tar", last modified: Fri May 10 15:20:13 2024, max compression
```

## Comparing `python_sdk_remote-0.0.93.tar` & `python_sdk_remote-0.0.94.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.756741 python_sdk_remote-0.0.93/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/get_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/http_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:13.675476 python_sdk_remote-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 15:20:13.675476 python_sdk_remote-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:13.671476 python_sdk_remote-0.0.94/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:13.675476 python_sdk_remote-0.0.94/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/get_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:20:13.675476 python_sdk_remote-0.0.94/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 15:20:13.000000 python_sdk_remote-0.0.94/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-10 15:20:13.000000 python_sdk_remote-0.0.94/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:20:13.000000 python_sdk_remote-0.0.94/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 15:20:13.000000 python_sdk_remote-0.0.94/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 15:20:13.000000 python_sdk_remote-0.0.94/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:20:13.675476 python_sdk_remote-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-10 15:19:59.000000 python_sdk_remote-0.0.94/setup.py
```

### Comparing `python_sdk_remote-0.0.93/PKG-INFO` & `python_sdk_remote-0.0.94/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.93
+Version: 0.0.94
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: url-remote
-Requires-Dist: http-status-codes
 
 This is a package for sharing common functions used in different repositories
```

### Comparing `python_sdk_remote-0.0.93/README.md` & `python_sdk_remote-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote/src/constants.py` & `python_sdk_remote-0.0.94/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote/src/http_response.py` & `python_sdk_remote-0.0.94/python_sdk_remote/src/http_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 import json
-from http_constants import status
+from typing import Any
+from http import HTTPStatus
 
 from .mini_logger import MiniLogger as logger
 
 HEADERS_KEY = 'headers'
 AUTHORIZATION_KEY = 'authorization'
 AUTHORIZATION_PREFIX = 'Bearer '
 
 # TODO Align those methods with typescript-sdk https://github.com/circles-zone/typescript-sdk-remote-typescript-package/blob/dev/typescript-sdk/src/utils/index.ts  # noqa501
 # TODO Shall we create also createInternalServerErrorHttpResponse(), createOkHttpResponse() like we have in TypeScript?
 
-# Former name was create_http_headers()
+# TODO: add handler wrapper?
+
+def get_payload_dict_from_event(event: dict) -> dict:
+    """Extracts params sent with payload"""
+    return json.loads(event.get('body') or '{}')
+
+def get_path_parameters_dict_from_event(event: dict) -> dict:
+    """Extracts params sent implicitly: `url/param?test=5` -> param
+    (when the path is defined with /{param})"""
+    return event.get('pathParameters') or {}
+
+def get_query_string_parameters_from_event(event: dict) -> dict:
+    """Extracts params sent explicitly: `url/test?a=1&b=2` ->  {'a': '1', 'b': '2'}"""
+    return event.get("queryStringParameters") or {}  # params sent with ?a=1&b=2
+
 def create_authorization_http_headers(user_jwt: str) -> dict:
     logger.start(object={"user_jwt": user_jwt})
     authorization_http_headers = {
         'Content-Type': 'application/json',
         'Authorization': AUTHORIZATION_PREFIX + user_jwt,
     }
     logger.end(object={"authorization_http_headers": authorization_http_headers})
@@ -36,37 +51,37 @@
     return_http_headers = {
         "Content-Type": "application/json",
         "Access-Control-Allow-Origin": "*",
     }
     logger.end(object={"return_http_headers": return_http_headers})
     return return_http_headers
 
-def create_error_http_response(exception: Exception) -> dict:
+def create_error_http_response(exception: Exception, status_code: HTTPStatus) -> dict:
     logger.start(object={"exception": exception})
     error_http_response = {
-            "statusCode": status.BAD_GATEWAY,
+            "statusCode": HTTPStatus.value,
             "headers": create_return_http_headers(),
             "body": create_http_body({"error": str(exception)})
         }
     logger.end(object={"error_http_response": error_http_response})
     return error_http_response
 
 
-def create_ok_http_response(body: dict) -> dict:
+def create_ok_http_response(body: Any) -> dict:
     logger.start(object={"body": body})
     ok_http_response = {
-        "statusCode": status.OK,
+        "statusCode": HTTPStatus.OK.value,
         "headers": create_return_http_headers(),
         "body": create_http_body(body)
     }
     logger.end(object={"ok_http_response": ok_http_response})
     return ok_http_response
 
 
 # https://google.github.io/styleguide/jsoncstyleguide.xml?showone=Property_Name_Format#Property_Name_Format
-def create_http_body(body: dict) -> str:
+def create_http_body(body: Any) -> str:
     # TODO console.warning() if the body is not a valid camelCase JSON
     # https://stackoverflow.com/questions/17156078/converting-identifier-naming-between-camelcase-and-underscores-during-json-seria
     logger.start(object={"body": body})
     http_body = json.dumps(body)
     logger.end(object={"http_body": http_body})
     return http_body
```

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote/src/mini_logger.py` & `python_sdk_remote-0.0.94/python_sdk_remote/src/mini_logger.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote/src/our_object.py` & `python_sdk_remote-0.0.94/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote/src/unified_json.py` & `python_sdk_remote-0.0.94/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote/src/utilities.py` & `python_sdk_remote-0.0.94/python_sdk_remote/src/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 
 from .http_response import (create_authorization_http_headers, get_user_jwt_from_event,  # noqa - used for backwards compatibility
                             create_return_http_headers, create_error_http_response, create_ok_http_response,
                             create_http_body)
 from .mini_logger import MiniLogger as logger
 
 load_dotenv()
+# raise Exception("Failed to load environment variables from .env file\n"
+#                 "Please check if the file exists, maybe you are not in the right venv?")
 
+# TODO: add cache with/out timeout decorator
+
+DEFAULT_LANG_CODE_STR = "en"
 
 def timedelta_to_time_format(time_delta: timedelta) -> str:
     """
     Convert a timedelta to a time format in HH:MM:SS.
 
     Parameters:
         time_delta (datetime.timedelta): The timedelta to be converted.
```

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote/src/validate_environment.py` & `python_sdk_remote-0.0.94/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote.egg-info/PKG-INFO` & `python_sdk_remote-0.0.94/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.93
+Version: 0.0.94
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: url-remote
-Requires-Dist: http-status-codes
 
 This is a package for sharing common functions used in different repositories
```

### Comparing `python_sdk_remote-0.0.93/python_sdk_remote.egg-info/SOURCES.txt` & `python_sdk_remote-0.0.94/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.93/setup.py` & `python_sdk_remote-0.0.94/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.93',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.94',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
@@ -20,11 +20,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "python-dotenv",
-        "url-remote",
-        "http-status-codes"
+        "url-remote"
     ]
 )
```

