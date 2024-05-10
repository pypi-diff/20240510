# Comparing `tmp/stockdex-0.4.0.tar.gz` & `tmp/stockdex-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdex-0.4.0.tar", last modified: Sat Apr 20 21:59:37 2024, max compression
+gzip compressed data, was "stockdex-0.5.0.tar", last modified: Fri May 10 21:25:32 2024, max compression
```

## Comparing `stockdex-0.4.0.tar` & `stockdex-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:59:37.758919 stockdex-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-20 21:59:37.758919 stockdex-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-20 21:59:25.000000 stockdex-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 21:59:37.758919 stockdex-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-20 21:59:25.000000 stockdex-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:59:37.734920 stockdex-0.4.0/stockdex/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:59:37.738920 stockdex-0.4.0/stockdex/chromedriver_linux64/
--rw-r--r--   0 runner    (1001) docker     (127)   326542 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/chromedriver_linux64/LICENSE.chromedriver
--rwxr-xr-x   0 runner    (1001) docker     (127) 15039112 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/chromedriver_linux64/chromedriver
--rw-r--r--   0 runner    (1001) docker     (127)    14778 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/digrin_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/selenium_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/ticker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/ticker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16683 2024-04-20 21:59:25.000000 stockdex-0.4.0/stockdex/yahoo_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:59:37.738920 stockdex-0.4.0/stockdex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-20 21:59:37.000000 stockdex-0.4.0/stockdex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-20 21:59:37.000000 stockdex-0.4.0/stockdex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 21:59:37.000000 stockdex-0.4.0/stockdex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-20 21:59:37.000000 stockdex-0.4.0/stockdex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 21:59:37.000000 stockdex-0.4.0/stockdex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:59:37.754919 stockdex-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 21:59:25.000000 stockdex-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-20 21:59:25.000000 stockdex-0.4.0/tests/test_digrin_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-20 21:59:25.000000 stockdex-0.4.0/tests/test_justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-20 21:59:25.000000 stockdex-0.4.0/tests/test_nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-20 21:59:25.000000 stockdex-0.4.0/tests/test_ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-20 21:59:25.000000 stockdex-0.4.0/tests/test_ticker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-20 21:59:25.000000 stockdex-0.4.0/tests/test_yahoo_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:25:32.201087 stockdex-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-10 21:25:32.201087 stockdex-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-10 21:25:24.000000 stockdex-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:25:32.201087 stockdex-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-10 21:25:24.000000 stockdex-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:25:32.181087 stockdex-0.5.0/stockdex/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:25:32.185087 stockdex-0.5.0/stockdex/chromedriver_linux64/
+-rw-r--r--   0 runner    (1001) docker     (127)   326542 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/chromedriver_linux64/LICENSE.chromedriver
+-rwxr-xr-x   0 runner    (1001) docker     (127) 15039112 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/chromedriver_linux64/chromedriver
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/digrin_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/justetf_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/selenium_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/ticker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/yahoo_api_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16876 2024-05-10 21:25:24.000000 stockdex-0.5.0/stockdex/yahoo_web_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:25:32.181087 stockdex-0.5.0/stockdex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-10 21:25:32.000000 stockdex-0.5.0/stockdex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-10 21:25:32.000000 stockdex-0.5.0/stockdex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:25:32.000000 stockdex-0.5.0/stockdex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 21:25:32.000000 stockdex-0.5.0/stockdex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 21:25:32.000000 stockdex-0.5.0/stockdex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:25:32.201087 stockdex-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:25:24.000000 stockdex-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-10 21:25:24.000000 stockdex-0.5.0/tests/test_digrin_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-10 21:25:24.000000 stockdex-0.5.0/tests/test_justetf_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-10 21:25:24.000000 stockdex-0.5.0/tests/test_nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-10 21:25:24.000000 stockdex-0.5.0/tests/test_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-10 21:25:24.000000 stockdex-0.5.0/tests/test_yahoo_api_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-05-10 21:25:24.000000 stockdex-0.5.0/tests/test_yahoo_web_interface.py
```

### Comparing `stockdex-0.4.0/PKG-INFO` & `stockdex-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -24,30 +24,33 @@
 Stockdex is a Python package that provides a simple interface to access financial data from Yahoo Finance. Data is returned as a pandas DataFrame.
 
 # Installation 
 
 Install the package using pip:
 
 ```bash
-pip install stockdex
+pip install stockdex -U
 ``` 
 
 # Usage
 
-Create `Ticker` object by passing the ticker symbol. Ticker objects are the main interface to retrieve stock data.
-
+To access main functions, use `ticker`property from `TickerFactory` class. The `Ticker` class is used to access data from Various data sources. The `TickerFactory` class requires a data source to be passed to it. Here is an example of how to begin using the package:
 ```python
-from stockdex import Ticker
+from stockdex import TickerFactory
 
-# Pick arbitrary ticker
-ticker = Ticker('AAPL')
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_api").ticker
 ```
 
-## Fundamental data from `Yahoo Finance` API (fast queries through Yahoo Finance API):
+After creating the `Ticker` object, you can access functions defined for each data source. Below are some examples of how to access data from supported data sources.
+
+## Data from `Yahoo Finance` API (fast queries through Yahoo Finance API):
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_api").ticker
 
 # Price data (use range and dataGranularity to make range and granularity more specific)
 price = ticker.price(range='1y', dataGranularity='1d')
 
 # Current trading period of the stock (pre-market, regular, post-market trading periods)
 current_trading_period = ticker.current_trading_period
 
@@ -55,16 +58,20 @@
 income_statement = ticker.income_statement(frequency='quarterly')
 cash_flow = ticker.cash_flow(format='raw')
 balance_sheet = ticker.balance_sheet(period1=datetime(2020, 1, 1))
 financials = ticker.financials(period1=datetime(2022, 1, 1), period2=datetime.today())
 ```
 
 
-## Fundamental data with criteria from `Yahoo Finance` website (web scraping):
+## Data from `Yahoo Finance` website (web scraping):
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_web").ticker
+
 # Summary including general financial information
 summary = ticker.summary
 
 # Financial data as it is seen in the yahoo finance website
 income_stmt_web = ticker.income_stmt_web
 balance_sheet = ticker.balance_sheet_web
 cash_flow = ticker.cashflow_web
@@ -88,46 +95,52 @@
 
 # Statistics
 valuation_measures = ticker.valuation_measures
 financial_highlights = ticker.financial_highlights
 trading_information = ticker.trading_information
 ```
 
