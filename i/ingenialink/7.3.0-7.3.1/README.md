# Comparing `tmp/ingenialink-7.3.0.tar.gz` & `tmp/ingenialink-7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingenialink-7.3.0.tar", last modified: Tue Apr 23 09:31:12 2024, max compression
+gzip compressed data, was "ingenialink-7.3.1.tar", last modified: Thu May  9 16:00:01 2024, max compression
```

## Comparing `ingenialink-7.3.0.tar` & `ingenialink-7.3.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/
--rw-rw-rw-   0        0        0    17630 2024-04-23 09:30:10.000000 ingenialink-7.3.0/LICENSE.md
--rw-rw-rw-   0        0        0       35 2024-04-23 09:30:10.000000 ingenialink-7.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2586 2024-04-23 09:31:12.681591 ingenialink-7.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2024-04-23 09:30:10.000000 ingenialink-7.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/
--rw-rw-rw-   0        0        0     1414 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/FoE/
--rw-rw-rw-   0        0        0       23 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/bin/FoE/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/FoE/linux/
--rw-rw-rw-   0        0        0   148512 2024-04-23 09:24:47.000000 ingenialink-7.3.0/ingenialink/bin/FoE/linux/FoEUpdateFirmware
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/FoE/win_64x/
--rwxrwxrwx   0        0        0    44032 2024-04-23 09:24:47.000000 ingenialink-7.3.0/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/bin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/canopen/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/__init__.py
--rw-rw-rw-   0        0        0     2779 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/dictionary.py
--rw-rw-rw-   0        0        0    38811 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/network.py
--rw-rw-rw-   0        0        0     2875 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/register.py
--rw-rw-rw-   0        0        0     5239 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/servo.py
--rw-rw-rw-   0        0        0      974 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/constants.py
--rw-rw-rw-   0        0        0    41826 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/dictionary.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/enums/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/enums/__init__.py
--rw-rw-rw-   0        0        0     1389 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/enums/register.py
--rw-rw-rw-   0        0        0     2892 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/enums/servo.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/eoe/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/eoe/__init__.py
--rw-rw-rw-   0        0        0    13578 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/eoe/network.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/ethercat/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/__init__.py
--rw-rw-rw-   0        0        0     6532 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/dictionary.py
--rw-rw-rw-   0        0        0    19540 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/network.py
--rw-rw-rw-   0        0        0      249 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/register.py
--rw-rw-rw-   0        0        0     9439 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/servo.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/ethernet/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/__init__.py
--rw-rw-rw-   0        0        0     2724 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/dictionary.py
--rw-rw-rw-   0        0        0    11937 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/network.py
--rw-rw-rw-   0        0        0     2823 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/register.py
--rw-rw-rw-   0        0        0     6068 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/servo.py
--rw-rw-rw-   0        0        0     3725 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/exceptions.py
--rw-rw-rw-   0        0        0     2412 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/network.py
--rw-rw-rw-   0        0        0    21882 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/pdo.py
--rw-rw-rw-   0        0        0     8024 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/poller.py
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/py.typed
--rw-rw-rw-   0        0        0     8649 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/register.py
--rw-rw-rw-   0        0        0    50678 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/servo.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.665944 ingenialink-7.3.0/ingenialink/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/__init__.py
--rw-rw-rw-   0        0        0     9012 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/_utils.py
--rw-rw-rw-   0        0        0     4486 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/constants.py
--rw-rw-rw-   0        0        0      684 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/errors.py
--rw-rw-rw-   0        0        0     7327 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/mcb.py
--rw-rw-rw-   0        0        0     4337 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/udp.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.665944 ingenialink-7.3.0/ingenialink/virtual/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/__init__.py
--rw-rw-rw-   0        0        0     3224 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/dictionary.py
--rw-rw-rw-   0        0        0     2094 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/network.py
--rw-rw-rw-   0        0        0      315 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/servo.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/ingenialink.egg-info/
--rw-rw-rw-   0        0        0     2586 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1824 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2024-04-23 09:30:10.000000 ingenialink-7.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 09:31:12.681591 ingenialink-7.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1775 2024-04-23 09:30:10.000000 ingenialink-7.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/tests/
--rw-rw-rw-   0        0        0     7579 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_dictionary.py
--rw-rw-rw-   0        0        0     3157 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_mcb.py
--rw-rw-rw-   0        0        0     7922 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_register.py
--rw-rw-rw-   0        0        0    16973 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_servo.py
--rw-rw-rw-   0        0        0      914 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_utils.py
--rw-rw-rw-   0        0        0     7966 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_virtual_drive.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/virtual_drive/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/__init__.py
--rw-rw-rw-   0        0        0    68129 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/core.py
--rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/virtual_drive/resources/
--rw-rw-rw-   0        0        0    29066 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xcf
--rw-rw-rw-   0        0        0   267648 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xdf
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.647783 ingenialink-7.3.1/
+-rw-rw-rw-   0        0        0    17630 2024-05-09 15:59:10.000000 ingenialink-7.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0       35 2024-05-09 15:59:10.000000 ingenialink-7.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2586 2024-05-09 16:00:01.647783 ingenialink-7.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2024-05-09 15:59:10.000000 ingenialink-7.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.616532 ingenialink-7.3.1/ingenialink/
+-rw-rw-rw-   0        0        0     1394 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.616532 ingenialink-7.3.1/ingenialink/bin/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/bin/FoE/
+-rw-rw-rw-   0        0        0       23 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/bin/FoE/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/bin/FoE/linux/
+-rw-rw-rw-   0        0        0   148512 2024-05-09 15:53:05.000000 ingenialink-7.3.1/ingenialink/bin/FoE/linux/FoEUpdateFirmware
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/bin/FoE/win_64x/
+-rwxrwxrwx   0        0        0    44032 2024-05-09 15:53:05.000000 ingenialink-7.3.1/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/bin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/canopen/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/canopen/__init__.py
+-rw-rw-rw-   0        0        0     2779 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/canopen/dictionary.py
+-rw-rw-rw-   0        0        0    39765 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/canopen/network.py
+-rw-rw-rw-   0        0        0     2875 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/canopen/register.py
+-rw-rw-rw-   0        0        0     5383 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/canopen/servo.py
+-rw-rw-rw-   0        0        0      974 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/constants.py
+-rw-rw-rw-   0        0        0    41826 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/dictionary.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/enums/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/enums/__init__.py
+-rw-rw-rw-   0        0        0     1389 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/enums/register.py
+-rw-rw-rw-   0        0        0     2892 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/enums/servo.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/eoe/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/eoe/__init__.py
+-rw-rw-rw-   0        0        0    13578 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/eoe/network.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/ethercat/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethercat/__init__.py
+-rw-rw-rw-   0        0        0     6532 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethercat/dictionary.py
+-rw-rw-rw-   0        0        0    19856 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethercat/network.py
+-rw-rw-rw-   0        0        0      249 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethercat/register.py
+-rw-rw-rw-   0        0        0     9439 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethercat/servo.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.632169 ingenialink-7.3.1/ingenialink/ethernet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethernet/__init__.py
+-rw-rw-rw-   0        0        0     2724 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethernet/dictionary.py
+-rw-rw-rw-   0        0        0    11937 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethernet/network.py
+-rw-rw-rw-   0        0        0     2823 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethernet/register.py
+-rw-rw-rw-   0        0        0     6068 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/ethernet/servo.py
+-rw-rw-rw-   0        0        0     3725 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/exceptions.py
+-rw-rw-rw-   0        0        0     2412 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/network.py
+-rw-rw-rw-   0        0        0    21882 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/pdo.py
+-rw-rw-rw-   0        0        0     8024 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/poller.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/py.typed
+-rw-rw-rw-   0        0        0     8649 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/register.py
+-rw-rw-rw-   0        0        0    50937 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/servo.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.647783 ingenialink-7.3.1/ingenialink/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/utils/__init__.py
+-rw-rw-rw-   0        0        0     9012 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/utils/_utils.py
+-rw-rw-rw-   0        0        0     4486 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/utils/constants.py
+-rw-rw-rw-   0        0        0      684 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/utils/errors.py
+-rw-rw-rw-   0        0        0     7327 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/utils/mcb.py
+-rw-rw-rw-   0        0        0     4337 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/utils/udp.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.647783 ingenialink-7.3.1/ingenialink/virtual/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/virtual/__init__.py
+-rw-rw-rw-   0        0        0     3224 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/virtual/dictionary.py
+-rw-rw-rw-   0        0        0     2094 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/virtual/network.py
+-rw-rw-rw-   0        0        0      315 2024-05-09 15:59:10.000000 ingenialink-7.3.1/ingenialink/virtual/servo.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.647783 ingenialink-7.3.1/ingenialink.egg-info/
+-rw-rw-rw-   0        0        0     2586 2024-05-09 16:00:01.000000 ingenialink-7.3.1/ingenialink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1824 2024-05-09 16:00:01.000000 ingenialink-7.3.1/ingenialink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 16:00:01.000000 ingenialink-7.3.1/ingenialink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2024-05-09 16:00:01.000000 ingenialink-7.3.1/ingenialink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 16:00:01.000000 ingenialink-7.3.1/ingenialink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2024-05-09 15:59:10.000000 ingenialink-7.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 16:00:01.647783 ingenialink-7.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1775 2024-05-09 15:59:10.000000 ingenialink-7.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.647783 ingenialink-7.3.1/tests/
+-rw-rw-rw-   0        0        0     7579 2024-05-09 15:59:10.000000 ingenialink-7.3.1/tests/test_dictionary.py
+-rw-rw-rw-   0        0        0     3157 2024-05-09 15:59:10.000000 ingenialink-7.3.1/tests/test_mcb.py
+-rw-rw-rw-   0        0        0     7922 2024-05-09 15:59:10.000000 ingenialink-7.3.1/tests/test_register.py
+-rw-rw-rw-   0        0        0    17121 2024-05-09 15:59:10.000000 ingenialink-7.3.1/tests/test_servo.py
+-rw-rw-rw-   0        0        0      914 2024-05-09 15:59:10.000000 ingenialink-7.3.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0     7966 2024-05-09 15:59:10.000000 ingenialink-7.3.1/tests/test_virtual_drive.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.647783 ingenialink-7.3.1/virtual_drive/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/virtual_drive/__init__.py
+-rw-rw-rw-   0        0        0    68129 2024-05-09 15:59:10.000000 ingenialink-7.3.1/virtual_drive/core.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:59:10.000000 ingenialink-7.3.1/virtual_drive/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-09 16:00:01.647783 ingenialink-7.3.1/virtual_drive/resources/
+-rw-rw-rw-   0        0        0    29066 2024-05-09 15:59:10.000000 ingenialink-7.3.1/virtual_drive/resources/virtual_drive.xcf
+-rw-rw-rw-   0        0        0   267648 2024-05-09 15:59:10.000000 ingenialink-7.3.1/virtual_drive/resources/virtual_drive.xdf
```

### Comparing `ingenialink-7.3.0/LICENSE.md` & `ingenialink-7.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/PKG-INFO` & `ingenialink-7.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ingenialink
-Version: 7.3.0
+Version: 7.3.1
 Summary: IngeniaLink Communications Library
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.3.0
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.3.1
 Project-URL: Source, https://github.com/ingeniamc/ingenialink-python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ingenialink-7.3.0/README.rst` & `ingenialink-7.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/__init__.py` & `ingenialink-7.3.1/ingenialink/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from .network import NET_PROT, NET_STATE, NET_DEV_EVT, NET_TRANS_PROT, Network, EEPROM_FILE_FORMAT
