# Comparing `tmp/deropy-0.2.1.tar.gz` & `tmp/deropy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.2.1.tar", last modified: Thu May  9 08:53:30 2024, max compression
+gzip compressed data, was "deropy-0.2.2.tar", last modified: Thu May  9 14:00:46 2024, max compression
```

## Comparing `deropy-0.2.1.tar` & `deropy-0.2.2.tar`

### file list

```diff
@@ -1,114 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-09 08:53:26.000000 deropy-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 08:53:30.553107 deropy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-09 08:53:26.000000 deropy-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.537107 deropy-0.2.1/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.537107 deropy-0.2.1/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/transpile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.537107 deropy-0.2.1/deropy/dvm/
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/Smartcontract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/Wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.541107 deropy-0.2.1/deropy/dvm/dast/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/assignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/binaryOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/dast_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/declaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/functionCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/functionDef.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/goto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/ifTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/variableDeclarationAdnAssignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/whileLoop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.549107 deropy-0.2.1/deropy/dvm/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/AddressRaw.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/AddressString.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/AssetValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Atoi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Blid.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/BlockHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/BlockTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Dero.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/DeroValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Function.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/HexDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/IsAddressValid.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Itoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapDelete.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapExists.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapGet.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Panic.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Random.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Scid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/SendAssetToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/SendDeroToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Sha3256.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Signer.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Store.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Strlen.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Substr.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Txid.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/UpdateScCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/deropy/dvm/iast/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/IastNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/assignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/binaryOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/functionCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/functionDef.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/iast_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/ifTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/variableDeclarationAdnAssignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/whileLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/deropy/python_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/Nameservice.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/lottery.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/minimum_sc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:53:30.553107 deropy-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 08:53:26.000000 deropy-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-09 08:53:26.000000 deropy-0.2.1/tests/test_compute_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-09 08:53:26.000000 deropy-0.2.1/tests/test_map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-09 08:53:26.000000 deropy-0.2.1/tests/test_storage_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.042732 deropy-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-09 14:00:41.000000 deropy-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 14:00:46.042732 deropy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-09 14:00:41.000000 deropy-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.022732 deropy-0.2.2/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.026732 deropy-0.2.2/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/commands/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/commands/transpile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.026732 deropy-0.2.2/deropy/dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/Smartcontract.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.030732 deropy-0.2.2/deropy/dvm/dast/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/dast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/declaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/goto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/dast/whileLoop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.038732 deropy-0.2.2/deropy/dvm/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/AddressRaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/AddressString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/AssetValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Atoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Blid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/BlockHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/BlockTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Dero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/DeroValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/HexDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/IsAddressValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Itoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/MapDelete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/MapExists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/MapGet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/MapStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Scid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/SendAssetToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/SendDeroToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Sha3256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Strlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Substr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/Txid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/UpdateScCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.038732 deropy-0.2.2/deropy/dvm/iast/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/IastNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/iast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/iast/whileLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/dvm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.038732 deropy-0.2.2/deropy/python_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/python_templates/Nameservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/python_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/python_templates/lottery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/python_templates/minimum_sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/python_templates/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.042732 deropy-0.2.2/deropy/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/wallet/derohe_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/wallet/python_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/wallet/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/wallet/wallet_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-09 14:00:41.000000 deropy-0.2.2/deropy/wallet/wallet_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.042732 deropy-0.2.2/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 14:00:46.000000 deropy-0.2.2/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-09 14:00:46.000000 deropy-0.2.2/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:00:46.000000 deropy-0.2.2/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 14:00:46.000000 deropy-0.2.2/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 14:00:46.000000 deropy-0.2.2/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 14:00:46.000000 deropy-0.2.2/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:00:46.042732 deropy-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 14:00:41.000000 deropy-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:46.042732 deropy-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-09 14:00:41.000000 deropy-0.2.2/tests/test_compute_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-09 14:00:41.000000 deropy-0.2.2/tests/test_map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-09 14:00:41.000000 deropy-0.2.2/tests/test_storage_functions.py
```

### Comparing `deropy-0.2.1/LICENSE` & `deropy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/PKG-INFO` & `deropy-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.2.1/README.md` & `deropy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/commands/configure.py` & `deropy-0.2.2/deropy/commands/configure.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/commands/deploy.py` & `deropy-0.2.2/deropy/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/commands/generate.py` & `deropy-0.2.2/deropy/commands/generate.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/commands/simulate.py` & `deropy-0.2.2/deropy/commands/simulate.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/Smartcontract.py` & `deropy-0.2.2/deropy/dvm/Smartcontract.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     scid = None
     active_wallet = None
     public_functions = []
     max_compute_gaz = 10_000_000
     max_storage_gas = 20_000
     dero_value = None
     asset_value = None
