# Comparing `tmp/synthetix-0.1.8.tar.gz` & `tmp/synthetix-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetix-0.1.8.tar", last modified: Wed Apr 17 22:17:29 2024, max compression
+gzip compressed data, was "synthetix-0.1.9.tar", last modified: Tue Apr 30 21:46:04 2024, max compression
```

## Comparing `synthetix-0.1.8.tar` & `synthetix-0.1.9.tar`

### file list

```diff
@@ -1,92 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 22:17:15.000000 synthetix-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-17 22:17:29.341613 synthetix-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-17 22:17:15.000000 synthetix-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:17:29.341613 synthetix-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 22:17:15.000000 synthetix-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.325613 synthetix-0.1.8/synthetix/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.325613 synthetix-0.1.8/synthetix/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.325613 synthetix-0.1.8/synthetix/contracts/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/1/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/1/CannonRegistry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/10/
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/10/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/420/
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/420/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.329613 synthetix-0.1.8/synthetix/contracts/deployments/421614/
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/421614/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.333613 synthetix-0.1.8/synthetix/contracts/deployments/8453/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/USDC.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/8453/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/contracts/deployments/84532/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/MintableToken.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/Pyth.json
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/84532/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/contracts/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/core/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/perps/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/perps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37760 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/perps/perps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/pyth/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.337613 synthetix-0.1.8/synthetix/spot/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/spot/spot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/synthetix/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-17 22:17:15.000000 synthetix-0.1.8/synthetix/utils/wei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/synthetix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 22:17:29.000000 synthetix-0.1.8/synthetix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:17:29.341613 synthetix-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_perps_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_spot_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_susd.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 22:17:15.000000 synthetix-0.1.8/tests/test_synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.397599 synthetix-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 21:45:50.000000 synthetix-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-30 21:46:04.397599 synthetix-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-30 21:45:50.000000 synthetix-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:46:04.397599 synthetix-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-30 21:45:50.000000 synthetix-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.381599 synthetix-0.1.9/synthetix/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.381599 synthetix-0.1.9/synthetix/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.381599 synthetix-0.1.9/synthetix/contracts/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.381599 synthetix-0.1.9/synthetix/contracts/deployments/1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/1/CannonRegistry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.385599 synthetix-0.1.9/synthetix/contracts/deployments/10/
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/10/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/10/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/10/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/10/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.385599 synthetix-0.1.9/synthetix/contracts/deployments/420/
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/420/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.385599 synthetix-0.1.9/synthetix/contracts/deployments/421614/
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/421614/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.389599 synthetix-0.1.9/synthetix/contracts/deployments/8453/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/8453/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.393599 synthetix-0.1.9/synthetix/contracts/deployments/84532/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/MintableToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/Pyth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/84532/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/contracts/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.393599 synthetix-0.1.9/synthetix/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.393599 synthetix-0.1.9/synthetix/perps/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/perps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41163 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/perps/perps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.393599 synthetix-0.1.9/synthetix/pyth/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.393599 synthetix-0.1.9/synthetix/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.393599 synthetix-0.1.9/synthetix/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/spot/spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.397599 synthetix-0.1.9/synthetix/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-30 21:45:50.000000 synthetix-0.1.9/synthetix/utils/wei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.397599 synthetix-0.1.9/synthetix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-30 21:46:04.000000 synthetix-0.1.9/synthetix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-30 21:46:04.000000 synthetix-0.1.9/synthetix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:46:04.000000 synthetix-0.1.9/synthetix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 21:46:04.000000 synthetix-0.1.9/synthetix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 21:46:04.000000 synthetix-0.1.9/synthetix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:46:04.397599 synthetix-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-04-30 21:45:50.000000 synthetix-0.1.9/tests/test_perps_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 21:45:50.000000 synthetix-0.1.9/tests/test_spot_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-30 21:45:50.000000 synthetix-0.1.9/tests/test_susd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-30 21:45:50.000000 synthetix-0.1.9/tests/test_synthetix.py
```

### Comparing `synthetix-0.1.8/PKG-INFO` & `synthetix-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.8
+Version: 0.1.9
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.8/README.md` & `synthetix-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/setup.py` & `synthetix-0.1.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="synthetix",
-    version="0.1.8",
+    version="0.1.9",
     description="Synthetix protocol SDK",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Synthetix DAO",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `synthetix-0.1.8/synthetix/constants.py` & `synthetix-0.1.9/synthetix/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/contracts.py` & `synthetix-0.1.9/synthetix/contracts/contracts.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/1/CannonRegistry.json` & `synthetix-0.1.9/synthetix/contracts/deployments/1/CannonRegistry.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/10/PerpsV2MarketData.json` & `synthetix-0.1.9/synthetix/contracts/deployments/10/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/10/USDProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/10/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/10/WETH.json` & `synthetix-0.1.9/synthetix/contracts/deployments/10/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/10/sUSD.json` & `synthetix-0.1.9/synthetix/contracts/deployments/10/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/AccountProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/CoreProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsAccountProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsMarketProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2Market.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/PerpsV2MarketData.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/SpotMarketProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/USDProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/WETH.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/420/sUSD.json` & `synthetix-0.1.9/synthetix/contracts/deployments/420/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/421614/WETH.json` & `synthetix-0.1.9/synthetix/contracts/deployments/421614/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/AccountProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/CoreProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsAccountProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/PerpsMarketProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/SpotMarketProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/USDC.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/USDC.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/USDProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/8453/WETH.json` & `synthetix-0.1.9/synthetix/contracts/deployments/8453/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/AccountProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/CoreProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/MintableToken.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/MintableToken.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsAccountProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/PerpsMarketProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/Pyth.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/Pyth.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/SpotMarketProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/USDProxy.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/contracts/deployments/84532/WETH.json` & `synthetix-0.1.9/synthetix/contracts/deployments/84532/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/core/core.py` & `synthetix-0.1.9/synthetix/core/core.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/perps/perps.py` & `synthetix-0.1.9/synthetix/perps/perps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for interacting with Synthetix Perps V3."""
 
 import time
