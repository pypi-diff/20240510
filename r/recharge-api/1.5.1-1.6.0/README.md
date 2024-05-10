# Comparing `tmp/recharge_api-1.5.1.tar.gz` & `tmp/recharge_api-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recharge_api-1.5.1.tar", last modified: Thu May  9 13:31:45 2024, max compression
+gzip compressed data, was "recharge_api-1.6.0.tar", last modified: Fri May 10 08:22:20 2024, max compression
```

## Comparing `recharge_api-1.5.1.tar` & `recharge_api-1.6.0.tar`

### file list

```diff
@@ -1,34 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.366180 recharge_api-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 13:31:41.000000 recharge_api-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-09 13:31:45.366180 recharge_api-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 13:31:41.000000 recharge_api-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 13:31:41.000000 recharge_api-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.362180 recharge_api-1.5.1/recharge/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.362180 recharge_api-1.5.1/recharge/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.366180 recharge_api-1.5.1/recharge/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/async_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/checkouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/discounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/metafields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/onetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/products.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-09 13:31:41.000000 recharge_api-1.5.1/recharge/api/v1/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:31:45.366180 recharge_api-1.5.1/recharge_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:31:45.000000 recharge_api-1.5.1/recharge_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 13:31:45.366180 recharge_api-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.456666 recharge_api-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-10 08:22:13.000000 recharge_api-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 08:22:20.456666 recharge_api-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-10 08:22:13.000000 recharge_api-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 08:22:13.000000 recharge_api-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.444666 recharge_api-1.6.0/recharge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.444666 recharge_api-1.6.0/recharge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.448666 recharge_api-1.6.0/recharge/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.452666 recharge_api-1.6.0/recharge/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/bundle_selections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/retention_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.456666 recharge_api-1.6.0/recharge_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 08:22:20.456666 recharge_api-1.6.0/setup.cfg
```

### Comparing `recharge_api-1.5.1/LICENSE` & `recharge_api-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/PKG-INFO` & `recharge_api-1.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recharge-api
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python API Wrapper for Recharge
 Home-page: http://github.com/ChemicalLuck/recharge-api
 Author: ChemicalLuck
 License: MIT
 Keywords: api recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
@@ -30,36 +30,59 @@
 ## Usage
 
 ```python
 from recharge import RechargeAPI
 
 client = Recharge(access_token='XXXXX')
 
-response = client.Order.list({'status': 'QUEUED', 'limit': '250'})
+response = client.v1.Order.list({'status': 'QUEUED', 'limit': '250'})
 
 for order in response['orders']:
     print(order['id'])
 ```
 
 For more details on the content of the reponses, visit the (official recharge API docs)[https://developer.rechargepayments.com].
 
 ## Resources Available
-- Addresses
-- Charges
-- Checkouts
-- Customers
-- Discounts
-- Metafields
-- Notifications
-- Onetimes
-- Orders
-- Products
+### v1(2021-01)
+- Address
+- Charge
+- Checkout
+- Customer
+- Discount
+- Metafield
+- Notification
+- Onetime
+- Order
+- Product
 - Shop
-- Subscriptions
-- Webhooks
-- Async Batches
+- Subscription
+- Webhook
+- Async Batch
+### v2(2021-11)
+- Address
+- BundleSelection
+- Charge
+- Checkout
+- Collection
+- Customer
+- Discount
+- Metafield
+- Notification
+- Onetime
+- Order
+- Payment Method
+- Plan
+- Retention Strategy
+- Subscription
+- Webhook
+- Async Batch
+- Token
+- Account
+- Event
+- Store
 
 ## License
 MIT. See LICENSE for more details.
 
 ## Acknowledgements
 This project is a fork of recharge-api by BuluBox which is no longer available.
```

### Comparing `recharge_api-1.5.1/recharge/api/__init__.py` & `recharge_api-1.6.0/recharge/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "read_events",
     "write_retention_strategies",
     "read_gift_purchases",
     "write_gift_purchases",
     "read_gift_purchases",
     "write_gift_purchases",
     "read_bundle_products",
+    "read_credit_summary",
 ]
 
 log = logging.getLogger(__name__)
 
 
 class RechargeResource(object):
     """
@@ -49,17 +50,17 @@
     """
 
     base_url = "https://api.rechargeapps.com"
     object_list_key = None
 
     def __init__(
         self,
-        access_token=None,
-        debug=False,
-        scopes: list[RechargeScope] | None = None,
+        access_token,
+        debug,
+        scopes: list[RechargeScope],
     ):
         self.headers = {
             "Accept": "application/json",
             "Content-Type": "application/json",
             "X-Recharge-Access-Token": access_token,
         }
         self.debug = debug
