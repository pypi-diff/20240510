# Comparing `tmp/airbyte_source_chargebee-0.4.2.tar.gz` & `tmp/airbyte_source_chargebee-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_chargebee-0.4.2.tar", max compression
+gzip compressed data, was "airbyte_source_chargebee-0.5.0.tar", max compression
```

## Comparing `airbyte_source_chargebee-0.4.2.tar` & `airbyte_source_chargebee-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     4555 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/README.md
--rw-r--r--   0        0        0      783 2024-03-14 16:25:04.246597 airbyte_source_chargebee-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      130 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/__init__.py
--rw-r--r--   0        0        0     5731 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/components.py
--rw-r--r--   0        0        0    14973 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/manifest.yaml
--rw-r--r--   0        0        0      239 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/run.py
--rw-r--r--   0        0        0     3501 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/addon.json
--rw-r--r--   0        0        0     1068 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/attached_item.json
--rw-r--r--   0        0        0      669 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/comment.json
--rw-r--r--   0        0        0      863 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/contact.json
--rw-r--r--   0        0        0     2998 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/coupon.json
--rw-r--r--   0        0        0    12322 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/credit_note.json
--rw-r--r--   0        0        0     9383 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/customer.json
--rw-r--r--   0        0        0     1694 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/differential_price.json
--rw-r--r--   0        0        0     1037 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/event.json
--rw-r--r--   0        0        0     2097 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/gift.json
--rw-r--r--   0        0        0     1048 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/hosted_page.json
--rw-r--r--   0        0        0    17602 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/invoice.json
--rw-r--r--   0        0        0     1941 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/item.json
--rw-r--r--   0        0        0      683 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/item_family.json
--rw-r--r--   0        0        0     3836 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/item_price.json
--rw-r--r--   0        0        0    10496 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/order.json
--rw-r--r--   0        0        0     4176 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/payment_source.json
--rw-r--r--   0        0        0     5440 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/plan.json
--rw-r--r--   0        0        0      995 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/promotional_credit.json
--rw-r--r--   0        0        0    10376 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/quote.json
--rw-r--r--   0        0        0     5935 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/quote_line_group.json
--rw-r--r--   0        0        0      328 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/shared/_definitions.json
--rw-r--r--   0        0        0      659 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/site_migration_detail.json
--rw-r--r--   0        0        0    14400 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/subscription.json
--rw-r--r--   0        0        0     5111 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/transaction.json
--rw-r--r--   0        0        0     2364 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/unbilled_charge.json
--rw-r--r--   0        0        0     1051 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/schemas/virtual_bank_account.json
--rw-r--r--   0        0        0      478 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/source.py
--rw-r--r--   0        0        0     1474 2024-03-14 15:28:03.000000 airbyte_source_chargebee-0.4.2/source_chargebee/spec.yaml
--rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 airbyte_source_chargebee-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     4555 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/README.md
+-rw-r--r--   0        0        0      778 2024-04-10 14:44:33.437692 airbyte_source_chargebee-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/__init__.py
+-rw-r--r--   0        0        0     6477 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/components.py
+-rw-r--r--   0        0        0    14973 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/run.py
+-rw-r--r--   0        0        0     3501 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/addon.json
+-rw-r--r--   0        0        0     1068 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/attached_item.json
+-rw-r--r--   0        0        0      669 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/comment.json
+-rw-r--r--   0        0        0      863 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/contact.json
+-rw-r--r--   0        0        0     2998 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/coupon.json
+-rw-r--r--   0        0        0    12322 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/credit_note.json
+-rw-r--r--   0        0        0     9383 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/customer.json
+-rw-r--r--   0        0        0     1694 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/differential_price.json
+-rw-r--r--   0        0        0     1037 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/event.json
+-rw-r--r--   0        0        0     2097 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/gift.json
+-rw-r--r--   0        0        0     1048 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/hosted_page.json
+-rw-r--r--   0        0        0    17602 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/invoice.json
+-rw-r--r--   0        0        0     1941 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/item.json
+-rw-r--r--   0        0        0      683 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/item_family.json
+-rw-r--r--   0        0        0     3836 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/item_price.json
+-rw-r--r--   0        0        0    10496 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/order.json
+-rw-r--r--   0        0        0     4176 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/payment_source.json
+-rw-r--r--   0        0        0     5440 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/plan.json
+-rw-r--r--   0        0        0      995 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/promotional_credit.json
+-rw-r--r--   0        0        0    10376 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/quote.json
+-rw-r--r--   0        0        0     5935 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/quote_line_group.json
+-rw-r--r--   0        0        0      328 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/shared/_definitions.json
+-rw-r--r--   0        0        0      659 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/site_migration_detail.json
+-rw-r--r--   0        0        0    14400 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/subscription.json
+-rw-r--r--   0        0        0     5111 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/transaction.json
+-rw-r--r--   0        0        0     2364 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/unbilled_charge.json
+-rw-r--r--   0        0        0     1051 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/schemas/virtual_bank_account.json
+-rw-r--r--   0        0        0      478 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/source.py
+-rw-r--r--   0        0        0     1474 2024-04-10 14:41:26.126114 airbyte_source_chargebee-0.5.0/source_chargebee/spec.yaml
+-rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 airbyte_source_chargebee-0.5.0/PKG-INFO
```

### Comparing `airbyte_source_chargebee-0.4.2/README.md` & `airbyte_source_chargebee-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/pyproject.toml` & `airbyte_source_chargebee-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.4.2"
+version = "0.5.0"
 name = "airbyte-source-chargebee"
 description = "Source implementation for Chargebee."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,17 +18,17 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_chargebee" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0.67.1"