-from eth_utils import decode_hex
+from eth_utils import encode_hex, decode_hex
 from ..utils import ether_to_wei, wei_to_ether
 from ..utils.multicall import (
     call_erc7412,
     multicall_erc7412,
     write_erc7412,
     make_fulfillment_request,
 )
@@ -41,23 +41,18 @@
     :param Pyth pyth: An instance of the Pyth class.
     :param int | None default_account_id: The default ``account_id`` to use for transactions.
 
     :return: An instance of the Perps class.
     :rtype: Perps
     """
 
-    def __init__(self, snx, pyth, default_account_id: int = None):
+    def __init__(self, snx, default_account_id: int = None):
         self.snx = snx
-        self.pyth = pyth
         self.logger = snx.logger
-
-        if "PythERC7412Wrapper" in snx.contracts:
-            self.erc7412_enabled = False
-        else:
-            self.erc7412_enabled = False
+        self.erc7412_enabled = True
 
         # check if perps is deployed on this network
         if "PerpsMarketProxy" in snx.contracts:
             self.market_proxy = snx.contracts["PerpsMarketProxy"]["contract"]
             self.account_proxy = snx.contracts["PerpsAccountProxy"]["contract"]
 
             try:
@@ -68,17 +63,15 @@
 
             try:
                 self.get_markets()
             except Exception as e:
                 self.logger.warning(f"Failed to fetch markets: {e}")
 
     # internals
-    def _resolve_market(
-        self, market_id: int, market_name: str, collateral: bool = False
-    ):
+    def _resolve_market(self, market_id: int, market_name: str):
         """
         Look up the market_id and market_name for a market. If only one is provided,
         the other is resolved. If both are provided, they are checked for consistency.
 
         :param int | None market_id: The id of the market. If not known, provide `None`.
         :param str | None market_name: The name of the market. If not known, provide `None`.
 