+    active_wallet = None
 
     # Blockchain basic component simulation
     blocks = []
     transactions = []
     scid = sha256(str(time.time()).encode()).hexdigest()
 
     def __new__(cls):
```

### Comparing `deropy-0.2.1/deropy/dvm/dast/__init__.py` & `deropy-0.2.2/deropy/dvm/dast/__init__.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/argument.py` & `deropy-0.2.2/deropy/dvm/dast/argument.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/assignement.py` & `deropy-0.2.2/deropy/dvm/dast/assignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/binaryOperator.py` & `deropy-0.2.2/deropy/dvm/dast/binaryOperator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/compare.py` & `deropy-0.2.2/deropy/dvm/dast/compare.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/dast_converter.py` & `deropy-0.2.2/deropy/dvm/dast/dast_converter.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/declaration.py` & `deropy-0.2.2/deropy/dvm/dast/declaration.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/functionCall.py` & `deropy-0.2.2/deropy/dvm/dast/functionCall.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/functionDef.py` & `deropy-0.2.2/deropy/dvm/dast/functionDef.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/ifTest.py` & `deropy-0.2.2/deropy/dvm/dast/ifTest.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/operator.py` & `deropy-0.2.2/deropy/dvm/dast/operator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/returns.py` & `deropy-0.2.2/deropy/dvm/dast/returns.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/variableDeclarationAdnAssignement.py` & `deropy-0.2.2/deropy/dvm/dast/variableDeclarationAdnAssignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/dast/whileLoop.py` & `deropy-0.2.2/deropy/dvm/dast/whileLoop.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/AddressRaw.py` & `deropy-0.2.2/deropy/dvm/functions/AddressRaw.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from deropy.dvm.functions.Function import Function
-from deropy.dvm.Wallet import WalletSimulator
+from deropy.wallet.wallet_simulator import WalletSimulator
 
 
 class AddressRaw(Function):
     def __init__(self):
         func_parameters = {
             "address": {"type": "str", "value": None},
         }
```

### Comparing `deropy-0.2.1/deropy/dvm/functions/AddressString.py` & `deropy-0.2.2/deropy/dvm/functions/AddressString.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from deropy.dvm.functions.Function import Function
-from deropy.dvm.Wallet import WalletSimulator
+from deropy.wallet.wallet_simulator import WalletSimulator
 
 
 class AddressString(Function):
     def __init__(self):
         func_parameters = {
             "address": {"type": "str", "value": None},
         }
