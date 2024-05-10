# Comparing `tmp/fast_tradier_client-1.0.1.tar.gz` & `tmp/fast_tradier_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-1.0.1.tar", last modified: Thu May  9 06:02:02 2024, max compression
+gzip compressed data, was "fast_tradier_client-1.0.2.tar", last modified: Fri May 10 01:18:13 2024, max compression
```

## Comparing `fast_tradier_client-1.0.1.tar` & `fast_tradier_client-1.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/
--rw-rw-rw-   0 root         (0) root         (0)    16877 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/FastTradierAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)    16334 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/FastTradierClient.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerClient.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IModel.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/DataClassModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/ModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/account/
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/AccountBalance.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/AccountOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/Position.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/market_data/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/Hlocv.py
--rw-rw-rw-   0 root         (0) root         (0)     1841 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/TradierQuote.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/models/trading/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/EquityOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/OptionOrder.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/OrderBase.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/PriceTypes.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/Sides.py
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/TOSTradierConverter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.106282 fast_tradier_client-1.0.1/fast_tradier/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/OptionUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/TimeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/YFinanceQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-09 06:02:02.000000 fast_tradier_client-1.0.1/fast_tradier_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 06:02:02.110282 fast_tradier_client-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-09 06:01:19.000000 fast_tradier_client-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.737324 fast_tradier_client-1.0.2/fast_tradier/
+-rw-rw-rw-   0 root         (0) root         (0)    16899 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/FastTradierAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    16356 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/FastTradierClient.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/DataClassModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/ModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/account/
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/AccountBalance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/AccountOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/Position.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/market_data/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/Hlocv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/TradierQuote.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/trading/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/EquityOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/OptionOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/OrderBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/PriceTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/Sides.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/OptionUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/TimeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/YFinanceQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/setup.py
```

### Comparing `fast_tradier_client-1.0.1/LICENSE` & `fast_tradier_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/PKG-INFO` & `fast_tradier_client-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.1/README.md` & `fast_tradier_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-1.0.2/fast_tradier/FastTradierAsyncClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,18 +129,18 @@
             if 'quotes' in json_res and json_res['quotes'] is not None:
                 quote_objs = json_res['quotes']['quote']
 
                 if quote_objs is not None:
                     if isinstance(quote_objs, List):
                         '''API returns a list of quotes if input is a list of tickers'''
                         for quote_obj in quote_objs:
-                            results.append(Quote(quote_obj))
+                            results.append(Quote(**quote_obj))
                     elif isinstance(quote_objs, Dict):
                         '''API returns a single Dict object if input is a single ticker'''
-                        results = [Quote(quote_objs)]
+                        results = [Quote(**quote_objs)]
             return results
         finally:
             if not self.keep_client_alive:
                 await client.aclose()
 
     async def get_history_async(self, symbol: str, start_date: date, end_date: date, interval: Interval = Interval.Daily, open_hours_only: bool = True) -> Optional[pd.DataFrame]:
         url = f'{self.host_base}markets/history'
@@ -164,16 +164,16 @@
                     json_data_arr = json_res['history']['day']
                 elif interval == Interval.Weekly:
                     json_data_arr = json_res['history']['week']
                 else:
                     json_data_arr = json_res['history']['month']
 
                 for his_json in json_data_arr:
-                    cur_hlocv = Hlocv(his_json)
-                    row = [cur_hlocv.date, cur_hlocv.open, cur_hlocv.high, cur_hlocv.low, cur_hlocv.close, cur_hlocv.volume]
+                    cur_hlocv = Hlocv(**his_json)
+                    row = [cur_hlocv.date, cur_hlocv.open_price, cur_hlocv.high, cur_hlocv.low, cur_hlocv.close, cur_hlocv.volume]
                     history_data.append(row)
 
             if len(history_data) > 0:
                 df = pd.DataFrame(history_data)
                 df.columns = ['Date', 'Open', 'High', 'Low', 'Close', 'Volume']
                 df['Date'] = pd.to_datetime(df['Date'])
                 df.set_index('Date', inplace=True)
@@ -197,18 +197,18 @@
         try:
             retrieved_orders = []
             response = await client.get(url=url, params={'includeTags': 'true'}, headers=self.__auth_headers)
             json_res = response.json()
             if 'orders' in json_res:
                 order_obj = json_res['orders']['order']
                 if isinstance(order_obj, Dict):