@@ -121,33 +114,58 @@
         """
         if len(market_names) == 0:
             market_names = [
                 self.market_meta[market]["symbol"] for market in self.market_meta
             ]
 
         # fetch the data from pyth
+        filtered_market_names = [
+            m for m in market_names if m in self.snx.pyth.price_feed_ids
+        ]
+        # if no markets, return an empty list
+        if len(filtered_market_names) == 0:
+            return []
+
         feed_ids = [
-            self.snx.pyth.price_feed_ids[market_name] for market_name in market_names
+            self.snx.pyth.price_feed_ids[market_name]
+            for market_name in filtered_market_names
         ]
-        price_update_data = self.snx.pyth.get_feeds_data(feed_ids)
+        if not self.snx.is_fork:
+            pyth_data = self.snx.pyth.get_price_from_ids(feed_ids)
+            price_update_data = pyth_data["price_update_data"]
+            price_metadata = pyth_data["meta"]
+        else:
+            # if it's a fork, get the price for the latest block
+            # this avoids providing "future" prices to the contract on a fork
+            block = self.snx.web3.eth.get_block("latest")
+
+            # set a manual 60 second staleness
+            publish_time = block.timestamp - 60
+            pyth_data = self.snx.pyth.get_price_from_ids(
+                feed_ids, publish_time=publish_time
+            )
+            price_update_data = pyth_data["price_update_data"]
+            price_metadata = pyth_data["meta"]
 
         # prepare the oracle call
         raw_feed_ids = [decode_hex(feed_id) for feed_id in feed_ids]
         args = (1, 30, raw_feed_ids)
 
         to, data, _ = make_fulfillment_request(
             self.snx,
             self.snx.contracts["PythERC7412Wrapper"]["address"],
             price_update_data,
             args,
         )
         value = len(market_names)
 
         # return this formatted for the multicall
-        return (to, True, value, data)
+        # set `require_success` to False in this case, since sometimes
+        # the wrapper will return an error if the price has already been updated
+        return [(to, False, value, data)], price_metadata
 
     # read
     # TODO: get_market_settings
     # TODO: get_order_fees
     def get_markets(self):
         """
         Fetch the ids and summaries for all perps markets. Market summaries include
@@ -176,26 +194,45 @@
         market_ids = self.market_proxy.functions.getMarkets().call()
 
         # fetch and store the metadata
         market_metadata = multicall_erc7412(
             self.snx, self.market_proxy, "metadata", market_ids
         )
 
+        # fetch settlement strategies to get feed_ids
+        settlement_strategy_inputs = [(market_id, 0) for market_id in market_ids]
+        settlement_strategies = multicall_erc7412(
+            self.snx,
+            self.market_proxy,
+            "getSettlementStrategy",
+            settlement_strategy_inputs,
+        )
+
         self.market_meta = {
             market_id: {
                 "name": market_metadata[ind][0],
                 "symbol": market_metadata[ind][1],
+                "feed_id": encode_hex(settlement_strategies[ind][4]),
             }
             for ind, market_id in enumerate(market_ids)
         }
 
+        # update pyth price feed ids
+        self.snx.pyth.update_price_feed_ids(
+            {
+                self.market_meta[market]["symbol"]: self.market_meta[market]["feed_id"]
+                for market in self.market_meta
+            }
+        )
+
         # fetch the market summaries
         market_summaries = self.get_market_summaries(market_ids)
-
         markets_by_id = {summary["market_id"]: summary for summary in market_summaries}
+
+        # make markets by market name
         markets_by_name = {
             summary["market_name"]: summary for summary in market_summaries
         }
         self.markets_by_id, self.markets_by_name = markets_by_id, markets_by_name
         return markets_by_id, markets_by_name
 
     def get_order(self, account_id: int = None, fetch_settlement_strategy: bool = True):
