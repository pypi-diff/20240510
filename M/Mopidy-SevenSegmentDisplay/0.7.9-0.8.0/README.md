# Comparing `tmp/mopidy_sevensegmentdisplay-0.7.9.tar.gz` & `tmp/mopidy_sevensegmentdisplay-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopidy_sevensegmentdisplay-0.7.9.tar", last modified: Sun Apr 14 20:03:42 2024, max compression
+gzip compressed data, was "mopidy_sevensegmentdisplay-0.8.0.tar", last modified: Fri May 10 11:41:51 2024, max compression
```

## Comparing `mopidy_sevensegmentdisplay-0.7.9.tar` & `mopidy_sevensegmentdisplay-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:03:42.231369 mopidy_sevensegmentdisplay-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:03:42.231369 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-14 20:03:42.000000 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-14 20:03:42.000000 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:03:42.000000 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 20:03:42.000000 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:03:42.000000 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 20:03:42.000000 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 20:03:42.000000 mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-14 20:03:42.231369 mopidy_sevensegmentdisplay-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:03:42.231369 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/cava.config
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/ext.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/led.py
--rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/lib_nrf24.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/max7219.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/music.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:03:42.231369 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/alwan.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/alwan.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:03:42.231369 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 20:03:42.235369 mopidy_sevensegmentdisplay-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-14 20:03:37.000000 mopidy_sevensegmentdisplay-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:41:51.068561 mopidy_sevensegmentdisplay-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:41:51.068561 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-10 11:41:51.000000 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-10 11:41:51.000000 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:41:51.000000 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-10 11:41:51.000000 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:41:50.000000 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 11:41:51.000000 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 11:41:51.000000 mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-10 11:41:51.068561 mopidy_sevensegmentdisplay-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:41:51.064561 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/cava.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/ext.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/max7219.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:41:51.064561 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/alwan.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/alwan.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:41:51.064561 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-10 11:41:51.068561 mopidy_sevensegmentdisplay-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 11:41:46.000000 mopidy_sevensegmentdisplay-0.8.0/setup.py
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/LICENSE` & `mopidy_sevensegmentdisplay-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO` & `mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.9
+Version: 0.8.0
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt` & `mopidy_sevensegmentdisplay-0.8.0/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 mopidy_sevensegmentdisplay/display.py
 mopidy_sevensegmentdisplay/equalizer.py
 mopidy_sevensegmentdisplay/ext.conf
 mopidy_sevensegmentdisplay/gpio.py
 mopidy_sevensegmentdisplay/http.py
 mopidy_sevensegmentdisplay/ir.py
 mopidy_sevensegmentdisplay/led.py
-mopidy_sevensegmentdisplay/lib_nrf24.py
 mopidy_sevensegmentdisplay/light_sensor.py
 mopidy_sevensegmentdisplay/max7219.py
 mopidy_sevensegmentdisplay/menu.py
 mopidy_sevensegmentdisplay/music.py
 mopidy_sevensegmentdisplay/run.sh
 mopidy_sevensegmentdisplay/threader.py
 mopidy_sevensegmentdisplay/timer.py
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/PKG-INFO` & `mopidy_sevensegmentdisplay-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.9
+Version: 0.8.0
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/README.md` & `mopidy_sevensegmentdisplay-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/__init__.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from mopidy import config, ext
 from .http import factory_decorator
 from .actor import Frontend
 
-__version__ = '0.7.9'
+__version__ = '0.8.0'
 
 
 class Extension(ext.Extension):
     dist_name = 'Mopidy-SevenSegmentDisplay'
     ext_name = 'sevensegmentdisplay'
     version = __version__
 
@@ -31,15 +31,15 @@
         schema['light_sensor_time_from'] = config.Integer()
         schema['light_sensor_time_to'] = config.Integer()
         schema['alert_files'] = config.String(optional=True)
         schema['display_min_brightness'] = config.Integer()
         schema['display_max_brightness'] = config.Integer()
         schema['equalizer_enabled'] = config.Boolean()
         schema['led_enabled'] = config.Boolean()
