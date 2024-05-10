# Comparing `tmp/fast_tradier_client-1.0.tar.gz` & `tmp/fast_tradier_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-1.0.tar", last modified: Wed May  8 02:11:48 2024, max compression
+gzip compressed data, was "fast_tradier_client-1.0.1.tar", last modified: Thu May  9 06:02:02 2024, max compression
```

## Comparing `fast_tradier_client-1.0.tar` & `fast_tradier_client-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11012 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/
--rw-rw-rw-   0 root         (0) root         (0)    16877 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/FastTradierAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)    16334 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/FastTradierClient.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerClient.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IModel.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/DataClassModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/ModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/account/
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/AccountBalance.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/AccountOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/Position.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/market_data/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/Hlocv.py
--rw-rw-rw-   0 root         (0) root         (0)     1841 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/TradierQuote.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/trading/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/EquityOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/OptionOrder.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/OrderBase.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/PriceTypes.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/Sides.py
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/TOSTradierConverter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/OptionUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/TimeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/YFinanceQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/fast_tradier_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11012 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/
+-rw-rw-rw-   0 root         (0) root         (0)    16877 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/FastTradierAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    16334 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/FastTradierClient.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/DataClassModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/ModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/account/
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/AccountBalance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/AccountOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/Position.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/market_data/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/Hlocv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/TradierQuote.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/trading/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/EquityOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/OptionOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/OrderBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/PriceTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/Sides.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/OptionUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/TimeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/YFinanceQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/setup.py
```

### Comparing `fast_tradier_client-1.0/LICENSE` & `fast_tradier_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/PKG-INFO` & `fast_tradier_client-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 1.0
+Version: 1.0.1
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0/README.md` & `fast_tradier_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-1.0.1/fast_tradier/FastTradierAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/FastTradierClient.py` & `fast_tradier_client-1.0.1/fast_tradier/FastTradierClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/models/ModelBase.py` & `fast_tradier_client-1.0.1/fast_tradier/models/ModelBase.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/models/account/AccountBalance.py` & `fast_tradier_client-1.0.1/fast_tradier/models/account/AccountBalance.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/models/account/AccountOrder.py` & `fast_tradier_client-1.0.1/fast_tradier/models/account/AccountOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/models/market_data/Quote.py` & `fast_tradier_client-1.0.1/fast_tradier/models/market_data/Quote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-1.0.1/fast_tradier/models/market_data/TradierQuote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/models/trading/EquityOrder.py` & `fast_tradier_client-1.0.1/fast_tradier/models/trading/EquityOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/models/trading/OptionOrder.py` & `fast_tradier_client-1.0.1/fast_tradier/models/trading/OptionOrder.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
         setattr(self, "price", new_price)
 
     def set_status(self, new_staus: str) -> None:
         setattr(self, "status", new_staus)
 
     def set_ticker(self, ticker_name: str) -> None:
         setattr(self, "ticker", ticker_name)
+    
+    def set_id(self, new_id: int) -> None:
+        setattr(self, "id", new_id)
 
     def clone_option_legs(self, reverse_side: bool = False) -> List[OptionLeg]:
         '''deep clone option_legs'''
         cloned_legs = []
         for opt_leg in self.option_legs:
             leg = OptionLeg(**(opt_leg.to_json()))
             if reverse_side:
```

### Comparing `fast_tradier_client-1.0/fast_tradier/models/trading/TOSTradierConverter.py` & `fast_tradier_client-1.0.1/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/utils/OptionUtils.py` & `fast_tradier_client-1.0.1/fast_tradier/utils/OptionUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-1.0.1/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier/utils/YFinanceQuoteProvider.py` & `fast_tradier_client-1.0.1/fast_tradier/utils/YFinanceQuoteProvider.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-1.0.1/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 1.0
+Version: 1.0.1
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-1.0.1/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0/pyproject.toml` & `fast_tradier_client-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "1.0"
+version = "1.0.1"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

