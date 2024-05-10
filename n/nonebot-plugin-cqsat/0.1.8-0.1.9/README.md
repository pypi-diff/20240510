# Comparing `tmp/nonebot-plugin-cqsat-0.1.8.tar.gz` & `tmp/nonebot-plugin-cqsat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cqsat-0.1.8.tar", last modified: Mon Sep 11 17:52:22 2023, max compression
+gzip compressed data, was "nonebot-plugin-cqsat-0.1.9.tar", last modified: Thu Sep 28 18:29:35 2023, max compression
```

## Comparing `nonebot-plugin-cqsat-0.1.8.tar` & `nonebot-plugin-cqsat-0.1.9.tar`

### file list

```diff
@@ -1,93 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.588525 nonebot-plugin-cqsat-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2023-09-11 17:52:22.588525 nonebot-plugin-cqsat-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.572525 nonebot-plugin-cqsat-0.1.8/cqsat/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.572525 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.576525 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/
--rw-r--r--   0 runner    (1001) docker     (127)   161387 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/A.json
--rw-r--r--   0 runner    (1001) docker     (127)   282636 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/B.json
--rw-r--r--   0 runner    (1001) docker     (127)   442381 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/C.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.584525 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0497.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0498.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0499.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0500.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0501.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0502.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    17027 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0503.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0504.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0505.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0506.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0507.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0508.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0509.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0510.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0511.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    13831 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0594.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0595.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0596.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0597.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    11752 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0598.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0599.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0600.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0601.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0602.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    12424 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0603.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    37302 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0604.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    68550 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0605.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    52089 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0606.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    45355 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0607.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    52629 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0608.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    43611 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0609.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    18311 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0610.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47079 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0611.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    26943 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0612.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    60117 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0613.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    33774 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0614.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    62805 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0734.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    52168 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0735.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    55498 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0736.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    58412 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0740.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    57669 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0741.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    56133 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0742.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    57173 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0743.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    56601 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0744.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    55239 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0745.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   107908 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0927.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   107610 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0928.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    95560 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0938.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    28026 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0941.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    72144 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0942.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   127576 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0943.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    73505 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0944.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   126097 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0945.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.584525 nonebot-plugin-cqsat-0.1.8/cqsat/exercise/
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/exercise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/exercise/exam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.584525 nonebot-plugin-cqsat-0.1.8/cqsat/mgsl/
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/mgsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/mgsl/calculate_mgsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.584525 nonebot-plugin-cqsat-0.1.8/cqsat/pre/
--rw-r--r--   0 runner    (1001) docker     (127)   121993 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/pre/A.txt
--rw-r--r--   0 runner    (1001) docker     (127)   207947 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/pre/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)   326871 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/pre/C.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/pre/pre.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.584525 nonebot-plugin-cqsat-0.1.8/cqsat/sat/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/sat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/sat/calculate_sat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/sat/sat_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/cqsat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 17:52:22.588525 nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2023-09-11 17:52:22.000000 nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2023-09-11 17:52:22.000000 nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-11 17:52:22.000000 nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-11 17:52:22.000000 nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-11 17:52:22.000000 nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-11 17:52:22.588525 nonebot-plugin-cqsat-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-11 17:52:11.000000 nonebot-plugin-cqsat-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.276964 nonebot-plugin-cqsat-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2023-09-28 18:29:35.276964 nonebot-plugin-cqsat-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.256964 nonebot-plugin-cqsat-0.1.9/cqsat/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.252964 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.256964 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/
+-rw-r--r--   0 runner    (1001) docker     (127)   161387 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/A.json
+-rw-r--r--   0 runner    (1001) docker     (127)   282636 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/B.json
+-rw-r--r--   0 runner    (1001) docker     (127)   442381 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/C.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.268964 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0497.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0498.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0499.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0500.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0501.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0502.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    17027 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0503.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0504.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0505.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0506.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0507.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0508.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0509.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0510.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0511.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    13831 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0594.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0595.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0596.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0597.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0598.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0599.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0600.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0601.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0602.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0603.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    37302 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0604.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    68550 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0605.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    52089 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0606.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    45355 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0607.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    52629 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0608.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    43611 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0609.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    18311 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0610.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47079 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0611.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    26943 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0612.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    60117 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0613.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    33774 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0614.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    62805 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0734.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    52168 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0735.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    55498 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0736.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    58412 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0740.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    57669 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0741.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    56133 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0742.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    57173 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0743.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    56601 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0744.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    55239 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0745.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   107908 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0927.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   107610 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0928.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    95560 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0938.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    28026 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0941.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    72144 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0942.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   127576 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0943.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    73505 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0944.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   126097 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0945.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.252964 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/voices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.268964 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/voices/prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/voices/prefix/unknown_pre.mp3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.268964 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/voices/suffix/
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/voices/suffix/mdc1200.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/voices/suffix/mdc1200_2.mp3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.268964 nonebot-plugin-cqsat-0.1.9/cqsat/entertainment/
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/entertainment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.272964 nonebot-plugin-cqsat-0.1.9/cqsat/exercise/
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/exercise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/exercise/exam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/media_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.272964 nonebot-plugin-cqsat-0.1.9/cqsat/mgsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/mgsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/mgsl/calculate_mgsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.272964 nonebot-plugin-cqsat-0.1.9/cqsat/pre/
+-rw-r--r--   0 runner    (1001) docker     (127)   121993 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/pre/A.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   207947 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/pre/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   326871 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/pre/C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/pre/pre.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.272964 nonebot-plugin-cqsat-0.1.9/cqsat/sat/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/sat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/sat/calculate_sat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17542 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/sat/sat_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/cqsat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 18:29:35.272964 nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2023-09-28 18:29:35.000000 nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-09-28 18:29:35.000000 nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 18:29:35.000000 nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-28 18:29:35.000000 nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-28 18:29:35.000000 nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 18:29:35.276964 nonebot-plugin-cqsat-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-28 18:29:22.000000 nonebot-plugin-cqsat-0.1.9/setup.py
```

### Comparing `nonebot-plugin-cqsat-0.1.8/LICENSE` & `nonebot-plugin-cqsat-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/PKG-INFO` & `nonebot-plugin-cqsat-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cqsat
-Version: 0.1.8
+Version: 0.1.9
 Summary: nonebot2 业余无线电卫星
 Home-page: https://github.com/yzyyz1387/cqsat
 Author: yzyyz1387
 Author-email: youzyyz1384@gmail.com
 Keywords: ham,nonebot2,nonebot,radio,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -226,14 +226,24 @@
 <details>
   <summary> <h3>点击查看截图</h3></summary>
 
 ![](img/readme/cancel.gif)
 
 </details>
 