+from ingenialink.enums.register import REG_ACCESS, REG_DTYPE, REG_PHY
 from ingenialink.enums.servo import (
-    SERVO_STATE,
     SERVO_FLAGS,
     SERVO_MODE,
-    SERVO_UNITS_TORQUE,
+    SERVO_STATE,
+    SERVO_UNITS_ACC,
     SERVO_UNITS_POS,
+    SERVO_UNITS_TORQUE,
     SERVO_UNITS_VEL,
-    SERVO_UNITS_ACC,
 )
+from ingenialink.poller import Poller
 from ingenialink.servo import Servo
 
+from .canopen.dictionary import CanopenDictionaryV2
+from .canopen.network import CAN_BAUDRATE, CAN_DEVICE, CanopenNetwork
+from .canopen.register import CanopenRegister
+from .canopen.servo import CanopenServo
+from .ethercat.network import EthercatNetwork
 from .ethernet.network import EthernetNetwork
 from .ethernet.servo import EthernetServo
-
-from .ethercat.network import EthercatNetwork
-
-from .canopen.servo import CanopenServo
-from .canopen.network import CanopenNetwork, CAN_DEVICE, CAN_DEVICE, CAN_BAUDRATE
-from .canopen.register import CanopenRegister
-from .canopen.dictionary import CanopenDictionaryV2
-
-from ingenialink.enums.register import REG_DTYPE, REG_ACCESS, REG_PHY
-
-from ingenialink.poller import Poller
+from .network import EEPROM_FILE_FORMAT, NET_DEV_EVT, NET_PROT, NET_STATE, NET_TRANS_PROT, Network
 
 __all__ = [
     "EEPROM_FILE_FORMAT",
     "NET_PROT",
     "NET_DEV_EVT",
     "NET_STATE",
     "NET_TRANS_PROT",
@@ -50,8 +46,8 @@
     "CAN_BAUDRATE",
     "CanopenServo",
     "CanopenRegister",
     "Poller",
     "CanopenDictionaryV2",
 ]
 