@@ -249,16 +286,15 @@
         :param [int] market_ids: A list of market ids to fetch.
         :return: A list of market summaries in the order of the input ``market_ids``.
         :rtype: [dict]
         """
         # TODO: Fetch for market names
         # get fresh prices to provide to the oracle
         if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call()
-            calls = [oracle_call]
+            calls, _ = self._prepare_oracle_call()
         else:
             calls = []
 
         inputs = [(market_id,) for market_id in market_ids]
 
         markets = multicall_erc7412(
             self.snx, self.market_proxy, "getMarketSummary", inputs, calls=calls
@@ -283,14 +319,15 @@
             ) = market
             market_id = market_ids[ind]
 
             market_summaries.append(
                 {
                     "market_id": market_id,
                     "market_name": self.market_meta[market_id]["symbol"],
+                    "feed_id": self.market_meta[market_id]["feed_id"],
                     "skew": wei_to_ether(skew),
                     "size": wei_to_ether(size),
                     "max_open_interest": wei_to_ether(max_open_interest),
                     "interest_rate": wei_to_ether(interest_rate),
                     "current_funding_rate": wei_to_ether(current_funding_rate),
                     "current_funding_velocity": wei_to_ether(current_funding_velocity),
                     "index_price": wei_to_ether(index_price),
@@ -309,16 +346,15 @@
         :return: A dictionary with the market summary.
         :rtype: dict
         """
         market_id, market_name = self._resolve_market(market_id, market_name)
 
         # get a fresh price to provide to the oracle
         if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call([market_name])
-            calls = [oracle_call]
+            calls, _ = self._prepare_oracle_call()
         else:
             calls = []
 
         (
             skew,
             size,
             max_open_interest,
@@ -429,16 +465,15 @@
         :rtype: dict
         """
         if not account_id:
             account_id = self.default_account_id
 
         # get fresh prices to provide to the oracle
         if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call()
-            calls = [oracle_call]
+            calls, _ = self._prepare_oracle_call()
         else:
             calls = []
 
         # TODO: expand multicall capability to handle multiple functions
         total_collateral_value = call_erc7412(
             self.snx,
             self.market_proxy,
@@ -519,16 +554,15 @@
         :rtype: bool
         """
         if not account_id:
             account_id = self.default_account_id
 
         # get fresh prices to provide to the oracle
         if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call()
-            calls = [oracle_call]
+            calls, _ = self._prepare_oracle_call()
         else:
             calls = []
 
         can_liquidate = call_erc7412(
             self.snx, self.market_proxy, "canLiquidate", account_id, calls=calls
         )
 
@@ -542,16 +576,15 @@
         :return: A list of tuples containing the ``account_id`` and a boolean indicating if the account is eligible for liquidation.
         :rtype: [(int, bool)]
         """
         account_ids = [(account_id,) for account_id in account_ids]
 
         # get fresh prices to provide to the oracle
         if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call()
-            calls = [oracle_call]
+            calls, _ = self._prepare_oracle_call()
         else:
             calls = []
 
         can_liquidates = multicall_erc7412(
             self.snx, self.market_proxy, "canLiquidate", account_ids, calls=calls
         )
 
@@ -584,16 +617,15 @@
         """
         market_id, market_name = self._resolve_market(market_id, market_name)
         if not account_id:
             account_id = self.default_account_id
 
         # get a fresh price to provide to the oracle
         if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call([market_name])
-            calls = [oracle_call]
+            calls, _ = self._prepare_oracle_call([market_name])
         else:
             calls = []
 
         pnl, accrued_funding, position_size, owed_interest = call_erc7412(
             self.snx,
             self.market_proxy,
             "getOpenPosition",
@@ -650,16 +682,15 @@
             ]
 
         # make the function inputs
         clean_inputs = [(account_id, market_id) for market_id in market_ids]
 
         # get a fresh price to provide to the oracle
         if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call(market_names)
-            calls = [oracle_call]
+            calls, _ = self._prepare_oracle_call(market_names)
         else:
             calls = []
 
         open_positions = multicall_erc7412(
             self.snx, self.market_proxy, "getOpenPosition", clean_inputs, calls=calls
         )
 
@@ -675,14 +706,74 @@
             for ind, (pnl, accrued_funding, position_size, owedInterest) in enumerate(
                 open_positions
             )
             if abs(position_size) > 0
         }
         return open_positions
 