-## NASDAQ data from `NASDAQ` website (web scraping):
+<!-- ## NASDAQ data from `NASDAQ` website (web scraping):
 
 Data on NASDAQ website gets updated more frequently than Yahoo Finance data. Below are some of the data that can be retrieved from the NASDAQ website.
 
 ```python
 # Data about quarterly and yearly earnings, updated on the same day as the earnings release (yahoo finance data is updated after a few days)
 
 quarterly_earnings_surprise = ticker.quarterly_earnings_surprise
 yearly_earnings_forecast = ticker.yearly_earnings_forecast
 quarterly_earnings_forecast = ticker.quarterly_earnings_forecast
 
 price_to_earnings_ratio = ticker.price_to_earnings_ratio
 forecast_price_to_earnings__growth_rates = ticker.forecast_peg_rate
-```
+``` -->
 
 ## Stocks data from `Digrin` (web scraping):
 
 Data on Digrin website includes all historical data of the stock in certain categories, unlike Yahoo Finance which only provides the last 5 years of data at most.
 
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="digrin").ticker
+
 # Complete historical data of the stock in certain categories
 dividend = ticker.dividend
 payout_ratio = ticker.payout_ratio
 stock_splits = ticker.stock_splits
 ```
 
 ## EU ETF data from `justETF` (web scraping):
 
 For EU ETFS, the `isin` and `security_type` should be passed to the `Ticker` object. The `isin` is the International Securities Identification Number of the ETF and the `security_type` should be set to `etf`.
 
 ```python
-etf = Ticker(isin='IE00B4L5Y983', security_type='etf')
+from stockdex import TickerFactory
+
+etf = TickerFactory(isin="IE00B4L5Y983", security_type="etf", data_source="justetf").ticker
 
 etf_general_info = etf.etf_general_info
 etf_wkn = etf.etf_wkn
 etf_description = etf.etf_description
 
 # Basic data about the ETF
 etf_basics = etf.etf_basics
```

### Comparing `stockdex-0.4.0/README.md` & `stockdex-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 Stockdex is a Python package that provides a simple interface to access financial data from Yahoo Finance. Data is returned as a pandas DataFrame.
 
 # Installation 
 
 Install the package using pip:
 
 ```bash
-pip install stockdex
+pip install stockdex -U
 ``` 
 
 # Usage
 
-Create `Ticker` object by passing the ticker symbol. Ticker objects are the main interface to retrieve stock data.
-
+To access main functions, use `ticker`property from `TickerFactory` class. The `Ticker` class is used to access data from Various data sources. The `TickerFactory` class requires a data source to be passed to it. Here is an example of how to begin using the package:
 ```python
-from stockdex import Ticker
+from stockdex import TickerFactory
 
-# Pick arbitrary ticker
-ticker = Ticker('AAPL')
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_api").ticker
 ```
 
-## Fundamental data from `Yahoo Finance` API (fast queries through Yahoo Finance API):
+After creating the `Ticker` object, you can access functions defined for each data source. Below are some examples of how to access data from supported data sources.
+
+## Data from `Yahoo Finance` API (fast queries through Yahoo Finance API):
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_api").ticker
 
 # Price data (use range and dataGranularity to make range and granularity more specific)
 price = ticker.price(range='1y', dataGranularity='1d')
 
 # Current trading period of the stock (pre-market, regular, post-market trading periods)
 current_trading_period = ticker.current_trading_period
 
@@ -43,16 +46,20 @@
 income_statement = ticker.income_statement(frequency='quarterly')
 cash_flow = ticker.cash_flow(format='raw')
 balance_sheet = ticker.balance_sheet(period1=datetime(2020, 1, 1))
 financials = ticker.financials(period1=datetime(2022, 1, 1), period2=datetime.today())
 ```
 
 
-## Fundamental data with criteria from `Yahoo Finance` website (web scraping):
+## Data from `Yahoo Finance` website (web scraping):
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_web").ticker
+
 # Summary including general financial information
 summary = ticker.summary
 
 # Financial data as it is seen in the yahoo finance website
 income_stmt_web = ticker.income_stmt_web
 balance_sheet = ticker.balance_sheet_web
 cash_flow = ticker.cashflow_web
@@ -76,46 +83,52 @@
 
 # Statistics
 valuation_measures = ticker.valuation_measures
 financial_highlights = ticker.financial_highlights
 trading_information = ticker.trading_information
 ```
 
-## NASDAQ data from `NASDAQ` website (web scraping):
+<!-- ## NASDAQ data from `NASDAQ` website (web scraping):
 
 Data on NASDAQ website gets updated more frequently than Yahoo Finance data. Below are some of the data that can be retrieved from the NASDAQ website.
 
 ```python
 # Data about quarterly and yearly earnings, updated on the same day as the earnings release (yahoo finance data is updated after a few days)
 
 quarterly_earnings_surprise = ticker.quarterly_earnings_surprise
 yearly_earnings_forecast = ticker.yearly_earnings_forecast
 quarterly_earnings_forecast = ticker.quarterly_earnings_forecast
 
 price_to_earnings_ratio = ticker.price_to_earnings_ratio
 forecast_price_to_earnings__growth_rates = ticker.forecast_peg_rate
-```
+``` -->
 
 ## Stocks data from `Digrin` (web scraping):
 
 Data on Digrin website includes all historical data of the stock in certain categories, unlike Yahoo Finance which only provides the last 5 years of data at most.
 
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="digrin").ticker
+
 # Complete historical data of the stock in certain categories
 dividend = ticker.dividend
 payout_ratio = ticker.payout_ratio
 stock_splits = ticker.stock_splits
 ```
 
 ## EU ETF data from `justETF` (web scraping):
 
 For EU ETFS, the `isin` and `security_type` should be passed to the `Ticker` object. The `isin` is the International Securities Identification Number of the ETF and the `security_type` should be set to `etf`.
 
 ```python
-etf = Ticker(isin='IE00B4L5Y983', security_type='etf')
+from stockdex import TickerFactory
+
+etf = TickerFactory(isin="IE00B4L5Y983", security_type="etf", data_source="justetf").ticker
 
 etf_general_info = etf.etf_general_info
 etf_wkn = etf.etf_wkn
 etf_description = etf.etf_description
 
 # Basic data about the ETF
 etf_basics = etf.etf_basics
```

### Comparing `stockdex-0.4.0/setup.py` & `stockdex-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.4.0/stockdex/chromedriver_linux64/LICENSE.chromedriver` & `stockdex-0.5.0/stockdex/chromedriver_linux64/LICENSE.chromedriver`

 * *Files identical despite different names*

### Comparing `stockdex-0.4.0/stockdex/chromedriver_linux64/chromedriver` & `stockdex-0.5.0/stockdex/chromedriver_linux64/chromedriver`

 * *Files identical despite different names*

### Comparing `stockdex-0.4.0/stockdex/config.py` & `stockdex-0.5.0/stockdex/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File for configuration of the stockdex package
 
 from typing import Literal
 
 VALID_SECURITY_TYPES = Literal["stock", "etf", "cryptocurrency", "index", "commodity"]
