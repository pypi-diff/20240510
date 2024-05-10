# Comparing `tmp/lumibot-3.4.0.tar.gz` & `tmp/lumibot-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.4.0.tar", last modified: Wed May  8 05:18:01 2024, max compression
+gzip compressed data, was "lumibot-3.4.1.tar", last modified: Fri May 10 18:40:36 2024, max compression
```

## Comparing `lumibot-3.4.0.tar` & `lumibot-3.4.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.778898 lumibot-3.4.0/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.4.0/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-08 05:18:01.778836 lumibot-3.4.0/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.4.0/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.765012 lumibot-3.4.0/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.766736 lumibot-3.4.0/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    31484 2024-04-10 21:16:31.000000 lumibot-3.4.0/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    14588 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.767959 lumibot-3.4.0/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    42389 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-04-16 22:57:26.000000 lumibot-3.4.0/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    27085 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.769849 lumibot-3.4.0/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.4.0/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.4.0/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15512 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.4.0/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.4.0/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.771091 lumibot-3.4.0/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.4.0/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21849 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28373 2024-05-08 05:17:06.000000 lumibot-3.4.0/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.772752 lumibot-3.4.0/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-04-16 22:57:26.000000 lumibot-3.4.0/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.4.0/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.773453 lumibot-3.4.0/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53879 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   149930 2024-04-16 01:12:34.000000 lumibot-3.4.0/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39943 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.774978 lumibot-3.4.0/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.4.0/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26283 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.4.0/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15762 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.775319 lumibot-3.4.0/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7995 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.775667 lumibot-3.4.0/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.778519 lumibot-3.4.0/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3260 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.4.0/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-05-08 05:18:01.779197 lumibot-3.4.0/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1809 2024-05-08 05:17:27.000000 lumibot-3.4.0/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.777443 lumibot-3.4.0/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.778346 lumibot-3.4.0/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      553 2024-05-08 03:43:54.000000 lumibot-3.4.0/tests/backtest/fixtures.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    17600 2024-05-08 03:43:54.000000 lumibot-3.4.0/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1928 2024-05-08 03:43:54.000000 lumibot-3.4.0/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.4.0/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.4.0/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.514211 lumibot-3.4.1/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.4.1/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-10 18:40:36.514111 lumibot-3.4.1/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.4.1/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.501153 lumibot-3.4.1/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.502671 lumibot-3.4.1/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    31699 2024-05-10 17:14:24.000000 lumibot-3.4.1/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    14588 2024-05-08 03:43:54.000000 lumibot-3.4.1/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.503419 lumibot-3.4.1/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    42389 2024-05-08 03:43:54.000000 lumibot-3.4.1/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-04-16 22:57:26.000000 lumibot-3.4.1/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    27085 2024-05-08 03:43:54.000000 lumibot-3.4.1/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.505091 lumibot-3.4.1/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.4.1/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.4.1/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15521 2024-05-10 17:41:22.000000 lumibot-3.4.1/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.4.1/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.4.1/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.506415 lumibot-3.4.1/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9605 2024-05-10 17:15:05.000000 lumibot-3.4.1/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21849 2024-05-08 03:43:54.000000 lumibot-3.4.1/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28373 2024-05-08 05:17:06.000000 lumibot-3.4.1/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.507702 lumibot-3.4.1/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-04-16 22:57:26.000000 lumibot-3.4.1/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.4.1/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.508310 lumibot-3.4.1/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53859 2024-05-10 16:59:36.000000 lumibot-3.4.1/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   149930 2024-04-16 01:12:34.000000 lumibot-3.4.1/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39943 2024-05-08 03:43:54.000000 lumibot-3.4.1/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.510058 lumibot-3.4.1/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.4.1/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26283 2024-05-08 03:43:54.000000 lumibot-3.4.1/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.4.1/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15762 2024-05-08 03:43:54.000000 lumibot-3.4.1/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.510311 lumibot-3.4.1/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7997 2024-05-10 16:59:36.000000 lumibot-3.4.1/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.510637 lumibot-3.4.1/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.4.1/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.513436 lumibot-3.4.1/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-10 18:40:36.000000 lumibot-3.4.1/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3260 2024-05-10 18:40:36.000000 lumibot-3.4.1/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-10 18:40:36.000000 lumibot-3.4.1/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-05-10 18:40:36.000000 lumibot-3.4.1/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-05-10 18:40:36.000000 lumibot-3.4.1/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.4.1/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-05-10 18:40:36.514670 lumibot-3.4.1/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1809 2024-05-10 18:38:57.000000 lumibot-3.4.1/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.512334 lumibot-3.4.1/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-10 18:40:36.513229 lumibot-3.4.1/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      553 2024-05-08 03:43:54.000000 lumibot-3.4.1/tests/backtest/fixtures.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    17580 2024-05-10 16:59:36.000000 lumibot-3.4.1/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1928 2024-05-08 03:43:54.000000 lumibot-3.4.1/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.4.1/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.4.1/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.4.1/tests/test_tradingfee.py
```

### Comparing `lumibot-3.4.0/LICENSE` & `lumibot-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/PKG-INFO` & `lumibot-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.4.0
+Version: 3.4.1
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.4.0/README.md` & `lumibot-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/__init__.py` & `lumibot-3.4.1/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.4.1/lumibot/backtesting/backtesting_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,19 +400,23 @@
             return
 
         # Check that the position is an options contract
         if position.asset.asset_type != "option":
             logging.error(f"Cannot cash settle non-option contract {position.asset}")
             return
 
