# Comparing `tmp/cvxportfolio-1.3.1.tar.gz` & `tmp/cvxportfolio-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-1.3.1.tar", last modified: Mon Apr 15 19:13:29 2024, max compression
+gzip compressed data, was "cvxportfolio-1.3.2.tar", last modified: Fri May 10 05:07:00 2024, max compression
```

## Comparing `cvxportfolio-1.3.1.tar` & `cvxportfolio-1.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/
--rw-r--r--   0 enzo      (1000) enzo      (1000)      199 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/AUTHORS
--rw-r--r--   0 enzo      (1000) enzo      (1000)    11358 2023-12-13 09:54:59.000000 cvxportfolio-1.3.1/LICENSE
--rw-r--r--   0 enzo      (1000) enzo      (1000)    13950 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/PKG-INFO
--rw-r--r--   0 enzo      (1000) enzo      (1000)    12599 2024-04-06 09:38:48.000000 cvxportfolio-1.3.1/README.rst
-drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/
--rw-r--r--   0 enzo      (1000) enzo      (1000)     1013 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/__init__.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     3174 2024-04-04 19:18:10.000000 cvxportfolio-1.3.1/cvxportfolio/cache.py
-drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/constraints/
--rw-r--r--   0 enzo      (1000) enzo      (1000)     1678 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/constraints/__init__.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     5548 2024-04-02 16:10:25.000000 cvxportfolio-1.3.1/cvxportfolio/constraints/base_constraints.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    35921 2024-04-04 17:26:07.000000 cvxportfolio-1.3.1/cvxportfolio/constraints/constraints.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    42653 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/costs.py
-drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/data/
--rw-r--r--   0 enzo      (1000) enzo      (1000)     1102 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/data/__init__.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    35784 2024-04-06 09:18:10.000000 cvxportfolio-1.3.1/cvxportfolio/data/market_data.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    51122 2024-04-04 19:45:16.000000 cvxportfolio-1.3.1/cvxportfolio/data/symbol_data.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     2385 2024-03-16 05:48:22.000000 cvxportfolio-1.3.1/cvxportfolio/errors.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    30419 2024-04-04 17:32:53.000000 cvxportfolio-1.3.1/cvxportfolio/estimator.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    48403 2024-03-22 08:30:04.000000 cvxportfolio-1.3.1/cvxportfolio/forecast.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     7981 2024-04-04 17:24:49.000000 cvxportfolio-1.3.1/cvxportfolio/hyperparameters.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    38894 2024-04-06 07:46:09.000000 cvxportfolio-1.3.1/cvxportfolio/policies.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    37195 2024-04-04 17:33:55.000000 cvxportfolio-1.3.1/cvxportfolio/result.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    11062 2024-04-02 16:10:25.000000 cvxportfolio-1.3.1/cvxportfolio/returns.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    21541 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/risks.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    32701 2024-03-31 17:12:52.000000 cvxportfolio-1.3.1/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio/tests/
--rw-r--r--   0 enzo      (1000) enzo      (1000)     6099 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     1285 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/__main__.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)   156730 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo      (1000) enzo      (1000)   149356 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo      (1000) enzo      (1000)    14857 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    12037 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    50193 2024-04-04 19:56:22.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    14443 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    27339 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     6249 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_hyperparameters.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    31934 2024-04-04 18:04:07.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     9101 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_result.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     4779 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     9985 2024-04-03 14:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)    46115 2024-04-04 19:23:59.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)     3389 2024-04-04 15:00:04.000000 cvxportfolio-1.3.1/cvxportfolio/tests/test_utils.py
--rw-r--r--   0 enzo      (1000) enzo      (1000)   116620 2023-10-14 06:46:10.000000 cvxportfolio-1.3.1/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo      (1000) enzo      (1000)     6364 2024-04-04 17:26:30.000000 cvxportfolio-1.3.1/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/cvxportfolio.egg-info/
--rw-r--r--   0 enzo      (1000) enzo      (1000)    13950 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo      (1000) enzo      (1000)     1337 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo      (1000) enzo      (1000)        1 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo      (1000) enzo      (1000)      231 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo      (1000) enzo      (1000)       13 2024-04-15 19:13:29.000000 cvxportfolio-1.3.1/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo      (1000) enzo      (1000)     2753 2024-04-15 19:06:41.000000 cvxportfolio-1.3.1/pyproject.toml
--rw-r--r--   0 enzo      (1000) enzo      (1000)       38 2024-04-15 19:13:29.181006 cvxportfolio-1.3.1/setup.cfg
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)      199 2023-10-14 06:46:10.000000 cvxportfolio-1.3.2/AUTHORS
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    11358 2023-12-13 09:54:59.000000 cvxportfolio-1.3.2/LICENSE
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    14052 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/PKG-INFO
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    12599 2024-04-06 09:38:48.000000 cvxportfolio-1.3.2/README.rst
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/cvxportfolio/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1013 2024-05-10 05:01:36.000000 cvxportfolio-1.3.2/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     3174 2024-05-08 16:30:44.000000 cvxportfolio-1.3.2/cvxportfolio/cache.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/cvxportfolio/constraints/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1678 2024-05-10 05:01:36.000000 cvxportfolio-1.3.2/cvxportfolio/constraints/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     5548 2024-04-02 16:10:25.000000 cvxportfolio-1.3.2/cvxportfolio/constraints/base_constraints.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    35921 2024-04-04 17:26:07.000000 cvxportfolio-1.3.2/cvxportfolio/constraints/constraints.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    42653 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/costs.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/cvxportfolio/data/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1102 2024-05-10 05:01:36.000000 cvxportfolio-1.3.2/cvxportfolio/data/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    35848 2024-05-08 16:30:44.000000 cvxportfolio-1.3.2/cvxportfolio/data/market_data.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    51122 2024-05-08 16:30:44.000000 cvxportfolio-1.3.2/cvxportfolio/data/symbol_data.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     2385 2024-03-16 05:48:22.000000 cvxportfolio-1.3.2/cvxportfolio/errors.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    30419 2024-04-04 17:32:53.000000 cvxportfolio-1.3.2/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    48403 2024-03-22 08:30:04.000000 cvxportfolio-1.3.2/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     7981 2024-04-04 17:24:49.000000 cvxportfolio-1.3.2/cvxportfolio/hyperparameters.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    38934 2024-05-09 17:01:41.000000 cvxportfolio-1.3.2/cvxportfolio/policies.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    37195 2024-04-04 17:33:55.000000 cvxportfolio-1.3.2/cvxportfolio/result.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    11062 2024-04-02 16:10:25.000000 cvxportfolio-1.3.2/cvxportfolio/returns.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    21541 2024-04-04 15:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/risks.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    32701 2024-05-08 16:30:44.000000 cvxportfolio-1.3.2/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/cvxportfolio/tests/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     6377 2024-05-10 05:01:36.000000 cvxportfolio-1.3.2/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1285 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/__main__.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)   156730 2023-10-14 06:46:10.000000 cvxportfolio-1.3.2/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo      (1000) enzo      (1000)   149356 2023-10-14 06:46:10.000000 cvxportfolio-1.3.2/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    14857 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    12037 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    50193 2024-05-08 16:30:44.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    14443 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    27339 2024-04-04 15:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     6249 2024-04-04 15:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_hyperparameters.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    32176 2024-05-09 17:08:36.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     9101 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_result.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     4779 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     9985 2024-04-03 14:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    46115 2024-05-08 16:30:44.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     3389 2024-04-04 15:00:04.000000 cvxportfolio-1.3.2/cvxportfolio/tests/test_utils.py
+-rw-r--r--   0 enzo      (1000) enzo      (1000)   116620 2023-10-14 06:46:10.000000 cvxportfolio-1.3.2/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     6364 2024-04-04 17:26:30.000000 cvxportfolio-1.3.2/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo      (1000) enzo      (1000)        0 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo      (1000) enzo      (1000)    14052 2024-05-10 05:07:00.000000 cvxportfolio-1.3.2/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     1337 2024-05-10 05:07:00.000000 cvxportfolio-1.3.2/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)        1 2024-05-10 05:07:00.000000 cvxportfolio-1.3.2/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)      255 2024-05-10 05:07:00.000000 cvxportfolio-1.3.2/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)       13 2024-05-10 05:07:00.000000 cvxportfolio-1.3.2/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo      (1000) enzo      (1000)     2783 2024-05-10 05:01:36.000000 cvxportfolio-1.3.2/pyproject.toml
+-rw-r--r--   0 enzo      (1000) enzo      (1000)       38 2024-05-10 05:07:00.545650 cvxportfolio-1.3.2/setup.cfg
```

### Comparing `cvxportfolio-1.3.1/LICENSE` & `cvxportfolio-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/PKG-INFO` & `cvxportfolio-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 1.3.1
+Version: 1.3.2
 Summary: Portfolio optimization and back-testing.
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Maintainer-email: Enzo Busseti <enzo.busseti@gmail.com>
 License: Apache License (2.0)
 Project-URL: Homepage, https://www.cvxportfolio.com
 Project-URL: Repository, https://github.com/cvxgrp/cvxportfolio
 Description-Content-Type: text/x-rst