+VALID_DATA_SOURCES = Literal["yahoo_web", "yahoo_api", "justetf", "digrin"]
 
 BASE_URL = "https://query2.finance.yahoo.com/v8/finance"
 FUNDAMENTALS_BASE_URL = (
     "https://query2.finance.yahoo.com/ws/fundamentals-timeseries/v1/finance/timeseries"
 )
 JUSTETF_BASE_URL = "https://www.justetf.com/en"
 NASDAQ_BASE_URL = "https://www.nasdaq.com/market-activity/stocks"
```

### Comparing `stockdex-0.4.0/stockdex/digrin_interface.py` & `stockdex-0.5.0/stockdex/digrin_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.4.0/stockdex/exceptions.py` & `stockdex-0.5.0/stockdex/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Module for custom exceptions
 """
 
+from stockdex.config import VALID_DATA_SOURCES
+
 
 class NoISINError(Exception):
     def __init__(self, message: str = "No ISIN provided") -> None:
         self.message = message
         super().__init__(self.message)
 
     def __str__(self) -> str:
@@ -38,7 +40,25 @@
         super().__init__(self.message)
 
     def __str__(self) -> str:
         return f"""
             {self.message}. Wrong security type has been used,
             make sure to use one of the following: {self.valid_types}
             """
+
+
+class WrongDataSource(Exception):
+    """
+    The exception to be shown when a method is called on the wrong data source
+    """
+
+    def __init__(
+        self,
+        given_source: str = None,
+    ) -> None:
+        self.given_source = given_source
+
+    def __str__(self) -> str:
+        return f"""
+            Wrong data source has been used,
+            make sure to use one of the following: {VALID_DATA_SOURCES}
+            """
```

### Comparing `stockdex-0.4.0/stockdex/justetf.py` & `stockdex-0.5.0/stockdex/justetf_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,51 +79,14 @@
 
         soup = BeautifulSoup(response.text, "html.parser")
 
         description = soup.find("div", {"id": "etf-description"}).text
 
         return description
 
-    # @property
-    # def etf_quote(self) -> pd.DataFrame:
-    #     """
-    #     Get the quote of the ETF
-
-    #     columns may include:
-    #     - Currency
-    #     - Price
-
-    #     Args:
-    #     ----------------
-    #     isin (str): ISIN of the ETF
-
-    #     Returns:
-    #     ----------------
-    #     pd.DataFrame: DataFrame containing the quote of the ETF
-    #     """
-    #     url = f"{JUSTETF_BASE_URL}/etf-profile.html?isin={self.isin}"
-
-    #     # build selenium interface object if not already built
-    #     if not hasattr(self, "selenium_interface"):
-    #         self.selenium_interface = selenium_interface()
-
-    #     soup = self.selenium_interface.get_html_content(url)
-
-    #     data_df = pd.DataFrame()
-
-    #     quote = soup.find("div", {"id": "realtime-quotes"})
-    #     currency, price = tuple(
-    #         quote.find("div", {"class": "col-xs-7"})
-    #         .find("div", {"class": "val"})
-    #         .text.split(" ")
-    #     )
-
-    #     data_df["currency"] = [currency]
-    #     data_df["price"] = [price]
-
     @property
     def etf_basics(self) -> pd.DataFrame:
         """
         Get the baisc information of the ETF
 
         columns may include:
         - Fund size
```

### Comparing `stockdex-0.4.0/stockdex/lib.py` & `stockdex-0.5.0/stockdex/lib.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.4.0/stockdex/nasdaq_interface.py` & `stockdex-0.5.0/stockdex/nasdaq_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,25 @@
         url = f"{NASDAQ_BASE_URL}/{self.ticker.lower()}/earnings"
 
         # build selenium interface object if not already built
         if not hasattr(self, "selenium_interface"):
             self.selenium_interface = selenium_interface(use_custom_user_agent=True)
 
         soup = self.selenium_interface.get_html_content(url)
+
+        # with open("earnings.html", "w") as f:
+        #     f.write(str(soup.prettify()))
+
+        # parent_div = self.find_parent_by_text(
+        #     soup=soup, tag="h2", text="Yearly Earnings Forecast"
+        # ).parent.parent
+
+        # table = parent_div.find("div", {"part": "table-row"})
+
+        # earnings_table = soup.find("div", {"class": "jupiter22-earnings-forecast"})
         earnings_table = soup.find("table", {"class": "earnings-forecast__table"})
 
         columns = earnings_table.find(
             "tr", {"class": "earnings-forecast__header"}
         ).find_all("th")
         columns = [column.text for column in columns]
 
@@ -174,16 +185,14 @@
         url = f"{NASDAQ_BASE_URL}/{self.ticker.lower()}/price-earnings-peg-ratios"
 
         # build selenium interface object if not already built
         if not hasattr(self, "selenium_interface"):
             self.selenium_interface = selenium_interface(use_custom_user_agent=True)
 
         soup = self.selenium_interface.get_html_content(url)
-        with open("nasdaq.html", "w") as f:
-            f.write(str(soup.prettify()))
 
         table = soup.find("tbody", {"class": "price-earnings-peg-ratios__table-body"})
         index, value = [], []
 
         for row in table.find_all("tr"):
             index.append(row.find("th").text)
             value.append(row.find("td").text)
@@ -205,16 +214,14 @@
         url = f"{NASDAQ_BASE_URL}/{self.ticker.lower()}/price-earnings-peg-ratios"
 
         # build selenium interface object if not already built
         if not hasattr(self, "selenium_interface"):
             self.selenium_interface = selenium_interface(use_custom_user_agent=True)
 
         soup = self.selenium_interface.get_html_content(url)
-        with open("nasdaq.html", "w") as f:
-            f.write(str(soup.prettify()))
 
         table = soup.find_all(
             "tbody", {"class": "price-earnings-peg-ratios__table-body"}
         )[1]
         index, value = [], []
 
         for row in table.find_all("tr"):
```

### Comparing `stockdex-0.4.0/stockdex/selenium_interface.py` & `stockdex-0.5.0/stockdex/selenium_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.4.0/stockdex/ticker_api.py` & `stockdex-0.5.0/stockdex/yahoo_api_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 
 from datetime import datetime
 from typing import Literal
 
 import pandas as pd
 
 from stockdex import config
-from stockdex.config import VALID_SECURITY_TYPES
+from stockdex.config import VALID_DATA_SOURCES, VALID_SECURITY_TYPES
 from stockdex.ticker_base import TickerBase
 
 
-class TickerAPI(TickerBase):
+class YahooAPI(TickerBase):
     def __init__(
         self,
         ticker: str = "",
         isin: str = "",
         security_type: VALID_SECURITY_TYPES = "stock",
+        data_source: VALID_DATA_SOURCES = "yahoo_api",
     ) -> None:
         self.ticker = ticker
         self.isin = isin
         self.security_type = security_type
+        self.data_source = data_source
 
     today = datetime.today()
     five_years_ago = today.replace(year=today.year - 5)
 
     def price(
         self,
         range: Literal[
```

### Comparing `stockdex-0.4.0/stockdex/ticker_base.py` & `stockdex-0.5.0/stockdex/ticker_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 Base class for ticker objects to inherit from
 """
 