+### 查看Tevel系列卫星截图
+- 发送`/t` 即可查看网站https://www.df2et.de/tevel/的截图
+
+
+### 娱乐信令
+- 发送`/v` ，根据提示回复一条语音，即可对该语音加上信令音
+- 可选参数
+  - `-p` 加前置音 例如：`/v -p`
+  - `-n[数字]` 加噪音 例如：`/v -n5`
+
 ### 网格 【私聊、群内】
 
 - 发送 `我的网格` 查询用户绑定qth的网格
 - 发送 `计算网格 +地名` 计算指定地址的网格，如 `计算网格 北京`
 - 发送 `计算网格+经度+  +纬度` 计算指定位置的网格 经纬度用空格分隔
   - 不加经纬度相当于 `我的网格` 指令
 
@@ -277,13 +287,14 @@
 
 - [X]  追星
 - [X]  相关计算
 - [X]  刷题
 - [ ]  刷题错误记录、常错记录
 - [ ]  模拟考试
 - [ ]  卫星状态、卫星列表加入图片支持
+- [ ]  [#5](https://github.com/yzyyz1387/cqsat/issues/5)
 
 ## 参考资料
 
 [PyEphem Home Page — PyEphem home page (rhodesmill.org)](https://rhodesmill.org/pyephem/)
 
 刁宁辉,刘建强,孙从容,等. 基于SGP4模型的卫星轨道计算[J]. 遥感信息,2012,27(4):64-70. DOI:10.3969/j.issn.1000-3177.2012.04.011.
```

### Comparing `nonebot-plugin-cqsat-0.1.8/README.md` & `nonebot-plugin-cqsat-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -204,14 +204,24 @@
 <details>
   <summary> <h3>点击查看截图</h3></summary>
 
 ![](img/readme/cancel.gif)
 
 </details>
 
+### 查看Tevel系列卫星截图
+- 发送`/t` 即可查看网站https://www.df2et.de/tevel/的截图
+
+
+### 娱乐信令
+- 发送`/v` ，根据提示回复一条语音，即可对该语音加上信令音
+- 可选参数
+  - `-p` 加前置音 例如：`/v -p`
+  - `-n[数字]` 加噪音 例如：`/v -n5`
+
 ### 网格 【私聊、群内】
 
 - 发送 `我的网格` 查询用户绑定qth的网格
 - 发送 `计算网格 +地名` 计算指定地址的网格，如 `计算网格 北京`
 - 发送 `计算网格+经度+  +纬度` 计算指定位置的网格 经纬度用空格分隔
   - 不加经纬度相当于 `我的网格` 指令
 
@@ -255,13 +265,14 @@
 
 - [X]  追星
 - [X]  相关计算
 - [X]  刷题
 - [ ]  刷题错误记录、常错记录
 - [ ]  模拟考试
 - [ ]  卫星状态、卫星列表加入图片支持
+- [ ]  [#5](https://github.com/yzyyz1387/cqsat/issues/5)
 
 ## 参考资料
 
 [PyEphem Home Page — PyEphem home page (rhodesmill.org)](https://rhodesmill.org/pyephem/)
 
 刁宁辉,刘建强,孙从容,等. 基于SGP4模型的卫星轨道计算[J]. 遥感信息,2012,27(4):64-70. DOI:10.3969/j.issn.1000-3177.2012.04.011.
```

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/__init__.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 # @Time    : 2022/8/21 2:09
 # @Author  : yzyyz
 # @Email   :  youzyyz1384@qq.com
 # @File    : __init__.py.py
 # @Software: PyCharm
 from . import (
     exercise,
+    entertainment,
     mgsl,
     sat,
+    config,
     log,
     path,
-    utils
+    utils,
+    media_utils
                )
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="HAM助手",
     description="业余无线电相关工具",
     usage="可刷题、模拟考试，追踪卫星等",
```

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/A.json` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/A.json`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/B.json` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/B.json`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/C.json` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/C.json`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0497.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0497.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0498.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0498.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0499.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0499.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0500.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0500.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0501.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0501.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0502.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0502.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0503.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0503.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0504.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0504.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0505.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0505.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0506.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0506.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0507.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0507.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0508.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0508.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0509.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0509.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0510.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0510.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0511.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0511.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0594.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0594.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0595.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0595.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0596.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0596.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0597.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0597.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0598.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0598.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0599.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0599.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0600.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0600.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0601.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0601.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0602.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0602.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0603.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0603.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0604.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0604.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0605.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0605.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0606.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0606.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0607.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0607.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0608.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0608.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0609.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0609.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0610.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0610.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0611.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0611.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0612.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0612.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0613.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0613.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0614.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0614.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0734.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0734.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0735.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0735.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0736.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0736.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0740.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0740.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0741.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0741.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0742.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0742.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0743.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0743.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0744.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0744.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0745.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0745.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0927.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0927.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0928.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0928.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0938.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0938.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0941.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0941.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0942.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0942.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0943.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0943.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0944.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0944.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/cqsat_resource/bank/imgs/LK0945.jpg` & `nonebot-plugin-cqsat-0.1.9/cqsat/cqsat_resource/bank/imgs/LK0945.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/exercise/__init__.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/exercise/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/exercise/exam.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/exercise/exam.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/log.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/log.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/mgsl/__init__.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/mgsl/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/mgsl/calculate_mgsl.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/mgsl/calculate_mgsl.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/pre/A.txt` & `nonebot-plugin-cqsat-0.1.9/cqsat/pre/A.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/pre/B.txt` & `nonebot-plugin-cqsat-0.1.9/cqsat/pre/B.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/pre/C.txt` & `nonebot-plugin-cqsat-0.1.9/cqsat/pre/C.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/pre/pre.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/pre/pre.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/sat/sat_handle.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/sat/sat_handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 logger = log()
 Path.mkdir(LOCAL) if not Path.exists(LOCAL) else ...
 
 bind_qth = on_command("绑定位置", aliases={"绑定QTH", "绑Qth", "绑定qth"}, block=True)
 
 
-@bind_qth.got("QTH", prompt="请输入：\n  地名 \n或者输入：\n   经度 纬度 海拔\n\n参数用空格分隔\n")
+@bind_qth.got("QTH", prompt="请输入：\n  地名 \n或者输入：\n   经度 纬度 海拔\n\n参数用空格分隔\n\n发送【取消】来取消操作")
 async def _(
         event: MessageEvent,
         state: T_State,
         qth: str = ArgStr("QTH")):
     if not Path.exists(LOCAL):
         Path.mkdir(LOCAL)
     qq = event.user_id
@@ -67,15 +67,15 @@
     except ValueError:
         await sub.reject_arg("QTH", "请输入：\n  地名 \n或者输入：\n   经度 纬度 海拔\n\n参数用空格分隔\n")
 
 
 sub = on_command("订阅卫星", priority=2, block=True)
 
 
-@sub.got("Sat", prompt="你要订阅那颗卫星？\n多颗卫星用空格分隔")
+@sub.got("Sat", prompt="你要订阅那颗卫星？\n多颗卫星用空格分隔\n发送【取消】来取消操作")
 async def _(
         event: GroupMessageEvent,
         state: T_State,
         sat: str = ArgStr("Sat"), ):
     qq = event.user_id
     group = event.group_id
     sat_s = (await data2Tle())
@@ -88,33 +88,34 @@
         await sub.finish("没有找到QTH文件，请发送【绑定位置】来绑定QTH\n绑定后可以发送【订阅卫星】来订阅卫星")
     if qq in qth:
         if sat == "天宫" or sat == "中国空间站" or sat in ["TIANGONG", "tiangong"]:
             state["sat"] = ["天宫"]
         else:
             user_sat = sat.split(" ")
             if len(user_sat) == 1:
-                if sat or sat.upper() in sat_s:
+                if sat in sat_s or sat.upper() in sat_s:
                     state["sat"] = [sat.upper()]
                 else:
-                    await sub.reject_arg("Sat", f"没有找到{sat},请重新输入：")
+                    await sub.reject_arg("Sat",
+                                         f"没有找到{sat},请重新输入：\n\n输入【算了】取消操作\n输入【卫星列表】查看收录卫星")
             else:
                 temp = []
                 for sat_ in user_sat:
                     if sat_ == "天宫" or sat == "中国空间站" or sat in ["TIANGONG", "tiangong"]:
                         temp.append("天宫")
                     elif sat_.upper() in sat_s:
                         temp.append(sat_.upper())
                     else:
-                        await sub.send(f"没有找到{sat_}")
+                        await sub.send(f"没有找到{sat_}，\n输入【卫星列表】查看收录卫星")
                 state["sat"] = temp
     else:
         await sub.finish("请先发送【绑定位置】来绑定QTH\n绑定后可以发送【订阅卫星】来订阅卫星")
 
 
-@sub.got("E_angle", prompt="请输入最低仰角：")
+@sub.got("E_angle", prompt="请输入最低仰角：\n发送【取消】来取消操作")
 async def _(
         event: GroupMessageEvent,
         state: T_State,
         ang: str = ArgStr("E_angle")):
     qq = event.user_id
     group = event.group_id
     # sat = state["sat"]
@@ -214,27 +215,62 @@
 
 @refer_sat.handle()
 async def _(bot: Bot, event: MessageEvent, state: T_State, args: Message = CommandArg()):
     sat_dict = (await data2Tle())
     sat_list = []
     for i in sat_dict.keys():
         sat_list.append(i)
-    reply = "\n".join(sat_list)
-    await refer_sat.send(f"卫星列表：\n{reply}")
+    sat_list = [sat_list[i:i + 50] for i in range(0, len(sat_list), 50)]
+    messages = []
+    for sat in sat_list:
+        reply = "\n".join(sat)
+        messages.append(reply)
+    if isinstance(event, GroupMessageEvent):
+        await bot.send_group_forward_msg(
+            group_id=event.group_id,
+            messages=[
+                {
+                    "type": "node",
+                    "data": {
+                        "name": "卫星列表",
+                        "uin": bot.self_id,
+                        "content": r
+                    },
+                }
+                for r in messages
+            ])
+    else:
+        await bot.send_private_forward_msg(
+            user_id=bot.self_id,
+            messages=[
+                {
+                    "type": "node",
+                    "data": {
+                        "name": "卫星列表",
+                        "uin": bot.self_id,
+                        "content": r
+                    },
+                }
+                for r in messages
+            ])
 
 
 specified = on_command("查询卫星", aliases={"计算卫星"}, block=True)
 
 
 @specified.handle()
 async def _(bot: Bot, event: MessageEvent, state: T_State, args: Message = CommandArg()):
     qq = event.user_id
     input_arg = str(args).split(" ")
     sat_dict = (await data2Tle())
     sat = input_arg[0]
+    sat_ = ""
+    out = []
+    if not sat:
+        await specified.finish("请发送 计算卫星 卫星名称 分钟数（可选）\n例如：\n计算卫星 AO-73 10\n计算卫星 AO-73")
     try:
         qth = (await yaml_load(QTH))[qq]
     except KeyError:
         qth = ["0", "0", "0"]
         await specified.finish("你没有设置QTH，请发送【绑定位置】绑定QTH")
     except FileNotFoundError:
         qth = ["0", "0", "0"]
@@ -242,68 +278,80 @@
     try:
         add = int(input_arg[1])
     except IndexError:
         add = 0
         await specified.send(f"你没有发送时间，将计算 {sat} 现在的状态")
     time = (datetime.utcnow() + timedelta(minutes=add)).strftime("%Y-%m-%d %H:%M:%S")
     send_time = (datetime.now() + timedelta(minutes=add)).strftime("%Y-%m-%d %H:%M:%S")
-    if not isChinese(sat):
-        sat_ = sat.upper()
-    else:
+
+    # if sat in ["天宫", "天宫号", "中国空间站"] or sat.upper():
+    if isChinese(sat):
+        if sat in ['天宫', '天宫号', '中国空间站', '空间站', '天和', '核心舱']:
+            sat_dict = (await get_tian_gong())
+            sat = '天宫'
+        elif sat == '国际空间站':
+            pass
+    elif sat.upper() in ['TIANGONG', 'CSS', 'TIANHE']:
+        sat = '天宫'
         sat_dict = (await get_tian_gong())
-    reply = "{sat}不存在"
+    else:
+        sat = sat.upper()
+    reply = '{sat}不存在'
     if sat in sat_dict:
+        if sat_dict[sat][1] == "<head>":
+            await specified.finish("通过celestrak下载天宫数据时被禁止，这通常是过量访问导致的，可尝试删除 cqsat/tle_cache/css.cache "
+                                   "文件，若不成功，可在两小时后再次删除此文件再试")
         out = await calculate(sat, qth, time=time)
-    elif sat_ in sat_dict:
-        out = await calculate(sat_, qth, time=time)
-    if out:
-        reply = f"对于QTH:：{qth}\n{sat} 在 {send_time} ：\n仰角为：{round(float(out[1]), 2)}°\n方位角:{round(float(out[0]), 2)}°\n相对速率为：{round(float(out[2]), 2)} "
+        if out:
+            reply = f"对于QTH:：{qth}\n{sat} 在 {send_time} ：\n仰角为：{round(float(out[1]), 2)}°\n方位角:{round(float(out[0]), 2)}°\n相对速率为：{round(float(out[2]), 2)} "
+        else:
+            reply = '哪里出错了 QWQ'
     await specified.send(reply)
 
 
-
 async def aps():
     if not Path.exists(CONFIG):
         return
-    elif read_all(CONFIG) == "":
+    elif (await read_all(CONFIG)) == "":
         return
     today = datetime.now().strftime("%Y-%m-%d")
     try:
-        # FIXME 目前是每次都下载
         await download_ham_sat()
         data = (await yaml_load(CONFIG))
     except FileNotFoundError:
         data = await download_ham_sat()
+        # FIXME ↑？？？
 
     for group in data:
         for qq in data[group]:
             for sat in data[group][qq]:
                 try:
                     last = parse(data[group][qq][sat]["last_send"])
                 except ParserError:
                     last = parse("2001-11-04 00:00:00")
                 except TypeError:
                     last = parse("2001-11-04 00:00:00")
                 now_to_calculate = (datetime.now()).strftime("%Y-%m-%d %H:%M:%S")
                 min_add = 10
-                if int((parse(now_to_calculate) - last).total_seconds() / 60) >= 60:
+                if int((parse(now_to_calculate) - last).total_seconds() / 60) >= 30:
                     now = (datetime.utcnow() + timedelta(minutes=min_add)).strftime("%Y-%m-%d %H:%M:%S")
-                    result = await calculate(sat, data[group][qq][sat]["qth"], now)
+                    qth = (await yaml_load(QTH))[qq]
+                    result = await calculate(sat, qth, now)
                     sated = []
                     if float(result[1]) > 0:
                         logger.info(f"@{qq} 订阅的 {sat} 将入境，正准备计算最高仰角")
                         i = 0
                         az_list = []
                         alt_list = []
                         time_highest_point = {}
-                        result_ = await calculate(sat, data[group][qq][sat]["qth"], now)
+                        result_ = await calculate(sat, qth, now)
                         while float(result_[1]) >= 0:
                             now = (datetime.utcnow() + timedelta(minutes=min_add + int(i))).strftime(
                                 "%Y-%m-%d %H:%M:%S")
-                            result_ = await calculate(sat, data[group][qq][sat]["qth"], now)
+                            result_ = await calculate(sat, qth, now)
                             i += 1
                             az_list.append(float(result_[0]))
                             alt_list.append(float(result_[1]))
                             logger.debug("方位角信息：")
                             logger.debug(az_list)
                             logger.debug("仰角信息：")
                             logger.debug(alt_list)
@@ -330,13 +378,29 @@
                                     logger.error("消息发送失败，账号可能被风控")
                                 sated.append(sat)
                             data[group][qq][sat]["last_send"] = now_to_calculate
                             await yaml_dump(CONFIG, data)
                         else:
                             logger.info("最高仰角小于用户设定的值，不需要提醒")
                 else:
-                    logger.info("一小时内该卫星已过境，跳过此卫星")
+                    logger.info("半小时内该卫星已过境，跳过此卫星")
+                    pass
 
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 scheduler.add_job(aps, 'cron', minute="0/1", id="sat")
+
+# 定时任务
+
+query_tevel = on_command("/小火车", aliases={"/t", "/查询小火车"}, block=True)
+
+
+@query_tevel.handle()
+async def query_tevel_(bot: Bot, event: MessageEvent, state: T_State, args: Message = CommandArg()):
+    if not args:
+        url = "https://www.df2et.de/tevel/"
+        await shoot_scr(url, img_output=SHOOTS_OUT_PATH / "tevel.png")
+        try:
+            await query_tevel.send(MessageSegment.image(f"file:///{Path(SHOOTS_OUT_PATH / 'tevel.png').resolve()}"))
+        except:
+            await query_tevel.send("图片发送失败，哪里出错了？")
```

### Comparing `nonebot-plugin-cqsat-0.1.8/cqsat/utils.py` & `nonebot-plugin-cqsat-0.1.9/cqsat/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -238,7 +238,35 @@
     await write_(state_for_time, json.dumps(state_2))
     if state["pic_to_send"]:
         await matcher.send(MessageSegment.image(f"file:///{(IMG / state['pic_to_send']).absolute()}"))
         await matcher.reject(state["user_notice"] + reply)
     else:
         await matcher.reject(state["user_notice"] + reply)
     return state
+    # FIXME 此处return无法访问，但是能跑？
+
+
+async def shoot_scr(url, locator="html", img_output="out.png"):
+    browser = await browser_init()
+    context = await browser.new_context(locale="zh-CN")
+    page = await context.new_page()
+    await page.goto(url)
+    await page.locator(locator).screenshot(path=img_output)
+    await browser.close()
+
+
+def MsgText(data: str):
+    """
+    返回消息文本段内容(即去除 cq 码后的内容)
+    :param data: event.json()
+    :return: str
+    """
+    try:
+        data = json.loads(data)
+        # 过滤出类型为 text 的【并且过滤内容为空的】
+        msg_text_list = filter(lambda x: x['type'] == 'text' and x['data']['text'].replace(' ', '') != '',
+                               data['message'])
+        # 拼接成字符串并且去除两端空格
+        msg_text = ' '.join(map(lambda x: x['data']['text'].strip(), msg_text_list)).strip()
+        return msg_text
+    except:
+        return ''
```

### Comparing `nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/PKG-INFO` & `nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cqsat
-Version: 0.1.8
+Version: 0.1.9
 Summary: nonebot2 业余无线电卫星
 Home-page: https://github.com/yzyyz1387/cqsat
 Author: yzyyz1387
 Author-email: youzyyz1384@gmail.com
 Keywords: ham,nonebot2,nonebot,radio,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -226,14 +226,24 @@
 <details>
   <summary> <h3>点击查看截图</h3></summary>
 
 ![](img/readme/cancel.gif)
 
 </details>
 
+### 查看Tevel系列卫星截图
+- 发送`/t` 即可查看网站https://www.df2et.de/tevel/的截图
+
+
+### 娱乐信令
+- 发送`/v` ，根据提示回复一条语音，即可对该语音加上信令音
+- 可选参数
+  - `-p` 加前置音 例如：`/v -p`
+  - `-n[数字]` 加噪音 例如：`/v -n5`
+
 ### 网格 【私聊、群内】
 
 - 发送 `我的网格` 查询用户绑定qth的网格
 - 发送 `计算网格 +地名` 计算指定地址的网格，如 `计算网格 北京`
 - 发送 `计算网格+经度+  +纬度` 计算指定位置的网格 经纬度用空格分隔
   - 不加经纬度相当于 `我的网格` 指令
 
@@ -277,13 +287,14 @@
 
 - [X]  追星
 - [X]  相关计算
 - [X]  刷题
 - [ ]  刷题错误记录、常错记录
 - [ ]  模拟考试
 - [ ]  卫星状态、卫星列表加入图片支持
+- [ ]  [#5](https://github.com/yzyyz1387/cqsat/issues/5)
 
 ## 参考资料
 
 [PyEphem Home Page — PyEphem home page (rhodesmill.org)](https://rhodesmill.org/pyephem/)
 
 刁宁辉,刘建强,孙从容,等. 基于SGP4模型的卫星轨道计算[J]. 遥感信息,2012,27(4):64-70. DOI:10.3969/j.issn.1000-3177.2012.04.011.
```

### Comparing `nonebot-plugin-cqsat-0.1.8/nonebot_plugin_cqsat.egg-info/SOURCES.txt` & `nonebot-plugin-cqsat-0.1.9/nonebot_plugin_cqsat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 cqsat/__init__.py
+cqsat/config.py
 cqsat/log.py
+cqsat/media_utils.py
 cqsat/path.py
 cqsat/utils.py
 cqsat/cqsat_resource/bank/A.json
 cqsat/cqsat_resource/bank/B.json
 cqsat/cqsat_resource/bank/C.json
 cqsat/cqsat_resource/bank/imgs/LK0497.jpg
 cqsat/cqsat_resource/bank/imgs/LK0498.jpg
@@ -58,14 +60,18 @@
 cqsat/cqsat_resource/bank/imgs/LK0928.jpg
 cqsat/cqsat_resource/bank/imgs/LK0938.jpg
 cqsat/cqsat_resource/bank/imgs/LK0941.jpg
 cqsat/cqsat_resource/bank/imgs/LK0942.jpg
 cqsat/cqsat_resource/bank/imgs/LK0943.jpg
 cqsat/cqsat_resource/bank/imgs/LK0944.jpg
 cqsat/cqsat_resource/bank/imgs/LK0945.jpg
+cqsat/cqsat_resource/voices/prefix/unknown_pre.mp3
+cqsat/cqsat_resource/voices/suffix/mdc1200.mp3
+cqsat/cqsat_resource/voices/suffix/mdc1200_2.mp3
+cqsat/entertainment/__init__.py
 cqsat/exercise/__init__.py
 cqsat/exercise/exam.py
 cqsat/mgsl/__init__.py
 cqsat/mgsl/calculate_mgsl.py
 cqsat/pre/A.txt
 cqsat/pre/B.txt
 cqsat/pre/C.txt
```

### Comparing `nonebot-plugin-cqsat-0.1.8/setup.py` & `nonebot-plugin-cqsat-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-cqsat",
-    version="0.1.8",
+    version="0.1.9",
     author="yzyyz1387",
     author_email="youzyyz1384@gmail.com",
     keywords=("ham", "nonebot2", "nonebot", "radio", "nonebot_plugin"),
     description="""nonebot2 业余无线电卫星""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yzyyz1387/cqsat",
```

