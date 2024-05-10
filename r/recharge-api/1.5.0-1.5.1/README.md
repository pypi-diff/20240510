# Comparing `tmp/recharge_api-1.5.0.tar.gz` & `tmp/recharge_api-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recharge_api-1.5.0.tar", last modified: Wed May  1 13:04:48 2024, max compression
+gzip compressed data, was "recharge_api-1.5.1.tar", last modified: Thu May  9 13:31:45 2024, max compression
```

## Comparing `recharge_api-1.5.0.tar` & `recharge_api-1.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.223780 recharge_api-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-01 13:04:44.000000 recharge_api-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-01 13:04:48.223780 recharge_api-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 13:04:44.000000 recharge_api-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 13:04:44.000000 recharge_api-1.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.219780 recharge_api-1.5.0/recharge/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.219780 recharge_api-1.5.0/recharge/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.223780 recharge_api-1.5.0/recharge/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/async_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/checkouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/discounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/metafields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/onetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/products.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8728 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-01 13:04:44.000000 recharge_api-1.5.0/recharge/api/v1/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:04:48.223780 recharge_api-1.5.0/recharge_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 13:04:48.000000 recharge_api-1.5.0/recharge_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-01 13:04:48.227780 recharge_api-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.366180 recharge_api-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 13:31:41.000000 recharge_api-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-09 13:31:45.366180 recharge_api-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 13:31:41.000000 recharge_api-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 13:31:41.000000 recharge_api-1.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.362180 recharge_api-1.5.1/recharge/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.362180 recharge_api-1.5.1/recharge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.366180 recharge_api-1.5.1/recharge/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.366180 recharge_api-1.5.1/recharge_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 13:31:45.366180 recharge_api-1.5.1/setup.cfg
```

### Comparing `recharge_api-1.5.0/LICENSE` & `recharge_api-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/PKG-INFO` & `recharge_api-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recharge-api
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python API Wrapper for Recharge
 Home-page: http://github.com/ChemicalLuck/recharge-api
 Author: ChemicalLuck
 License: MIT
 Keywords: api recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `recharge_api-1.5.0/README.md` & `recharge_api-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/__init__.py` & `recharge_api-1.5.1/recharge/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/api/__init__.py` & `recharge_api-1.5.1/recharge/api/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/api/v1/__init__.py` & `recharge_api-1.5.1/recharge/api/v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from .shop import ShopResource
-from .products import ProductResource
-from .orders import OrderResource
-from .customers import CustomerResource
-from .checkouts import CheckoutResource
-from .tokens import TokenResource
-from .charges import ChargeResource
-from .webhooks import WebhookResource
-from .subscriptions import SubscriptionResource
-from .onetimes import OnetimeResource
 from .addresses import AddressResource
+from .charges import ChargeResource
+from .checkouts import CheckoutResource
+from .customers import CustomerResource
 from .discounts import DiscountResource
 from .metafields import MetafieldResource
-from .async_batches import AsyncBatchResource
 from .notifications import NotificationResource
+from .onetimes import OnetimeResource
+from .orders import OrderResource
+from .products import ProductResource
+from .shop import ShopResource
+from .subscriptions import SubscriptionResource
+from .webhooks import WebhookResource
+from .async_batches import AsyncBatchResource
+from .tokens import TokenResource
+
 
 __all__ = [
-    "ShopResource",
-    "ProductResource",
-    "OrderResource",
-    "CustomerResource",
-    "CheckoutResource",
-    "TokenResource",
-    "ChargeResource",
-    "WebhookResource",
-    "SubscriptionResource",
-    "OnetimeResource",
     "AddressResource",
+    "ChargeResource",
+    "CheckoutResource",
+    "CustomerResource",
     "DiscountResource",
     "MetafieldResource",
-    "AsyncBatchResource",
     "NotificationResource",
+    "OnetimeResource",
+    "OrderResource",
+    "ProductResource",
+    "ShopResource",
+    "SubscriptionResource",
+    "WebhookResource",
+    "AsyncBatchResource",
+    "TokenResource",
 ]
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/addresses.py` & `recharge_api-1.5.1/recharge/api/v1/addresses.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,43 +99,47 @@
     object_list_key = "addresses"
 
     def create(self, customer_id, body: AddressCreateBody):
         """Create an address for the customer.
         https://developer.rechargepayments.com/2021-01/addresses/create_address
         """
         required_scopes: list[RechargeScope] = ["write_customers"]
-        self.check_scopes("POST /customers/:customer_id/addresses", required_scopes)
+        self.check_scopes(
+            f"POST /customers/:customer_id/{self.object_list_key}", required_scopes
+        )
 
         url = f"{self.base_url}/customers/{customer_id}/{self.object_list_key}"
         return self._http_post(url, body)
 
     def get(self, address_id: str):
         """Get an address by ID.
         https://developer.rechargepayments.com/2021-01/addresses/retrieve_address
         """
         required_scopes: list[RechargeScope] = ["read_customers"]
-        self.check_scopes(f"GET {self.object_list_key}/:address_id", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/:address_id", required_scopes)
 
         return self._http_get(f"{self.url}/{address_id}")
 
     def update(self, address_id, body: AddressUpdateBody | None = None):
         """Update an address by ID.
         https://developer.rechargepayments.com/2021-01/addresses/update_address
         """
         required_scopes: list[RechargeScope] = ["write_customers"]
-        self.check_scopes(f"PUT {self.object_list_key}/:id", required_scopes)
+        self.check_scopes(f"PUT /{self.object_list_key}/:id", required_scopes)
 
         return self._http_put(f"{self.url}/{address_id}", body)
 
     def delete(self, address_id):
         """Delete an address by ID.
         https://developer.rechargepayments.com/2021-01/addresses/delete_address
         """
         required_scopes: list[RechargeScope] = ["write_customers"]
-        self.check_scopes(f"DELETE {self.object_list_key}/:address_id", required_scopes)
+        self.check_scopes(
+            f"DELETE /{self.object_list_key}/:address_id", required_scopes
+        )
 
         return self._http_delete(f"{self.url}/{address_id}")
 
     def list(self, customer_id, query: AddressListQuery | None = None):
         """List all addresses for a customer.
         https://developer.rechargepayments.com/2021-01/addresses/list_addresses
         """
@@ -149,15 +153,15 @@
         )
 
     def count(self, query: AddressCountQuery | None = None):
         """Retrieve the count of addresses.
         https://developer.rechargepayments.com/2021-01/addresses/count_addresses
         """
         required_scopes: list[RechargeScope] = ["read_customers"]
-        self.check_scopes("GET /addresses/count", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/count", required_scopes)
 
         return self._http_get(f"{self.url}/count", query)
 
     def validate(self, body: AddressValidateBody):
         """Validate an address.
         https://developer.rechargepayments.com/2021-01/addresses/validate_address
         """
@@ -169,21 +173,23 @@
         address_id,
         body: AddressApplyDiscountBody,
     ):
         """Apply a discount code to an address.
         https://developer.rechargepayments.com/2021-01/discounts/discounts_apply_address
         """
         required_scopes: list[RechargeScope] = ["write_discounts"]
-        self.check_scopes("POST /addresses/:address_id/apply_discount", required_scopes)
+        self.check_scopes(
+            f"POST /{self.object_list_key}/:address_id/apply_discount", required_scopes
+        )
 
         return self._http_post(f"{self.url}/{address_id}/apply_discount", body)
 
     def remove_discount(self, address_id: str):
         """Remove a discount from an address.
         https://developer.rechargepayments.com/2021-01/discounts/discounts_remove_from_address_or_charge
         """
         required_scopes: list[RechargeScope] = ["write_discounts"]
         self.check_scopes(
-            "POST /addresses/:address_id/remove_discount", required_scopes
+            f"POST /{self.object_list_key}/:address_id/remove_discount", required_scopes
         )
 
         return self._http_post(f"{self.url}/{address_id}/remove_discount")
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/async_batches.py` & `recharge_api-1.5.1/recharge/api/v1/async_batches.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     object_list_key = "async_batches"
 
     def create(self, body: AsyncBatchCreateBody):
         """Create an async batch.
         https://developer.rechargepayments.com/2021-01/async_batch_endpoints
         """
         required_scopes: list[RechargeScope] = ["write_batches"]
-        self.check_scopes("POST /async_batches", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
 
         return self._http_post(self.url, body)
 
     def create_task(self, batch_id, body: AsyncBatchCreateTaskBody):
         """Create a task for an async batch.
         https://developer.rechargepayments.com/2021-01/async_batch_endpoints
         """
@@ -86,24 +86,24 @@
         return self._http_post(f"{self.url}/{batch_id}/tasks", body)
 
     def get(self, batch_id):
         """Get an async batch.
         https://developer.rechargepayments.com/2021-01/async_batch_endpoints
         """
         required_scopes: list[RechargeScope] = ["read_batches"]
-        self.check_scopes("GET /async_batches/:batch_id", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/:batch_id", required_scopes)
 
         return self._http_get(f"{self.url}/{batch_id}")
 
     def list(self):
         """List async batches.
         https://developer.rechargepayments.com/2021-01/async_batch_endpoints
         """
         required_scopes: list[RechargeScope] = ["read_batches"]
-        self.check_scopes("GET /async_batches", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url)
 
     def list_tasks(
         self,
         batch_id,
     ):
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/charges.py` & `recharge_api-1.5.1/recharge/api/v1/charges.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,102 +56,115 @@
 
 
 class ChargeRefundBody(TypedDict, total=False):
     amount: Required[str]
     full_refund: bool
 
 
+class ChargeApplyDiscountCodeBody(TypedDict):
+    discount_code: str
+
+
+class ChargeApplyDiscountIdBody(TypedDict):
+    discount_id: str
+
+
+ChargeApplyDiscountBody: TypeAlias = (
+    ChargeApplyDiscountCodeBody | ChargeApplyDiscountIdBody
+)
+
+
 class ChargeResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/charges
     """
 
     object_list_key = "charges"
 
     def get(self, charge_id: str):
         """Get a charge by id.
         https://developer.rechargepayments.com/2021-01/charges/charge_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
-        self.check_scopes(f"GET {self.object_list_key}/:charge_id", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/:charge_id", required_scopes)
 
         return self._http_get(f"{self.url}/{charge_id}")
 
     def list(self, query: ChargeListQuery | None = None):
         """List charges.
         https://developer.rechargepayments.com/2021-01/charges/charge_list
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
-        self.check_scopes(f"GET {self.object_list_key}", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url, query)
 
     def count(self, query: ChargeCountQuery | None = None):
         """Count charges.
         https://developer.rechargepayments.com/2021-01/charges/charge_count
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
-        self.check_scopes(f"GET {self.object_list_key}/count", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/count", required_scopes)
 
         return self._http_get(f"{self.url}/count", query)
 
     def change_next_charge_date(
         self, charge_id: str, body: ChargeChangeNextChargeDateBody
     ):
         """Change the date of a queued charge.
         https://developer.rechargepayments.com/2021-01/charges/charge_change_next_date
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
         self.check_scopes(
-            f"POST {self.object_list_key}/:charge_id/change_next_charge_date",
+            f"POST /{self.object_list_key}/:charge_id/change_next_charge_date",
             required_scopes,
         )
 
         return self._http_put(f"{self.url}/{charge_id}/change_next_charge_date", body)
 
     def skip(self, charge_id: str, body: ChargeSkipBody):
         """Skip a charge.
         https://developer.rechargepayments.com/2021-01/charges/charge_skip
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
         self.check_scopes(
-            f"POST {self.object_list_key}/:charge_id/skip", required_scopes
+            f"POST /{self.object_list_key}/:charge_id/skip", required_scopes
         )
 
         return self._http_post(f"{self.url}/{charge_id}/skip", body)
 
     def unskip(self, charge_id: str, body: ChargeSkipBody):
         """Unskip a charge.
         https://developer.rechargepayments.com/2021-01/charges/charge_unskip
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
         self.check_scopes(
-            f"POST {self.object_list_key}/:charge_id/unskip", required_scopes
+            f"POST /{self.object_list_key}/:charge_id/unskip", required_scopes
         )
 
         return self._http_post(f"{self.url}/{charge_id}/unskip", body)
 
     def refund(self, charge_id: str, body: ChargeRefundBody):
         """Refund a charge.
         https://developer.rechargepayments.com/2021-01/charges/charge_refund
         """
         required_scopes: list[RechargeScope] = ["write_orders", "write_payments"]
         self.check_scopes(
-            f"POST {self.object_list_key}/:charge_id/refund", required_scopes
+            f"POST /{self.object_list_key}/:charge_id/refund", required_scopes
         )
 
         return self._http_post(f"{self.url}/{charge_id}/refund", body)
 
     def process(self, charge_id: str):
         """Process a charge.
         https://developer.rechargepayments.com/2021-01/charges/charge_process
         """
         required_scopes: list[RechargeScope] = ["write_payments"]
         self.check_scopes(
-            f"POST {self.object_list_key}/:charge_id/process", required_scopes
+            f"POST /{self.object_list_key}/:charge_id/process", required_scopes
         )
 
         return self._http_post(f"{self.url}/{charge_id}/process", None)
 
     def capture(self, charge_id: str):
         """Capture a charge.
         https://developer.rechargepayments.com/2021-01/charges/charge_capture
@@ -159,11 +172,33 @@
         required_scopes: list[RechargeScope] = [
             "write_orders",
             "write_payments",
             "write_subscriptions",
             "write_customers",
         ]
         self.check_scopes(
-            f"POST {self.object_list_key}/:charge_id/capture", required_scopes
+            f"POST /{self.object_list_key}/:charge_id/capture", required_scopes
         )
 
         return self._http_post(f"{self.url}/{charge_id}/capture_payment", None)
+
+    def apply_discount(self, charge_id: str, body: ChargeApplyDiscountBody):
+        """Apply a discount to a charge.
+        https://developer.rechargepayments.com/2021-01/charges/charge_apply_discount
+        """
+        required_scopes: list[RechargeScope] = ["write_orders"]
+        self.check_scopes(
+            f"POST /{self.object_list_key}/:charge_id/apply_discount", required_scopes
+        )
+
+        return self._http_post(f"{self.url}/{charge_id}/apply_discount", body)
+
+    def remove_discount(self, charge_id: str):
+        """Remove a discount from a charge.
+        https://developer.rechargepayments.com/2021-01/charges/charge_remove_discount
+        """
+        required_scopes: list[RechargeScope] = ["write_orders"]
+        self.check_scopes(
+            f"POST /{self.object_list_key}/:charge_id/remove_discount", required_scopes
+        )
+
+        return self._http_post(f"{self.url}/{charge_id}/remove_discount")
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/checkouts.py` & `recharge_api-1.5.1/recharge/api/v1/checkouts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/api/v1/customers.py` & `recharge_api-1.5.1/recharge/api/v1/customers.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/api/v1/discounts.py` & `recharge_api-1.5.1/recharge/api/v1/discounts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/api/v1/metafields.py` & `recharge_api-1.5.1/recharge/api/v1/metafields.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/api/v1/notifications.py` & `recharge_api-1.5.1/recharge/api/v1/notifications.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,12 @@
 
     def send_email(self, customer_id, body: NotificationSendEmailBody):
         """
         Send an email notification to a customer.
         https://developer.rechargepayments.com/2021-01/notifications/notifications_get_account_access
         """
         required_scopes: list[RechargeScope] = ["write_notifications"]
-        self.check_scopes(
-            f"POST /customers/{customer_id}/notifications", required_scopes
-        )
+        self.check_scopes("POST /customers/:customer_id/notifications", required_scopes)
 
         return self._http_post(
             f"{self.url}/customers/{customer_id}/notifications", body
         )
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/onetimes.py` & `recharge_api-1.5.1/recharge/api/v1/onetimes.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,46 +54,48 @@
     object_list_key = "onetimes"
 
     def create(self, body: OnetimeCreateBody):
         """Create a Onetime
         https://developer.rechargepayments.com/2021-01/onetimes/onetimes_create
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("POST /onetimes", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
 
         return self._http_post(self.url, body)
 
     def get(self, onetime_id: str):
         """Get a Onetime
         https://developer.rechargepayments.com/2021-01/onetimes/onetimes_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_subscriptions"]
-        self.check_scopes("GET /onetimes/:onetime_id", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/:onetime_id", required_scopes)
 
         return self._http_get(f"{self.url}/{onetime_id}")
 
     def update(self, onetime_id: str, body: OnetimeUpdateBody):
         """Update a Onetime
         https://developer.rechargepayments.com/2021-01/onetimes/onetimes_update
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("PUT /onetimes/:onetime_id", required_scopes)
+        self.check_scopes(f"PUT /{self.object_list_key}/:onetime_id", required_scopes)
 
         return self._http_put(f"{self.url}/{onetime_id}", body)
 
     def delete(self, onetime_id: str):
         """Delete a Onetime.
         https://developer.rechargepayments.com/2021-01/onetimes/onetimes_delete
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("DELETE /onetimes/:onetime_id", required_scopes)
+        self.check_scopes(
+            f"DELETE /{self.object_list_key}/:onetime_id", required_scopes
+        )
 
         return self._http_delete(f"{self.url}/{onetime_id}")
 
     def list(self, query: OnetimeListQuery):
         """List Onetimes.
         https://developer.rechargepayments.com/2021-01/onetimes/onetimes_list
         """
         required_scopes: list[RechargeScope] = ["read_subscriptions"]
-        self.check_scopes("GET /onetimes", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url, query)
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/orders.py` & `recharge_api-1.5.1/recharge/api/v1/orders.py`

 * *Files 19% similar despite different names*