-        # Create a stock asset for the underlying asset
-        underlying_asset = Asset(
-            symbol=position.asset.symbol,
-            asset_type="stock",
-        )
+        # First check if the option asset has an underlying asset
+        if position.asset.underlying_asset is None:
+            # Create a stock asset for the underlying asset
+            underlying_asset = Asset(
+                symbol=position.asset.symbol,
+                asset_type="stock",
+            )
+        else:
+            underlying_asset = position.asset.underlying_asset
 
         # Get the price of the underlying asset
         underlying_price = self.get_last_price(underlying_asset)
 
         # Calculate profit/loss per contract
         if position.asset.right == "CALL":
             profit_loss_per_contract = underlying_price - position.asset.strike
```

### Comparing `lumibot-3.4.0/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.4.1/lumibot/backtesting/polygon_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/brokers/alpaca.py` & `lumibot-3.4.1/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/brokers/broker.py` & `lumibot-3.4.1/lumibot/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/brokers/ccxt.py` & `lumibot-3.4.1/lumibot/brokers/ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/brokers/interactive_brokers.py` & `lumibot-3.4.1/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/brokers/tradier.py` & `lumibot-3.4.1/lumibot/brokers/tradier.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/alpaca_data.py` & `lumibot-3.4.1/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.4.1/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.4.1/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/ccxt_data.py` & `lumibot-3.4.1/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/data_source.py` & `lumibot-3.4.1/lumibot/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.4.1/lumibot/data_sources/data_source_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/exceptions.py` & `lumibot-3.4.1/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.4.1/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/pandas_data.py` & `lumibot-3.4.1/lumibot/data_sources/pandas_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     def find_asset_in_data_store(self, asset, quote=None):
         if asset in self._data_store:
             return asset
         elif quote is not None:
             asset = (asset, quote)
             if asset in self._data_store:
                 return asset
