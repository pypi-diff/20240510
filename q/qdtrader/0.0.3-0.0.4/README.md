# Comparing `tmp/qdtrader-0.0.3.tar.gz` & `tmp/qdtrader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdtrader-0.0.3.tar", last modified: Wed May  8 03:31:42 2024, max compression
+gzip compressed data, was "qdtrader-0.0.4.tar", last modified: Fri May 10 10:11:32 2024, max compression
```

## Comparing `qdtrader-0.0.3.tar` & `qdtrader-0.0.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.240573 qdtrader-0.0.3/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qdtrader-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       66 2024-04-29 01:13:07.000000 qdtrader-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    11368 2024-05-08 03:31:42.237572 qdtrader-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9092 2024-05-08 03:30:44.000000 qdtrader-0.0.3/README.md
--rw-rw-rw-   0        0        0     1055 2024-05-08 03:31:32.000000 qdtrader-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 03:31:42.241579 qdtrader-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.042810 qdtrader-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.164272 qdtrader-0.0.3/src/qdtrader/
--rw-rw-rw-   0        0        0     1961 2024-01-19 04:51:36.000000 qdtrader-0.0.3/src/qdtrader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.178460 qdtrader-0.0.3/src/qdtrader/linux/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.184601 qdtrader-0.0.3/src/qdtrader/linux/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-27 13:49:20.000000 qdtrader-0.0.3/src/qdtrader/linux/pytransform/__init__.py
--rw-rw-rw-   0        0        0  1198080 2023-03-27 13:49:20.000000 qdtrader-0.0.3/src/qdtrader/linux/pytransform/_pytransform.so
--rw-rw-rw-   0        0        0    32946 2023-03-27 13:56:11.000000 qdtrader-0.0.3/src/qdtrader/linux/qestockmarket.py
--rw-rw-rw-   0        0        0     8425 2024-05-06 06:13:38.000000 qdtrader-0.0.3/src/qdtrader/prodtables.py
--rw-rw-rw-   0        0        0    13928 2023-08-09 04:15:09.000000 qdtrader-0.0.3/src/qdtrader/qeaccount.py
--rw-rw-rw-   0        0        0    29534 2022-07-28 14:12:29.000000 qdtrader-0.0.3/src/qdtrader/qearbit.py
--rw-rw-rw-   0        0        0     6390 2024-04-29 05:59:48.000000 qdtrader-0.0.3/src/qdtrader/qeasyncdata.py
--rw-rw-rw-   0        0        0    27472 2023-05-28 09:40:41.000000 qdtrader-0.0.3/src/qdtrader/qeasyncstrat.py
--rw-rw-rw-   0        0        0   130203 2024-05-06 06:14:49.000000 qdtrader-0.0.3/src/qdtrader/qebacktestmul.py
--rw-rw-rw-   0        0        0    42851 2024-05-06 09:52:07.000000 qdtrader-0.0.3/src/qdtrader/qecontext.py
--rw-rw-rw-   0        0        0     1321 2023-01-31 07:13:39.000000 qdtrader-0.0.3/src/qdtrader/qectpconst_wrap.py
--rw-rw-rw-   0        0        0    19883 2024-05-06 09:52:07.000000 qdtrader-0.0.3/src/qdtrader/qectpmarket.py
--rw-rw-rw-   0        0        0    25270 2024-05-06 06:15:51.000000 qdtrader-0.0.3/src/qdtrader/qectpmarket_wrap.py
--rw-rw-rw-   0        0        0    60402 2023-06-08 17:02:50.000000 qdtrader-0.0.3/src/qdtrader/qectptrader.py
--rw-rw-rw-   0        0        0   112647 2024-01-18 02:20:27.000000 qdtrader-0.0.3/src/qdtrader/qectptrader_wrap.py
--rw-rw-rw-   0        0        0     8193 2024-05-07 02:23:04.000000 qdtrader-0.0.3/src/qdtrader/qeglobal.py
--rw-rw-rw-   0        0        0    57309 2023-06-08 15:24:32.000000 qdtrader-0.0.3/src/qdtrader/qehtstrader.py
--rw-rw-rw-   0        0        0    54745 2024-01-17 03:31:20.000000 qdtrader-0.0.3/src/qdtrader/qeinterface.py
--rw-rw-rw-   0        0        0     5460 2023-05-26 15:26:39.000000 qdtrader-0.0.3/src/qdtrader/qelogger.py
--rw-rw-rw-   0        0        0    37097 2024-05-07 01:48:29.000000 qdtrader-0.0.3/src/qdtrader/qemain.py
--rw-rw-rw-   0        0        0     1844 2023-02-02 15:02:07.000000 qdtrader-0.0.3/src/qdtrader/qemonitor_log_web.py
--rw-rw-rw-   0        0        0     1861 2023-04-21 09:35:33.000000 qdtrader-0.0.3/src/qdtrader/qeoption.py
--rw-rw-rw-   0        0        0     3867 2024-05-06 06:16:57.000000 qdtrader-0.0.3/src/qdtrader/qeplugins.py
--rw-rw-rw-   0        0        0    37970 2024-05-07 02:25:20.000000 qdtrader-0.0.3/src/qdtrader/qeredisdb.py
--rw-rw-rw-   0        0        0    11585 2023-12-13 02:54:10.000000 qdtrader-0.0.3/src/qdtrader/qeriskctl.py
--rw-rw-rw-   0        0        0    57155 2024-04-29 02:54:26.000000 qdtrader-0.0.3/src/qdtrader/qesimtrader.py
--rw-rw-rw-   0        0        0    12252 2022-07-28 14:14:40.000000 qdtrader-0.0.3/src/qdtrader/qestatistics.py
--rw-rw-rw-   0        0        0      196 2023-06-17 09:48:34.000000 qdtrader-0.0.3/src/qdtrader/qestockmarket.py
--rw-rw-rw-   0        0        0     4261 2023-02-02 11:34:52.000000 qdtrader-0.0.3/src/qdtrader/qestratmarket_wrap.py
--rw-rw-rw-   0        0        0    27804 2023-08-21 03:33:22.000000 qdtrader-0.0.3/src/qdtrader/qestratprocess.py
--rw-rw-rw-   0        0        0     1642 2024-05-07 02:21:18.000000 qdtrader-0.0.3/src/qdtrader/qesysconf.py
--rw-rw-rw-   0        0        0     1227 2023-07-20 05:43:32.000000 qdtrader-0.0.3/src/qdtrader/qetype.py
--rw-rw-rw-   0        0        0     4596 2024-01-02 07:34:27.000000 qdtrader-0.0.3/src/qdtrader/qeudpclient.py
--rw-rw-rw-   0        0        0    49779 2023-05-26 16:03:19.000000 qdtrader-0.0.3/src/qdtrader/qeweb.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.199174 qdtrader-0.0.3/src/qdtrader/static/
--rw-rw-rw-   0        0        0   583536 2022-05-13 15:56:55.000000 qdtrader-0.0.3/src/qdtrader/static/canvas.js
--rw-rw-rw-   0        0        0     7284 2022-05-09 10:12:32.000000 qdtrader-0.0.3/src/qdtrader/static/jquery.pagination.js
--rw-rw-rw-   0        0        0     3342 2022-05-12 07:11:40.000000 qdtrader-0.0.3/src/qdtrader/static/jquery.timers.js
--rw-rw-rw-   0        0        0     2604 2022-02-25 07:14:44.000000 qdtrader-0.0.3/src/qdtrader/static/theme.css
--rw-rw-rw-   0        0        0      110 2023-02-01 11:46:22.000000 qdtrader-0.0.3/src/qdtrader/sysconfig.json
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.215572 qdtrader-0.0.3/src/qdtrader/templates/
--rw-rw-rw-   0        0        0    21926 2022-11-01 13:36:55.000000 qdtrader-0.0.3/src/qdtrader/templates/backtest.html
--rw-rw-rw-   0        0        0     3042 2022-03-23 12:37:06.000000 qdtrader-0.0.3/src/qdtrader/templates/base.html
--rw-rw-rw-   0        0        0     4074 2022-07-23 10:41:02.000000 qdtrader-0.0.3/src/qdtrader/templates/fundhome.html
--rw-rw-rw-   0        0        0    44342 2022-05-12 10:53:16.000000 qdtrader-0.0.3/src/qdtrader/templates/image_all.html
--rw-rw-rw-   0        0        0    32333 2022-06-23 07:29:42.000000 qdtrader-0.0.3/src/qdtrader/templates/image_ex.html
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.219577 qdtrader-0.0.3/src/qdtrader/win/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.228574 qdtrader-0.0.3/src/qdtrader/win/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-25 08:40:43.000000 qdtrader-0.0.3/src/qdtrader/win/pytransform/__init__.py
--rw-rw-rw-   0        0        0  1165824 2023-03-27 13:40:41.000000 qdtrader-0.0.3/src/qdtrader/win/pytransform/_pytransform.dll
--rw-rw-rw-   0        0        0    34080 2023-03-27 13:42:57.000000 qdtrader-0.0.3/src/qdtrader/win/qestockmarket.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:31:42.235575 qdtrader-0.0.3/src/qdtrader.egg-info/
--rw-rw-rw-   0        0        0    11368 2024-05-08 03:31:41.000000 qdtrader-0.0.3/src/qdtrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2024-05-08 03:31:42.000000 qdtrader-0.0.3/src/qdtrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:31:41.000000 qdtrader-0.0.3/src/qdtrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      279 2024-05-08 03:31:41.000000 qdtrader-0.0.3/src/qdtrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 03:31:41.000000 qdtrader-0.0.3/src/qdtrader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:32.008116 qdtrader-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qdtrader-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       66 2024-04-29 01:13:07.000000 qdtrader-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    11368 2024-05-10 10:11:32.007472 qdtrader-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9092 2024-05-08 03:30:44.000000 qdtrader-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1055 2024-05-10 09:27:42.000000 qdtrader-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:11:32.008116 qdtrader-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.841717 qdtrader-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.941350 qdtrader-0.0.4/src/qdtrader/
+-rw-rw-rw-   0        0        0     1961 2024-01-19 04:51:36.000000 qdtrader-0.0.4/src/qdtrader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.958393 qdtrader-0.0.4/src/qdtrader/linux/
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.958393 qdtrader-0.0.4/src/qdtrader/linux/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-27 13:49:20.000000 qdtrader-0.0.4/src/qdtrader/linux/pytransform/__init__.py
+-rw-rw-rw-   0        0        0  1198080 2023-03-27 13:49:20.000000 qdtrader-0.0.4/src/qdtrader/linux/pytransform/_pytransform.so
+-rw-rw-rw-   0        0        0    32946 2023-03-27 13:56:11.000000 qdtrader-0.0.4/src/qdtrader/linux/qestockmarket.py
+-rw-rw-rw-   0        0        0     8425 2024-05-06 06:13:38.000000 qdtrader-0.0.4/src/qdtrader/prodtables.py
+-rw-rw-rw-   0        0        0    13928 2023-08-09 04:15:09.000000 qdtrader-0.0.4/src/qdtrader/qeaccount.py
+-rw-rw-rw-   0        0        0    29534 2022-07-28 14:12:29.000000 qdtrader-0.0.4/src/qdtrader/qearbit.py
+-rw-rw-rw-   0        0        0     6390 2024-04-29 05:59:48.000000 qdtrader-0.0.4/src/qdtrader/qeasyncdata.py
+-rw-rw-rw-   0        0        0    27472 2023-05-28 09:40:41.000000 qdtrader-0.0.4/src/qdtrader/qeasyncstrat.py
+-rw-rw-rw-   0        0        0   130353 2024-05-10 02:09:31.000000 qdtrader-0.0.4/src/qdtrader/qebacktestmul.py
+-rw-rw-rw-   0        0        0    42851 2024-05-06 09:52:07.000000 qdtrader-0.0.4/src/qdtrader/qecontext.py
+-rw-rw-rw-   0        0        0     1321 2023-01-31 07:13:39.000000 qdtrader-0.0.4/src/qdtrader/qectpconst_wrap.py
+-rw-rw-rw-   0        0        0    19883 2024-05-06 09:52:07.000000 qdtrader-0.0.4/src/qdtrader/qectpmarket.py
+-rw-rw-rw-   0        0        0    25270 2024-05-06 06:15:51.000000 qdtrader-0.0.4/src/qdtrader/qectpmarket_wrap.py
+-rw-rw-rw-   0        0        0    60402 2023-06-08 17:02:50.000000 qdtrader-0.0.4/src/qdtrader/qectptrader.py
+-rw-rw-rw-   0        0        0   112647 2024-01-18 02:20:27.000000 qdtrader-0.0.4/src/qdtrader/qectptrader_wrap.py
+-rw-rw-rw-   0        0        0     8193 2024-05-07 02:23:04.000000 qdtrader-0.0.4/src/qdtrader/qeglobal.py
+-rw-rw-rw-   0        0        0    57309 2023-06-08 15:24:32.000000 qdtrader-0.0.4/src/qdtrader/qehtstrader.py
+-rw-rw-rw-   0        0        0    54745 2024-01-17 03:31:20.000000 qdtrader-0.0.4/src/qdtrader/qeinterface.py
+-rw-rw-rw-   0        0        0     5460 2023-05-26 15:26:39.000000 qdtrader-0.0.4/src/qdtrader/qelogger.py
+-rw-rw-rw-   0        0        0    37097 2024-05-07 01:48:29.000000 qdtrader-0.0.4/src/qdtrader/qemain.py
+-rw-rw-rw-   0        0        0     1844 2023-02-02 15:02:07.000000 qdtrader-0.0.4/src/qdtrader/qemonitor_log_web.py
+-rw-rw-rw-   0        0        0     1861 2023-04-21 09:35:33.000000 qdtrader-0.0.4/src/qdtrader/qeoption.py
+-rw-rw-rw-   0        0        0     3867 2024-05-06 06:16:57.000000 qdtrader-0.0.4/src/qdtrader/qeplugins.py
+-rw-rw-rw-   0        0        0    37959 2024-05-09 02:58:07.000000 qdtrader-0.0.4/src/qdtrader/qeredisdb.py
+-rw-rw-rw-   0        0        0    11585 2023-12-13 02:54:10.000000 qdtrader-0.0.4/src/qdtrader/qeriskctl.py
+-rw-rw-rw-   0        0        0    57155 2024-04-29 02:54:26.000000 qdtrader-0.0.4/src/qdtrader/qesimtrader.py
+-rw-rw-rw-   0        0        0    12252 2022-07-28 14:14:40.000000 qdtrader-0.0.4/src/qdtrader/qestatistics.py
+-rw-rw-rw-   0        0        0      196 2023-06-17 09:48:34.000000 qdtrader-0.0.4/src/qdtrader/qestockmarket.py
+-rw-rw-rw-   0        0        0     4261 2023-02-02 11:34:52.000000 qdtrader-0.0.4/src/qdtrader/qestratmarket_wrap.py
+-rw-rw-rw-   0        0        0    27804 2023-08-21 03:33:22.000000 qdtrader-0.0.4/src/qdtrader/qestratprocess.py
+-rw-rw-rw-   0        0        0     1642 2024-05-07 02:21:18.000000 qdtrader-0.0.4/src/qdtrader/qesysconf.py
+-rw-rw-rw-   0        0        0     1227 2023-07-20 05:43:32.000000 qdtrader-0.0.4/src/qdtrader/qetype.py
+-rw-rw-rw-   0        0        0     4596 2024-01-02 07:34:27.000000 qdtrader-0.0.4/src/qdtrader/qeudpclient.py
+-rw-rw-rw-   0        0        0    49779 2023-05-26 16:03:19.000000 qdtrader-0.0.4/src/qdtrader/qeweb.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.975009 qdtrader-0.0.4/src/qdtrader/static/
+-rw-rw-rw-   0        0        0   583536 2022-05-13 15:56:55.000000 qdtrader-0.0.4/src/qdtrader/static/canvas.js
+-rw-rw-rw-   0        0        0     7284 2022-05-09 10:12:32.000000 qdtrader-0.0.4/src/qdtrader/static/jquery.pagination.js
+-rw-rw-rw-   0        0        0     3342 2022-05-12 07:11:40.000000 qdtrader-0.0.4/src/qdtrader/static/jquery.timers.js
+-rw-rw-rw-   0        0        0     2604 2022-02-25 07:14:44.000000 qdtrader-0.0.4/src/qdtrader/static/theme.css
+-rw-rw-rw-   0        0        0      110 2023-02-01 11:46:22.000000 qdtrader-0.0.4/src/qdtrader/sysconfig.json
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.990541 qdtrader-0.0.4/src/qdtrader/templates/
+-rw-rw-rw-   0        0        0    21926 2022-11-01 13:36:55.000000 qdtrader-0.0.4/src/qdtrader/templates/backtest.html
+-rw-rw-rw-   0        0        0     3042 2022-03-23 12:37:06.000000 qdtrader-0.0.4/src/qdtrader/templates/base.html
+-rw-rw-rw-   0        0        0     4074 2022-07-23 10:41:02.000000 qdtrader-0.0.4/src/qdtrader/templates/fundhome.html
+-rw-rw-rw-   0        0        0    44342 2022-05-12 10:53:16.000000 qdtrader-0.0.4/src/qdtrader/templates/image_all.html
+-rw-rw-rw-   0        0        0    32333 2022-06-23 07:29:42.000000 qdtrader-0.0.4/src/qdtrader/templates/image_ex.html
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.991229 qdtrader-0.0.4/src/qdtrader/win/
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.991229 qdtrader-0.0.4/src/qdtrader/win/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-25 08:40:43.000000 qdtrader-0.0.4/src/qdtrader/win/pytransform/__init__.py
+-rw-rw-rw-   0        0        0  1165824 2023-03-27 13:40:41.000000 qdtrader-0.0.4/src/qdtrader/win/pytransform/_pytransform.dll
+-rw-rw-rw-   0        0        0    34080 2023-03-27 13:42:57.000000 qdtrader-0.0.4/src/qdtrader/win/qestockmarket.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:11:31.991229 qdtrader-0.0.4/src/qdtrader.egg-info/
+-rw-rw-rw-   0        0        0    11368 2024-05-10 10:11:31.000000 qdtrader-0.0.4/src/qdtrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2024-05-10 10:11:31.000000 qdtrader-0.0.4/src/qdtrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:11:31.000000 qdtrader-0.0.4/src/qdtrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      279 2024-05-10 10:11:31.000000 qdtrader-0.0.4/src/qdtrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 10:11:31.000000 qdtrader-0.0.4/src/qdtrader.egg-info/top_level.txt
```

### Comparing `qdtrader-0.0.3/LICENSE` & `qdtrader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/PKG-INFO` & `qdtrader-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdtrader
-Version: 0.0.3
+Version: 0.0.4
 Summary: QuantDo Trader SDK for quants
 Author-email: Fisher Yu <yuzs@quantdo.com.cn>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,17 +37,17 @@
 Requires-Dist: ctpwrapper>=6.6.9
 Requires-Dist: Flask>=1.1.1
 Requires-Dist: Flask_Bootstrap>=3.3.7.1
 Requires-Dist: Flask_Compress>=1.12
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: nest_asyncio>=1.5.5
 Requires-Dist: numpy>=1.21.6