-        schema['led_pipes'] = config.String(optional=True)
+        schema['led_ips'] = config.String()
         return schema
 
     def setup(self, registry):
         registry.add('frontend', Frontend)
         registry.add('http:app', {
             'name': self.ext_name,
             'factory': factory_decorator(Frontend.worker),
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/actor.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/actor.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/alert.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/alert.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/animation.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/animation.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/clock.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/clock.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/display.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/display.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/equalizer.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/equalizer.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/ext.conf` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/ext.conf`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 light_sensor_time_to = 4
 
 display_min_brightness = 2
 display_max_brightness = 15
 
 equalizer_enabled = true
 led_enabled = true
-led_pipes = [[135, 34, 67, 64, 72], [135, 3, 18, 56, 72]]
+led_ips = []
 
 alert_files = [
 				  { "name": "sounds/01.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/02.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/03.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/04.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/05.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/gpio.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/gpio.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/http.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/http.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/ir.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/ir.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/light_sensor.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/light_sensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     _max_value = 26000
     _channel = None
     _value = 0.5
 
     def __init__(self, enabled, timeout, sudden_change_callback, sudden_change_timeout_callback):
         super(LightSensor, self).__init__()
-        
+
         self._timeout = timeout
         self._sudden_change_callback = sudden_change_callback
         self._sudden_change_timeout_callback = sudden_change_timeout_callback
 
         if (not enabled):
             return
 
@@ -94,15 +94,15 @@
             if (self._value < min_value and max(values) > max_value):
                 self._sudden_change_callback(datetime.now(), True)
                 timeout = 0
             elif (self._value > max_value and min(values) < min_value):
                 self._sudden_change_callback(datetime.now(), False)
                 timeout = 0
 
-            if (timeout > self._timeout * 60 * 10):
+            if (timeout > self._timeout * 60 * 20):
                 self._sudden_change_timeout_callback()
                 timeout = -1
 
             index = (index + 1) % size
             values[index] = self._value
 
             if (timeout >= 0):
@@ -127,10 +127,13 @@
         except Exception as inst:
             logging.error(inst)
 
             return self._value
 
     def get_value(self):
         return self._value
+
+    def is_dark(self):
+        return self.get_value() < 1000 / self._max_value
     
     def get_draw_sleep_animation(self):
         return self.ANIMATION_SLEEP
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/max7219.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/max7219.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/menu.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/menu.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/music.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/music.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/alwan.min.css` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/alwan.min.css`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/alwan.min.js` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/alwan.min.js`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/bootstrap-theme.css` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/bootstrap.css` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/bootstrap.js` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/static/jquery.js` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/static/jquery.js`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/templates/base.html` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/templates/base.html`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/templates/index.html` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/templates/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -71,14 +71,22 @@
         {% for timer in worker.timer_alert.get() %}
         <li>{{ timer.get() }}</li>
         {% end %}
         {% end %}
     </ul>
 
     <p>
+        {{ worker.light_sensor.get_value() * 26000 }}
+        <br />
+        Light/Dark Ratio: {{ worker.light_sensor.get_value() }}
+        <br />
+        Is Dark: {{ worker.light_sensor.is_dark() }}
+    </p>
+
+    <p>
         <span id="colorPicker"></span>
         <button onclick="post({ red: 0, green: 0, blue: 0 })">Off (black)</button>
     </p>
 </div>
 
 <script src="/sevensegmentdisplay/static/alwan.min.js"></script>
 <link rel="stylesheet" href="/sevensegmentdisplay/static/alwan.min.css" />
```

#### html2text {}

```diff
@@ -13,9 +13,12 @@
 Timer alert[Unknown INPUT type][Unknown INPUT type]
 Add Clear Decrease Increase Run
     * {% if not worker.timer_alert.is_set() %}
     * {{ None }}
     * {% else %} {% for timer in worker.timer_alert.get() %}
     * {{ timer.get() }}
     * {% end %} {% end %}
+{{ worker.light_sensor.get_value() * 26000 }}
+Light/Dark Ratio: {{ worker.light_sensor.get_value() }}
+Is Dark: {{ worker.light_sensor.is_dark() }}
 Off (black)
 {% end %}
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/timer.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/timer.py`

 * *Files identical despite different names*

### Comparing `mopidy_sevensegmentdisplay-0.7.9/mopidy_sevensegmentdisplay/worker.py` & `mopidy_sevensegmentdisplay-0.8.0/mopidy_sevensegmentdisplay/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             self.gpio = Gpio(
                 self.config['buttons_enabled'],
                 self.play_stop_music,
                 self._on_menu_click,
                 self._on_menu_click_left,
                 self._on_menu_click_right,
                 self.config['relay_enabled'])
-            self.led = Led(self.config['led_enabled'], self.config['led_pipes'])
+            self.led = Led(self.config['led_enabled'], self.config['led_ips'])
             self.ir_sender = IrSender(self.config['ir_remote'], self.gpio.switch_relay)
             self.timer_on = TimerOn(self.play_music)
             self.timer_off = TimerOff(self.stop_music)
             self.alert = Alert(self.music,
                                self.ir_sender,
                                self.config['alert_files'])
             self.timer_alert = TimerAlert(self.run_alert)
@@ -354,15 +354,18 @@
     def on_mute(self, mute):
         if mute:
             self.on_volume_changed(0)
         else:
             self.on_volume_changed()
 
     def on_new_track_playing(self):
-        self.led.set_random_color()
+        if (self.light_sensor.is_dark()):
+            self.led.set_random_color()
+        else:
+            self.led.set_none_color()
 
     def on_volume_changed(self, volume=None):
         if (self.menu is not None and self.music is not None and self.music.is_volume_changed(volume)):
             self.menu.draw_sub_menu(self.MENU_VOLUME)
 
     def on_playback_state_changed(self, old_state, new_state):
         if (old_state != new_state):
```

### Comparing `mopidy_sevensegmentdisplay-0.7.9/setup.py` & `mopidy_sevensegmentdisplay-0.8.0/setup.py`

 * *Files identical despite different names*

