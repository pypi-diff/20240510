# Comparing `tmp/python_roborock-2.1.1.tar.gz` & `tmp/python_roborock-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-2.1.1.tar", max compression
+gzip compressed data, was "python_roborock-2.2.0.tar", max compression
```

## Comparing `python_roborock-2.1.1.tar` & `python_roborock-2.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2024-05-08 13:21:17.495140 python_roborock-2.1.1/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-08 13:21:17.495140 python_roborock-2.1.1/README.md
--rw-r--r--   0        0        0     1677 2024-05-08 13:21:18.183148 python_roborock-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      165 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/__init__.py
--rw-r--r--   0        0        0     4107 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/api.py
--rw-r--r--   0        0        0     6826 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/cli.py
--rw-r--r--   0        0        0     7144 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/cloud_api.py
--rw-r--r--   0        0        0    14400 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/code_mappings.py
--rw-r--r--   0        0        0     7912 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/command_cache.py
--rw-r--r--   0        0        0     2386 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/const.py
--rw-r--r--   0        0        0    27991 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/containers.py
--rw-r--r--   0        0        0     1962 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/exceptions.py
--rw-r--r--   0        0        0     4367 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/local_api.py
--rw-r--r--   0        0        0    12315 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/protocol.py
--rw-r--r--   0        0        0        0 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/py.typed
--rw-r--r--   0        0        0      834 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/roborock_future.py
--rw-r--r--   0        0        0     5464 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/roborock_message.py
--rw-r--r--   0        0        0    23536 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/roborock_typing.py
--rw-r--r--   0        0        0     3465 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/util.py
--rw-r--r--   0        0        0      183 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/version_1_apis/__init__.py
--rw-r--r--   0        0        0    20099 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/version_1_apis/roborock_client_v1.py
--rw-r--r--   0        0        0     3477 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/version_1_apis/roborock_local_client_v1.py
--rw-r--r--   0        0        0     3342 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/version_1_apis/roborock_mqtt_client_v1.py
--rw-r--r--   0        0        0      111 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/version_a01_apis/__init__.py
--rw-r--r--   0        0        0     7342 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/version_a01_apis/roborock_client_a01.py
--rw-r--r--   0        0        0     2961 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/version_a01_apis/roborock_mqtt_client_a01.py
--rw-r--r--   0        0        0    13040 2024-05-08 13:21:17.499140 python_roborock-2.1.1/roborock/web_api.py
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-09 22:02:21.121070 python_roborock-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-09 22:02:21.121070 python_roborock-2.2.0/README.md
+-rw-r--r--   0        0        0     1677 2024-05-09 22:02:21.837068 python_roborock-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/__init__.py
+-rw-r--r--   0        0        0     4123 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/api.py
+-rw-r--r--   0        0        0     6826 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/cli.py
+-rw-r--r--   0        0        0     7144 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/cloud_api.py
+-rw-r--r--   0        0        0    14400 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/code_mappings.py
+-rw-r--r--   0        0        0     7912 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/command_cache.py
+-rw-r--r--   0        0        0     2386 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/const.py
+-rw-r--r--   0        0        0    27991 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/containers.py
+-rw-r--r--   0        0        0     1962 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/exceptions.py
+-rw-r--r--   0        0        0     4367 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/local_api.py
+-rw-r--r--   0        0        0    12315 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/protocol.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/py.typed
+-rw-r--r--   0        0        0      834 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/roborock_future.py
+-rw-r--r--   0        0        0     5464 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/roborock_message.py
+-rw-r--r--   0        0        0    23536 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/roborock_typing.py
+-rw-r--r--   0        0        0     3465 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/util.py
+-rw-r--r--   0        0        0      183 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/__init__.py
+-rw-r--r--   0        0        0    20099 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/roborock_client_v1.py
+-rw-r--r--   0        0        0     3477 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/roborock_local_client_v1.py
+-rw-r--r--   0        0        0     3358 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/roborock_mqtt_client_v1.py
+-rw-r--r--   0        0        0      111 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_a01_apis/__init__.py
+-rw-r--r--   0        0        0     7424 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_a01_apis/roborock_client_a01.py
+-rw-r--r--   0        0        0     3043 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py
+-rw-r--r--   0        0        0    13040 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/web_api.py
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-2.2.0/PKG-INFO
```

### Comparing `python_roborock-2.1.1/LICENSE` & `python_roborock-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/README.md` & `python_roborock-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/pyproject.toml` & `python_roborock-2.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "2.1.1"
+version = "2.2.0"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 documentation = "https://python-roborock.readthedocs.io/"
 classifiers = [
```

### Comparing `python_roborock-2.1.1/roborock/api.py` & `python_roborock-2.2.0/roborock/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,18 @@
         self._logger = RoborockLoggerAdapter(device_info.device.name, _LOGGER)
         self.is_available: bool = True
         self.queue_timeout = queue_timeout
 
     def __del__(self) -> None:
         self.release()
 
-    def release(self):
+    def release(self) -> None:
         self.sync_disconnect()
 
-    async def async_release(self):
+    async def async_release(self) -> None:
         await self.async_disconnect()
 
     @property
     def diagnostic_data(self) -> dict:
         return self._diagnostic_data
 
     @property
```

### Comparing `python_roborock-2.1.1/roborock/cli.py` & `python_roborock-2.2.0/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/cloud_api.py` & `python_roborock-2.2.0/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/code_mappings.py` & `python_roborock-2.2.0/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/command_cache.py` & `python_roborock-2.2.0/roborock/command_cache.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/const.py` & `python_roborock-2.2.0/roborock/const.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/containers.py` & `python_roborock-2.2.0/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/exceptions.py` & `python_roborock-2.2.0/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/local_api.py` & `python_roborock-2.2.0/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/protocol.py` & `python_roborock-2.2.0/roborock/protocol.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/roborock_future.py` & `python_roborock-2.2.0/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/roborock_message.py` & `python_roborock-2.2.0/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/roborock_typing.py` & `python_roborock-2.2.0/roborock/roborock_typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/util.py` & `python_roborock-2.2.0/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/version_1_apis/roborock_client_v1.py` & `python_roborock-2.2.0/roborock/version_1_apis/roborock_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/version_1_apis/roborock_local_client_v1.py` & `python_roborock-2.2.0/roborock/version_1_apis/roborock_local_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/roborock/version_1_apis/roborock_mqtt_client_v1.py` & `python_roborock-2.2.0/roborock/version_1_apis/roborock_mqtt_client_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,9 +67,9 @@
         params: list | dict | int | None = None,
     ):
         request_id, timestamp, payload = self._get_payload(method, params, True)
         request_protocol = RoborockMessageProtocol.RPC_REQUEST
         roborock_message = RoborockMessage(timestamp=timestamp, protocol=request_protocol, payload=payload)
         return await self.send_message(roborock_message)
 