@@ -20,26 +20,29 @@
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-github-style; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 Requires-Dist: diff_cover; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: autopep8; extra == "dev"
 Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: beautifulsoup4; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: beautifulsoup4; extra == "examples"
 Requires-Dist: lxml; extra == "examples"
 Requires-Dist: clarabel; extra == "examples"
 Requires-Dist: ecos; extra == "examples"
+Provides-Extra: test
+Requires-Dist: osqp; extra == "test"
+Requires-Dist: ecos; extra == "test"
+Requires-Dist: coverage[toml]; extra == "test"
 
 `Cvxportfolio <https://www.cvxportfolio.com>`_
 ==============================================
 
 |CVXportfolio on PyPI| |linting: pylint| |Coverage Status|
 |Documentation Status| |Apache 2.0 License| |Anaconda-Server Badge|
```

### Comparing `cvxportfolio-1.3.1/README.rst` & `cvxportfolio-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/__init__.py` & `cvxportfolio-1.3.2/cvxportfolio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Cvxportfolio __init__ module.
 
 This module only republishes the api of a selection of cvxportfolio
 modules. The __all__ attribute of each is used.
 """
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 
 from .constraints import *
 from .costs import *
 from .data import *
 from .hyperparameters import *
 from .policies import *
 from .result import *
```

### Comparing `cvxportfolio-1.3.1/cvxportfolio/cache.py` & `cvxportfolio-1.3.2/cvxportfolio/cache.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/constraints/__init__.py` & `cvxportfolio-1.3.2/cvxportfolio/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/constraints/base_constraints.py` & `cvxportfolio-1.3.2/cvxportfolio/constraints/base_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/constraints/constraints.py` & `cvxportfolio-1.3.2/cvxportfolio/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/costs.py` & `cvxportfolio-1.3.2/cvxportfolio/costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/data/__init__.py` & `cvxportfolio-1.3.2/cvxportfolio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/data/market_data.py` & `cvxportfolio-1.3.2/cvxportfolio/data/market_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 import numpy as np
 import pandas as pd
 
 from ..errors import DataError
 from ..utils import (hash_, make_numeric, periods_per_year_from_datetime_index,
                      resample_returns, set_pd_read_only)
-from .symbol_data import ( # pylint: disable=unused-import
-    BASE_LOCATION, OLHCV, Fred, SymbolData, YahooFinance, _loader_csv,
-    _loader_pickle, _loader_sqlite, _storer_csv, _storer_pickle,
-    _storer_sqlite)
+from .symbol_data import BASE_LOCATION  # pylint: disable=unused-import
+from .symbol_data import (OLHCV, Fred, SymbolData, YahooFinance, _loader_csv,
+                          _loader_pickle, _loader_sqlite, _storer_csv,
+                          _storer_pickle, _storer_sqlite)
 
 logger = logging.getLogger(__name__)
 
 __all__ = ['DownloadedMarketData', 'MarketData', 'UserProvidedMarketData']
 
 
 class MarketData:
```

### Comparing `cvxportfolio-1.3.1/cvxportfolio/data/symbol_data.py` & `cvxportfolio-1.3.2/cvxportfolio/data/symbol_data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/errors.py` & `cvxportfolio-1.3.2/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/estimator.py` & `cvxportfolio-1.3.2/cvxportfolio/estimator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/forecast.py` & `cvxportfolio-1.3.2/cvxportfolio/forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/hyperparameters.py` & `cvxportfolio-1.3.2/cvxportfolio/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/policies.py` & `cvxportfolio-1.3.2/cvxportfolio/policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -839,16 +839,16 @@
             # these warnings are thrown on numerical inaccuracies reported by
             # the solver and accounted for by cvxpy; we expect expert users
             # to set the solver options explicitely and/or setting verbose=True
             # in the cvxpy_kwargs
             warnings.filterwarnings(
                 "ignore", category=UserWarning,
                 message='Solution may be inaccurate')
-            # cvxpy 1.4 FutureWarnings
-            if cp.__version__[:3] == '1.4':
+            # cvxpy 1.4 and 1.5 FutureWarnings about ECOS deprecation
+            if cp.__version__[:3] in ['1.4', '1.5']:
                 warnings.filterwarnings("ignore", category=FutureWarning)
             try:
                 self._problem.solve(**self.cvxpy_kwargs)
             except cp.SolverError as exc:
                 # try to solve with SCS; it's the most robust
                 logger.error(
                     'CVXPY with settings %s reported numerical solver failure'
```

### Comparing `cvxportfolio-1.3.1/cvxportfolio/result.py` & `cvxportfolio-1.3.2/cvxportfolio/result.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/returns.py` & `cvxportfolio-1.3.2/cvxportfolio/returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/risks.py` & `cvxportfolio-1.3.2/cvxportfolio/risks.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/simulator.py` & `cvxportfolio-1.3.2/cvxportfolio/simulator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/__init__.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """We make the tests a sub-package so we can ship them."""
 
 import logging
-import shutil
-import tempfile
 import time
 import unittest
 from pathlib import Path
+from tempfile import TemporaryDirectory
 
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 import cvxportfolio as cvx
 
@@ -30,16 +29,19 @@
 
 class CvxportfolioTest(unittest.TestCase):
     """Base class for Cvxportfolio unit tests."""
 
     @classmethod
     def setUpClass(cls):
         """Initialize test class."""
-        cls.datadir = Path(tempfile.mkdtemp())
-        logger.info('created %s', cls.datadir)
+        # gets deleted automatically when de-referenced
+        # pylint: disable=consider-using-with
+        cls._tempdir = TemporaryDirectory()
+        cls.datadir = Path(cls._tempdir.name)
+        logger.info('using TemporaryDirectory %s', cls.datadir)
 
         cls.sigma = pd.read_csv(
             Path(__file__).parent / "sigmas.csv",
             index_col=0, parse_dates=[0])
         cls.returns = pd.read_csv(
             Path(__file__).parent /
             "returns.csv", index_col=0, parse_dates=[0])
@@ -59,26 +61,28 @@
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
 
         # with this we make sure we don't keep asking YahooFinance and Fred
         # for new data during the test execution
         cls.data_grace_period = pd.Timedelta('10d')
 
-        # with this we suppress the warnings thrown in Cvxpy 1.4
-        cls.default_socp_solver = 'ECOS'
+        # working around CVXPY-ECOS deprecation issues
+        try:
+            import ecos as _  # pylint: disable=import-outside-toplevel
+            cls.default_socp_solver = 'ECOS'
+        except ImportError: # pragma: no cover
+            cls.default_socp_solver = None # lets CVXPY choose
 
         # not necessary for now, but good to control
         cls.default_qp_solver = 'OSQP'
         cls.timers = {}
 
     @classmethod
     def tearDownClass(cls):
         """Finalize test class."""
-        logger.info('removing %s', cls.datadir)
-        shutil.rmtree(cls.datadir)
         print('Timing report:')
         print(pd.Series(cls.timers))
 
     @staticmethod
     def strip_tz_and_hour(market_data):
         """Transform DFs indexes from datetime with tz to date without tz.