-        elif isinstance(asset, Asset) and asset.asset_type in ["option", "future", "stock"]:
+        elif isinstance(asset, Asset) and asset.asset_type in ["option", "future", "stock", "index"]:
             asset = (asset, Asset("USD", "forex"))
             if asset in self._data_store:
                 return asset
         return None
 
     def _pull_source_symbol_bars(
         self,
```

### Comparing `lumibot-3.4.0/lumibot/data_sources/tradier_data.py` & `lumibot-3.4.1/lumibot/data_sources/tradier_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/data_sources/yahoo_data.py` & `lumibot-3.4.1/lumibot/data_sources/yahoo_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/entities/asset.py` & `lumibot-3.4.1/lumibot/entities/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         Options strike as string.
     right : str
         'CALL' or 'PUT'
         default : ""
     multiplier : int
         Price multiplier.
         default : 1
+    underlying_asset : Asset
+        Underlying asset for options.
 
     Attributes
     ----------
     symbol : string (required)
         The symbol used to retrieve stock quotes if stock. The underlying
         symbol if option. For Forex: The base currency.
     asset_type : (string, default: `stock`)
@@ -114,14 +116,15 @@
     symbol: str
     asset_type: str = "stock"
     expiration: date = None
     strike: float = 0.0
     right: str = None
     multiplier: int = 1
     precision: str = None
+    underlying_asset: "Asset" = None
 
     # Pull the asset types from the AssetType class
     _asset_types: list = [v for k, v in AssetType.__dict__.items() if not k.startswith("__")]
 
     # Pull the rights from the OptionRight class
     _right: list = [v for k, v in OptionRight.__dict__.items() if not k.startswith("__")]
 
@@ -130,20 +133,26 @@
         symbol: str,
         asset_type: str = "stock",
         expiration: date = None,
         strike: float = 0.0,
         right: str = None,
         multiplier: int = 1,
         precision: str = None,
+        underlying_asset: "Asset" = None,
     ):
         self.symbol = symbol
         self.asset_type = asset_type
         self.strike = strike
         self.multiplier = multiplier
         self.precision = precision
+        self.underlying_asset = underlying_asset
+
+        # If the underlying asset is set but the symbol is not, set the symbol to the underlying asset symbol
+        if self.underlying_asset is not None and self.symbol is None:
+            self.symbol = self.underlying_asset.symbol
 
         # If the expiration is a datetime object, convert it to date
         if isinstance(expiration, datetime):
             self.expiration = expiration.date()
         else:
             self.expiration = expiration
```

### Comparing `lumibot-3.4.0/lumibot/entities/bar.py` & `lumibot-3.4.1/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/entities/bars.py` & `lumibot-3.4.1/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/entities/data.py` & `lumibot-3.4.1/lumibot/entities/data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/entities/order.py` & `lumibot-3.4.1/lumibot/entities/order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/entities/position.py` & `lumibot-3.4.1/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/entities/trading_fee.py` & `lumibot-3.4.1/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.4.1/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.4.1/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.4.1/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.4.1/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.4.1/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.4.1/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.4.1/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.4.1/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.4.1/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/stock_oco.py` & `lumibot-3.4.1/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/example_strategies/strangle.py` & `lumibot-3.4.1/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/strategies/_strategy.py` & `lumibot-3.4.1/lumibot/strategies/_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1043,23 +1043,23 @@
 
         # Filename defaults
         if not logdir:
             logdir = "logs"
 
         datestring = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         basename = f"{name + '_' if name is not None else ''}{datestring}"
-        if plot_file_html is None:
+        if not plot_file_html:
             plot_file_html = f"{logdir}/{basename}_trades.html"
-        if trades_file is None:
+        if not trades_file:
             trades_file = f"{logdir}/{basename}_trades.csv"
-        if tearsheet_file is None:
+        if not tearsheet_file:
             tearsheet_file = f"{logdir}/{basename}_tearsheet.html"
-        if settings_file is None:
+        if not settings_file:
             settings_file = f"{logdir}/{basename}_settings.json"
