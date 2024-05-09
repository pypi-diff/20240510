# Comparing `tmp/telstra_messaging-3.1.0.tar.gz` & `tmp/telstra_messaging-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telstra_messaging-3.1.0.tar", max compression
+gzip compressed data, was "telstra_messaging-3.3.4.tar", max compression
```

## Comparing `telstra_messaging-3.1.0.tar` & `telstra_messaging-3.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11378 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/LICENSE
--rw-r--r--   0        0        0    27526 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/README.md
--rw-r--r--   0        0        0      888 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/__init__.py
--rw-r--r--   0        0        0       40 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/__init__.py
--rw-r--r--   0        0        0      762 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/exceptions.py
--rw-r--r--   0        0        0     4678 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/free_trial_numbers.py
--rw-r--r--   0        0        0     1056 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/health_check.py
--rw-r--r--   0        0        0    31562 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/message.py
--rw-r--r--   0        0        0     2814 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/oauth.py
--rw-r--r--   0        0        0     8768 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/reports.py
--rw-r--r--   0        0        0      903 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/types.py
--rw-r--r--   0        0        0       38 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/__init__.py
--rw-r--r--   0        0        0      743 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/callback_url.py
--rw-r--r--   0        0        0     6152 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/config.py
--rw-r--r--   0        0        0     1315 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/error_response.py
--rw-r--r--   0        0        0     2043 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/free_trial_number.py
--rw-r--r--   0        0        0      933 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/message_id.py
--rw-r--r--   0        0        0      409 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/querystring.py
--rw-r--r--   0        0        0     2961 2023-07-04 01:58:39.690227 telstra_messaging-3.1.0/telstra/messaging/utils/reports_dates.py
--rw-r--r--   0        0        0      929 2023-07-04 01:58:39.694228 telstra_messaging-3.1.0/telstra/messaging/utils/schedule_send.py
--rw-r--r--   0        0        0     1662 2023-07-04 01:58:39.694228 telstra_messaging-3.1.0/telstra/messaging/utils/virtual_number.py
--rw-r--r--   0        0        0    20267 2023-07-04 01:58:39.694228 telstra_messaging-3.1.0/telstra/messaging/virtual_number.py
--rw-r--r--   0        0        0    28024 1970-01-01 00:00:00.000000 telstra_messaging-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11378 2024-05-09 09:48:10.590731 telstra_messaging-3.3.4/LICENSE
+-rw-r--r--   0        0        0    27526 2024-05-09 09:48:10.590731 telstra_messaging-3.3.4/README.md
+-rw-r--r--   0        0        0      888 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/pyproject.toml
+-rw-r--r--   0        0        0       32 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/__init__.py
+-rw-r--r--   0        0        0      762 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/exceptions.py
+-rw-r--r--   0        0        0     4678 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/free_trial_numbers.py
+-rw-r--r--   0        0        0     1056 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/health_check.py
+-rw-r--r--   0        0        0    31562 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/message.py
+-rw-r--r--   0        0        0     2981 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/oauth.py
+-rw-r--r--   0        0        0     8768 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/reports.py
+-rw-r--r--   0        0        0      903 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/types.py
+-rw-r--r--   0        0        0       38 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/__init__.py
+-rw-r--r--   0        0        0      743 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/callback_url.py
+-rw-r--r--   0        0        0     6152 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/config.py
+-rw-r--r--   0        0        0     1315 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/error_response.py
+-rw-r--r--   0        0        0     2043 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/free_trial_number.py
+-rw-r--r--   0        0        0      933 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/message_id.py
+-rw-r--r--   0        0        0      409 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/querystring.py
+-rw-r--r--   0        0        0     2961 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/reports_dates.py
+-rw-r--r--   0        0        0      929 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/schedule_send.py
+-rw-r--r--   0        0        0     1662 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/utils/virtual_number.py
+-rw-r--r--   0        0        0    20267 2024-05-09 09:48:10.594731 telstra_messaging-3.3.4/telstra/messaging/virtual_number.py
+-rw-r--r--   0        0        0    28075 1970-01-01 00:00:00.000000 telstra_messaging-3.3.4/PKG-INFO
```

### Comparing `telstra_messaging-3.1.0/LICENSE` & `telstra_messaging-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/README.md` & `telstra_messaging-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/pyproject.toml` & `telstra_messaging-3.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telstra.messaging"
-version = "3.1.0"
+version = "3.3.4"
 readme = "README.md"
 description = "SDK for the Telstra Messaging API V3 - Beta"
 license = "Apache-2.0"
 authors = ["David Andersson <david-andersson@users.noreply.github.com >"]
 include = ["telstra"]
 exclude = ["tests"]
 packages = [
```

### Comparing `telstra_messaging-3.1.0/telstra/messaging/exceptions.py` & `telstra_messaging-3.3.4/telstra/messaging/exceptions.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/free_trial_numbers.py` & `telstra_messaging-3.3.4/telstra/messaging/free_trial_numbers.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/health_check.py` & `telstra_messaging-3.3.4/telstra/messaging/health_check.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/message.py` & `telstra_messaging-3.3.4/telstra/messaging/message.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/oauth.py` & `telstra_messaging-3.3.4/telstra/messaging/oauth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Handles OAuth interactions."""
 
 import dataclasses
 import json
 import math
 import time
+from typing import Optional
 from urllib import error, parse, request
 
 from . import exceptions
 from .utils import config
 
 _URL = "https://products.api.telstra.com/v2/oauth/token"
 
@@ -24,29 +25,38 @@
         retrieved_at: The time when the token was retrieved.
 
         expired: Whether the token is expired.
         authorization: The value of the Authorization header with the token.
 
     """
 
-    def __init__(self, access_token: str, token_type: str, expires_in: str):
+    def __init__(
+        self,
+        access_token: str,
+        token_type: str,
+        expires_in: str,
+        scope: Optional[str] = None,
+    ):
         """Construct."""
         self.retrieved_at = math.ceil(time.time())
         self.access_token = access_token
         self.token_type = token_type
         self.expires_in = int(expires_in)
+        self.scope = scope
 
     # The access token
     access_token: str
     # The type of the token
     token_type: str
     # The time to expiry
     expires_in: int
     # The time it was created
     retrieved_at: int
+    # scope
+    scope: Optional[str]
 
     @property
     def expired(self):
         """Whether the tokens are expired."""
         return math.ceil(time.time()) >= self.retrieved_at + self.expires_in
 
     @property
@@ -80,15 +90,15 @@
 
     """
     data = parse.urlencode(
         {
             "grant_type": "client_credentials",
             "client_id": config.get().telstra_client_id,
             "client_secret": config.get().telstra_client_secret,
-            "scope": "free-trial-numbers:read free-trial-numbers:write virtual-numbers:read virtual-numbers:write messages:read messaging:write reports:read reports:write",
+            "scope": "free-trial-numbers:read free-trial-numbers:write messages:read messages:write virtual-numbers:read virtual-numbers:write reports:read reports:write",
         }
     ).encode("ascii")
     headers = {"Content-Type": "application/x-www-form-urlencoded", "Accept": "*/*"}
     oauth_request = request.Request(_URL, data=data, headers=headers, method="POST")
     try:
         with request.urlopen(oauth_request) as response:
             return TToken(**json.loads(response.read().decode()))
```

### Comparing `telstra_messaging-3.1.0/telstra/messaging/reports.py` & `telstra_messaging-3.3.4/telstra/messaging/reports.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/types.py` & `telstra_messaging-3.3.4/telstra/messaging/types.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/callback_url.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/callback_url.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/config.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/config.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/error_response.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/error_response.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/free_trial_number.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/free_trial_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/message_id.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/message_id.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/reports_dates.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/reports_dates.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/schedule_send.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/schedule_send.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/utils/virtual_number.py` & `telstra_messaging-3.3.4/telstra/messaging/utils/virtual_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/telstra/messaging/virtual_number.py` & `telstra_messaging-3.3.4/telstra/messaging/virtual_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.1.0/PKG-INFO` & `telstra_messaging-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: telstra-messaging
-Version: 3.1.0
+Name: telstra.messaging
+Version: 3.3.4
 Summary: SDK for the Telstra Messaging API V3 - Beta
 License: Apache-2.0
 Author: David Andersson
 Author-email: david-andersson@users.noreply.github.com 
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Telstra Messaging
 
 The SDK for the Telstra Messaging API enables you to send and receive messages
 to Australian mobile numbers. For more information about this product, please
 see here:
```