```

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/__main__.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/returns.csv` & `cvxportfolio-1.3.2/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-1.3.2/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_costs.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_data.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_hyperparameters.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_policies.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Unit tests for the policy objects."""
 
 import unittest
+import warnings
 
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 import cvxportfolio as cvx
 from cvxportfolio.errors import DataError, PortfolioOptimizationError
@@ -356,19 +357,23 @@
 
         # print(np.linalg.eigh(self.returns.iloc[:121, :-1].cov().values)[0])
 
         # REPLICATE WITH CVXPY
 
         covariance = self.returns.iloc[:121, :-1].cov(ddof=0).values
         w = cp.Variable(self.N)
-        cp.Problem(
-            cp.Maximize(w[:-1].T @ self.returns.iloc[:121, :-1].mean().values -
-            2 * cp.quad_form(w[:-1], covariance) -
-            5 * 1E-4 * cp.sum(cp.abs(w - curw)[:-1])),
-            [w >= 0, w <= 1, sum(w) == 1]).solve(solver='ECOS')
+        with warnings.catch_warnings():
+            if cp.__version__[:3] in ['1.4', '1.5']:
+                warnings.filterwarnings("ignore", category=FutureWarning)
+            cp.Problem(
+                cp.Maximize(w[:-1].T @ self.returns.iloc[:121, :-1].mean().values -
+                2 * cp.quad_form(w[:-1], covariance) -
+                5 * 1E-4 * cp.sum(cp.abs(w - curw)[:-1])),
+                [w >= 0, w <= 1, sum(w) == 1]).solve(
+                    solver=self.default_socp_solver)
 
         cvxpy_result = pd.Series(w.value, self.returns.columns)
 
         # print(cvxpy_result)
 
         # print(cvxportfolio_result - cvxpy_result)
         self.assertTrue(np.allclose(
```

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_result.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_returns.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_risks.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_risks.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/test_utils.py` & `cvxportfolio-1.3.2/cvxportfolio/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/tests/volumes.csv` & `cvxportfolio-1.3.2/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio/utils.py` & `cvxportfolio-1.3.2/cvxportfolio/utils.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/cvxportfolio.egg-info/PKG-INFO` & `cvxportfolio-1.3.2/cvxportfolio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 1.3.1
+Version: 1.3.2
 Summary: Portfolio optimization and back-testing.
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Maintainer-email: Enzo Busseti <enzo.busseti@gmail.com>
 License: Apache License (2.0)
 Project-URL: Homepage, https://www.cvxportfolio.com
 Project-URL: Repository, https://github.com/cvxgrp/cvxportfolio
 Description-Content-Type: text/x-rst