+from typing import Union
+
 import requests
+from bs4 import BeautifulSoup
 
 from stockdex.lib import get_user_agent
 
 
 class TickerBase:
     request_headers = {
         "User-Agent": get_user_agent(),
@@ -28,7 +31,18 @@
         session = requests.Session()
         response = session.get(url, headers=self.request_headers, timeout=2)
         # If the HTTP GET request can't be served
         if response.status_code != 200:
             raise Exception("Failed to load page, check if the ticker symbol exists")
 
         return response
+
+    def find_parent_by_text(
+        self, soup: BeautifulSoup, tag: str, text: str
+    ) -> Union[None, str]:
+        """
+        Method that finds the parent of a tag by its text from a BeautifulSoup object
+        """
+        for element in soup.find_all(tag):
+            if text in element.get_text():
+                return element
+        return None
```

### Comparing `stockdex-0.4.0/stockdex/yahoo_web.py` & `stockdex-0.5.0/stockdex/yahoo_web_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,15 +428,21 @@
         # URL of the website to scrape
         url = f"https://finance.yahoo.com/quote/{self.ticker}/key-statistics"
         response = self.get_response(url)
 
         # Parse the HTML content of the website
         soup = BeautifulSoup(response.content, "html.parser")
 
-        table = soup.find("table", {"class": "table svelte-179gefj"})
+        # find element with test Valuation Measures
+        parent_section = self.find_parent_by_text(
+            soup, "h3", "Valuation Measures"
+        ).parent.parent
+
+        # looking for "table svelte-104jbnt"
+        table = parent_section.find("table")
 
         data_df = pd.DataFrame()
 
         headers = [item.text for item in table.find("thead").find("tr").find_all("th")]
         data_df = pd.DataFrame(columns=headers)
 
         for row in table.find("tbody").find_all("tr"):
```

### Comparing `stockdex-0.4.0/stockdex.egg-info/PKG-INFO` & `stockdex-0.5.0/stockdex.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -24,30 +24,33 @@
 Stockdex is a Python package that provides a simple interface to access financial data from Yahoo Finance. Data is returned as a pandas DataFrame.
 
 # Installation 
 
 Install the package using pip:
 
 ```bash
-pip install stockdex
+pip install stockdex -U
 ``` 
 
 # Usage
 
-Create `Ticker` object by passing the ticker symbol. Ticker objects are the main interface to retrieve stock data.
-
+To access main functions, use `ticker`property from `TickerFactory` class. The `Ticker` class is used to access data from Various data sources. The `TickerFactory` class requires a data source to be passed to it. Here is an example of how to begin using the package:
 ```python
-from stockdex import Ticker
+from stockdex import TickerFactory
 
-# Pick arbitrary ticker
-ticker = Ticker('AAPL')
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_api").ticker
 ```
 
-## Fundamental data from `Yahoo Finance` API (fast queries through Yahoo Finance API):
+After creating the `Ticker` object, you can access functions defined for each data source. Below are some examples of how to access data from supported data sources.
+
+## Data from `Yahoo Finance` API (fast queries through Yahoo Finance API):
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_api").ticker
 
 # Price data (use range and dataGranularity to make range and granularity more specific)
 price = ticker.price(range='1y', dataGranularity='1d')
 
 # Current trading period of the stock (pre-market, regular, post-market trading periods)
 current_trading_period = ticker.current_trading_period
 
@@ -55,16 +58,20 @@
 income_statement = ticker.income_statement(frequency='quarterly')
 cash_flow = ticker.cash_flow(format='raw')
 balance_sheet = ticker.balance_sheet(period1=datetime(2020, 1, 1))
 financials = ticker.financials(period1=datetime(2022, 1, 1), period2=datetime.today())
 ```
 
 
-## Fundamental data with criteria from `Yahoo Finance` website (web scraping):
+## Data from `Yahoo Finance` website (web scraping):
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="yahoo_web").ticker
+
 # Summary including general financial information
 summary = ticker.summary
 
 # Financial data as it is seen in the yahoo finance website
 income_stmt_web = ticker.income_stmt_web
 balance_sheet = ticker.balance_sheet_web
 cash_flow = ticker.cashflow_web
@@ -88,46 +95,52 @@
 
 # Statistics
 valuation_measures = ticker.valuation_measures
 financial_highlights = ticker.financial_highlights
 trading_information = ticker.trading_information
 ```
 
-## NASDAQ data from `NASDAQ` website (web scraping):
+<!-- ## NASDAQ data from `NASDAQ` website (web scraping):
 
 Data on NASDAQ website gets updated more frequently than Yahoo Finance data. Below are some of the data that can be retrieved from the NASDAQ website.
 
 ```python
 # Data about quarterly and yearly earnings, updated on the same day as the earnings release (yahoo finance data is updated after a few days)
 
 quarterly_earnings_surprise = ticker.quarterly_earnings_surprise
 yearly_earnings_forecast = ticker.yearly_earnings_forecast
 quarterly_earnings_forecast = ticker.quarterly_earnings_forecast
 
 price_to_earnings_ratio = ticker.price_to_earnings_ratio
 forecast_price_to_earnings__growth_rates = ticker.forecast_peg_rate
-```
+``` -->
 
 ## Stocks data from `Digrin` (web scraping):
 
 Data on Digrin website includes all historical data of the stock in certain categories, unlike Yahoo Finance which only provides the last 5 years of data at most.
 
 ```python
+from stockdex import TickerFactory
+
+ticker = TickerFactory(ticker="AAPL", data_source="digrin").ticker
+
 # Complete historical data of the stock in certain categories
 dividend = ticker.dividend
 payout_ratio = ticker.payout_ratio
 stock_splits = ticker.stock_splits
 ```
 
 ## EU ETF data from `justETF` (web scraping):
 
 For EU ETFS, the `isin` and `security_type` should be passed to the `Ticker` object. The `isin` is the International Securities Identification Number of the ETF and the `security_type` should be set to `etf`.
 
 ```python
-etf = Ticker(isin='IE00B4L5Y983', security_type='etf')
+from stockdex import TickerFactory
+
+etf = TickerFactory(isin="IE00B4L5Y983", security_type="etf", data_source="justetf").ticker
 
 etf_general_info = etf.etf_general_info
 etf_wkn = etf.etf_wkn
 etf_description = etf.etf_description
 
 # Basic data about the ETF
 etf_basics = etf.etf_basics
```

### Comparing `stockdex-0.4.0/stockdex.egg-info/SOURCES.txt` & `stockdex-0.5.0/stockdex.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 README.md
 setup.py
 stockdex/__init__.py
 stockdex/config.py
 stockdex/digrin_interface.py
 stockdex/exceptions.py
-stockdex/justetf.py
+stockdex/justetf_interface.py
 stockdex/lib.py
 stockdex/nasdaq_interface.py
 stockdex/selenium_interface.py
 stockdex/ticker.py
-stockdex/ticker_api.py
 stockdex/ticker_base.py
-stockdex/yahoo_web.py
+stockdex/yahoo_api_interface.py
+stockdex/yahoo_web_interface.py
 stockdex.egg-info/PKG-INFO
 stockdex.egg-info/SOURCES.txt
 stockdex.egg-info/dependency_links.txt
 stockdex.egg-info/requires.txt
 stockdex.egg-info/top_level.txt
 stockdex/chromedriver_linux64/LICENSE.chromedriver
 stockdex/chromedriver_linux64/chromedriver
 tests/__init__.py
 tests/test_digrin_interface.py
-tests/test_justetf.py
+tests/test_justetf_interface.py
 tests/test_nasdaq_interface.py
 tests/test_ticker.py
-tests/test_ticker_api.py
-tests/test_yahoo_web.py
+tests/test_yahoo_api_interface.py
+tests/test_yahoo_web_interface.py
```

### Comparing `stockdex-0.4.0/tests/test_digrin_interface.py` & `stockdex-0.5.0/tests/test_digrin_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Module to test the Digrin_Interface class
 """
 
 import pandas as pd
 import pytest
 
-from stockdex.ticker import Ticker
+from stockdex.ticker import TickerFactory
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("ASML"),
         ("CAT"),
         ("BAC"),
     ],
 )
 def test_dividend(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker=ticker, data_source="digrin").ticker
     dividend = ticker.dividend
 
     # Check if the response is as expected
     assert isinstance(dividend, pd.DataFrame)
     assert dividend.shape[0] > 0
     assert dividend.shape[1] == 5
 
@@ -34,15 +34,15 @@
         ("MSFT"),
         ("ASML"),
         ("CAT"),
         ("BAC"),
     ],
 )
 def test_payout_ratio(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker=ticker, data_source="digrin").ticker
     payout_ratio = ticker.payout_ratio
 
     # Check if the response is as expected
     assert isinstance(payout_ratio, pd.DataFrame)
     assert payout_ratio.shape[0] > 1
     assert payout_ratio.shape[1] == 2
 
@@ -54,14 +54,14 @@
         ("MSFT"),
         ("ASML"),
         ("CAT"),
         ("BAC"),
     ],
 )
 def test_stock_splits(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker=ticker, data_source="digrin").ticker
     stock_splits = ticker.stock_splits
 
     # Check if the response is as expected
     assert isinstance(stock_splits, pd.DataFrame)
     assert stock_splits.shape[0] > 1
     assert stock_splits.shape[1] == 2
```

### Comparing `stockdex-0.4.0/tests/test_justetf.py` & `stockdex-0.5.0/tests/test_justetf_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 Module to test the justetf module.
 """
 
 import pandas as pd
 import pytest
 
 from stockdex.exceptions import WrongSecurityType
-from stockdex.ticker import Ticker
+from stockdex.ticker import TickerFactory
 
 
 @pytest.mark.parametrize(
     "isin",
     [
         ("IE00B4L5Y983"),
         ("IE00B53SZB19"),
     ],
 )
 def test_etf_general_info(isin: str) -> None:
     """
     Test the ter property of the JustETF class
     """
-    etf = Ticker(isin=isin, security_type="etf")
+    etf = TickerFactory(isin=isin, security_type="etf", data_source="justetf").ticker
 
     etf_general_info = etf.etf_general_info
     assert isinstance(etf_general_info, pd.DataFrame)
     assert etf_general_info.shape[0] == 1
     assert etf_general_info.shape[1] >= 5
     assert etf_general_info.iloc[0]["TER"] != ""
     for i in range(1, etf_general_info.shape[1]):
@@ -32,77 +32,89 @@
 
 
 def test_etf_general_info_wrong_security_type() -> None:
     """
     Test the WrongSecurityType exception
     """
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="IE00B4L5Y983", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            isin="IE00B4L5Y983",
+            security_type="wrong_security_type",
+            data_source="justetf",
+        ).ticker
         ticker.etf_general_info
 
 
 @pytest.mark.parametrize(
     "isin, expected",
     [
         ("IE00B4L5Y983", "A0RPWH"),
         ("IE00B53SZB19", "A0YEDL"),
     ],
 )
 def test_etf_wkn(isin: str, expected: str) -> None:
     """
     Test the wkn property of the JustETF class
     """