-                    retrieved_orders = [AccountOrder(order_obj)]
+                    retrieved_orders = [AccountOrder(**order_obj)]
                 elif isinstance(order_obj, List):
                     for order_json in order_obj:
-                        retrieved_orders.append(AccountOrder(order_json))
+                        retrieved_orders.append(AccountOrder(**order_json))
 
             return retrieved_orders
         finally:
             if not self.keep_client_alive:
                 await client.aclose()
 
     async def get_option_expirations_async(self, symbol: str) -> List[str]:
@@ -339,17 +339,17 @@
                                         headers=self.__auth_headers)
             res = response.json()
             results = []
             if res['positions'] is not None and 'position' in res['positions']:
                 pos_obj = res['positions']['position']
                 if isinstance(pos_obj, List):
                     for position_dict in pos_obj:
-                        results.append(Position(position_dict))
+                        results.append(Position(**position_dict))
                 elif isinstance(pos_obj, Dict):
-                    results = [Position(pos_obj)]
+                    results = [Position(**pos_obj)]
             return results
         finally:
             if not self.keep_client_alive:
                 await client.aclose()
 
     async def get_account_balance_async(self) -> Optional[AccountBalance]:
         url = f'{self.host_base}accounts/{self.account_id}/balances'
@@ -357,12 +357,12 @@
         try:
             response = await client.get(url=url,
                                         params={},
                                         headers=self.__auth_headers)
             res = response.json()
             result = None
             if res['balances'] is not None:
-                result = AccountBalance(res['balances'])
+                result = AccountBalance(**res['balances'])
             return result
         finally:
             if not self.keep_client_alive:
                 await client.aclose()
```

### Comparing `fast_tradier_client-1.0.1/fast_tradier/FastTradierClient.py` & `fast_tradier_client-1.0.2/fast_tradier/FastTradierClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,18 +128,18 @@
             if 'quotes' in json_res and json_res['quotes'] is not None:
                 quote_objs = json_res['quotes']['quote']
 
                 if quote_objs is not None:
                     if isinstance(quote_objs, List):
                         '''API returns a list of quotes if input is a list of tickers'''
                         for quote_obj in quote_objs:
-                            results.append(Quote(quote_obj))
+                            results.append(Quote(**quote_obj))
                     elif isinstance(quote_objs, Dict):
                         '''API returns a single Dict object if input is a single ticker'''
-                        results = [Quote(quote_objs)]
+                        results = [Quote(**quote_objs)]
             return results
         finally:
             if not self.keep_client_alive:
                 client.close()
 
     def get_history(self, symbol: str, start_date: date, end_date: date, interval: Interval = Interval.Daily, open_hours_only: bool = True) -> Optional[pd.DataFrame]:
         url = f'{self.host_base}markets/history'
@@ -163,16 +163,16 @@
                     json_data_arr = json_res['history']['day']
                 elif interval == Interval.Weekly:
                     json_data_arr = json_res['history']['week']
                 else:
                     json_data_arr = json_res['history']['month']
 
                 for his_json in json_data_arr:
-                    cur_hlocv = Hlocv(his_json)
-                    row = [cur_hlocv.date, cur_hlocv.open, cur_hlocv.high, cur_hlocv.low, cur_hlocv.close, cur_hlocv.volume]
+                    cur_hlocv = Hlocv(**his_json)
+                    row = [cur_hlocv.date, cur_hlocv.open_price, cur_hlocv.high, cur_hlocv.low, cur_hlocv.close, cur_hlocv.volume]
                     history_data.append(row)
 
             if len(history_data) > 0:
                 df = pd.DataFrame(history_data)
                 df.columns = ['Date', 'Open', 'High', 'Low', 'Close', 'Volume']
                 df['Date'] = pd.to_datetime(df['Date'])
                 df.set_index('Date', inplace=True)
@@ -195,18 +195,18 @@
         try:
             retrieved_orders = []
             response = client.get(url=url, params={'includeTags': 'true'}, headers=self.__auth_headers)
             json_res = response.json()
             if 'orders' in json_res:
                 order_obj = json_res['orders']['order']
                 if isinstance(order_obj, Dict):
-                    retrieved_orders = [AccountOrder(order_obj)]
+                    retrieved_orders = [AccountOrder(**order_obj)]
                 elif isinstance(order_obj, List):
                     for order_json in order_obj:
-                        retrieved_orders.append(AccountOrder(order_json))
+                        retrieved_orders.append(AccountOrder(**order_json))
 
             return retrieved_orders
         finally:
             if not self.keep_client_alive:
                 client.close()
 
     def get_option_expirations(self, symbol: str) -> List[str]:
@@ -333,17 +333,17 @@
                                 headers=self.__auth_headers)
             res = response.json()
             results = []
             if res['positions'] is not None and 'position' in res['positions']:
                 pos_obj = res['positions']['position']
                 if isinstance(pos_obj, List):
                     for position_dict in pos_obj:
-                        results.append(Position(position_dict))
+                        results.append(Position(**position_dict))
                 elif isinstance(pos_obj, Dict):
-                    results = [Position(pos_obj)]
+                    results = [Position(**pos_obj)]
             return results
         finally:
             if not self.keep_client_alive:
                 client.close()
 
     def get_account_balance(self) -> Optional[AccountBalance]:
         url = f'{self.host_base}accounts/{self.account_id}/balances'
@@ -351,12 +351,12 @@
         balances = None
         try:
             response = client.get(url=url,
                                     params={},
                                     headers=self.__auth_headers)
             res = response.json()
             if res['balances'] is not None:
-                balances = AccountBalance(res['balances'])
+                balances = AccountBalance(**res['balances'])
             return balances
         finally:
             if not self.keep_client_alive:
                 client.close()
```

### Comparing `fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/models/ModelBase.py` & `fast_tradier_client-1.0.2/fast_tradier/models/ModelBase.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/models/account/AccountOrder.py` & `fast_tradier_client-1.0.2/fast_tradier/models/account/AccountOrder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from dataclasses import dataclass
-from typing import Dict, Optional, List
-
+from typing import Dict, Mapping, Optional, List, Any
+from pydantic import Field, ConfigDict
 from fast_tradier.models.DataClassModelBase import DataClassModelBase
+from fast_tradier.models.ModelBase import NewModelBase
 
-@dataclass
-class Leg(DataClassModelBase):
+class Leg(NewModelBase):
     id: int
     type: str
     symbol: str
     side: str
     quantity: float
     status: str
     duration: str
@@ -18,48 +18,42 @@
     exec_quantity: float
     last_fill_price: float
     last_fill_quantity: float
     remaining_quantity: float
     create_date: str
     transaction_date: str
     # class: str
-    class_type: str
-    option_symbol: Optional[str]
-    def __init__(self, api_resp_dict: Dict):
-        super().__init__(api_resp_dict)
-        if 'class' in api_resp_dict:
-            self.class_type = api_resp_dict['class']
+    class_: Optional[str] = Field(..., alias="class")
+    option_symbol: Optional[str] = None
+    model_config = ConfigDict(populate_by_name=True)
+    
+    def to_json(self) -> Mapping[str, Any]:
+        result = self.model_dump(by_alias=True)
+        return result
 
-@dataclass
-class AccountOrder(DataClassModelBase):
+class AccountOrder(NewModelBase):
     id: int
-    type: str
+    # type: str
+    type_: str = Field(..., alias="type")
     symbol: str
     side: str
     quantity: float
     status: str
     duration: str
-    price: float
+    price: Optional[float] = None
     avg_fill_price: float
     exec_quantity: float
     last_fill_price: float
     last_fill_quantity: float
     remaining_quantity: float
     create_date: str
     transaction_date: str
-    class_type: str
-    num_legs: Optional[int]
-    strategy: Optional[str]
-    leg: Optional[List[Leg]]
-    
-    def __init__(self, api_resp_dict: Dict):
-        super().__init__(api_resp_dict)
-        for k, v in api_resp_dict.items():
-            k_upper = k.upper()
-            if k_upper == 'CLASS':
-                self.class_type = v
-            elif k_upper == 'LEG':
-                self.leg = []
-                for cur_leg in v:
-                    self.leg.append(Leg(cur_leg))
-            else:
-                setattr(self, k, v)
+    # class_type: str
+    class_: Optional[str] = Field(..., alias="class")
+    num_legs: Optional[int] = None
+    strategy: Optional[str] = None
+    leg: Optional[List[Leg]] = []
+    model_config = ConfigDict(populate_by_name=True)
+
+    def to_json(self) -> Mapping[str, Any]:
+        result = self.model_dump(by_alias=True)
+        return result
```

### Comparing `fast_tradier_client-1.0.1/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-1.0.2/fast_tradier/models/trading/EquityOrder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,91 @@
-from typing import Dict, Tuple
-
 from fast_tradier.models.ModelBase import ModelBase
