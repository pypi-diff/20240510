# Comparing `tmp/emhass-0.8.6.tar.gz` & `tmp/emhass-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emhass-0.8.6.tar", last modified: Sun Apr  7 11:53:22 2024, max compression
+gzip compressed data, was "emhass-0.9.0.tar", last modified: Fri May 10 20:15:36 2024, max compression
```

## Comparing `emhass-0.8.6.tar` & `emhass-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.849832 emhass-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-07 11:53:19.000000 emhass-0.8.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-07 11:53:19.000000 emhass-0.8.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-07 11:53:19.000000 emhass-0.8.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-07 11:53:19.000000 emhass-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-07 11:53:19.000000 emhass-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-07 11:53:22.849832 emhass-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33584 2024-04-07 11:53:19.000000 emhass-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.841832 emhass-0.8.6/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_load_cost_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_load_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_prod_price_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_train_load_clustering.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_train_load_forecast.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_weather_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_latest.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_perfect_optim_cost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_perfect_optim_profit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_perfect_optim_self-consumption.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_df_final.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_get_data_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_scrapper_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_solarforecast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_solcast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-07 11:53:19.000000 emhass-0.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:53:22.849832 emhass-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-07 11:53:19.000000 emhass-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.837832 emhass-0.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.841832 emhass-0.8.6/src/emhass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37580 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/data/
--rw-r--r--   0 runner    (1001) docker     (127)   168272 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/data/cec_inverters.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)  1655747 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/data/cec_modules.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)    45704 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    37197 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    18406 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/advanced.html
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/basic.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/img/emhass_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/img/emhass_logo_short.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/img/feather-sprite.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/script.js
--rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/templates/template.html
--rw-r--r--   0 runner    (1001) docker     (127)    42394 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.849832 emhass-0.8.6/src/emhass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.849832 emhass-0.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    25232 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30769 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-10 20:15:32.000000 emhass-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-10 20:15:32.000000 emhass-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 20:15:32.000000 emhass-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 20:15:32.000000 emhass-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-10 20:15:32.000000 emhass-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35602 2024-05-10 20:15:36.103846 emhass-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34444 2024-05-10 20:15:32.000000 emhass-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.095846 emhass-0.9.0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_load_cost_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_load_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_prod_price_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_train_load_clustering.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_train_load_forecast.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_weather_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-10 20:15:32.000000 emhass-0.9.0/data/heating_prediction.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_latest.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_perfect_optim_cost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_perfect_optim_profit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_perfect_optim_self-consumption.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_df_final.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_get_data_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_scrapper_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_solarforecast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_solcast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-10 20:15:32.000000 emhass-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:15:36.103846 emhass-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-10 20:15:32.000000 emhass-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.091846 emhass-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.095846 emhass-0.9.0/src/emhass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.099846 emhass-0.9.0/src/emhass/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   168272 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/data/cec_inverters.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)  1655747 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/data/cec_modules.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)    47259 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/machine_learning_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37252 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.099846 emhass-0.9.0/src/emhass/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/advanced.html
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/basic.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/src/emhass/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/img/emhass_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/img/emhass_logo_short.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/img/feather-sprite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/src/emhass/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/templates/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47801 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23055 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/src/emhass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35602 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    30422 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31834 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_machine_learning_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_retrieve_hass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_utils.py
```

### Comparing `emhass-0.8.6/CHANGELOG.md` & `emhass-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## 0.9.0 - 2024-05-10
+### Improvement
+- On this new version we now have a new method to train a regression model using Scikit-Learn methods. This is the contribution of @gieljnssns. Check the dedicated section the documentation to this new feature: [https://emhass.readthedocs.io/en/latest/mlregressor.html](https://emhass.readthedocs.io/en/latest/mlregressor.html)
+- Again another bunch of nice improvements by @GeoDerp:
+  - Added Dictionary var containing EMHASS paths
+  - MLForcaster error suppression
+  - Add `freq` as runtime parameter
+  - Improved documentation added README buttons
+- Bumping dependencies:
+  - Bump h5py from 3.10.0 to 3.11.0
+  - Bump myst-parser from 2.0.0 to 3.0.1
+  - Bump skforecast from 0.11.0 to 0.12.0
+
 ## 0.8.6 - 2024-04-07
 ### Fix
 - Fixed bug from forecast out method related to issue 240
 - Fix patch for some issues with package file paths
 
 ## 0.8.5 - 2024-04-01
 ### Improvement
```

### Comparing `emhass-0.8.6/CODE_OF_CONDUCT.md` & `emhass-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/CONTRIBUTING.md` & `emhass-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/LICENSE` & `emhass-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/PKG-INFO` & `emhass-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.8.6
+Version: 0.9.0
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,19 +20,19 @@
 Requires-Dist: scipy==1.12.0
 Requires-Dist: pandas<=2.0.3
 Requires-Dist: pvlib>=0.10.2
 Requires-Dist: protobuf>=3.0.0
 Requires-Dist: pytz>=2021.1
 Requires-Dist: requests>=2.25.1
 Requires-Dist: beautifulsoup4>=4.9.3
-Requires-Dist: h5py==3.10.0
+Requires-Dist: h5py==3.11.0
 Requires-Dist: pulp>=2.4
 Requires-Dist: pyyaml>=5.4.1
 Requires-Dist: tables<=3.9.1
-Requires-Dist: skforecast==0.11.0
+Requires-Dist: skforecast==0.12.0
 Requires-Dist: flask>=2.0.3
 Requires-Dist: waitress>=2.1.1
 Requires-Dist: plotly>=5.6.0
 
 <div align="center">
   <br>
   <img alt="EMHASS" src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/emhass_logo.png" width="300px">
@@ -59,14 +59,28 @@
   <a href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/emhass">
   </a>
   <a href="https://emhass.readthedocs.io/en/latest/">
     <img alt="Read the Docs" src="https://img.shields.io/readthedocs/emhass">
   </a>
 </p>
+<div align="center">
+ <a href="https://emhass.readthedocs.io/en/latest/">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Documentation_button.svg" alt="Documentation">
+  </a>
+   <a href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Community_button.svg" alt="Community">
+  </a>
+  <a href="https://github.com/davidusb-geek/emhass/issues">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Issues_button.svg" alt="Issues">
+  </a>
+  <a href="https://github.com/davidusb-geek/emhass-add-on">
+     <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/EMHASS_Add_on_button.svg" alt="EMHASS Add-on">
+  </a>
+</div>
 <br>
 <p align="center">
 If you like this work please consider buying a coffee ;-) 
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/davidusbgeek" target="_blank">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" >
@@ -103,15 +117,15 @@
 EMHASS was designed to be integrated with Home Assistant, hence it's name. 
 Installation instructions and example Home Assistant automation configurations are given below.
 
 You must follow these steps to make EMHASS work properly:
 
 1) Define all the parameters in the configuration file according to your installation. See the description for each parameter in the **configuration** section.
 
-2) You most notably will need to define the main data entering EMHASS. This will be the `sensor_power_photovoltaics` for the name of the your hass variable containing the PV produced power and the variable `sensor_power_load_no_var_loads` for the load power of your household excluding the power of the deferrable loads that you want to optimize.
+2) You most notably will need to define the main data entering EMHASS. This will be the `sensor.power_photovoltaics` for the name of the your hass variable containing the PV produced power and the variable `sensor.power_load_no_var_loads` for the load power of your household excluding the power of the deferrable loads that you want to optimize.
 
 3) Launch the actual optimization and check the results. This can be done manually using the buttons in the web ui or with a `curl` command like this: `curl -i -H 'Content-Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-optim`.
 
 4) If you’re satisfied with the optimization results then you can set the optimization and data publish task commands in an automation. You can read more about this on the **usage** section below.
 
 5) The final step is to link the deferrable loads variables to real switchs on your installation. An example code for this using automations and the shell command integration is presented below in the **usage** section.
 
@@ -366,15 +380,15 @@
 
 - Load power forecast: how much power your house will demand on the next 24h. This is given in Watts.
 
 - Load cost forecast: the price of the energy from the grid on the next 24h. This is given in EUR/kWh.
 
 - PV production selling price forecast: at what price are you selling your excess PV production on the next 24h. This is given in EUR/kWh.
 
-The sensor containing the load data should be specified in parameter `var_load` in the configuration file. As we want to optimize the household energies, when need to forecast the load power conumption. The default method for this is a naive approach using 1-day persistence. The load data variable should not contain the data from the deferrable loads themselves. For example, lets say that you set your deferrable load to be the washing machine. The variable that you should enter in EMHASS will be: `var_load: 'sensor.power_load_no_var_loads'` and `sensor_power_load_no_var_loads = sensor_power_load - sensor_power_washing_machine`. This is supposing that the overall load of your house is contained in variable: `sensor_power_load`. The sensor `sensor_power_load_no_var_loads` can be easily created with a new template sensor in Home Assistant.
+The sensor containing the load data should be specified in parameter `var_load` in the configuration file. As we want to optimize the household energies, when need to forecast the load power conumption. The default method for this is a naive approach using 1-day persistence. The load data variable should not contain the data from the deferrable loads themselves. For example, lets say that you set your deferrable load to be the washing machine. The variable that you should enter in EMHASS will be: `var_load: 'sensor.power_load_no_var_loads'` and `sensor.power_load_no_var_loads = sensor.power_load - sensor.power_washing_machine`. This is supposing that the overall load of your house is contained in variable: `sensor.power_load`. The sensor `sensor.power_load_no_var_loads` can be easily created with a new template sensor in Home Assistant.
 
 If you are implementing a MPC controller, then you should also need to provide some data at the optimization runtime using the key `runtimeparams`.
 
 The valid values to pass for both forecast data and MPC related data are explained below.
 
 ### Forecast data
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.8.6 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.9.0 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: wheel
 Requires-Dist: numpy==1.26.4 Requires-Dist: scipy==1.12.0 Requires-Dist:
 pandas<=2.0.3 Requires-Dist: pvlib>=0.10.2 Requires-Dist: protobuf>=3.0.0
 Requires-Dist: pytz>=2021.1 Requires-Dist: requests>=2.25.1 Requires-Dist:
-beautifulsoup4>=4.9.3 Requires-Dist: h5py==3.10.0 Requires-Dist: pulp>=2.4
+beautifulsoup4>=4.9.3 Requires-Dist: h5py==3.11.0 Requires-Dist: pulp>=2.4
 Requires-Dist: pyyaml>=5.4.1 Requires-Dist: tables<=3.9.1 Requires-Dist:
-skforecast==0.11.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
+skforecast==0.12.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
 Requires-Dist: plotly>=5.6.0
 
                                    [EMHASS]
               ************ EEnneerrggyy MMaannaaggeemmeenntt ffoorr HHoommee AAssssiissttaanntt ************
 
  _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/
   _g_i_t_h_u_b_/_d_a_v_i_d_u_s_b_-_g_e_e_k_/_e_m_h_a_s_s_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_B_W_7_K_S_C_H_N_9_0_]
          _[_G_i_t_H_u_b_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_R_e_a_d_ _t_h_e_ _D_o_c_s_]
+               _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_m_m_u_n_i_t_y_]_[_I_s_s_u_e_s_]_[_E_M_H_A_S_S_ _A_d_d_-_o_n_]
 
            If you like this work please consider buying a coffee ;-)
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 EHMASS is a Python module designed to optimize your home energy interfacing
 with Home Assistant. ## Introduction EMHASS (Energy Management for Home
 Assistant) is an optimization tool designed for residential households. The
 package uses a Linear Programming approach to optimize energy usage while
@@ -73,17 +74,17 @@
 approach and a main configuration file defined by the user. EMHASS was designed
 to be integrated with Home Assistant, hence it's name. Installation
 instructions and example Home Assistant automation configurations are given
 below. You must follow these steps to make EMHASS work properly: 1) Define all
 the parameters in the configuration file according to your installation. See
 the description for each parameter in the **configuration** section. 2) You
 most notably will need to define the main data entering EMHASS. This will be
-the `sensor_power_photovoltaics` for the name of the your hass variable
+the `sensor.power_photovoltaics` for the name of the your hass variable
 containing the PV produced power and the variable
-`sensor_power_load_no_var_loads` for the load power of your household excluding
+`sensor.power_load_no_var_loads` for the load power of your household excluding
 the power of the deferrable loads that you want to optimize. 3) Launch the
 actual optimization and check the results. This can be done manually using the
 buttons in the web ui or with a `curl` command like this: `curl -i -H 'Content-
 Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-
 optim`. 4) If youâre satisfied with the optimization results then you can set
 the optimization and data publish task commands in an automation. You can read
 more about this on the **usage** section below. 5) The final step is to link
@@ -319,18 +320,18 @@
 be specified in parameter `var_load` in the configuration file. As we want to
 optimize the household energies, when need to forecast the load power
 conumption. The default method for this is a naive approach using 1-day
 persistence. The load data variable should not contain the data from the
 deferrable loads themselves. For example, lets say that you set your deferrable
 load to be the washing machine. The variable that you should enter in EMHASS
 will be: `var_load: 'sensor.power_load_no_var_loads'` and
-`sensor_power_load_no_var_loads = sensor_power_load -
-sensor_power_washing_machine`. This is supposing that the overall load of your
-house is contained in variable: `sensor_power_load`. The sensor
-`sensor_power_load_no_var_loads` can be easily created with a new template
+`sensor.power_load_no_var_loads = sensor.power_load -
+sensor.power_washing_machine`. This is supposing that the overall load of your
+house is contained in variable: `sensor.power_load`. The sensor
+`sensor.power_load_no_var_loads` can be easily created with a new template
 sensor in Home Assistant. If you are implementing a MPC controller, then you
 should also need to provide some data at the optimization runtime using the key
 `runtimeparams`. The valid values to pass for both forecast data and MPC
 related data are explained below. ### Forecast data It is possible to provide
 EMHASS with your own forecast data. For this just add the data as list of
 values to a data dictionary during the call to `emhass` using the
 `runtimeparams` option. For example if using the add-on or the standalone
```

### Comparing `emhass-0.8.6/README.md` & `emhass-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,28 @@
   <a href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/emhass">
   </a>
   <a href="https://emhass.readthedocs.io/en/latest/">
     <img alt="Read the Docs" src="https://img.shields.io/readthedocs/emhass">
   </a>
 </p>
+<div align="center">
+ <a href="https://emhass.readthedocs.io/en/latest/">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Documentation_button.svg" alt="Documentation">
+  </a>
+   <a href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Community_button.svg" alt="Community">
+  </a>
+  <a href="https://github.com/davidusb-geek/emhass/issues">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Issues_button.svg" alt="Issues">
+  </a>
+  <a href="https://github.com/davidusb-geek/emhass-add-on">
+     <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/EMHASS_Add_on_button.svg" alt="EMHASS Add-on">
+  </a>
+</div>
 <br>
 <p align="center">
 If you like this work please consider buying a coffee ;-) 
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/davidusbgeek" target="_blank">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" >
@@ -68,15 +82,15 @@
 EMHASS was designed to be integrated with Home Assistant, hence it's name. 
 Installation instructions and example Home Assistant automation configurations are given below.
 
 You must follow these steps to make EMHASS work properly:
 
 1) Define all the parameters in the configuration file according to your installation. See the description for each parameter in the **configuration** section.
 
-2) You most notably will need to define the main data entering EMHASS. This will be the `sensor_power_photovoltaics` for the name of the your hass variable containing the PV produced power and the variable `sensor_power_load_no_var_loads` for the load power of your household excluding the power of the deferrable loads that you want to optimize.
+2) You most notably will need to define the main data entering EMHASS. This will be the `sensor.power_photovoltaics` for the name of the your hass variable containing the PV produced power and the variable `sensor.power_load_no_var_loads` for the load power of your household excluding the power of the deferrable loads that you want to optimize.
 
 3) Launch the actual optimization and check the results. This can be done manually using the buttons in the web ui or with a `curl` command like this: `curl -i -H 'Content-Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-optim`.
 
 4) If you’re satisfied with the optimization results then you can set the optimization and data publish task commands in an automation. You can read more about this on the **usage** section below.
 
 5) The final step is to link the deferrable loads variables to real switchs on your installation. An example code for this using automations and the shell command integration is presented below in the **usage** section.
 
@@ -331,15 +345,15 @@
 
 - Load power forecast: how much power your house will demand on the next 24h. This is given in Watts.
 
 - Load cost forecast: the price of the energy from the grid on the next 24h. This is given in EUR/kWh.
 
 - PV production selling price forecast: at what price are you selling your excess PV production on the next 24h. This is given in EUR/kWh.
 
-The sensor containing the load data should be specified in parameter `var_load` in the configuration file. As we want to optimize the household energies, when need to forecast the load power conumption. The default method for this is a naive approach using 1-day persistence. The load data variable should not contain the data from the deferrable loads themselves. For example, lets say that you set your deferrable load to be the washing machine. The variable that you should enter in EMHASS will be: `var_load: 'sensor.power_load_no_var_loads'` and `sensor_power_load_no_var_loads = sensor_power_load - sensor_power_washing_machine`. This is supposing that the overall load of your house is contained in variable: `sensor_power_load`. The sensor `sensor_power_load_no_var_loads` can be easily created with a new template sensor in Home Assistant.
+The sensor containing the load data should be specified in parameter `var_load` in the configuration file. As we want to optimize the household energies, when need to forecast the load power conumption. The default method for this is a naive approach using 1-day persistence. The load data variable should not contain the data from the deferrable loads themselves. For example, lets say that you set your deferrable load to be the washing machine. The variable that you should enter in EMHASS will be: `var_load: 'sensor.power_load_no_var_loads'` and `sensor.power_load_no_var_loads = sensor.power_load - sensor.power_washing_machine`. This is supposing that the overall load of your house is contained in variable: `sensor.power_load`. The sensor `sensor.power_load_no_var_loads` can be easily created with a new template sensor in Home Assistant.
 
 If you are implementing a MPC controller, then you should also need to provide some data at the optimization runtime using the key `runtimeparams`.
 
 The valid values to pass for both forecast data and MPC related data are explained below.
 
 ### Forecast data
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 
                                    [EMHASS]
               ************ EEnneerrggyy MMaannaaggeemmeenntt ffoorr HHoommee AAssssiissttaanntt ************
 
  _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/
   _g_i_t_h_u_b_/_d_a_v_i_d_u_s_b_-_g_e_e_k_/_e_m_h_a_s_s_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_B_W_7_K_S_C_H_N_9_0_]
          _[_G_i_t_H_u_b_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_R_e_a_d_ _t_h_e_ _D_o_c_s_]
+               _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_m_m_u_n_i_t_y_]_[_I_s_s_u_e_s_]_[_E_M_H_A_S_S_ _A_d_d_-_o_n_]
 
            If you like this work please consider buying a coffee ;-)
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 EHMASS is a Python module designed to optimize your home energy interfacing
 with Home Assistant. ## Introduction EMHASS (Energy Management for Home
 Assistant) is an optimization tool designed for residential households. The
 package uses a Linear Programming approach to optimize energy usage while
@@ -57,17 +58,17 @@
 approach and a main configuration file defined by the user. EMHASS was designed
 to be integrated with Home Assistant, hence it's name. Installation
 instructions and example Home Assistant automation configurations are given
 below. You must follow these steps to make EMHASS work properly: 1) Define all
 the parameters in the configuration file according to your installation. See
 the description for each parameter in the **configuration** section. 2) You
 most notably will need to define the main data entering EMHASS. This will be
-the `sensor_power_photovoltaics` for the name of the your hass variable
+the `sensor.power_photovoltaics` for the name of the your hass variable
 containing the PV produced power and the variable
-`sensor_power_load_no_var_loads` for the load power of your household excluding
+`sensor.power_load_no_var_loads` for the load power of your household excluding
 the power of the deferrable loads that you want to optimize. 3) Launch the
 actual optimization and check the results. This can be done manually using the
 buttons in the web ui or with a `curl` command like this: `curl -i -H 'Content-
 Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-
 optim`. 4) If youâre satisfied with the optimization results then you can set
 the optimization and data publish task commands in an automation. You can read
 more about this on the **usage** section below. 5) The final step is to link
@@ -303,18 +304,18 @@
 be specified in parameter `var_load` in the configuration file. As we want to
 optimize the household energies, when need to forecast the load power
 conumption. The default method for this is a naive approach using 1-day
 persistence. The load data variable should not contain the data from the
 deferrable loads themselves. For example, lets say that you set your deferrable
 load to be the washing machine. The variable that you should enter in EMHASS
 will be: `var_load: 'sensor.power_load_no_var_loads'` and
-`sensor_power_load_no_var_loads = sensor_power_load -
-sensor_power_washing_machine`. This is supposing that the overall load of your
-house is contained in variable: `sensor_power_load`. The sensor
-`sensor_power_load_no_var_loads` can be easily created with a new template
+`sensor.power_load_no_var_loads = sensor.power_load -
+sensor.power_washing_machine`. This is supposing that the overall load of your
+house is contained in variable: `sensor.power_load`. The sensor
+`sensor.power_load_no_var_loads` can be easily created with a new template
 sensor in Home Assistant. If you are implementing a MPC controller, then you
 should also need to provide some data at the optimization runtime using the key
 `runtimeparams`. The valid values to pass for both forecast data and MPC
 related data are explained below. ### Forecast data It is possible to provide
 EMHASS with your own forecast data. For this just add the data as list of
 values to a data dictionary during the call to `emhass` using the
 `runtimeparams` option. For example if using the add-on or the standalone
```

### Comparing `emhass-0.8.6/data/data_load_cost_forecast.csv` & `emhass-0.9.0/data/data_load_cost_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/data_load_forecast.csv` & `emhass-0.9.0/data/data_load_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/data_prod_price_forecast.csv` & `emhass-0.9.0/data/data_prod_price_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/data_train_load_clustering.pkl` & `emhass-0.9.0/data/data_train_load_clustering.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/data_train_load_forecast.pkl` & `emhass-0.9.0/data/data_train_load_forecast.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/data_weather_forecast.csv` & `emhass-0.9.0/data/data_weather_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/opt_res_latest.csv` & `emhass-0.9.0/data/opt_res_latest.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/opt_res_perfect_optim_cost.csv` & `emhass-0.9.0/data/opt_res_perfect_optim_cost.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/opt_res_perfect_optim_profit.csv` & `emhass-0.9.0/data/opt_res_perfect_optim_profit.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/opt_res_perfect_optim_self-consumption.csv` & `emhass-0.9.0/data/opt_res_perfect_optim_self-consumption.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/test_df_final.pkl` & `emhass-0.9.0/data/test_df_final.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/test_response_get_data_get_method.pbz2` & `emhass-0.9.0/data/test_response_get_data_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/test_response_scrapper_get_method.pbz2` & `emhass-0.9.0/data/test_response_scrapper_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/test_response_solarforecast_get_method.pbz2` & `emhass-0.9.0/data/test_response_solarforecast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/data/test_response_solcast_get_method.pbz2` & `emhass-0.9.0/data/test_response_solcast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/setup.py` & `emhass-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='emhass',  # Required
-    version='0.8.6',  # Required
+    version='0.9.0',  # Required
     description='An Energy Management System for Home Assistant',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/davidusb-geek/emhass',  # Optional
     author='David HERNANDEZ',  # Optional
     author_email='davidusb@gmail.com',  # Optional
     classifiers=[  # Optional
@@ -44,19 +44,19 @@
         'scipy==1.12.0',
         'pandas<=2.0.3',
         'pvlib>=0.10.2',
         'protobuf>=3.0.0',
         'pytz>=2021.1',
         'requests>=2.25.1',
         'beautifulsoup4>=4.9.3',
-        'h5py==3.10.0',
+        'h5py==3.11.0',
         'pulp>=2.4',
         'pyyaml>=5.4.1',
         'tables<=3.9.1',
-        'skforecast==0.11.0',
+        'skforecast==0.12.0',
         'flask>=2.0.3',
         'waitress>=2.1.1',
         'plotly>=5.6.0'
     ],  # Optional
     entry_points={  # Optional
         'console_scripts': [
             'emhass=emhass.command_line:main',
```

### Comparing `emhass-0.8.6/src/emhass/command_line.py` & `emhass-0.9.0/src/emhass/command_line.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,191 +4,296 @@
 import argparse
 import os
 import pathlib
 import logging
 import json
 import copy
 import pickle
-import time
-import numpy as np
-import pandas as pd
 from datetime import datetime, timezone
 from typing import Optional, Tuple
+from importlib.metadata import version
+import numpy as np
+import pandas as pd
+
 from distutils.util import strtobool
 
-from importlib.metadata import version
 from emhass.retrieve_hass import RetrieveHass
 from emhass.forecast import Forecast
 from emhass.machine_learning_forecaster import MLForecaster
 from emhass.optimization import Optimization
+from emhass.machine_learning_regressor import MLRegressor
 from emhass import utils
 
 
-def set_input_data_dict(config_path: pathlib.Path, base_path: str, costfun: str, 
+def set_input_data_dict(emhass_conf: dict, costfun: str, 
     params: str, runtimeparams: str, set_type: str, logger: logging.Logger,
     get_data_from_file: Optional[bool] = False) -> dict:
     """
     Set up some of the data needed for the different actions.
     
-    :param config_path: The complete absolute path where the config.yaml file is located
-    :type config_path: pathlib.Path
-    :param base_path: The parent folder of the config_path
-    :type base_path: str
+    :param emhass_conf: Dictionary containing the needed emhass paths
+    :type emhass_conf: dict
     :param costfun: The type of cost function to use for optimization problem
     :type costfun: str
     :param params: Configuration parameters passed from data/options.json
     :type params: str
-    :param runtimeparams: Runtime optimization parameters passed as a dictionnary
+    :param runtimeparams: Runtime optimization parameters passed as a dictionary
     :type runtimeparams: str
     :param set_type: Set the type of setup based on following type of optimization
     :type set_type: str
     :param logger: The passed logger object
     :type logger: logging object
     :param get_data_from_file: Use data from saved CSV file (useful for debug)
     :type get_data_from_file: bool, optional
     :return: A dictionnary with multiple data used by the action functions
     :rtype: dict
 
     """
     logger.info("Setting up needed data")
     # Parsing yaml
     retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(
-        config_path, use_secrets=not(get_data_from_file), params=params)
+        emhass_conf, use_secrets=not(get_data_from_file), params=params)
     # Treat runtimeparams
     params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
-        runtimeparams, params, retrieve_hass_conf, 
-        optim_conf, plant_conf, set_type, logger)
+        runtimeparams,
+        params,
+        retrieve_hass_conf,
+        optim_conf,
+        plant_conf,
+        set_type,
+        logger,
+    )
     # Define main objects
     rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'], 
                       retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'], 
-                      params, base_path, logger, get_data_from_file=get_data_from_file)
+                      params, emhass_conf, logger, get_data_from_file=get_data_from_file)
     fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf,
-                    params, base_path, logger, get_data_from_file=get_data_from_file)
+                    params, emhass_conf, logger, get_data_from_file=get_data_from_file)
     opt = Optimization(retrieve_hass_conf, optim_conf, plant_conf, 
                        fcst.var_load_cost, fcst.var_prod_price, 
-                       costfun, base_path, logger)
+                       costfun, emhass_conf, logger)
     # Perform setup based on type of action
     if set_type == "perfect-optim":
         # Retrieve data from hass
         if get_data_from_file:
-            with open(pathlib.Path(base_path) / 'data' / 'test_df_final.pkl', 'rb') as inp:
+            with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
+            retrieve_hass_conf['var_load'] = str(var_list[0])
+            retrieve_hass_conf['var_PV'] = str(var_list[1])
+            retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
         else:
-            days_list = utils.get_days_list(retrieve_hass_conf['days_to_retrieve'])
-            var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
-            if not rh.get_data(days_list, var_list,
-                               minimal_response=False, significant_changes_only=False):
-                return False 
-        if not rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
-                               set_zero_min = retrieve_hass_conf['set_zero_min'], 
-                               var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
-                               var_interp = retrieve_hass_conf['var_interp']):
+            days_list = utils.get_days_list(retrieve_hass_conf["days_to_retrieve"])
+            var_list = [retrieve_hass_conf["var_load"], retrieve_hass_conf["var_PV"]]
+            if not rh.get_data(
+                days_list,
+                var_list,
+                minimal_response=False,
+                significant_changes_only=False,
+            ):
+                return False
+        if not rh.prepare_data(
+            retrieve_hass_conf["var_load"],
+            load_negative=retrieve_hass_conf["load_negative"],
+            set_zero_min=retrieve_hass_conf["set_zero_min"],
+            var_replace_zero=retrieve_hass_conf["var_replace_zero"],
+            var_interp=retrieve_hass_conf["var_interp"],
+        ):
             return False
         df_input_data = rh.df_final.copy()
         # What we don't need for this type of action
         P_PV_forecast, P_load_forecast, df_input_data_dayahead = None, None, None
     elif set_type == "dayahead-optim":
         # Get PV and load forecasts
-        df_weather = fcst.get_weather_forecast(method=optim_conf['weather_forecast_method'])
+        df_weather = fcst.get_weather_forecast(
+            method=optim_conf["weather_forecast_method"]
+        )
         P_PV_forecast = fcst.get_power_from_weather(df_weather)
         P_load_forecast = fcst.get_load_forecast(method=optim_conf['load_forecast_method'])
         if isinstance(P_load_forecast,bool) and not P_load_forecast:
             logger.error("Unable to get sensor power photovoltaics, or sensor power load no var loads. Check HA sensors and their daily data")
             return False
-        df_input_data_dayahead = pd.DataFrame(np.transpose(np.vstack([P_PV_forecast.values,P_load_forecast.values])),
-                                              index=P_PV_forecast.index,
-                                              columns=['P_PV_forecast', 'P_load_forecast'])
+        df_input_data_dayahead = pd.DataFrame(
+            np.transpose(np.vstack([P_PV_forecast.values, P_load_forecast.values])),
+            index=P_PV_forecast.index,
+            columns=["P_PV_forecast", "P_load_forecast"],
+        )
         df_input_data_dayahead = utils.set_df_index_freq(df_input_data_dayahead)
         params = json.loads(params)
-        if 'prediction_horizon' in params['passed_data'] and params['passed_data']['prediction_horizon'] is not None:
-            prediction_horizon = params['passed_data']['prediction_horizon']
-            df_input_data_dayahead = copy.deepcopy(df_input_data_dayahead)[df_input_data_dayahead.index[0]:df_input_data_dayahead.index[prediction_horizon-1]]
+        if (
+            "prediction_horizon" in params["passed_data"]
+            and params["passed_data"]["prediction_horizon"] is not None
+        ):
+            prediction_horizon = params["passed_data"]["prediction_horizon"]
+            df_input_data_dayahead = copy.deepcopy(df_input_data_dayahead)[
+                df_input_data_dayahead.index[0] : df_input_data_dayahead.index[
+                    prediction_horizon - 1
+                ]
+            ]
         # What we don't need for this type of action
         df_input_data, days_list = None, None
     elif set_type == "naive-mpc-optim":
         # Retrieve data from hass
         if get_data_from_file:
-            with open(pathlib.Path(base_path) / 'data' / 'test_df_final.pkl', 'rb') as inp:
+            with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
+            retrieve_hass_conf['var_load'] = str(var_list[0])
+            retrieve_hass_conf['var_PV'] = str(var_list[1])
+            retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
         else:
             days_list = utils.get_days_list(1)
-            var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
-            if not rh.get_data(days_list, var_list,
-                               minimal_response=False, significant_changes_only=False):
+            var_list = [retrieve_hass_conf["var_load"], retrieve_hass_conf["var_PV"]]
+            if not rh.get_data(
+                days_list,
+                var_list,
+                minimal_response=False,
+                significant_changes_only=False,
+            ):
                 return False
-        if not rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
-                               set_zero_min = retrieve_hass_conf['set_zero_min'], 
-                               var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
-                               var_interp = retrieve_hass_conf['var_interp']):
+        if not rh.prepare_data(
+            retrieve_hass_conf["var_load"],
+            load_negative=retrieve_hass_conf["load_negative"],
+            set_zero_min=retrieve_hass_conf["set_zero_min"],
+            var_replace_zero=retrieve_hass_conf["var_replace_zero"],
+            var_interp=retrieve_hass_conf["var_interp"],
+        ):
             return False
         df_input_data = rh.df_final.copy()
         # Get PV and load forecasts
         df_weather = fcst.get_weather_forecast(method=optim_conf['weather_forecast_method'])
         P_PV_forecast = fcst.get_power_from_weather(df_weather, set_mix_forecast=True, df_now=df_input_data)
         P_load_forecast = fcst.get_load_forecast(method=optim_conf['load_forecast_method'], set_mix_forecast=True, df_now=df_input_data)
+        if isinstance(P_load_forecast,bool) and not P_load_forecast:
+            logger.error("Unable to get sensor power photovoltaics, or sensor power load no var loads. Check HA sensors and their daily data")
+            return False
         df_input_data_dayahead = pd.concat([P_PV_forecast, P_load_forecast], axis=1)
         df_input_data_dayahead = utils.set_df_index_freq(df_input_data_dayahead)
-        df_input_data_dayahead.columns = ['P_PV_forecast', 'P_load_forecast']
+        df_input_data_dayahead.columns = ["P_PV_forecast", "P_load_forecast"]
         params = json.loads(params)
-        if 'prediction_horizon' in params['passed_data'] and params['passed_data']['prediction_horizon'] is not None:
-            prediction_horizon = params['passed_data']['prediction_horizon']
-            df_input_data_dayahead = copy.deepcopy(df_input_data_dayahead)[df_input_data_dayahead.index[0]:df_input_data_dayahead.index[prediction_horizon-1]]
-    elif set_type == "forecast-model-fit" or set_type == "forecast-model-predict" or set_type == "forecast-model-tune":
+        if (
+            "prediction_horizon" in params["passed_data"]
+            and params["passed_data"]["prediction_horizon"] is not None
+        ):
+            prediction_horizon = params["passed_data"]["prediction_horizon"]
+            df_input_data_dayahead = copy.deepcopy(df_input_data_dayahead)[
+                df_input_data_dayahead.index[0] : df_input_data_dayahead.index[
+                    prediction_horizon - 1
+                ]
+            ]
+    elif (
+        set_type == "forecast-model-fit"
+        or set_type == "forecast-model-predict"
+        or set_type == "forecast-model-tune"
+    ):
         df_input_data_dayahead = None
         P_PV_forecast, P_load_forecast = None, None
         params = json.loads(params)
         # Retrieve data from hass
-        days_to_retrieve = params['passed_data']['days_to_retrieve']
-        model_type = params['passed_data']['model_type']
-        var_model = params['passed_data']['var_model']
+        days_to_retrieve = params["passed_data"]["days_to_retrieve"]
+        model_type = params["passed_data"]["model_type"]
+        var_model = params["passed_data"]["var_model"]
         if get_data_from_file:
             days_list = None
             filename = 'data_train_'+model_type+'.pkl'
-            data_path = pathlib.Path(base_path) / 'data' / filename
-            with open(data_path, 'rb') as inp:
+            filename_path = emhass_conf['data_path'] / filename
+            with open(filename_path, 'rb') as inp:
                 df_input_data, _ = pickle.load(inp)
-            df_input_data = df_input_data[df_input_data.index[-1] - pd.offsets.Day(days_to_retrieve):]
+            df_input_data = df_input_data[
+                df_input_data.index[-1] - pd.offsets.Day(days_to_retrieve) :
+            ]
         else:
             days_list = utils.get_days_list(days_to_retrieve)
             var_list = [var_model]
             if not rh.get_data(days_list, var_list):
                 return False
             df_input_data = rh.df_final.copy()