-    etf = Ticker(isin=isin, security_type="etf")
+    etf = TickerFactory(isin=isin, security_type="etf", data_source="justetf").ticker
 
     etf_wkn = etf.etf_wkn
     assert isinstance(etf_wkn, str)
     assert etf_wkn == expected
 
 
 def test_etf_wkn_wrong_security_type() -> None:
     """
     Test the WrongSecurityType exception
     """
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="IE00B4L5Y983", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            isin="IE00B4L5Y983",
+            security_type="wrong_security_type",
+            data_source="justetf",
+        ).ticker
         ticker.etf_wkn
 
 
 def test_no_isin() -> None:
     """
     Test the NoISINError exception
     """
     with pytest.raises(Exception):
-        Ticker(isin="", security_type="etf")
+        TickerFactory(isin="", security_type="etf", data_source="justetf").ticker
 
 
 @pytest.mark.parametrize(
     "isin",
     [
         ("IE00B4L5Y983"),
         ("IE00B53SZB19"),
     ],
 )
 def test_etf_description(isin: str) -> None:
     """
     Test the description property of the JustETF class
     """
-    etf = Ticker(isin=isin, security_type="etf")
+    etf = TickerFactory(isin=isin, security_type="etf", data_source="justetf").ticker
 
     etf_description = etf.etf_description
     assert isinstance(etf_description, str)
     assert len(etf_description) > 0
 
 
 def test_etf_description_wrong_security_type() -> None:
     """
     Test the WrongSecurityType exception
     """
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="IE00B4L5Y983", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            isin="IE00B4L5Y983",
+            security_type="wrong_security_type",
+            data_source="justetf",
+        ).ticker
         ticker.etf_description
 
 
 # @pytest.mark.parametrize(
 #     "isin",
 #     [
 #         ("IE00B4L5Y983"),
@@ -126,15 +138,15 @@
         ("IE00B53SZB19"),
     ],
 )
 def test_etf_basics(isin: str) -> None:
     """
     Test the etf_basics property of the JustETF class
     """