-
-class TradierQuote(ModelBase):
-    def __init__(self, symbol: str, type: str, open: float, high: float, low: float, close: float, volume: float, bid: float, ask: float, last_price: float) -> None:
-        self.__symbol = symbol
-        self.__type = type #stock or option
-        self.__open = open
-        self.__high = high
-        self.__low = low
-        self.__close = close
-        self.__volume = volume
-        self.__bid = bid
-        self.__ask = ask
-        self.__mid = None if bid is None or ask is None else (bid + ask) / 2.0
-        self.__last_price = last_price
+from typing import List, Dict, Optional
+from fast_tradier.models.trading.Sides import EquityOrderSide
+from fast_tradier.models.trading.PriceTypes import EquityPriceType
+from fast_tradier.models.trading.Duration import Duration
+from fast_tradier.models.trading.OrderBase import OrderBase
+
+class EquityOrder(OrderBase):
+    def __init__(self, ticker: str, quantity: float, price: float, side: EquityOrderSide, price_type: EquityPriceType, duration: Duration, stop: Optional[float] = None) -> None:
+        self.__ticker = ticker
+        self.__quantity = quantity
+        self.__price = price
+        self.__side = side.value
+        self.__price_type = price_type.value
+        self.__duration = duration.value
+        self.__stop = stop
+        self.__status = None
+        self.__order_class = 'equity'
+        self.__id = None
 
     @property
-    def ohlcv(self) -> Tuple:
-        return self.__open, self.__high, self.__low, self.__close, self.__volume
+    def ticker(self) -> str:
+        return self.__ticker
     
     @property
-    def quote_type(self) -> str:
-        return self.__type
+    def quantity(self) -> float:
+        return self.__quantity
+    
+    @quantity.setter
+    def quantity(self, new_value: float):
+        self.__quantity = new_value
 
     @property
-    def open_price(self) -> float:
-        return self.__open
+    def price(self) -> float:
+        return self.__price
+
+    @price.setter
+    def price(self, new_value : float):
+        self.__price = new_value
 
     @property
-    def volume(self) -> float:
-        return self.__volume
+    def side(self) -> str:
+        return self.__side
 
     @property
-    def bid(self) -> float:
-        return self.__bid
+    def price_type(self) -> str:
+        return self.__price_type
 
     @property
-    def ask(self) -> float:
-        return self.__ask
+    def duration(self) -> str:
+        return self.__duration
 
     @property
-    def mid(self) -> float:
-        return self.__mid
+    def status(self) -> str:
+        return self.__status
+
+    @status.setter
+    def status(self, new_value: str):
+        self.__status = new_value
 
     @property
-    def last_price(self) -> float:
-        return self.__last_price
+    def id(self) -> int:
+        return self.__id
+
+    @id.setter
+    def id(self, new_value: int):
+        self.__id = new_value
+
+    @property
+    def order_class(self) -> str:
+        return self.__order_class
 
     @property
-    def symbol(self) -> str:
-        return self.__symbol
+    def stop(self) -> Optional[float]:
+        return self.__stop
 
     def __iter__(self):
-        yield from {
-            "symbol": self.symbol,
-            "type": self.quote_type,
-            "open": self.open_price,
-            "high": self.__high,
-            "low": self.__low,
-            "close": self.__close,
-            "volume": self.volume,
-            "bid": self.bid,
-            "ask": self.ask,
-            "last_price": self.last_price
-        }.items()
+        result = {
+            "id": self.id,
+            "status": self.status,
+            "side": self.side,
+            "symbol": self.ticker,
+            "quantity": self.quantity,
+            "duration": self.duration,
+            "price": self.price,
+            "type": self.price_type,
+            "class": self.order_class,
+            "stop": self.stop
+        }
+
+        yield from result.items()
```

### Comparing `fast_tradier_client-1.0.1/fast_tradier/models/trading/OptionOrder.py` & `fast_tradier_client-1.0.2/fast_tradier/models/trading/OptionOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/models/trading/TOSTradierConverter.py` & `fast_tradier_client-1.0.2/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/utils/OptionUtils.py` & `fast_tradier_client-1.0.2/fast_tradier/utils/OptionUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-1.0.2/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier/utils/YFinanceQuoteProvider.py` & `fast_tradier_client-1.0.2/fast_tradier/utils/YFinanceQuoteProvider.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-1.0.2/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.1/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-1.0.2/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.1/pyproject.toml` & `fast_tradier_client-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