-        if indicators_file is None:
+        if not indicators_file:
             indicators_file = f"{logdir}/{basename}_indicators.html"
 
         self.write_backtest_settings(settings_file)
 
         backtesting_broker = self.broker
         backtesting_broker.export_trade_events_to_csv(trades_file)
         self.plot_returns_vs_benchmark(
```

### Comparing `lumibot-3.4.0/lumibot/strategies/strategy.py` & `lumibot-3.4.1/lumibot/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/strategies/strategy_executor.py` & `lumibot-3.4.1/lumibot/strategies/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/__init__.py` & `lumibot-3.4.1/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/black_scholes.py` & `lumibot-3.4.1/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/ccxt_data_store.py` & `lumibot-3.4.1/lumibot/tools/ccxt_data_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/decorators.py` & `lumibot-3.4.1/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/helpers.py` & `lumibot-3.4.1/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/indicators.py` & `lumibot-3.4.1/lumibot/tools/indicators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/lumibot_time.py` & `lumibot-3.4.1/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/pandas.py` & `lumibot-3.4.1/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/polygon_helper.py` & `lumibot-3.4.1/lumibot/tools/polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/types.py` & `lumibot-3.4.1/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/tools/yahoo_helper.py` & `lumibot-3.4.1/lumibot/tools/yahoo_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/traders/trader.py` & `lumibot-3.4.1/lumibot/traders/trader.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             result = True
         return result
 
     def add_strategy(self, strategy):
         """Adds a strategy to the trader"""
         self._strategies.append(strategy)
 
-    def run_all(self, async_=False, show_plot=True, show_tearsheet=True, save_tearsheet=True, show_indicators=True, tearsheet_file=""):
+    def run_all(self, async_=False, show_plot=True, show_tearsheet=True, save_tearsheet=True, show_indicators=True, tearsheet_file=None):
         """
         run all strategies
 
         Parameters
         ----------
         async_: bool
             Whether to run the strategies asynchronously or not. This is not implemented yet.
```

### Comparing `lumibot-3.4.0/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.4.1/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot/trading_builtins/safe_list.py` & `lumibot-3.4.1/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot.egg-info/PKG-INFO` & `lumibot-3.4.1/lumibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.4.0
+Version: 3.4.1
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.4.0/lumibot.egg-info/SOURCES.txt` & `lumibot-3.4.1/lumibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/lumibot.egg-info/requires.txt` & `lumibot-3.4.1/lumibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/pyproject.toml` & `lumibot-3.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/setup.cfg` & `lumibot-3.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/setup.py` & `lumibot-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.4.0",
+    version="3.4.1",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
```

### Comparing `lumibot-3.4.0/tests/backtest/fixtures.py` & `lumibot-3.4.1/tests/backtest/fixtures.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/backtest/test_example_strategies.py` & `lumibot-3.4.1/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.4.1/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/backtest/test_polygon.py` & `lumibot-3.4.1/tests/backtest/test_polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         )
         broker = BacktestingBroker(data_source=data_source)
         poly_strat_obj = PolygonBacktestStrat(
             broker=broker,
         )
         trader = Trader(logfile="", backtest=True)
         trader.add_strategy(poly_strat_obj)
-        results = trader.run_all(show_plot=False, show_tearsheet=False, save_tearsheet=False, tearsheet_file="")
+        results = trader.run_all(show_plot=False, show_tearsheet=False, save_tearsheet=True)
 
         assert results
         self.verify_backtest_results(poly_strat_obj)
 
     def test_intraday_daterange(self):
         tzinfo = pytz.timezone("America/New_York")
         backtesting_start = datetime.datetime(2024, 2, 7).astimezone(tzinfo)
```

### Comparing `lumibot-3.4.0/tests/backtest/test_strategy_executor.py` & `lumibot-3.4.1/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/backtest/test_yahoo.py` & `lumibot-3.4.1/tests/backtest/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_alpaca.py` & `lumibot-3.4.1/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_alpaca_old.py` & `lumibot-3.4.1/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_asset.py` & `lumibot-3.4.1/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_backtesting_broker.py` & `lumibot-3.4.1/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_ccxt.py` & `lumibot-3.4.1/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_ccxt_store.py` & `lumibot-3.4.1/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_interactive_brokers.py` & `lumibot-3.4.1/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_order.py` & `lumibot-3.4.1/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_polygon_helper.py` & `lumibot-3.4.1/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_strategy_methods.py` & `lumibot-3.4.1/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.0/tests/test_tradier.py` & `lumibot-3.4.1/tests/test_tradier.py`

 * *Files identical despite different names*