-Requires-Dist: pandas>=1.3.5
+Requires-Dist: pandas>=2.2.2
 Requires-Dist: python_dateutil>=2.8.2
-Requires-Dist: qdsdk>=0.0.4
+Requires-Dist: qdsdk>=0.0.5
 Requires-Dist: quantstats>=0.0.59
 Requires-Dist: redis>=5.0.4
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: passlib>=1.7.4
 
 # qdtrader量化交易工具包
```

### Comparing `qdtrader-0.0.3/README.md` & `qdtrader-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/pyproject.toml` & `qdtrader-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qdtrader"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Fisher Yu", email="yuzs@quantdo.com.cn" },
 ]
 description = "QuantDo Trader SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -23,17 +23,17 @@
   'ctpwrapper>=6.6.9',
   'Flask>=1.1.1',
   'Flask_Bootstrap>=3.3.7.1',
   'Flask_Compress>=1.12',
   'matplotlib>=3.8.4',
   'nest_asyncio>=1.5.5',
   'numpy>=1.21.6',
-  'pandas>=1.3.5',
+  'pandas>=2.2.2',
   'python_dateutil>=2.8.2',
-  'qdsdk>=0.0.4',
+  'qdsdk>=0.0.5',
   'quantstats>=0.0.59',
   'redis>=5.0.4',
   'scipy>=1.13.0',
   'passlib>=1.7.4'
 ]
 [project.urls]
 "Homepage" = "https://doc.quantdo.com.cn/helpbook/index.html#/cn/qdsdk/0.0.1/README"