```

### Comparing `recharge_api-1.5.1/recharge/api/v1/__init__.py` & `recharge_api-1.6.0/recharge/api/v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .shop import ShopResource
 from .subscriptions import SubscriptionResource
 from .webhooks import WebhookResource
 from .async_batches import AsyncBatchResource
 from .tokens import TokenResource
 
 
+
 __all__ = [
     "AddressResource",
     "ChargeResource",
     "CheckoutResource",
     "CustomerResource",
     "DiscountResource",
     "MetafieldResource",
```

### Comparing `recharge_api-1.5.1/recharge/api/v1/addresses.py` & `recharge_api-1.6.0/recharge/api/v1/addresses.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/async_batches.py` & `recharge_api-1.6.0/recharge/api/v1/async_batches.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/charges.py` & `recharge_api-1.6.0/recharge/api/v1/charges.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/checkouts.py` & `recharge_api-1.6.0/recharge/api/v1/checkouts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/customers.py` & `recharge_api-1.6.0/recharge/api/v1/customers.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/discounts.py` & `recharge_api-1.6.0/recharge/api/v1/discounts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/metafields.py` & `recharge_api-1.6.0/recharge/api/v1/metafields.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/notifications.py` & `recharge_api-1.6.0/recharge/api/v1/notifications.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/onetimes.py` & `recharge_api-1.6.0/recharge/api/v1/onetimes.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/orders.py` & `recharge_api-1.6.0/recharge/api/v1/orders.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/products.py` & `recharge_api-1.6.0/recharge/api/v1/products.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/shop.py` & `recharge_api-1.6.0/recharge/api/v1/shop.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/subscriptions.py` & `recharge_api-1.6.0/recharge/api/v1/subscriptions.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/tokens.py` & `recharge_api-1.6.0/recharge/api/v1/tokens.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge/api/v1/webhooks.py` & `recharge_api-1.6.0/recharge/api/v1/webhooks.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.5.1/recharge_api.egg-info/PKG-INFO` & `recharge_api-1.6.0/recharge_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recharge-api
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python API Wrapper for Recharge
 Home-page: http://github.com/ChemicalLuck/recharge-api
 Author: ChemicalLuck
 License: MIT
 Keywords: api recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
@@ -30,36 +30,59 @@
 ## Usage
 
 ```python
 from recharge import RechargeAPI
 
 client = Recharge(access_token='XXXXX')
 
-response = client.Order.list({'status': 'QUEUED', 'limit': '250'})
+response = client.v1.Order.list({'status': 'QUEUED', 'limit': '250'})
 
 for order in response['orders']:
     print(order['id'])
 ```
 
 For more details on the content of the reponses, visit the (official recharge API docs)[https://developer.rechargepayments.com].
 
 ## Resources Available
-- Addresses
-- Charges
-- Checkouts
-- Customers
-- Discounts
-- Metafields
-- Notifications
-- Onetimes
-- Orders
-- Products
+### v1(2021-01)
+- Address
+- Charge
+- Checkout
+- Customer
+- Discount
+- Metafield
+- Notification
+- Onetime
+- Order
+- Product
 - Shop
-- Subscriptions
-- Webhooks
-- Async Batches
+- Subscription
+- Webhook
+- Async Batch
+### v2(2021-11)
+- Address
+- BundleSelection
+- Charge
+- Checkout
+- Collection
+- Customer
+- Discount
+- Metafield
+- Notification
+- Onetime
+- Order
+- Payment Method
+- Plan
+- Retention Strategy
+- Subscription
+- Webhook
+- Async Batch
+- Token
+- Account
+- Event
+- Store
 
 ## License
 MIT. See LICENSE for more details.
 
 ## Acknowledgements
 This project is a fork of recharge-api by BuluBox which is no longer available.
```

### Comparing `recharge_api-1.5.1/setup.cfg` & `recharge_api-1.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = recharge-api
-version = 1.5.1
+version = 1.6.0
 author = ChemicalLuck
 description = Python API Wrapper for Recharge
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/ChemicalLuck/recharge-api
 license = MIT
 keywords = api recharge
```