-freezegun = "^1.4.0"
+airbyte-cdk = "^0"
 
 [tool.poetry.scripts]
 source-chargebee = "source_chargebee.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6.1"
 pytest = "^6.2"
+freezegun = "^1.4.0"
```

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/components.py` & `airbyte_source_chargebee-0.5.0/source_chargebee/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,20 +49,22 @@
         """
         record["custom_fields"] = [{"name": k, "value": record.pop(k)} for k in record.copy() if k.startswith("cf_")]
         return record
 
 
 @dataclass
 class IncrementalSingleSliceCursor(Cursor):
+
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
@@ -109,23 +111,37 @@
 
     def set_initial_state(self, stream_state: StreamState):
         cursor_field = self.cursor_field.eval(self.config)
         cursor_value = stream_state.get(cursor_field)
         if cursor_value:
             self._state[cursor_field] = cursor_value
             self._state["prior_state"] = self._state.copy()
+            self._cursor = cursor_value
+
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
 
-    def close_slice(self, stream_slice: StreamSlice, most_recent_record: Optional[Record]) -> None:
-        latest_record = self._state if self.is_greater_than_or_equal(self._state, most_recent_record) else most_recent_record
-        if latest_record:
-            cursor_field = self.cursor_field.eval(self.config)
-            self._state[cursor_field] = latest_record[cursor_field]
+        if self.is_greater_than_or_equal(record, self._state):
+            self._cursor = record_cursor_value
+
+    def close_slice(self, stream_slice: StreamSlice) -> None:
+        cursor_field = self.cursor_field.eval(self.config)
+        self._state[cursor_field] = self._cursor
 
     def stream_slices(self) -> Iterable[Mapping[str, Any]]:
-        yield {}
+        yield StreamSlice(partition={}, cursor_slice={})
 
     def should_be_synced(self, record: Record) -> bool:
         """
         Evaluating if a record should be synced allows for filtering and stop condition on pagination
         """
         record_cursor_value = record.get(self.cursor_field.eval(self.config))
         return bool(record_cursor_value)
```

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/manifest.yaml` & `airbyte_source_chargebee-0.5.0/source_chargebee/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/addon.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/addon.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/attached_item.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/attached_item.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/comment.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/comment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/contact.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/contact.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/coupon.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/coupon.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/credit_note.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/credit_note.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/customer.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/customer.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/differential_price.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/differential_price.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/event.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/event.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/gift.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/gift.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/hosted_page.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/hosted_page.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/invoice.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/invoice.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/item.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/item.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/item_family.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/item_family.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/item_price.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/item_price.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/order.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/order.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/payment_source.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/payment_source.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/plan.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/plan.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/promotional_credit.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/promotional_credit.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/quote.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/quote.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/quote_line_group.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/quote_line_group.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/site_migration_detail.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/site_migration_detail.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/subscription.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/subscription.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/transaction.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/transaction.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/unbilled_charge.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/unbilled_charge.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/schemas/virtual_bank_account.json` & `airbyte_source_chargebee-0.5.0/source_chargebee/schemas/virtual_bank_account.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/source_chargebee/spec.yaml` & `airbyte_source_chargebee-0.5.0/source_chargebee/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.4.2/PKG-INFO` & `airbyte_source_chargebee-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-chargebee
-Version: 0.4.2
+Version: 0.5.0
 Summary: Source implementation for Chargebee.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0.67.1,<0.68.0)
-Requires-Dist: freezegun (>=1.4.0,<2.0.0)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/chargebee
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Chargebee source connector
```