-    etf = Ticker(isin=isin, security_type="etf")
+    etf = TickerFactory(isin=isin, security_type="etf", data_source="justetf").ticker
 
     etf_basics = etf.etf_basics
     assert isinstance(etf_basics, pd.DataFrame)
     assert etf_basics.shape[0] == 1
     assert etf_basics.shape[1] >= 5
 
     expceted_columns = [
@@ -150,43 +162,51 @@
 
 
 def test_etf_basics_wrong_security_type() -> None:
     """
     Test the WrongSecurityType exception
     """
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="IE00B4L5Y983", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            isin="IE00B4L5Y983",
+            security_type="wrong_security_type",
+            data_source="justetf",
+        ).ticker
         ticker.etf_basics
 
 
 @pytest.mark.parametrize(
     "isin",
     [
         ("IE00B4L5Y983"),
         ("IE00B53SZB19"),
     ],
 )
 def test_etf_holdings_companies(isin: str) -> None:
     """
     Test the etf_holdings property of the JustETF class
     """
-    etf = Ticker(isin=isin, security_type="etf")
+    etf = TickerFactory(isin=isin, security_type="etf", data_source="justetf").ticker
 
     etf_holdings = etf.etf_holdings_companies
     assert isinstance(etf_holdings, pd.DataFrame)
     assert etf_holdings.shape[0] == 10
     assert etf_holdings.shape[1] == 1
 
 
 def test_etf_holdings_companies_wrong_security_type() -> None:
     """
     Test the WrongSecurityType exception
     """
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="IE00B4L5Y983", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            isin="IE00B4L5Y983",
+            security_type="wrong_security_type",
+            data_source="justetf",
+        ).ticker
         ticker.etf_holdings_companies
 
 
 @pytest.mark.parametrize(
     "isin",
     [
         ("IE00B4L5Y983"),
@@ -194,28 +214,32 @@
     ],
 )
 def test_etf_holdings_countries(isin: str) -> None:
     """
     Test the etf_holdings property of the JustETF class
     """
 
-    etf = Ticker(isin=isin, security_type="etf")
+    etf = TickerFactory(isin=isin, security_type="etf", data_source="justetf").ticker
 
     etf_holdings = etf.etf_holdings_countries
     assert isinstance(etf_holdings, pd.DataFrame)
     assert etf_holdings.shape[0] >= 2
     assert etf_holdings.shape[1] == 1
 
 
 def test_etf_holdings_countries_wrong_security_type() -> None:
     """
     Test the WrongSecurityType exception
     """
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="IE00B4L5Y983", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            isin="IE00B4L5Y983",
+            security_type="wrong_security_type",
+            data_source="justetf",
+        ).ticker
         ticker.etf_holdings_countries
 
 
 @pytest.mark.parametrize(
     "isin",
     [
         ("IE00B4L5Y983"),
@@ -223,22 +247,26 @@
     ],
 )
 def test_etf_holdings_sectors(isin: str) -> None:
     """
     Test the etf_holdings property of the JustETF class
     """
 
-    etf = Ticker(isin=isin, security_type="etf")
+    etf = TickerFactory(isin=isin, security_type="etf", data_source="justetf").ticker
 
     etf_holdings = etf.etf_holdings_sectors
     assert isinstance(etf_holdings, pd.DataFrame)
     assert etf_holdings.shape[0] >= 2
     assert etf_holdings.shape[1] == 1
 
 
 def test_etf_holdings_sectors_wrong_security_type() -> None:
     """
     Test the WrongSecurityType exception
     """
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="IE00B4L5Y983", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            isin="IE00B4L5Y983",
+            security_type="wrong_security_type",
+            data_source="justetf",
+        ).ticker
         ticker.etf_holdings_sectors
```

### Comparing `stockdex-0.4.0/tests/test_nasdaq_interface.py` & `stockdex-0.5.0/tests/test_nasdaq_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 Module to test the NasdaqInterface class
 """
 
 import pandas as pd
 import pytest
 
 from stockdex.exceptions import WrongSecurityType
-from stockdex.ticker import Ticker
+from stockdex.ticker import TickerFactory
+
+pytestmark = pytest.mark.skip(
+    reason="""Skip the entire module as nasdaq is
+              not supported anymore due to nasdaq
+              website changes"""
+)
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("NVDA"),
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_quarterly_earnings_surprise(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="nasdaq").ticker
     response = ticker.quarterly_earnings_surprise
 
     assert response is not None
     assert isinstance(response, pd.DataFrame)
     assert response.shape[0] > 1
     assert response.shape[1] > 1
 
@@ -35,29 +41,31 @@
         "% Surprise",
     ]
     assert response.columns.tolist() == expected_columns
 
 
 def test_quarterly_earnings_surprise_wrong_securiy_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(ticker="AAPL", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="wrong_security_type", data_source="nasdaq"
+        ).ticker
         ticker.quarterly_earnings_surprise
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("NVDA"),
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_yearly_earnings_forecast(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="nasdaq").ticker
     response = ticker.yearly_earnings_forecast
 
     assert response is not None
     assert isinstance(response, pd.DataFrame)
     assert response.shape[0] > 1
     assert response.shape[1] > 1
 
@@ -70,29 +78,31 @@
 
     for column in expected_columns:
         assert column in response.columns.tolist()
 
 
 def test_yearly_earnings_forecast_wrong_securiy_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(ticker="AAPL", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="wrong_security_type", data_source="nasdaq"
+        ).ticker
         ticker.yearly_earnings_forecast
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("NVDA"),
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_quarterly_earnings_forecast(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="nasdaq").ticker
     response = ticker.quarterly_earnings_forecast
 
     assert response is not None
     assert isinstance(response, pd.DataFrame)
     assert response.shape[0] > 1
     assert response.shape[1] > 1
 
@@ -105,59 +115,65 @@
 
     for column in expected_columns:
         assert column in response.columns.tolist()
 
 
 def test_quarterly_earnings_forecast_wrong_securiy_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(ticker="AAPL", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="wrong_security_type", data_source="nasdaq"
+        ).ticker
         ticker.quarterly_earnings_forecast
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("NVDA"),
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_price_to_earnings_ratio(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="nasdaq").ticker
     price_to_earnings_ratio = ticker.price_to_earnings_ratio
 
     assert price_to_earnings_ratio is not None
     assert isinstance(price_to_earnings_ratio, pd.DataFrame)
     assert price_to_earnings_ratio.shape[0] > 1
     assert price_to_earnings_ratio.shape[1] == 1
 
 
 def test_price_to_earnings_ratio_wrong_securiy_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(ticker="AAPL", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="wrong_security_type", data_source="nasdaq"
+        ).ticker
         ticker.price_to_earnings_ratio
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("NVDA"),
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_forecast_peg_rate(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="nasdaq").ticker
     forecast_peg_rate = ticker.forecast_peg_rate
 
     assert forecast_peg_rate is not None
     assert isinstance(forecast_peg_rate, pd.DataFrame)
     assert forecast_peg_rate.shape[0] > 1
     assert forecast_peg_rate.shape[1] == 1
 
 
 def test_forecast_peg_rate_wrong_securiy_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(ticker="AAPL", security_type="wrong_security_type")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="wrong_security_type", data_source="nasdaq"
+        ).ticker
         ticker.forecast_peg_rate
```

### Comparing `stockdex-0.4.0/tests/test_ticker.py` & `stockdex-0.5.0/tests/test_ticker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import pytest
 
-from stockdex.ticker import Ticker
+from stockdex.exceptions import WrongDataSource
+from stockdex.ticker import TickerFactory
 
 
 @pytest.mark.parametrize(
     "ticker, expected_response",
     [
         ("AAPL", 200),
         ("GOOGL", 200),
         ("MSFT", 200),
     ],
 )
 def test_get_response(ticker, expected_response):
     # Create a Ticker object
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker=ticker).ticker
 
     # Send an HTTP GET request to the website
     response = ticker.get_response(f"https://finance.yahoo.com/quote/{ticker.ticker}")
 
     # Check if the response is as expected
     assert response.status_code == expected_response
+
+
+def test_data_source_invalid():
+    # Create a Ticker object
+    ticker = TickerFactory(ticker="AAPL")
+
+    # Check if the exception is raised
+    with pytest.raises(WrongDataSource):
+        ticker.data_source = "invalid_data_source"
```

### Comparing `stockdex-0.4.0/tests/test_ticker_api.py` & `stockdex-0.5.0/tests/test_yahoo_api_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 import pandas as pd
 import pytest
 
-from stockdex.ticker import Ticker
+from stockdex.ticker import TickerFactory
 
 
 @pytest.mark.parametrize(
     "ticker, range, dataGranularity",
     [
         ("AAPL", "1d", "1h"),
         ("GOOGL", "1d", "1h"),
@@ -17,18 +17,18 @@
         ("MSFT", "1d", "1d"),
         ("NVDA", "max", "3mo"),
         ("SAP", "1y", "1mo"),
     ],
 )
 def test_price(ticker, range, dataGranularity):
     """
