# Comparing `tmp/recharge_api-1.6.1.tar.gz` & `tmp/recharge_api-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recharge_api-1.6.1.tar", last modified: Fri May 10 11:01:45 2024, max compression
+gzip compressed data, was "recharge_api-1.6.2.tar", last modified: Fri May 10 11:04:13 2024, max compression
```

## Comparing `recharge_api-1.6.1.tar` & `recharge_api-1.6.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.997528 recharge_api-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-10 11:01:39.000000 recharge_api-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-10 11:01:45.997528 recharge_api-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-10 11:01:39.000000 recharge_api-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 11:01:39.000000 recharge_api-1.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.989528 recharge_api-1.6.1/recharge/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.989528 recharge_api-1.6.1/recharge/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.993528 recharge_api-1.6.1/recharge/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/async_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/checkouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/discounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/metafields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/onetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/products.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.997528 recharge_api-1.6.1/recharge/api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/async_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/bundle_selections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/checkouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/discounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/metafields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/onetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/payment_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/products.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/retention_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.997528 recharge_api-1.6.1/recharge_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 11:01:45.997528 recharge_api-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:04:13.822682 recharge_api-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-10 11:04:06.000000 recharge_api-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-10 11:04:13.822682 recharge_api-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-10 11:04:06.000000 recharge_api-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 11:04:06.000000 recharge_api-1.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:04:13.814682 recharge_api-1.6.2/recharge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:04:13.814682 recharge_api-1.6.2/recharge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:04:13.818682 recharge_api-1.6.2/recharge/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v1/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:04:13.822682 recharge_api-1.6.2/recharge/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/bundle_selections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/retention_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-10 11:04:06.000000 recharge_api-1.6.2/recharge/api/v2/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:04:13.822682 recharge_api-1.6.2/recharge_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-10 11:04:13.000000 recharge_api-1.6.2/recharge_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-10 11:04:13.000000 recharge_api-1.6.2/recharge_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:04:13.000000 recharge_api-1.6.2/recharge_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:04:13.000000 recharge_api-1.6.2/recharge_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 11:04:13.000000 recharge_api-1.6.2/recharge_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 11:04:13.000000 recharge_api-1.6.2/recharge_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 11:04:13.822682 recharge_api-1.6.2/setup.cfg
```

### Comparing `recharge_api-1.6.1/LICENSE` & `recharge_api-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.1/PKG-INFO` & `recharge_api-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recharge-api
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python API Wrapper for Recharge
 Home-page: http://github.com/ChemicalLuck/recharge-api
 Author: ChemicalLuck
 License: MIT
 Keywords: api recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `recharge_api-1.6.1/README.md` & `recharge_api-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.1/recharge/__init__.py` & `recharge_api-1.6.2/recharge/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from typing import Literal, TypeAlias
+from requests import Session
 
 import recharge.api.v1 as v1
 import recharge.api.v2 as v2
-
 from recharge.api import RechargeScope
 
-RechargeVersion: TypeAlias = Literal["2021-01", "2021-11"]
-
 
 class RechargeAPIv1Helper:
     def __init__(
         self,
-        access_token: str,
+        session: Session,
         debug: bool = False,
         scopes: list[RechargeScope] = [],
     ):
-        kwargs = {"access_token": access_token, "debug": debug, "scopes": scopes}
+        kwargs = {"session": session, "debug": debug, "scopes": scopes}
 
         self.Address = v1.AddressResource(**kwargs)
         self.Charge = v1.ChargeResource(**kwargs)
         self.Checkout = v1.CheckoutResource(**kwargs)
         self.Customer = v1.CustomerResource(**kwargs)
         self.Order = v1.OrderResource(**kwargs)
         self.Subscription = v1.SubscriptionResource(**kwargs)
@@ -33,19 +30,19 @@
         self.Notification = v1.NotificationResource(**kwargs)
         self.Token = v1.TokenResource(**kwargs)
 
 
 class RechargeAPIv2Helper:
     def __init__(
         self,
-        access_token: str,
+        session: Session,
         debug: bool = False,
         scopes: list[RechargeScope] = [],
     ):
-        kwargs = {"access_token": access_token, "debug": debug, "scopes": scopes}
+        kwargs = {"session": session, "debug": debug, "scopes": scopes}
 
         self.Address = v2.AddressResource(**kwargs)
         self.BundleSelection = v2.BundleSelectionResource(**kwargs)
         self.Charge = v2.ChargeResource(**kwargs)
         self.Checkout = v2.CheckoutResource(**kwargs)
         self.Collection = v2.CollectionResource(**kwargs)
         self.Customer = v2.CustomerResource(**kwargs)
@@ -64,19 +61,26 @@
         self.Account = v2.AccountResource(**kwargs)
         self.Event = v2.EventResource(**kwargs)
         self.Store = v2.StoreResource(**kwargs)
 
 
 class RechargeAPI(object):
     def __init__(self, access_token: str, debug=False):
-        self.access_token = access_token
+        self.headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+            "X-Recharge-Access-Token": access_token,
+        }
+        self.session = Session()
+        self.session.headers.update(self.headers)
+
         self.debug = debug
 
         kwargs = {
-            "access_token": access_token,
+            "session": self.session,
             "debug": debug,
         }
 
         from recharge.api.v1 import TokenResource
 
         self.Token = TokenResource(**kwargs)
 
@@ -84,8 +88,8 @@
 
         kwargs["scopes"] = self.scopes
 
         self.v1 = RechargeAPIv1Helper(**kwargs)
         self.v2 = RechargeAPIv2Helper(**kwargs)
 
 
-__all__ = ["RechargeAPI", "RechargeVersion"]
+__all__ = ["RechargeAPI"]
```