```

### Comparing `qdtrader-0.0.3/src/qdtrader/__init__.py` & `qdtrader-0.0.4/src/qdtrader/__init__.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/linux/pytransform/__init__.py` & `qdtrader-0.0.4/src/qdtrader/linux/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/linux/pytransform/_pytransform.so` & `qdtrader-0.0.4/src/qdtrader/linux/pytransform/_pytransform.so`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/linux/qestockmarket.py` & `qdtrader-0.0.4/src/qdtrader/linux/qestockmarket.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/prodtables.py` & `qdtrader-0.0.4/src/qdtrader/prodtables.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeaccount.py` & `qdtrader-0.0.4/src/qdtrader/qeaccount.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qearbit.py` & `qdtrader-0.0.4/src/qdtrader/qearbit.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeasyncdata.py` & `qdtrader-0.0.4/src/qdtrader/qeasyncdata.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeasyncstrat.py` & `qdtrader-0.0.4/src/qdtrader/qeasyncstrat.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qebacktestmul.py` & `qdtrader-0.0.4/src/qdtrader/qebacktestmul.py`

 * *Files 0% similar despite different names*

```diff
@@ -1960,15 +1960,16 @@
         if len(context.orders) > 0:
             if context.ROrders is None : 
                 context.ROrders = pd.DataFrame.from_dict(context.orders, orient='index')
                 context.ROrders.index = context.ROrders.index + daynum
             else:
                 ROrders = pd.DataFrame.from_dict(context.orders, orient='index')
                 ROrders.index = ROrders.index + daynum
-                context.ROrders = context.ROrders.append(ROrders)
+                # context.ROrders = context.ROrders.append(ROrders) # Pandas Dataframe append was deprecated on version 1.4
+                context.ROrders = pd.concat([context.ROrders, ROrders], ignore_index=True)
 
         if context.ROrders is None:    
             context.ROrders = pd.DataFrame()
         #if len(context.Cancels) > 0:
         #    Cancels = pd.DataFrame.from_dict(context.Cancels, orient='index')
         #    Cancels.columns = ['orderid', 'daycancels']
         #else:
```

