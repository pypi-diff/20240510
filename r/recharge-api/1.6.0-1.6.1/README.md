# Comparing `tmp/recharge_api-1.6.0.tar.gz` & `tmp/recharge_api-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recharge_api-1.6.0.tar", last modified: Fri May 10 08:22:20 2024, max compression
+gzip compressed data, was "recharge_api-1.6.1.tar", last modified: Fri May 10 11:01:45 2024, max compression
```

## Comparing `recharge_api-1.6.0.tar` & `recharge_api-1.6.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.456666 recharge_api-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-10 08:22:13.000000 recharge_api-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 08:22:20.456666 recharge_api-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-10 08:22:13.000000 recharge_api-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 08:22:13.000000 recharge_api-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.444666 recharge_api-1.6.0/recharge/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.444666 recharge_api-1.6.0/recharge/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.448666 recharge_api-1.6.0/recharge/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/async_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/checkouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/discounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/metafields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/onetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/products.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v1/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.452666 recharge_api-1.6.0/recharge/api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/async_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/bundle_selections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/checkouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/discounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/metafields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/onetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/payment_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/products.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/retention_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-10 08:22:13.000000 recharge_api-1.6.0/recharge/api/v2/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:22:20.456666 recharge_api-1.6.0/recharge_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 08:22:20.000000 recharge_api-1.6.0/recharge_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 08:22:20.456666 recharge_api-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.997528 recharge_api-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-10 11:01:39.000000 recharge_api-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-10 11:01:45.997528 recharge_api-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-10 11:01:39.000000 recharge_api-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 11:01:39.000000 recharge_api-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.989528 recharge_api-1.6.1/recharge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.989528 recharge_api-1.6.1/recharge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.993528 recharge_api-1.6.1/recharge/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v1/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.997528 recharge_api-1.6.1/recharge/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/async_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/bundle_selections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/checkouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/discounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/metafields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/onetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/retention_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-10 11:01:39.000000 recharge_api-1.6.1/recharge/api/v2/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:01:45.997528 recharge_api-1.6.1/recharge_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 11:01:45.000000 recharge_api-1.6.1/recharge_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 11:01:45.997528 recharge_api-1.6.1/setup.cfg
```

### Comparing `recharge_api-1.6.0/LICENSE` & `recharge_api-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/__init__.py` & `recharge_api-1.6.1/recharge/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/__init__.py` & `recharge_api-1.6.1/recharge/api/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/__init__.py` & `recharge_api-1.6.1/recharge/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/addresses.py` & `recharge_api-1.6.1/recharge/api/v1/addresses.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/async_batches.py` & `recharge_api-1.6.1/recharge/api/v1/async_batches.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/charges.py` & `recharge_api-1.6.1/recharge/api/v1/charges.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/checkouts.py` & `recharge_api-1.6.1/recharge/api/v1/checkouts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/customers.py` & `recharge_api-1.6.1/recharge/api/v1/customers.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/discounts.py` & `recharge_api-1.6.1/recharge/api/v1/discounts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/metafields.py` & `recharge_api-1.6.1/recharge/api/v1/metafields.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,31 @@
     value: Required[str]
     value_type: Required[MetafieldValueType]
 
 
 class MetafieldUpdateBody(TypedDict, total=False):
     description: str
     owner_id: str
-    owner_resource: MetafieldOwnerResource
+    owner_resource: Required[MetafieldOwnerResource]
     value: str
     value_type: MetafieldValueType
 
 
 class MetafieldListQuery(TypedDict, total=False):
     limit: str
     namespace: str
     owner_id: str
-    owner_resource: MetafieldOwnerResource
+    owner_resource: Required[MetafieldOwnerResource]
     page: str
 
 
 class MetafieldCountQuery(TypedDict, total=False):
     namespace: str
     owner_id: str
-    owner_resource: MetafieldOwnerResource
+    owner_resource: Required[MetafieldOwnerResource]
 
 
 MetafieldOwnerResourceScopeMap: dict[str, dict[str, RechargeScope]] = {
     "address": {
         "read": "read_customers",
         "write": "write_customers",
     },
```

### Comparing `recharge_api-1.6.0/recharge/api/v1/notifications.py` & `recharge_api-1.6.1/recharge/api/v1/notifications.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/onetimes.py` & `recharge_api-1.6.1/recharge/api/v1/onetimes.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/orders.py` & `recharge_api-1.6.1/recharge/api/v1/orders.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/products.py` & `recharge_api-1.6.1/recharge/api/v1/products.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/shop.py` & `recharge_api-1.6.1/recharge/api/v1/shop.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/subscriptions.py` & `recharge_api-1.6.1/recharge/api/v1/subscriptions.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/tokens.py` & `recharge_api-1.6.1/recharge/api/v1/tokens.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v1/webhooks.py` & `recharge_api-1.6.1/recharge/api/v1/webhooks.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/__init__.py` & `recharge_api-1.6.1/recharge/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/accounts.py` & `recharge_api-1.6.1/recharge/api/v2/accounts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/addresses.py` & `recharge_api-1.6.1/recharge/api/v2/addresses.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/async_batches.py` & `recharge_api-1.6.1/recharge/api/v2/async_batches.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/bundle_selections.py` & `recharge_api-1.6.1/recharge/api/v2/bundle_selections.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/charges.py` & `recharge_api-1.6.1/recharge/api/v2/charges.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/checkouts.py` & `recharge_api-1.6.1/recharge/api/v2/checkouts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/collections.py` & `recharge_api-1.6.1/recharge/api/v2/collections.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/customers.py` & `recharge_api-1.6.1/recharge/api/v2/customers.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/discounts.py` & `recharge_api-1.6.1/recharge/api/v2/discounts.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/events.py` & `recharge_api-1.6.1/recharge/api/v2/events.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/metafields.py` & `recharge_api-1.6.1/recharge/api/v2/metafields.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/notifications.py` & `recharge_api-1.6.1/recharge/api/v2/notifications.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/onetimes.py` & `recharge_api-1.6.1/recharge/api/v2/onetimes.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/orders.py` & `recharge_api-1.6.1/recharge/api/v2/orders.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/payment_methods.py` & `recharge_api-1.6.1/recharge/api/v2/payment_methods.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/plans.py` & `recharge_api-1.6.1/recharge/api/v2/plans.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/products.py` & `recharge_api-1.6.1/recharge/api/v2/products.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/retention_strategies.py` & `recharge_api-1.6.1/recharge/api/v2/retention_strategies.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/store.py` & `recharge_api-1.6.1/recharge/api/v2/store.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/subscriptions.py` & `recharge_api-1.6.1/recharge/api/v2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/tokens.py` & `recharge_api-1.6.1/recharge/api/v2/tokens.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge/api/v2/webhooks.py` & `recharge_api-1.6.1/recharge/api/v2/webhooks.py`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/recharge_api.egg-info/SOURCES.txt` & `recharge_api-1.6.1/recharge_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recharge_api-1.6.0/setup.cfg` & `recharge_api-1.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = recharge-api
-version = 1.6.0
+version = 1.6.1
 author = ChemicalLuck
 description = Python API Wrapper for Recharge
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/ChemicalLuck/recharge-api
 license = MIT
 keywords = api recharge
```