+
+    elif set_type == "regressor-model-fit" or set_type == "regressor-model-predict":
+
+        df_input_data, df_input_data_dayahead = None, None
+        P_PV_forecast, P_load_forecast = None, None
+        params = json.loads(params)
+        days_list = None
+        csv_file = params["passed_data"].get("csv_file", None)
+        if "features" in params["passed_data"]:
+            features = params["passed_data"]["features"]
+        if "target" in params["passed_data"]:
+            target = params["passed_data"]["target"]
+        if "timestamp" in params["passed_data"]:
+            timestamp = params["passed_data"]["timestamp"]
+        if csv_file:
+            if get_data_from_file:
+                base_path = emhass_conf["data_path"]  # + "/data"
+                filename_path = pathlib.Path(base_path) / csv_file
+
+            else:
+                filename_path = emhass_conf["data_path"] / csv_file
+
+            if filename_path.is_file():
+                df_input_data = pd.read_csv(filename_path, parse_dates=True)
+
+            else:
+                logger.error("The CSV file " + csv_file + " was not found in path: " + str(emhass_conf["data_path"]))
+                return False
+                #raise ValueError("The CSV file " + csv_file + " was not found.")
+            required_columns = []
+            required_columns.extend(features)
+            required_columns.append(target)
+            if timestamp is not None:
+                required_columns.append(timestamp)
+
+            if not set(required_columns).issubset(df_input_data.columns):
+                logger.error("The cvs file does not contain the required columns.")
+                msg = f"CSV file should contain the following columns: {', '.join(required_columns)}"
+                logger.error(msg)
+                return False
+                #raise ValueError(
+                #    msg,
+                #)
+
     elif set_type == "publish-data":
         df_input_data, df_input_data_dayahead = None, None
         P_PV_forecast, P_load_forecast = None, None
         days_list = None
     else:
-        logger.error("The passed action argument and hence the set_type parameter for setup is not valid")
+        logger.error(
+            "The passed action argument and hence the set_type parameter for setup is not valid",
+        )
         df_input_data, df_input_data_dayahead = None, None
         P_PV_forecast, P_load_forecast = None, None
         days_list = None
 
-    # The input data dictionnary to return
+    # The input data dictionary to return
     input_data_dict = {
-        'root': base_path,
+        'emhass_conf': emhass_conf,
         'retrieve_hass_conf': retrieve_hass_conf,
         'rh': rh,
         'opt': opt,
         'fcst': fcst,
         'df_input_data': df_input_data,
         'df_input_data_dayahead': df_input_data_dayahead,
         'P_PV_forecast': P_PV_forecast,
         'P_load_forecast': P_load_forecast,
         'costfun': costfun,
         'params': params,
         'days_list': days_list
     }
     return input_data_dict
-    
-def perfect_forecast_optim(input_data_dict: dict, logger: logging.Logger,
-    save_data_to_file: Optional[bool] = True, debug: Optional[bool] = False) -> pd.DataFrame:
+
+
+def perfect_forecast_optim(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    save_data_to_file: Optional[bool] = True,
+    debug: Optional[bool] = False,
+) -> pd.DataFrame:
     """
     Perform a call to the perfect forecast optimization routine.
-    
+
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
     :param save_data_to_file: Save optimization results to CSV file
     :type save_data_to_file: bool, optional
     :param debug: A debug option useful for unittests
@@ -199,32 +304,41 @@
     """
     logger.info("Performing perfect forecast optimization")
     # Load cost and prod price forecast
     df_input_data = input_data_dict['fcst'].get_load_cost_forecast(
         input_data_dict['df_input_data'], 
         method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'],
         list_and_perfect=True)
+    if isinstance(df_input_data,bool) and not df_input_data:
+        return False
     df_input_data = input_data_dict['fcst'].get_prod_price_forecast(
         df_input_data, method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'],
         list_and_perfect=True)
+    if isinstance(df_input_data,bool) and not df_input_data:
+        return False 
     opt_res = input_data_dict['opt'].perform_perfect_forecast_optim(df_input_data, input_data_dict['days_list'])
     # Save CSV file for analysis
     if save_data_to_file:
-        filename = 'opt_res_perfect_optim_'+input_data_dict['costfun']+'.csv'
-    else: # Just save the latest optimization results
-        filename = 'opt_res_latest.csv'
+        filename = "opt_res_perfect_optim_" + input_data_dict["costfun"] + ".csv"
+    else:  # Just save the latest optimization results
+        filename = "opt_res_latest.csv"
     if not debug:
-        opt_res.to_csv(pathlib.Path(input_data_dict['root']) / filename, index_label='timestamp')
+        opt_res.to_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
     return opt_res