+    def get_quote(
+        self,
+        size: float,
+        price: float = None,
+        market_id: int = None,
+        market_name: str = None,
+        account_id: int = None,
+        include_required_margin: bool = True,
+    ):
+        """
+        Get a quote for the size of an order in a specified market. The quote includes
+        the provided price and the fill price of the order after price impact. If a price
+        is not provided, a price will be fetched from Pyth. Provide either a ``market_id``
+        or ``market_name``.
+
+        :param float size: The size of the order to quote.
+        :param float | None price: The price to quote the order at. If not provided, the current market price is used.
+        :param int | None market_id: The id of the market to quote the order for.
+        :param str | None market_name: The name of the market to quote the order for.
+        :return: A dictionary with the quote information.
+        :rtype: dict
+        """
+        if not account_id:
+            account_id = self.default_account_id
+
+        market_id, market_name = self._resolve_market(market_id, market_name)
+        feed_id = self.markets_by_id[market_id]["feed_id"]
+
+        if not price:
+            calls, meta = self._prepare_oracle_call([market_name])
+            price = meta[feed_id]["price"]
+        else:
+            calls = []
+            price = price
+
+        fill_price = call_erc7412(
+            self.snx,
+            self.market_proxy,
+            "fillPrice",
+            (market_id, ether_to_wei(size), ether_to_wei(price)),
+            calls=calls,
+        )
+
+        result = {
+            "order_size": size,
+            "index_price": price,
+            "fill_price": wei_to_ether(fill_price),
+        }
+
+        if include_required_margin and account_id:
+            required_margin = call_erc7412(
+                self.snx,
+                self.market_proxy,
+                "requiredMarginForOrderWithPrice",
+                (account_id, market_id, ether_to_wei(size), ether_to_wei(price)),
+                calls=calls,
+            )
+            result["required_margin"] = wei_to_ether(required_margin)
+        return result
+
     # transactions
     def create_account(self, account_id: int = None, submit: bool = False):
         """
         Create a perps account. An account NFT is minted to the sender, who
         owns the account.
 
         :param int | None account_id: Specify the id of the account. If the id already exists,
@@ -905,30 +996,23 @@
             time.sleep(duration)
         else:
             # TODO: check if expired
             self.logger.info(f"Order is ready to be settled")
 
         # get fresh prices to provide to the oracle
         market_name = self._resolve_market(order["market_id"], None)[1]
-        if self.erc7412_enabled:
-            oracle_call = self._prepare_oracle_call([market_name])
-            calls = [oracle_call]
-        else:
-            calls = []
-
         # prepare the transaction
         tx_tries = 0
         while tx_tries < max_tx_tries:
             try:
                 tx_params = write_erc7412(
                     self.snx,
                     self.market_proxy,
                     "settleOrder",
                     [account_id],
-                    calls=calls,
                 )
             except Exception as e:
                 self.logger.error(f"settleOrder error: {e}")
                 tx_tries += 1
                 time.sleep(tx_delay)
                 continue
```

### Comparing `synthetix-0.1.8/synthetix/queries/config.py` & `synthetix-0.1.9/synthetix/queries/config.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/queries/gql.py` & `synthetix-0.1.9/synthetix/queries/gql.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/queries/queries.py` & `synthetix-0.1.9/synthetix/queries/queries.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix/spot/spot.py` & `synthetix-0.1.9/synthetix/spot/spot.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,16 @@
     :param Synthetix snx: An instance of the Synthetix class.
     :param Pyth pyth: An instance of the Pyth class.
 
     :return: An instance of the Spot class.
     :rtype: Spot
     """
 
-    def __init__(self, snx, pyth):
+    def __init__(self, snx):
         self.snx = snx
-        self.pyth = pyth
         self.logger = snx.logger
 
         # check if spot is deployed on this network
         if "SpotMarketProxy" in snx.contracts:
             self.market_proxy = snx.contracts["SpotMarketProxy"]["contract"]
             self.markets_by_id, self.markets_by_name = self.get_markets()
 