-__version__ = "7.3.0"
+__version__ = "7.3.1"
```

### Comparing `ingenialink-7.3.0/ingenialink/bin/FoE/linux/FoEUpdateFirmware` & `ingenialink-7.3.1/ingenialink/bin/FoE/linux/FoEUpdateFirmware`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe` & `ingenialink-7.3.1/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/canopen/dictionary.py` & `ingenialink-7.3.1/ingenialink/canopen/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/canopen/network.py` & `ingenialink-7.3.1/ingenialink/canopen/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import tempfile
 from collections import OrderedDict, defaultdict
 from enum import Enum
 from threading import Thread
 from time import sleep
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+import can
 import canopen
 import ingenialogger
 from can import CanError
 
 
 from ingenialink.canopen.register import CanopenRegister
 from ingenialink.canopen.servo import (
@@ -129,14 +130,30 @@
     CAN_BAUDRATE.Baudrate_250K: 3,
     CAN_BAUDRATE.Baudrate_125K: 4,
     CAN_BAUDRATE.Baudrate_100K: 5,
     CAN_BAUDRATE.Baudrate_50K: 6,
 }
 
 
+class CustomIXXATListener(can.Listener):
+    """Custom listener for IXXAT connection.
+    It is used to ignore the exceptions that occur when
+    the error limit is reached.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def on_message_received(self, msg: can.Message) -> None:
+        pass
+
+    def on_error(self, exc: Exception) -> None:
+        logger.error(f"An exception occurred with the IXXAT connection. Exception: {exc}")
+
+
 class NetStatusListener(Thread):
     """Network status listener thread to check if the drive is alive.
 
     Args:
         network: Network instance of the CANopen communication.
 
     """
@@ -183,14 +200,15 @@
         baudrate: Baudrate to communicate through.
 
     """
 
     DRIVE_INFO_INDEX = 0x1018
     PRODUCT_CODE_SUB_IX = 2
     REVISION_NUMBER_SUB_IX = 3
+    NODE_GUARDING_PERIOD_S = 1
 
     def __init__(
         self,
         device: CAN_DEVICE,
         channel: int = 0,
         baudrate: CAN_BAUDRATE = CAN_BAUDRATE.Baudrate_1M,
     ):
@@ -210,14 +228,22 @@
         self.__observers_fw_load_progress: List[Callable[[int], Any]] = []
         self.__observers_fw_load_errors_enabled: List[Callable[[bool], Any]] = []
 
         self.__fw_load_status_msg = ""
         self.__fw_load_progress = 0
         self.__fw_load_errors_enabled = True
 
+        self.__connection_args = {
+            "bustype": self.__device,
+            "channel": self.__channel,
+            "bitrate": self.__baudrate,
+        }
+        if self.__device == CAN_DEVICE.PCAN.value:
+            self.__connection_args["auto_reset"] = True
+
     def scan_slaves(self) -> List[int]:
         """Scans for nodes in the network.
 
         Returns:
             Containing all the detected node IDs.
 
         """
@@ -322,15 +348,15 @@
         self._setup_connection()
         if self._connection is None:
             raise ILError("Connection has not been established")
         if target in nodes:
             try:
                 node = self._connection.add_node(target)
 
-                node.nmt.start_node_guarding(1)
+                node.nmt.start_node_guarding(self.NODE_GUARDING_PERIOD_S)
 
                 servo = CanopenServo(
                     target, node, dictionary, servo_status_listener=servo_status_listener
                 )
                 self.servos.append(servo)
                 self._set_servo_state(target, NET_STATE.CONNECTED)
                 if net_status_listener:
@@ -358,85 +384,85 @@
         servo.stop_status_listener()
         self.servos.remove(servo)
         if not self.servos:
             self._teardown_connection()
 
     def _setup_connection(self) -> None:
         """Creates a network interface object establishing an empty connection
-        with all the network attributes already specified."""
+        with all the network attributes already specified.
+
+        """
         if self._connection is None:
             self._connection = canopen.Network()
-            connection_args = {
-                "bustype": self.__device,
-                "channel": self.__channel,
-                "bitrate": self.__baudrate,
-            }
-            if self.__device == CAN_DEVICE.PCAN.value:
-                connection_args["auto_reset"] = True
+            if self.__device == CAN_DEVICE.IXXAT.value:
+                self._connection.listeners.append(CustomIXXATListener())
             try:
-                self._connection.connect(**connection_args)
+                self._connection.connect(**self.__connection_args)
             except CanError as e:
-                logger.error("Transceiver not found in network. Exception: %s", e)
+                logger.error(f"Transceiver not found in network. Exception: {e}")
                 raise ILError(
                     "Error connecting to the transceiver. "
                     "Please verify the transceiver "
                     "is properly connected."
                 )
             except OSError as e:
-                logger.error("Transceiver drivers not properly installed. Exception: %s", e)
+                logger.error(f"Transceiver drivers not properly installed. Exception: {e}")
                 if hasattr(e, "winerror") and e.winerror == 126:
                     e.strerror = "Driver module not found. Drivers might not be properly installed."
                 raise ILError(e)
             except Exception as e:
-                logger.error("Failed trying to connect. Exception: %s", e)
-                raise ILError("Failed trying to connect. {}".format(e))
+                error_message = f"Failed trying to connect. Exception: {e}"
+                logger.error(error_message)
+                raise ILError(error_message)
         else:
             logger.info("Connection already established")
 
     def _teardown_connection(self) -> None:
         """Tears down the already established connection
         and deletes the network interface"""
         if self._connection is None:
             logger.warning("Can not disconnect. The connection is not established yet.")
             return
-        self._connection.disconnect()
+        try:
+            self._connection.disconnect()
+        except VCIError as e:
+            logger.error(f"An exception occurred during the teardown connection. Exception: {e}")
         self._connection = None
         logger.info("Tear down connection.")
 
     def _reset_connection(self) -> None:
         """Resets the established CANopen network.
 
         Raises:
             ILError: If the connection was not established yet.
         """
         if self._connection is None:
             raise ILError("Can not reset connection. The connection is not established yet.")
         try:
             self._connection.disconnect()
         except BaseException as e:
-            logger.error("Disconnection failed. Exception: %", e)
+            logger.error(f"Disconnection failed. Exception: {e}")
 
         try:
             for node in self._connection.scanner.nodes:
                 self._connection.nodes[node].nmt.stop_node_guarding()
             if self._connection.bus:
                 self._connection.bus.flush_tx_buffer()
                 logger.info("Bus flushed")
         except Exception as e:
-            logger.error("Could not stop guarding. Exception: %", e)
-
+            logger.error(f"Could not stop guarding. Exception: {e}")
+        if self.__device == CAN_DEVICE.IXXAT.value:
+            self._connection.listeners.append(CustomIXXATListener())
         try:
-            self._connection.connect(
-                bustype=self.__device, channel=self.__channel, bitrate=self.__baudrate
-            )
+            self._connection.connect(**self.__connection_args)
             for servo in self.servos:
-                node = self._connection.add_node(servo.target)
-                node.nmt.start_node_guarding(1)
+                servo.node = self._connection.add_node(servo.target)
+                servo.node.nmt.start_node_guarding(self.NODE_GUARDING_PERIOD_S)
         except BaseException as e:
-            logger.error("Connection failed. Exception: %s", e)
+            logger.error(f"Connection failed. Exception: {e}")
 
     def load_firmware(  # type: ignore [override]
         self,
         target: int,
         fw_file: str,
         callback_status_msg: Optional[Callable[[str], None]] = None,
         callback_progress: Optional[Callable[[int], None]] = None,
@@ -947,15 +973,15 @@
         for servo in self.servos:
             logger.info("Node connected: %i", servo.target)
             node = self._connection.add_node(servo.target)
 
         # Reset all nodes to default state
         self._connection.lss.send_switch_state_global(self._connection.lss.WAITING_STATE)
 
-        self._connection.nodes[target_node].nmt.start_node_guarding(1)
+        self._connection.nodes[target_node].nmt.start_node_guarding(self.NODE_GUARDING_PERIOD_S)
 
     def subscribe_to_status(self, node_id: int, callback: Callable[[NET_DEV_EVT], Any]) -> None:  # type: ignore [override]
         """Subscribe to network state changes.
 
         Args:
             node_id: Drive's node ID.
             callback: Callback function.
```