```diff
@@ -99,95 +99,101 @@
     object_list_key = "orders"
 
     def get(self, order_id: str):
         """Get an order.
         https://developer.rechargepayments.com/2021-01/orders/orders_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
-        self.check_scopes(f"GET /orders/{order_id}", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/:order_id", required_scopes)
 
         return self._http_get(f"{self.url}/{order_id}")
 
     def update(self, order_id: str, body: OrderUpdateBody):
         """Update an order.
         https://developer.rechargepayments.com/2021-01/orders/orders_update
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
-        self.check_scopes(f"PUT /orders/{order_id}", required_scopes)
+        self.check_scopes(f"PUT /{self.object_list_key}/:order_id", required_scopes)
 
         return self._http_put(f"{self.url}/{order_id}", body)
 
     def delete(self, order_id: str):
         """Delete an order.
         https://developer.rechargepayments.com/2021-01/orders/orders_delete
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
-        self.check_scopes(f"DELETE /orders/{order_id}", required_scopes)
+        self.check_scopes(f"DELETE /{self.object_list_key}/:order_id", required_scopes)
 
         return self._http_delete(f"{self.url}/{order_id}")
 
     def list(self, query: OrderListQuery):
         """List orders.
         https://developer.rechargepayments.com/2021-01/orders/orders_list
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
-        self.check_scopes("GET /orders", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url, query)
 
     def count(self, query: OrderCountQuery):
         """Count orders.
         https://developer.rechargepayments.com/2021-01/orders/orders_count
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
-        self.check_scopes("GET /orders/count", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/count", required_scopes)
 
         return self._http_get(f"{self.url}/count", query)
 
     def change_date(self, order_id: str, body: OrderChangeDateBody):
         """Change the date of a queued order.
         https://developer.rechargepayments.com/2021-01/orders/orders_change_date
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
-        self.check_scopes("POST /orders/:order_id/change_date", required_scopes)
+        self.check_scopes(
+            f"POST /{self.object_list_key}/:order_id/change_date", required_scopes
+        )
 
         return self._http_post(
             f"{self.url}/{order_id}/change_date",
             body,
         )
 
     def change_variant(
         self, order_id: str, old_variant_id: str, body: OrderChangeVariantBody
     ):
         """Change an order variant.
         https://developer.rechargepayments.com/v1#change-an-order-variant
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
         self.check_scopes(
-            "PUT /orders/:order_id/update_shopify_variant/:old_variant_id",
+            f"PUT /{self.object_list_key}/:order_id/update_shopify_variant/:old_variant_id",
             required_scopes,
         )
 
         return self._http_put(
             f"{self.url}/{order_id}/update_shopify_variant/{old_variant_id}", body
         )
 
     def clone(self, order_id: str, charge_id: str, body: OrderCloneBody):
         """Clone an order.
         https://developer.rechargepayments.com/2021-01/orders/orders_clone
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
-        self.check_scopes("POST /orders/:order_id/clone", required_scopes)
+        self.check_scopes(
+            f"POST /{self.object_list_key}/:order_id/clone", required_scopes
+        )
 
         return self._http_post(
             f"{self.url}/clone_order_on_success_charge/{order_id}/charge/{charge_id}",
             body,
         )
 
     def delay(self, order_id: str):
         """Delay an order.
         https://developer.rechargepayments.com/2021-01/orders/orders_delay
         """
         required_scopes: list[RechargeScope] = ["write_orders"]
-        self.check_scopes("POST /orders/:order_id/delay", required_scopes)
+        self.check_scopes(
+            f"POST /{self.object_list_key}/:order_id/delay", required_scopes
+        )
 
         return self._http_post(f"{self.url}/{order_id}/delay", None)
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/products.py` & `recharge_api-1.5.1/recharge/api/v1/products.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,55 +90,57 @@
     object_list_key = "products"
 
     def create(self, body: ProductCreateBody):
         """Create a product.
         https://developer.rechargepayments.com/2021-01/products/products_create
         """
         required_scopes: list[RechargeScope] = ["write_products"]
-        self.check_scopes("POST /products", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
 
         return self._http_post(self.url, body)
 
     def get(self, product_id: str):
         """Get a product.
         https://developer.rechargepayments.com/2021-01/products/products_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_products"]
-        self.check_scopes(f"GET /products/{product_id}", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/:product_id", required_scopes)
 
         return self._http_get(f"{self.url}/{product_id}")
 
     def update(self, product_id: str, body: ProductUpdateBody):
         """Update a product.
         https://developer.rechargepayments.com/2021-01/products/products_update
         """
         required_scopes: list[RechargeScope] = ["write_products"]
-        self.check_scopes(f"PUT /products/{product_id}", required_scopes)
+        self.check_scopes(f"PUT /{self.object_list_key}/:product_id", required_scopes)
 
         return self._http_put(f"{self.url}/{product_id}", body)
 
     def delete(self, product_id: str):
         """Delete a product.
         https://developer.rechargepayments.com/2021-01/products/products_delete
         """
         required_scopes: list[RechargeScope] = ["write_products"]
-        self.check_scopes(f"DELETE /products/{product_id}", required_scopes)
+        self.check_scopes(
+            f"DELETE /{self.object_list_key}/:product_id", required_scopes
+        )
 
         return self._http_delete(f"{self.url}/{product_id}")
 
     def list(self, query: ProductListQuery):
         """List products.
         https://developer.rechargepayments.com/2021-01/products/products_list
         """
         required_scopes: list[RechargeScope] = ["read_products"]
-        self.check_scopes("GET /products", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url, query)
 
     def count(self):
         """Count products.
         https://developer.rechargepayments.com/2021-01/products/products_count
         """
         required_scopes: list[RechargeScope] = ["read_products"]
-        self.check_scopes("GET /products/count", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/count", required_scopes)
 
         return self._http_get(f"{self.url}/count")
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/shop.py` & `recharge_api-1.5.1/recharge/api/v1/shop.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     object_list_key = "shop"
 
     def get(self):
         """Retrieve store using the Recharge API.
         https://developer.rechargepayments.com/2021-01/shop/shop_retrieve
         """
         required_scopes: list[RechargeScope] = ["store_info"]
-        self.check_scopes("GET /shop", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(f"{self.url}")
 
     def shipping_countries(self):
         """Retrieve shipping countries where items can be shipped.
         https://developer.rechargepayments.com/2021-01/shop/shop_shipping_countries
         """
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/subscriptions.py` & `recharge_api-1.5.1/recharge/api/v1/subscriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,126 +125,134 @@
     object_list_key = "subscriptions"
 
     def create(self, body: SubscriptionCreateBody):
         """Create a subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_create
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("POST /subscriptions", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
 
         return self._http_post(self.url, body)
 
     def get(self, subscription_id: str):
         """Get a subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_subscriptions"]
-        self.check_scopes("GET /subscriptions/:subscription_id", required_scopes)
+        self.check_scopes(
+            f"GET /{self.object_list_key}/:subscription_id", required_scopes
+        )
 
         return self._http_get(f"{self.url}/{subscription_id}")
 
     def update(self, subscription_id: str, body: SubscriptionUpdateBody):
         """Update a subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_update
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("PUT /subscriptions/:subscription_id", required_scopes)
+        self.check_scopes(
+            f"PUT /{self.object_list_key}/:subscription_id", required_scopes
+        )
 
         return self._http_put(f"{self.url}/{subscription_id}", body)
 
     def delete(self, subscription_id: str, body: SubscriptionDeleteBody):
         """Delete a subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_delete
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("DELETE /subscriptions/:subscription_id", required_scopes)
+        self.check_scopes(
+            f"DELETE /{self.object_list_key}/:subscription_id", required_scopes
+        )
 
         return self._http_delete(f"{self.url}/{subscription_id}", body)
 
     def list(self, query: SubscriptionListQuery):
         """List subscriptions.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_list
         """
         required_scopes: list[RechargeScope] = ["read_subscriptions"]
-        self.check_scopes("GET /subscriptions", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url, query)
 
     def count(self, query: SubscriptionCountQuery):
         """Count subscriptions.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_count
         """
         required_scopes: list[RechargeScope] = ["read_subscriptions"]
-        self.check_scopes("GET /subscriptions/count", required_scopes)
+        self.check_scopes(f"GET /{self.object_list_key}/count", required_scopes)
 
         return self._http_get(f"{self.url}/count", query)
 
     def change_date(self, subscription_id: str, body: SubscriptionChangeDateBody):
         """Change the date of a queued subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_change_date
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(
-            "POST /subscriptions/:subscription_id/change_date", required_scopes
+            f"POST /{self.object_list_key}/:subscription_id/change_date",
+            required_scopes,
         )
 
         return self._http_post(f"{self.url}/{subscription_id}/change_date", body)
 
     def change_address(self, subscription_id: str, body: SubscriptionChangeAddressBody):
         """Change the address of a subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_change_address
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(
-            "POST /subscriptions/:subscription_id/change_address", required_scopes
+            f"POST /{self.object_list_key}/:subscription_id/change_address",
+            required_scopes,
         )
 
         return self._http_post(f"{self.url}/{subscription_id}/change_address", body)
 
     def cancel(self, subscription_id: str):
         """Cancel a subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_cancel
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(
-            "POST /subscriptions/:subscription_id/cancel", required_scopes
+            f"POST /{self.object_list_key}/:subscription_id/cancel", required_scopes
         )
 
         return self._http_post(f"{self.url}/{subscription_id}/cancel", {})
 
     def activate(self, subscription_id: str):
         """Activate a cancelled subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_activate
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(
-            "POST /subscriptions/:subscription_id/activate", required_scopes
+            f"POST /{self.object_list_key}/:subscription_id/activate", required_scopes
         )
 
         return self._http_post(f"{self.url}/{subscription_id}/activate", {})
 
     def bulk_create(self, body: SubscriptionBulkCreateBody):
         """Bulk create subscriptions.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_bulk_create
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("POST /subscriptions/bulk_create", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}/bulk_create", required_scopes)
 
         return self._http_post(f"{self.url}/bulk_create", body)
 
     def bulk_update(self, body: SubscriptionBulkUpdateBody):
         """Bulk update subscriptions.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_bulk_update
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("POST /subscriptions/bulk_update", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}/bulk_update", required_scopes)
 
         return self._http_post(f"{self.url}/bulk_update", body)
 
     def bulk_delete(self, body: SubscriptionBulkDeleteBody):
         """Bulk delete subscriptions.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_bulk_delete
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
-        self.check_scopes("POST /subscriptions/bulk_delete", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}/bulk_delete", required_scopes)
 
         return self._http_post(f"{self.url}/bulk_delete", body)
```