-    async def get_map_v1(self):
+    async def get_map_v1(self) -> bytes | None:
         return await self.send_command(RoborockCommand.GET_MAP_V1)
```

### Comparing `python_roborock-2.1.1/roborock/version_a01_apis/roborock_client_a01.py` & `python_roborock-2.2.0/roborock/version_a01_apis/roborock_client_a01.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,10 +133,12 @@
                     if data_point_protocol in entries:
                         # Auto convert into data struct we want.
                         converted_response = entries[data_point_protocol].post_process_fn(data_point)
                         queue = self._waiting_queue.get(int(data_point_number))
                         if queue and queue.protocol == protocol:
                             queue.resolve((converted_response, None))
 
-    async def update_values(self, dyad_data_protocols: list[RoborockDyadDataProtocol | RoborockZeoProtocol]):
+    async def update_values(
+        self, dyad_data_protocols: list[RoborockDyadDataProtocol | RoborockZeoProtocol]
+    ) -> dict[RoborockDyadDataProtocol | RoborockZeoProtocol, typing.Any]:
         """This should handle updating for each given protocol."""
         raise NotImplementedError
```

### Comparing `python_roborock-2.1.1/roborock/version_a01_apis/roborock_mqtt_client_a01.py` & `python_roborock-2.2.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,17 @@
                 if isinstance(response, BaseException):
                     self._logger.warning("Timed out get req for %s after %s s", dps, self.queue_timeout)
                     dps_responses[dps] = None
                 else:
                     dps_responses[dps] = response[0]
         return dps_responses
 
-    async def update_values(self, dyad_data_protocols: list[RoborockDyadDataProtocol | RoborockZeoProtocol]):
+    async def update_values(
+        self, dyad_data_protocols: list[RoborockDyadDataProtocol | RoborockZeoProtocol]
+    ) -> dict[RoborockDyadDataProtocol | RoborockZeoProtocol, typing.Any]:
         payload = {"dps": {RoborockDyadDataProtocol.ID_QUERY: str([int(protocol) for protocol in dyad_data_protocols])}}
         return await self.send_message(
             RoborockMessage(
                 protocol=RoborockMessageProtocol.RPC_REQUEST,
                 version=b"A01",
                 payload=pad(json.dumps(payload).encode("utf-8"), AES.block_size),
             )
```

### Comparing `python_roborock-2.1.1/roborock/web_api.py` & `python_roborock-2.2.0/roborock/web_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.1.1/PKG-INFO` & `python_roborock-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 2.1.1
+Version: 2.2.0
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 2.1.1 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 2.2.0 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
```