-    
-def dayahead_forecast_optim(input_data_dict: dict, logger: logging.Logger,
-    save_data_to_file: Optional[bool] = False, debug: Optional[bool] = False) -> pd.DataFrame:
+
+
+def dayahead_forecast_optim(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    save_data_to_file: Optional[bool] = False,
+    debug: Optional[bool] = False,
+) -> pd.DataFrame:
     """
     Perform a call to the day-ahead optimization routine.
-    
+
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
     :param save_data_to_file: Save optimization results to CSV file
     :type save_data_to_file: bool, optional
     :param debug: A debug option useful for unittests
@@ -234,34 +348,45 @@
 
     """
     logger.info("Performing day-ahead forecast optimization")
     # Load cost and prod price forecast
     df_input_data_dayahead = input_data_dict['fcst'].get_load_cost_forecast(
         input_data_dict['df_input_data_dayahead'],
         method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'])
+    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
+        return False 
     df_input_data_dayahead = input_data_dict['fcst'].get_prod_price_forecast(
         df_input_data_dayahead, 
         method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'])
+    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
+        return False 
     opt_res_dayahead = input_data_dict['opt'].perform_dayahead_forecast_optim(
         df_input_data_dayahead, input_data_dict['P_PV_forecast'], input_data_dict['P_load_forecast'])
     # Save CSV file for publish_data
     if save_data_to_file:
-        today = datetime.now(timezone.utc).replace(hour=0, minute=0, second=0, microsecond=0)
-        filename = 'opt_res_dayahead_'+today.strftime("%Y_%m_%d")+'.csv'
-    else: # Just save the latest optimization results
-        filename = 'opt_res_latest.csv'
+        today = datetime.now(timezone.utc).replace(
+            hour=0, minute=0, second=0, microsecond=0
+        )
+        filename = "opt_res_dayahead_" + today.strftime("%Y_%m_%d") + ".csv"
+    else:  # Just save the latest optimization results
+        filename = "opt_res_latest.csv"
     if not debug:
-        opt_res_dayahead.to_csv(pathlib.Path(input_data_dict['root']) / filename, index_label='timestamp')
+        opt_res_dayahead.to_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
     return opt_res_dayahead
 
-def naive_mpc_optim(input_data_dict: dict, logger: logging.Logger,
-    save_data_to_file: Optional[bool] = False, debug: Optional[bool] = False) -> pd.DataFrame:
+
+def naive_mpc_optim(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    save_data_to_file: Optional[bool] = False,
+    debug: Optional[bool] = False,
+) -> pd.DataFrame:
     """
     Perform a call to the naive Model Predictive Controller optimization routine.
-    
+
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
     :param save_data_to_file: Save optimization results to CSV file
     :type save_data_to_file: bool, optional
     :param debug: A debug option useful for unittests
@@ -271,38 +396,54 @@
 
     """
     logger.info("Performing naive MPC optimization")
     # Load cost and prod price forecast
     df_input_data_dayahead = input_data_dict['fcst'].get_load_cost_forecast(
         input_data_dict['df_input_data_dayahead'],
         method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'])
+    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
+        return False 
     df_input_data_dayahead = input_data_dict['fcst'].get_prod_price_forecast(
         df_input_data_dayahead, method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'])
+    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
+        return False 
     # The specifics params for the MPC at runtime
-    prediction_horizon = input_data_dict['params']['passed_data']['prediction_horizon']
-    soc_init = input_data_dict['params']['passed_data']['soc_init']
-    soc_final = input_data_dict['params']['passed_data']['soc_final']
-    def_total_hours = input_data_dict['params']['passed_data']['def_total_hours']
-    def_start_timestep = input_data_dict['params']['passed_data']['def_start_timestep']
-    def_end_timestep = input_data_dict['params']['passed_data']['def_end_timestep']
-    opt_res_naive_mpc = input_data_dict['opt'].perform_naive_mpc_optim(
-        df_input_data_dayahead, input_data_dict['P_PV_forecast'], input_data_dict['P_load_forecast'],
-        prediction_horizon, soc_init, soc_final, def_total_hours, def_start_timestep, def_end_timestep)
+    prediction_horizon = input_data_dict["params"]["passed_data"]["prediction_horizon"]
+    soc_init = input_data_dict["params"]["passed_data"]["soc_init"]
+    soc_final = input_data_dict["params"]["passed_data"]["soc_final"]
+    def_total_hours = input_data_dict["params"]["passed_data"]["def_total_hours"]
+    def_start_timestep = input_data_dict["params"]["passed_data"]["def_start_timestep"]
+    def_end_timestep = input_data_dict["params"]["passed_data"]["def_end_timestep"]
+    opt_res_naive_mpc = input_data_dict["opt"].perform_naive_mpc_optim(
+        df_input_data_dayahead,
+        input_data_dict["P_PV_forecast"],
+        input_data_dict["P_load_forecast"],
+        prediction_horizon,
+        soc_init,
+        soc_final,
+        def_total_hours,
+        def_start_timestep,
+        def_end_timestep,
+    )
     # Save CSV file for publish_data
     if save_data_to_file:
-        today = datetime.now(timezone.utc).replace(hour=0, minute=0, second=0, microsecond=0)
-        filename = 'opt_res_naive_mpc_'+today.strftime("%Y_%m_%d")+'.csv'
-    else: # Just save the latest optimization results
-        filename = 'opt_res_latest.csv'
+        today = datetime.now(timezone.utc).replace(
+            hour=0, minute=0, second=0, microsecond=0
+        )
+        filename = "opt_res_naive_mpc_" + today.strftime("%Y_%m_%d") + ".csv"
+    else:  # Just save the latest optimization results
+        filename = "opt_res_latest.csv"
     if not debug:
-        opt_res_naive_mpc.to_csv(pathlib.Path(input_data_dict['root']) / filename, index_label='timestamp')
+        opt_res_naive_mpc.to_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
     return opt_res_naive_mpc
 
-def forecast_model_fit(input_data_dict: dict, logger: logging.Logger,
-    debug: Optional[bool] = False) -> Tuple[pd.DataFrame, pd.DataFrame, MLForecaster]:
+
+def forecast_model_fit(
+    input_data_dict: dict, logger: logging.Logger, debug: Optional[bool] = False
+) -> Tuple[pd.DataFrame, pd.DataFrame, MLForecaster]:
     """Perform a forecast model fit from training data retrieved from Home Assistant.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param debug: True to debug, useful for unit testing, defaults to False
@@ -313,30 +454,36 @@
     data = copy.deepcopy(input_data_dict['df_input_data'])
     model_type = input_data_dict['params']['passed_data']['model_type']
     var_model = input_data_dict['params']['passed_data']['var_model']
     sklearn_model = input_data_dict['params']['passed_data']['sklearn_model']
     num_lags = input_data_dict['params']['passed_data']['num_lags']
     split_date_delta = input_data_dict['params']['passed_data']['split_date_delta']
     perform_backtest = input_data_dict['params']['passed_data']['perform_backtest']
-    root = input_data_dict['root']
     # The ML forecaster object
-    mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, root, logger)
+    mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, input_data_dict['emhass_conf'], logger)
     # Fit the ML model
-    df_pred, df_pred_backtest = mlf.fit(split_date_delta=split_date_delta, 
-                                        perform_backtest=perform_backtest)
+    df_pred, df_pred_backtest = mlf.fit(
+        split_date_delta=split_date_delta, perform_backtest=perform_backtest
+    )
     # Save model
     if not debug:
         filename = model_type+'_mlf.pkl'
-        with open(pathlib.Path(root) / filename, 'wb') as outp:
+        filename_path = input_data_dict['emhass_conf']['data_path'] / filename
+        with open(filename_path, 'wb') as outp:
             pickle.dump(mlf, outp, pickle.HIGHEST_PROTOCOL)
     return df_pred, df_pred_backtest, mlf
 
-def forecast_model_predict(input_data_dict: dict, logger: logging.Logger,
-    use_last_window: Optional[bool] = True, debug: Optional[bool] = False,
-    mlf: Optional[MLForecaster] = None) -> pd.DataFrame:
+
+def forecast_model_predict(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    use_last_window: Optional[bool] = True,
+    debug: Optional[bool] = False,
+    mlf: Optional[MLForecaster] = None,
+) -> pd.DataFrame:
     r"""Perform a forecast model predict using a previously trained skforecast model.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param use_last_window: True if the 'last_window' option should be used for the \
@@ -351,59 +498,85 @@
         and unit testing. In production the actual model will be read from a saved pickle file. Defaults to None
     :type mlf: Optional[mlforecaster], optional
     :return: The DataFrame containing the forecast prediction data
     :rtype: pd.DataFrame
     """
     # Load model
     model_type = input_data_dict['params']['passed_data']['model_type']
-    root = input_data_dict['root']
     filename = model_type+'_mlf.pkl'
-    filename_path = pathlib.Path(root) / filename
+    filename_path = input_data_dict['emhass_conf']['data_path'] / filename
     if not debug:
         if filename_path.is_file():
-            with open(filename_path, 'rb') as inp:
+            with open(filename_path, "rb") as inp:
                 mlf = pickle.load(inp)
         else:
-            logger.error("The ML forecaster file was not found, please run a model fit method before this predict method")
+            logger.error(
+                "The ML forecaster file was not found, please run a model fit method before this predict method",
+            )
             return
     # Make predictions
     if use_last_window:
-        data_last_window = copy.deepcopy(input_data_dict['df_input_data'])
+        data_last_window = copy.deepcopy(input_data_dict["df_input_data"])
     else:
         data_last_window = None
     predictions = mlf.predict(data_last_window)
     # Publish data to a Home Assistant sensor
-    model_predict_publish = input_data_dict['params']['passed_data']['model_predict_publish']
-    model_predict_entity_id = input_data_dict['params']['passed_data']['model_predict_entity_id']
-    model_predict_unit_of_measurement = input_data_dict['params']['passed_data']['model_predict_unit_of_measurement']
-    model_predict_friendly_name = input_data_dict['params']['passed_data']['model_predict_friendly_name']
-    publish_prefix = input_data_dict['params']['passed_data']['publish_prefix']
+    model_predict_publish = input_data_dict["params"]["passed_data"][
+        "model_predict_publish"
+    ]
+    model_predict_entity_id = input_data_dict["params"]["passed_data"][
+        "model_predict_entity_id"
+    ]
+    model_predict_unit_of_measurement = input_data_dict["params"]["passed_data"][
+        "model_predict_unit_of_measurement"
+    ]
+    model_predict_friendly_name = input_data_dict["params"]["passed_data"][
+        "model_predict_friendly_name"
+    ]
+    publish_prefix = input_data_dict["params"]["passed_data"]["publish_prefix"]
     if model_predict_publish is True:
         # Estimate the current index
-        now_precise = datetime.now(input_data_dict['retrieve_hass_conf']['time_zone']).replace(second=0, microsecond=0)
-        if input_data_dict['retrieve_hass_conf']['method_ts_round'] == 'nearest':
-            idx_closest = predictions.index.get_indexer([now_precise], method='nearest')[0]
-        elif input_data_dict['retrieve_hass_conf']['method_ts_round'] == 'first':
-            idx_closest = predictions.index.get_indexer([now_precise], method='ffill')[0]
-        elif input_data_dict['retrieve_hass_conf']['method_ts_round'] == 'last':
-            idx_closest = predictions.index.get_indexer([now_precise], method='bfill')[0]
+        now_precise = datetime.now(
+            input_data_dict["retrieve_hass_conf"]["time_zone"]
+        ).replace(second=0, microsecond=0)
+        if input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "nearest":
+            idx_closest = predictions.index.get_indexer(
+                [now_precise], method="nearest"
+            )[0]
+        elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "first":
+            idx_closest = predictions.index.get_indexer([now_precise], method="ffill")[
+                0
+            ]
+        elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "last":
+            idx_closest = predictions.index.get_indexer([now_precise], method="bfill")[
+                0
+            ]
         if idx_closest == -1:
-            idx_closest = predictions.index.get_indexer([now_precise], method='nearest')[0]
+            idx_closest = predictions.index.get_indexer(
+                [now_precise], method="nearest"
+            )[0]
         # Publish Load forecast
-        input_data_dict['rh'].post_data(predictions, idx_closest, 
-                                        model_predict_entity_id,
-                                        model_predict_unit_of_measurement, 
-                                        model_predict_friendly_name,
-                                        type_var = 'mlforecaster',
-                                        publish_prefix=publish_prefix)
+        input_data_dict["rh"].post_data(
+            predictions,
+            idx_closest,
+            model_predict_entity_id,
+            model_predict_unit_of_measurement,
+            model_predict_friendly_name,
+            type_var="mlforecaster",
+            publish_prefix=publish_prefix,
+        )
     return predictions
 
-def forecast_model_tune(input_data_dict: dict, logger: logging.Logger,
-    debug: Optional[bool] = False, mlf: Optional[MLForecaster] = None
-    ) -> Tuple[pd.DataFrame, MLForecaster]:
+
+def forecast_model_tune(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    debug: Optional[bool] = False,
+    mlf: Optional[MLForecaster] = None,
+) -> Tuple[pd.DataFrame, MLForecaster]:
     """Tune a forecast model hyperparameters using bayesian optimization.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param debug: True to debug, useful for unit testing, defaults to False
@@ -412,266 +585,524 @@
         and unit testing. In production the actual model will be read from a saved pickle file. Defaults to None
     :type mlf: Optional[mlforecaster], optional
     :return: The DataFrame containing the forecast data results using the optimized model
     :rtype: pd.DataFrame
     """
     # Load model
     model_type = input_data_dict['params']['passed_data']['model_type']
-    root = input_data_dict['root']
     filename = model_type+'_mlf.pkl'
-    filename_path = pathlib.Path(root) / filename
+    filename_path = input_data_dict['emhass_conf']['data_path'] / filename
     if not debug:
         if filename_path.is_file():
-            with open(filename_path, 'rb') as inp:
+            with open(filename_path, "rb") as inp:
                 mlf = pickle.load(inp)
         else:
-            logger.error("The ML forecaster file was not found, please run a model fit method before this tune method")
+            logger.error(
+                "The ML forecaster file was not found, please run a model fit method before this tune method",
+            )
             return None, None
     # Tune the model
     df_pred_optim = mlf.tune(debug=debug)
     # Save model
     if not debug:
         filename = model_type+'_mlf.pkl'
-        with open(pathlib.Path(root) / filename, 'wb') as outp:
-            pickle.dump(mlf, outp, pickle.HIGHEST_PROTOCOL)
+        filename_path = input_data_dict['emhass_conf']['data_path'] / filename
+        with open(filename_path, 'wb') as outp:
+            pickle.dump(mlf, outp, pickle.HIGHEST_PROTOCOL)       
     return df_pred_optim, mlf
 
-def publish_data(input_data_dict: dict, logger: logging.Logger,
-    save_data_to_file: Optional[bool] = False, 
-    opt_res_latest: Optional[pd.DataFrame] = None) -> pd.DataFrame:
+
+def regressor_model_fit(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    debug: Optional[bool] = False,
+) -> None:
+    """Perform a forecast model fit from training data retrieved from Home Assistant.
+
+    :param input_data_dict: A dictionnary with multiple data used by the action functions
+    :type input_data_dict: dict
+    :param logger: The passed logger object
+    :type logger: logging.Logger
+    :param debug: True to debug, useful for unit testing, defaults to False
+    :type debug: Optional[bool], optional
     """
-    Publish the data obtained from the optimization results.
+    data = copy.deepcopy(input_data_dict["df_input_data"])
+    if "model_type" in input_data_dict["params"]["passed_data"]:
+        model_type = input_data_dict["params"]["passed_data"]["model_type"]
+    else:
+        logger.error("parameter: 'model_type' not passed")
+        return False
+    if "regression_model" in input_data_dict["params"]["passed_data"]:
+        regression_model = input_data_dict["params"]["passed_data"]["regression_model"]
+    else:
+        logger.error("parameter: 'regression_model' not passed")
+        return False
+    if "features" in input_data_dict["params"]["passed_data"]:
+        features = input_data_dict["params"]["passed_data"]["features"]
+    else:
+        logger.error("parameter: 'features' not passed")
+        return False    
+    if "target" in input_data_dict["params"]["passed_data"]:
+        target = input_data_dict["params"]["passed_data"]["target"]
+    else:
+        logger.error("parameter: 'target' not passed")
+        return False        
+    if "timestamp" in input_data_dict["params"]["passed_data"]:
+        timestamp = input_data_dict["params"]["passed_data"]["timestamp"]
+    else:
+        logger.error("parameter: 'timestamp' not passed")
+        return False       
+    if "date_features" in input_data_dict["params"]["passed_data"]:
+        date_features = input_data_dict["params"]["passed_data"]["date_features"]
+    else:
+        logger.error("parameter: 'date_features' not passed")
+        return False           
+
+    # The MLRegressor object
+    mlr = MLRegressor(
+        data,
+        model_type,
+        regression_model,
+        features,
+        target,
+        timestamp,
+        logger,
+    )
+    # Fit the ML model
+    mlr.fit(date_features=date_features)
+    # Save model
+    if not debug:
+        filename = model_type + "_mlr.pkl"
+        filename_path = input_data_dict["emhass_conf"]["data_path"] / filename
+        with open(filename_path, "wb") as outp:
+            pickle.dump(mlr, outp, pickle.HIGHEST_PROTOCOL)
+    return mlr
+
+
+def regressor_model_predict(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    debug: Optional[bool] = False,
+    mlr: Optional[MLRegressor] = None,
+) -> None:
+    """Perform a prediction from csv file.
+
+    :param input_data_dict: A dictionnary with multiple data used by the action functions
+    :type input_data_dict: dict
+    :param logger: The passed logger object
+    :type logger: logging.Logger
+    :param debug: True to debug, useful for unit testing, defaults to False
+    :type debug: Optional[bool], optional
+    """
+    if "model_type" in input_data_dict["params"]["passed_data"]:
+        model_type = input_data_dict["params"]["passed_data"]["model_type"]
+    else:
+        logger.error("parameter: 'model_type' not passed")
+        return False   
+    filename = model_type + "_mlr.pkl"
+    filename_path = input_data_dict["emhass_conf"]["data_path"] / filename
+    if not debug:
+        if filename_path.is_file():
+            with open(filename_path, "rb") as inp:
+                mlr = pickle.load(inp)
+        else:
+            logger.error(
+                "The ML forecaster file was not found, please run a model fit method before this predict method",
+            )
+            return False
+    if "new_values" in input_data_dict["params"]["passed_data"]:    
+        new_values = input_data_dict["params"]["passed_data"]["new_values"]
+    else:
+        logger.error("parameter: 'new_values' not passed")
+        return False         
+    # Predict from csv file
+    prediction = mlr.predict(new_values)
     
+    mlr_predict_entity_id = input_data_dict["params"]["passed_data"].get("mlr_predict_entity_id","sensor.mlr_predict")
+    mlr_predict_unit_of_measurement = input_data_dict["params"]["passed_data"].get("mlr_predict_unit_of_measurement","h")
+    mlr_predict_friendly_name = input_data_dict["params"]["passed_data"].get("mlr_predict_friendly_name","mlr predictor")
+    # Publish prediction
+    idx = 0
+    if not debug:
+        input_data_dict["rh"].post_data(
+            prediction,
+            idx,
+            mlr_predict_entity_id,
+            mlr_predict_unit_of_measurement,
+            mlr_predict_friendly_name,
+            type_var="mlregressor",
+        )
+    return prediction
+
+
+def publish_data(
+    input_data_dict: dict,
+    logger: logging.Logger,
+    save_data_to_file: Optional[bool] = False,
+    opt_res_latest: Optional[pd.DataFrame] = None,
+) -> pd.DataFrame:
+    """
+    Publish the data obtained from the optimization results.
+
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
     :param save_data_to_file: If True we will read data from optimization results in dayahead CSV file
     :type save_data_to_file: bool, optional
     :return: The output data of the optimization readed from a CSV file in the data folder
     :rtype: pd.DataFrame
 
     """
     logger.info("Publishing data to HASS instance")
     # Check if a day ahead optimization has been performed (read CSV file)
     if save_data_to_file:
-        today = datetime.now(timezone.utc).replace(hour=0, minute=0, second=0, microsecond=0)
-        filename = 'opt_res_dayahead_'+today.strftime("%Y_%m_%d")+'.csv'
+        today = datetime.now(timezone.utc).replace(
+            hour=0, minute=0, second=0, microsecond=0
+        )
+        filename = "opt_res_dayahead_" + today.strftime("%Y_%m_%d") + ".csv"
     else:
-        filename = 'opt_res_latest.csv'
+        filename = "opt_res_latest.csv"
     if opt_res_latest is None:
-        if not os.path.isfile(pathlib.Path(input_data_dict['root']) / filename):
+        if not os.path.isfile(input_data_dict['emhass_conf']['data_path'] / filename):
             logger.error("File not found error, run an optimization task first.")
             return
         else:
-            opt_res_latest = pd.read_csv(pathlib.Path(input_data_dict['root']) / filename, index_col='timestamp')
+            opt_res_latest = pd.read_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_col='timestamp')
             opt_res_latest.index = pd.to_datetime(opt_res_latest.index)
-            opt_res_latest.index.freq = input_data_dict['retrieve_hass_conf']['freq']
+            opt_res_latest.index.freq = input_data_dict["retrieve_hass_conf"]["freq"]
     # Estimate the current index
-    now_precise = datetime.now(input_data_dict['retrieve_hass_conf']['time_zone']).replace(second=0, microsecond=0)
-    if input_data_dict['retrieve_hass_conf']['method_ts_round'] == 'nearest':
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method='nearest')[0]
-    elif input_data_dict['retrieve_hass_conf']['method_ts_round'] == 'first':
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method='ffill')[0]
-    elif input_data_dict['retrieve_hass_conf']['method_ts_round'] == 'last':
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method='bfill')[0]
+    now_precise = datetime.now(
+        input_data_dict["retrieve_hass_conf"]["time_zone"]
+    ).replace(second=0, microsecond=0)
+    if input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "nearest":
+        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="nearest")[
+            0
+        ]
+    elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "first":
+        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="ffill")[0]
+    elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "last":
+        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="bfill")[0]
     if idx_closest == -1:
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method='nearest')[0]
+        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="nearest")[
+            0
+        ]
     # Publish the data
-    params = json.loads(input_data_dict['params'])
-    publish_prefix = params['passed_data']['publish_prefix']
+    params = json.loads(input_data_dict["params"])
+    publish_prefix = params["passed_data"]["publish_prefix"]
     # Publish PV forecast
-    custom_pv_forecast_id = params['passed_data']['custom_pv_forecast_id']
-    input_data_dict['rh'].post_data(opt_res_latest['P_PV'], idx_closest, 
-                                    custom_pv_forecast_id["entity_id"], 
-                                    custom_pv_forecast_id["unit_of_measurement"],
-                                    custom_pv_forecast_id["friendly_name"],
-                                    type_var = 'power',
-                                    publish_prefix = publish_prefix)
+    custom_pv_forecast_id = params["passed_data"]["custom_pv_forecast_id"]
+    input_data_dict["rh"].post_data(
+        opt_res_latest["P_PV"],
+        idx_closest,
+        custom_pv_forecast_id["entity_id"],
+        custom_pv_forecast_id["unit_of_measurement"],
+        custom_pv_forecast_id["friendly_name"],
+        type_var="power",
+        publish_prefix=publish_prefix,
+    )
     # Publish Load forecast
-    custom_load_forecast_id = params['passed_data']['custom_load_forecast_id']
-    input_data_dict['rh'].post_data(opt_res_latest['P_Load'], idx_closest, 
-                                    custom_load_forecast_id["entity_id"], 
-                                    custom_load_forecast_id["unit_of_measurement"],
-                                    custom_load_forecast_id["friendly_name"],
-                                    type_var = 'power',
-                                    publish_prefix = publish_prefix)
-    cols_published = ['P_PV', 'P_Load']
+    custom_load_forecast_id = params["passed_data"]["custom_load_forecast_id"]
+    input_data_dict["rh"].post_data(
+        opt_res_latest["P_Load"],
+        idx_closest,
+        custom_load_forecast_id["entity_id"],
+        custom_load_forecast_id["unit_of_measurement"],
+        custom_load_forecast_id["friendly_name"],
+        type_var="power",
+        publish_prefix=publish_prefix,
+    )
+    cols_published = ["P_PV", "P_Load"]
     # Publish deferrable loads
-    custom_deferrable_forecast_id = params['passed_data']['custom_deferrable_forecast_id']
-    for k in range(input_data_dict['opt'].optim_conf['num_def_loads']):
+    custom_deferrable_forecast_id = params["passed_data"][
+        "custom_deferrable_forecast_id"
+    ]
+    for k in range(input_data_dict["opt"].optim_conf["num_def_loads"]):
         if "P_deferrable{}".format(k) not in opt_res_latest.columns:
-            logger.error("P_deferrable{}".format(k)+" was not found in results DataFrame. Optimization task may need to be relaunched or it did not converge to a solution.")
+            logger.error(
+                "P_deferrable{}".format(k)
+                + " was not found in results DataFrame. Optimization task may need to be relaunched or it did not converge to a solution.",
+            )
         else:
-            input_data_dict['rh'].post_data(opt_res_latest["P_deferrable{}".format(k)], idx_closest, 
-                                            custom_deferrable_forecast_id[k]["entity_id"], 
-                                            custom_deferrable_forecast_id[k]["unit_of_measurement"],
-                                            custom_deferrable_forecast_id[k]["friendly_name"],
-                                            type_var = 'deferrable',
-                                            publish_prefix = publish_prefix)
-            cols_published = cols_published+["P_deferrable{}".format(k)]
+            input_data_dict["rh"].post_data(
+                opt_res_latest["P_deferrable{}".format(k)],
+                idx_closest,
+                custom_deferrable_forecast_id[k]["entity_id"],
+                custom_deferrable_forecast_id[k]["unit_of_measurement"],
+                custom_deferrable_forecast_id[k]["friendly_name"],
+                type_var="deferrable",
+                publish_prefix=publish_prefix,
+            )
+            cols_published = cols_published + ["P_deferrable{}".format(k)]
     # Publish battery power
-    if input_data_dict['opt'].optim_conf['set_use_battery']:
-        if 'P_batt' not in opt_res_latest.columns:
-            logger.error("P_batt was not found in results DataFrame. Optimization task may need to be relaunched or it did not converge to a solution.")
-        else:
-            custom_batt_forecast_id = params['passed_data']['custom_batt_forecast_id']
-            input_data_dict['rh'].post_data(opt_res_latest['P_batt'], idx_closest,
-                                            custom_batt_forecast_id["entity_id"], 
-                                            custom_batt_forecast_id["unit_of_measurement"],
-                                            custom_batt_forecast_id["friendly_name"],
-                                            type_var = 'batt',
-                                            publish_prefix = publish_prefix)
-            cols_published = cols_published+["P_batt"]
-            custom_batt_soc_forecast_id = params['passed_data']['custom_batt_soc_forecast_id']
-            input_data_dict['rh'].post_data(opt_res_latest['SOC_opt']*100, idx_closest,
-                                            custom_batt_soc_forecast_id["entity_id"], 
-                                            custom_batt_soc_forecast_id["unit_of_measurement"],
-                                            custom_batt_soc_forecast_id["friendly_name"],
-                                            type_var = 'SOC',
-                                            publish_prefix = publish_prefix)
-            cols_published = cols_published+["SOC_opt"]
+    if input_data_dict["opt"].optim_conf["set_use_battery"]:
+        if "P_batt" not in opt_res_latest.columns:
+            logger.error(
+                "P_batt was not found in results DataFrame. Optimization task may need to be relaunched or it did not converge to a solution.",
+            )
+        else:
+            custom_batt_forecast_id = params["passed_data"]["custom_batt_forecast_id"]
+            input_data_dict["rh"].post_data(
+                opt_res_latest["P_batt"],
+                idx_closest,
+                custom_batt_forecast_id["entity_id"],
+                custom_batt_forecast_id["unit_of_measurement"],
+                custom_batt_forecast_id["friendly_name"],
+                type_var="batt",
+                publish_prefix=publish_prefix,
+            )
+            cols_published = cols_published + ["P_batt"]
+            custom_batt_soc_forecast_id = params["passed_data"][
+                "custom_batt_soc_forecast_id"
+            ]
+            input_data_dict["rh"].post_data(
+                opt_res_latest["SOC_opt"] * 100,
+                idx_closest,
+                custom_batt_soc_forecast_id["entity_id"],
+                custom_batt_soc_forecast_id["unit_of_measurement"],
+                custom_batt_soc_forecast_id["friendly_name"],
+                type_var="SOC",
+                publish_prefix=publish_prefix,
+            )
+            cols_published = cols_published + ["SOC_opt"]
     # Publish grid power
-    custom_grid_forecast_id = params['passed_data']['custom_grid_forecast_id']
-    input_data_dict['rh'].post_data(opt_res_latest['P_grid'], idx_closest, 
-                                    custom_grid_forecast_id["entity_id"], 
-                                    custom_grid_forecast_id["unit_of_measurement"],
-                                    custom_grid_forecast_id["friendly_name"],
-                                    type_var = 'power',
-                                    publish_prefix = publish_prefix)
-    cols_published = cols_published+["P_grid"]
+    custom_grid_forecast_id = params["passed_data"]["custom_grid_forecast_id"]
+    input_data_dict["rh"].post_data(
+        opt_res_latest["P_grid"],
+        idx_closest,
+        custom_grid_forecast_id["entity_id"],
+        custom_grid_forecast_id["unit_of_measurement"],
+        custom_grid_forecast_id["friendly_name"],
+        type_var="power",
+        publish_prefix=publish_prefix,
+    )
+    cols_published = cols_published + ["P_grid"]
     # Publish total value of cost function
-    custom_cost_fun_id = params['passed_data']['custom_cost_fun_id']
-    col_cost_fun = [i for i in opt_res_latest.columns if 'cost_fun_' in i]
-    input_data_dict['rh'].post_data(opt_res_latest[col_cost_fun], idx_closest, 
-                                    custom_cost_fun_id["entity_id"], 
-                                    custom_cost_fun_id["unit_of_measurement"],
-                                    custom_cost_fun_id["friendly_name"],
-                                    type_var = 'cost_fun',
-                                    publish_prefix = publish_prefix)
+    custom_cost_fun_id = params["passed_data"]["custom_cost_fun_id"]
+    col_cost_fun = [i for i in opt_res_latest.columns if "cost_fun_" in i]
+    input_data_dict["rh"].post_data(
+        opt_res_latest[col_cost_fun],
+        idx_closest,
+        custom_cost_fun_id["entity_id"],
+        custom_cost_fun_id["unit_of_measurement"],
+        custom_cost_fun_id["friendly_name"],
+        type_var="cost_fun",
+        publish_prefix=publish_prefix,
+    )
     # Publish the optimization status
-    custom_cost_fun_id = params['passed_data']['custom_optim_status_id']
+    custom_cost_fun_id = params["passed_data"]["custom_optim_status_id"]
     if "optim_status" not in opt_res_latest:
-        opt_res_latest["optim_status"] = 'Optimal'
-        logger.warning("no optim_status in opt_res_latest, run an optimization task first")
-    input_data_dict['rh'].post_data(opt_res_latest['optim_status'], idx_closest, 
-                                    custom_cost_fun_id["entity_id"], 
-                                    custom_cost_fun_id["unit_of_measurement"],
-                                    custom_cost_fun_id["friendly_name"],
-                                    type_var = 'optim_status',
-                                    publish_prefix = publish_prefix)
-    cols_published = cols_published+["optim_status"]
+        opt_res_latest["optim_status"] = "Optimal"
+        logger.warning(
+            "no optim_status in opt_res_latest, run an optimization task first",
+        )
+    input_data_dict["rh"].post_data(
+        opt_res_latest["optim_status"],
+        idx_closest,
+        custom_cost_fun_id["entity_id"],
+        custom_cost_fun_id["unit_of_measurement"],
+        custom_cost_fun_id["friendly_name"],
+        type_var="optim_status",
+        publish_prefix=publish_prefix,
+    )
+    cols_published = cols_published + ["optim_status"]
     # Publish unit_load_cost
-    custom_unit_load_cost_id = params['passed_data']['custom_unit_load_cost_id']
-    input_data_dict['rh'].post_data(opt_res_latest['unit_load_cost'], idx_closest, 
-                                    custom_unit_load_cost_id["entity_id"], 
-                                    custom_unit_load_cost_id["unit_of_measurement"],
-                                    custom_unit_load_cost_id["friendly_name"],
-                                    type_var = 'unit_load_cost',
-                                    publish_prefix = publish_prefix)
-    cols_published = cols_published+["unit_load_cost"]
+    custom_unit_load_cost_id = params["passed_data"]["custom_unit_load_cost_id"]
+    input_data_dict["rh"].post_data(
+        opt_res_latest["unit_load_cost"],
+        idx_closest,
+        custom_unit_load_cost_id["entity_id"],
+        custom_unit_load_cost_id["unit_of_measurement"],
+        custom_unit_load_cost_id["friendly_name"],
+        type_var="unit_load_cost",
+        publish_prefix=publish_prefix,
+    )
+    cols_published = cols_published + ["unit_load_cost"]
     # Publish unit_prod_price
-    custom_unit_prod_price_id = params['passed_data']['custom_unit_prod_price_id']
-    input_data_dict['rh'].post_data(opt_res_latest['unit_prod_price'], idx_closest, 
-                                    custom_unit_prod_price_id["entity_id"], 
-                                    custom_unit_prod_price_id["unit_of_measurement"],
-                                    custom_unit_prod_price_id["friendly_name"],
-                                    type_var = 'unit_prod_price',
-                                    publish_prefix = publish_prefix)
-    cols_published = cols_published+["unit_prod_price"]
+    custom_unit_prod_price_id = params["passed_data"]["custom_unit_prod_price_id"]
+    input_data_dict["rh"].post_data(
+        opt_res_latest["unit_prod_price"],
+        idx_closest,
+        custom_unit_prod_price_id["entity_id"],
+        custom_unit_prod_price_id["unit_of_measurement"],
+        custom_unit_prod_price_id["friendly_name"],
+        type_var="unit_prod_price",
+        publish_prefix=publish_prefix,
+    )
+    cols_published = cols_published + ["unit_prod_price"]
     # Create a DF resuming what has been published
     opt_res = opt_res_latest[cols_published].loc[[opt_res_latest.index[idx_closest]]]
     return opt_res
-    
-        
+
+
 def main():
     r"""Define the main command line entry function.
 
     This function may take several arguments as inputs. You can type `emhass --help` to see the list of options:
-    
+
     - action: Set the desired action, options are: perfect-optim, dayahead-optim,
       naive-mpc-optim, publish-data, forecast-model-fit, forecast-model-predict, forecast-model-tune
-      
+
     - config: Define path to the config.yaml file
-    
+
     - costfun: Define the type of cost function, options are: profit, cost, self-consumption
-    
+
     - log2file: Define if we should log to a file or not
-    
+
     - params: Configuration parameters passed from data/options.json if using the add-on
-    
+
     - runtimeparams: Pass runtime optimization parameters as dictionnary
-    
+
     - debug: Use True for testing purposes
-    
+
     """
     # Parsing arguments
     parser = argparse.ArgumentParser()
     parser.add_argument('--action', type=str, help='Set the desired action, options are: perfect-optim, dayahead-optim,\
         naive-mpc-optim, publish-data, forecast-model-fit, forecast-model-predict, forecast-model-tune')
     parser.add_argument('--config', type=str, help='Define path to the config.yaml file')
+    parser.add_argument('--data', type=str, help='Define path to the Data files (.csv & .pkl)')
+    parser.add_argument('--root', type=str, help='Define path emhass root')
     parser.add_argument('--costfun', type=str, default='profit', help='Define the type of cost function, options are: profit, cost, self-consumption')
     parser.add_argument('--log2file', type=strtobool, default='False', help='Define if we should log to a file or not')
     parser.add_argument('--params', type=str, default=None, help='Configuration parameters passed from data/options.json')
     parser.add_argument('--runtimeparams', type=str, default=None, help='Pass runtime optimization parameters as dictionnary')
     parser.add_argument('--debug', type=strtobool, default='False', help='Use True for testing purposes')
     args = parser.parse_args()
     # The path to the configuration files
-    config_path = pathlib.Path(args.config)
-    base_path = str(config_path.parent)
+    
+    if args.config is not None:
+        config_path = pathlib.Path(args.config)
+    else:
+        config_path = pathlib.Path(str(utils.get_root(__file__, num_parent=2) / 'config_emhass.yaml' ))
+
+    if args.data is not None:
+        data_path = pathlib.Path(args.data)
+    else:
+        data_path = (config_path.parent / 'data/')
+
+    if args.root is not None:
+        root_path = pathlib.Path(args.root)
+    else:
+        root_path = config_path.parent
+    
+    emhass_conf = {}
+    emhass_conf['config_path'] = config_path
+    emhass_conf['data_path'] = data_path
+    emhass_conf['root_path'] = root_path
     # create logger
-    logger, ch = utils.get_logger(__name__, base_path, save_to_file=bool(args.log2file))
+    logger, ch = utils.get_logger(__name__, emhass_conf, save_to_file=bool(args.log2file))
+    
+    logger.debug("config path: " + str(config_path))
+    logger.debug("data path: " + str(data_path))
+    logger.debug("root path: " + str(root_path))
+
+
+    if not config_path.exists():
+        logger.error("Could not find config_emhass.yaml file in: " + str(config_path))
+        logger.error("Try setting config file path with --config" )
+        return False
+
+    if not os.path.isdir(data_path):
+        logger.error("Could not find data foulder in: " + str(data_path))
+        logger.error("Try setting data path with --data" )
+        return False
+
+    if not os.path.isdir(root_path / 'src'):
+        logger.error("Could not find emhass/src foulder in: " + str(root_path))
+        logger.error("Try setting emhass root path with --root" )
+        return False
+
     # Additionnal argument
     try:
-        parser.add_argument('--version', action='version', version='%(prog)s '+version('emhass'))
+        parser.add_argument(
+            "--version",
+            action="version",
+            version="%(prog)s " + version("emhass"),
+        )
         args = parser.parse_args()
     except Exception:
-        logger.info("Version not found for emhass package. Or importlib exited with PackageNotFoundError.")
+        logger.info(
+            "Version not found for emhass package. Or importlib exited with PackageNotFoundError.",
+        )
     # Setup parameters
-    input_data_dict = set_input_data_dict(config_path, base_path, 
+    input_data_dict = set_input_data_dict(emhass_conf, 
                                           args.costfun, args.params, args.runtimeparams, args.action, 
                                           logger, args.debug)
     # Perform selected action
-    if args.action == 'perfect-optim':
+    if args.action == "perfect-optim":
         opt_res = perfect_forecast_optim(input_data_dict, logger, debug=args.debug)
-    elif args.action == 'dayahead-optim':
+    elif args.action == "dayahead-optim":
         opt_res = dayahead_forecast_optim(input_data_dict, logger, debug=args.debug)
-    elif args.action == 'naive-mpc-optim':
+    elif args.action == "naive-mpc-optim":
         opt_res = naive_mpc_optim(input_data_dict, logger, debug=args.debug)
-    elif args.action == 'forecast-model-fit':
-        df_fit_pred, df_fit_pred_backtest, mlf = forecast_model_fit(input_data_dict, logger, debug=args.debug)
+    elif args.action == "forecast-model-fit":
+        df_fit_pred, df_fit_pred_backtest, mlf = forecast_model_fit(
+            input_data_dict, logger, debug=args.debug
+        )
         opt_res = None
-    elif args.action == 'forecast-model-predict':
+    elif args.action == "forecast-model-predict":
         if args.debug:
             _, _, mlf = forecast_model_fit(input_data_dict, logger, debug=args.debug)
         else:
             mlf = None
-        df_pred = forecast_model_predict(input_data_dict, logger, debug=args.debug, mlf=mlf)
+        df_pred = forecast_model_predict(
+            input_data_dict, logger, debug=args.debug, mlf=mlf
+        )
         opt_res = None
-    elif args.action == 'forecast-model-tune':
+    elif args.action == "forecast-model-tune":
         if args.debug:
             _, _, mlf = forecast_model_fit(input_data_dict, logger, debug=args.debug)
         else:
             mlf = None
-        df_pred_optim, mlf = forecast_model_tune(input_data_dict, logger, debug=args.debug, mlf=mlf)
+        df_pred_optim, mlf = forecast_model_tune(
+            input_data_dict, logger, debug=args.debug, mlf=mlf
+        )
+        opt_res = None
+    elif args.action == "regressor-model-fit":
+        mlr = regressor_model_fit(input_data_dict, logger, debug=args.debug)
         opt_res = None
-    elif args.action == 'publish-data':
+    elif args.action == "regressor-model-predict":
+        if args.debug:
+            mlr = regressor_model_fit(input_data_dict, logger, debug=args.debug)
+        else:
+            mlr = None
+        prediction = regressor_model_predict(
+            input_data_dict,
+            logger,
+            debug=args.debug,
+            mlr=mlr,
+        )
+        opt_res = None
+    elif args.action == "publish-data":
         opt_res = publish_data(input_data_dict, logger)
     else:
         logger.error("The passed action argument is not valid")
+        logger.error("Try setting --action: perfect-optim, dayahead-optim, naive-mpc-optim, forecast-model-fit, forecast-model-predict, forecast-model-tune or publish-data")
         opt_res = None
     logger.info(opt_res)
     # Flush the logger
     ch.close()
     logger.removeHandler(ch)
-    if args.action == 'perfect-optim' or args.action == 'dayahead-optim' or \
-        args.action == 'naive-mpc-optim' or args.action == 'publish-data':
+    if (
+        args.action == "perfect-optim"
+        or args.action == "dayahead-optim"
+        or args.action == "naive-mpc-optim"
+        or args.action == "publish-data"
+    ):
         return opt_res
-    elif args.action == 'forecast-model-fit':
+    elif args.action == "forecast-model-fit":
         return df_fit_pred, df_fit_pred_backtest, mlf
-    elif args.action == 'forecast-model-predict':
+    elif args.action == "forecast-model-predict":
         return df_pred
-    elif args.action == 'forecast-model-tune':
+    elif args.action == "regressor-model-fit":
+        return mlr
+    elif args.action == "regressor-model-predict":
+        return prediction
+    elif args.action == "forecast-model-tune":
         return df_pred_optim, mlf
+    else: 
+        return opt_res
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `emhass-0.8.6/src/emhass/data/cec_inverters.pbz2` & `emhass-0.9.0/src/emhass/data/cec_inverters.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/data/cec_modules.pbz2` & `emhass-0.9.0/src/emhass/data/cec_modules.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/forecast.py` & `emhass-0.9.0/src/emhass/forecast.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import pathlib
+import os
 import pickle
 import copy
 import logging
 import json
 from typing import Optional
 import bz2
 import pickle as cPickle
@@ -19,15 +20,15 @@
 from pvlib.location import Location
 from pvlib.modelchain import ModelChain
 from pvlib.temperature import TEMPERATURE_MODEL_PARAMETERS
 from pvlib.irradiance import disc
 
 from emhass.retrieve_hass import RetrieveHass
 from emhass.machine_learning_forecaster import MLForecaster
-from emhass.utils import get_days_list, get_root, set_df_index_freq
+from emhass.utils import get_days_list, set_df_index_freq
 
 
 class Forecast(object):
     r"""
     Generate weather, load and costs forecasts needed as inputs to the optimization.
     
     In EMHASS we have basically 4 forecasts to deal with:
@@ -94,33 +95,33 @@
     
     The data columns in these files will correspond to the data in the units expected
     for each forecasting method.
     
     """
 
     def __init__(self, retrieve_hass_conf: dict, optim_conf: dict, plant_conf: dict, 
-                 params: str, base_path: str, logger: logging.Logger, 
+                 params: str, emhass_conf: dict, logger: logging.Logger, 
                  opt_time_delta: Optional[int] = 24,
                  get_data_from_file: Optional[bool] = False) -> None:
         """
         Define constructor for the forecast class.
         
-        :param retrieve_hass_conf: Dictionnary containing the needed configuration
+        :param retrieve_hass_conf: Dictionary containing the needed configuration
             data from the configuration file, specific to retrieve data from HASS
         :type retrieve_hass_conf: dict
-        :param optim_conf: Dictionnary containing the needed configuration
+        :param optim_conf: Dictionary containing the needed configuration
             data from the configuration file, specific for the optimization task
         :type optim_conf: dict
-        :param plant_conf: Dictionnary containing the needed configuration
+        :param plant_conf: Dictionary containing the needed configuration
             data from the configuration file, specific for the modeling of the PV plant
         :type plant_conf: dict
         :param params: Configuration parameters passed from data/options.json
         :type params: str
-        :param base_path: The path to the yaml configuration file
-        :type base_path: str
+        :param emhass_conf: Dictionary containing the needed emhass paths
+        :type emhass_conf: dict
         :param logger: The passed logger object
         :type logger: logging object
         :param opt_time_delta: The time delta in hours used to generate forecasts, 
             a value of 24 will generate 24 hours of forecast data, defaults to 24
         :type opt_time_delta: int, optional
         :param get_data_from_file: Select if data should be retrieved from a 
             previously saved pickle useful for testing or directly from connection to
@@ -137,15 +138,15 @@
         self.timeStep = self.freq.seconds/3600 # in hours
         self.time_delta = pd.to_timedelta(opt_time_delta, "hours")
         self.var_PV = self.retrieve_hass_conf['var_PV']
         self.var_load = self.retrieve_hass_conf['var_load']
         self.var_load_new = self.var_load+'_positive'
         self.lat = self.retrieve_hass_conf['lat'] 
         self.lon = self.retrieve_hass_conf['lon']
-        self.root = base_path
+        self.emhass_conf = emhass_conf
         self.logger = logger
         self.get_data_from_file = get_data_from_file
         self.var_load_cost = 'unit_load_cost'
         self.var_prod_price = 'unit_prod_price'
         if params is None:
             self.params = params
         else:
@@ -165,25 +166,27 @@
         if params is not None:
             if 'prediction_horizon' in list(self.params['passed_data'].keys()):
                 if self.params['passed_data']['prediction_horizon'] is not None:
                     self.forecast_dates = self.forecast_dates[0:self.params['passed_data']['prediction_horizon']]
         
         
     def get_weather_forecast(self, method: Optional[str] = 'scrapper',
-                             csv_path: Optional[str] = "/data/data_weather_forecast.csv") -> pd.DataFrame:
+                             csv_path: Optional[str] = "data_weather_forecast.csv") -> pd.DataFrame:
         r"""
         Get and generate weather forecast data.
         
         :param method: The desired method, options are 'scrapper', 'csv', 'list', 'solcast' and \
             'solar.forecast'. Defaults to 'scrapper'.
         :type method: str, optional
         :return: The DataFrame containing the forecasted data
         :rtype: pd.DataFrame
         
         """
+        csv_path  = self.emhass_conf['data_path'] / csv_path
+
         self.logger.info("Retrieving weather forecast data using method = "+method)
         self.weather_forecast_method = method # Saving this attribute for later use to identify csv method usage
         if method == 'scrapper':
             freq_scrap = pd.to_timedelta(60, "minutes") # The scrapping time step is 60min
             forecast_dates_scrap = pd.date_range(start=self.start_forecast,
                                                  end=self.end_forecast-freq_scrap, 
                                                  freq=freq_scrap).round(freq_scrap, ambiguous='infer', nonexistent='shift_forward')
@@ -288,15 +291,15 @@
                 data_tmp.loc[data_tmp.index[mask_down_data_df['yhat']==True],:] = 0.0
                 data_tmp.interpolate(inplace=True)
                 if len(data) == 0:
                     data = copy.deepcopy(data_tmp)
                 else:
                     data = data + data_tmp
         elif method == 'csv': # reading from a csv file
-            weather_csv_file_path = self.root + csv_path
+            weather_csv_file_path = csv_path
             # Loading the csv file, we will consider that this is the PV power in W
             data = pd.read_csv(weather_csv_file_path, header=None, names=['ts', 'yhat'])
             # Check if the passed data has the correct length       
             if len(data) < len(self.forecast_dates):
                 self.logger.error("Passed data from CSV is not long enough")
             else:
                 # Ensure correct length
@@ -410,17 +413,17 @@
                 P_PV_forecast = df_weather['yhat']
                 P_PV_forecast.name = None
             else: # We will transform the weather data into electrical power
                 # Transform to power (Watts)
                 # Setting the main parameters of the PV plant
                 location = Location(latitude=self.lat, longitude=self.lon)
                 temp_params = TEMPERATURE_MODEL_PARAMETERS['sapm']['close_mount_glass_glass']
-                cec_modules = bz2.BZ2File(get_root(__file__, num_parent=2) / 'emhass/data/cec_modules.pbz2', "rb")
+                cec_modules = bz2.BZ2File(self.emhass_conf['root_path'] / 'src/emhass/data/cec_modules.pbz2', "rb")
                 cec_modules = cPickle.load(cec_modules)
-                cec_inverters = bz2.BZ2File(get_root(__file__, num_parent=2) / 'emhass/data/cec_inverters.pbz2', "rb")
+                cec_inverters = bz2.BZ2File(self.emhass_conf['root_path'] / 'src/emhass/data/cec_inverters.pbz2', "rb")
                 cec_inverters = cPickle.load(cec_inverters)
                 if type(self.plant_conf['module_model']) == list:
                     P_PV_forecast = pd.Series(0, index=df_weather.index)
                     for i in range(len(self.plant_conf['module_model'])):
                         # Selecting correct module and inverter
                         module = cec_modules[self.plant_conf['module_model'][i]]
                         inverter = cec_inverters[self.plant_conf['inverter_model'][i]]
@@ -514,15 +517,17 @@
             df_csv.drop(['ts'], axis=1, inplace=True)
             df_csv = set_df_index_freq(df_csv)
             if list_and_perfect:
                 days_list = df_final.index.day.unique().tolist()
             else:
                 days_list = df_csv.index.day.unique().tolist()
         else:
-            load_csv_file_path = self.root + csv_path
+            if not os.path.exists(csv_path):
+                csv_path = self.emhass_conf['data_path'] / csv_path
+            load_csv_file_path = csv_path    
             df_csv = pd.read_csv(load_csv_file_path, header=None, names=['ts', 'yhat'])
             df_csv.index = forecast_dates_csv
             df_csv.drop(['ts'], axis=1, inplace=True)
             df_csv = set_df_index_freq(df_csv)
             days_list = df_final.index.day.unique().tolist()
         forecast_out = pd.DataFrame()
         for day in days_list:
@@ -568,15 +573,15 @@
                     forecast_tp = pd.DataFrame(
                         df_csv.between_time(first_hour, last_hour).values,
                         index=fcst_index)
                 forecast_out = pd.concat([forecast_out, forecast_tp], axis=0)
         return forecast_out
     
     def get_load_forecast(self, days_min_load_forecast: Optional[int] = 3, method: Optional[str] = 'naive',
-                          csv_path: Optional[str] = "/data/data_load_forecast.csv",
+                          csv_path: Optional[str] = "data_load_forecast.csv",
                           set_mix_forecast:Optional[bool] = False, df_now:Optional[pd.DataFrame] = pd.DataFrame(),
                           use_last_window: Optional[bool] = True, mlf: Optional[MLForecaster] = None,
                           debug: Optional[bool] = False) -> pd.Series:
         r"""
         Get and generate the load forecast data.
         
         :param days_min_load_forecast: The number of last days to retrieve that \
@@ -606,26 +611,34 @@
         :type mlf: mlforecaster, optional
         :param debug: The DataFrame containing the now/current data.
         :type debug: Bool, optional
         :return: The DataFrame containing the electrical load power in Watts
         :rtype: pd.DataFrame
 
         """
+        csv_path  = self.emhass_conf['data_path'] / csv_path
+        
         if method == 'naive' or method == 'mlforecaster': # retrieving needed data for these methods
             self.logger.info("Retrieving data from hass for load forecast using method = "+method)
             var_list = [self.var_load]
             var_replace_zero = None
             var_interp = [self.var_load]
             time_zone_load_foreacast = None
             # We will need to retrieve a new set of load data according to the days_min_load_forecast parameter
             rh = RetrieveHass(self.retrieve_hass_conf['hass_url'], self.retrieve_hass_conf['long_lived_token'], 
-                               self.freq, time_zone_load_foreacast, self.params, self.root, self.logger)
+                               self.freq, time_zone_load_foreacast, self.params, self.emhass_conf, self.logger)
             if self.get_data_from_file:
-                with open(pathlib.Path(self.root) / 'data' / 'test_df_final.pkl', 'rb') as inp:
-                    rh.df_final, days_list, _ = pickle.load(inp)
+                filename_path = self.emhass_conf['data_path'] / 'test_df_final.pkl'
+                with open(filename_path, 'rb') as inp:
+                    rh.df_final, days_list, var_list = pickle.load(inp)
+                    self.var_load = var_list[0]
+                    self.retrieve_hass_conf['var_load'] = self.var_load
+                    var_interp = [var_list[0]]
+                    self.var_list = [var_list[0]]
+                    self.var_load_new = self.var_load+'_positive'
             else:
                 days_list = get_days_list(days_min_load_forecast) 
                 if not rh.get_data(days_list, var_list):
                     return False
             if  not rh.prepare_data(self.retrieve_hass_conf['var_load'], load_negative = self.retrieve_hass_conf['load_negative'],
                             set_zero_min = self.retrieve_hass_conf['set_zero_min'], 
                             var_replace_zero = var_replace_zero, 
@@ -639,38 +652,46 @@
             # Force forecast_out length to avoid mismatches
             forecast_out = forecast_out.iloc[0:len(self.forecast_dates)]
             forecast_out.index = self.forecast_dates
         elif method == 'mlforecaster': # using a custom forecast model with machine learning
             # Load model
             model_type = self.params['passed_data']['model_type']
             filename = model_type+'_mlf.pkl'
-            filename_path = pathlib.Path(self.root) / filename
+            filename_path = self.emhass_conf['data_path'] / filename
             if not debug:
                 if filename_path.is_file():
                     with open(filename_path, 'rb') as inp:
                         mlf = pickle.load(inp)
                 else:
                     self.logger.error("The ML forecaster file was not found, please run a model fit method before this predict method")
+                    return False
             # Make predictions
             if use_last_window:
                 data_last_window = copy.deepcopy(df)
                 data_last_window = data_last_window.rename(columns={self.var_load_new: self.var_load})
             else:
                 data_last_window = None
             forecast_out = mlf.predict(data_last_window)
-            # Force forecast_out length to avoid mismatches
-            forecast_out = forecast_out.iloc[0:len(self.forecast_dates)]
+            # Force forecast length to avoid mismatches
+            self.logger.debug("Number of ML predict forcast data generated (lags_opt): " + str(len(forecast_out.index)))
+            self.logger.debug("Number of forcast dates obtained: " + str(len(self.forecast_dates)))
+            if len(self.forecast_dates) < len(forecast_out.index):
+                forecast_out = forecast_out.iloc[0:len(self.forecast_dates)]
+            # To be removed once bug is fixed
+            elif len(self.forecast_dates) > len(forecast_out.index):
+                self.logger.error("Unable to obtain: " + str(len(self.forecast_dates))  + " lags_opt values from sensor: power load no var loads, check optimization_time_step/freq and historic_days_to_retrieve/days_to_retrieve parameters")
+                return False
             # Define DataFrame
             data_dict = {'ts':self.forecast_dates, 'yhat':forecast_out.values.tolist()}
             data = pd.DataFrame.from_dict(data_dict)
             # Define index
             data.set_index('ts', inplace=True)
             forecast_out = data.copy().loc[self.forecast_dates]
         elif method == 'csv': # reading from a csv file
-            load_csv_file_path = self.root + csv_path
+            load_csv_file_path = csv_path
             df_csv = pd.read_csv(load_csv_file_path, header=None, names=['ts', 'yhat'])
             if len(df_csv) < len(self.forecast_dates):
                 self.logger.error("Passed data from CSV is not long enough")
             else:
                 # Ensure correct length
                 df_csv = df_csv.loc[df_csv.index[0:len(self.forecast_dates)],:]
                 # Define index
@@ -679,25 +700,27 @@
                 forecast_out = df_csv.copy().loc[self.forecast_dates]
         elif method == 'list': # reading a list of values
             # Loading data from passed list
             data_list = self.params['passed_data']['load_power_forecast']
             # Check if the passed data has the correct length
             if len(data_list) < len(self.forecast_dates) and self.params['passed_data']['prediction_horizon'] is None:
                 self.logger.error("Passed data from passed list is not long enough")
+                return False
             else:
                 # Ensure correct length
                 data_list = data_list[0:len(self.forecast_dates)]
                 # Define DataFrame
                 data_dict = {'ts':self.forecast_dates, 'yhat':data_list}
                 data = pd.DataFrame.from_dict(data_dict)
                 # Define index
                 data.set_index('ts', inplace=True)
                 forecast_out = data.copy().loc[self.forecast_dates]
         else:
             self.logger.error("Passed method is not valid")
+            return False
         P_Load_forecast = copy.deepcopy(forecast_out['yhat'])
         if set_mix_forecast:
             P_Load_forecast = Forecast.get_mix_forecast(
                 df_now, P_Load_forecast, 
                 self.params['passed_data']['alpha'], self.params['passed_data']['beta'], self.var_load_new)
         return P_Load_forecast
     
@@ -719,14 +742,16 @@
             defaults to "data_load_cost_forecast.csv"
         :type csv_path: str, optional
         :return: The input DataFrame with one additionnal column appended containing
             the load cost for each time observation.
         :rtype: pd.DataFrame
 
         """
+        csv_path  = self.emhass_conf['data_path'] / csv_path
+
         if method == 'hp_hc_periods':
             df_final[self.var_load_cost] = self.optim_conf['load_cost_hc']
             list_df_hp = []
             for key, period_hp in self.optim_conf['list_hp_periods'].items():
                 list_df_hp.append(df_final[self.var_load_cost].between_time(
                     period_hp[0]['start'], period_hp[1]['end']))
             for df_hp in list_df_hp:
@@ -738,31 +763,34 @@
             df_final[self.var_load_cost] = forecast_out
         elif method == 'list': # reading a list of values
             # Loading data from passed list
             data_list = self.params['passed_data']['load_cost_forecast']
             # Check if the passed data has the correct length
             if len(data_list) < len(self.forecast_dates) and self.params['passed_data']['prediction_horizon'] is None:
                 self.logger.error("Passed data from passed list is not long enough")
+                return False
             else:
                 # Ensure correct length
                 data_list = data_list[0:len(self.forecast_dates)]
                 # Define the correct dates
                 forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
                 forecast_out = self.get_forecast_out_from_csv_or_list(
                     df_final, forecast_dates_csv, None, data_list=data_list, list_and_perfect=list_and_perfect)
                 # Fill the final DF
                 df_final[self.var_load_cost] = forecast_out
         else:
             self.logger.error("Passed method is not valid")
+            return False
             
         return df_final
     
     def get_prod_price_forecast(self, df_final: pd.DataFrame, method: Optional[str] = 'constant',
-                                csv_path: Optional[str] = "/data/data_prod_price_forecast.csv",
-                                list_and_perfect: Optional[bool] = False) -> pd.DataFrame:
+                               csv_path: Optional[str] = "data_prod_price_forecast.csv", 
+                               list_and_perfect: Optional[bool] = False) -> pd.DataFrame:
+
         r"""
         Get the unit power production price for the energy injected to the grid.\
         This is the price of the energy injected to the utility in a vector \
         sampled at the fixed freq value.
         
         :param df_input_data: The DataFrame containing all the input data retrieved
             from hass
@@ -775,35 +803,40 @@
             defaults to "/data/data_load_cost_forecast.csv"
         :type csv_path: str, optional
         :return: The input DataFrame with one additionnal column appended containing
             the power production price for each time observation.
         :rtype: pd.DataFrame
 
         """
+
+        csv_path  = self.emhass_conf['data_path'] / csv_path
+
         if method == 'constant':
             df_final[self.var_prod_price] = self.optim_conf['prod_sell_price']
         elif method == 'csv':
             forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
             forecast_out = self.get_forecast_out_from_csv_or_list(df_final,
                                                           forecast_dates_csv,
                                                           csv_path)
             df_final[self.var_prod_price] = forecast_out
         elif method == 'list': # reading a list of values
             # Loading data from passed list
             data_list = self.params['passed_data']['prod_price_forecast']
             # Check if the passed data has the correct length
             if len(data_list) < len(self.forecast_dates) and self.params['passed_data']['prediction_horizon'] is None:
                 self.logger.error("Passed data from passed list is not long enough")
+                return False
             else:
                 # Ensure correct length
                 data_list = data_list[0:len(self.forecast_dates)]
                 # Define the correct dates
                 forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
                 forecast_out = self.get_forecast_out_from_csv_or_list(
                     df_final, forecast_dates_csv, None, data_list=data_list, list_and_perfect=list_and_perfect)
                 # Fill the final DF
                 df_final[self.var_prod_price] = forecast_out
         else:
             self.logger.error("Passed method is not valid")
+            return False
             
         return df_final
```

### Comparing `emhass-0.8.6/src/emhass/machine_learning_forecaster.py` & `emhass-0.9.0/src/emhass/machine_learning_forecaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     - `predict`: to obtain a forecast from a pre-trained model.
     
     - `tune`: to optimize the models hyperparameters using bayesian optimization. 
     
     """
 
     def __init__(self, data: pd.DataFrame, model_type: str, var_model: str, sklearn_model: str,
-                 num_lags: int, root: str, logger: logging.Logger) -> None:
+                 num_lags: int, emhass_conf: dict, logger: logging.Logger) -> None:
         r"""Define constructor for the forecast class.
 
         :param data: The data that will be used for train/test
         :type data: pd.DataFrame
         :param model_type: A unique name defining this model and useful to identify \
             for what it will be used for.
         :type model_type: str
@@ -52,25 +52,25 @@
         :param sklearn_model: The `scikit-learn` model that will be used. For now only \
             this options are possible: `LinearRegression`, `ElasticNet` and `KNeighborsRegressor`.
         :type sklearn_model: str
         :param num_lags: The number of auto-regression lags to consider. A good starting point \
             is to fix this as one day. For example if your time step is 30 minutes, then fix this \
             to 48, if the time step is 1 hour the fix this to 24 and so on.
         :type num_lags: int
-        :param root: The parent folder of the path where the config.yaml file is located
-        :type root: str
+        :param emhass_conf: Dictionary containing the needed emhass paths
+        :type emhass_conf: dict
         :param logger: The passed logger object
         :type logger: logging.Logger
         """
         self.data = data
         self.model_type = model_type
         self.var_model = var_model
         self.sklearn_model = sklearn_model
         self.num_lags = num_lags
-        self.root = root
+        self.emhass_conf = emhass_conf
         self.logger = logger
         self.is_tuned = False
         # A quick data preparation
         self.data.index = pd.to_datetime(self.data.index)
         self.data.sort_index(inplace=True)
         self.data = self.data[~self.data.index.duplicated(keep='first')]
```

### Comparing `emhass-0.8.6/src/emhass/optimization.py` & `emhass-0.9.0/src/emhass/optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     
     - perform_naive_mpc_optim
     
     """
 
     def __init__(self, retrieve_hass_conf: dict, optim_conf: dict, plant_conf: dict, 
                  var_load_cost: str, var_prod_price: str, 
-                 costfun: str, base_path: str, logger: logging.Logger, 
+                 costfun: str, emhass_conf: dict, logger: logging.Logger, 
                  opt_time_delta: Optional[int] = 24) -> None:
         r"""
         Define constructor for Optimization class.
         
         :param retrieve_hass_conf: Configuration parameters used to retrieve data \
             from hass
         :type retrieve_hass_conf: dict
@@ -46,16 +46,16 @@
         :type plant_conf: dict
         :param var_load_cost: The column name for the unit load cost.
         :type var_load_cost: str
         :param var_prod_price: The column name for the unit power production price.
         :type var_prod_price: str
         :param costfun: The type of cost function to use for optimization problem
         :type costfun: str
-        :param base_path: The path to the yaml configuration file
-        :type base_path: str
+        :param emhass_conf: Dictionary containing the needed emhass paths
+        :type emhass_conf: dict
         :param logger: The passed logger object
         :type logger: logging object
         :param opt_time_delta: The number of hours to optimize. If days_list has \
             more than one day then the optimization will be peformed by chunks of \
             opt_time_delta periods, defaults to 24
         :type opt_time_delta: float, optional
         
@@ -67,14 +67,15 @@
         self.time_zone = self.retrieve_hass_conf['time_zone']
         self.timeStep = self.freq.seconds/3600 # in hours
         self.time_delta = pd.to_timedelta(opt_time_delta, "hours") # The period of optimization
         self.var_PV = self.retrieve_hass_conf['var_PV']
         self.var_load = self.retrieve_hass_conf['var_load']
         self.var_load_new = self.var_load+'_positive'
         self.costfun = costfun
+        # self.emhass_conf = emhass_conf
         self.logger = logger
         self.var_load_cost = var_load_cost
         self.var_prod_price = var_prod_price
         self.optim_status = None
         if 'lp_solver' in optim_conf.keys():
             self.lp_solver = optim_conf['lp_solver']
         else:
```

### Comparing `emhass-0.8.6/src/emhass/retrieve_hass.py` & `emhass-0.9.0/src/emhass/retrieve_hass.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,51 +27,56 @@
     - prepare_data: to apply some data treatment in preparation for the optimization task
     
     - post_data: Post passed data to hass
     
     """
 
     def __init__(self, hass_url: str, long_lived_token: str, freq: pd.Timedelta, 
-                 time_zone: datetime.timezone, params: str, base_path: str, logger: logging.Logger,
+                 time_zone: datetime.timezone, params: str, emhass_conf: dict, logger: logging.Logger,
                  get_data_from_file: Optional[bool] = False) -> None:
         """
         Define constructor for RetrieveHass class.
-        
+
         :param hass_url: The URL of the Home Assistant instance
         :type hass_url: str
         :param long_lived_token: The long lived token retrieved from the configuration pane
         :type long_lived_token: str
         :param freq: The frequency of the data DateTimeIndexes
         :type freq: pd.TimeDelta
         :param time_zone: The time zone
         :type time_zone: datetime.timezone
         :param params: Configuration parameters passed from data/options.json
         :type params: str
-        :param base_path: The path to the yaml configuration file
-        :type base_path: str
+        :param emhass_conf: Dictionary containing the needed emhass paths
+        :type emhass_conf: dict
         :param logger: The passed logger object
         :type logger: logging object
-        :param get_data_from_file: Select if data should be retrieved from a 
+        :param get_data_from_file: Select if data should be retrieved from a
         previously saved pickle useful for testing or directly from connection to
         hass database
         :type get_data_from_file: bool, optional
 
         """
         self.hass_url = hass_url
         self.long_lived_token = long_lived_token
         self.freq = freq
         self.time_zone = time_zone
         self.params = params
-        self.base_path = base_path
+        # self.emhass_conf = emhass_conf
         self.logger = logger
         self.get_data_from_file = get_data_from_file
 
-    def get_data(self, days_list: pd.date_range, var_list: list, minimal_response: Optional[bool] = False,
-                 significant_changes_only: Optional[bool] = False, 
-                 test_url: Optional[str] = 'empty') -> None:
+    def get_data(
+        self,
+        days_list: pd.date_range,
+        var_list: list,
+        minimal_response: Optional[bool] = False,
+        significant_changes_only: Optional[bool] = False,
+        test_url: Optional[str] = "empty",
+    ) -> None:
         r"""
         Retrieve the actual data from hass.
         
         :param days_list: A list of days to retrieve. The ISO format should be used \
             and the timezone is UTC. The frequency of the data_range should be freq='D'
         :type days_list: pandas.date_range
         :param var_list: The list of variables to retrive from hass. These should \
@@ -88,88 +93,127 @@
         :rtype: pandas.DataFrame
         
         .. warning:: The minimal_response and significant_changes_only options \
             are experimental
         """
         self.logger.info("Retrieve hass get data method initiated...")
         self.df_final = pd.DataFrame()
-        x = 0 #iterate based on days
+        x = 0  # iterate based on days
         # Looping on each day from days list
         for day in days_list:
-        
+
             for i, var in enumerate(var_list):
-                
-                if test_url == 'empty':
-                    if self.hass_url == "http://supervisor/core/api": # If we are using the supervisor API
-                        url = self.hass_url+"/history/period/"+day.isoformat()+"?filter_entity_id="+var
-                    else: # Otherwise the Home Assistant Core API it is
-                        url = self.hass_url+"api/history/period/"+day.isoformat()+"?filter_entity_id="+var
-                    if minimal_response: # A support for minimal response
+
+                if test_url == "empty":
+                    if (
+                        self.hass_url == "http://supervisor/core/api"
+                    ):  # If we are using the supervisor API
+                        url = (
+                            self.hass_url
+                            + "/history/period/"
+                            + day.isoformat()
+                            + "?filter_entity_id="
+                            + var
+                        )
+                    else:  # Otherwise the Home Assistant Core API it is
+                        url = (
+                            self.hass_url
+                            + "api/history/period/"
+                            + day.isoformat()
+                            + "?filter_entity_id="
+                            + var
+                        )
+                    if minimal_response:  # A support for minimal response
                         url = url + "?minimal_response"
-                    if significant_changes_only: # And for signicant changes only (check the HASS restful API for more info)
+                    if (
+                        significant_changes_only
+                    ):  # And for signicant changes only (check the HASS restful API for more info)
                         url = url + "?significant_changes_only"
                 else:
                     url = test_url
                 headers = {
                     "Authorization": "Bearer " + self.long_lived_token,
                     "content-type": "application/json",
                 }
                 try:
                     response = get(url, headers=headers)
                 except Exception:
-                    self.logger.error("Unable to access Home Assistance instance, check URL")
-                    self.logger.error("If using addon, try setting url and token to 'empty'")
+                    self.logger.error(
+                        "Unable to access Home Assistance instance, check URL"
+                    )
+                    self.logger.error(
+                        "If using addon, try setting url and token to 'empty'"
+                    )
                     return False
                 else:
                     if response.status_code == 401:
-                        self.logger.error("Unable to access Home Assistance instance, TOKEN/KEY")
-                        self.logger.error("If using addon, try setting url and token to 'empty'")
+                        self.logger.error(
+                            "Unable to access Home Assistance instance, TOKEN/KEY"
+                        )
+                        self.logger.error(
+                            "If using addon, try setting url and token to 'empty'"
+                        )
                         return False
                     if response.status_code > 299:
                         return f"Request Get Error: {response.status_code}"
-                '''import bz2 # Uncomment to save a serialized data for tests
+                """import bz2 # Uncomment to save a serialized data for tests
                 import _pickle as cPickle
                 with bz2.BZ2File("data/test_response_get_data_get_method.pbz2", "w") as f: 
-                    cPickle.dump(response, f)'''
-                try: # Sometimes when there are connection problems we need to catch empty retrieved json
+                    cPickle.dump(response, f)"""
+                try:  # Sometimes when there are connection problems we need to catch empty retrieved json
                     data = response.json()[0]
                 except IndexError:
                     if x == 0:
-                        self.logger.error("The retrieved JSON is empty, A sensor:" + var + " may have 0 days of history or passed sensor may not be correct")
+                        self.logger.error("The retrieved JSON is empty, A sensor:" + var + " may have 0 days of history, passed sensor may not be correct, or days to retrieve is set too heigh")
                     else:
                         self.logger.error("The retrieved JSON is empty for day:"+ str(day) +", days_to_retrieve may be larger than the recorded history of sensor:" + var + " (check your recorder settings)")
                     return False
                 df_raw = pd.DataFrame.from_dict(data)
+                # self.logger.info(str(df_raw))
                 if len(df_raw) == 0:
                     if x == 0:
-                        self.logger.error("The retrieved Dataframe is empty, A sensor:" + var + " may have 0 days of history or passed sensor may not be correct")
+                        self.logger.error(
+                            "The retrieved Dataframe is empty, A sensor:"
+                            + var
+                            + " may have 0 days of history or passed sensor may not be correct"
+                        )
                     else:
                         self.logger.error("Retrieved empty Dataframe for day:"+ str(day) +", days_to_retrieve may be larger than the recorded history of sensor:" + var + " (check your recorder settings)")
                     return False
+                # self.logger.info(self.freq.seconds)
+                if len(df_raw) < ((60 / (self.freq.seconds / 60)) * 24) and x != len(days_list) -1: #check if there is enough Dataframes for passed frequency per day (not inc current day)
+                    self.logger.debug("sensor:"  + var + " retrieved Dataframe count: " + str(len(df_raw))  + ", on day: " + str(day) + ". This is less than freq value passed: " + str(self.freq))
                 if i == 0: # Defining the DataFrame container
                     from_date = pd.to_datetime(df_raw['last_changed'], format="ISO8601").min()
                     to_date = pd.to_datetime(df_raw['last_changed'], format="ISO8601").max()
                     ts = pd.to_datetime(pd.date_range(start=from_date, end=to_date, freq=self.freq), 
                                         format='%Y-%d-%m %H:%M').round(self.freq, ambiguous='infer', nonexistent='shift_forward')
                     df_day = pd.DataFrame(index = ts)
                 # Caution with undefined string data: unknown, unavailable, etc.
-                df_tp = df_raw.copy()[['state']].replace(
-                    ['unknown', 'unavailable', ''], np.nan).astype(float).rename(columns={'state': var})
+                df_tp = (
+                    df_raw.copy()[["state"]]
+                    .replace(["unknown", "unavailable", ""], np.nan)
+                    .astype(float)
+                    .rename(columns={"state": var})
+                )
                 # Setting index, resampling and concatenation
-                df_tp.set_index(pd.to_datetime(df_raw['last_changed'], format="ISO8601"), inplace=True)
+                df_tp.set_index(
+                    pd.to_datetime(df_raw["last_changed"], format="ISO8601"),
+                    inplace=True,
+                )
                 df_tp = df_tp.resample(self.freq).mean()
                 df_day = pd.concat([df_day, df_tp], axis=1)
-            
-            x += 1
             self.df_final = pd.concat([self.df_final, df_day], axis=0)
+            x += 1 
         self.df_final = set_df_index_freq(self.df_final)
         if self.df_final.index.freq != self.freq:
-            self.logger.error("The inferred freq from data is not equal to the defined freq in passed parameters")
+            self.logger.error("The inferred freq:" + str(self.df_final.index.freq) + " from data is not equal to the defined freq in passed:" + str(self.freq))
             return False
         return True
+           
     
     def prepare_data(self, var_load: str, load_negative: Optional[bool] = False, set_zero_min: Optional[bool] = True,
                      var_replace_zero: Optional[list] = None, var_interp: Optional[list] = None) -> None:
         r"""
         Apply some data treatment in preparation for the optimization task.
         
         :param var_load: The name of the variable for the household load consumption.
@@ -188,86 +232,107 @@
         :type var_interp: list, optional
         :return: The DataFrame populated with the retrieved data from hass and \
             after the data treatment
         :rtype: pandas.DataFrame
         
         """
         try:
-            if load_negative: # Apply the correct sign to load power
-                self.df_final[var_load+'_positive'] = -self.df_final[var_load]
+            if load_negative:  # Apply the correct sign to load power
+                self.df_final[var_load + "_positive"] = -self.df_final[var_load]
             else:
-                self.df_final[var_load+'_positive'] = self.df_final[var_load]
+                self.df_final[var_load + "_positive"] = self.df_final[var_load]
             self.df_final.drop([var_load], inplace=True, axis=1)
         except KeyError:
-            self.logger.error("Variable "+var_load+" was not found. This is typically because no data could be retrieved from Home Assistant")
+            self.logger.error(
+                "Variable "
+                + var_load
+                + " was not found. This is typically because no data could be retrieved from Home Assistant"
+            )
             return False
         except ValueError:
-            self.logger.error("sensor.power_photovoltaics and sensor.power_load_no_var_loads should not be the same")
-            return False   
-        if set_zero_min: # Apply minimum values
+            self.logger.error(
+                "sensor.power_photovoltaics and sensor.power_load_no_var_loads should not be the same"
+            )
+            return False
+        if set_zero_min:  # Apply minimum values
             self.df_final.clip(lower=0.0, inplace=True, axis=1)
             self.df_final.replace(to_replace=0.0, value=np.nan, inplace=True)
         new_var_replace_zero = []
         new_var_interp = []
         # Just changing the names of variables to contain the fact that they are considered positive
         if var_replace_zero is not None:
             for string in var_replace_zero:
-                new_string = string.replace(var_load, var_load+'_positive')
+                new_string = string.replace(var_load, var_load + "_positive")
                 new_var_replace_zero.append(new_string)
         else:
             new_var_replace_zero = None
         if var_interp is not None:
             for string in var_interp:
-                new_string = string.replace(var_load, var_load+'_positive')
+                new_string = string.replace(var_load, var_load + "_positive")
                 new_var_interp.append(new_string)
         else:
             new_var_interp = None
         # Treating NaN replacement: either by zeros or by linear interpolation
         if new_var_replace_zero is not None:
-            self.df_final[new_var_replace_zero] = self.df_final[new_var_replace_zero].fillna(0.0)
+            self.df_final[new_var_replace_zero] = self.df_final[
+                new_var_replace_zero
+            ].fillna(0.0)
         if new_var_interp is not None:
             self.df_final[new_var_interp] = self.df_final[new_var_interp].interpolate(
-                method='linear', axis=0, limit=None)
+                method="linear", axis=0, limit=None
+            )
             self.df_final[new_var_interp] = self.df_final[new_var_interp].fillna(0.0)
         # Setting the correct time zone on DF index
         if self.time_zone is not None:
             self.df_final.index = self.df_final.index.tz_convert(self.time_zone)
         # Drop datetimeindex duplicates on final DF
-        self.df_final = self.df_final[~self.df_final.index.duplicated(keep='first')]
+        self.df_final = self.df_final[~self.df_final.index.duplicated(keep="first")]
         return True
-    
+
     @staticmethod
-    def get_attr_data_dict(data_df: pd.DataFrame, idx: int, entity_id: str, 
-                           unit_of_measurement: str, friendly_name: str, 
-                           list_name: str, state: float) -> dict:
-        list_df = copy.deepcopy(data_df).loc[data_df.index[idx]:].reset_index()
-        list_df.columns = ['timestamps', entity_id]
-        ts_list = [str(i) for i in list_df['timestamps'].tolist()]
-        vals_list = [str(np.round(i,2)) for i in list_df[entity_id].tolist()]
+    def get_attr_data_dict(
+        data_df: pd.DataFrame,
+        idx: int,
+        entity_id: str,
+        unit_of_measurement: str,
+        friendly_name: str,
+        list_name: str,
+        state: float,
+    ) -> dict:
+        list_df = copy.deepcopy(data_df).loc[data_df.index[idx] :].reset_index()
+        list_df.columns = ["timestamps", entity_id]
+        ts_list = [str(i) for i in list_df["timestamps"].tolist()]
+        vals_list = [str(np.round(i, 2)) for i in list_df[entity_id].tolist()]
         forecast_list = []
         for i, ts in enumerate(ts_list):
             datum = {}
             datum["date"] = ts
-            datum[entity_id.split('sensor.')[1]] = vals_list[i]
+            datum[entity_id.split("sensor.")[1]] = vals_list[i]
             forecast_list.append(datum)
         data = {
             "state": "{:.2f}".format(state),
             "attributes": {
                 "unit_of_measurement": unit_of_measurement,
                 "friendly_name": friendly_name,
-                list_name: forecast_list
-            }
+                list_name: forecast_list,
+            },
         }
         return data
-    
-    def post_data(self, data_df: pd.DataFrame, idx: int, entity_id: str, 
-                  unit_of_measurement: str, friendly_name: str,
-                  type_var: str,
-                  from_mlforecaster: Optional[bool]=False,
-                  publish_prefix: Optional[str]="") -> None:
+
+    def post_data(
+        self,
+        data_df: pd.DataFrame,
+        idx: int,
+        entity_id: str,
+        unit_of_measurement: str,
+        friendly_name: str,
+        type_var: str,
+        from_mlforecaster: Optional[bool] = False,
+        publish_prefix: Optional[str] = "",
+    ) -> None:
         r"""
         Post passed data to hass.
         
         :param data_df: The DataFrame containing the data that will be posted \
             to hass. This should be a one columns DF or a series.
         :type data_df: pd.DataFrame
         :param idx: The int index of the location of the data within the passed \
@@ -282,76 +347,143 @@
         :param type_var: A variable to indicate the type of variable: power, SOC, etc.
         :type type_var: str
         :param publish_prefix: A common prefix for all published data entity_id.
         :type publish_prefix: str, optional
 
         """
         # Add a possible prefix to the entity ID
-        entity_id = entity_id.replace('sensor.', 'sensor.'+publish_prefix)
+        entity_id = entity_id.replace("sensor.", "sensor." + publish_prefix)
         # Set the URL
-        if self.hass_url == "http://supervisor/core/api": # If we are using the supervisor API
-            url = self.hass_url+"/states/"+entity_id
-        else: # Otherwise the Home Assistant Core API it is
-            url = self.hass_url+"api/states/"+entity_id
+        if (
+            self.hass_url == "http://supervisor/core/api"
+        ):  # If we are using the supervisor API
+            url = self.hass_url + "/states/" + entity_id
+        else:  # Otherwise the Home Assistant Core API it is
+            url = self.hass_url + "api/states/" + entity_id
         headers = {
             "Authorization": "Bearer " + self.long_lived_token,
             "content-type": "application/json",
         }
         # Preparing the data dict to be published
-        if type_var == 'cost_fun':
-            state = np.round(data_df.sum()[0],2)
-        elif type_var == 'unit_load_cost' or type_var == 'unit_prod_price':
-            state = np.round(data_df.loc[data_df.index[idx]],4)
-        elif type_var == 'optim_status':
+        if type_var == "cost_fun":
+            state = np.round(data_df.sum()[0], 2)
+        elif type_var == "unit_load_cost" or type_var == "unit_prod_price":
+            state = np.round(data_df.loc[data_df.index[idx]], 4)
+        elif type_var == "optim_status":
             state = data_df.loc[data_df.index[idx]]
+        elif type_var == "mlregressor":
+            state = data_df[idx]
         else:
-            state = np.round(data_df.loc[data_df.index[idx]],2)
-        if type_var == 'power':
-            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
-                                                    friendly_name, "forecasts", state)
-        elif type_var == 'deferrable':
-            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
-                                                    friendly_name, "deferrables_schedule", state)
-        elif type_var == 'batt':
-            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
-                                                    friendly_name, "battery_scheduled_power", state)
-        elif type_var == 'SOC':
-            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
-                                                    friendly_name, "battery_scheduled_soc", state)
-        elif type_var == 'unit_load_cost':
-            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
-                                                    friendly_name, "unit_load_cost_forecasts", state)
-        elif type_var == 'unit_prod_price':
-            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
-                                                    friendly_name, "unit_prod_price_forecasts", state)
-        elif type_var == 'mlforecaster':
-            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
-                                                    friendly_name, "scheduled_forecast", state)
-        elif type_var == 'optim_status':
+            state = np.round(data_df.loc[data_df.index[idx]], 2)
+        if type_var == "power":
+            data = RetrieveHass.get_attr_data_dict(
+                data_df,
+                idx,
+                entity_id,
+                unit_of_measurement,
+                friendly_name,
+                "forecasts",
+                state,
+            )
+        elif type_var == "deferrable":
+            data = RetrieveHass.get_attr_data_dict(
+                data_df,
+                idx,
+                entity_id,
+                unit_of_measurement,
+                friendly_name,
+                "deferrables_schedule",
+                state,
+            )
+        elif type_var == "batt":
+            data = RetrieveHass.get_attr_data_dict(
+                data_df,
+                idx,
+                entity_id,
+                unit_of_measurement,
+                friendly_name,
+                "battery_scheduled_power",
+                state,
+            )
+        elif type_var == "SOC":
+            data = RetrieveHass.get_attr_data_dict(
+                data_df,
+                idx,
+                entity_id,
+                unit_of_measurement,
+                friendly_name,
+                "battery_scheduled_soc",
+                state,
+            )
+        elif type_var == "unit_load_cost":
+            data = RetrieveHass.get_attr_data_dict(
+                data_df,
+                idx,
+                entity_id,
+                unit_of_measurement,
+                friendly_name,
+                "unit_load_cost_forecasts",
+                state,
+            )
+        elif type_var == "unit_prod_price":
+            data = RetrieveHass.get_attr_data_dict(
+                data_df,
+                idx,
+                entity_id,
+                unit_of_measurement,
+                friendly_name,
+                "unit_prod_price_forecasts",
+                state,
+            )
+        elif type_var == "mlforecaster":
+            data = RetrieveHass.get_attr_data_dict(
+                data_df,
+                idx,
+                entity_id,
+                unit_of_measurement,
+                friendly_name,
+                "scheduled_forecast",
+                state,
+            )
+        elif type_var == "optim_status":
             data = {
                 "state": state,
                 "attributes": {
                     "unit_of_measurement": unit_of_measurement,
-                    "friendly_name": friendly_name
-                }
+                    "friendly_name": friendly_name,
+                },
+            }
+        elif type_var == "mlregressor":
+            data = {
+                "state": state,
+                "attributes": {
+                    "unit_of_measurement": unit_of_measurement,
+                    "friendly_name": friendly_name,
+                },
             }
         else:
             data = {
                 "state": "{:.2f}".format(state),
                 "attributes": {
                     "unit_of_measurement": unit_of_measurement,
-                    "friendly_name": friendly_name
-                }
+                    "friendly_name": friendly_name,
+                },
             }
         # Actually post the data
         if self.get_data_from_file:
-            class response: pass
+
+            class response:
+                pass
+
             response.status_code = 200
             response.ok = True
         else:
             response = post(url, headers=headers, data=json.dumps(data))
         # Treating the response status and posting them on the logger
         if response.ok:
-            self.logger.info("Successfully posted to "+entity_id+" = "+str(state))
+            self.logger.info("Successfully posted to " + entity_id + " = " + str(state))
         else:
-            self.logger.info("The status code for received curl command response is: "+str(response.status_code))
+            self.logger.info(
+                "The status code for received curl command response is: "
+                + str(response.status_code)
+            )
         return response, data
```

### Comparing `emhass-0.8.6/src/emhass/static/advanced.html` & `emhass-0.9.0/src/emhass/static/advanced.html`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 <h4>Use the button below to publish the optimized variables at the current timestamp</h4>
 <button type="button" id="publish-data" class="button button1">Publish Optimization Results</button>
 <h4>Use the buttons below to fit, predict and tune a machine learning model for testing</h4>
 <button type="button" id="forecast-model-fit" class="button button1">ML forecast model fit</button>
 <button type="button" id="forecast-model-predict" class="button button2">ML forecast model
     predict</button>
 <button type="button" id="forecast-model-tune" class="button button3">ML forecast model tune</button>
+</br></br>
+<button type="button" id="regressor-model-fit" class="button button1">ML regressor model fit</button>
+<button type="button" id="regressor-model-predict" class="button button2">ML regressor model predict</button>
 <!-- -->
 <!--dynamic input elements section -->
 <h4>Input Runtime Parameters</h4>
 <div class="input-button-container">
     <div class="input-buttons">
         <button type="button" id="input-plus">+</button>
         <button type="button" id="input-minus">-</button>
```

### Comparing `emhass-0.8.6/src/emhass/static/basic.html` & `emhass-0.9.0/src/emhass/static/basic.html`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/static/img/emhass_icon.png` & `emhass-0.9.0/src/emhass/static/img/emhass_icon.png`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/static/img/emhass_logo_short.svg` & `emhass-0.9.0/src/emhass/static/img/emhass_logo_short.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/static/img/feather-sprite.svg` & `emhass-0.9.0/src/emhass/static/img/feather-sprite.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/static/script.js` & `emhass-0.9.0/src/emhass/static/script.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -12,14 +12,16 @@
     switch (page) {
         case "advanced":
             [
                 "dayahead-optim",
                 "forecast-model-fit",
                 "forecast-model-predict",
                 "forecast-model-tune",
+                "regressor-model-fit",
+                "regressor-model-predict",
                 "perfect-optim",
                 "publish-data",
                 "naive-mpc-optim"
             ].forEach((id) =>
                 document.getElementById(id).addEventListener("click", () => formAction(id, "advanced"))
             );
             ["input-plus", "input-minus"].forEach((id) =>
```

### Comparing `emhass-0.8.6/src/emhass/static/style.css` & `emhass-0.9.0/src/emhass/static/style.css`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/templates/index.html` & `emhass-0.9.0/src/emhass/templates/index.html`

 * *Files identical despite different names*

### Comparing `emhass-0.8.6/src/emhass/utils.py` & `emhass-0.9.0/src/emhass/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from typing import Tuple, Optional
-import numpy as np, pandas as pd
-import yaml, pytz, logging, pathlib, json, copy
 from datetime import datetime, timedelta, timezone
+import logging
+import pathlib
+import json
+import copy
+import numpy as np
+import pandas as pd
+import yaml
+import pytz
+
+
 import plotly.express as px
+
 pd.options.plotting.backend = "plotly"
 
 from emhass.machine_learning_forecaster import MLForecaster
 
 
 def get_root(file: str, num_parent: Optional[int] = 3) -> str:
     """
     Get the root absolute path of the working directory.
-    
+
     :param file: The passed file path with __file__
     :return: The root path
     :param num_parent: The number of parents levels up to desired root folder
     :type num_parent: int, optional
     :rtype: str
-    
+
     """
     if num_parent == 3:
         root = pathlib.Path(file).resolve().parent.parent.parent
     elif num_parent == 2:
         root = pathlib.Path(file).resolve().parent.parent
     elif num_parent == 1:
         root = pathlib.Path(file).resolve().parent
     else:
         raise ValueError("num_parent value not valid, must be between 1 and 3")
     return root
 
-def get_logger(fun_name: str, config_path: str, save_to_file: Optional[bool] = True,
+def get_logger(fun_name: str, emhass_conf: dict, save_to_file: Optional[bool] = True,
                logging_level: Optional[str] = "DEBUG") -> Tuple[logging.Logger, logging.StreamHandler]:
     """
     Create a simple logger object.
-    
+
     :param fun_name: The Python function object name where the logger will be used
     :type fun_name: str
-    :param config_path: The path to the yaml configuration file
-    :type config_path: str
+    :param emhass_conf: Dictionary containing the needed emhass paths
+    :type emhass_conf: dict
     :param save_to_file: Write log to a file, defaults to True
     :type save_to_file: bool, optional
     :return: The logger object and the handler
     :rtype: object
-    
+
     """
-	# create logger object
+    # create logger object
     logger = logging.getLogger(fun_name)
     logger.propagate = True
     logger.fileSetting = save_to_file
     if save_to_file:
-        ch = logging.FileHandler(config_path + '/data/logger_emhass.log')
+        ch = logging.FileHandler(emhass_conf['data_path'] / 'logger_emhass.log')
     else:
         ch = logging.StreamHandler()
     if logging_level == "DEBUG":
         logger.setLevel(logging.DEBUG)
         ch.setLevel(logging.DEBUG)
     elif logging_level == "INFO":
         logger.setLevel(logging.INFO)
@@ -66,48 +75,60 @@
         ch.setLevel(logging.WARNING)
     elif logging_level == "ERROR":
         logger.setLevel(logging.ERROR)
         ch.setLevel(logging.ERROR)
     else:
         logger.setLevel(logging.DEBUG)
         ch.setLevel(logging.DEBUG)
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+    formatter = logging.Formatter(
+        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    )
     ch.setFormatter(formatter)
     logger.addHandler(ch)
 
     return logger, ch
 
-def get_forecast_dates(freq: int, delta_forecast: int, 
-                       timedelta_days: Optional[int] = 0) -> pd.core.indexes.datetimes.DatetimeIndex:
+
+def get_forecast_dates(
+    freq: int, delta_forecast: int, timedelta_days: Optional[int] = 0
+) -> pd.core.indexes.datetimes.DatetimeIndex:
     """
     Get the date_range list of the needed future dates using the delta_forecast parameter.
 
     :param freq: Optimization time step.
     :type freq: int
     :param delta_forecast: Number of days to forecast in the future to be used for the optimization.
     :type delta_forecast: int
     :param timedelta_days: Number of truncated days needed for each optimization iteration, defaults to 0
     :type timedelta_days: Optional[int], optional
     :return: A list of future forecast dates.
     :rtype: pd.core.indexes.datetimes.DatetimeIndex
-    
+
     """
     freq = pd.to_timedelta(freq, "minutes")
     start_forecast = pd.Timestamp(datetime.now()).replace(hour=0, minute=0, second=0, microsecond=0)
     end_forecast = (start_forecast + pd.Timedelta(days=delta_forecast)).replace(microsecond=0)
     forecast_dates = pd.date_range(start=start_forecast, 
         end=end_forecast+timedelta(days=timedelta_days)-freq, 
         freq=freq).round(freq, ambiguous='infer', nonexistent='shift_forward')
     return forecast_dates
 
-def treat_runtimeparams(runtimeparams: str, params: str, retrieve_hass_conf: dict, optim_conf: dict, plant_conf: dict,
-                        set_type: str, logger: logging.Logger) -> Tuple[str, dict]:
+
+def treat_runtimeparams(
+    runtimeparams: str,
+    params: str,
+    retrieve_hass_conf: dict,
+    optim_conf: dict,
+    plant_conf: dict,
+    set_type: str,
+    logger: logging.Logger,
+) -> Tuple[str, dict]:
     """
-    Treat the passed optimization runtime parameters. 
-    
+    Treat the passed optimization runtime parameters.
+
     :param runtimeparams: Json string containing the runtime parameters dict.
     :type runtimeparams: str
     :param params: Configuration parameters passed from data/options.json
     :type params: str
     :param retrieve_hass_conf: Container for data retrieving parameters.
     :type retrieve_hass_conf: dict
     :param optim_conf: Container for optimization parameters.
@@ -116,101 +137,175 @@
     :type plant_conf: dict
     :param set_type: The type of action to be performed.
     :type set_type: str
     :param logger: The logger object.
     :type logger: logging.Logger
     :return: Returning the params and optimization parameter container.
     :rtype: Tuple[str, dict]
-    
+
     """
-    if (params != None) and (params != 'null'):
+    if (params != None) and (params != "null"):
         params = json.loads(params)
     else:
         params = {}
     # Some default data needed
     custom_deferrable_forecast_id = []
-    for k in range(optim_conf['num_def_loads']):
-        custom_deferrable_forecast_id.append({
-            "entity_id": "sensor.p_deferrable{}".format(k), 
-            "unit_of_measurement": "W", 
-            "friendly_name": "Deferrable Load {}".format(k)
-        })
-    default_passed_dict = {'custom_pv_forecast_id': {"entity_id": "sensor.p_pv_forecast", "unit_of_measurement": "W", "friendly_name": "PV Power Forecast"},
-                           'custom_load_forecast_id': {"entity_id": "sensor.p_load_forecast", "unit_of_measurement": "W", "friendly_name": "Load Power Forecast"},
-                           'custom_batt_forecast_id': {"entity_id": "sensor.p_batt_forecast", "unit_of_measurement": "W", "friendly_name": "Battery Power Forecast"},
-                           'custom_batt_soc_forecast_id': {"entity_id": "sensor.soc_batt_forecast", "unit_of_measurement": "%", "friendly_name": "Battery SOC Forecast"},
-                           'custom_grid_forecast_id': {"entity_id": "sensor.p_grid_forecast", "unit_of_measurement": "W", "friendly_name": "Grid Power Forecast"},
-                           'custom_cost_fun_id': {"entity_id": "sensor.total_cost_fun_value", "unit_of_measurement": "", "friendly_name": "Total cost function value"},
-                           'custom_optim_status_id': {"entity_id": "sensor.optim_status", "unit_of_measurement": "", "friendly_name": "EMHASS optimization status"},
-                           'custom_unit_load_cost_id': {"entity_id": "sensor.unit_load_cost", "unit_of_measurement": "€/kWh", "friendly_name": "Unit Load Cost"},
-                           'custom_unit_prod_price_id': {"entity_id": "sensor.unit_prod_price", "unit_of_measurement": "€/kWh", "friendly_name": "Unit Prod Price"},
-                           'custom_deferrable_forecast_id': custom_deferrable_forecast_id,
-                           'publish_prefix': ""}
-    if 'passed_data' in params.keys():
+    for k in range(optim_conf["num_def_loads"]):
+        custom_deferrable_forecast_id.append(
+            {
+                "entity_id": "sensor.p_deferrable{}".format(k),
+                "unit_of_measurement": "W",
+                "friendly_name": "Deferrable Load {}".format(k),
+            }
+        )
+    default_passed_dict = {
+        "custom_pv_forecast_id": {
+            "entity_id": "sensor.p_pv_forecast",
+            "unit_of_measurement": "W",
+            "friendly_name": "PV Power Forecast",
+        },
+        "custom_load_forecast_id": {
+            "entity_id": "sensor.p_load_forecast",
+            "unit_of_measurement": "W",
+            "friendly_name": "Load Power Forecast",
+        },
+        "custom_batt_forecast_id": {
+            "entity_id": "sensor.p_batt_forecast",
+            "unit_of_measurement": "W",
+            "friendly_name": "Battery Power Forecast",
+        },
+        "custom_batt_soc_forecast_id": {
+            "entity_id": "sensor.soc_batt_forecast",
+            "unit_of_measurement": "%",
+            "friendly_name": "Battery SOC Forecast",
+        },
+        "custom_grid_forecast_id": {
+            "entity_id": "sensor.p_grid_forecast",
+            "unit_of_measurement": "W",
+            "friendly_name": "Grid Power Forecast",
+        },
+        "custom_cost_fun_id": {
+            "entity_id": "sensor.total_cost_fun_value",
+            "unit_of_measurement": "",
+            "friendly_name": "Total cost function value",
+        },
+        "custom_optim_status_id": {
+            "entity_id": "sensor.optim_status",
+            "unit_of_measurement": "",
+            "friendly_name": "EMHASS optimization status",
+        },
+        "custom_unit_load_cost_id": {
+            "entity_id": "sensor.unit_load_cost",
+            "unit_of_measurement": "€/kWh",
+            "friendly_name": "Unit Load Cost",
+        },
+        "custom_unit_prod_price_id": {
+            "entity_id": "sensor.unit_prod_price",
+            "unit_of_measurement": "€/kWh",
+            "friendly_name": "Unit Prod Price",
+        },
+        "custom_deferrable_forecast_id": custom_deferrable_forecast_id,
+        "publish_prefix": "",
+    }
+    if "passed_data" in params.keys():
         for key, value in default_passed_dict.items():
-            params['passed_data'][key] = value
+            params["passed_data"][key] = value
     else:
-        params['passed_data'] = default_passed_dict
+        params["passed_data"] = default_passed_dict
     if runtimeparams is not None:
         runtimeparams = json.loads(runtimeparams)
-        freq = int(retrieve_hass_conf['freq'].seconds/60.0)
-        delta_forecast = int(optim_conf['delta_forecast'].days)
+        freq = int(retrieve_hass_conf["freq"].seconds / 60.0)
+        delta_forecast = int(optim_conf["delta_forecast"].days)
         forecast_dates = get_forecast_dates(freq, delta_forecast)
+        if set_type == "regressor-model-fit":            
+            if "csv_file" in runtimeparams:
+                csv_file = runtimeparams["csv_file"]
+                params["passed_data"]["csv_file"] = csv_file
+            if "features" in runtimeparams:
+                features = runtimeparams["features"]
+                params["passed_data"]["features"] = features
+            if "target" in runtimeparams:
+                target = runtimeparams["target"]
+                params["passed_data"]["target"] = target
+            if "timestamp" not in runtimeparams:
+                params["passed_data"]["timestamp"] = None
+            else:
+                timestamp = runtimeparams["timestamp"]
+                params["passed_data"]["timestamp"] = timestamp
+            if "date_features" not in runtimeparams:
+                params["passed_data"]["date_features"] = []
+            else:
+                date_features = runtimeparams["date_features"]
+                params["passed_data"]["date_features"] = date_features
+        if set_type == "regressor-model-predict":
+            if "new_values" in runtimeparams:
+                new_values = runtimeparams["new_values"]
+                params["passed_data"]["new_values"] = new_values
+            if "csv_file" in runtimeparams:
+                csv_file = runtimeparams["csv_file"]
+                params["passed_data"]["csv_file"] = csv_file
+            if "features" in runtimeparams:
+                features = runtimeparams["features"]
+                params["passed_data"]["features"] = features
+            if "target" in runtimeparams:
+                target = runtimeparams["target"]
+                params["passed_data"]["target"] = target
+
         # Treating special data passed for MPC control case
-        if set_type == 'naive-mpc-optim':
-            if 'prediction_horizon' not in runtimeparams.keys():
-                prediction_horizon = 10 # 10 time steps by default
-            else:
-                prediction_horizon = runtimeparams['prediction_horizon']
-            params['passed_data']['prediction_horizon'] = prediction_horizon
-            if 'soc_init' not in runtimeparams.keys():
-                soc_init = plant_conf['SOCtarget']
-            else:
-                soc_init = runtimeparams['soc_init']
-            params['passed_data']['soc_init'] = soc_init
-            if 'soc_final' not in runtimeparams.keys():
-                soc_final = plant_conf['SOCtarget']
-            else:
-                soc_final = runtimeparams['soc_final']
-            params['passed_data']['soc_final'] = soc_final
-            if 'def_total_hours' not in runtimeparams.keys():
-                def_total_hours = optim_conf['def_total_hours']
-            else:
-                def_total_hours = runtimeparams['def_total_hours']
-            params['passed_data']['def_total_hours'] = def_total_hours
-            if 'def_start_timestep' not in runtimeparams.keys():
-                def_start_timestep = optim_conf['def_start_timestep']
-            else:
-                def_start_timestep = runtimeparams['def_start_timestep']
-            params['passed_data']['def_start_timestep'] = def_start_timestep
-            if 'def_end_timestep' not in runtimeparams.keys():
-                def_end_timestep = optim_conf['def_end_timestep']
-            else:
-                def_end_timestep = runtimeparams['def_end_timestep']
-            params['passed_data']['def_end_timestep'] = def_end_timestep
-            if 'alpha' not in runtimeparams.keys():
+        if set_type == "naive-mpc-optim":
+            if "prediction_horizon" not in runtimeparams.keys():
+                prediction_horizon = 10  # 10 time steps by default
+            else:
+                prediction_horizon = runtimeparams["prediction_horizon"]
+            params["passed_data"]["prediction_horizon"] = prediction_horizon
+            if "soc_init" not in runtimeparams.keys():
+                soc_init = plant_conf["SOCtarget"]
+            else:
+                soc_init = runtimeparams["soc_init"]
+            params["passed_data"]["soc_init"] = soc_init
+            if "soc_final" not in runtimeparams.keys():
+                soc_final = plant_conf["SOCtarget"]
+            else:
+                soc_final = runtimeparams["soc_final"]
+            params["passed_data"]["soc_final"] = soc_final
+            if "def_total_hours" not in runtimeparams.keys():
+                def_total_hours = optim_conf["def_total_hours"]
+            else:
+                def_total_hours = runtimeparams["def_total_hours"]
+            params["passed_data"]["def_total_hours"] = def_total_hours
+            if "def_start_timestep" not in runtimeparams.keys():
+                def_start_timestep = optim_conf["def_start_timestep"]
+            else:
+                def_start_timestep = runtimeparams["def_start_timestep"]
+            params["passed_data"]["def_start_timestep"] = def_start_timestep
+            if "def_end_timestep" not in runtimeparams.keys():
+                def_end_timestep = optim_conf["def_end_timestep"]
+            else:
+                def_end_timestep = runtimeparams["def_end_timestep"]
+            params["passed_data"]["def_end_timestep"] = def_end_timestep
+            if "alpha" not in runtimeparams.keys():
                 alpha = 0.5
             else:
-                alpha = runtimeparams['alpha']
-            params['passed_data']['alpha'] = alpha
-            if 'beta' not in runtimeparams.keys():
+                alpha = runtimeparams["alpha"]
+            params["passed_data"]["alpha"] = alpha
+            if "beta" not in runtimeparams.keys():
                 beta = 0.5
             else:
-                beta = runtimeparams['beta']
-            params['passed_data']['beta'] = beta
+                beta = runtimeparams["beta"]
+            params["passed_data"]["beta"] = beta
             forecast_dates = copy.deepcopy(forecast_dates)[0:prediction_horizon]
         else:
-            params['passed_data']['prediction_horizon'] = None
-            params['passed_data']['soc_init'] = None
-            params['passed_data']['soc_final'] = None
-            params['passed_data']['def_total_hours'] = None
-            params['passed_data']['def_start_timestep'] = None
-            params['passed_data']['def_end_timestep'] = None
-            params['passed_data']['alpha'] = None
-            params['passed_data']['beta'] = None
+            params["passed_data"]["prediction_horizon"] = None
+            params["passed_data"]["soc_init"] = None
+            params["passed_data"]["soc_final"] = None
+            params["passed_data"]["def_total_hours"] = None
+            params["passed_data"]["def_start_timestep"] = None
+            params["passed_data"]["def_end_timestep"] = None
+            params["passed_data"]["alpha"] = None
+            params["passed_data"]["beta"] = None
         # Treat passed forecast data lists
         list_forecast_key = ['pv_power_forecast', 'load_power_forecast', 'load_cost_forecast', 'prod_price_forecast']
         forecast_methods = ['weather_forecast_method', 'load_forecast_method', 'load_cost_forecast_method', 'prod_price_forecast_method']
         for method, forecast_key in enumerate(list_forecast_key):
             if forecast_key in runtimeparams.keys():
                 if type(runtimeparams[forecast_key]) == list and len(runtimeparams[forecast_key]) >= len(forecast_dates):
                     params['passed_data'][forecast_key] = runtimeparams[forecast_key]
@@ -222,305 +317,419 @@
                 if len(list_non_digits) > 0:
                     logger.warning(f"There are non numeric values on the passed data for {forecast_key}, check for missing values (nans, null, etc)")
                     for x in list_non_digits:
                         logger.warning(f"This value in {forecast_key} was detected as non digits: {str(x)}")
             else:
                 params['passed_data'][forecast_key] = None
         # Treat passed data for forecast model fit/predict/tune at runtime
-        if 'days_to_retrieve' not in runtimeparams.keys():
+        if "days_to_retrieve" not in runtimeparams.keys():
             days_to_retrieve = 9
         else:
-            days_to_retrieve = runtimeparams['days_to_retrieve']
-        params['passed_data']['days_to_retrieve'] = days_to_retrieve
-        if 'model_type' not in runtimeparams.keys():
+            days_to_retrieve = runtimeparams["days_to_retrieve"]
+        params["passed_data"]["days_to_retrieve"] = days_to_retrieve
+        if "model_type" not in runtimeparams.keys():
             model_type = "load_forecast"
         else:
-            model_type = runtimeparams['model_type']
-        params['passed_data']['model_type'] = model_type
-        if 'var_model' not in runtimeparams.keys():
+            model_type = runtimeparams["model_type"]
+        params["passed_data"]["model_type"] = model_type
+        if "var_model" not in runtimeparams.keys():
             var_model = "sensor.power_load_no_var_loads"
         else:
-            var_model = runtimeparams['var_model']
-        params['passed_data']['var_model'] = var_model
-        if 'sklearn_model' not in runtimeparams.keys():
+            var_model = runtimeparams["var_model"]
+        params["passed_data"]["var_model"] = var_model
+        if "sklearn_model" not in runtimeparams.keys():
             sklearn_model = "KNeighborsRegressor"
         else:
-            sklearn_model = runtimeparams['sklearn_model']
-        params['passed_data']['sklearn_model'] = sklearn_model
-        if 'num_lags' not in runtimeparams.keys():
+            sklearn_model = runtimeparams["sklearn_model"]
+        params["passed_data"]["sklearn_model"] = sklearn_model
+        if "regression_model" not in runtimeparams.keys():
+            regression_model = "AdaBoostRegression"
+        else:
+            regression_model = runtimeparams["regression_model"]
+        params["passed_data"]["regression_model"] = regression_model
+        if "num_lags" not in runtimeparams.keys():
             num_lags = 48
         else:
-            num_lags = runtimeparams['num_lags']
-        params['passed_data']['num_lags'] = num_lags
-        if 'split_date_delta' not in runtimeparams.keys():
-            split_date_delta = '48h'
-        else:
-            split_date_delta = runtimeparams['split_date_delta']
-        params['passed_data']['split_date_delta'] = split_date_delta
-        if 'perform_backtest' not in runtimeparams.keys():
+            num_lags = runtimeparams["num_lags"]
+        params["passed_data"]["num_lags"] = num_lags
+        if "split_date_delta" not in runtimeparams.keys():
+            split_date_delta = "48h"
+        else:
+            split_date_delta = runtimeparams["split_date_delta"]
+        params["passed_data"]["split_date_delta"] = split_date_delta
+        if "perform_backtest" not in runtimeparams.keys():
             perform_backtest = False
         else:
-            perform_backtest = eval(str(runtimeparams['perform_backtest']).capitalize())
-        params['passed_data']['perform_backtest'] = perform_backtest
-        if 'model_predict_publish' not in runtimeparams.keys():
+            perform_backtest = eval(str(runtimeparams["perform_backtest"]).capitalize())
+        params["passed_data"]["perform_backtest"] = perform_backtest
+        if "model_predict_publish" not in runtimeparams.keys():
             model_predict_publish = False
         else:
-            model_predict_publish = eval(str(runtimeparams['model_predict_publish']).capitalize())
-        params['passed_data']['model_predict_publish'] = model_predict_publish
-        if 'model_predict_entity_id' not in runtimeparams.keys():
+            model_predict_publish = eval(
+                str(runtimeparams["model_predict_publish"]).capitalize()
+            )
+        params["passed_data"]["model_predict_publish"] = model_predict_publish
+        if "model_predict_entity_id" not in runtimeparams.keys():
             model_predict_entity_id = "sensor.p_load_forecast_custom_model"
         else:
-            model_predict_entity_id = runtimeparams['model_predict_entity_id']
-        params['passed_data']['model_predict_entity_id'] = model_predict_entity_id
-        if 'model_predict_unit_of_measurement' not in runtimeparams.keys():
+            model_predict_entity_id = runtimeparams["model_predict_entity_id"]
+        params["passed_data"]["model_predict_entity_id"] = model_predict_entity_id
+        if "model_predict_unit_of_measurement" not in runtimeparams.keys():
             model_predict_unit_of_measurement = "W"
         else:
-            model_predict_unit_of_measurement = runtimeparams['model_predict_unit_of_measurement']
-        params['passed_data']['model_predict_unit_of_measurement'] = model_predict_unit_of_measurement
-        if 'model_predict_friendly_name' not in runtimeparams.keys():
+            model_predict_unit_of_measurement = runtimeparams[
+                "model_predict_unit_of_measurement"
+            ]
+        params["passed_data"][
+            "model_predict_unit_of_measurement"
+        ] = model_predict_unit_of_measurement
+        if "model_predict_friendly_name" not in runtimeparams.keys():
             model_predict_friendly_name = "Load Power Forecast custom ML model"
         else:
-            model_predict_friendly_name = runtimeparams['model_predict_friendly_name']
-        params['passed_data']['model_predict_friendly_name'] = model_predict_friendly_name
-        # Treat optimization configuration parameters passed at runtime 
-        if 'num_def_loads' in runtimeparams.keys():
-            optim_conf['num_def_loads'] = runtimeparams['num_def_loads']
-        if 'P_deferrable_nom' in runtimeparams.keys():
-            optim_conf['P_deferrable_nom'] = runtimeparams['P_deferrable_nom']
-        if 'def_total_hours' in runtimeparams.keys():
-            optim_conf['def_total_hours'] = runtimeparams['def_total_hours']
-        if 'def_start_timestep' in runtimeparams.keys():
-            optim_conf['def_start_timestep'] = runtimeparams['def_start_timestep']
-        if 'def_end_timestep' in runtimeparams.keys():
-            optim_conf['def_end_timestep'] = runtimeparams['def_end_timestep']
-        if 'treat_def_as_semi_cont' in runtimeparams.keys():
-            optim_conf['treat_def_as_semi_cont'] = [eval(str(k).capitalize()) for k in runtimeparams['treat_def_as_semi_cont']]
-        if 'set_def_constant' in runtimeparams.keys():
-            optim_conf['set_def_constant'] = [eval(str(k).capitalize()) for k in runtimeparams['set_def_constant']]
-        if 'solcast_api_key' in runtimeparams.keys():
-            retrieve_hass_conf['solcast_api_key'] = runtimeparams['solcast_api_key']
-            optim_conf['weather_forecast_method'] = 'solcast'
-        if 'solcast_rooftop_id' in runtimeparams.keys():
-            retrieve_hass_conf['solcast_rooftop_id'] = runtimeparams['solcast_rooftop_id']
-            optim_conf['weather_forecast_method'] = 'solcast'
-        if 'solar_forecast_kwp' in runtimeparams.keys():
-            retrieve_hass_conf['solar_forecast_kwp'] = runtimeparams['solar_forecast_kwp']
-            optim_conf['weather_forecast_method'] = 'solar.forecast'
-        if 'weight_battery_discharge' in runtimeparams.keys():
-            optim_conf['weight_battery_discharge'] = runtimeparams['weight_battery_discharge']
-        if 'weight_battery_charge' in runtimeparams.keys():
-            optim_conf['weight_battery_charge'] = runtimeparams['weight_battery_charge']
+            model_predict_friendly_name = runtimeparams["model_predict_friendly_name"]
+        params["passed_data"][
+            "model_predict_friendly_name"
+        ] = model_predict_friendly_name
+        if "mlr_predict_entity_id" not in runtimeparams.keys():
+            mlr_predict_entity_id = "sensor.mlr_predict"
+        else:
+            mlr_predict_entity_id = runtimeparams["mlr_predict_entity_id"]
+        params["passed_data"]["mlr_predict_entity_id"] = mlr_predict_entity_id
+        if "mlr_predict_unit_of_measurement" not in runtimeparams.keys():
+            mlr_predict_unit_of_measurement = None
+        else:
+            mlr_predict_unit_of_measurement = runtimeparams[
+                "mlr_predict_unit_of_measurement"
+            ]
+        params["passed_data"][
+            "mlr_predict_unit_of_measurement"
+        ] = mlr_predict_unit_of_measurement
+        if "mlr_predict_friendly_name" not in runtimeparams.keys():
+            mlr_predict_friendly_name = "mlr predictor"
+        else:
+            mlr_predict_friendly_name = runtimeparams["mlr_predict_friendly_name"]
+        params["passed_data"]["mlr_predict_friendly_name"] = mlr_predict_friendly_name
+        # Treat optimization configuration parameters passed at runtime
+        if "num_def_loads" in runtimeparams.keys():
+            optim_conf["num_def_loads"] = runtimeparams["num_def_loads"]
+        if "P_deferrable_nom" in runtimeparams.keys():
+            optim_conf["P_deferrable_nom"] = runtimeparams["P_deferrable_nom"]
+        if "def_total_hours" in runtimeparams.keys():
+            optim_conf["def_total_hours"] = runtimeparams["def_total_hours"]
+        if "def_start_timestep" in runtimeparams.keys():
+            optim_conf["def_start_timestep"] = runtimeparams["def_start_timestep"]
+        if "def_end_timestep" in runtimeparams.keys():
+            optim_conf["def_end_timestep"] = runtimeparams["def_end_timestep"]
+        if "treat_def_as_semi_cont" in runtimeparams.keys():
+            optim_conf["treat_def_as_semi_cont"] = [
+                eval(str(k).capitalize())
+                for k in runtimeparams["treat_def_as_semi_cont"]
+            ]
+        if "set_def_constant" in runtimeparams.keys():
+            optim_conf["set_def_constant"] = [
+                eval(str(k).capitalize()) for k in runtimeparams["set_def_constant"]
+            ]
+        if "solcast_api_key" in runtimeparams.keys():
+            retrieve_hass_conf["solcast_api_key"] = runtimeparams["solcast_api_key"]
+            optim_conf["weather_forecast_method"] = "solcast"
+        if "solcast_rooftop_id" in runtimeparams.keys():
+            retrieve_hass_conf["solcast_rooftop_id"] = runtimeparams[
+                "solcast_rooftop_id"
+            ]
+            optim_conf["weather_forecast_method"] = "solcast"
+        if "solar_forecast_kwp" in runtimeparams.keys():
+            retrieve_hass_conf["solar_forecast_kwp"] = runtimeparams[
+                "solar_forecast_kwp"
+            ]
+            optim_conf["weather_forecast_method"] = "solar.forecast"
+        if "weight_battery_discharge" in runtimeparams.keys():
+            optim_conf["weight_battery_discharge"] = runtimeparams[
+                "weight_battery_discharge"
+            ]
+        if "weight_battery_charge" in runtimeparams.keys():
+            optim_conf["weight_battery_charge"] = runtimeparams["weight_battery_charge"]
+        if 'freq' in runtimeparams.keys():
+            retrieve_hass_conf['freq'] = pd.to_timedelta(runtimeparams['freq'], "minutes")
         # Treat plant configuration parameters passed at runtime
-        if 'SOCtarget' in runtimeparams.keys():
-            plant_conf['SOCtarget'] = runtimeparams['SOCtarget']
+        if "SOCtarget" in runtimeparams.keys():
+            plant_conf["SOCtarget"] = runtimeparams["SOCtarget"]
         # Treat custom entities id's and friendly names for variables
-        if 'custom_pv_forecast_id' in runtimeparams.keys():
-            params['passed_data']['custom_pv_forecast_id'] = runtimeparams['custom_pv_forecast_id']
-        if 'custom_load_forecast_id' in runtimeparams.keys():
-            params['passed_data']['custom_load_forecast_id'] = runtimeparams['custom_load_forecast_id']
-        if 'custom_batt_forecast_id' in runtimeparams.keys():
-            params['passed_data']['custom_batt_forecast_id'] = runtimeparams['custom_batt_forecast_id']
-        if 'custom_batt_soc_forecast_id' in runtimeparams.keys():
-            params['passed_data']['custom_batt_soc_forecast_id'] = runtimeparams['custom_batt_soc_forecast_id']
-        if 'custom_grid_forecast_id' in runtimeparams.keys():
-            params['passed_data']['custom_grid_forecast_id'] = runtimeparams['custom_grid_forecast_id']
-        if 'custom_cost_fun_id' in runtimeparams.keys():
-            params['passed_data']['custom_cost_fun_id'] = runtimeparams['custom_cost_fun_id']
-        if 'custom_optim_status_id' in runtimeparams.keys():
-            params['passed_data']['custom_optim_status_id'] = runtimeparams['custom_optim_status_id']
-        if 'custom_unit_load_cost_id' in runtimeparams.keys():
-            params['passed_data']['custom_unit_load_cost_id'] = runtimeparams['custom_unit_load_cost_id']
-        if 'custom_unit_prod_price_id' in runtimeparams.keys():
-            params['passed_data']['custom_unit_prod_price_id'] = runtimeparams['custom_unit_prod_price_id']
-        if 'custom_deferrable_forecast_id' in runtimeparams.keys():
-            params['passed_data']['custom_deferrable_forecast_id'] = runtimeparams['custom_deferrable_forecast_id']
+        if "custom_pv_forecast_id" in runtimeparams.keys():
+            params["passed_data"]["custom_pv_forecast_id"] = runtimeparams[
+                "custom_pv_forecast_id"
+            ]
+        if "custom_load_forecast_id" in runtimeparams.keys():
+            params["passed_data"]["custom_load_forecast_id"] = runtimeparams[
+                "custom_load_forecast_id"
+            ]
+        if "custom_batt_forecast_id" in runtimeparams.keys():
+            params["passed_data"]["custom_batt_forecast_id"] = runtimeparams[
+                "custom_batt_forecast_id"
+            ]
+        if "custom_batt_soc_forecast_id" in runtimeparams.keys():
+            params["passed_data"]["custom_batt_soc_forecast_id"] = runtimeparams[
+                "custom_batt_soc_forecast_id"
+            ]
+        if "custom_grid_forecast_id" in runtimeparams.keys():
+            params["passed_data"]["custom_grid_forecast_id"] = runtimeparams[
+                "custom_grid_forecast_id"
+            ]
+        if "custom_cost_fun_id" in runtimeparams.keys():
+            params["passed_data"]["custom_cost_fun_id"] = runtimeparams[
+                "custom_cost_fun_id"
+            ]
+        if "custom_optim_status_id" in runtimeparams.keys():
+            params["passed_data"]["custom_optim_status_id"] = runtimeparams[
+                "custom_optim_status_id"
+            ]
+        if "custom_unit_load_cost_id" in runtimeparams.keys():
+            params["passed_data"]["custom_unit_load_cost_id"] = runtimeparams[
+                "custom_unit_load_cost_id"
+            ]
+        if "custom_unit_prod_price_id" in runtimeparams.keys():
+            params["passed_data"]["custom_unit_prod_price_id"] = runtimeparams[
+                "custom_unit_prod_price_id"
+            ]
+        if "custom_deferrable_forecast_id" in runtimeparams.keys():
+            params["passed_data"]["custom_deferrable_forecast_id"] = runtimeparams[
+                "custom_deferrable_forecast_id"
+            ]
         # A condition to put a prefix on all published data
-        if 'publish_prefix' not in runtimeparams.keys():
+        if "publish_prefix" not in runtimeparams.keys():
             publish_prefix = ""
         else:
-            publish_prefix = runtimeparams['publish_prefix']
-        params['passed_data']['publish_prefix'] = publish_prefix
+            publish_prefix = runtimeparams["publish_prefix"]
+        params["passed_data"]["publish_prefix"] = publish_prefix
     # Serialize the final params
     params = json.dumps(params)
     return params, retrieve_hass_conf, optim_conf, plant_conf
 
-def get_yaml_parse(config_path: str, use_secrets: Optional[bool] = True,
+def get_yaml_parse(emhass_conf: dict, use_secrets: Optional[bool] = True,
                    params: Optional[str] = None) -> Tuple[dict, dict, dict]:
     """
     Perform parsing of the config.yaml file.
     
-    :param config_path: The path to the yaml configuration file
-    :type config_path: str
+    :param emhass_conf: Dictionary containing the needed emhass paths
+    :type emhass_conf: dict
     :param use_secrets: Indicate if we should use a secrets file or not.
         Set to False for unit tests.
     :type use_secrets: bool, optional
     :param params: Configuration parameters passed from data/options.json
     :type params: str
     :return: A tuple with the dictionaries containing the parsed data
     :rtype: tuple(dict)
 
     """
-    base = config_path.parent
     if params is None:
-        with open(config_path, 'r') as file:
+        with open(emhass_conf["config_path"], 'r') as file:
             input_conf = yaml.load(file, Loader=yaml.FullLoader)
     else:
         input_conf = json.loads(params)
     if use_secrets:
         if params is None:
-            with open(base / 'secrets_emhass.yaml', 'r') as file:
+            with open(emhass_conf["root_path"] / 'secrets_emhass.yaml', 'r') as file: #assume secrets file is in root path 
                 input_secrets = yaml.load(file, Loader=yaml.FullLoader)
         else:
-            input_secrets = input_conf.pop('params_secrets', None)
-   
-    if (type(input_conf['retrieve_hass_conf']) == list): #if using old config version 
-        retrieve_hass_conf = dict({key:d[key] for d in input_conf['retrieve_hass_conf'] for key in d})
+            input_secrets = input_conf.pop("params_secrets", None)
+
+    if type(input_conf["retrieve_hass_conf"]) == list:  # if using old config version
+        retrieve_hass_conf = dict(
+            {key: d[key] for d in input_conf["retrieve_hass_conf"] for key in d}
+        )
     else:
-        retrieve_hass_conf = input_conf.get('retrieve_hass_conf', {})
-        
+        retrieve_hass_conf = input_conf.get("retrieve_hass_conf", {})
+
     if use_secrets:
         retrieve_hass_conf.update(input_secrets)
     else:
-        retrieve_hass_conf['hass_url'] = 'http://supervisor/core/api'
-        retrieve_hass_conf['long_lived_token'] = '${SUPERVISOR_TOKEN}'
-        retrieve_hass_conf['time_zone'] = 'Europe/Paris'
-        retrieve_hass_conf['lat'] = 45.83
-        retrieve_hass_conf['lon'] = 6.86
-        retrieve_hass_conf['alt'] = 4807.8
-    retrieve_hass_conf['freq'] = pd.to_timedelta(retrieve_hass_conf['freq'], "minutes")
-    retrieve_hass_conf['time_zone'] = pytz.timezone(retrieve_hass_conf['time_zone'])
-    
-    if (type(input_conf['optim_conf']) == list):
-        optim_conf = dict({key:d[key] for d in input_conf['optim_conf'] for key in d})
-    else:
-        optim_conf = input_conf.get('optim_conf', {})
+        retrieve_hass_conf["hass_url"] = "http://supervisor/core/api"
+        retrieve_hass_conf["long_lived_token"] = "${SUPERVISOR_TOKEN}"
+        retrieve_hass_conf["time_zone"] = "Europe/Paris"
+        retrieve_hass_conf["lat"] = 45.83
+        retrieve_hass_conf["lon"] = 6.86
+        retrieve_hass_conf["alt"] = 4807.8
+    retrieve_hass_conf["freq"] = pd.to_timedelta(retrieve_hass_conf["freq"], "minutes")
+    retrieve_hass_conf["time_zone"] = pytz.timezone(retrieve_hass_conf["time_zone"])
+
+    if type(input_conf["optim_conf"]) == list:
+        optim_conf = dict({key: d[key] for d in input_conf["optim_conf"] for key in d})
+    else:
+        optim_conf = input_conf.get("optim_conf", {})
+
+    optim_conf["list_hp_periods"] = dict(
+        (key, d[key]) for d in optim_conf["list_hp_periods"] for key in d
+    )
+    optim_conf["delta_forecast"] = pd.Timedelta(days=optim_conf["delta_forecast"])
 
-    optim_conf['list_hp_periods'] = dict((key,d[key]) for d in optim_conf['list_hp_periods'] for key in d)
-    optim_conf['delta_forecast'] = pd.Timedelta(days=optim_conf['delta_forecast'])
-    
-    if (type(input_conf['plant_conf']) == list):
-        plant_conf = dict({key:d[key] for d in input_conf['plant_conf'] for key in d})
+    if type(input_conf["plant_conf"]) == list:
+        plant_conf = dict({key: d[key] for d in input_conf["plant_conf"] for key in d})
     else:
-        plant_conf = input_conf.get('plant_conf', {})
-    
+        plant_conf = input_conf.get("plant_conf", {})
+
     return retrieve_hass_conf, optim_conf, plant_conf
 
+
 def get_injection_dict(df: pd.DataFrame, plot_size: Optional[int] = 1366) -> dict:
     """
     Build a dictionary with graphs and tables for the webui.
 
     :param df: The optimization result DataFrame
     :type df: pd.DataFrame
     :param plot_size: Size of the plot figure in pixels, defaults to 1366
     :type plot_size: Optional[int], optional
     :return: A dictionary containing the graphs and tables in html format
     :rtype: dict
-    
+
     """
-    cols_p = [i for i in df.columns.to_list() if 'P_' in i]
+    cols_p = [i for i in df.columns.to_list() if "P_" in i]
     # Let's round the data in the DF
-    optim_status = df['optim_status'].unique().item()
-    df.drop('optim_status', axis=1, inplace=True)
-    cols_else = [i for i in df.columns.to_list() if 'P_' not in i]
+    optim_status = df["optim_status"].unique().item()
+    df.drop("optim_status", axis=1, inplace=True)
+    cols_else = [i for i in df.columns.to_list() if "P_" not in i]
     df = df.apply(pd.to_numeric)
     df[cols_p] = df[cols_p].astype(int)
     df[cols_else] = df[cols_else].round(3)
     # Create plots
     n_colors = len(cols_p)
-    colors = px.colors.sample_colorscale("jet", [n/(n_colors -1) for n in range(n_colors)])
-    fig_0 = px.line(df[cols_p], title='Systems powers schedule after optimization results', 
-                    template='presentation', line_shape="hv",
-                    color_discrete_sequence=colors)
-    fig_0.update_layout(xaxis_title='Timestamp', yaxis_title='System powers (W)')
-    if 'SOC_opt' in df.columns.to_list():
-        fig_1 = px.line(df['SOC_opt'], title='Battery state of charge schedule after optimization results', 
-                        template='presentation',  line_shape="hv",
-                        color_discrete_sequence=colors)
-        fig_1.update_layout(xaxis_title='Timestamp', yaxis_title='Battery SOC (%)')
-    cols_cost = [i for i in df.columns.to_list() if 'cost_' in i or 'unit_' in i]
+    colors = px.colors.sample_colorscale(
+        "jet", [n / (n_colors - 1) for n in range(n_colors)]
+    )
+    fig_0 = px.line(
+        df[cols_p],
+        title="Systems powers schedule after optimization results",
+        template="presentation",
+        line_shape="hv",
+        color_discrete_sequence=colors,
+    )
+    fig_0.update_layout(xaxis_title="Timestamp", yaxis_title="System powers (W)")
+    if "SOC_opt" in df.columns.to_list():
+        fig_1 = px.line(
+            df["SOC_opt"],
+            title="Battery state of charge schedule after optimization results",
+            template="presentation",
+            line_shape="hv",
+            color_discrete_sequence=colors,
+        )
+        fig_1.update_layout(xaxis_title="Timestamp", yaxis_title="Battery SOC (%)")
+    cols_cost = [i for i in df.columns.to_list() if "cost_" in i or "unit_" in i]
     n_colors = len(cols_cost)
-    colors = px.colors.sample_colorscale("jet", [n/(n_colors -1) for n in range(n_colors)])
-    fig_2 = px.line(df[cols_cost], title='Systems costs obtained from optimization results', 
-                    template='presentation', line_shape="hv",
-                    color_discrete_sequence=colors)
-    fig_2.update_layout(xaxis_title='Timestamp', yaxis_title='System costs (currency)')
+    colors = px.colors.sample_colorscale(
+        "jet", [n / (n_colors - 1) for n in range(n_colors)]
+    )
+    fig_2 = px.line(
+        df[cols_cost],
+        title="Systems costs obtained from optimization results",
+        template="presentation",
+        line_shape="hv",
+        color_discrete_sequence=colors,
+    )
+    fig_2.update_layout(xaxis_title="Timestamp", yaxis_title="System costs (currency)")
     # Get full path to image
-    image_path_0 = fig_0.to_html(full_html=False, default_width='75%')
-    if 'SOC_opt' in df.columns.to_list():
-        image_path_1 = fig_1.to_html(full_html=False, default_width='75%')
-    image_path_2 = fig_2.to_html(full_html=False, default_width='75%')
+    image_path_0 = fig_0.to_html(full_html=False, default_width="75%")
+    if "SOC_opt" in df.columns.to_list():
+        image_path_1 = fig_1.to_html(full_html=False, default_width="75%")
+    image_path_2 = fig_2.to_html(full_html=False, default_width="75%")
     # The tables
-    table1 = df.reset_index().to_html(classes='mystyle', index=False)
-    cost_cols = [i for i in df.columns if 'cost_' in i]
+    table1 = df.reset_index().to_html(classes="mystyle", index=False)
+    cost_cols = [i for i in df.columns if "cost_" in i]
     table2 = df[cost_cols].reset_index().sum(numeric_only=True)
-    table2['optim_status'] = optim_status
-    table2 = table2.to_frame(name='Value').reset_index(names='Variable').to_html(classes='mystyle', index=False)
+    table2["optim_status"] = optim_status
+    table2 = (
+        table2.to_frame(name="Value")
+        .reset_index(names="Variable")
+        .to_html(classes="mystyle", index=False)
+    )
     # The dict of plots
     injection_dict = {}
-    injection_dict['title'] = '<h2>EMHASS optimization results</h2>'
-    injection_dict['subsubtitle0'] = '<h4>Plotting latest optimization results</h4>'
-    injection_dict['figure_0'] = image_path_0
-    if 'SOC_opt' in df.columns.to_list():
-        injection_dict['figure_1'] = image_path_1
-    injection_dict['figure_2'] = image_path_2
-    injection_dict['subsubtitle1'] = '<h4>Last run optimization results table</h4>'
-    injection_dict['table1'] = table1
-    injection_dict['subsubtitle2'] = '<h4>Summary table for latest optimization results</h4>'
-    injection_dict['table2'] = table2
+    injection_dict["title"] = "<h2>EMHASS optimization results</h2>"
+    injection_dict["subsubtitle0"] = "<h4>Plotting latest optimization results</h4>"
+    injection_dict["figure_0"] = image_path_0
+    if "SOC_opt" in df.columns.to_list():
+        injection_dict["figure_1"] = image_path_1
+    injection_dict["figure_2"] = image_path_2
+    injection_dict["subsubtitle1"] = "<h4>Last run optimization results table</h4>"
+    injection_dict["table1"] = table1
+    injection_dict["subsubtitle2"] = (
+        "<h4>Summary table for latest optimization results</h4>"
+    )
+    injection_dict["table2"] = table2
     return injection_dict
 
-def get_injection_dict_forecast_model_fit(df_fit_pred: pd.DataFrame, mlf: MLForecaster) -> dict:
+
+def get_injection_dict_forecast_model_fit(
+    df_fit_pred: pd.DataFrame, mlf: MLForecaster
+) -> dict:
     """
     Build a dictionary with graphs and tables for the webui for special MLF fit case.
 
     :param df_fit_pred: The fit result DataFrame
     :type df_fit_pred: pd.DataFrame
     :param mlf: The MLForecaster object
     :type mlf: MLForecaster
     :return: A dictionary containing the graphs and tables in html format
     :rtype: dict
     """
     fig = df_fit_pred.plot()
-    fig.layout.template = 'presentation'
-    fig.update_yaxes(title_text = mlf.model_type)
-    fig.update_xaxes(title_text = "Time")
-    image_path_0 = fig.to_html(full_html=False, default_width='75%')
+    fig.layout.template = "presentation"
+    fig.update_yaxes(title_text=mlf.model_type)
+    fig.update_xaxes(title_text="Time")
+    image_path_0 = fig.to_html(full_html=False, default_width="75%")
     # The dict of plots
     injection_dict = {}
-    injection_dict['title'] = '<h2>Custom machine learning forecast model fit</h2>'
-    injection_dict['subsubtitle0'] = '<h4>Plotting train/test forecast model results for '+mlf.model_type+'</h4>'
-    injection_dict['subsubtitle0'] = '<h4>Forecasting variable '+mlf.var_model+'</h4>'
-    injection_dict['figure_0'] = image_path_0
+    injection_dict["title"] = "<h2>Custom machine learning forecast model fit</h2>"
+    injection_dict["subsubtitle0"] = (
+        "<h4>Plotting train/test forecast model results for " + mlf.model_type + "</h4>"
+    )
+    injection_dict["subsubtitle0"] = (
+        "<h4>Forecasting variable " + mlf.var_model + "</h4>"
+    )
+    injection_dict["figure_0"] = image_path_0
     return injection_dict
 
-def get_injection_dict_forecast_model_tune(df_pred_optim: pd.DataFrame, mlf: MLForecaster) -> dict:
+
+def get_injection_dict_forecast_model_tune(
+    df_pred_optim: pd.DataFrame, mlf: MLForecaster
+) -> dict:
     """
     Build a dictionary with graphs and tables for the webui for special MLF tune case.
 
     :param df_pred_optim: The tune result DataFrame
     :type df_pred_optim: pd.DataFrame
     :param mlf: The MLForecaster object
     :type mlf: MLForecaster
     :return: A dictionary containing the graphs and tables in html format
     :rtype: dict
     """
     fig = df_pred_optim.plot()
-    fig.layout.template = 'presentation'
-    fig.update_yaxes(title_text = mlf.model_type)
-    fig.update_xaxes(title_text = "Time")
-    image_path_0 = fig.to_html(full_html=False, default_width='75%')
+    fig.layout.template = "presentation"
+    fig.update_yaxes(title_text=mlf.model_type)
+    fig.update_xaxes(title_text="Time")
+    image_path_0 = fig.to_html(full_html=False, default_width="75%")
     # The dict of plots
     injection_dict = {}
-    injection_dict['title'] = '<h2>Custom machine learning forecast model tune</h2>'
-    injection_dict['subsubtitle0'] = '<h4>Performed a tuning routine using bayesian optimization for '+mlf.model_type+'</h4>'
-    injection_dict['subsubtitle0'] = '<h4>Forecasting variable '+mlf.var_model+'</h4>'
-    injection_dict['figure_0'] = image_path_0
+    injection_dict["title"] = "<h2>Custom machine learning forecast model tune</h2>"
+    injection_dict["subsubtitle0"] = (
+        "<h4>Performed a tuning routine using bayesian optimization for "
+        + mlf.model_type
+        + "</h4>"
+    )
+    injection_dict["subsubtitle0"] = (
+        "<h4>Forecasting variable " + mlf.var_model + "</h4>"
+    )
+    injection_dict["figure_0"] = image_path_0
     return injection_dict
 
-def build_params(params: dict, params_secrets: dict, options: dict, addon: int, logger: logging.Logger) -> dict:
+
+def build_params(
+    params: dict,
+    params_secrets: dict,
+    options: dict,
+    addon: int,
+    logger: logging.Logger,
+) -> dict:
     """
     Build the main params dictionary from the loaded options.json when using the add-on.
 
     :param params: The main params dictionary
     :type params: dict
     :param params_secrets: The dictionary containing the secret protected variables
     :type params_secrets: dict
@@ -531,53 +740,128 @@
     :param logger: The logger object
     :type logger: logging.Logger
     :return: The builded dictionary
     :rtype: dict
     """
     if addon == 1:
         # Updating variables in retrieve_hass_conf
-        params['retrieve_hass_conf']['freq'] = options.get('optimization_time_step',params['retrieve_hass_conf']['freq'])
-        params['retrieve_hass_conf']['days_to_retrieve'] = options.get('historic_days_to_retrieve',params['retrieve_hass_conf']['days_to_retrieve'])
-        params['retrieve_hass_conf']['var_PV'] = options.get('sensor_power_photovoltaics',params['retrieve_hass_conf']['var_PV'])
-        params['retrieve_hass_conf']['var_load'] = options.get('sensor_power_load_no_var_loads',params['retrieve_hass_conf']['var_load'])
-        params['retrieve_hass_conf']['load_negative'] = options.get('load_negative',params['retrieve_hass_conf']['load_negative'])
-        params['retrieve_hass_conf']['set_zero_min'] = options.get('set_zero_min',params['retrieve_hass_conf']['set_zero_min'])
-        params['retrieve_hass_conf']['var_replace_zero'] = [options.get('sensor_power_photovoltaics',params['retrieve_hass_conf']['var_replace_zero'])]
-        params['retrieve_hass_conf']['var_interp'] = [options.get('sensor_power_photovoltaics',params['retrieve_hass_conf']['var_PV']), options.get('sensor_power_load_no_var_loads',params['retrieve_hass_conf']['var_load'])]
-        params['retrieve_hass_conf']['method_ts_round'] = options.get('method_ts_round',params['retrieve_hass_conf']['method_ts_round'])
+        params["retrieve_hass_conf"]["freq"] = options.get(
+            "optimization_time_step", params["retrieve_hass_conf"]["freq"]
+        )
+        params["retrieve_hass_conf"]["days_to_retrieve"] = options.get(
+            "historic_days_to_retrieve",
+            params["retrieve_hass_conf"]["days_to_retrieve"],
+        )
+        params["retrieve_hass_conf"]["var_PV"] = options.get(
+            "sensor_power_photovoltaics", params["retrieve_hass_conf"]["var_PV"]
+        )
+        params["retrieve_hass_conf"]["var_load"] = options.get(
+            "sensor_power_load_no_var_loads", params["retrieve_hass_conf"]["var_load"]
+        )
+        params["retrieve_hass_conf"]["load_negative"] = options.get(
+            "load_negative", params["retrieve_hass_conf"]["load_negative"]
+        )
+        params["retrieve_hass_conf"]["set_zero_min"] = options.get(
+            "set_zero_min", params["retrieve_hass_conf"]["set_zero_min"]
+        )
+        params["retrieve_hass_conf"]["var_replace_zero"] = [
+            options.get(
+                "sensor_power_photovoltaics",
+                params["retrieve_hass_conf"]["var_replace_zero"],
+            )
+        ]
+        params["retrieve_hass_conf"]["var_interp"] = [
+            options.get(
+                "sensor_power_photovoltaics", params["retrieve_hass_conf"]["var_PV"]
+            ),
+            options.get(
+                "sensor_power_load_no_var_loads",
+                params["retrieve_hass_conf"]["var_load"],
+            ),
+        ]
+        params["retrieve_hass_conf"]["method_ts_round"] = options.get(
+            "method_ts_round", params["retrieve_hass_conf"]["method_ts_round"]
+        )
         # Update params Secrets if specified
-        params['params_secrets'] = params_secrets
-        params['params_secrets']['time_zone'] = options.get('time_zone',params_secrets['time_zone'])
-        params['params_secrets']['lat'] = options.get('Latitude',params_secrets['lat'])
-        params['params_secrets']['lon'] = options.get('Longitude',params_secrets['lon'])
-        params['params_secrets']['alt'] = options.get('Altitude',params_secrets['alt'])
+        params["params_secrets"] = params_secrets
+        params["params_secrets"]["time_zone"] = options.get(
+            "time_zone", params_secrets["time_zone"]
+        )
+        params["params_secrets"]["lat"] = options.get("Latitude", params_secrets["lat"])
+        params["params_secrets"]["lon"] = options.get(
+            "Longitude", params_secrets["lon"]
+        )
+        params["params_secrets"]["alt"] = options.get("Altitude", params_secrets["alt"])
         # Updating variables in optim_conf
-        params['optim_conf']['set_use_battery'] = options.get('set_use_battery',params['optim_conf']['set_use_battery'])
-        params['optim_conf']['num_def_loads'] = options.get('number_of_deferrable_loads',params['optim_conf']['num_def_loads'])
-        if options.get('list_nominal_power_of_deferrable_loads',None) != None: 
-            params['optim_conf']['P_deferrable_nom'] = [i['nominal_power_of_deferrable_loads'] for i in options.get('list_nominal_power_of_deferrable_loads')]
-        if options.get('list_operating_hours_of_each_deferrable_load',None) != None: 
-            params['optim_conf']['def_total_hours'] = [i['operating_hours_of_each_deferrable_load'] for i in options.get('list_operating_hours_of_each_deferrable_load')]
-        if options.get('list_treat_deferrable_load_as_semi_cont',None) != None: 
-            params['optim_conf']['treat_def_as_semi_cont'] = [i['treat_deferrable_load_as_semi_cont'] for i in options.get('list_treat_deferrable_load_as_semi_cont')]
-        params['optim_conf']['weather_forecast_method'] = options.get('weather_forecast_method',params['optim_conf']['weather_forecast_method'])
+        params["optim_conf"]["set_use_battery"] = options.get(
+            "set_use_battery", params["optim_conf"]["set_use_battery"]
+        )
+        params["optim_conf"]["num_def_loads"] = options.get(
+            "number_of_deferrable_loads", params["optim_conf"]["num_def_loads"]
+        )
+        if options.get("list_nominal_power_of_deferrable_loads", None) != None:
+            params["optim_conf"]["P_deferrable_nom"] = [
+                i["nominal_power_of_deferrable_loads"]
+                for i in options.get("list_nominal_power_of_deferrable_loads")
+            ]
+        if options.get("list_operating_hours_of_each_deferrable_load", None) != None:
+            params["optim_conf"]["def_total_hours"] = [
+                i["operating_hours_of_each_deferrable_load"]
+                for i in options.get("list_operating_hours_of_each_deferrable_load")
+            ]
+        if options.get("list_treat_deferrable_load_as_semi_cont", None) != None:
+            params["optim_conf"]["treat_def_as_semi_cont"] = [
+                i["treat_deferrable_load_as_semi_cont"]
+                for i in options.get("list_treat_deferrable_load_as_semi_cont")
+            ]
+        params["optim_conf"]["weather_forecast_method"] = options.get(
+            "weather_forecast_method", params["optim_conf"]["weather_forecast_method"]
+        )
         # Update optional param secrets
-        if params['optim_conf']['weather_forecast_method'] == "solcast":
-            params['params_secrets']['solcast_api_key'] = options.get('optional_solcast_api_key',params_secrets.get('solcast_api_key',"123456"))
-            params['params_secrets']['solcast_rooftop_id'] = options.get('optional_solcast_rooftop_id',params_secrets.get('solcast_rooftop_id',"123456"))
-        elif params['optim_conf']['weather_forecast_method'] == "solar.forecast":    
-            params['params_secrets']['solar_forecast_kwp'] = options.get('optional_solar_forecast_kwp',params_secrets.get('solar_forecast_kwp',5))
-        params['optim_conf']['load_forecast_method'] = options.get('load_forecast_method',params['optim_conf']['load_forecast_method'])
-        params['optim_conf']['delta_forecast'] = options.get('delta_forecast_daily',params['optim_conf']['delta_forecast'])
-        params['optim_conf']['load_cost_forecast_method'] = options.get('load_cost_forecast_method',params['optim_conf']['load_cost_forecast_method'])
-        if options.get('list_set_deferrable_load_single_constant',None) != None: 
-            params['optim_conf']['set_def_constant'] = [i['set_deferrable_load_single_constant'] for i in options.get('list_set_deferrable_load_single_constant')]
-        if options.get('list_peak_hours_periods_start_hours',None) != None and options.get('list_peak_hours_periods_end_hours',None) != None:
-            start_hours_list = [i['peak_hours_periods_start_hours'] for i in options['list_peak_hours_periods_start_hours']]
-            end_hours_list = [i['peak_hours_periods_end_hours'] for i in options['list_peak_hours_periods_end_hours']]
+        if params["optim_conf"]["weather_forecast_method"] == "solcast":
+            params["params_secrets"]["solcast_api_key"] = options.get(
+                "optional_solcast_api_key",
+                params_secrets.get("solcast_api_key", "123456"),
+            )
+            params["params_secrets"]["solcast_rooftop_id"] = options.get(
+                "optional_solcast_rooftop_id",
+                params_secrets.get("solcast_rooftop_id", "123456"),
+            )
+        elif params["optim_conf"]["weather_forecast_method"] == "solar.forecast":
+            params["params_secrets"]["solar_forecast_kwp"] = options.get(
+                "optional_solar_forecast_kwp",
+                params_secrets.get("solar_forecast_kwp", 5),
+            )
+        params["optim_conf"]["load_forecast_method"] = options.get(
+            "load_forecast_method", params["optim_conf"]["load_forecast_method"]
+        )
+        params["optim_conf"]["delta_forecast"] = options.get(
+            "delta_forecast_daily", params["optim_conf"]["delta_forecast"]
+        )
+        params["optim_conf"]["load_cost_forecast_method"] = options.get(
+            "load_cost_forecast_method",
+            params["optim_conf"]["load_cost_forecast_method"],
+        )
+        if options.get("list_set_deferrable_load_single_constant", None) != None:
+            params["optim_conf"]["set_def_constant"] = [
+                i["set_deferrable_load_single_constant"]
+                for i in options.get("list_set_deferrable_load_single_constant")
+            ]
+        if (
+            options.get("list_peak_hours_periods_start_hours", None) != None
+            and options.get("list_peak_hours_periods_end_hours", None) != None
+        ):
+            start_hours_list = [
+                i["peak_hours_periods_start_hours"]
+                for i in options["list_peak_hours_periods_start_hours"]
+            ]
+            end_hours_list = [
+                i["peak_hours_periods_end_hours"]
+                for i in options["list_peak_hours_periods_end_hours"]
+            ]
             num_peak_hours = len(start_hours_list)
             list_hp_periods_list = [{'period_hp_'+str(i+1):[{'start':start_hours_list[i]},{'end':end_hours_list[i]}]} for i in range(num_peak_hours)]
             params['optim_conf']['list_hp_periods'] = list_hp_periods_list
         params['optim_conf']['load_cost_hp'] = options.get('load_peak_hours_cost',params['optim_conf']['load_cost_hp'])
         params['optim_conf']['load_cost_hc'] = options.get('load_offpeak_hours_cost', params['optim_conf']['load_cost_hc'])
         params['optim_conf']['prod_price_forecast_method'] = options.get('production_price_forecast_method', params['optim_conf']['prod_price_forecast_method'])
         params['optim_conf']['prod_sell_price'] = options.get('photovoltaic_production_sell_price',params['optim_conf']['prod_sell_price'])
@@ -641,48 +925,64 @@
             for x in range(len(params['optim_conf']['def_total_hours']), params['optim_conf']['num_def_loads']):
                 params['optim_conf']['def_total_hours'].append(0)                   
         if params['optim_conf']['num_def_loads'] is not len(params['optim_conf']['P_deferrable_nom']):
             logger.warning("P_deferrable_nom / list_nominal_power_of_deferrable_loads does not match number in num_def_loads, adding default values to parameter")
             for x in range(len(params['optim_conf']['P_deferrable_nom']), params['optim_conf']['num_def_loads']):
                 params['optim_conf']['P_deferrable_nom'].append(0)   
         # days_to_retrieve should be no less then 2
-        if params['retrieve_hass_conf']['days_to_retrieve'] < 2:
-            params['retrieve_hass_conf']['days_to_retrieve'] = 2
-            logger.warning("days_to_retrieve should not be lower then 2, setting days_to_retrieve to 2. Make sure your sensors also have at least 2 days of history")
+        if params["retrieve_hass_conf"]["days_to_retrieve"] < 2:
+            params["retrieve_hass_conf"]["days_to_retrieve"] = 2
+            logger.warning(
+                "days_to_retrieve should not be lower then 2, setting days_to_retrieve to 2. Make sure your sensors also have at least 2 days of history"
+            )
     else:
-        params['params_secrets'] = params_secrets
+        params["params_secrets"] = params_secrets
     # The params dict
-    params['passed_data'] = {'pv_power_forecast':None,'load_power_forecast':None,'load_cost_forecast':None,'prod_price_forecast':None,
-                             'prediction_horizon':None,'soc_init':None,'soc_final':None,'def_total_hours':None,'def_start_timestep':None,'def_end_timestep':None,'alpha':None,'beta':None}
+    params["passed_data"] = {
+        "pv_power_forecast": None,
+        "load_power_forecast": None,
+        "load_cost_forecast": None,
+        "prod_price_forecast": None,
+        "prediction_horizon": None,
+        "soc_init": None,
+        "soc_final": None,
+        "def_total_hours": None,
+        "def_start_timestep": None,
+        "def_end_timestep": None,
+        "alpha": None,
+        "beta": None,
+    }
     return params
 
+
 def get_days_list(days_to_retrieve: int) -> pd.date_range:
     """
     Get list of past days from today to days_to_retrieve.
-    
+
     :param days_to_retrieve: Total number of days to retrieve from the past
     :type days_to_retrieve: int
     :return: The list of days
     :rtype: pd.date_range
 
     """
     today = datetime.now(timezone.utc).replace(minute=0, second=0, microsecond=0)
     d = (today - timedelta(days=days_to_retrieve)).isoformat()
-    days_list = pd.date_range(start=d, end=today.isoformat(), freq='D')
-    
+    days_list = pd.date_range(start=d, end=today.isoformat(), freq="D")
+
     return days_list
 
+
 def set_df_index_freq(df: pd.DataFrame) -> pd.DataFrame:
     """
     Set the freq of a DataFrame DateTimeIndex.
-    
+
     :param df: Input DataFrame
     :type df: pd.DataFrame
     :return: Input DataFrame with freq defined
     :rtype: pd.DataFrame
-    
+
     """
     idx_diff = np.diff(df.index)
     sampling = pd.to_timedelta(np.median(idx_diff))
     df = df[~df.index.duplicated()]
     df = df.asfreq(sampling)
     return df
```

### Comparing `emhass-0.8.6/src/emhass/web_server.py` & `emhass-0.9.0/src/emhass/web_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,66 +9,67 @@
 from pathlib import Path
 import os, json, argparse, pickle, yaml, logging,  re
 from distutils.util import strtobool
 
 from emhass.command_line import set_input_data_dict
 from emhass.command_line import perfect_forecast_optim, dayahead_forecast_optim, naive_mpc_optim
 from emhass.command_line import forecast_model_fit, forecast_model_predict, forecast_model_tune
+from emhass.command_line import regressor_model_fit, regressor_model_predict
 from emhass.command_line import publish_data
 from emhass.utils import get_injection_dict, get_injection_dict_forecast_model_fit, \
     get_injection_dict_forecast_model_tune, build_params
 
 # Define the Flask instance
 app = Flask(__name__)
 
 #check logfile for error, anything after string match if provided 
 def checkFileLog(refString=None):
     if (refString is not None): 
        logArray = grabLog(refString) #grab reduced log array
     else: 
-        if ((data_path / 'actionLogs.txt')).exists():
-            with open(str(data_path / 'actionLogs.txt'), "r") as fp:
+        if ((emhass_conf['data_path'] / 'actionLogs.txt')).exists():
+            with open(str(emhass_conf['data_path'] / 'actionLogs.txt'), "r") as fp:
                     logArray = fp.readlines()
     for logString in logArray:
             if (logString.split(' ', 1)[0] == "ERROR"):
                 return True     
     return False
 
 #find string in logs, append all lines after to return
 def grabLog(refString): 
     isFound = []
     output = []
-    if ((data_path / 'actionLogs.txt')).exists():
-            with open(str(data_path / 'actionLogs.txt'), "r") as fp:
+    if ((emhass_conf['data_path'] / 'actionLogs.txt')).exists():
+            with open(str(emhass_conf['data_path'] / 'actionLogs.txt'), "r") as fp:
                     logArray = fp.readlines()
             for x in range(len(logArray)-1): #find all matches and log key in isFound
                 if (re.search(refString,logArray[x])):
                    isFound.append(x)
             if len(isFound) != 0:
                 for x in range(isFound[-1],len(logArray)): #use isFound to extract last related action logs  
                     output.append(logArray[x])
     return output
 
 #clear the log file
 def clearFileLog(): 
-    if ((data_path / 'actionLogs.txt')).exists():
-        with open(str(data_path / 'actionLogs.txt'), "w") as fp:
+    if ((emhass_conf['data_path'] / 'actionLogs.txt')).exists():
+        with open(str(emhass_conf['data_path'] / 'actionLogs.txt'), "w") as fp:
             fp.truncate()    
 
 #initial index page render
 @app.route('/')
 def index():
     app.logger.info("EMHASS server online, serving index.html...")
     # Load HTML template
     file_loader = PackageLoader('emhass', 'templates')
     env = Environment(loader=file_loader)
     template = env.get_template('index.html')
     # Load cache dict
-    if (data_path / 'injection_dict.pkl').exists():
-        with open(str(data_path / 'injection_dict.pkl'), "rb") as fid:
+    if (emhass_conf['data_path'] / 'injection_dict.pkl').exists():
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "rb") as fid:
             injection_dict = pickle.load(fid)
     else:
         app.logger.warning("The data container dictionary is empty... Please launch an optimization task")
         injection_dict={}
 
     # replace {{basename}} in html template html with path root  
     # basename = request.headers.get("X-Ingress-Path", "")
@@ -81,35 +82,35 @@
 @app.route('/template/<action_name>', methods=['GET'])
 def template_action(action_name):
     app.logger.info(" >> Sending rendered template table data")
     if action_name == 'table-template':
         file_loader = PackageLoader('emhass', 'templates')
         env = Environment(loader=file_loader)
         template = env.get_template('template.html')
-        if (data_path / 'injection_dict.pkl').exists():
-            with open(str(data_path / 'injection_dict.pkl'), "rb") as fid:
+        if (emhass_conf['data_path'] / 'injection_dict.pkl').exists():
+            with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "rb") as fid:
                 injection_dict = pickle.load(fid)
         else:
             app.logger.warning("The data container dictionary is empty... Please launch an optimization task")
             injection_dict={}        
         return make_response(template.render(injection_dict=injection_dict))
 
 #post actions 
 @app.route('/action/<action_name>', methods=['POST'])
 def action_call(action_name):
-    with open(str(data_path / 'params.pkl'), "rb") as fid:
-        config_path, params = pickle.load(fid)
+    with open(str(emhass_conf['data_path'] / 'params.pkl'), "rb") as fid:
+        emhass_conf['config_path'], params = pickle.load(fid)
     runtimeparams = request.get_json(force=True)
     params = json.dumps(params)
     if runtimeparams is not None and runtimeparams != '{}':
         app.logger.info("Passed runtime parameters: " + str(runtimeparams))
     runtimeparams = json.dumps(runtimeparams)
     ActionStr = " >> Setting input data dict"
     app.logger.info(ActionStr)
-    input_data_dict = set_input_data_dict(config_path, str(data_path), costfun, 
+    input_data_dict = set_input_data_dict(emhass_conf, costfun, 
         params, runtimeparams, action_name, app.logger)
     if not input_data_dict:
         return make_response(grabLog(ActionStr), 400)
     if action_name == 'publish-data':
         ActionStr = " >> Publishing data..."
         app.logger.info(ActionStr)
         _ = publish_data(input_data_dict, app.logger)
@@ -118,49 +119,49 @@
             return make_response(msg, 201)
         return make_response(grabLog(ActionStr), 400)
     elif action_name == 'perfect-optim':
         ActionStr = " >> Performing perfect optimization..."
         app.logger.info(ActionStr)
         opt_res = perfect_forecast_optim(input_data_dict, app.logger)
         injection_dict = get_injection_dict(opt_res)
-        with open(str(data_path / 'injection_dict.pkl'), "wb") as fid:
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "wb") as fid:
             pickle.dump(injection_dict, fid)
         msg = f'EMHASS >> Action perfect-optim executed... \n'
         if not checkFileLog(ActionStr):
             return make_response(msg, 201)
         return make_response(grabLog(ActionStr), 400)
     elif action_name == 'dayahead-optim':
         ActionStr = " >> Performing dayahead optimization..."
         app.logger.info(ActionStr)
         opt_res = dayahead_forecast_optim(input_data_dict, app.logger)
         injection_dict = get_injection_dict(opt_res)
-        with open(str(data_path / 'injection_dict.pkl'), "wb") as fid:
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "wb") as fid:
             pickle.dump(injection_dict, fid)
         msg = f'EMHASS >> Action dayahead-optim executed... \n'
         if not checkFileLog(ActionStr):
             return make_response(msg, 201)
         return make_response(grabLog(ActionStr), 400)
     elif action_name == 'naive-mpc-optim':
         ActionStr = " >> Performing naive MPC optimization..."
         app.logger.info(ActionStr)
         opt_res = naive_mpc_optim(input_data_dict, app.logger)
         injection_dict = get_injection_dict(opt_res)
-        with open(str(data_path / 'injection_dict.pkl'), "wb") as fid:
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "wb") as fid:
             pickle.dump(injection_dict, fid)
         msg = f'EMHASS >> Action naive-mpc-optim executed... \n'
         if not checkFileLog(ActionStr):
             return make_response(msg, 201)
         return make_response(grabLog(ActionStr), 400)
     elif action_name == 'forecast-model-fit':
         ActionStr = " >> Performing a machine learning forecast model fit..."
         app.logger.info(ActionStr)
         df_fit_pred, _, mlf = forecast_model_fit(input_data_dict, app.logger)
         injection_dict = get_injection_dict_forecast_model_fit(
             df_fit_pred, mlf)
-        with open(str(data_path / 'injection_dict.pkl'), "wb") as fid:
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "wb") as fid:
             pickle.dump(injection_dict, fid)
         msg = f'EMHASS >> Action forecast-model-fit executed... \n'
         if not checkFileLog(ActionStr):
             return make_response(msg, 201)
         return make_response(grabLog(ActionStr), 400)
     elif action_name == 'forecast-model-predict':
         ActionStr = " >> Performing a machine learning forecast model predict..."
@@ -169,34 +170,50 @@
         if df_pred is None:
             return make_response(grabLog(ActionStr), 400)
         table1 = df_pred.reset_index().to_html(classes='mystyle', index=False)
         injection_dict = {}
         injection_dict['title'] = '<h2>Custom machine learning forecast model predict</h2>'
         injection_dict['subsubtitle0'] = '<h4>Performed a prediction using a pre-trained model</h4>'
         injection_dict['table1'] = table1
-        with open(str(data_path / 'injection_dict.pkl'), "wb") as fid:
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "wb") as fid:
             pickle.dump(injection_dict, fid)
         msg = f'EMHASS >> Action forecast-model-predict executed... \n'
         if not checkFileLog(ActionStr):
             return make_response(msg, 201)
         return make_response(grabLog(ActionStr), 400)
     elif action_name == 'forecast-model-tune':
         ActionStr = " >> Performing a machine learning forecast model tune..."
         app.logger.info(ActionStr)
         df_pred_optim, mlf = forecast_model_tune(input_data_dict, app.logger)    
         if df_pred_optim is None or  mlf is None:
             return make_response(grabLog(ActionStr), 400)
         injection_dict = get_injection_dict_forecast_model_tune(
             df_pred_optim, mlf)
-        with open(str(data_path / 'injection_dict.pkl'), "wb") as fid:
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "wb") as fid:
             pickle.dump(injection_dict, fid)
         msg = f'EMHASS >> Action forecast-model-tune executed... \n'
         if not checkFileLog(ActionStr):
             return make_response(msg, 201)
         return make_response(grabLog(ActionStr), 400)
+    elif action_name == 'regressor-model-fit':
+        ActionStr = " >> Performing a machine learning regressor fit..."
+        app.logger.info(ActionStr)
+        regressor_model_fit(input_data_dict, app.logger)
+        msg = f'EMHASS >> Action regressor-model-fit executed... \n'
+        if not checkFileLog(ActionStr):
+            return make_response(msg, 201)
+        return make_response(grabLog(ActionStr), 400)
+    elif action_name == 'regressor-model-predict':
+        ActionStr = " >> Performing a machine learning regressor predict..."
+        app.logger.info(ActionStr)
+        regressor_model_predict(input_data_dict, app.logger)
+        msg = f'EMHASS >> Action regressor-model-predict executed... \n'
+        if not checkFileLog(ActionStr):
+            return make_response(msg, 201)
+        return make_response(grabLog(ActionStr), 400)
     else:
         app.logger.error("ERROR: passed action is not valid")
         msg = f'EMHASS >> ERROR: Passed action is not valid... \n'
         return make_response(msg, 400)
 
 if __name__ == "__main__":
     # Parsing arguments
@@ -249,16 +266,21 @@
             options = None       
 
     #if data path specified by options.json
     if options is not None:
         if options.get('data_path', None) != None and options.get('data_path', None) != "default":
             DATA_PATH = options.get('data_path', None);   
 
+    #save paths to dictionary
     config_path = Path(CONFIG_PATH)
     data_path = Path(DATA_PATH)
+    emhass_conf = {}
+    emhass_conf['config_path'] = config_path
+    emhass_conf['data_path'] = data_path
+    emhass_conf['root_path'] = Path(config_path).parent #assume root is parent of config_path
     
     # Read the example default config file
     if config_path.exists():
         with open(config_path, 'r') as file:
             config = yaml.load(file, Loader=yaml.FullLoader)
         retrieve_hass_conf = config['retrieve_hass_conf']
         optim_conf = config['optim_conf']
@@ -270,16 +292,16 @@
     params = {}
     params['retrieve_hass_conf'] = retrieve_hass_conf
     params['optim_conf'] = optim_conf
     params['plant_conf'] = plant_conf
     web_ui_url = '0.0.0.0'
 
     # Initialize this global dict
-    if (data_path / 'injection_dict.pkl').exists():
-        with open(str(data_path / 'injection_dict.pkl'), "rb") as fid:
+    if (emhass_conf['data_path'] / 'injection_dict.pkl').exists():
+        with open(str(emhass_conf['data_path'] / 'injection_dict.pkl'), "rb") as fid:
             injection_dict = pickle.load(fid)
     else:
         injection_dict = None
     
     if args.addon==1:
         # The cost function
         costfun = options.get('costfun', 'profit')
@@ -380,27 +402,27 @@
                 app.logger.error("No specified Home Assistant KEY")     
                 raise Exception("Can not find Home Assistant KEY from secrets_emhass.yaml or ARG/ENV") 
     # Build params
     if use_options:
         params = build_params(params, params_secrets, options, 1, app.logger)
     else:
         params = build_params(params, params_secrets, options, args.addon, app.logger)
-    if os.path.exists(str(data_path)): 
-        with open(str(data_path / 'params.pkl'), "wb") as fid:
+    if os.path.exists(str(emhass_conf['data_path'])): 
+        with open(str(emhass_conf['data_path'] / 'params.pkl'), "wb") as fid:
             pickle.dump((config_path, params), fid)
     else: 
-        raise Exception("missing: " + str(data_path))        
+        raise Exception("missing: " + str(emhass_conf['data_path']))   
 
     # Define logger
     #stream logger
     ch = logging.StreamHandler() 
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
     ch.setFormatter(formatter)
     #Action File logger
-    fileLogger = logging.FileHandler(str(data_path / 'actionLogs.txt')) 
+    fileLogger = logging.FileHandler(str(emhass_conf['data_path'] / 'actionLogs.txt')) 
     formatter = logging.Formatter('%(levelname)s - %(name)s - %(message)s')
     fileLogger.setFormatter(formatter) # add format to Handler
     if logging_level == "DEBUG":
         app.logger.setLevel(logging.DEBUG)
         ch.setLevel(logging.DEBUG)
         fileLogger.setLevel(logging.DEBUG)
     elif logging_level == "INFO":
@@ -424,13 +446,13 @@
     app.logger.addHandler(fileLogger)   
     clearFileLog() #Clear Action File logger file, ready for new instance
 
     # Launch server
     port = int(os.environ.get('PORT', 5000))
     app.logger.info("Launching the emhass webserver at: http://"+web_ui_url+":"+str(port))
     app.logger.info("Home Assistant data fetch will be performed using url: "+hass_url)
-    app.logger.info("The data path is: "+str(data_path))
+    app.logger.info("The data path is: "+str(emhass_conf['data_path']))
     try:
         app.logger.info("Using core emhass version: "+version('emhass'))
     except PackageNotFoundError:
         app.logger.info("Using development emhass version")
     serve(app, host=web_ui_url, port=port, threads=8)
```

### Comparing `emhass-0.8.6/src/emhass.egg-info/PKG-INFO` & `emhass-0.9.0/src/emhass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.8.6
+Version: 0.9.0
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,19 +20,19 @@
 Requires-Dist: scipy==1.12.0
 Requires-Dist: pandas<=2.0.3
 Requires-Dist: pvlib>=0.10.2
 Requires-Dist: protobuf>=3.0.0
 Requires-Dist: pytz>=2021.1
 Requires-Dist: requests>=2.25.1
 Requires-Dist: beautifulsoup4>=4.9.3
-Requires-Dist: h5py==3.10.0
+Requires-Dist: h5py==3.11.0
 Requires-Dist: pulp>=2.4
 Requires-Dist: pyyaml>=5.4.1
 Requires-Dist: tables<=3.9.1
-Requires-Dist: skforecast==0.11.0
+Requires-Dist: skforecast==0.12.0
 Requires-Dist: flask>=2.0.3
 Requires-Dist: waitress>=2.1.1
 Requires-Dist: plotly>=5.6.0
 
 <div align="center">
   <br>
   <img alt="EMHASS" src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/emhass_logo.png" width="300px">
@@ -59,14 +59,28 @@
   <a href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/emhass">
   </a>
   <a href="https://emhass.readthedocs.io/en/latest/">
     <img alt="Read the Docs" src="https://img.shields.io/readthedocs/emhass">
   </a>
 </p>
+<div align="center">
+ <a href="https://emhass.readthedocs.io/en/latest/">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Documentation_button.svg" alt="Documentation">
+  </a>
+   <a href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Community_button.svg" alt="Community">
+  </a>
+  <a href="https://github.com/davidusb-geek/emhass/issues">
+      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Issues_button.svg" alt="Issues">
+  </a>
+  <a href="https://github.com/davidusb-geek/emhass-add-on">
+     <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/EMHASS_Add_on_button.svg" alt="EMHASS Add-on">
+  </a>
+</div>
 <br>
 <p align="center">
 If you like this work please consider buying a coffee ;-) 
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/davidusbgeek" target="_blank">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" >
@@ -103,15 +117,15 @@
 EMHASS was designed to be integrated with Home Assistant, hence it's name. 
 Installation instructions and example Home Assistant automation configurations are given below.
 
 You must follow these steps to make EMHASS work properly:
 
 1) Define all the parameters in the configuration file according to your installation. See the description for each parameter in the **configuration** section.
 
-2) You most notably will need to define the main data entering EMHASS. This will be the `sensor_power_photovoltaics` for the name of the your hass variable containing the PV produced power and the variable `sensor_power_load_no_var_loads` for the load power of your household excluding the power of the deferrable loads that you want to optimize.
+2) You most notably will need to define the main data entering EMHASS. This will be the `sensor.power_photovoltaics` for the name of the your hass variable containing the PV produced power and the variable `sensor.power_load_no_var_loads` for the load power of your household excluding the power of the deferrable loads that you want to optimize.
 
 3) Launch the actual optimization and check the results. This can be done manually using the buttons in the web ui or with a `curl` command like this: `curl -i -H 'Content-Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-optim`.
 
 4) If you’re satisfied with the optimization results then you can set the optimization and data publish task commands in an automation. You can read more about this on the **usage** section below.
 
 5) The final step is to link the deferrable loads variables to real switchs on your installation. An example code for this using automations and the shell command integration is presented below in the **usage** section.
 
@@ -366,15 +380,15 @@
 
 - Load power forecast: how much power your house will demand on the next 24h. This is given in Watts.
 
 - Load cost forecast: the price of the energy from the grid on the next 24h. This is given in EUR/kWh.
 
 - PV production selling price forecast: at what price are you selling your excess PV production on the next 24h. This is given in EUR/kWh.
 
-The sensor containing the load data should be specified in parameter `var_load` in the configuration file. As we want to optimize the household energies, when need to forecast the load power conumption. The default method for this is a naive approach using 1-day persistence. The load data variable should not contain the data from the deferrable loads themselves. For example, lets say that you set your deferrable load to be the washing machine. The variable that you should enter in EMHASS will be: `var_load: 'sensor.power_load_no_var_loads'` and `sensor_power_load_no_var_loads = sensor_power_load - sensor_power_washing_machine`. This is supposing that the overall load of your house is contained in variable: `sensor_power_load`. The sensor `sensor_power_load_no_var_loads` can be easily created with a new template sensor in Home Assistant.
+The sensor containing the load data should be specified in parameter `var_load` in the configuration file. As we want to optimize the household energies, when need to forecast the load power conumption. The default method for this is a naive approach using 1-day persistence. The load data variable should not contain the data from the deferrable loads themselves. For example, lets say that you set your deferrable load to be the washing machine. The variable that you should enter in EMHASS will be: `var_load: 'sensor.power_load_no_var_loads'` and `sensor.power_load_no_var_loads = sensor.power_load - sensor.power_washing_machine`. This is supposing that the overall load of your house is contained in variable: `sensor.power_load`. The sensor `sensor.power_load_no_var_loads` can be easily created with a new template sensor in Home Assistant.
 
 If you are implementing a MPC controller, then you should also need to provide some data at the optimization runtime using the key `runtimeparams`.
 
 The valid values to pass for both forecast data and MPC related data are explained below.
 
 ### Forecast data
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.8.6 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.9.0 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: wheel
 Requires-Dist: numpy==1.26.4 Requires-Dist: scipy==1.12.0 Requires-Dist:
 pandas<=2.0.3 Requires-Dist: pvlib>=0.10.2 Requires-Dist: protobuf>=3.0.0
 Requires-Dist: pytz>=2021.1 Requires-Dist: requests>=2.25.1 Requires-Dist:
-beautifulsoup4>=4.9.3 Requires-Dist: h5py==3.10.0 Requires-Dist: pulp>=2.4
+beautifulsoup4>=4.9.3 Requires-Dist: h5py==3.11.0 Requires-Dist: pulp>=2.4
 Requires-Dist: pyyaml>=5.4.1 Requires-Dist: tables<=3.9.1 Requires-Dist:
-skforecast==0.11.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
+skforecast==0.12.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
 Requires-Dist: plotly>=5.6.0
 
                                    [EMHASS]
               ************ EEnneerrggyy MMaannaaggeemmeenntt ffoorr HHoommee AAssssiissttaanntt ************
 
  _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/
   _g_i_t_h_u_b_/_d_a_v_i_d_u_s_b_-_g_e_e_k_/_e_m_h_a_s_s_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_B_W_7_K_S_C_H_N_9_0_]
          _[_G_i_t_H_u_b_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_R_e_a_d_ _t_h_e_ _D_o_c_s_]
+               _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_m_m_u_n_i_t_y_]_[_I_s_s_u_e_s_]_[_E_M_H_A_S_S_ _A_d_d_-_o_n_]
 
            If you like this work please consider buying a coffee ;-)
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 EHMASS is a Python module designed to optimize your home energy interfacing
 with Home Assistant. ## Introduction EMHASS (Energy Management for Home
 Assistant) is an optimization tool designed for residential households. The
 package uses a Linear Programming approach to optimize energy usage while
@@ -73,17 +74,17 @@
 approach and a main configuration file defined by the user. EMHASS was designed
 to be integrated with Home Assistant, hence it's name. Installation
 instructions and example Home Assistant automation configurations are given
 below. You must follow these steps to make EMHASS work properly: 1) Define all
 the parameters in the configuration file according to your installation. See
 the description for each parameter in the **configuration** section. 2) You
 most notably will need to define the main data entering EMHASS. This will be
-the `sensor_power_photovoltaics` for the name of the your hass variable
+the `sensor.power_photovoltaics` for the name of the your hass variable
 containing the PV produced power and the variable
-`sensor_power_load_no_var_loads` for the load power of your household excluding
+`sensor.power_load_no_var_loads` for the load power of your household excluding
 the power of the deferrable loads that you want to optimize. 3) Launch the
 actual optimization and check the results. This can be done manually using the
 buttons in the web ui or with a `curl` command like this: `curl -i -H 'Content-
 Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-
 optim`. 4) If youâre satisfied with the optimization results then you can set
 the optimization and data publish task commands in an automation. You can read
 more about this on the **usage** section below. 5) The final step is to link
@@ -319,18 +320,18 @@
 be specified in parameter `var_load` in the configuration file. As we want to
 optimize the household energies, when need to forecast the load power
 conumption. The default method for this is a naive approach using 1-day
 persistence. The load data variable should not contain the data from the
 deferrable loads themselves. For example, lets say that you set your deferrable
 load to be the washing machine. The variable that you should enter in EMHASS
 will be: `var_load: 'sensor.power_load_no_var_loads'` and
-`sensor_power_load_no_var_loads = sensor_power_load -
-sensor_power_washing_machine`. This is supposing that the overall load of your
-house is contained in variable: `sensor_power_load`. The sensor
-`sensor_power_load_no_var_loads` can be easily created with a new template
+`sensor.power_load_no_var_loads = sensor.power_load -
+sensor.power_washing_machine`. This is supposing that the overall load of your
+house is contained in variable: `sensor.power_load`. The sensor
+`sensor.power_load_no_var_loads` can be easily created with a new template
 sensor in Home Assistant. If you are implementing a MPC controller, then you
 should also need to provide some data at the optimization runtime using the key
 `runtimeparams`. The valid values to pass for both forecast data and MPC
 related data are explained below. ### Forecast data It is possible to provide
 EMHASS with your own forecast data. For this just add the data as list of
 values to a data dictionary during the call to `emhass` using the
 `runtimeparams` option. For example if using the add-on or the standalone
```

### Comparing `emhass-0.8.6/src/emhass.egg-info/SOURCES.txt` & `emhass-0.9.0/src/emhass.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 setup.py
 data/data_load_cost_forecast.csv
 data/data_load_forecast.csv
 data/data_prod_price_forecast.csv
 data/data_train_load_clustering.pkl
 data/data_train_load_forecast.pkl
 data/data_weather_forecast.csv
+data/heating_prediction.csv
 data/opt_res_latest.csv
 data/opt_res_perfect_optim_cost.csv
 data/opt_res_perfect_optim_profit.csv
 data/opt_res_perfect_optim_self-consumption.csv
 data/test_df_final.pkl
 data/test_response_get_data_get_method.pbz2
 data/test_response_scrapper_get_method.pbz2
 data/test_response_solarforecast_get_method.pbz2
 data/test_response_solcast_get_method.pbz2
 src/emhass/__init__.py
 src/emhass/command_line.py
 src/emhass/forecast.py
 src/emhass/machine_learning_forecaster.py
+src/emhass/machine_learning_regressor.py
 src/emhass/optimization.py
 src/emhass/retrieve_hass.py
 src/emhass/utils.py
 src/emhass/web_server.py
 src/emhass.egg-info/PKG-INFO
 src/emhass.egg-info/SOURCES.txt
 src/emhass.egg-info/dependency_links.txt
@@ -45,10 +47,11 @@
 src/emhass/static/img/emhass_logo_short.svg
 src/emhass/static/img/feather-sprite.svg
 src/emhass/templates/index.html
 src/emhass/templates/template.html
 tests/test_command_line_utils.py
 tests/test_forecast.py
 tests/test_machine_learning_forecaster.py
+tests/test_machine_learning_regressor.py
 tests/test_optimization.py
 tests/test_retrieve_hass.py
 tests/test_utils.py
```

### Comparing `emhass-0.8.6/tests/test_command_line_utils.py` & `emhass-0.9.0/tests/test_command_line_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,63 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import unittest
 from unittest.mock import patch
 import pandas as pd
 import pathlib, json, yaml, copy
+import numpy as np
 
 from emhass.command_line import set_input_data_dict
-from emhass.command_line import perfect_forecast_optim, dayahead_forecast_optim, naive_mpc_optim
-from emhass.command_line import forecast_model_fit, forecast_model_predict, forecast_model_tune
+from emhass.command_line import (
+    perfect_forecast_optim,
+    dayahead_forecast_optim,
+    naive_mpc_optim,
+)
+from emhass.command_line import (
+    forecast_model_fit,
+    forecast_model_predict,
+    forecast_model_tune,
+    regressor_model_fit,
+    regressor_model_predict,
+)
 from emhass.command_line import publish_data
 from emhass.command_line import main
 from emhass import utils
 
-# the root folder
+# create paths
 root = str(utils.get_root(__file__, num_parent=2))
+emhass_conf = {}
+emhass_conf['config_path'] = pathlib.Path(root) / 'config_emhass.yaml'
+emhass_conf['data_path'] = pathlib.Path(root) / 'data/'
+emhass_conf['root_path'] = pathlib.Path(root)
+
 # create logger
-logger, ch = utils.get_logger(__name__, root, save_to_file=False)
+logger, ch = utils.get_logger(__name__, emhass_conf, save_to_file=False)
 
 class TestCommandLineUtils(unittest.TestCase):
     
     @staticmethod
     def get_test_params():
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
                 'lon': 6.86,
                 'alt': 8000.0
-            }
-            })
+            }})
+        #Force config params for testing
+        params["retrieve_hass_conf"]['var_PV'] = 'sensor.power_photovoltaics'
+        params["retrieve_hass_conf"]['var_load'] = 'sensor.power_load_no_var_loads'
+        params["retrieve_hass_conf"]['var_replace_zero'] = ['sensor.power_photovoltaics']
+        params["retrieve_hass_conf"]['var_interp'] = ['sensor.power_photovoltaics','sensor.power_load_no_var_loads'] 
         return params
 
     def setUp(self):
         params = TestCommandLineUtils.get_test_params()
         runtimeparams = {
             'pv_power_forecast':[i+1 for i in range(48)],
             'load_power_forecast':[i+1 for i in range(48)],
@@ -45,38 +65,36 @@
             'prod_price_forecast':[i+1 for i in range(48)]
         }
         self.runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         self.params_json = json.dumps(params)
         
     def test_set_input_data_dict(self):
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'dayahead-optim'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertIsInstance(input_data_dict, dict)
         self.assertTrue(input_data_dict['df_input_data'] == None)
         self.assertIsInstance(input_data_dict['df_input_data_dayahead'], pd.DataFrame)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].index.freq is not None)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].isnull().sum().sum()==0)
         self.assertTrue(input_data_dict['fcst'].optim_conf['weather_forecast_method']=='list')
         self.assertTrue(input_data_dict['fcst'].optim_conf['load_forecast_method']=='list')
         self.assertTrue(input_data_dict['fcst'].optim_conf['load_cost_forecast_method']=='list')
         self.assertTrue(input_data_dict['fcst'].optim_conf['prod_price_forecast_method']=='list')
         action = 'publish-data'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertTrue(input_data_dict['df_input_data'] == None)
         self.assertTrue(input_data_dict['df_input_data_dayahead'] == None)
         self.assertTrue(input_data_dict['P_PV_forecast'] == None)
         self.assertTrue(input_data_dict['P_load_forecast'] == None)
         action = 'naive-mpc-optim'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertIsInstance(input_data_dict, dict)
         self.assertIsInstance(input_data_dict['df_input_data_dayahead'], pd.DataFrame)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].index.freq is not None)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].isnull().sum().sum()==0)
         self.assertTrue(len(input_data_dict['df_input_data_dayahead'])==10) # The default value for prediction_horizon
         runtimeparams = {
@@ -85,28 +103,28 @@
             'load_cost_forecast':[1,2,3,4,5,6,7,8,9,10],
             'prod_price_forecast':[1,2,3,4,5,6,7,8,9,10]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params = copy.deepcopy(json.loads(self.params_json))
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertIsInstance(input_data_dict, dict)
         self.assertIsInstance(input_data_dict['df_input_data_dayahead'], pd.DataFrame)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].index.freq is not None)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].isnull().sum().sum()==0)
         self.assertTrue(len(input_data_dict['df_input_data_dayahead'])==10) # The default value for prediction_horizon
         action = 'naive-mpc-optim'
         runtimeparams['prediction_horizon'] = 10
         runtimeparams_json = json.dumps(runtimeparams)
         params = copy.deepcopy(json.loads(self.params_json))
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertIsInstance(input_data_dict, dict)
         self.assertIsInstance(input_data_dict['df_input_data_dayahead'], pd.DataFrame)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].index.freq is not None)
         self.assertTrue(input_data_dict['df_input_data_dayahead'].isnull().sum().sum()==0)
         self.assertTrue(len(input_data_dict['df_input_data_dayahead'])==10) # The fixed value for prediction_horizon
         # Test passing just load cost and prod price as lists
@@ -115,40 +133,36 @@
         runtimeparams = {
             'load_cost_forecast':[i+1 for i in range(48)],
             'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertTrue(input_data_dict['fcst'].optim_conf['load_cost_forecast_method']=='list')
         self.assertTrue(input_data_dict['fcst'].optim_conf['prod_price_forecast_method']=='list')
     
     def test_webserver_get_injection_dict(self):
         # First perform a day-ahead optimization
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'dayahead-optim'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = dayahead_forecast_optim(input_data_dict, logger, debug=True)
         injection_dict = utils.get_injection_dict(opt_res)
         self.assertIsInstance(injection_dict, dict)
         self.assertIsInstance(injection_dict['table1'], str)
         self.assertIsInstance(injection_dict['table2'], str)
     
     def test_dayahead_forecast_optim(self):
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'dayahead-optim'
         params = copy.deepcopy(json.loads(self.params_json))
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = dayahead_forecast_optim(input_data_dict, logger, debug=True)
         self.assertIsInstance(opt_res, pd.DataFrame)
         self.assertTrue(opt_res.isnull().sum().sum()==0)
         self.assertTrue(len(opt_res)==len(params['passed_data']['pv_power_forecast']))
         # Test passing just load cost and prod price as lists
         action = 'dayahead-optim'
@@ -156,45 +170,41 @@
         runtimeparams = {
             'load_cost_forecast':[i+1 for i in range(48)],
             'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = dayahead_forecast_optim(input_data_dict, logger, debug=True)
         self.assertIsInstance(opt_res, pd.DataFrame)
         self.assertTrue(opt_res.isnull().sum().sum()==0)
         self.assertTrue(input_data_dict['fcst'].optim_conf['load_cost_forecast_method']=='list')
         self.assertTrue(input_data_dict['fcst'].optim_conf['prod_price_forecast_method']=='list')
         self.assertEqual(opt_res['unit_load_cost'].values.tolist(), runtimeparams['load_cost_forecast'])
         self.assertEqual(opt_res['unit_prod_price'].values.tolist(), runtimeparams['prod_price_forecast'])
         
     def test_perfect_forecast_optim(self):
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'perfect-optim'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = perfect_forecast_optim(input_data_dict, logger, debug=True)
         self.assertIsInstance(opt_res, pd.DataFrame)
         self.assertTrue(opt_res.isnull().sum().sum()==0)
         self.assertIsInstance(opt_res.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(opt_res.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertTrue('cost_fun_'+input_data_dict["costfun"] in opt_res.columns)
         
     def test_naive_mpc_optim(self):
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'naive-mpc-optim'
         params = copy.deepcopy(json.loads(self.params_json))
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = naive_mpc_optim(input_data_dict, logger, debug=True)
         self.assertIsInstance(opt_res, pd.DataFrame)
         self.assertTrue(opt_res.isnull().sum().sum()==0)
         self.assertTrue(len(opt_res)==10)
         # A test similar to the docs
         runtimeparams = {"pv_power_forecast":
@@ -203,52 +213,50 @@
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params['optim_conf']['weather_forecast_method'] = 'list'
         params['optim_conf']['load_forecast_method'] = 'naive'
         params['optim_conf']['load_cost_forecast_method'] = 'hp_hc_periods'
         params['optim_conf']['prod_price_forecast_method'] = 'constant'
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = naive_mpc_optim(input_data_dict, logger, debug=True)
         self.assertIsInstance(opt_res, pd.DataFrame)
         self.assertTrue(opt_res.isnull().sum().sum()==0)
         self.assertTrue(len(opt_res)==10)
         # Test publish after passing the forecast as list
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'naive-mpc-optim'
         params = copy.deepcopy(json.loads(self.params_json))
         params['retrieve_hass_conf']['method_ts_round'] = 'first'
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = naive_mpc_optim(input_data_dict, logger, debug=True)
         action = 'publish-data'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, None, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, None, 
                                               action, logger, get_data_from_file=True)
         opt_res_first = publish_data(input_data_dict, logger, opt_res_latest=opt_res)
         self.assertTrue(len(opt_res_first)==1)
         action = 'naive-mpc-optim'
         params = copy.deepcopy(json.loads(self.params_json))
         params['retrieve_hass_conf']['method_ts_round'] = 'last'
         params['optim_conf']['set_use_battery'] = True
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         opt_res = naive_mpc_optim(input_data_dict, logger, debug=True)
         action = 'publish-data'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, None, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, None, 
                                               action, logger, get_data_from_file=True)
         opt_res_last = publish_data(input_data_dict, logger, opt_res_latest=opt_res)
         self.assertTrue(len(opt_res_last)==1)
         # Reproduce when trying to publish data but params=None and runtimeparams=None
         action = 'publish-data'
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, None, None, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, None, None, 
                                               action, logger, get_data_from_file=True)
         opt_res_last = publish_data(input_data_dict, logger, opt_res_latest=opt_res)
         self.assertTrue(len(opt_res_last)==1)
         # Check if status is published
         from datetime import datetime
         now_precise = datetime.now(input_data_dict['retrieve_hass_conf']['time_zone']).replace(second=0, microsecond=0)
         idx_closest = opt_res.index.get_indexer([now_precise], method='nearest')[0]
@@ -260,16 +268,14 @@
                                         custom_cost_fun_id["friendly_name"],
                                         type_var = 'optim_status',
                                         publish_prefix = publish_prefix)
         self.assertTrue(hasattr(response, '__class__'))
         self.assertTrue(data['attributes']['friendly_name'] == 'EMHASS optimization status')
     
     def test_forecast_model_fit_predict_tune(self):
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'forecast-model-fit' # fit, predict and tune methods
         params = TestCommandLineUtils.get_test_params()
         runtimeparams = {
             "days_to_retrieve": 20,
             "model_type": "load_forecast",
             "var_model": "sensor.power_load_no_var_loads",
@@ -282,84 +288,173 @@
             "model_predict_unit_of_measurement": "W",
             "model_predict_friendly_name": "Load Power Forecast KNN regressor"
         }
         runtimeparams_json = json.dumps(runtimeparams)
         # params['passed_data'] = runtimeparams
         params['optim_conf']['load_forecast_method'] = 'skforecast'
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertTrue(input_data_dict['params']['passed_data']['model_type'] == 'load_forecast')
         self.assertTrue(input_data_dict['params']['passed_data']['sklearn_model'] == 'KNeighborsRegressor')
         self.assertTrue(input_data_dict['params']['passed_data']['perform_backtest'] == False)
         # Check that the default params are loaded
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, self.params_json, self.runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, self.params_json, self.runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         self.assertTrue(input_data_dict['params']['passed_data']['model_type'] == 'load_forecast')
         self.assertTrue(input_data_dict['params']['passed_data']['sklearn_model'] == 'KNeighborsRegressor')
         self.assertIsInstance(input_data_dict['df_input_data'], pd.DataFrame)
         # Test the fit method
         df_fit_pred, df_fit_pred_backtest, mlf = forecast_model_fit(input_data_dict, logger, debug=True)
         self.assertIsInstance(df_fit_pred, pd.DataFrame)
         self.assertTrue(df_fit_pred_backtest == None)
         # Test ijection_dict for fit method on webui
         injection_dict = utils.get_injection_dict_forecast_model_fit(df_fit_pred, mlf)
         self.assertIsInstance(injection_dict, dict)
         self.assertIsInstance(injection_dict['figure_0'], str)
         # Test the predict method on observations following the train period
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         df_pred = forecast_model_predict(input_data_dict, logger, use_last_window=False, debug=True, mlf=mlf)
         self.assertIsInstance(df_pred, pd.Series)
         self.assertTrue(df_pred.isnull().sum().sum() == 0)
         # Now a predict using last_window
         df_pred = forecast_model_predict(input_data_dict, logger, debug=True, mlf=mlf)
         self.assertIsInstance(df_pred, pd.Series)
         self.assertTrue(df_pred.isnull().sum().sum() == 0)
         # Test the tune method
-        df_pred_optim, mlf = forecast_model_tune(input_data_dict, logger, debug=True, mlf=mlf)
+        df_pred_optim, mlf = forecast_model_tune(
+            input_data_dict, logger, debug=True, mlf=mlf
+        )
         self.assertIsInstance(df_pred_optim, pd.DataFrame)
         self.assertTrue(mlf.is_tuned == True)
-        # Test ijection_dict for tune method on webui
+        # Test injection_dict for tune method on webui
         injection_dict = utils.get_injection_dict_forecast_model_tune(df_fit_pred, mlf)
         self.assertIsInstance(injection_dict, dict)
-        self.assertIsInstance(injection_dict['figure_0'], str)
+        self.assertIsInstance(injection_dict["figure_0"], str)
+
+    def test_regressor_model_fit_predict(self):
+        costfun = "profit"
+        action = "regressor-model-fit"  # fit and predict methods
+        params = TestCommandLineUtils.get_test_params()
+        runtimeparams = {
+            "csv_file": "heating_prediction.csv",
+            "features": ["degreeday", "solar"],
+            "target": "hour",
+            "regression_model": "AdaBoostRegression",
+            "model_type": "heating_hours_degreeday",
+            "timestamp": "timestamp",
+            "date_features": ["month", "day_of_week"],
+            "mlr_predict_entity_id": "sensor.predicted_hours_test",
+            "mlr_predict_unit_of_measurement": "h",
+            "mlr_predict_friendly_name": "Predicted hours",
+            "new_values": [12.79, 4.766, 1, 2],
+        }
+        runtimeparams_json = json.dumps(runtimeparams)
+        params_json = json.dumps(params)
+        input_data_dict = set_input_data_dict(
+            emhass_conf,
+            costfun,
+            params_json,
+            runtimeparams_json,
+            action,
+            logger,
+            get_data_from_file=True,
+        )
+        self.assertTrue(
+            input_data_dict["params"]["passed_data"]["model_type"]
+            == "heating_hours_degreeday",
+        )
+        self.assertTrue(
+            input_data_dict["params"]["passed_data"]["regression_model"]
+            == "AdaBoostRegression",
+        )
+        self.assertTrue(
+            input_data_dict["params"]["passed_data"]["csv_file"]
+            == "heating_prediction.csv",
+        )
+        mlr = regressor_model_fit(input_data_dict, logger, debug=True)
+
+        # def test_regressor_model_predict(self):
+        costfun = "profit"
+        action = "regressor-model-predict"  # predict methods
+        params = TestCommandLineUtils.get_test_params()
+        runtimeparams = {
+            "csv_file": "heating_prediction.csv",
+            "features": ["degreeday", "solar"],
+            "target": "hour",
+            "regression_model": "AdaBoostRegression",
+            "model_type": "heating_hours_degreeday",
+            "timestamp": "timestamp",
+            "date_features": ["month", "day_of_week"],
+            "mlr_predict_entity_id": "sensor.predicted_hours_test",
+            "mlr_predict_unit_of_measurement": "h",
+            "mlr_predict_friendly_name": "Predicted hours",
+            "new_values": [12.79, 4.766, 1, 2],
+        }
+        runtimeparams_json = json.dumps(runtimeparams)
+        params["passed_data"] = runtimeparams
+        params_json = json.dumps(params)
+
+        input_data_dict = set_input_data_dict(
+            emhass_conf,
+            costfun,
+            params_json,
+            runtimeparams_json,
+            action,
+            logger,
+            get_data_from_file=True,
+        )
+        self.assertTrue(
+            input_data_dict["params"]["passed_data"]["model_type"]
+            == "heating_hours_degreeday",
+        )
+        self.assertTrue(
+            input_data_dict["params"]["passed_data"]["mlr_predict_friendly_name"]
+            == "Predicted hours",
+        )
+
+        regressor_model_predict(input_data_dict, logger, debug=True, mlr=mlr)
+
     
-    @patch('sys.argv', ['main', '--action', 'test', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
+    @patch('sys.argv', ['main', '--action', 'test', '--config', str(emhass_conf['config_path']), 
                         '--debug', 'True'])
     def test_main_wrong_action(self):
         opt_res = main()
         self.assertEqual(opt_res, None)
         
-    @patch('sys.argv', ['main', '--action', 'perfect-optim', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
-                        '--debug', 'True'])
+    @patch('sys.argv', ['main', '--action', 'perfect-optim', '--config', str(emhass_conf['config_path']), 
+                        '--debug', 'True', '--params', json.dumps(get_test_params())])
     def test_main_perfect_forecast_optim(self):
         opt_res = main()
         self.assertIsInstance(opt_res, pd.DataFrame)
-        self.assertTrue(opt_res.isnull().sum().sum()==0)
+        self.assertTrue(opt_res.isnull().sum().sum() == 0)
         self.assertIsInstance(opt_res.index, pd.core.indexes.datetimes.DatetimeIndex)
-        self.assertIsInstance(opt_res.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
-        
+        self.assertIsInstance(
+            opt_res.index.dtype,
+            pd.core.dtypes.dtypes.DatetimeTZDtype,
+        )
+
     def test_main_dayahead_forecast_optim(self):
-        with patch('sys.argv', ['main', '--action', 'dayahead-optim', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
+        with patch('sys.argv', ['main', '--action', 'dayahead-optim', '--config', str(emhass_conf['config_path']), 
                                 '--params', self.params_json, '--runtimeparams', self.runtimeparams_json,
                                 '--debug', 'True']):
             opt_res = main()
         self.assertIsInstance(opt_res, pd.DataFrame)
-        self.assertTrue(opt_res.isnull().sum().sum()==0)
-        
+        self.assertTrue(opt_res.isnull().sum().sum() == 0)
+
     def test_main_naive_mpc_optim(self):
-        with patch('sys.argv', ['main', '--action', 'naive-mpc-optim', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
+        with patch('sys.argv', ['main', '--action', 'naive-mpc-optim', '--config', str(emhass_conf['config_path']), 
                                 '--params', self.params_json, '--runtimeparams', self.runtimeparams_json,
                                 '--debug', 'True']):
             opt_res = main()
         self.assertIsInstance(opt_res, pd.DataFrame)
-        self.assertTrue(opt_res.isnull().sum().sum()==0)
-        self.assertTrue(len(opt_res)==10)
-        
+        self.assertTrue(opt_res.isnull().sum().sum() == 0)
+        self.assertTrue(len(opt_res) == 10)
+
     def test_main_forecast_model_fit(self):
         params = copy.deepcopy(json.loads(self.params_json))
         runtimeparams = {
             "days_to_retrieve": 20,
             "model_type": "load_forecast",
             "var_model": "sensor.power_load_no_var_loads",
             "sklearn_model": "KNeighborsRegressor",
@@ -367,68 +462,136 @@
             "split_date_delta": '48h',
             "perform_backtest": False
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params['optim_conf']['load_forecast_method'] = 'skforecast'
         params_json = json.dumps(params)
-        with patch('sys.argv', ['main', '--action', 'forecast-model-fit', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
+        with patch('sys.argv', ['main', '--action', 'forecast-model-fit', '--config', str(emhass_conf['config_path']), 
                                 '--params', params_json, '--runtimeparams', runtimeparams_json,
                                 '--debug', 'True']):
             df_fit_pred, df_fit_pred_backtest, mlf = main()
         self.assertIsInstance(df_fit_pred, pd.DataFrame)
         self.assertTrue(df_fit_pred_backtest == None)
         
     def test_main_forecast_model_predict(self):
         params = copy.deepcopy(json.loads(self.params_json))
         runtimeparams = {
             "days_to_retrieve": 20,
             "model_type": "load_forecast",
             "var_model": "sensor.power_load_no_var_loads",
             "sklearn_model": "KNeighborsRegressor",
             "num_lags": 48,
-            "split_date_delta": '48h',
-            "perform_backtest": False
+            "split_date_delta": "48h",
+            "perform_backtest": False,
         }
         runtimeparams_json = json.dumps(runtimeparams)
-        params['passed_data'] = runtimeparams
-        params['optim_conf']['load_forecast_method'] = 'skforecast'
+        params["passed_data"] = runtimeparams
+        params["optim_conf"]["load_forecast_method"] = "skforecast"
         params_json = json.dumps(params)
-        with patch('sys.argv', ['main', '--action', 'forecast-model-predict', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
+        with patch('sys.argv', ['main', '--action', 'forecast-model-predict', '--config', str(emhass_conf['config_path']), 
                                 '--params', params_json, '--runtimeparams', runtimeparams_json,
                                 '--debug', 'True']):
             df_pred = main()
         self.assertIsInstance(df_pred, pd.Series)
         self.assertTrue(df_pred.isnull().sum().sum() == 0)
-        
+
     def test_main_forecast_model_tune(self):
         params = copy.deepcopy(json.loads(self.params_json))
         runtimeparams = {
             "days_to_retrieve": 20,
             "model_type": "load_forecast",
             "var_model": "sensor.power_load_no_var_loads",
             "sklearn_model": "KNeighborsRegressor",
             "num_lags": 48,
-            "split_date_delta": '48h',
-            "perform_backtest": False
+            "split_date_delta": "48h",
+            "perform_backtest": False,
         }
         runtimeparams_json = json.dumps(runtimeparams)
-        params['passed_data'] = runtimeparams
-        params['optim_conf']['load_forecast_method'] = 'skforecast'
+        params["passed_data"] = runtimeparams
+        params["optim_conf"]["load_forecast_method"] = "skforecast"
         params_json = json.dumps(params)
-        with patch('sys.argv', ['main', '--action', 'forecast-model-tune', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
+        with patch('sys.argv', ['main', '--action', 'forecast-model-tune', '--config', str(emhass_conf['config_path']), 
                                 '--params', params_json, '--runtimeparams', runtimeparams_json,
                                 '--debug', 'True']):
             df_pred_optim, mlf = main()
         self.assertIsInstance(df_pred_optim, pd.DataFrame)
         self.assertTrue(mlf.is_tuned == True)
+
+    def test_main_regressor_model_fit(self):
+        params = copy.deepcopy(json.loads(self.params_json))
+        runtimeparams = {
+            "csv_file": "heating_prediction.csv",
+            "features": ["degreeday", "solar"],
+            "target": "hour",
+            "regression_model": "AdaBoostRegression",
+            "model_type": "heating_hours_degreeday",
+            "timestamp": "timestamp",
+            "date_features": ["month", "day_of_week"],
+        }
+        runtimeparams_json = json.dumps(runtimeparams)
+        params["passed_data"] = runtimeparams
+        params_json = json.dumps(params)
+        with patch(
+            "sys.argv",
+            [
+                "main",
+                "--action",
+                "regressor-model-fit",
+                "--config",
+                str(emhass_conf["config_path"]),
+                "--params",
+                params_json,
+                "--runtimeparams",
+                runtimeparams_json,
+                "--debug",
+                "True",
+            ],
+        ):
+            mlr = main()
+
+    def test_main_regressor_model_predict(self):
+        params = copy.deepcopy(json.loads(self.params_json))
+        runtimeparams = {
+            "csv_file": "heating_prediction.csv",
+            "features": ["degreeday", "solar"],
+            "target": "hour",
+            "regression_model": "AdaBoostRegression",
+            "model_type": "heating_hours_degreeday",
+            "timestamp": "timestamp",
+            "date_features": ["month", "day_of_week"],
+            "new_values": [12.79, 4.766, 1, 2],
+        }
+        runtimeparams_json = json.dumps(runtimeparams)
+        params["passed_data"] = runtimeparams
+        params["optim_conf"]["load_forecast_method"] = "skforecast"
+        params_json = json.dumps(params)
+        with patch(
+            "sys.argv",
+            [
+                "main",
+                "--action",
+                "regressor-model-predict",
+                "--config",
+                str(emhass_conf["config_path"]),
+                "--params",
+                params_json,
+                "--runtimeparams",
+                runtimeparams_json,
+                "--debug",
+                "True",
+            ],
+        ):
+            prediction = main()
+        self.assertIsInstance(prediction, np.ndarray)
+
         
-    @patch('sys.argv', ['main', '--action', 'publish-data', '--config', str(pathlib.Path(root+'/config_emhass.yaml')), 
+    @patch('sys.argv', ['main', '--action', 'publish-data', '--config', str(emhass_conf['config_path']), 
                         '--debug', 'True'])
     def test_main_publish_data(self):
         opt_res = main()
-        self.assertTrue(opt_res==None)
+        self.assertFalse(opt_res.empty)
         
 if __name__ == '__main__':
     unittest.main()
     ch.close()
     logger.removeHandler(ch)
```

### Comparing `emhass-0.8.6/tests/test_forecast.py` & `emhass-0.9.0/tests/test_forecast.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 from emhass.machine_learning_forecaster import MLForecaster
 from emhass.forecast import Forecast
 from emhass.optimization import Optimization
 from emhass import utils
 
 # the root folder
 root = str(utils.get_root(__file__, num_parent=2))
+emhass_conf = {}
+emhass_conf['config_path'] = pathlib.Path(root) / 'config_emhass.yaml'
+emhass_conf['data_path'] = pathlib.Path(root) / 'data/'
+emhass_conf['root_path'] = pathlib.Path(root)
+
 # create logger
-logger, ch = utils.get_logger(__name__, root, save_to_file=False)
+logger, ch = utils.get_logger(__name__, emhass_conf, save_to_file=False)
 
 class TestForecast(unittest.TestCase):
     
     @staticmethod
     def get_test_params():
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
@@ -37,47 +42,51 @@
             }
             })
         return params
 
     def setUp(self):
         self.get_data_from_file = True
         params = None
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root) / 'config_emhass.yaml', use_secrets=False)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=False)
         self.retrieve_hass_conf, self.optim_conf, self.plant_conf = \
             retrieve_hass_conf, optim_conf, plant_conf
         self.rh = RetrieveHass(self.retrieve_hass_conf['hass_url'], self.retrieve_hass_conf['long_lived_token'], 
                                self.retrieve_hass_conf['freq'], self.retrieve_hass_conf['time_zone'],
-                               params, root, logger)
+                               params, emhass_conf, logger)
         if self.get_data_from_file:
-            with open(pathlib.Path(root) / 'data' / 'test_df_final.pkl', 'rb') as inp:
+            with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 self.rh.df_final, self.days_list, self.var_list = pickle.load(inp)
+            self.retrieve_hass_conf['var_load'] = str(self.var_list[0])
+            self.retrieve_hass_conf['var_PV'] = str(self.var_list[1])
+            self.retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            self.retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
         else:
             self.days_list = utils.get_days_list(self.retrieve_hass_conf['days_to_retrieve'])
             self.var_list = [self.retrieve_hass_conf['var_load'], self.retrieve_hass_conf['var_PV']]
             self.rh.get_data(self.days_list, self.var_list,
                             minimal_response=False, significant_changes_only=False)
         self.rh.prepare_data(self.retrieve_hass_conf['var_load'], load_negative = self.retrieve_hass_conf['load_negative'],
                              set_zero_min = self.retrieve_hass_conf['set_zero_min'], 
                              var_replace_zero = self.retrieve_hass_conf['var_replace_zero'], 
                              var_interp = self.retrieve_hass_conf['var_interp'])
         self.df_input_data = self.rh.df_final.copy()
         
         self.fcst = Forecast(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
-                             params, root, logger, get_data_from_file=self.get_data_from_file)
+                             params, emhass_conf, logger, get_data_from_file=self.get_data_from_file)
         # The default for test is csv read
         self.df_weather_scrap = self.fcst.get_weather_forecast(method='csv')
         self.P_PV_forecast = self.fcst.get_power_from_weather(self.df_weather_scrap)
         self.P_load_forecast = self.fcst.get_load_forecast(method=optim_conf['load_forecast_method'])
         self.df_input_data_dayahead = pd.concat([self.P_PV_forecast, self.P_load_forecast], axis=1)
         self.df_input_data_dayahead.columns = ['P_PV_forecast', 'P_load_forecast']
-        self.opt = Optimization(retrieve_hass_conf, optim_conf, plant_conf, 
+        self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price, 
-                                'profit', root, logger)
+                                'profit', emhass_conf, logger)
         self.input_data_dict = {
-            'root': root,
+            'emhass_conf': emhass_conf,
             'retrieve_hass_conf': self.retrieve_hass_conf,
             'df_input_data': self.df_input_data,
             'df_input_data_dayahead': self.df_input_data_dayahead,
             'opt': self.opt,
             'rh': self.rh,
             'fcst': self.fcst,
             'P_PV_forecast': self.P_PV_forecast,
@@ -102,15 +111,15 @@
         self.assertEqual(P_PV_forecast.index.tz, self.fcst.time_zone)
         self.assertEqual(len(self.df_weather_csv), len(P_PV_forecast))
         df_weather_none = self.fcst.get_weather_forecast(method='none')
         self.assertTrue(df_weather_none == None)
     
     def test_get_weather_forecast_scrapper_method_mock(self):
         with requests_mock.mock() as m:
-            data = bz2.BZ2File(str(pathlib.Path(root+'/data/test_response_scrapper_get_method.pbz2')), "rb")
+            data = bz2.BZ2File(str(emhass_conf['data_path'] / 'test_response_scrapper_get_method.pbz2'), "rb")
             data = cPickle.load(data)
             get_url = "https://clearoutside.com/forecast/"+str(round(self.fcst.lat, 2))+"/"+str(round(self.fcst.lon, 2))+"?desktop=true"
             m.get(get_url, content=data)
             df_weather_scrap = self.fcst.get_weather_forecast(method='scrapper')
             self.assertIsInstance(df_weather_scrap, type(pd.DataFrame()))
             self.assertIsInstance(df_weather_scrap.index, pd.core.indexes.datetimes.DatetimeIndex)
             self.assertIsInstance(df_weather_scrap.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
@@ -135,30 +144,30 @@
             self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
             self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
             self.assertEqual(P_PV_forecast.index.tz, self.fcst.time_zone)
             self.assertEqual(len(df_weather_scrap), len(P_PV_forecast))
 
     def test_get_weather_forecast_solcast_method_mock(self):
         with requests_mock.mock() as m:
-            data = bz2.BZ2File(str(pathlib.Path(root+'/data/test_response_solcast_get_method.pbz2')), "rb")
+            data = bz2.BZ2File(str(emhass_conf['data_path'] / 'test_response_solcast_get_method.pbz2'), "rb")
             data = cPickle.load(data)
             get_url = "https://api.solcast.com.au/rooftop_sites/123456/forecasts?hours=24"
             m.get(get_url, json=data.json())
             df_weather_scrap = self.fcst.get_weather_forecast(method='solcast')
             self.assertIsInstance(df_weather_scrap, type(pd.DataFrame()))
             self.assertIsInstance(df_weather_scrap.index, pd.core.indexes.datetimes.DatetimeIndex)
             self.assertIsInstance(df_weather_scrap.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
             self.assertEqual(df_weather_scrap.index.tz, self.fcst.time_zone)
             self.assertTrue(self.fcst.start_forecast < ts for ts in df_weather_scrap.index)
             self.assertEqual(len(df_weather_scrap), 
                             int(self.optim_conf['delta_forecast'].total_seconds()/3600/self.fcst.timeStep))
         
     def test_get_weather_forecast_solarforecast_method_mock(self):
         with requests_mock.mock() as m:
-            data = bz2.BZ2File(str(pathlib.Path(root+'/data/test_response_solarforecast_get_method.pbz2')), "rb")
+            data = bz2.BZ2File(str(emhass_conf['data_path'] / 'test_response_solarforecast_get_method.pbz2'), "rb")
             data = cPickle.load(data)
             for i in range(len(self.plant_conf['module_model'])):
                 get_url = "https://api.forecast.solar/estimate/"+str(round(self.fcst.lat, 2))+"/"+str(round(self.fcst.lon, 2))+\
                     "/"+str(self.plant_conf["surface_tilt"][i])+"/"+str(self.plant_conf["surface_azimuth"][i]-180)+\
                     "/"+str(5)
                 m.get(get_url, json=data)
                 df_weather_solarforecast = self.fcst.get_weather_forecast(method='solar.forecast')
@@ -167,15 +176,15 @@
                 self.assertIsInstance(df_weather_solarforecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
                 self.assertEqual(df_weather_solarforecast.index.tz, self.fcst.time_zone)
                 self.assertTrue(self.fcst.start_forecast < ts for ts in df_weather_solarforecast.index)
                 self.assertEqual(len(df_weather_solarforecast), 
                                 int(self.optim_conf['delta_forecast'].total_seconds()/3600/self.fcst.timeStep))
 
     def test_get_forecasts_with_lists(self):
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
@@ -188,38 +197,42 @@
             'load_power_forecast':[i+1 for i in range(48)],
             'load_cost_forecast':[i+1 for i in range(48)],
             'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, 
                                                                     use_secrets=False, params=params_json)
         set_type = "dayahead-optim"
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json, retrieve_hass_conf, 
             optim_conf, plant_conf, set_type, logger)
         rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'], 
                           retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'],
-                          params, root, logger)
+                          params, emhass_conf, logger)
         if self.get_data_from_file:
-            with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'rb') as inp:
+            with open((emhass_conf['data_path'] / 'test_df_final.pkl'), 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
+            retrieve_hass_conf['var_load'] = str(self.var_list[0])
+            retrieve_hass_conf['var_PV'] = str(self.var_list[1])
+            retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
         else:
             days_list = utils.get_days_list(retrieve_hass_conf['days_to_retrieve'])
             var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
             rh.get_data(days_list, var_list,
                         minimal_response=False, significant_changes_only=False)
         rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
                         set_zero_min = retrieve_hass_conf['set_zero_min'], 
                         var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
                         var_interp = retrieve_hass_conf['var_interp'])
         df_input_data = rh.df_final.copy()
         fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf, 
-                        params_json, root, logger, get_data_from_file=True)
+                        params_json, emhass_conf, logger, get_data_from_file=True)
         df_input_data = copy.deepcopy(df_input_data).iloc[-49:-1]
         P_PV_forecast = fcst.get_weather_forecast(method='list')
         df_input_data.index = P_PV_forecast.index
         df_input_data.index.freq = rh.df_final.index.freq
         self.assertIsInstance(P_PV_forecast, type(pd.DataFrame()))
         self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
@@ -242,15 +255,15 @@
         self.assertTrue(df_input_data['unit_load_cost'].values[-1] == 48)
         df_input_data = fcst.get_prod_price_forecast(df_input_data, method='list')
         self.assertTrue(fcst.var_prod_price in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         self.assertTrue(df_input_data['unit_prod_price'].values[0] == 1)
         self.assertTrue(df_input_data['unit_prod_price'].values[-1] == 48)
         # Test with longer lists
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
@@ -263,22 +276,22 @@
             'load_power_forecast':[i+1 for i in range(3*48)],
             'load_cost_forecast':[i+1 for i in range(3*48)],
             'prod_price_forecast':[i+1 for i in range(3*48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
-                                                                          use_secrets=False, params=params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, 
+                                                                    use_secrets=False, params=params_json)
         optim_conf['delta_forecast'] = pd.Timedelta(days=3)
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json, retrieve_hass_conf, 
             optim_conf, plant_conf, set_type, logger)
         fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf, 
-                        params_json, root, logger, get_data_from_file=True)
+                        params_json, emhass_conf, logger, get_data_from_file=True)
         P_PV_forecast = fcst.get_weather_forecast(method='list')
         self.assertIsInstance(P_PV_forecast, type(pd.DataFrame()))
         self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_PV_forecast.index.tz, fcst.time_zone)
         self.assertTrue(fcst.start_forecast < ts for ts in P_PV_forecast.index)
         self.assertTrue(P_PV_forecast.values[0][0] == 1)
@@ -302,15 +315,15 @@
         df_input_data_dayahead = fcst.get_prod_price_forecast(df_input_data_dayahead, method='list')
         self.assertTrue(fcst.var_prod_price in df_input_data_dayahead.columns)
         self.assertTrue(df_input_data_dayahead.isnull().sum().sum()==0)
         self.assertTrue(df_input_data_dayahead[fcst.var_prod_price].iloc[0] == 1)
         self.assertTrue(df_input_data_dayahead[fcst.var_prod_price].iloc[-1] == 3*48)
         
     def test_get_forecasts_with_lists_special_case(self):
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
@@ -321,38 +334,42 @@
         runtimeparams = {
             'load_cost_forecast':[i+1 for i in range(48)],
             'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, 
                                                                     use_secrets=False, params=params_json)
         set_type = "dayahead-optim"
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json, retrieve_hass_conf, 
             optim_conf, plant_conf, set_type, logger)
         rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'], 
                           retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'],
-                          params, root, logger)
+                          params, emhass_conf, logger)
         if self.get_data_from_file:
-            with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'rb') as inp:
+            with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
+            retrieve_hass_conf['var_load'] = str(self.var_list[0])
+            retrieve_hass_conf['var_PV'] = str(self.var_list[1])
+            retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
         else:
             days_list = utils.get_days_list(retrieve_hass_conf['days_to_retrieve'])
             var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
             rh.get_data(days_list, var_list,
                         minimal_response=False, significant_changes_only=False)
         rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
                         set_zero_min = retrieve_hass_conf['set_zero_min'], 
                         var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
                         var_interp = retrieve_hass_conf['var_interp'])
         df_input_data = rh.df_final.copy()
         fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf, 
-                        params_json, root, logger, get_data_from_file=True)
+                        params_json, emhass_conf, logger, get_data_from_file=True)
         df_input_data = copy.deepcopy(df_input_data).iloc[-49:-1]
         P_PV_forecast = fcst.get_weather_forecast()
         df_input_data.index = P_PV_forecast.index
         df_input_data.index.freq = rh.df_final.index.freq
         df_input_data = fcst.get_load_cost_forecast(
             df_input_data, method='list')
         self.assertTrue(fcst.var_load_cost in df_input_data.columns)
@@ -376,27 +393,27 @@
         self.plant_conf['module_model'] = [self.plant_conf['module_model'], self.plant_conf['module_model']]
         self.plant_conf['inverter_model'] = [self.plant_conf['inverter_model'], self.plant_conf['inverter_model']]
         self.plant_conf['surface_tilt'] = [30, 45]
         self.plant_conf['surface_azimuth'] = [270, 90]
         self.plant_conf['modules_per_string'] = [8, 8]
         self.plant_conf['strings_per_inverter'] = [1, 1]
         self.fcst = Forecast(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
-                             None, root, logger, get_data_from_file=self.get_data_from_file)
+                             None, emhass_conf, logger, get_data_from_file=self.get_data_from_file)
         df_weather_scrap = self.fcst.get_weather_forecast(method='csv')
         P_PV_forecast = self.fcst.get_power_from_weather(df_weather_scrap)
         self.assertIsInstance(P_PV_forecast, pd.core.series.Series)
         self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_PV_forecast.index.tz, self.fcst.time_zone)
         self.assertEqual(len(self.df_weather_scrap), len(P_PV_forecast))
         # Test the mixed forecast
         params = json.dumps({'passed_data':{'alpha':0.5,'beta':0.5}})
         df_input_data = self.input_data_dict['rh'].df_final.copy()
         self.fcst = Forecast(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
-                             params, root, logger, get_data_from_file=self.get_data_from_file)
+                             params, emhass_conf, logger, get_data_from_file=self.get_data_from_file)
         df_weather_scrap = self.fcst.get_weather_forecast(method='csv')
         P_PV_forecast = self.fcst.get_power_from_weather(df_weather_scrap, set_mix_forecast=True, df_now=df_input_data)
         self.assertIsInstance(P_PV_forecast, pd.core.series.Series)
         self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_PV_forecast.index.tz, self.fcst.time_zone)
         self.assertEqual(len(self.df_weather_scrap), len(P_PV_forecast))
@@ -409,15 +426,15 @@
         self.assertEqual(P_load_forecast.index.tz, self.fcst.time_zone)
         self.assertEqual(len(self.P_PV_forecast), len(P_load_forecast))
         print(">> The length of the load forecast = "+str(len(P_load_forecast)))
         # Test the mixed forecast
         params = json.dumps({'passed_data':{'alpha':0.5,'beta':0.5}})
         df_input_data = self.input_data_dict['rh'].df_final.copy()
         self.fcst = Forecast(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
-                             params, root, logger, get_data_from_file=self.get_data_from_file)
+                             params, emhass_conf, logger, get_data_from_file=self.get_data_from_file)
         P_load_forecast = self.fcst.get_load_forecast(set_mix_forecast=True, df_now=df_input_data)
         self.assertIsInstance(P_load_forecast, pd.core.series.Series)
         self.assertIsInstance(P_load_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_load_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_load_forecast.index.tz, self.fcst.time_zone)
         self.assertEqual(len(self.P_PV_forecast), len(P_load_forecast))
         # Test load forecast from csv
@@ -427,38 +444,36 @@
         self.assertIsInstance(P_load_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_load_forecast.index.tz, self.fcst.time_zone)
         self.assertEqual(len(self.P_PV_forecast), len(P_load_forecast))
         
     def test_get_load_forecast_mlforecaster(self):
         params = TestForecast.get_test_params()
         params_json = json.dumps(params)
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'forecast-model-fit' # fit, predict and tune methods
         params = copy.deepcopy(json.loads(params_json))
         runtimeparams = {
             "days_to_retrieve": 20,
             "model_type": "load_forecast",
             "var_model": "sensor.power_load_no_var_loads",
             "sklearn_model": "KNeighborsRegressor",
             "num_lags": 48
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params['optim_conf']['load_forecast_method'] = 'mlforecaster'
         params_json = json.dumps(params)
-        input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                               action, logger, get_data_from_file=True)
         data = copy.deepcopy(input_data_dict['df_input_data'])
         model_type = input_data_dict['params']['passed_data']['model_type']
         var_model = input_data_dict['params']['passed_data']['var_model']
         sklearn_model = input_data_dict['params']['passed_data']['sklearn_model']
         num_lags = input_data_dict['params']['passed_data']['num_lags']
-        mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, root, logger)
+        mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, emhass_conf, logger)
         mlf.fit()
         P_load_forecast = input_data_dict['fcst'].get_load_forecast(method="mlforecaster", use_last_window=False, 
                                                                     debug=True, mlf=mlf)
         self.assertIsInstance(P_load_forecast, pd.core.series.Series)
         self.assertIsInstance(P_load_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_load_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_load_forecast.index.tz, self.fcst.time_zone)
@@ -466,24 +481,24 @@
         self.assertEqual(len(self.P_PV_forecast), len(P_load_forecast))
         
     def test_get_load_cost_forecast(self):
         df_input_data = self.fcst.get_load_cost_forecast(self.df_input_data)
         self.assertTrue(self.fcst.var_load_cost in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         df_input_data = self.fcst.get_load_cost_forecast(self.df_input_data, method='csv',
-                                                         csv_path='/data/data_load_cost_forecast.csv')
+                                                         csv_path='data_load_cost_forecast.csv')
         self.assertTrue(self.fcst.var_load_cost in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         
     def test_get_prod_price_forecast(self):
         df_input_data = self.fcst.get_prod_price_forecast(self.df_input_data)
         self.assertTrue(self.fcst.var_prod_price in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         df_input_data = self.fcst.get_prod_price_forecast(self.df_input_data, method='csv',
-                                                          csv_path='/data/data_load_cost_forecast.csv')
+                                                          csv_path='data_load_cost_forecast.csv')
         self.assertTrue(self.fcst.var_prod_price in df_input_data.columns)
         self.assertTrue(df_input_data.isnull().sum().sum()==0)
         
 if __name__ == '__main__':
     unittest.main()
     ch.close()
     logger.removeHandler(ch)
```

### Comparing `emhass-0.8.6/tests/test_machine_learning_forecaster.py` & `emhass-0.9.0/tests/test_machine_learning_forecaster.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,27 @@
 from emhass.command_line import set_input_data_dict
 from emhass.retrieve_hass import RetrieveHass
 from emhass.machine_learning_forecaster import MLForecaster
 from emhass import utils
 
 # the root folder
 root = str(utils.get_root(__file__, num_parent=2))
+emhass_conf = {}
+emhass_conf['config_path'] = pathlib.Path(root) / 'config_emhass.yaml'
+emhass_conf['data_path'] = pathlib.Path(root) / 'data/'
+emhass_conf['root_path'] = pathlib.Path(root)
+
 # create logger
-logger, ch = utils.get_logger(__name__, root, save_to_file=False)
+logger, ch = utils.get_logger(__name__, emhass_conf, save_to_file=False)
 
 class TestMLForecaster(unittest.TestCase):
     
     @staticmethod
     def get_test_params():
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
@@ -40,46 +45,44 @@
             }
             })
         return params
 
     def setUp(self):
         params = TestMLForecaster.get_test_params()
         params_json = json.dumps(params)
-        config_path = pathlib.Path(root+'/config_emhass.yaml')
-        base_path = str(config_path.parent)
         costfun = 'profit'
         action = 'forecast-model-fit' # fit, predict and tune methods
         params = copy.deepcopy(json.loads(params_json))
         runtimeparams = {
             "days_to_retrieve": 20,
             "model_type": "load_forecast",
             "var_model": "sensor.power_load_no_var_loads",
             "sklearn_model": "KNeighborsRegressor",
             "num_lags": 48
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params['optim_conf']['load_forecast_method'] = 'skforecast'
         params_json = json.dumps(params)
-        self.input_data_dict = set_input_data_dict(config_path, base_path, costfun, params_json, runtimeparams_json, 
+        self.input_data_dict = set_input_data_dict(emhass_conf, costfun, params_json, runtimeparams_json, 
                                                    action, logger, get_data_from_file=True)
         data = copy.deepcopy(self.input_data_dict['df_input_data'])
         model_type = self.input_data_dict['params']['passed_data']['model_type']
         var_model = self.input_data_dict['params']['passed_data']['var_model']
         sklearn_model = self.input_data_dict['params']['passed_data']['sklearn_model']
         num_lags = self.input_data_dict['params']['passed_data']['num_lags']
-        self.mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, root, logger)
+        self.mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, emhass_conf, logger)
         
         get_data_from_file = True
         params = None
-        self.retrieve_hass_conf, self.optim_conf, _ = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), use_secrets=False)
+        self.retrieve_hass_conf, self.optim_conf, _ = utils.get_yaml_parse(emhass_conf, use_secrets=False)
         self.rh = RetrieveHass(self.retrieve_hass_conf['hass_url'], self.retrieve_hass_conf['long_lived_token'], 
                                self.retrieve_hass_conf['freq'], self.retrieve_hass_conf['time_zone'],
-                               params, root, logger, get_data_from_file=get_data_from_file)
-        with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'rb') as inp:
+                               params, emhass_conf, logger, get_data_from_file=get_data_from_file)
+        with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
             self.rh.df_final, self.days_list, self.var_list = pickle.load(inp)
         
     def test_fit(self):
         df_pred, df_pred_backtest = self.mlf.fit()
         self.assertIsInstance(self.mlf.forecaster, ForecasterAutoreg)
         self.assertIsInstance(df_pred, pd.DataFrame)
         self.assertTrue(df_pred_backtest == None)
@@ -122,26 +125,26 @@
         self.assertTrue(self.mlf.is_tuned == True)
         # Test LinearRegression
         data = copy.deepcopy(self.input_data_dict['df_input_data'])
         model_type = self.input_data_dict['params']['passed_data']['model_type']
         var_model = self.input_data_dict['params']['passed_data']['var_model']
         sklearn_model = 'LinearRegression'
         num_lags = self.input_data_dict['params']['passed_data']['num_lags']
-        self.mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, root, logger)
+        self.mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, emhass_conf, logger)
         self.mlf.fit()
         df_pred_optim = self.mlf.tune(debug=True)
         self.assertIsInstance(df_pred_optim, pd.DataFrame)
         self.assertTrue(self.mlf.is_tuned == True)
         # Test ElasticNet
         data = copy.deepcopy(self.input_data_dict['df_input_data'])
         model_type = self.input_data_dict['params']['passed_data']['model_type']
         var_model = self.input_data_dict['params']['passed_data']['var_model']
         sklearn_model = 'ElasticNet'
         num_lags = self.input_data_dict['params']['passed_data']['num_lags']
-        self.mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, root, logger)
+        self.mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, emhass_conf, logger)
         self.mlf.fit()
         df_pred_optim = self.mlf.tune(debug=True)
         self.assertIsInstance(df_pred_optim, pd.DataFrame)
         self.assertTrue(self.mlf.is_tuned == True)
         
         
 if __name__ == '__main__':
```

### Comparing `emhass-0.8.6/tests/test_optimization.py` & `emhass-0.9.0/tests/test_optimization.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,54 +12,62 @@
 from emhass.retrieve_hass import RetrieveHass
 from emhass.optimization import Optimization
 from emhass.forecast import Forecast
 from emhass.utils import get_root, get_yaml_parse, get_days_list, get_logger
 
 # the root folder
 root = str(get_root(__file__, num_parent=2))
+emhass_conf = {}
+emhass_conf['config_path'] = pathlib.Path(root) / 'config_emhass.yaml'
+emhass_conf['data_path'] = pathlib.Path(root) / 'data/'
+emhass_conf['root_path'] = pathlib.Path(root)
 # create logger
-logger, ch = get_logger(__name__, root, save_to_file=False)
+logger, ch = get_logger(__name__, emhass_conf, save_to_file=False)
 
 class TestOptimization(unittest.TestCase):
 
     def setUp(self):
         get_data_from_file = True
         params = None
-        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), use_secrets=False)
+        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(emhass_conf, use_secrets=False)
         self.retrieve_hass_conf, self.optim_conf, self.plant_conf = \
             retrieve_hass_conf, optim_conf, plant_conf
         self.rh = RetrieveHass(self.retrieve_hass_conf['hass_url'], self.retrieve_hass_conf['long_lived_token'], 
                                self.retrieve_hass_conf['freq'], self.retrieve_hass_conf['time_zone'],
-                               params, root, logger)
+                               params, emhass_conf, logger)
         if get_data_from_file:
-            with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'rb') as inp:
+            with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 self.rh.df_final, self.days_list, self.var_list = pickle.load(inp)
+            self.retrieve_hass_conf['var_load'] = str(self.var_list[0])
+            self.retrieve_hass_conf['var_PV'] = str(self.var_list[1])
+            self.retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            self.retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
         else:
             self.days_list = get_days_list(self.retrieve_hass_conf['days_to_retrieve'])
             self.var_list = [self.retrieve_hass_conf['var_load'], self.retrieve_hass_conf['var_PV']]
             self.rh.get_data(self.days_list, self.var_list,
                             minimal_response=False, significant_changes_only=False)
         self.rh.prepare_data(self.retrieve_hass_conf['var_load'], load_negative = self.retrieve_hass_conf['load_negative'],
                              set_zero_min = self.retrieve_hass_conf['set_zero_min'], 
                              var_replace_zero = self.retrieve_hass_conf['var_replace_zero'], 
                              var_interp = self.retrieve_hass_conf['var_interp'])
         self.df_input_data = self.rh.df_final.copy()
         
         self.fcst = Forecast(self.retrieve_hass_conf, self.optim_conf, self.plant_conf,
-                             params, root, logger, get_data_from_file=get_data_from_file)
+                             params, emhass_conf, logger, get_data_from_file=get_data_from_file)
         self.df_weather = self.fcst.get_weather_forecast(method='csv')
         self.P_PV_forecast = self.fcst.get_power_from_weather(self.df_weather)
         self.P_load_forecast = self.fcst.get_load_forecast(method=optim_conf['load_forecast_method'])
         self.df_input_data_dayahead = pd.concat([self.P_PV_forecast, self.P_load_forecast], axis=1)
         self.df_input_data_dayahead.columns = ['P_PV_forecast', 'P_load_forecast']
         
         self.costfun = 'profit'
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.df_input_data = self.fcst.get_load_cost_forecast(self.df_input_data)
         self.df_input_data = self.fcst.get_prod_price_forecast(self.df_input_data)
         self.input_data_dict = {
             'retrieve_hass_conf': retrieve_hass_conf,
         }
         
     def test_perform_perfect_forecast_optim(self):
@@ -83,80 +91,80 @@
         # Test the battery, dynamics and grid exchange contraints
         self.optim_conf.update({'set_use_battery': True})
         self.optim_conf.update({'set_nocharge_from_grid': True})
         self.optim_conf.update({'set_battery_dynamic': True})
         self.optim_conf.update({'set_nodischarge_to_grid': True})
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertIsInstance(self.opt_res_dayahead, type(pd.DataFrame()))
         self.assertTrue('P_batt' in self.opt_res_dayahead.columns)
         self.assertTrue('SOC_opt' in self.opt_res_dayahead.columns)
         self.assertAlmostEqual(self.opt_res_dayahead.loc[self.opt_res_dayahead.index[-1],'SOC_opt'], self.plant_conf['SOCtarget'])
         # Test table conversion
-        opt_res = pd.read_csv(root+'/data/opt_res_latest.csv', index_col='timestamp')
+        opt_res = pd.read_csv(emhass_conf['data_path'] / 'opt_res_latest.csv', index_col='timestamp')
         cost_cols = [i for i in opt_res.columns if 'cost_' in i]
         table = opt_res[cost_cols].reset_index().sum(numeric_only=True).to_frame(name='Cost Totals').reset_index()
         self.assertTrue(table.columns[0]=='index')
         self.assertTrue(table.columns[1]=='Cost Totals')
         # Check status
         self.assertTrue('optim_status' in self.opt_res_dayahead.columns)
         # Test treat_def_as_semi_cont and set_def_constant constraints
         self.optim_conf.update({'treat_def_as_semi_cont': [True, True]})
         self.optim_conf.update({'set_def_constant': [True, True]})
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertTrue(self.opt.optim_status == 'Optimal')
         self.optim_conf.update({'treat_def_as_semi_cont': [False, True]})
         self.optim_conf.update({'set_def_constant': [True, True]})
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertTrue(self.opt.optim_status == 'Optimal')
         self.optim_conf.update({'treat_def_as_semi_cont': [False, True]})
         self.optim_conf.update({'set_def_constant': [False, True]})
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertTrue(self.opt.optim_status == 'Optimal')
         self.optim_conf.update({'treat_def_as_semi_cont': [False, False]})
         self.optim_conf.update({'set_def_constant': [False, True]})
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertTrue(self.opt.optim_status == 'Optimal')
         self.optim_conf.update({'treat_def_as_semi_cont': [False, False]})
         self.optim_conf.update({'set_def_constant': [False, False]})
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertTrue(self.opt.optim_status == 'Optimal')
         # Test with different default solver, debug mode and batt SOC conditions
         del self.optim_conf['lp_solver']
         del self.optim_conf['lp_solver_path']
         self.optim_conf['set_use_battery'] = True
         soc_init = None
         soc_final = 0.3
         self.optim_conf['set_total_pv_sell'] = True
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         
         unit_load_cost = self.df_input_data_dayahead[self.opt.var_load_cost].values
         unit_prod_price = self.df_input_data_dayahead[self.opt.var_prod_price].values
         self.opt_res_dayahead = self.opt.perform_optimization(
             self.df_input_data_dayahead, self.P_PV_forecast.values.ravel(), 
             self.P_load_forecast.values.ravel(), unit_load_cost, unit_prod_price,
             soc_init = soc_init, soc_final = soc_final, debug = True)
@@ -166,29 +174,29 @@
         self.assertTrue('cost_fun_'+self.costfun in self.opt_res_dayahead.columns)
         self.assertTrue(self.opt.optim_status == 'Optimal')
         
     def test_perform_dayahead_forecast_optim_costfun_selfconso(self):
         costfun = 'self-consumption'
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                costfun, root, logger)
+                                costfun, emhass_conf, logger)
         self.df_input_data_dayahead = self.fcst.get_load_cost_forecast(self.df_input_data_dayahead)
         self.df_input_data_dayahead = self.fcst.get_prod_price_forecast(self.df_input_data_dayahead)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertIsInstance(self.opt_res_dayahead, type(pd.DataFrame()))
         self.assertIsInstance(self.opt_res_dayahead.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(self.opt_res_dayahead.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertTrue('cost_fun_selfcons' in self.opt_res_dayahead.columns)
         
     def test_perform_dayahead_forecast_optim_costfun_cost(self):
         costfun = 'cost'
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                costfun, root, logger)
+                                costfun, emhass_conf, logger)
         self.df_input_data_dayahead = self.fcst.get_load_cost_forecast(self.df_input_data_dayahead)
         self.df_input_data_dayahead = self.fcst.get_prod_price_forecast(self.df_input_data_dayahead)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertIsInstance(self.opt_res_dayahead, type(pd.DataFrame()))
         self.assertIsInstance(self.opt_res_dayahead.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(self.opt_res_dayahead.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
@@ -196,15 +204,15 @@
         
     def test_perform_dayahead_forecast_optim_aux(self):
         self.optim_conf['treat_def_as_semi_cont'] = [False, False]
         self.optim_conf['set_total_pv_sell'] = True
         self.optim_conf['set_def_constant'] = [True, True]
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         self.df_input_data_dayahead = self.fcst.get_load_cost_forecast(self.df_input_data_dayahead)
         self.df_input_data_dayahead = self.fcst.get_prod_price_forecast(self.df_input_data_dayahead)
         self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
             self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
         self.assertIsInstance(self.opt_res_dayahead, type(pd.DataFrame()))
         self.assertIsInstance(self.opt_res_dayahead.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(self.opt_res_dayahead.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
@@ -212,15 +220,15 @@
         solver_list = pl.listSolvers(onlyAvailable=True)
         for solver in solver_list:
             self.optim_conf['lp_solver'] = solver
             if os.getenv("LP_SOLVER_PATH", default=None) == None:
                 self.optim_conf['lp_solver_path'] = os.getenv("LP_SOLVER_PATH", default=None)            
             self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                     self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                    self.costfun, root, logger)
+                                    self.costfun, emhass_conf, logger)
             self.df_input_data_dayahead = self.fcst.get_load_cost_forecast(self.df_input_data_dayahead)
             self.df_input_data_dayahead = self.fcst.get_prod_price_forecast(self.df_input_data_dayahead)
             self.opt_res_dayahead = self.opt.perform_dayahead_forecast_optim(
                 self.df_input_data_dayahead, self.P_PV_forecast, self.P_load_forecast)
             self.assertIsInstance(self.opt_res_dayahead, type(pd.DataFrame()))
             self.assertIsInstance(self.opt_res_dayahead.index, pd.core.indexes.datetimes.DatetimeIndex)
             self.assertIsInstance(self.opt_res_dayahead.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
@@ -228,15 +236,15 @@
     def test_perform_naive_mpc_optim(self):
         self.df_input_data_dayahead = self.fcst.get_load_cost_forecast(self.df_input_data_dayahead)
         self.df_input_data_dayahead = self.fcst.get_prod_price_forecast(self.df_input_data_dayahead)
         # Test the battery
         self.optim_conf.update({'set_use_battery': True})
         self.opt = Optimization(self.retrieve_hass_conf, self.optim_conf, self.plant_conf, 
                                 self.fcst.var_load_cost, self.fcst.var_prod_price,  
-                                self.costfun, root, logger)
+                                self.costfun, emhass_conf, logger)
         prediction_horizon = 10
         soc_init = 0.4
         soc_final = 0.6
         def_total_hours = [2, 3]
         def_start_timestep = [-5, 0]
         def_end_timestep = [4, 0]
         self.opt_res_dayahead = self.opt.perform_naive_mpc_optim(
```

### Comparing `emhass-0.8.6/tests/test_retrieve_hass.py` & `emhass-0.9.0/tests/test_retrieve_hass.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,66 +10,78 @@
 import pickle as cPickle
 
 from emhass.retrieve_hass import RetrieveHass
 from emhass.utils import get_root, get_yaml_parse, get_days_list, get_logger
 
 # the root folder
 root = str(get_root(__file__, num_parent=2))
+emhass_conf = {}
+emhass_conf['config_path'] = pathlib.Path(root) / 'config_emhass.yaml'
+emhass_conf['data_path'] = pathlib.Path(root) / 'data/'
+emhass_conf['root_path'] = pathlib.Path(root)
+
 # create logger
-logger, ch = get_logger(__name__, root, save_to_file=False)
+logger, ch = get_logger(__name__, emhass_conf, save_to_file=False)
 
 class TestRetrieveHass(unittest.TestCase):
 
     def setUp(self):
         get_data_from_file = True
         save_data_to_file = False
         params = None
-        retrieve_hass_conf, _, _ = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), use_secrets=False)
+        retrieve_hass_conf, _, _ = get_yaml_parse(emhass_conf, use_secrets=False)
+        
+        #Force config params for testing
+        retrieve_hass_conf['var_PV'] = 'sensor.power_photovoltaics'
+        retrieve_hass_conf['var_load'] = 'sensor.power_load_no_var_loads'
+        retrieve_hass_conf['var_replace_zero'] = ['sensor.power_photovoltaics']
+        retrieve_hass_conf['var_interp'] = ['sensor.power_photovoltaics','sensor.power_load_no_var_loads'] 
+        
         self.retrieve_hass_conf = retrieve_hass_conf
         self.rh = RetrieveHass(self.retrieve_hass_conf['hass_url'], self.retrieve_hass_conf['long_lived_token'], 
                                self.retrieve_hass_conf['freq'], self.retrieve_hass_conf['time_zone'],
-                               params, root, logger, get_data_from_file=get_data_from_file)
+                               params, emhass_conf, logger, get_data_from_file=get_data_from_file)
         if get_data_from_file:
-            with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'rb') as inp:
+            with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 self.rh.df_final, self.days_list, self.var_list = pickle.load(inp)
         else:
             self.days_list = get_days_list(self.retrieve_hass_conf['days_to_retrieve'])
             self.var_list = [self.retrieve_hass_conf['var_load'], self.retrieve_hass_conf['var_PV']]
             self.rh.get_data(self.days_list, self.var_list,
                              minimal_response=False, significant_changes_only=False)
             if save_data_to_file:
-                with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'wb') as outp:
+                with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'wb') as outp:
                     pickle.dump((self.rh.df_final, self.days_list, self.var_list), 
                                 outp, pickle.HIGHEST_PROTOCOL)
         self.df_raw = self.rh.df_final.copy()
         
     def test_get_yaml_parse(self):
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
                 'lon': 6.86,
                 'alt': 4807.8
             }
             })
         params = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
+        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(emhass_conf, 
                                                                     use_secrets=True, params=params)
         self.assertIsInstance(retrieve_hass_conf, dict)
         self.assertTrue('hass_url' in retrieve_hass_conf.keys())
         self.assertTrue(retrieve_hass_conf['hass_url'] == 'http://supervisor/core/api')
         self.assertIsInstance(optim_conf, dict)
         self.assertIsInstance(plant_conf, dict)
     
     def test_yaml_parse_wab_server(self):
-        with open(pathlib.Path(root) / "config_emhass.yaml", 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             config = yaml.load(file, Loader=yaml.FullLoader)
         retrieve_hass_conf = config['retrieve_hass_conf']
         optim_conf = config['optim_conf']
         plant_conf = config['plant_conf']
         params = {}
         params['retrieve_hass_conf'] = retrieve_hass_conf
         params['optim_conf'] = optim_conf
@@ -86,15 +98,15 @@
         response = self.rh.get_data(days_list, var_list)
         self.assertFalse(response)
 
     def test_get_data_mock(self):
         with requests_mock.mock() as m:
             days_list = get_days_list(1)
             var_list = [self.retrieve_hass_conf['var_load']]
-            data = bz2.BZ2File(str(pathlib.Path(root+'/data/test_response_get_data_get_method.pbz2')), "rb")
+            data = bz2.BZ2File(str(emhass_conf['data_path'] / 'test_response_get_data_get_method.pbz2'), "rb")
             data = cPickle.load(data)
             m.get(self.retrieve_hass_conf['hass_url'], json=data.json())
             self.rh.get_data(days_list, var_list,
                              minimal_response=False, significant_changes_only=False,
                              test_url=self.retrieve_hass_conf['hass_url'])
             self.assertIsInstance(self.rh.df_final, type(pd.DataFrame()))
             self.assertIsInstance(self.rh.df_final.index, pd.core.indexes.datetimes.DatetimeIndex)
```

### Comparing `emhass-0.8.6/tests/test_utils.py` & `emhass-0.9.0/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,27 @@
 import pandas as pd
 import pathlib, json, yaml, copy
 
 from emhass import utils
 
 # the root folder
 root = str(utils.get_root(__file__, num_parent=2))
+emhass_conf = {}
+emhass_conf['config_path'] = pathlib.Path(root) / 'config_emhass.yaml'
+emhass_conf['data_path'] = pathlib.Path(root) / 'data/'
+emhass_conf['root_path'] = pathlib.Path(root)
+
 # create logger
-logger, ch = utils.get_logger(__name__, root, save_to_file=False)
+logger, ch = utils.get_logger(__name__, emhass_conf, save_to_file=False)
 
 class TestCommandLineUtils(unittest.TestCase):
     
     @staticmethod
     def get_test_params():
-        with open(root+'/config_emhass.yaml', 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
                 'long_lived_token': '${SUPERVISOR_TOKEN}',
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
@@ -43,33 +48,32 @@
         params['optim_conf']['weather_forecast_method'] = 'list'
         params['optim_conf']['load_forecast_method'] = 'list'
         params['optim_conf']['load_cost_forecast_method'] = 'list'
         params['optim_conf']['prod_price_forecast_method'] = 'list'
         self.params_json = json.dumps(params)
         
     def test_get_yaml_parse(self):
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), use_secrets=False)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=False)
         self.assertIsInstance(retrieve_hass_conf, dict)
         self.assertIsInstance(optim_conf, dict)
         self.assertIsInstance(plant_conf, dict)
         self.assertTrue(retrieve_hass_conf['alt'] == 4807.8)
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), use_secrets=True, params=self.params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=True, params=self.params_json)
         self.assertTrue(retrieve_hass_conf['alt'] == 8000.0)
         
     def test_get_forecast_dates(self):
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), use_secrets=True, params=self.params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=True, params=self.params_json)
         freq = int(retrieve_hass_conf['freq'].seconds/60.0)
         delta_forecast = int(optim_conf['delta_forecast'].days)
         forecast_dates = utils.get_forecast_dates(freq, delta_forecast)
         self.assertIsInstance(forecast_dates, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertTrue(len(forecast_dates)==int(delta_forecast*60*24/freq))
         
     def test_treat_runtimeparams(self):
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(
-            pathlib.Path(root+'/config_emhass.yaml'), use_secrets=True, params=self.params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=True, params=self.params_json)
         set_type = 'dayahead-optim'
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             self.runtimeparams_json, self.params_json,
             retrieve_hass_conf, optim_conf, plant_conf, set_type, logger)
         self.assertIsInstance(params, str)
         params = json.loads(params)
         self.assertIsInstance(params['passed_data']['pv_power_forecast'], list)
@@ -87,16 +91,15 @@
         self.assertIsInstance(params, str)
         params = json.loads(params)
         self.assertTrue(params['passed_data']['prediction_horizon'] == 10)
         self.assertTrue(params['passed_data']['soc_init'] == plant_conf['SOCtarget'])
         self.assertTrue(params['passed_data']['soc_final'] == plant_conf['SOCtarget'])
         self.assertTrue(params['passed_data']['def_total_hours'] == optim_conf['def_total_hours'])
         # This will be the case when using emhass in standalone mode
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(
-            pathlib.Path(root+'/config_emhass.yaml'), use_secrets=True, params=self.params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=True, params=self.params_json)
         params = json.dumps(None)
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             self.runtimeparams_json, params,
             retrieve_hass_conf, optim_conf, plant_conf, set_type, logger)
         self.assertIsInstance(params, str)
         params = json.loads(params)
         self.assertIsInstance(params['passed_data']['pv_power_forecast'], list)
@@ -128,16 +131,15 @@
         runtimeparams.update({'custom_grid_forecast_id':'my_custom_grid_forecast_id'})
         runtimeparams.update({'custom_cost_fun_id':'my_custom_cost_fun_id'})
         runtimeparams.update({'custom_optim_status_id':'my_custom_optim_status_id'})
         runtimeparams.update({'custom_unit_load_cost_id':'my_custom_unit_load_cost_id'})
         runtimeparams.update({'custom_unit_prod_price_id':'my_custom_unit_prod_price_id'})
         runtimeparams.update({'custom_deferrable_forecast_id':'my_custom_deferrable_forecast_id'})
         runtimeparams_json = json.dumps(runtimeparams)
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(
-            pathlib.Path(root+'/config_emhass.yaml'), use_secrets=True, params=self.params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=True, params=self.params_json)
         set_type = 'dayahead-optim'
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, self.params_json,
             retrieve_hass_conf, optim_conf, plant_conf, set_type, logger)
         self.assertIsInstance(params, str)
         params = json.loads(params)
         self.assertIsInstance(params['passed_data']['pv_power_forecast'], list)
@@ -178,16 +180,15 @@
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params['optim_conf']['weather_forecast_method'] = 'list'
         params['optim_conf']['load_forecast_method'] = 'list'
         params['optim_conf']['load_cost_forecast_method'] = 'list'
         params['optim_conf']['prod_price_forecast_method'] = 'list'
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(
-            pathlib.Path(root+'/config_emhass.yaml'), use_secrets=True, params=params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=True, params=params_json)
         set_type = 'dayahead-optim'
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json,
             retrieve_hass_conf, optim_conf, plant_conf, set_type, logger)
         params = json.loads(params)
         runtimeparams = json.loads(runtimeparams_json)
         self.assertTrue(len([x for x in runtimeparams['pv_power_forecast'] if not str(x).isdigit()])>0)
@@ -204,43 +205,41 @@
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params['optim_conf']['weather_forecast_method'] = 'list'
         params['optim_conf']['load_forecast_method'] = 'list'
         params['optim_conf']['load_cost_forecast_method'] = 'list'
         params['optim_conf']['prod_price_forecast_method'] = 'list'
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(
-            pathlib.Path(root+'/config_emhass.yaml'), use_secrets=True, params=params_json)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(emhass_conf, use_secrets=True, params=params_json)
         set_type = 'dayahead-optim'
         params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json,
             retrieve_hass_conf, optim_conf, plant_conf, set_type, logger)
         params = json.loads(params)
         runtimeparams = json.loads(runtimeparams_json)
         self.assertIsInstance(runtimeparams['pv_power_forecast'], str)
         self.assertIsInstance(runtimeparams['load_power_forecast'], str)
         self.assertIsInstance(runtimeparams['load_cost_forecast'], str)
         self.assertIsInstance(runtimeparams['prod_price_forecast'], str)
     
     def test_build_params(self):
-        config_path = root / pathlib.Path("config_emhass.yaml")
-        with open(config_path, 'r') as file:
+        with open(emhass_conf['config_path'], 'r') as file:
             config = yaml.load(file, Loader=yaml.FullLoader)
         retrieve_hass_conf = config['retrieve_hass_conf']
         optim_conf = config['optim_conf']
         plant_conf = config['plant_conf']
         params = {}
         params['retrieve_hass_conf'] = retrieve_hass_conf
         params['optim_conf'] = optim_conf
         params['plant_conf'] = plant_conf
-        options_json = root / pathlib.Path("options.json")
+        options_json = emhass_conf['root_path'] / "options.json"
         # Read options info
         with options_json.open('r') as data:
             options = json.load(data)
-        with open(root / pathlib.Path("secrets_emhass(example).yaml"), 'r') as file:
+        with open(emhass_conf['root_path'] / "secrets_emhass(example).yaml", 'r') as file:
             params_secrets = yaml.load(file, Loader=yaml.FullLoader)
         addon = 1
         params = utils.build_params(params, params_secrets, options, addon, logger)
         expected_keys = ['retrieve_hass_conf', 'params_secrets', 'optim_conf', 'plant_conf', 'passed_data']
         for key in expected_keys:
             self.assertTrue(key in params.keys())
         self.assertTrue(params['params_secrets']['time_zone'] == "Europe/Paris")
```

