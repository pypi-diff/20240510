# Comparing `tmp/airbyte_source_intercom-0.6.2.dev202403211932.tar.gz` & `tmp/airbyte_source_intercom-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_intercom-0.6.2.dev202403211932.tar", max compression
+gzip compressed data, was "airbyte_source_intercom-0.6.3.tar", max compression
```

## Comparing `airbyte_source_intercom-0.6.2.dev202403211932.tar` & `airbyte_source_intercom-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4537 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/README.md
--rw-r--r--   0        0        0      781 2024-03-21 19:32:56.298784 airbyte_source_intercom-0.6.2.dev202403211932/pyproject.toml
--rw-r--r--   0        0        0      128 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/__init__.py
--rw-r--r--   0        0        0    17630 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/components.py
--rw-r--r--   0        0        0    12953 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/manifest.yaml
--rw-r--r--   0        0        0      236 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/run.py
--rw-r--r--   0        0        0      702 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/activity_logs.json
--rw-r--r--   0        0        0     1494 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/admins.json
--rwxr-xr-x   0        0        0     2440 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/companies.json
--rw-r--r--   0        0        0     1189 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/company_attributes.json
--rwxr-xr-x   0        0        0      444 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/company_segments.json
--rw-r--r--   0        0        0     1112 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/contact_attributes.json
--rwxr-xr-x   0        0        0     8197 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/contacts.json
--rwxr-xr-x   0        0        0     2267 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/conversation_parts.json
--rwxr-xr-x   0        0        0    10592 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/conversations.json
--rwxr-xr-x   0        0        0      444 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/segments.json
--rw-r--r--   0        0        0      205 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/tags.json
--rw-r--r--   0        0        0      412 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/teams.json
--rw-r--r--   0        0        0      477 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/source.py
--rw-r--r--   0        0        0     2431 2024-03-21 19:30:12.386112 airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/spec.json
--rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 airbyte_source_intercom-0.6.2.dev202403211932/PKG-INFO
+-rw-r--r--   0        0        0     4537 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/README.md
+-rw-r--r--   0        0        0      765 2024-03-23 07:25:54.885189 airbyte_source_intercom-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/__init__.py
+-rw-r--r--   0        0        0    19399 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/components.py
+-rw-r--r--   0        0        0    13437 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/run.py
+-rw-r--r--   0        0        0      702 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/activity_logs.json
+-rw-r--r--   0        0        0     1494 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/admins.json
+-rwxr-xr-x   0        0        0     2440 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/companies.json
+-rw-r--r--   0        0        0     1189 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/company_attributes.json
+-rwxr-xr-x   0        0        0      444 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/company_segments.json
+-rw-r--r--   0        0        0     1112 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/contact_attributes.json
+-rwxr-xr-x   0        0        0     8197 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/contacts.json
+-rwxr-xr-x   0        0        0     2267 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/conversation_parts.json
+-rwxr-xr-x   0        0        0    10592 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/conversations.json
+-rwxr-xr-x   0        0        0      444 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/segments.json
+-rw-r--r--   0        0        0      205 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/tags.json
+-rw-r--r--   0        0        0      412 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/schemas/teams.json
+-rw-r--r--   0        0        0      477 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/source.py
+-rw-r--r--   0        0        0     2431 2024-03-23 07:06:10.000000 airbyte_source_intercom-0.6.3/source_intercom/spec.json
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 airbyte_source_intercom-0.6.3/PKG-INFO
```

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/README.md` & `airbyte_source_intercom-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/pyproject.toml` & `airbyte_source_intercom-0.6.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.6.2.dev202403211932"
+version = "0.6.3"
 name = "airbyte-source-intercom"
 description = "Source implementation for Intercom Yaml."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/components.py` & `airbyte_source_intercom-0.6.3/source_intercom/components.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 class IncrementalSingleSliceCursor(Cursor):
     cursor_field: Union[InterpolatedString, str]
     config: Config
     parameters: InitVar[Mapping[str, Any]]
 
     def __post_init__(self, parameters: Mapping[str, Any]):
         self._state = {}
+        self._cursor = None
         self.cursor_field = InterpolatedString.create(self.cursor_field, parameters=parameters)
 
     def get_request_params(
         self,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
@@ -83,20 +84,34 @@
 
     def set_initial_state(self, stream_state: StreamState):
         cursor_field = self.cursor_field.eval(self.config)
         cursor_value = stream_state.get(cursor_field)
         if cursor_value:
             self._state[cursor_field] = cursor_value
             self._state["prior_state"] = self._state.copy()
+            self._cursor = cursor_value
 
-    def close_slice(self, stream_slice: StreamSlice, most_recent_record: Optional[Record]) -> None:
-        latest_record = self._state if self.is_greater_than_or_equal(self._state, most_recent_record) else most_recent_record
-        if latest_record:
-            cursor_field = self.cursor_field.eval(self.config)
-            self._state[cursor_field] = latest_record[cursor_field]
+    def observe(self, stream_slice: StreamSlice, record: Record) -> None:
+        """
+        Register a record with the cursor; the cursor instance can then use it to manage the state of the in-progress stream read.
+
+        :param stream_slice: The current slice, which may or may not contain the most recently observed record
+        :param record: the most recently-read record, which the cursor can use to update the stream state. Outwardly-visible changes to the
+          stream state may need to be deferred depending on whether the source reliably orders records by the cursor field.
+        """
+        record_cursor_value = record.get(self.cursor_field.eval(self.config))
+        if not record_cursor_value:
+            return
+
+        if self.is_greater_than_or_equal(record, self._state):
+            self._cursor = record_cursor_value
+
+    def close_slice(self, stream_slice: StreamSlice) -> None:
+        cursor_field = self.cursor_field.eval(self.config)
+        self._state[cursor_field] = self._cursor
 
     def stream_slices(self) -> Iterable[Mapping[str, Any]]:
         yield StreamSlice(partition={}, cursor_slice={})
 
     def should_be_synced(self, record: Record) -> bool:
         """
         Evaluating if a record should be synced allows for filtering and stop condition on pagination
@@ -134,59 +149,94 @@
         self.parent_config: ParentStreamConfig = self.parent_stream_configs[0]
         self.parent_stream: Stream = self.parent_config.stream
         self.parent_stream_name: str = self.parent_stream.name
         self.parent_cursor_field: str = self.parent_stream.cursor_field
         self.parent_sync_mode: SyncMode = SyncMode.incremental if self.parent_stream.supports_incremental is True else SyncMode.full_refresh
         self.substream_slice_field: str = self.parent_stream_configs[0].partition_field.eval(self.config)
         self.parent_field: str = self.parent_stream_configs[0].parent_key.eval(self.config)
+        self._parent_cursor: Optional[str] = None
 
     def set_initial_state(self, stream_state: StreamState):
         super().set_initial_state(stream_state=stream_state)
         if self.parent_stream_name in stream_state and stream_state.get(self.parent_stream_name, {}).get(self.parent_cursor_field):
-            parent_stream_state = {self.parent_cursor_field: stream_state[self.parent_stream_name][self.parent_cursor_field]}
+            parent_stream_state = {
+                self.parent_cursor_field: stream_state[self.parent_stream_name][self.parent_cursor_field],
+            }
             self._state[self.parent_stream_name] = parent_stream_state
             if "prior_state" in self._state:
                 self._state["prior_state"][self.parent_stream_name] = parent_stream_state
 
-    def close_slice(self, stream_slice: StreamSlice, most_recent_record: Optional[Record]) -> None:
-        super().close_slice(stream_slice=stream_slice, most_recent_record=most_recent_record)
-        if self.parent_stream:
-            self._state[self.parent_stream_name] = self.parent_stream.state
+    def observe(self, stream_slice: StreamSlice, record: Record) -> None:
+        """
+        Extended the default method to be able to track the parent STATE.
+        """
+
+        # save parent cursor value (STATE) from slice
+        parent_cursor = stream_slice.get(self.parent_stream_name)
+        if parent_cursor:
+            self._parent_cursor = parent_cursor.get(self.parent_cursor_field)
+
+        # observe the substream
+        super().observe(stream_slice, record)
+
+    def close_slice(self, stream_slice: StreamSlice) -> None:
+        super().close_slice(stream_slice=stream_slice)
 
     def stream_slices(self) -> Iterable[Mapping[str, Any]]:
         parent_state = (self._state or {}).get(self.parent_stream_name, {})
         slices_generator: Iterable[StreamSlice] = self.read_parent_stream(self.parent_sync_mode, self.parent_cursor_field, parent_state)
         yield from [slice for slice in slices_generator] if self.parent_complete_fetch else slices_generator
 
+    def track_parent_cursor(self, parent_record: dict) -> None:
+        """
+        Tracks the Parent Stream Cursor, using `parent_cursor_field`.
+        """
+        self._parent_cursor = parent_record.get(self.parent_cursor_field)
+        if self._parent_cursor:
+            self._state[self.parent_stream_name] = {self.parent_cursor_field: self._parent_cursor}
+
     def read_parent_stream(
-        self, sync_mode: SyncMode, cursor_field: Optional[str], stream_state: Mapping[str, Any]
+        self,
+        sync_mode: SyncMode,
+        cursor_field: Optional[str],
+        stream_state: Mapping[str, Any],
     ) -> Iterable[Mapping[str, Any]]:
+
         self.parent_stream.state = stream_state
 
         parent_stream_slices_gen = self.parent_stream.stream_slices(
-            sync_mode=sync_mode, cursor_field=cursor_field, stream_state=stream_state
+            sync_mode=sync_mode,
+            cursor_field=cursor_field,
+            stream_state=stream_state,
         )
 
         for parent_slice in parent_stream_slices_gen:
             parent_records_gen = self.parent_stream.read_records(
-                sync_mode=sync_mode, cursor_field=cursor_field, stream_slice=parent_slice, stream_state=stream_state
+                sync_mode=sync_mode,
+                cursor_field=cursor_field,
+                stream_slice=parent_slice,
+                stream_state=stream_state,
             )
 
             for parent_record in parent_records_gen:
+                # update parent cursor
+                self.track_parent_cursor(parent_record)
                 substream_slice_value = parent_record.get(self.parent_field)
                 if substream_slice_value:
                     cursor_field = self.cursor_field.eval(self.config)
+                    substream_cursor_value = self._state.get(cursor_field)
+                    parent_cursor_value = self._state.get(self.parent_stream_name, {}).get(self.parent_cursor_field)
                     yield StreamSlice(
                         partition={
                             self.substream_slice_field: substream_slice_value,
                         },
                         cursor_slice={
-                            cursor_field: self._state.get(cursor_field),
+                            cursor_field: substream_cursor_value,
                             self.parent_stream_name: {
-                                self.parent_cursor_field: self._state.get(self.parent_stream_name, {}).get(self.parent_cursor_field)
+                                self.parent_cursor_field: parent_cursor_value,
                             },
                         },
                     )
 
 
 @dataclass
 class IntercomRateLimiter:
```

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/manifest.yaml` & `airbyte_source_intercom-0.6.3/source_intercom/manifest.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,17 @@
     class_name: source_intercom.components.HttpRequesterWithRateLimiter
     url_base: "https://api.intercom.io/"
     http_method: "GET"
     authenticator:
       type: BearerAuthenticator
       api_token: "{{ config['access_token'] }}"
     request_headers:
-      # API version header
-      # There are 404 - User Not Found issue, when `2.10` is used, for certain users:
-      # https://github.com/airbytehq/oncall/issues/4514
-      Intercom-Version: "'2.9'"
+      # There is a bug in interpolation, causing the `2.10` string to be evaluated to `2.1`, cutting off the `0`.
+      # the workaround is to put the `string` inside the `string`, then it's evaluated properly to `2.10`
+      Intercom-Version: "'2.10'"
       Accept: "application/json"
     error_handler:
       type: "DefaultErrorHandler"
   retriever:
     description: "Base Retriever for Full Refresh streams"
     record_selector:
       $ref: "#/definitions/selector"
@@ -290,14 +289,24 @@
     $ref: "#/definitions/stream_incremental_search"
     $parameters:
       name: "contacts"
       path: "contacts/search"
       page_size: 150
   conversations:
     $ref: "#/definitions/stream_incremental_search"
+    retriever:
+      $ref: "#/definitions/stream_incremental_search/retriever"
+      requester:
+        $ref: "#/definitions/requester_incremental_search"
+        request_headers:
+          # API version header
+          # There are 404 - User Not Found issue, when `2.10` is used, for certain users:
+          # https://github.com/airbytehq/oncall/issues/4514
+          Intercom-Version: "2.9"
+          Accept: "application/json"
     $parameters:
       name: "conversations"
       path: "conversations/search"
       data_field: "conversations"
       page_size: 150
 
   # activity logs stream is incremental based on created_at field
```

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/activity_logs.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/activity_logs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/admins.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/admins.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/companies.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/companies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/company_attributes.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/company_attributes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/contact_attributes.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/contact_attributes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/contacts.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/conversation_parts.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/conversation_parts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/schemas/conversations.json` & `airbyte_source_intercom-0.6.3/source_intercom/schemas/conversations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/source_intercom/spec.json` & `airbyte_source_intercom-0.6.3/source_intercom/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.2.dev202403211932/PKG-INFO` & `airbyte_source_intercom-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-intercom
-Version: 0.6.2.dev202403211932
+Version: 0.6.3
 Summary: Source implementation for Intercom Yaml.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