-    Test the price property of the TickerAPI class
+    Test the price property of the YahooAPI class
     """
 
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker).ticker
     price = ticker.price(range=range, dataGranularity=dataGranularity)
 
     assert price.columns.tolist() == [
         "timestamp",
         "volume",
         "close",
         "open",
@@ -48,18 +48,18 @@
     [
         ("AAPL"),
         ("ASML"),
     ],
 )
 def test_current_trading_period(ticker):
     """
-    Test the price property of the TickerAPI class
+    Test the price property of the YahooAPI class
     """
 
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker).ticker
     current_trading_period = ticker.current_trading_period
 
     assert current_trading_period.columns.tolist() == [
         "pre",
         "regular",
         "post",
     ]
@@ -83,15 +83,15 @@
         ("GOOGL", "quarterly", "fmt", datetime(2021, 1, 1), datetime.today()),
         ("MSFT", "quarterly", "fmt", datetime(2023, 1, 1), datetime(2024, 1, 1)),
         ("NVDA", "quarterly", "raw", datetime(2020, 1, 1), datetime.today()),
         ("FMC", "quarterly", "raw", datetime(2021, 1, 1), datetime.today()),
     ],
 )
 def test_income_statement(ticker, frequency, format, period1, period2):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker).ticker
     income_statement = ticker.income_statement(
         frequency=frequency, format=format, period1=period1, period2=period2
     )
 
     assert isinstance(income_statement, pd.DataFrame)
     assert income_statement.shape[0] > 0
     assert income_statement.shape[1] > 0
@@ -104,15 +104,15 @@
         ("GOOGL", "quarterly", "fmt", datetime(2021, 1, 1), datetime.today()),
         ("MSFT", "quarterly", "fmt", datetime(2023, 1, 1), datetime(2024, 1, 1)),
         ("NVDA", "quarterly", "raw", datetime(2020, 1, 1), datetime.today()),
         ("FMC", "quarterly", "raw", datetime(2021, 1, 1), datetime.today()),
     ],
 )
 def test_cash_flow(ticker, frequency, format, period1, period2):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker).ticker
     cash_flow = ticker.cash_flow(
         frequency=frequency, format=format, period1=period1, period2=period2
     )
 
     assert isinstance(cash_flow, pd.DataFrame)
     assert cash_flow.shape[0] > 0
     assert cash_flow.shape[1] > 0
@@ -125,15 +125,15 @@
         ("GOOGL", "quarterly", "fmt", datetime(2021, 1, 1), datetime.today()),
         ("MSFT", "quarterly", "fmt", datetime(2023, 1, 1), datetime(2024, 1, 1)),
         ("NVDA", "quarterly", "raw", datetime(2020, 1, 1), datetime.today()),
         ("FMC", "quarterly", "raw", datetime(2021, 1, 1), datetime.today()),
     ],
 )
 def test_balance_sheet(ticker, frequency, format, period1, period2):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker).ticker
     balance_sheet = ticker.balance_sheet(
         frequency=frequency, format=format, period1=period1, period2=period2
     )
 
     assert isinstance(balance_sheet, pd.DataFrame)
     assert balance_sheet.shape[0] > 0
     assert balance_sheet.shape[1] > 0
@@ -146,15 +146,15 @@
         ("GOOGL", "quarterly", "fmt", datetime(2021, 1, 1), datetime.today()),
         ("MSFT", "quarterly", "fmt", datetime(2023, 1, 1), datetime(2024, 1, 1)),
         ("NVDA", "quarterly", "raw", datetime(2020, 1, 1), datetime.today()),
         ("FMC", "quarterly", "raw", datetime(2021, 1, 1), datetime.today()),
     ],
 )
 def test_financials(ticker, frequency, format, period1, period2):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker).ticker
     financials = ticker.financials(
         frequency=frequency, format=format, period1=period1, period2=period2
     )
 
     assert isinstance(financials, pd.DataFrame)
     assert financials.shape[0] > 0
     assert financials.shape[1] > 0
```

### Comparing `stockdex-0.4.0/tests/test_yahoo_web.py` & `stockdex-0.5.0/tests/test_yahoo_web_interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,140 +2,154 @@
 Module to test the YahooWeb class.
 """
 
 import pandas as pd
 import pytest
 
 from stockdex.exceptions import WrongSecurityType