### Comparing `recharge_api-1.5.0/recharge/api/v1/tokens.py` & `recharge_api-1.5.1/recharge/api/v1/tokens.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/recharge/api/v1/webhooks.py` & `recharge_api-1.5.1/recharge/api/v1/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def create(self, body: WebhookCreateBody):
         """Create a webhook.
         https://developer.rechargepayments.com/2021-01/webhooks_endpoints/webhooks_create
         """
         resource = body["topic"].split("/")[0]
         required_scopes: list[RechargeScope] = [WebhookTopicMap[resource]]
-        self.check_scopes("POST /webhooks", required_scopes)
+        self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
 
         return self._http_post(self.url, body)
 
     def get(self, webhook_id: str):
         """Get a webhook.
         https://developer.rechargepayments.com/2021-01/webhooks_endpoints/webhooks_retrieve
         """
```

### Comparing `recharge_api-1.5.0/recharge_api.egg-info/PKG-INFO` & `recharge_api-1.5.1/recharge_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recharge-api
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python API Wrapper for Recharge
 Home-page: http://github.com/ChemicalLuck/recharge-api
 Author: ChemicalLuck
 License: MIT
 Keywords: api recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `recharge_api-1.5.0/recharge_api.egg-info/SOURCES.txt` & `recharge_api-1.5.1/recharge_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.0/setup.cfg` & `recharge_api-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = recharge-api
-version = 1.5.0
+version = 1.5.1
 author = ChemicalLuck
 description = Python API Wrapper for Recharge
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/ChemicalLuck/recharge-api
 license = MIT
 keywords = api recharge
```