### Comparing `qdtrader-0.0.3/src/qdtrader/qecontext.py` & `qdtrader-0.0.4/src/qdtrader/qecontext.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qectpconst_wrap.py` & `qdtrader-0.0.4/src/qdtrader/qectpconst_wrap.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qectpmarket.py` & `qdtrader-0.0.4/src/qdtrader/qectpmarket.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qectpmarket_wrap.py` & `qdtrader-0.0.4/src/qdtrader/qectpmarket_wrap.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qectptrader.py` & `qdtrader-0.0.4/src/qdtrader/qectptrader.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qectptrader_wrap.py` & `qdtrader-0.0.4/src/qdtrader/qectptrader_wrap.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeglobal.py` & `qdtrader-0.0.4/src/qdtrader/qeglobal.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qehtstrader.py` & `qdtrader-0.0.4/src/qdtrader/qehtstrader.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeinterface.py` & `qdtrader-0.0.4/src/qdtrader/qeinterface.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qelogger.py` & `qdtrader-0.0.4/src/qdtrader/qelogger.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qemain.py` & `qdtrader-0.0.4/src/qdtrader/qemain.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qemonitor_log_web.py` & `qdtrader-0.0.4/src/qdtrader/qemonitor_log_web.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeoption.py` & `qdtrader-0.0.4/src/qdtrader/qeoption.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeplugins.py` & `qdtrader-0.0.4/src/qdtrader/qeplugins.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeredisdb.py` & `qdtrader-0.0.4/src/qdtrader/qeredisdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     return _wrapper
 
 
 def init_redis():
     global my_redis
     try:
         is_exe_mode = getExemode()