-from stockdex.ticker import Ticker
+from stockdex.ticker import TickerFactory
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_cashflow_web(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     cashflow_web_df = ticker.cashflow_web
 
     # Check if the response is as expected
     assert isinstance(cashflow_web_df, pd.DataFrame)
     assert cashflow_web_df.shape[0] >= 3
     assert cashflow_web_df.shape[1] > 5
 
 
 def test_cashflow_web_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.cashflow_web
 
 
 @pytest.mark.parametrize(
     "ticker",
     [("AAPL"), ("GOOGL"), ("TSLA")],
 )
 def test_balance_sheet_web(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     balance_sheet_web_df = ticker.balance_sheet_web
 
     # Check if the response is as expected
     assert isinstance(balance_sheet_web_df, pd.DataFrame)
     assert balance_sheet_web_df.shape[0] >= 3
     assert balance_sheet_web_df.shape[1] > 5
 
 
 def test_balance_sheet_web_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.balance_sheet_web
 
 
 @pytest.mark.parametrize(
     "ticker",
     [("AAPL"), ("GOOGL"), ("TSLA")],
 )
 def test_income_stmt_web(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     income_stmt_web_df = ticker.income_stmt_web
 
     # Check if the response is as expected
     assert isinstance(income_stmt_web_df, pd.DataFrame)
     assert income_stmt_web_df.shape[0] >= 3
     assert income_stmt_web_df.shape[1] > 5
 
 
 def test_income_stmt_web_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.income_stmt_web
 
 
 @pytest.mark.parametrize(
     "ticker, security_type",
     [
         ("AAPL", "stock"),
         ("GOOGL", "stock"),
         ("MSFT", "stock"),
         ("QQQ", "etf"),
     ],
 )
 def test_calls(ticker, security_type):
-    ticker = Ticker(ticker, security_type=security_type)
+    ticker = TickerFactory(
+        ticker, security_type=security_type, data_source="yahoo_web"
+    ).ticker
     calls = ticker.calls
 
     # Check if the response is as expected
     assert isinstance(calls, pd.DataFrame)
     assert calls.shape[0] > 0
 
 
 def test_calls_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="wrong_type")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="wrong_type", data_source="yahoo_web"
+        ).ticker
         ticker.calls
 
 
 @pytest.mark.parametrize(
     "ticker, security_type",
     [
         ("AAPL", "stock"),
         ("GOOGL", "stock"),
         ("MSFT", "stock"),
         ("QQQ", "etf"),
     ],
 )
 def test_puts(ticker, security_type):
-    ticker = Ticker(ticker, security_type=security_type)
+    ticker = TickerFactory(
+        ticker, security_type=security_type, data_source="yahoo_web"
+    ).ticker
     puts = ticker.puts
 
     # Check if the response is as expected
     assert isinstance(puts, pd.DataFrame)
     assert puts.shape[0] > 0
 
 
 def test_puts_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="wrong_type")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="wrong_type", data_source="yahoo_web"
+        ).ticker
         ticker.puts
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("ASML"),
         ("TSLA"),
     ],
 )
 def test_description(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     description = ticker.description
 
     # Check if the response is as expected
     assert isinstance(description, str)
     assert len(description) > 0
 
 
@@ -143,170 +157,184 @@
     "ticker",
     [
         ("AAPL"),
         ("TSLA"),
     ],
 )
 def test_key_executives(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     key_executives = ticker.key_executives
 
     # Check if the response is as expected
     assert isinstance(key_executives, pd.DataFrame)
     assert key_executives.shape[0] > 0
 
 
 def test_key_executives_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.key_executives
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("ASML"),
         ("TSLA"),
     ],
 )
 def test_corporate_governance(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     corporate_governance = ticker.corporate_governance
 
     # Check if the response is as expected
     assert isinstance(corporate_governance, str)
     assert len(corporate_governance) > 0
 
 
 def test_corporate_governance_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.corporate_governance
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("ASML"),
         ("TSLA"),
     ],
 )
 def test_major_holders(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     major_holders = ticker.major_holders
 
     # Check if the response is as expected
     assert isinstance(major_holders, pd.DataFrame)
     assert major_holders.shape[0] > 0
     assert major_holders.shape[1] == 2
 
 
 def test_major_holders_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.major_holders
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("ASML"),
         ("TSLA"),
     ],
 )
 def test_top_institutional_holders(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     top_institutional_holders = ticker.top_institutional_holders
 
     # Check if the response is as expected
     assert isinstance(top_institutional_holders, pd.DataFrame)
     assert top_institutional_holders.shape[0] > 0
     assert top_institutional_holders.shape[1] == 5
 
 
 def test_top_institutional_holders_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.top_institutional_holders
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("ASML"),
         ("TSLA"),
     ],
 )
 def test_top_mutual_fund_holders(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     top_mutual_fund_holders = ticker.top_mutual_fund_holders
 
     # Check if the response is as expected
     assert isinstance(top_mutual_fund_holders, pd.DataFrame)
     assert top_mutual_fund_holders.shape[0] > 0
     assert top_mutual_fund_holders.shape[1] == 5
 
 
 def test_top_mutual_fund_holders_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.top_mutual_fund_holders
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_summary(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     summary_df = ticker.summary
 
     # Check if the response is as expected
     assert isinstance(summary_df, pd.DataFrame)
     assert summary_df.shape[0] > 0
 
 
 def test_summary_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.summary
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_analysis(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     analysis_df = ticker.analysis
 
     # Check if the response is as expected
     assert isinstance(analysis_df, pd.DataFrame)
     assert analysis_df.shape[0] > 0
 
 
 def test_analysis_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.analysis
 
 
 # @pytest.mark.skip(
 #     reason="This test is skipped because github actions is not able to access the yahoo finance page"  # noqa E501
 # )
 @pytest.mark.parametrize(
@@ -314,71 +342,77 @@
     [
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_valuation_measures(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     valuation_measures_df = ticker.valuation_measures
 
     # Check if the response is as expected
     assert isinstance(valuation_measures_df, pd.DataFrame)
     assert valuation_measures_df.shape[0] > 0
     assert valuation_measures_df.shape[1] > 3
     assert isinstance(valuation_measures_df.iloc[0, 0], (int, float, str))
 
 
 def test_valuation_measures_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.valuation_measures
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_financial_highlights(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     financial_highlights_df = ticker.financial_highlights
 
     # Check if the response is as expected
     assert isinstance(financial_highlights_df, pd.DataFrame)
     assert financial_highlights_df.shape[0] > 0
     assert financial_highlights_df.shape[1] == 1
     assert isinstance(financial_highlights_df.iloc[0, 0], (int, float, str))
 
 
 def test_financial_highlights_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.financial_highlights
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
         ("GOOGL"),
         ("MSFT"),
     ],
 )
 def test_trading_information(ticker):
-    ticker = Ticker(ticker)
+    ticker = TickerFactory(ticker, data_source="yahoo_web").ticker
     trading_information_df = ticker.trading_information
 
     # Check if the response is as expected
     assert isinstance(trading_information_df, pd.DataFrame)
     assert trading_information_df.shape[0] > 0
     assert trading_information_df.shape[1] == 1
     assert isinstance(trading_information_df.iloc[0, 0], (int, float, str))
 
 
 def test_trading_information_wrong_security_type():
     with pytest.raises(WrongSecurityType):
-        ticker = Ticker(isin="AAPL", security_type="etf")
+        ticker = TickerFactory(
+            ticker="AAPL", security_type="etf", data_source="yahoo_web"
+        ).ticker
         ticker.trading_information
```