### Comparing `ingenialink-7.3.0/ingenialink/canopen/register.py` & `ingenialink-7.3.1/ingenialink/canopen/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/canopen/servo.py` & `ingenialink-7.3.1/ingenialink/canopen/servo.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,7 +147,12 @@
             subnode, ipb_address, dtype, size
         )
 
     @property
     def node(self) -> canopen.RemoteNode:
         """Remote node of the servo."""
         return self.__node
+
+    @node.setter
+    def node(self, node: canopen.RemoteNode) -> None:
+        """Remote node of the servo."""
+        self.__node = node
```

### Comparing `ingenialink-7.3.0/ingenialink/constants.py` & `ingenialink-7.3.1/ingenialink/constants.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/dictionary.py` & `ingenialink-7.3.1/ingenialink/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/enums/register.py` & `ingenialink-7.3.1/ingenialink/enums/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/enums/servo.py` & `ingenialink-7.3.1/ingenialink/enums/servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/eoe/network.py` & `ingenialink-7.3.1/ingenialink/eoe/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/ethercat/dictionary.py` & `ingenialink-7.3.1/ingenialink/ethercat/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/ethercat/network.py` & `ingenialink-7.3.1/ingenialink/ethercat/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,20 +446,28 @@
                     check=True,
                     shell=True,
                     encoding="utf-8",
                 )
             except subprocess.CalledProcessError as e:
                 raise ILFirmwareLoadError("Could not change the FoE binary permissions.") from e
         try:
-            subprocess.run(
-                f"{exec_path} {self.interface_name} {slave_id} {fw_file}",
-                check=True,
-                shell=True,
-                encoding="utf-8",
-            )
+            if sys_name == "linux":
+                subprocess.run(
+                    f"{exec_path} {self.interface_name} {slave_id} {fw_file}",
+                    check=True,
+                    shell=True,
+                    encoding="utf-8",
+                )
+            else:
+                subprocess.run(
+                    [exec_path, self.interface_name, f"{slave_id}", fw_file],
+                    check=True,
+                    shell=True,
+                    encoding="utf-8",
+                )
         except subprocess.CalledProcessError as e:
             foe_return_error = self.FOE_ERRORS.get(e.returncode, self.UNKNOWN_FOE_ERROR)
             raise ILFirmwareLoadError(
                 f"The firmware file could not be loaded correctly. {foe_return_error}"
             ) from e
         logger.info("Firmware updated successfully")
```

### Comparing `ingenialink-7.3.0/ingenialink/ethercat/servo.py` & `ingenialink-7.3.1/ingenialink/ethercat/servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/ethernet/dictionary.py` & `ingenialink-7.3.1/ingenialink/ethernet/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/ethernet/network.py` & `ingenialink-7.3.1/ingenialink/ethernet/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/ethernet/register.py` & `ingenialink-7.3.1/ingenialink/ethernet/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/ethernet/servo.py` & `ingenialink-7.3.1/ingenialink/ethernet/servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/exceptions.py` & `ingenialink-7.3.1/ingenialink/exceptions.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/network.py` & `ingenialink-7.3.1/ingenialink/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/pdo.py` & `ingenialink-7.3.1/ingenialink/pdo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/poller.py` & `ingenialink-7.3.1/ingenialink/poller.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/register.py` & `ingenialink-7.3.1/ingenialink/register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/servo.py` & `ingenialink-7.3.1/ingenialink/servo.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,17 @@
     DIST_DATA = "DISTURBANCE_DATA"
     MONITORING_ACTUAL_NUMBER_SAMPLES = "MON_CFG_CYCLES_VALUE"
     DISTURBANCE_REMOVE_REGISTERS_OLD = "DIST_CMD_RM_REGS"
     MONITORING_REMOVE_REGISTERS_OLD = "MON_CMD_RM_REG"
     DISTURBANCE_ADD_REGISTERS_OLD = "DIST_CMD_ADD_REG"
     MONITORING_ADD_REGISTERS_OLD = "MON_OP_ADD_REG"
 
