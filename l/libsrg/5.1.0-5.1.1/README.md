# Comparing `tmp/libsrg-5.1.0.tar.gz` & `tmp/libsrg-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsrg-5.1.0.tar", max compression
+gzip compressed data, was "libsrg-5.1.1.tar", max compression
```

## Comparing `libsrg-5.1.0.tar` & `libsrg-5.1.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.1.0/README.md
--rw-r--r--   0        0        0     1464 2024-05-03 23:47:01.853721 libsrg-5.1.0/libsrg/AppTemplate.py
--rw-r--r--   0        0        0    11933 2024-05-06 15:12:41.996241 libsrg-5.1.0/libsrg/Config.py
--rwxr-xr-x   0        0        0     2603 2024-05-04 14:04:12.419228 libsrg-5.1.0/libsrg/ElapsedTime.py
--rwxr-xr-x   0        0        0     8847 2024-05-06 15:00:11.302960 libsrg-5.1.0/libsrg/Info.py
--rwxr-xr-x   0        0        0     4027 2024-05-03 23:47:01.866721 libsrg-5.1.0/libsrg/LevelBanner.py
--rwxr-xr-x   0        0        0     1514 2024-05-03 23:47:01.870721 libsrg-5.1.0/libsrg/LoggerGUIProxy.py
--rwxr-xr-x   0        0        0     6135 2024-05-03 23:47:01.873721 libsrg-5.1.0/libsrg/LoggingAppBase.py
--rwxr-xr-x   0        0        0     8167 2024-05-03 23:47:01.876721 libsrg-5.1.0/libsrg/LoggingCounter.py
--rwxr-xr-x   0        0        0      593 2024-05-03 23:47:01.880721 libsrg-5.1.0/libsrg/LoggingUtils.py
--rwxr-xr-x   0        0        0     1854 2024-05-03 23:47:01.884721 libsrg-5.1.0/libsrg/LoggingWatcher.py
--rwxr-xr-x   0        0        0     3644 2024-05-03 23:47:01.888721 libsrg-5.1.0/libsrg/NagiosBase.py
--rwxr-xr-x   0        0        0     7209 2024-05-04 13:52:43.434938 libsrg-5.1.0/libsrg/Runner.py
--rwxr-xr-x   0        0        0     4903 2024-05-03 23:47:01.898721 libsrg-5.1.0/libsrg/Runner2.py
--rw-r--r--   0        0        0     4523 2024-05-06 14:42:50.143127 libsrg-5.1.0/libsrg/Statistics/ADStatsBase.py
--rw-r--r--   0        0        0     2275 2024-04-11 13:40:23.574158 libsrg-5.1.0/libsrg/Statistics/AnalogStatsBase.py
--rw-r--r--   0        0        0     1436 2024-04-08 17:02:20.928118 libsrg-5.1.0/libsrg/Statistics/AnalogStatsCumulative.py
--rw-r--r--   0        0        0     2302 2024-05-06 14:43:05.792050 libsrg-5.1.0/libsrg/Statistics/AnalogStatsFading.py
--rw-r--r--   0        0        0     1590 2024-04-12 18:46:46.468186 libsrg-5.1.0/libsrg/Statistics/AnalogStatsSlidingWindow.py
--rw-r--r--   0        0        0     1593 2024-04-11 13:40:23.559158 libsrg-5.1.0/libsrg/Statistics/DiscreteStatsBase.py
--rw-r--r--   0        0        0      774 2024-04-08 17:02:20.912118 libsrg-5.1.0/libsrg/Statistics/DiscreteStatsCumulative.py
--rw-r--r--   0        0        0     1583 2024-04-11 13:02:36.159113 libsrg-5.1.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py
--rw-r--r--   0        0        0     1839 2024-04-11 13:46:23.627270 libsrg-5.1.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py
--rw-r--r--   0        0        0     2784 2024-04-17 20:08:12.373031 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
--rw-r--r--   0        0        0     2344 2024-04-11 13:56:04.322214 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
--rw-r--r--   0        0        0     3915 2024-04-11 13:59:27.002140 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
--rw-r--r--   0        0        0     2933 2024-04-12 18:46:46.483186 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
--rw-r--r--   0        0        0     1605 2024-04-09 15:09:14.481097 libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
--rw-r--r--   0        0        0     2607 2024-04-11 00:45:26.519787 libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.511124 libsrg-5.1.0/libsrg/Statistics/UnitTests/__init__.py
--rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
--rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
--rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     4175 2024-04-24 16:16:17.492580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.512123 libsrg-5.1.0/libsrg/Statistics/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-21 12:42:50.605797 libsrg-5.1.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
--rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0     4439 2024-04-11 13:40:23.886156 libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0      172 2024-04-08 17:02:46.932966 libsrg-5.1.0/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2222 2024-04-09 15:09:14.520097 libsrg-5.1.0/libsrg/TKGUI/GuiBase.py
--rw-r--r--   0        0        0      448 2024-04-09 15:09:14.568096 libsrg-5.1.0/libsrg/TKGUI/GuiRequest.py
--rw-r--r--   0        0        0     3424 2024-04-09 15:09:14.527097 libsrg-5.1.0/libsrg/TKGUI/GuiRequestQueue.py
--rw-r--r--   0        0        0    10694 2024-04-09 15:09:14.560097 libsrg-5.1.0/libsrg/TKGUI/LoggerGUI.py
--rw-r--r--   0        0        0        1 2023-01-31 17:16:02.479077 libsrg-5.1.0/libsrg/TKGUI/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
--rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
--rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
--rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.1.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
--rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.1.0/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5498 2024-04-17 20:14:51.866892 libsrg-5.1.0/libsrg/UnitTests/Config_test.py
--rw-r--r--   0        0        0      470 2024-05-06 14:29:21.184142 libsrg-5.1.0/libsrg/UnitTests/Info_test.py
--rw-r--r--   0        0        0     1259 2024-04-17 20:14:51.874892 libsrg-5.1.0/libsrg/UnitTests/RolloverTest_filename.py
--rw-r--r--   0        0        0     1309 2024-04-17 20:14:51.850892 libsrg-5.1.0/libsrg/UnitTests/RolloverTest_logfile.py
--rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.1.0/libsrg/UnitTests/Sample.env
--rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.1.0/libsrg/UnitTests/Sample.ini
--rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.1.0/libsrg/UnitTests/Sample.json
--rw-r--r--   0        0        0        0 2024-05-06 14:46:32.169025 libsrg-5.1.0/libsrg/UnitTests/__init__.py
--rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.1.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
--rwxr-xr-x   0        0        0      114 2024-05-03 23:47:01.900721 libsrg-5.1.0/libsrg/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-06 15:13:06.778118 libsrg-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.1.1/README.md
+-rw-r--r--   0        0        0     1464 2024-05-03 23:47:01.853721 libsrg-5.1.1/libsrg/AppTemplate.py
+-rw-r--r--   0        0        0    11933 2024-05-06 15:12:41.996241 libsrg-5.1.1/libsrg/Config.py
+-rwxr-xr-x   0        0        0     2603 2024-05-04 14:04:12.419228 libsrg-5.1.1/libsrg/ElapsedTime.py
+-rwxr-xr-x   0        0        0     8969 2024-05-10 00:36:18.128675 libsrg-5.1.1/libsrg/Info.py
+-rwxr-xr-x   0        0        0     4027 2024-05-03 23:47:01.866721 libsrg-5.1.1/libsrg/LevelBanner.py
+-rwxr-xr-x   0        0        0     1514 2024-05-03 23:47:01.870721 libsrg-5.1.1/libsrg/LoggerGUIProxy.py
+-rwxr-xr-x   0        0        0     6135 2024-05-03 23:47:01.873721 libsrg-5.1.1/libsrg/LoggingAppBase.py
+-rwxr-xr-x   0        0        0     8167 2024-05-03 23:47:01.876721 libsrg-5.1.1/libsrg/LoggingCounter.py
+-rwxr-xr-x   0        0        0      593 2024-05-03 23:47:01.880721 libsrg-5.1.1/libsrg/LoggingUtils.py
+-rwxr-xr-x   0        0        0     1854 2024-05-03 23:47:01.884721 libsrg-5.1.1/libsrg/LoggingWatcher.py
+-rwxr-xr-x   0        0        0     3644 2024-05-03 23:47:01.888721 libsrg-5.1.1/libsrg/NagiosBase.py
+-rwxr-xr-x   0        0        0     7209 2024-05-04 13:52:43.434938 libsrg-5.1.1/libsrg/Runner.py
+-rwxr-xr-x   0        0        0     4903 2024-05-03 23:47:01.898721 libsrg-5.1.1/libsrg/Runner2.py
+-rw-r--r--   0        0        0     4523 2024-05-06 14:42:50.143127 libsrg-5.1.1/libsrg/Statistics/ADStatsBase.py
+-rw-r--r--   0        0        0     2275 2024-04-11 13:40:23.574158 libsrg-5.1.1/libsrg/Statistics/AnalogStatsBase.py
+-rw-r--r--   0        0        0     1436 2024-04-08 17:02:20.928118 libsrg-5.1.1/libsrg/Statistics/AnalogStatsCumulative.py
+-rw-r--r--   0        0        0     2302 2024-05-06 14:43:05.792050 libsrg-5.1.1/libsrg/Statistics/AnalogStatsFading.py
+-rw-r--r--   0        0        0     1590 2024-04-12 18:46:46.468186 libsrg-5.1.1/libsrg/Statistics/AnalogStatsSlidingWindow.py
+-rw-r--r--   0        0        0     1593 2024-04-11 13:40:23.559158 libsrg-5.1.1/libsrg/Statistics/DiscreteStatsBase.py
+-rw-r--r--   0        0        0      774 2024-04-08 17:02:20.912118 libsrg-5.1.1/libsrg/Statistics/DiscreteStatsCumulative.py
+-rw-r--r--   0        0        0     1583 2024-04-11 13:02:36.159113 libsrg-5.1.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py
+-rw-r--r--   0        0        0     1839 2024-04-11 13:46:23.627270 libsrg-5.1.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py
+-rw-r--r--   0        0        0     2784 2024-04-17 20:08:12.373031 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
+-rw-r--r--   0        0        0     2344 2024-04-11 13:56:04.322214 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
+-rw-r--r--   0        0        0     3915 2024-04-11 13:59:27.002140 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+-rw-r--r--   0        0        0     2933 2024-04-12 18:46:46.483186 libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0     1605 2024-04-09 15:09:14.481097 libsrg-5.1.1/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+-rw-r--r--   0        0        0     2607 2024-04-11 00:45:26.519787 libsrg-5.1.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:48:22.511124 libsrg-5.1.1/libsrg/Statistics/UnitTests/__init__.py
+-rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
+-rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     4175 2024-04-24 16:16:17.492580 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-07 19:48:22.512123 libsrg-5.1.1/libsrg/Statistics/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-21 12:42:50.605797 libsrg-5.1.1/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
+-rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0     4439 2024-04-11 13:40:23.886156 libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0      172 2024-04-08 17:02:46.932966 libsrg-5.1.1/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2222 2024-04-09 15:09:14.520097 libsrg-5.1.1/libsrg/TKGUI/GuiBase.py
+-rw-r--r--   0        0        0      448 2024-04-09 15:09:14.568096 libsrg-5.1.1/libsrg/TKGUI/GuiRequest.py
+-rw-r--r--   0        0        0     3424 2024-04-09 15:09:14.527097 libsrg-5.1.1/libsrg/TKGUI/GuiRequestQueue.py
+-rw-r--r--   0        0        0    10694 2024-04-09 15:09:14.560097 libsrg-5.1.1/libsrg/TKGUI/LoggerGUI.py
+-rw-r--r--   0        0        0        1 2023-01-31 17:16:02.479077 libsrg-5.1.1/libsrg/TKGUI/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
+-rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
+-rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
+-rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.1.1/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
+-rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.1.1/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5498 2024-04-17 20:14:51.866892 libsrg-5.1.1/libsrg/UnitTests/Config_test.py
+-rw-r--r--   0        0        0      470 2024-05-06 14:29:21.184142 libsrg-5.1.1/libsrg/UnitTests/Info_test.py
+-rw-r--r--   0        0        0     1259 2024-04-17 20:14:51.874892 libsrg-5.1.1/libsrg/UnitTests/RolloverTest_filename.py
+-rw-r--r--   0        0        0     1309 2024-04-17 20:14:51.850892 libsrg-5.1.1/libsrg/UnitTests/RolloverTest_logfile.py
+-rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.1.1/libsrg/UnitTests/Sample.env
+-rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.1.1/libsrg/UnitTests/Sample.ini
+-rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.1.1/libsrg/UnitTests/Sample.json
+-rw-r--r--   0        0        0        0 2024-05-06 14:46:32.169025 libsrg-5.1.1/libsrg/UnitTests/__init__.py
+-rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.1.1/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
+-rwxr-xr-x   0        0        0      114 2024-05-03 23:47:01.900721 libsrg-5.1.1/libsrg/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-10 00:36:30.486614 libsrg-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.1.1/PKG-INFO
```

### Comparing `libsrg-5.1.0/LICENSE.txt` & `libsrg-5.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/README.md` & `libsrg-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/AppTemplate.py` & `libsrg-5.1.1/libsrg/AppTemplate.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Config.py` & `libsrg-5.1.1/libsrg/Config.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/ElapsedTime.py` & `libsrg-5.1.1/libsrg/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Info.py` & `libsrg-5.1.1/libsrg/Info.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,20 +210,22 @@
         :param prefix:  string top be prepended at the start of field names
         """
         config = Config()
         if prefix is None:
             prefix = ""
         for k, v in self.__dict__.items():
             if k not in ["logger", "config", "osrelease"]:
-                config.set_item(f"{prefix}{k.lower()}", v)
+                if isinstance(v,(int,float,str,bool)):
+                    config.set_item(f"{prefix}{k.lower()}", v)
 
         if "osrelease" in self.__dict__ and self.__dict__["osrelease"]:
             for k, v in self.osrelease.items():
-                config.set_item(f"{prefix}osrelease.{k}", v)
-                config.set_item(f"{prefix}osrelease.{k.lower()}", v)
+                if isinstance(v,(int,float,str,bool)):
+                    config.set_item(f"{prefix}osrelease.{k}", v)
+                    config.set_item(f"{prefix}osrelease.{k.lower()}", v)
         return config
 
 
 if __name__ == '__main__':
     import pprint
 
     # info = Info("nas0")
```

### Comparing `libsrg-5.1.0/libsrg/LevelBanner.py` & `libsrg-5.1.1/libsrg/LevelBanner.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/LoggerGUIProxy.py` & `libsrg-5.1.1/libsrg/LoggerGUIProxy.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/LoggingAppBase.py` & `libsrg-5.1.1/libsrg/LoggingAppBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/LoggingCounter.py` & `libsrg-5.1.1/libsrg/LoggingCounter.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/LoggingUtils.py` & `libsrg-5.1.1/libsrg/LoggingUtils.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/LoggingWatcher.py` & `libsrg-5.1.1/libsrg/LoggingWatcher.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/NagiosBase.py` & `libsrg-5.1.1/libsrg/NagiosBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Runner.py` & `libsrg-5.1.1/libsrg/Runner.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Runner2.py` & `libsrg-5.1.1/libsrg/Runner2.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/ADStatsBase.py` & `libsrg-5.1.1/libsrg/Statistics/ADStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/AnalogStatsBase.py` & `libsrg-5.1.1/libsrg/Statistics/AnalogStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/AnalogStatsCumulative.py` & `libsrg-5.1.1/libsrg/Statistics/AnalogStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/AnalogStatsFading.py` & `libsrg-5.1.1/libsrg/Statistics/AnalogStatsFading.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/AnalogStatsSlidingWindow.py` & `libsrg-5.1.1/libsrg/Statistics/AnalogStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/DiscreteStatsBase.py` & `libsrg-5.1.1/libsrg/Statistics/DiscreteStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/DiscreteStatsCumulative.py` & `libsrg-5.1.1/libsrg/Statistics/DiscreteStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py` & `libsrg-5.1.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.1.1/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/TKGUI/GuiBase.py` & `libsrg-5.1.1/libsrg/TKGUI/GuiBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/TKGUI/GuiRequestQueue.py` & `libsrg-5.1.1/libsrg/TKGUI/GuiRequestQueue.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/TKGUI/LoggerGUI.py` & `libsrg-5.1.1/libsrg/TKGUI/LoggerGUI.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc` & `libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc` & `libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc` & `libsrg-5.1.1/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc` & `libsrg-5.1.1/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/UnitTests/Config_test.py` & `libsrg-5.1.1/libsrg/UnitTests/Config_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/UnitTests/RolloverTest_filename.py` & `libsrg-5.1.1/libsrg/UnitTests/RolloverTest_filename.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/UnitTests/RolloverTest_logfile.py` & `libsrg-5.1.1/libsrg/UnitTests/RolloverTest_logfile.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.1/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.1.0/pyproject.toml` & `libsrg-5.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsrg"
-version = "5.1.0"
+version = "5.1.1"
 description = "Utility lib logging, statistics, subprocesses"
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
```

### Comparing `libsrg-5.1.0/PKG-INFO` & `libsrg-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 5.1.0
+Version: 5.1.1
 Summary: Utility lib logging, statistics, subprocesses
 Author: Steve Goncalo
 Author-email: steven@goncalo.us
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