### Comparing `recharge_api-1.6.1/recharge/api/__init__.py` & `recharge_api-1.6.2/recharge/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import time
 from typing import Any, Literal, Mapping, TypeAlias
 
 import requests
 
+RechargeVersion: TypeAlias = Literal["2021-01", "2021-11"]
+
 RechargeScope: TypeAlias = Literal[
     "write_orders",
     "read_orders",
     "read_discounts",
     "write_discounts",
     "write_subscriptions",
     "read_subscriptions",
@@ -47,26 +49,23 @@
 
     Refer to the API docs to see the expected responses.
     https://developer.rechargepayments.com/
     """
 
     base_url = "https://api.rechargeapps.com"
     object_list_key = None
+    recharge_version: RechargeVersion = "2021-11"
 
     def __init__(
         self,
-        access_token,
-        debug,
-        scopes: list[RechargeScope],
+        session: requests.Session,
+        debug: bool = False,
+        scopes: list[RechargeScope] = [],
     ):
-        self.headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/json",
-            "X-Recharge-Access-Token": access_token,
-        }
+        self.session = session
         self.debug = debug
         self.scopes = scopes
 
         self.allowed_endpoints = []
 
     def check_scopes(self, endpoint: str, scopes: list[RechargeScope]):
         if endpoint in self.allowed_endpoints:
@@ -91,48 +90,56 @@
             log.info(url)
             log.info(response.headers["X-Recharge-Limit"])
 
     @property
     def url(self) -> str:
         return f"{self.base_url}/{self.object_list_key}"
 
+    def update_headers(self):
+        self.session.headers.update({"X-Recharge-Version": self.recharge_version})
+
     def _http_delete(self, url: str, body: Mapping[str, Any] | None = None):
-        response = requests.delete(url, headers=self.headers, json=body)
-        log.info(url)
-        log.info(response.headers["X-Recharge-Limit"])
+        self.update_headers()
+        response = self.session.delete(url, json=body)
+        self.log(url, response)
         if response.status_code == 429:
-            return self._http_delete(url)
+            return self._http_delete(url, body)
         return response
 
     def _http_get(self, url: str, query: Mapping[str, Any] | None = None):
-        response = requests.get(url, params=query, headers=self.headers)
+        self.update_headers()
+        print(url)
+        response = self.session.get(url, params=query)
+        print(response.text)
         self.log(url, response)
         if response.status_code == 429:
             time.sleep(1)
-            return self._http_get(url)
+            return self._http_get(url, query)
         return response.json()
 
     def _http_put(
         self,
         url: str,
         body: Mapping[str, Any] | None = None,
         query: Mapping[str, Any] | None = None,
     ):
-        response = requests.put(url, json=body, params=query, headers=self.headers)
+        self.update_headers()
+        response = self.session.put(url, json=body, params=query)
         self.log(url, response)
         if response.status_code == 429:
             time.sleep(1)
             return self._http_put(url, body)
         return response.json()
 
     def _http_post(
         self,
         url: str,
         body: Mapping[str, Any] | None = None,
         query: Mapping[str, Any] | None = None,
     ):
-        response = requests.post(url, json=body, params=query, headers=self.headers)
+        self.update_headers()
+        response = self.session.post(url, json=body, params=query)
         self.log(url, response)
         if response.status_code == 429:
             time.sleep(1)
             return self._http_post(url, body)
         return response.json()
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/__init__.py` & `recharge_api-1.6.2/recharge/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.1/recharge/api/v1/addresses.py` & `recharge_api-1.6.2/recharge/api/v1/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class AddressNoteAttributes(TypedDict):
     name: str
     value: str
 
 
@@ -93,14 +93,15 @@
 
 class AddressResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/addresses
     """
 
     object_list_key = "addresses"
+    recharge_version: RechargeVersion = "2021-01"
 
     def create(self, customer_id, body: AddressCreateBody):
         """Create an address for the customer.
         https://developer.rechargepayments.com/2021-01/addresses/create_address
         """
         required_scopes: list[RechargeScope] = ["write_customers"]
         self.check_scopes(
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/async_batches.py` & `recharge_api-1.6.2/recharge/api/v1/async_batches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 from .addresses import AddressApplyDiscountBody, AddressRemoveDiscountBody
 from .discounts import DiscountCreateBody, DiscountUpdateBody, DiscountDeleteBody
 from .onetimes import OnetimeCreateBody, OnetimeDeleteBody
 from .products import ProductCreateBody, ProductDeleteBody, ProductUpdateBody
 from .subscriptions import (
     SubscriptionBulkCreateBody,
@@ -60,14 +60,15 @@
 
 class AsyncBatchResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/async_batch_endpoints
     """
 
     object_list_key = "async_batches"
+    resource_version: RechargeVersion = "2021-01"
 
     def create(self, body: AsyncBatchCreateBody):
         """Create an async batch.
         https://developer.rechargepayments.com/2021-01/async_batch_endpoints
         """
         required_scopes: list[RechargeScope] = ["write_batches"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/charges.py` & `recharge_api-1.6.2/recharge/api/v1/charges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 ChargeStatus: TypeAlias = Literal[
     "SUCCESS", "QUEUED", "ERROR", "REFUNDED", "PARTIALLY_REFUNDED", "SKIPPED"
 ]
 
 
@@ -75,14 +75,15 @@
 
 class ChargeResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/charges
     """
 
     object_list_key = "charges"
+    recharge_version: RechargeVersion = "2021-01"
 
     def get(self, charge_id: str):
         """Get a charge by id.
         https://developer.rechargepayments.com/2021-01/charges/charge_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
         self.check_scopes(f"GET /{self.object_list_key}/:charge_id", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/checkouts.py` & `recharge_api-1.6.2/recharge/api/v1/checkouts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class CheckoutUtmParams(TypedDict, total=False):
     utm_campaign: str
     utm_content: str
     utm_data_source: str
     utm_source: str
@@ -144,14 +144,15 @@
 
 class CheckoutResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/checkouts
     """
 
     object_list_key = "checkouts"
+    resource_version: RechargeVersion = "2021-01"
 
     def create(self, body: CheckoutCreateBody):
         """Create a new checkout.
         https://developer.rechargepayments.com/2021-01/checkouts/checkout_create
         """
         required_scopes: list[RechargeScope] = ["write_checkouts"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/customers.py` & `recharge_api-1.6.2/recharge/api/v1/customers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class CustomerCreateBody(TypedDict, total=False):
     accepts_marketing: bool
     billing_address1: Required[str]
     billing_address2: str
     billing_city: Required[str]
@@ -69,14 +69,15 @@
 
 class CustomerResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/customers
     """
 
     object_list_key = "customers"
+    recharge_version: RechargeVersion = "2021-01"
 
     def create(self, body: CustomerCreateBody):
         """Create a customer.
         https://developer.rechargepayments.com/2021-01/customers/customers_create
         """
         required_scopes: list[RechargeScope] = ["write_customers", "write_payments"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
@@ -113,14 +114,15 @@
         return self._http_delete(f"{self.url}/{customer_id}")
 
     def list(self, query: CustomerListQuery | None = None):
         """List customers.
         https://developer.rechargepayments.com/2021-01/customers/customers_list
         """
         required_scopes: list[RechargeScope] = ["read_customers"]
+        print(query)
         self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url, query)
 
     def count(self, query: CustomerCountQuery | None = None):
         """Retrieve a count of customers.
         https://developer.rechargepayments.com/2021-01/customers/customers_count
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/discounts.py` & `recharge_api-1.6.2/recharge/api/v1/discounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 DiscountProductType: TypeAlias = Literal["ALL", "ONETIME", "SUBSCRIPTION"]
 
 DiscountAppliesToResource: TypeAlias = Literal[
     "shopify_product", "shopify_collection_id"
 ]
 
@@ -84,14 +84,15 @@
 
 class DiscountResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/discounts
     """
 
     object_list_key = "discounts"
+    recharge_version: RechargeVersion = "2021-01"
 
     def create(self, body: DiscountCreateBody):
         """Create a discount.
         https://developer.rechargepayments.com/2021-01/discounts/discounts_create
         """
         required_scopes: list[RechargeScope] = ["write_discounts"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/metafields.py` & `recharge_api-1.6.2/recharge/api/v1/metafields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 MetafieldOwnerResource: TypeAlias = Literal[
     "address", "store", "customer", "subscription", "order", "charge"
 ]
 
 MetafieldValueType: TypeAlias = Literal["string", "json_string", "integer"]
 
@@ -78,14 +78,15 @@
 
 class MetafieldResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/metafields
     """
 
     object_list_key = "metafields"
+    resource_version: RechargeVersion = "2021-01"
 
     def create(self, body: MetafieldCreateBody):
         """Create a metafield.
         https://developer.rechargepayments.com/2021-01/metafields/metafields_create
         """
         resource = body["owner_resource"]
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/notifications.py` & `recharge_api-1.6.2/recharge/api/v2/notifications.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Literal, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
-NotificationTemplateType: TypeAlias = Literal["upcoming_charge", "get_account_access"]
+NotificationTemplateType: TypeAlias = Literal[
+    "upcoming_charge", "get_account_access", "shopify_update_payment_information"
+]
 
 
 class NotificationTemplateVars(TypedDict, total=False):
     address_id: int
     charge_id: int
 
 
@@ -15,21 +17,26 @@
     type: Literal["email"]
     template_type: NotificationTemplateType
     template_vars: NotificationTemplateVars
 
 
 class NotificationResource(RechargeResource):
     """
-    https://developer.rechargepayments.com/2021-01/notifications
+    https://developer.rechargepayments.com/2021-11/notifications
     """
 
-    def send_email(self, customer_id, body: NotificationSendEmailBody):
+    object_list_key = "notifications"
+    resource_version: RechargeVersion = "2021-11"
+
+    def send_email(self, customer_id: str, body: NotificationSendEmailBody):
         """
         Send an email notification to a customer.
-        https://developer.rechargepayments.com/2021-01/notifications/notifications_get_account_access
+        https://developer.rechargepayments.com/2021-11/notifications/notifications_send
         """
         required_scopes: list[RechargeScope] = ["write_notifications"]
-        self.check_scopes("POST /customers/:customer_id/notifications", required_scopes)
+        self.check_scopes(
+            f"POST /customers/:customer_id/{self.object_list_key}", required_scopes
+        )
 
         return self._http_post(
-            f"{self.url}/customers/{customer_id}/notifications", body
+            f"{self.base_url}/customers/{customer_id}/{self.object_list_key}", body
         )
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/onetimes.py` & `recharge_api-1.6.2/recharge/api/v1/onetimes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Required, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class OnetimeProperty(TypedDict):
     name: str
     value: str
 
 
@@ -48,14 +48,15 @@
 
 class OnetimeResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/onetimes
     """
 
     object_list_key = "onetimes"
+    recharge_version: RechargeVersion = "2021-01"
 
     def create(self, body: OnetimeCreateBody):
         """Create a Onetime
         https://developer.rechargepayments.com/2021-01/onetimes/onetimes_create
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/orders.py` & `recharge_api-1.6.2/recharge/api/v1/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class OrderBillingAddress(TypedDict, total=False):
     address1: str
     province: str
     address2: str
     city: str
@@ -93,14 +93,15 @@
 
 class OrderResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/orders
     """
 
     object_list_key = "orders"
+    recharge_version: RechargeVersion = "2021-01"
 
     def get(self, order_id: str):
         """Get an order.
         https://developer.rechargepayments.com/2021-01/orders/orders_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
         self.check_scopes(f"GET /{self.object_list_key}/:order_id", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/products.py` & `recharge_api-1.6.2/recharge/api/v1/products.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 ProductDiscountType: TypeAlias = Literal["percentage"]
 
 ProductStorefrontPurchaseOptions: TypeAlias = Literal[
     "subscription_only", "subscription_and_onetime"
 ]
 
@@ -84,14 +84,15 @@
 
 class ProductResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/products
     """
 
     object_list_key = "products"
+    recharge_version: RechargeVersion = "2021-01"
 
     def create(self, body: ProductCreateBody):
         """Create a product.
         https://developer.rechargepayments.com/2021-01/products/products_create
         """
         required_scopes: list[RechargeScope] = ["write_products"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/shop.py` & `recharge_api-1.6.2/recharge/api/v1/shop.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class ShopResource(RechargeResource):
     """
     https://developer.rechargepayments.com/v1#shop
     """
 
     object_list_key = "shop"
+    recharge_version: RechargeVersion = "2021-01"
 
     def get(self):
         """Retrieve store using the Recharge API.
         https://developer.rechargepayments.com/2021-01/shop/shop_retrieve
         """
         required_scopes: list[RechargeScope] = ["store_info"]
         self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/subscriptions.py` & `recharge_api-1.6.2/recharge/api/v1/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 SubscriptionOrderIntervalUnit: TypeAlias = Literal["day", "week", "month"]
 
 
 class SubscriptionProperty(TypedDict):
     name: str
@@ -119,14 +119,15 @@
 
 class SubscriptionResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/subscriptions
     """
 
     object_list_key = "subscriptions"
+    resource_version: RechargeVersion = "2021-01"
 
     def create(self, body: SubscriptionCreateBody):
         """Create a subscription.
         https://developer.rechargepayments.com/2021-01/subscriptions/subscriptions_create
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/tokens.py` & `recharge_api-1.6.2/recharge/api/v1/tokens.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class TokenClient(TypedDict):
     name: str
     email: str
 
 
@@ -17,13 +17,14 @@
 
 class TokenResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/token_information/token_information_object
     """
 
     object_list_key = "token_information"
+    recharge_version: RechargeVersion = "2021-01"
 
     def get(self) -> TokenInformation:
         """Get token information.
         https://developer.rechargepayments.com/2021-01/token_information/token_information_retrieve
         """
         return self._http_get(f"{self.url}")
```

### Comparing `recharge_api-1.6.1/recharge/api/v1/webhooks.py` & `recharge_api-1.6.2/recharge/api/v1/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 WebhookTopic: TypeAlias = Literal[
     "address/created",
     "address/updated",
     "async_batch/processed",
     "bundle_selection/created",
     "bundle_selection/updated",
@@ -83,14 +83,15 @@
 
 class WebhookResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-01/webhooks_endpoints/webhooks_object
     """
 
     object_list_key = "webhooks"
+    recharge_version: RechargeVersion = "2021-01"
 
     def create(self, body: WebhookCreateBody):
         """Create a webhook.
         https://developer.rechargepayments.com/2021-01/webhooks_endpoints/webhooks_create
         """
         resource = body["topic"].split("/")[0]
         required_scopes: list[RechargeScope] = [WebhookTopicMap[resource]]
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/__init__.py` & `recharge_api-1.6.2/recharge/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.1/recharge/api/v2/accounts.py` & `recharge_api-1.6.2/recharge/api/v2/accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class AccountResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/accounts
     """
 
     object_list_key = "accounts"
+    recharge_version: RechargeVersion = "2021-11"
 
     def get(self, account_id: str):
         """Get an account.
         https://developer.rechargepayments.com/2021-11/accounts/account_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_accounts"]
         self.check_scopes(f"GET /{self.object_list_key}/:account_id", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/addresses.py` & `recharge_api-1.6.2/recharge/api/v2/addresses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Required, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class AddressOrderAttributes(TypedDict):
     name: str
     value: str
 
 
@@ -88,14 +88,15 @@
 
 class AddressResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/addresses
     """
 
     object_list_key = "addresses"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: AddressCreateBody):
         """Create an address for the customer.
         https://developer.rechargepayments.com/2021-11/addresses/create_address
         """
         required_scopes: list[RechargeScope] = ["write_customers"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/async_batches.py` & `recharge_api-1.6.2/recharge/api/v2/async_batches.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 from .discounts import DiscountCreateBody, DiscountUpdateBody, DiscountDeleteBody
 from .plans import (
     PlanCreateBody,
     PlanUpdateBody,
     PlanDeleteBody,
 )
@@ -49,14 +49,15 @@
 
 class AsyncBatchResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/async_batch_endpoints
     """
 
     object_list_key = "async_batches"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: AsyncBatchCreateBody):
         """Create an async batch.
         https://developer.rechargepayments.com/2021-11/async_batch_endpoints/async_batch_endpoints_create
         """
         required_scopes: list[RechargeScope] = ["write_batches"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/bundle_selections.py` & `recharge_api-1.6.2/recharge/api/v2/bundle_selections.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from recharge.api import RechargeResource, RechargeScope
+from typing import Literal, TypedDict
 
-from typing import TypedDict, Literal
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 BundleSelectionListSortBy = Literal[
     "id-asc", "id-desc", "updated_at-asc", "updated_at-desc"
 ]
 
 
 class BundleSelectionListQuery(TypedDict, total=False):
@@ -38,14 +38,15 @@
 
 class BundleSelectionResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/bundle_selections
     """
 
     object_list_key = "bundle_selections"
+    recharge_version: RechargeVersion = "2021-11"
 
     def list(self, query: BundleSelectionListQuery | None = None):
         """List bundle selections.
         https://developer.rechargepayments.com/2021-11/bundle_selections/bundle_selections_list
         """
         required_scopes: list[RechargeScope] = ["read_subscriptions"]
         self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/charges.py` & `recharge_api-1.6.2/recharge/api/v2/charges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 ChargeStatus: TypeAlias = Literal[
     "SUCCESS", "QUEUED", "ERROR", "REFUNDED", "PARTIALLY_REFUNDED", "SKIPPED"
 ]
 
 ChargeListSortBy: TypeAlias = Literal[
@@ -75,14 +75,15 @@
 
 class ChargeResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/charges
     """
 
     object_list_key = "charges"
+    recharge_version: RechargeVersion = "2021-11"
 
     def get(self, charge_id: str):
         """Get a charge by id.
         https://developer.rechargepayments.com/2021-11/charges/charge_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
         self.check_scopes(f"GET /{self.object_list_key}/:charge_id", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/checkouts.py` & `recharge_api-1.6.2/recharge/api/v2/checkouts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class CheckoutUtmParams(TypedDict, total=False):
     utm_campaign: str
     utm_content: str
     utm_data_source: str
     utm_source: str
@@ -188,14 +188,15 @@
 
 class CheckoutResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/checkouts
     """
 
     object_list_key = "checkouts"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: CheckoutCreateBody):
         """Create a new checkout.
         https://developer.rechargepayments.com/2021-11/checkouts/checkout_create
         """
         required_scopes: list[RechargeScope] = ["write_checkouts"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/collections.py` & `recharge_api-1.6.2/recharge/api/v2/collections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Required, TypedDict, TypeAlias, Literal
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 CollectionCreateSortOrder: TypeAlias = Literal[
     "id-asc", "id-desc", "title-asc", "title-desc", "created-asc", "created-desc"
 ]
 
 
 class CollectionCreateBody(TypedDict, total=False):
@@ -41,14 +41,15 @@
 
 class CollectionResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/collections
     """
 
     object_list_key = "collections"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: CollectionCreateBody):
         """Create a collection.
         https://developer.rechargepayments.com/2021-11/collections/collections_create
         """
         required_scopes: list[RechargeScope] = ["write_products"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/customers.py` & `recharge_api-1.6.2/recharge/api/v2/customers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class CustomerCreateExternalCustomerId(TypedDict, total=False):
     ecommerce: str
 
 
 class CustomerCreateBody(TypedDict, total=False):
@@ -50,14 +50,15 @@
 
 class CustomerResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/customers
     """
 
     object_list_key = "customers"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: CustomerCreateBody):
         """Create a customer.
         https://developer.rechargepayments.com/2021-11/customers/customers_create
         """
         required_scopes: list[RechargeScope] = [
             "write_customers",
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/discounts.py` & `recharge_api-1.6.2/recharge/api/v2/discounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 DiscountProductType: TypeAlias = Literal["ALL", "ONETIME", "SUBSCRIPTION"]
 
 DiscountAppliesToResource: TypeAlias = Literal[
     "shopify_product", "shopify_collection_id"
 ]
 
@@ -89,14 +89,15 @@
 
 class DiscountResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/discounts
     """
 
     object_list_key = "discounts"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: DiscountCreateBody):
         """Create a discount.
         https://developer.rechargepayments.com/2021-11/discounts/discounts_create
         """
         required_scopes: list[RechargeScope] = ["write_discounts"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/events.py` & `recharge_api-1.6.2/recharge/api/v2/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class EventListQuery(TypedDict, total=False):
     create_at_min: str
     created_at_max: str
     object_type: str
     object_id: int
@@ -15,14 +15,15 @@
 
 class EventResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/events
     """
 
     object_list_key = "events"
+    recharge_version: RechargeVersion = "2021-11"
 
     def list(self, query: EventListQuery | None = None):
         """List events.
         https://developer.rechargepayments.com/2021-11/events/events_list
         """
         required_scopes: list[RechargeScope] = ["read_events"]
         self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/metafields.py` & `recharge_api-1.6.2/recharge/api/v2/metafields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 MetafieldOwnerResource: TypeAlias = Literal[
     "address", "store", "customer", "subscription", "order", "charge"
 ]
 
 MetafieldValueType: TypeAlias = Literal["string", "json_string", "integer"]
 
@@ -72,14 +72,15 @@
 
 class MetafieldResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/metafields
     """
 
     object_list_key = "metafields"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: MetafieldCreateBody):
         """Create a metafield.
         https://developer.rechargepayments.com/2021-11/metafields/metafields_create
         """
         resource = body["owner_resource"]
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/onetimes.py` & `recharge_api-1.6.2/recharge/api/v2/onetimes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Required, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class OnetimeProperty(TypedDict):
     name: str
     value: str
 
 
@@ -62,14 +62,15 @@
 
 class OnetimeResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/onetimes
     """
 
     object_list_key = "onetimes"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: OnetimeCreateBody):
         """Create a Onetime
         https://developer.rechargepayments.com/2021-11/onetimes/onetimes_create
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/orders.py` & `recharge_api-1.6.2/recharge/api/v2/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class OrderCloneBody(TypedDict, total=False):
     scheduled_at: str
 
 
 class OrderBillingAddress(TypedDict, total=False):
@@ -134,14 +134,15 @@
 
 class OrderResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/orders
     """
 
     object_list_key = "orders"
+    recharge_version: RechargeVersion = "2021-11"
 
     def get(self, order_id: str):
         """Get an order.
         https://developer.rechargepayments.com/2021-11/orders/orders_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_orders"]
         self.check_scopes(f"GET /{self.object_list_key}/:order_id", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/payment_methods.py` & `recharge_api-1.6.2/recharge/api/v2/payment_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import TypeAlias, TypedDict, Literal, Required
-from recharge.api import RechargeResource, RechargeScope
+from typing import Literal, Required, TypeAlias, TypedDict
+
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 PaymentMethodType: TypeAlias = Literal[
     "CREDIT_CARD", "PAYPAL", "APPLE_PAY", "GOOGLE_PAY", "SEPA_DEBIT"
 ]
 
 PaymentMethodProcessorName: TypeAlias = Literal[
     "stripe", "braintree", "authorize", "shopify_payments", "mollie"
@@ -46,14 +47,15 @@
 
 class PaymentMethodResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/payment_methods
     """
 
     object_list_key = "payment_methods"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: PaymentMethodCreateBody):
         """Create a payment method.
         https://developer.rechargepayments.com/2021-11/payment_methods/payment_methods_create
         """
         required_scopes: list[RechargeScope] = ["write_payment_methods"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/plans.py` & `recharge_api-1.6.2/recharge/api/v2/plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class PlanChannelSettingsApi(TypedDict):
     display: bool
 
 
 class PlanChannelSettingsCustomerPortal(TypedDict):
@@ -100,14 +100,15 @@
 
 class PlanResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/plans
     """
 
     object_list_key = "plans"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: PlanCreateBody):
         """Create a plan.
         https://developer.rechargepayments.com/2021-11/plans/plans_create
         """
         required_scopes: list[RechargeScope] = ["write_products"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/products.py` & `recharge_api-1.6.2/recharge/api/v2/products.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 ProductDiscountType: TypeAlias = Literal["percentage"]
 
 
 class ProductExternalProductId(TypedDict):
     ecommerce: str
 
@@ -88,58 +88,59 @@
 
 class ProductListQuery(TypedDict, total=False):
     external_product_ids: str
 
 
 class ProductResource(RechargeResource):
     """
-    https://developer.rechargepayments.com/2021-01/products
+    https://developer.rechargepayments.com/2021-11/products
     """
 
     object_list_key = "products"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: ProductCreateBody):
         """Create a product.
-        https://developer.rechargepayments.com/2021-01/products/products_create
+        https://developer.rechargepayments.com/2021-11/products/products_create
         """
         required_scopes: list[RechargeScope] = ["write_products"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
 
         return self._http_post(self.url, body)
 
     def get(self, product_id: str):
         """Get a product.
-        https://developer.rechargepayments.com/2021-01/products/products_retrieve
+        https://developer.rechargepayments.com/2021-11/products/products_retrieve
         """
         required_scopes: list[RechargeScope] = ["read_products"]
         self.check_scopes(f"GET /{self.object_list_key}/:product_id", required_scopes)
 
         return self._http_get(f"{self.url}/{product_id}")
 
     def update(self, product_id: str, body: ProductUpdateBody):
         """Update a product.
-        https://developer.rechargepayments.com/2021-01/products/products_update
+        https://developer.rechargepayments.com/2021-11/products/products_update
         """
         required_scopes: list[RechargeScope] = ["write_products"]
         self.check_scopes(f"PUT /{self.object_list_key}/:product_id", required_scopes)
 
         return self._http_put(f"{self.url}/{product_id}", body)
 
     def delete(self, product_id: str):
         """Delete a product.
-        https://developer.rechargepayments.com/2021-01/products/products_delete
+        https://developer.rechargepayments.com/2021-11/products/products_delete
         """
         required_scopes: list[RechargeScope] = ["write_products"]
         self.check_scopes(
             f"DELETE /{self.object_list_key}/:product_id", required_scopes
         )
 
         return self._http_delete(f"{self.url}/{product_id}")
 
     def list(self, query: ProductListQuery | None = None):
         """List products.
-        https://developer.rechargepayments.com/2021-01/products/products_list
+        https://developer.rechargepayments.com/2021-11/products/products_list
         """
         required_scopes: list[RechargeScope] = ["read_products"]
         self.check_scopes(f"GET /{self.object_list_key}", required_scopes)
 
         return self._http_get(self.url, query)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/retention_strategies.py` & `recharge_api-1.6.2/recharge/api/v2/retention_strategies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from recharge.api import RechargeResource, RechargeScope
-
 from typing import Literal, Required, TypeAlias, TypedDict
 
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 RetentionStrategyCancellationFlowType: TypeAlias = Literal["subscription", "membership"]
 
 RetentionStrategyIncentiveType: TypeAlias = Literal[
     "delay_subscription", "discount", "skip_charge", "swap_product"
 ]
 
@@ -28,14 +27,15 @@
 
 class RetentionStrategyResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/retention_strategies
     """
 
     object_list_key = "retention_strategies"
+    resource_version: RechargeVersion = "2021-11"
 
     def create(self, body: RetentionStrategyCreateBody):
         """Create a retention strategy.
         https://developer.rechargepayments.com/2021-11/retention_strategies/retention_strategies_create
         """
         required_scopes: list[RechargeScope] = ["write_retention_strategies"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/subscriptions.py` & `recharge_api-1.6.2/recharge/api/v2/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypeAlias, TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 SubscriptionOrderIntervalUnit: TypeAlias = Literal["day", "week", "month"]
 
 
 class SubscriptionProperty(TypedDict):
     name: str
@@ -121,14 +121,15 @@
 
 class SubscriptionResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/subscriptions
     """
 
     object_list_key = "subscriptions"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: SubscriptionCreateBody):
         """Create a subscription.
         https://developer.rechargepayments.com/2021-11/subscriptions/subscriptions_create
         """
         required_scopes: list[RechargeScope] = ["write_subscriptions"]
         self.check_scopes(f"POST /{self.object_list_key}", required_scopes)
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/tokens.py` & `recharge_api-1.6.2/recharge/api/v2/tokens.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypedDict
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 
 class TokenClient(TypedDict):
     name: str
     email: str
 
 
@@ -17,13 +17,14 @@
 
 class TokenResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/token_information/token_information_object
     """
 
     object_list_key = "token_information"
+    recharge_version: RechargeVersion = "2021-11"
 
     def get(self) -> TokenInformation:
         """Get token information.
         https://developer.rechargepayments.com/2021-11/token_information/token_information_retrieve
         """
         return self._http_get(f"{self.url}")
```

### Comparing `recharge_api-1.6.1/recharge/api/v2/webhooks.py` & `recharge_api-1.6.2/recharge/api/v2/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Literal, Required, TypedDict, TypeAlias
 
-from recharge.api import RechargeResource, RechargeScope
+from recharge.api import RechargeResource, RechargeScope, RechargeVersion
 
 WebhookTopic: TypeAlias = Literal[
     "address/created",
     "address/updated",
     "async_batch/processed",
     "bundle_selection/created",
     "bundle_selection/updated",
@@ -84,14 +84,15 @@
 
 class WebhookResource(RechargeResource):
     """
     https://developer.rechargepayments.com/2021-11/webhooks_endpoints/webhooks_object
     """
 
     object_list_key = "webhooks"
+    recharge_version: RechargeVersion = "2021-11"
 
     def create(self, body: WebhookCreateBody):
         """Create a webhook.
         https://developer.rechargepayments.com/2021-11/webhooks_endpoints/webhooks_create
         """
         resource = body["topic"].split("/")[0]
         required_scopes: list[RechargeScope] = [WebhookTopicMap[resource]]
```

### Comparing `recharge_api-1.6.1/recharge_api.egg-info/PKG-INFO` & `recharge_api-1.6.2/recharge_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recharge-api
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python API Wrapper for Recharge
 Home-page: http://github.com/ChemicalLuck/recharge-api
 Author: ChemicalLuck
 License: MIT
 Keywords: api recharge
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `recharge_api-1.6.1/recharge_api.egg-info/SOURCES.txt` & `recharge_api-1.6.2/recharge_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.1/setup.cfg` & `recharge_api-1.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = recharge-api
-version = 1.6.1
+version = 1.6.2
 author = ChemicalLuck
 description = Python API Wrapper for Recharge
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/ChemicalLuck/recharge-api
 license = MIT
 keywords = api recharge
```