+    DICTIONARY_INTERFACE_ATTR_CAN = "CAN"
+    DICTIONARY_INTERFACE_ATTR_ETH = "ETH"
+
     interface: Interface
 
     def __init__(
         self,
         target: Union[int, str],
         dictionary_path: str,
         servo_status_listener: bool = False,
@@ -332,16 +335,20 @@
         version.text = "2"
         default_language = ET.SubElement(header, "DefaultLanguage")
         default_language.text = "en_US"
 
         body = ET.SubElement(tree, "Body")
         device = ET.SubElement(body, "Device")
         registers = ET.SubElement(device, "Registers")
-
-        device.set("Interface", str(self.dictionary.interface))
+        interface = (
+            self.DICTIONARY_INTERFACE_ATTR_CAN
+            if self.dictionary.interface == Interface.CAN
+            else self.DICTIONARY_INTERFACE_ATTR_ETH
+        )
+        device.set("Interface", interface)
         if self.dictionary.part_number is not None:
             device.set("PartNumber", self.dictionary.part_number)
         device.set("ProductCode", str(prod_code))
         device.set("RevisionNumber", str(rev_number))
         device.set("firmwareVersion", str(self.dictionary.firmware_version))
 
         access_ops = {value: key for key, value in self.dictionary.access_xdf_options.items()}
```

### Comparing `ingenialink-7.3.0/ingenialink/utils/_utils.py` & `ingenialink-7.3.1/ingenialink/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/utils/constants.py` & `ingenialink-7.3.1/ingenialink/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/utils/errors.py` & `ingenialink-7.3.1/ingenialink/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/utils/mcb.py` & `ingenialink-7.3.1/ingenialink/utils/mcb.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/utils/udp.py` & `ingenialink-7.3.1/ingenialink/utils/udp.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/virtual/dictionary.py` & `ingenialink-7.3.1/ingenialink/virtual/dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink/virtual/network.py` & `ingenialink-7.3.1/ingenialink/virtual/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/ingenialink.egg-info/PKG-INFO` & `ingenialink-7.3.1/ingenialink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ingenialink
-Version: 7.3.0
+Version: 7.3.1
 Summary: IngeniaLink Communications Library
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.3.0
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.3.1
 Project-URL: Source, https://github.com/ingeniamc/ingenialink-python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ingenialink-7.3.0/ingenialink.egg-info/SOURCES.txt` & `ingenialink-7.3.1/ingenialink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/setup.py` & `ingenialink-7.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/tests/test_dictionary.py` & `ingenialink-7.3.1/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/tests/test_mcb.py` & `ingenialink-7.3.1/tests/test_mcb.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/tests/test_register.py` & `ingenialink-7.3.1/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/tests/test_servo.py` & `ingenialink-7.3.1/tests/test_servo.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,20 @@
     if "RevisionNumber" in device.attrib and rev_number is not None:
         assert int(device.attrib.get("RevisionNumber")) == rev_number
 
     if servo.dictionary.part_number is None:
         assert "PartNumber" not in device.attrib
     else:
         assert device.attrib["PartNumber"] == servo.dictionary.part_number
-    assert device.attrib.get("Interface") == servo.dictionary.interface
+    interface = (
+        servo.DICTIONARY_INTERFACE_ATTR_CAN
+        if isinstance(servo, CanopenServo)
+        else servo.DICTIONARY_INTERFACE_ATTR_ETH
+    )
+    assert device.attrib.get("Interface") == interface
     assert device.attrib.get("firmwareVersion") == servo.dictionary.firmware_version
     # TODO: check name and family? These are not stored at the dictionary
 
     assert len(saved_registers) > 0
     for saved_register in saved_registers:
         subnode = int(saved_register.attrib.get("subnode"))
```

### Comparing `ingenialink-7.3.0/tests/test_utils.py` & `ingenialink-7.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/tests/test_virtual_drive.py` & `ingenialink-7.3.1/tests/test_virtual_drive.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/virtual_drive/core.py` & `ingenialink-7.3.1/virtual_drive/core.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xcf` & `ingenialink-7.3.1/virtual_drive/resources/virtual_drive.xcf`

 * *Files identical despite different names*

### Comparing `ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xdf` & `ingenialink-7.3.1/virtual_drive/resources/virtual_drive.xdf`

 * *Files identical despite different names*