@@ -20,26 +20,29 @@
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-github-style; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 Requires-Dist: diff_cover; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: autopep8; extra == "dev"
 Requires-Dist: docformatter; extra == "dev"
 Requires-Dist: beautifulsoup4; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: beautifulsoup4; extra == "examples"
 Requires-Dist: lxml; extra == "examples"
 Requires-Dist: clarabel; extra == "examples"
 Requires-Dist: ecos; extra == "examples"
+Provides-Extra: test
+Requires-Dist: osqp; extra == "test"
+Requires-Dist: ecos; extra == "test"
+Requires-Dist: coverage[toml]; extra == "test"
 
 `Cvxportfolio <https://www.cvxportfolio.com>`_
 ==============================================
 
 |CVXportfolio on PyPI| |linting: pylint| |Coverage Status|
 |Documentation Status| |Apache 2.0 License| |Anaconda-Server Badge|
```

### Comparing `cvxportfolio-1.3.1/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-1.3.2/cvxportfolio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvxportfolio-1.3.1/pyproject.toml` & `cvxportfolio-1.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [project]
 name = "cvxportfolio"
-version = "1.3.1"
+version = "1.3.2"
 description = "Portfolio optimization and back-testing."
 readme = "README.rst"
 license = {text = "Apache License (2.0)"}
 authors = [{name = "Enzo Busseti"}, {name = "Stephen Boyd"},
     {name = "Steven Diamond"}, {name = "BlackRock Inc."}]
 maintainers = [{name = "Enzo Busseti", email = "enzo.busseti@gmail.com"}]
 dependencies = ["pandas", "numpy", "matplotlib", "requests", "cvxpy",
     "multiprocess", # robustifies usage w/ 3rd party modules
     "scs" # it's hardcoded as fallback solver if numerical errors
     ]
 
 [project.optional-dependencies]
 docs = ["sphinx", "furo", "sphinx-github-style"]
-dev = ["build", "twine", "coverage", "diff_cover", "pylint", "isort",
+dev = ["build", "twine", "diff_cover", "pylint", "isort",
     "autopep8", "docformatter", "beautifulsoup4"]
 examples = ['beautifulsoup4', 'lxml', 'clarabel', 'ecos']
+test = ['osqp', 'ecos', 'coverage[toml]']
 
 [project.urls]
 Homepage = "https://www.cvxportfolio.com"
 Repository = "https://github.com/cvxgrp/cvxportfolio"
 
 [build-system]
 requires = ["setuptools"]
```