-        print(f"init redis connection, ExeMode <{is_exe_mode}> and config = <{redis_config}>")
+        print(f"init redis, ExeMode <{is_exe_mode}> and config = <{redis_config}>")
         if not is_exe_mode:
             pool = redis.ConnectionPool(
                 host=redis_config['host'],
                 port=redis_config['port'],
                 password=redis_config['passwd'],
                 db=0,
                 decode_responses=True
```

### Comparing `qdtrader-0.0.3/src/qdtrader/qeriskctl.py` & `qdtrader-0.0.4/src/qdtrader/qeriskctl.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qesimtrader.py` & `qdtrader-0.0.4/src/qdtrader/qesimtrader.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qestatistics.py` & `qdtrader-0.0.4/src/qdtrader/qestatistics.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qestratmarket_wrap.py` & `qdtrader-0.0.4/src/qdtrader/qestratmarket_wrap.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qestratprocess.py` & `qdtrader-0.0.4/src/qdtrader/qestratprocess.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qesysconf.py` & `qdtrader-0.0.4/src/qdtrader/qesysconf.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qetype.py` & `qdtrader-0.0.4/src/qdtrader/qetype.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeudpclient.py` & `qdtrader-0.0.4/src/qdtrader/qeudpclient.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/qeweb.py` & `qdtrader-0.0.4/src/qdtrader/qeweb.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/static/canvas.js` & `qdtrader-0.0.4/src/qdtrader/static/canvas.js`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/static/jquery.pagination.js` & `qdtrader-0.0.4/src/qdtrader/static/jquery.pagination.js`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/static/jquery.timers.js` & `qdtrader-0.0.4/src/qdtrader/static/jquery.timers.js`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/static/theme.css` & `qdtrader-0.0.4/src/qdtrader/static/theme.css`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/templates/backtest.html` & `qdtrader-0.0.4/src/qdtrader/templates/backtest.html`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/templates/base.html` & `qdtrader-0.0.4/src/qdtrader/templates/base.html`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/templates/fundhome.html` & `qdtrader-0.0.4/src/qdtrader/templates/fundhome.html`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/templates/image_all.html` & `qdtrader-0.0.4/src/qdtrader/templates/image_all.html`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/templates/image_ex.html` & `qdtrader-0.0.4/src/qdtrader/templates/image_ex.html`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/win/pytransform/__init__.py` & `qdtrader-0.0.4/src/qdtrader/win/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/win/pytransform/_pytransform.dll` & `qdtrader-0.0.4/src/qdtrader/win/pytransform/_pytransform.dll`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader/win/qestockmarket.py` & `qdtrader-0.0.4/src/qdtrader/win/qestockmarket.py`

 * *Files identical despite different names*

### Comparing `qdtrader-0.0.3/src/qdtrader.egg-info/PKG-INFO` & `qdtrader-0.0.4/src/qdtrader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdtrader
-Version: 0.0.3
+Version: 0.0.4
 Summary: QuantDo Trader SDK for quants
 Author-email: Fisher Yu <yuzs@quantdo.com.cn>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,17 +37,17 @@
 Requires-Dist: ctpwrapper>=6.6.9
 Requires-Dist: Flask>=1.1.1
 Requires-Dist: Flask_Bootstrap>=3.3.7.1
 Requires-Dist: Flask_Compress>=1.12
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: nest_asyncio>=1.5.5
 Requires-Dist: numpy>=1.21.6
-Requires-Dist: pandas>=1.3.5
+Requires-Dist: pandas>=2.2.2
 Requires-Dist: python_dateutil>=2.8.2
-Requires-Dist: qdsdk>=0.0.4
+Requires-Dist: qdsdk>=0.0.5
 Requires-Dist: quantstats>=0.0.59
 Requires-Dist: redis>=5.0.4
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: passlib>=1.7.4
 
 # qdtrader量化交易工具包
```

### Comparing `qdtrader-0.0.3/src/qdtrader.egg-info/SOURCES.txt` & `qdtrader-0.0.4/src/qdtrader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