@@ -386,17 +385,14 @@
         :return: The transaction dict if submit=False, otherwise the tx hash.
         """
         market_id, market_name = self._resolve_market(market_id, market_name)
 
         # fix the amount
         amount = 2**256 - 1 if amount is None else ether_to_wei(amount)
         synth_contract = self._get_synth_contract(market_id)
-        tx_data = synth_contract.encodeABI(
-            fn_name="approve", args=[target_address, amount]
-        )
 
         tx_params = self.snx._get_tx_params()
         tx_params = synth_contract.functions.approve(
             target_address, amount
         ).build_transaction(tx_params)
 
         if submit:
```

### Comparing `synthetix-0.1.8/synthetix/synthetix.py` & `synthetix-0.1.9/synthetix/synthetix.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         max_price_impact: float = DEFAULT_SLIPPAGE,
         use_estimate_gas: bool = True,
         cannon_config: dict = None,
         gql_endpoint_perps: str = None,
         gql_endpoint_rates: str = None,
         satsuma_api_key: str = None,
         price_service_endpoint: str = None,
+        pyth_cache_ttl: int = 60,
         gas_multiplier: float = DEFAULT_GAS_MULTIPLIER,
         is_fork: bool = False,
     ):
         args = parse_args()
         self.logger = setup_logging(args.debug, args.verbose)
 
         # init account variables
@@ -237,18 +238,18 @@
         # init pyth
         if (
             not price_service_endpoint
             and self.network_id in DEFAULT_PRICE_SERVICE_ENDPOINTS
         ):
             price_service_endpoint = DEFAULT_PRICE_SERVICE_ENDPOINTS[self.network_id]
 
-        self.pyth = Pyth(self, price_service_endpoint=price_service_endpoint)
+        self.pyth = Pyth(self, cache_ttl=pyth_cache_ttl, price_service_endpoint=price_service_endpoint)
         self.core = Core(self, core_account_id)
-        self.perps = Perps(self, self.pyth, perps_account_id)
-        self.spot = Spot(self, self.pyth)
+        self.spot = Spot(self)
+        self.perps = Perps(self, perps_account_id)
 
     def _load_contracts(self):
         """
         Initializes and sets up contracts according to the connected chain.
         On calling this function, the following contracts are connected and set up:
         * ``PerpsV2MarketData``
         * ``PerpsV2MarketProxy`` (for each V2 market)
```

### Comparing `synthetix-0.1.8/synthetix/utils/multicall.py` & `synthetix-0.1.9/synthetix/utils/multicall.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,35 +85,40 @@
         # decode error data
         address, feed_ids, args = decode_erc7412_error(snx, error.data)
         update_type = args[0]
 
         if update_type == 1:
             # fetch the data from pyth for those feed ids
             if not snx.is_fork:
-                price_update_data = snx.pyth.get_feeds_data(feed_ids)
+                pyth_data = snx.pyth.get_price_from_ids(feed_ids)
+                price_update_data = pyth_data["price_update_data"]
             else:
                 # if it's a fork, get the price for the latest block
                 # this avoids providing "future" prices to the contract on a fork
                 block = snx.web3.eth.get_block("latest")
-                price_update_data = [
-                    snx.pyth.get_benchmark_data(feed_id, block.timestamp)[0]
-                    for feed_id in feed_ids
-                ]
+
+                # set a manual 60 second staleness
+                publish_time = block.timestamp - 60
+                pyth_data = snx.pyth.get_price_from_ids(
+                    feed_ids, publish_time=publish_time
+                )
+                price_update_data = pyth_data["price_update_data"]
 
             # create a new request
             to, data, value = make_fulfillment_request(
                 snx, address, price_update_data, args
             )
         elif update_type == 2:
             # fetch the data from pyth for those feed ids
-            price_update_data, _, _ = snx.pyth.get_benchmark_data(feed_ids[0], args[1])
+            pyth_data = snx.pyth.get_price_from_ids(feed_ids, publish_time=args[1])
+            price_update_data = pyth_data["price_update_data"]
 
             # create a new request
             to, data, value = make_fulfillment_request(
-                snx, address, [price_update_data], args
+                snx, address, price_update_data, args
             )
         else:
             snx.logger.error(f"Unknown update type: {update_type}")
             raise error
 
         calls = [(to, True, value, data)] + calls
         return calls
@@ -138,15 +143,15 @@
 def write_erc7412(snx, contract, function_name, args, tx_params={}, calls=[]):
     # prepare the initial call
     this_call = [
         (
             contract.address,
             True,
             0 if "value" not in tx_params else tx_params["value"],
-            bytes.fromhex(contract.encodeABI(fn_name=function_name, args=args)[2:]),
+            contract.encodeABI(fn_name=function_name, args=args),
         )
     ]
     calls = calls + this_call
 
     while True:
         try:
             # unpack calls into the multicallThrough inputs