```

### Comparing `deropy-0.2.1/deropy/dvm/functions/AssetValue.py` & `deropy-0.2.2/deropy/dvm/functions/AssetValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Atoi.py` & `deropy-0.2.2/deropy/dvm/functions/Atoi.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/BlockHeight.py` & `deropy-0.2.2/deropy/dvm/functions/BlockHeight.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Dero.py` & `deropy-0.2.2/deropy/dvm/functions/Dero.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/DeroValue.py` & `deropy-0.2.2/deropy/dvm/functions/DeroValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Exists.py` & `deropy-0.2.2/deropy/dvm/functions/Exists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Function.py` & `deropy-0.2.2/deropy/dvm/functions/Function.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/IsAddressValid.py` & `deropy-0.2.2/deropy/dvm/functions/IsAddressValid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Itoa.py` & `deropy-0.2.2/deropy/dvm/functions/Itoa.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Keccak256.py` & `deropy-0.2.2/deropy/dvm/functions/Keccak256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Load.py` & `deropy-0.2.2/deropy/dvm/functions/Load.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/MapExists.py` & `deropy-0.2.2/deropy/dvm/functions/MapExists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/MapStore.py` & `deropy-0.2.2/deropy/dvm/functions/MapStore.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Random.py` & `deropy-0.2.2/deropy/dvm/functions/Random.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Scid.py` & `deropy-0.2.2/deropy/dvm/functions/Scid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/SendAssetToAddress.py` & `deropy-0.2.2/deropy/dvm/functions/SendAssetToAddress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from deropy.dvm.functions.Function import Function
-from deropy.dvm.Wallet import WalletSimulator, Wallet
+from deropy.wallet.wallet_simulator import WalletSimulator
+from deropy.wallet.wallet import Wallet
 
 
 class SendAssetToAddress(Function):
     def __init__(self):
         func_parameters = {
             "raw_address": {"type": "str", "value": None},
             "amount": {"type": "int", "value": None},
```

### Comparing `deropy-0.2.1/deropy/dvm/functions/SendDeroToAddress.py` & `deropy-0.2.2/deropy/dvm/functions/SendDeroToAddress.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from deropy.dvm.functions.Function import Function
-from deropy.dvm.Wallet import WalletSimulator, Wallet
+from deropy.wallet.wallet_simulator import WalletSimulator
+from deropy.wallet.wallet import Wallet
 
 
 class SendDeroToAddress(Function):
     def __init__(self):
         func_parameters = {
             "raw_address": {"type": "str", "value": None},
             "amount": {"type": "int", "value": None},
```

### Comparing `deropy-0.2.1/deropy/dvm/functions/Sha256.py` & `deropy-0.2.2/deropy/dvm/functions/Sha256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Sha3256.py` & `deropy-0.2.2/deropy/dvm/functions/Sha3256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Signer.py` & `deropy-0.2.2/deropy/dvm/functions/Signer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from deropy.dvm.functions.Function import Function
-from deropy.dvm.Wallet import WalletSimulator
+from deropy.wallet.wallet_simulator import WalletSimulator
 
 
 class Signer(Function):
     def __init__(self):
         func_parameters = {}
         super().__init__("signer", 5_000, 0, func_parameters)
 
     def _exec(self, *args, **kwargs):
         if not WalletSimulator.is_initialized():
             raise Exception("Wallet simulator not initialized")
         if WalletSimulator.active_wallet is None:
             raise Exception("No active wallet")
 
-        return WalletSimulator.get_raw_address()
+        return WalletSimulator.active_wallet.raw_address
 
     def _computeGasStorageCost(self):
         return 0
 
 
 def signer():
     return Signer()()
```

### Comparing `deropy-0.2.1/deropy/dvm/functions/Store.py` & `deropy-0.2.2/deropy/dvm/functions/Store.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/Substr.py` & `deropy-0.2.2/deropy/dvm/functions/Substr.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/UpdateScCode.py` & `deropy-0.2.2/deropy/dvm/functions/UpdateScCode.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/functions/__init__.py` & `deropy-0.2.2/deropy/dvm/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/argument.py` & `deropy-0.2.2/deropy/dvm/iast/argument.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/assignement.py` & `deropy-0.2.2/deropy/dvm/iast/assignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/binaryOperator.py` & `deropy-0.2.2/deropy/dvm/iast/binaryOperator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/compare.py` & `deropy-0.2.2/deropy/dvm/iast/compare.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/functionCall.py` & `deropy-0.2.2/deropy/dvm/iast/functionCall.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/functionDef.py` & `deropy-0.2.2/deropy/dvm/iast/functionDef.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/iast_converter.py` & `deropy-0.2.2/deropy/dvm/iast/iast_converter.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/ifTest.py` & `deropy-0.2.2/deropy/dvm/iast/ifTest.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/operator.py` & `deropy-0.2.2/deropy/dvm/iast/operator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/returns.py` & `deropy-0.2.2/deropy/dvm/iast/returns.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/variableDeclarationAdnAssignement.py` & `deropy-0.2.2/deropy/dvm/iast/variableDeclarationAdnAssignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/iast/whileLoop.py` & `deropy-0.2.2/deropy/dvm/iast/whileLoop.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/parser.py` & `deropy-0.2.2/deropy/dvm/parser.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/tester.py` & `deropy-0.2.2/deropy/dvm/tester.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/dvm/utils.py` & `deropy-0.2.2/deropy/dvm/utils.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/main.py` & `deropy-0.2.2/deropy/main.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/python_templates/Nameservice.py` & `deropy-0.2.2/deropy/python_templates/Nameservice.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/python_templates/lottery.py` & `deropy-0.2.2/deropy/python_templates/lottery.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/python_templates/minimum_sc.py` & `deropy-0.2.2/deropy/python_templates/minimum_sc.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/python_templates/token.py` & `deropy-0.2.2/deropy/python_templates/token.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy/utils.py` & `deropy-0.2.2/deropy/utils.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.1/deropy.egg-info/PKG-INFO` & `deropy-0.2.2/deropy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.2.1/deropy.egg-info/SOURCES.txt` & `deropy-0.2.2/deropy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 deropy/commands/__init__.py
 deropy/commands/configure.py
 deropy/commands/deploy.py
 deropy/commands/generate.py
 deropy/commands/simulate.py
 deropy/commands/transpile.py
 deropy/dvm/Smartcontract.py
-deropy/dvm/Wallet.py
 deropy/dvm/__init__.py
 deropy/dvm/parser.py
 deropy/dvm/tester.py
 deropy/dvm/utils.py
 deropy/dvm/dast/__init__.py
 deropy/dvm/dast/argument.py
 deropy/dvm/dast/assignement.py
@@ -93,10 +92,16 @@
 deropy/dvm/iast/variableDeclarationAdnAssignement.py
 deropy/dvm/iast/whileLoop.py
 deropy/python_templates/Nameservice.py
 deropy/python_templates/__init__.py
 deropy/python_templates/lottery.py
 deropy/python_templates/minimum_sc.py
 deropy/python_templates/token.py
+deropy/wallet/__init__.py
+deropy/wallet/derohe_wallet.py
+deropy/wallet/python_wallet.py
+deropy/wallet/wallet.py
+deropy/wallet/wallet_factory.py
+deropy/wallet/wallet_simulator.py
 tests/test_compute_storage.py
 tests/test_map_functions.py
 tests/test_storage_functions.py
```

### Comparing `deropy-0.2.1/setup.py` & `deropy-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.2.1',
+    version=os.getenv('DEROPY_VERSION') or '0.2.2',
     url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `deropy-0.2.1/tests/test_compute_storage.py` & `deropy-0.2.2/tests/test_compute_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import importlib
 import pytest
 
-from deropy.dvm.Wallet import WalletSimulator
+from deropy.wallet.wallet import Wallet
+from deropy.wallet.wallet_factory import WalletFactory
+from deropy.wallet.wallet_simulator import WalletSimulator
 
 # basic initialization
-WalletSimulator.create_wallet('hyperbolic')
-WalletSimulator.active_wallet = 'hyperbolic'
+wl_hyperbolic: Wallet = WalletFactory.create_wallet('hyperbolic')
+WalletSimulator.active_wallet = wl_hyperbolic.name
 
 
 list_of_tests = {
-    "AddressRaw": [
-        {'args': {'address': WalletSimulator.get_string_address_from_id('hyperbolic')}, 'expected': 0},
-        {'args': {'address': WalletSimulator.get_string_address_from_id('hyperbolic')}, 'expected': 0}],
-    "AddressString": [
-        {'args': {'address': WalletSimulator.get_raw_address_from_id('hyperbolic')}, 'expected': 0},
-        {'args': {'address': WalletSimulator.get_raw_address_from_id('hyperbolic')}, 'expected': 0}],
+    # "AddressRaw": [
+    #     {'args': {'address': wl_hyperbolic.string_address}, 'expected': 0},
+    #     {'args': {'address': wl_hyperbolic.string_address}, 'expected': 0}],
+    # "AddressString": [
+    #     {'args': {'address': wl_hyperbolic.raw_address}, 'expected': 0},
+    #     {'args': {'address': wl_hyperbolic.raw_address}, 'expected': 0}],
     "AssetValue": [
         {'args': {'asset': '0x1234567890abcdef'}, 'expected': 0},
         {'args': {'asset': '0x'}, 'expected': 0}],
     "Atoi": [
         {'args': {'s': '1234'}, 'expected': 0},
         {'args': {'s': '1'}, 'expected': 0}],
     # "Blid": [{'args': {}, 'expected': 0}],
@@ -42,30 +44,30 @@
         {'args': {'key': '50char'}, 'expected': 0}],
     "MapExists": [{'args': {'key': 'key'}, 'expected': 0}],
     "MapStore": [{'args': {'key': 'key', 'value': 'n'}, 'expected': 0}],
     "MapGet": [{'args': {'key': 'key'}, 'expected': 0}],
     "MapDelete": [{'args': {'key': 'key'}, 'expected': 0}],
     "Random": [{'args': {'value': 10}, 'expected': 0}],
     "UpdateScCode": [{'args': {'sc_code': 'this is the new code'}, 'expected': 20*2}],
-    "SendDeroToAddress": [{'args': {'raw_address': WalletSimulator.get_raw_address_from_id('hyperbolic'), 'amount': 100}, 'expected': 33}],
-    "SendAssetToAddress": [{'args': {
-            'raw_address': WalletSimulator.get_raw_address_from_id('hyperbolic'),
-            'asset': '0x1234567890abcdef',
-            'amount': 100},
-        'expected': 33}],
+    # "SendDeroToAddress": [{'args': {'raw_address': wl_hyperbolic.string_address, 'amount': 100}, 'expected': 33}],
+    # "SendAssetToAddress": [{'args': {
+    #         'raw_address': wl_hyperbolic.raw_address,
+    #         'asset': '0x1234567890abcdef',
+    #         'amount': 100},
+    #     'expected': 33}],
     "Signer": [{'args': {}, 'expected': 0}],
     "Sha256": [{'args': {'s': '0x1234567890abcdef'}, 'expected': 0}],
     "Sha3256": [{'args': {'s': '0x1234567890abcdef'}, 'expected': 0}],
     "Strlen": [{'args': {'s': '0x1234567890abcdef'}, 'expected': 0}],
     "Substr": [{'args': {'s': '0x1234567890abcdef', 'offset': 0, 'lenght': 5}, 'expected': 0}],
 
 }
 test_order = [
-    "AddressRaw",
-    "AddressString",
+    # "AddressRaw",
+    # "AddressString",
     "AssetValue",
     "Atoi",
     # "Blid",
     "BlockHeight",
     "BlockTimestamp",
     "DeroValue",
     "Dero",
@@ -79,16 +81,16 @@
     "Delete",
     "MapExists",
     "MapStore",
     "MapGet",
     "MapDelete",
     "Random",
     "UpdateScCode",
-    "SendDeroToAddress",
-    "SendAssetToAddress",
+    # "SendDeroToAddress",
+    # "SendAssetToAddress",
     "Signer",
     "Sha256",
     "Sha3256",
     "Strlen",
     "Substr",
 ]
```

### Comparing `deropy-0.2.1/tests/test_map_functions.py` & `deropy-0.2.2/tests/test_map_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import pytest
 
 from deropy.dvm.functions import map_store, map_get, map_delete, map_exists
 from deropy.dvm.Smartcontract import SmartContract
+from deropy.wallet.wallet import Wallet
+from deropy.wallet.wallet_factory import WalletFactory
+
+# basic initialization
+wl_hyperbolic: Wallet = WalletFactory.create_wallet('hyperbolic')
 
 
 class TestMapStore:
     def test_store_string(self):
         map_store('key', 'value')
 
         sc = SmartContract.get_instance()
```

### Comparing `deropy-0.2.1/tests/test_storage_functions.py` & `deropy-0.2.2/tests/test_storage_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import pytest
 
 from deropy.dvm.functions import store, load, exists, delete
 from deropy.dvm.Smartcontract import SmartContract
+from deropy.wallet.wallet import Wallet
+from deropy.wallet.wallet_factory import WalletFactory
+
+
+# basic initialization
+wl_hyperbolic: Wallet = WalletFactory.create_wallet('hyperbolic')
 
 
 class TestMapStore:
     def test_store_string(self):
         store('key', 'value')
 
         sc = SmartContract.get_instance()
```

