# Comparing `tmp/airbyte_source_iterable-0.5.1.dev202405100053.tar.gz` & `tmp/airbyte_source_iterable-0.5.1.dev202405100143.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_iterable-0.5.1.dev202405100053.tar", max compression
+gzip compressed data, was "airbyte_source_iterable-0.5.1.dev202405100143.tar", max compression
```

## Comparing `airbyte_source_iterable-0.5.1.dev202405100053.tar` & `airbyte_source_iterable-0.5.1.dev202405100143.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4542 2024-05-10 00:50:18.809655 airbyte_source_iterable-0.5.1.dev202405100053/README.md
--rw-r--r--   0        0        0      887 2024-05-10 00:53:28.700198 airbyte_source_iterable-0.5.1.dev202405100053/pyproject.toml
--rw-r--r--   0        0        0       65 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/__init__.py
--rw-r--r--   0        0        0     1374 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/components.py
--rw-r--r--   0        0        0    13996 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/manifest.yaml
--rw-r--r--   0        0        0      236 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/run.py
--rw-r--r--   0        0        0     2494 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/campaigns.json
--rw-r--r--   0        0        0      168 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/campaigns_metrics.json
--rw-r--r--   0        0        0      605 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/channels.json
--rw-r--r--   0        0        0     1755 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_bounce.json
--rw-r--r--   0        0        0     2749 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_click.json
--rw-r--r--   0        0        0     1704 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_complaint.json
--rw-r--r--   0        0        0     2257 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_open.json
--rw-r--r--   0        0        0     5994 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send.json
--rw-r--r--   0        0        0     6124 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send_skip.json
--rw-r--r--   0        0        0     1773 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_subscribe.json
--rw-r--r--   0        0        0     2665 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_unsubscribe.json
--rw-r--r--   0        0        0     1193 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/events.json
--rw-r--r--   0        0        0      307 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/list_users.json
--rw-r--r--   0        0        0      521 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/lists.json
--rw-r--r--   0        0        0      437 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/message_types.json
--rw-r--r--   0        0        0      158 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/metadata.json
--rw-r--r--   0        0        0     1156 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/templates.json
--rw-r--r--   0        0        0    14569 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/users.json
--rw-r--r--   0        0        0     6482 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/slice_generators.py
--rw-r--r--   0        0        0     4537 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/source.py
--rw-r--r--   0        0        0     1009 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/spec.json
--rw-r--r--   0        0        0    19468 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/streams.py
--rw-r--r--   0        0        0      649 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/utils.py
--rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 airbyte_source_iterable-0.5.1.dev202405100053/PKG-INFO
+-rw-r--r--   0        0        0     4542 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/README.md
+-rw-r--r--   0        0        0      887 2024-05-10 01:43:38.287632 airbyte_source_iterable-0.5.1.dev202405100143/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/__init__.py
+-rw-r--r--   0        0        0     1374 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/components.py
+-rw-r--r--   0        0        0    13996 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/run.py
+-rw-r--r--   0        0        0     2494 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/campaigns.json
+-rw-r--r--   0        0        0      168 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/campaigns_metrics.json
+-rw-r--r--   0        0        0      605 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/channels.json
+-rw-r--r--   0        0        0     1755 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_bounce.json
+-rw-r--r--   0        0        0     2749 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_click.json
+-rw-r--r--   0        0        0     1704 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_complaint.json
+-rw-r--r--   0        0        0     2257 2024-05-10 01:40:30.009186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_open.json
+-rw-r--r--   0        0        0     5994 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_send.json
+-rw-r--r--   0        0        0     6124 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_send_skip.json
+-rw-r--r--   0        0        0     1773 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_subscribe.json
+-rw-r--r--   0        0        0     2665 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_unsubscribe.json
+-rw-r--r--   0        0        0     1193 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/events.json
+-rw-r--r--   0        0        0      307 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/list_users.json
+-rw-r--r--   0        0        0      521 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/lists.json
+-rw-r--r--   0        0        0      437 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/message_types.json
+-rw-r--r--   0        0        0      158 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/metadata.json
+-rw-r--r--   0        0        0     1156 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/templates.json
+-rw-r--r--   0        0        0    14569 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/users.json
+-rw-r--r--   0        0        0     6482 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/slice_generators.py
+-rw-r--r--   0        0        0     4537 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/source.py
+-rw-r--r--   0        0        0     1009 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/spec.json
+-rw-r--r--   0        0        0    19468 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/streams.py
+-rw-r--r--   0        0        0      649 2024-05-10 01:40:30.013186 airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/utils.py
+-rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 airbyte_source_iterable-0.5.1.dev202405100143/PKG-INFO
```

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/README.md` & `airbyte_source_iterable-0.5.1.dev202405100143/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/pyproject.toml` & `airbyte_source_iterable-0.5.1.dev202405100143/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.1.dev202405100053"
+version = "0.5.1.dev202405100143"
 name = "airbyte-source-iterable"
 description = "Source implementation for Iterable."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/components.py` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 #
 
 import json
 from dataclasses import dataclass
 from io import StringIO
 
 import requests
+from typing import Iterable
 from airbyte_cdk.sources.declarative.extractors.dpath_extractor import DpathExtractor
 from airbyte_cdk.sources.declarative.types import Config, Record, StreamSlice, StreamState
 
 
 @dataclass
 class XJsonRecordExtractor(DpathExtractor):
     def extract_records(self, response: requests.Response) -> list[Record]:
-        return [json.loads(record) for record in response.iter_lines()]
+        for record in response.iter_lines():
+            yield json.loads(record)
 
 
 @dataclass
 class ListUsersRecordExtractor(DpathExtractor):
-    def extract_records(self, response: requests.Response) -> list[Record]:
-        return [{"email": record.decode()} for record in response.iter_lines()]
+    def extract_records(self, response: requests.Response) -> Iterable[Record]:
+        for record in response.iter_lines():
+            yield {"email": record.decode()}
 
 
 @dataclass
 class EventsRecordExtractor(DpathExtractor):
     common_fields = ("itblInternal", "_type", "createdAt", "email")
 
-    def extract_records(self, response: requests.Response) -> list[Record]:
+    def extract_records(self, response: requests.Response) -> Iterable[Record]:
         jsonl_records = StringIO(response.text)
-        records = []
         for record in jsonl_records:
             record_dict = json.loads(record)
             record_dict_common_fields = {}
             for field in self.common_fields:
                 record_dict_common_fields[field] = record_dict.pop(field, None)
-
-            records.append({**record_dict_common_fields, "data": record_dict})
-
-        return records
+            yield {**record_dict_common_fields, "data": record_dict}
```

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/manifest.yaml` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/campaigns.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/channels.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/channels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_bounce.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_bounce.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_click.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_click.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_complaint.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_complaint.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_open.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_open.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_send.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send_skip.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_send_skip.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_subscribe.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_subscribe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_unsubscribe.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/email_unsubscribe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/events.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/lists.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/templates.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/templates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/users.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/slice_generators.py` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/slice_generators.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/source.py` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/spec.json` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/streams.py` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/utils.py` & `airbyte_source_iterable-0.5.1.dev202405100143/source_iterable/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405100053/PKG-INFO` & `airbyte_source_iterable-0.5.1.dev202405100143/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-iterable
-Version: 0.5.1.dev202405100053
+Version: 0.5.1.dev202405100143
 Summary: Source implementation for Iterable.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