```

### Comparing `synthetix-0.1.8/synthetix/utils/wei.py` & `synthetix-0.1.9/synthetix/utils/wei.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/synthetix.egg-info/PKG-INFO` & `synthetix-0.1.9/synthetix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.8
+Version: 0.1.9
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.8/synthetix.egg-info/SOURCES.txt` & `synthetix-0.1.9/synthetix.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 synthetix/contracts/deployments/84532/USDProxy.json
 synthetix/contracts/deployments/84532/WETH.json
 synthetix/core/__init__.py
 synthetix/core/core.py
 synthetix/perps/__init__.py
 synthetix/perps/perps.py
 synthetix/pyth/__init__.py
-synthetix/pyth/constants.py
 synthetix/pyth/pyth.py
 synthetix/queries/__init__.py
 synthetix/queries/config.py
 synthetix/queries/gql.py
 synthetix/queries/queries.py
 synthetix/spot/__init__.py
 synthetix/spot/spot.py
```

### Comparing `synthetix-0.1.8/tests/test_perps_v3.py` & `synthetix-0.1.9/tests/test_perps_v3.py`

 * *Files 11% similar despite different names*

```diff
@@ -165,14 +165,56 @@
     assert settlement_strategy["price_verification_contract"] is not None
     assert settlement_strategy["feed_id"] is not None
     assert settlement_strategy["settlement_reward"] is not None
     assert settlement_strategy["disabled"] is not None
     assert settlement_strategy["commitment_price_delay"] is not None
 
 
+def test_perps_quote(snx):
+    """The instance can fetch a quote"""
+    long_quote = snx.perps.get_quote(1, market_id=100)
+    short_quote = snx.perps.get_quote(-1, market_id=100)
+
+    assert long_quote is not None
+    assert long_quote["order_size"] is not None
+    assert long_quote["index_price"] is not None
+    assert long_quote["fill_price"] is not None
+    assert long_quote["required_margin"] is not None
+
+    assert short_quote is not None
+    assert short_quote["order_size"] is not None
+    assert short_quote["index_price"] is not None
+    assert short_quote["fill_price"] is not None
+    assert short_quote["required_margin"] is not None
+
+    # the short fill price should be less than the long fill price
+    assert short_quote["fill_price"] < long_quote["fill_price"]
+
+
+def test_perps_quote_with_price(snx):
+    """The instance can fetch a quote with a fill price"""
+    long_quote = snx.perps.get_quote(1, price=2500, market_id=100)
+    short_quote = snx.perps.get_quote(-1, price=2500, market_id=100)
+
+    assert long_quote is not None
+    assert long_quote["order_size"] is not None
+    assert long_quote["index_price"] is not None
+    assert long_quote["fill_price"] is not None
+    assert long_quote["required_margin"] is not None
+
+    assert short_quote is not None
+    assert short_quote["order_size"] is not None
+    assert short_quote["index_price"] is not None
+    assert short_quote["fill_price"] is not None
+    assert short_quote["required_margin"] is not None
+
+    # the short fill price should be less than the long fill price
+    assert short_quote["fill_price"] < long_quote["fill_price"]
+
+
 def test_perps_order(snx, logger):
     """The instance can fetch an order for an account"""
     order = snx.perps.get_order(fetch_settlement_strategy=False)
 
     logger.info(f"Address: {snx.address} - order: {order}")
     assert order is not None
     assert order["commitment_time"] is not None
@@ -222,14 +264,15 @@
 
     deposit_tx = snx.perps.modify_collateral(1, market_name="sUSD")
     logger.info(f"Address: {snx.address} - deposit: {deposit_tx}")
 
     assert deposit_tx is not None
 
 
+@pytest.mark.skip(reason="Disabling since we don't know the account has margin")
 def test_perps_commit_order(snx, logger):
     """User can prepare a commit order transaction"""
     order = snx.perps.commit_order(1, market_name="ETH")
 
     assert order is not None
     assert order["from"] == snx.address
     assert order["data"] is not None
```

### Comparing `synthetix-0.1.8/tests/test_spot_v3.py` & `synthetix-0.1.9/tests/test_spot_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.8/tests/test_susd.py` & `synthetix-0.1.9/tests/test_susd.py`

 * *Files identical despite different names*

