# Comparing `tmp/android_prober-0.1.5.tar.gz` & `tmp/android_prober-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android_prober-0.1.5.tar", last modified: Fri May 10 03:47:19 2024, max compression
+gzip compressed data, was "android_prober-0.1.6.tar", last modified: Fri May 10 04:02:52 2024, max compression
```

## Comparing `android_prober-0.1.5.tar` & `android_prober-0.1.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-10 03:47:14.000000 android_prober-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-10 03:47:19.545820 android_prober-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-10 03:47:14.000000 android_prober-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.533820 android_prober-0.1.5/android_prober/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.537820 android_prober-0.1.5/android_prober/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/vibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.541820 android_prober-0.1.5/android_prober/facades/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/call.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/service.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/vibrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.533820 android_prober-0.1.5/android_prober/platforms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.541820 android_prober-0.1.5/android_prober/platforms/android/
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/realtime_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober/platforms/generics/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/vibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/proxy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/wrappers/register_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.533820 android_prober-0.1.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/examples/webview-app/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 03:47:14.000000 android_prober-0.1.5/examples/webview-app/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 03:47:19.545820 android_prober-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-10 03:47:14.000000 android_prober-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.965757 android_prober-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-10 04:02:47.000000 android_prober-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-10 04:02:52.965757 android_prober-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-10 04:02:47.000000 android_prober-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.957757 android_prober-0.1.6/android_prober/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.961757 android_prober-0.1.6/android_prober/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/apis/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.961757 android_prober-0.1.6/android_prober/facades/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/facades/vibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.953757 android_prober-0.1.6/android_prober/platforms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.961757 android_prober-0.1.6/android_prober/platforms/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/android/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/android/realtime_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/android/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/android/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.965757 android_prober-0.1.6/android_prober/platforms/generics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/platforms/generics/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/proxy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.965757 android_prober-0.1.6/android_prober/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.965757 android_prober-0.1.6/android_prober/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-10 04:02:47.000000 android_prober-0.1.6/android_prober/wrappers/register_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.965757 android_prober-0.1.6/android_prober.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-10 04:02:52.000000 android_prober-0.1.6/android_prober.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-10 04:02:52.000000 android_prober-0.1.6/android_prober.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:02:52.000000 android_prober-0.1.6/android_prober.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 04:02:52.000000 android_prober-0.1.6/android_prober.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 04:02:52.000000 android_prober-0.1.6/android_prober.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.957757 android_prober-0.1.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:02:52.965757 android_prober-0.1.6/examples/webview-app/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 04:02:47.000000 android_prober-0.1.6/examples/webview-app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:02:52.965757 android_prober-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-10 04:02:47.000000 android_prober-0.1.6/setup.py
```

### Comparing `android_prober-0.1.5/LICENSE` & `android_prober-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/PKG-INFO` & `android_prober-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `android_prober-0.1.5/README.md` & `android_prober-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/__init__.py` & `android_prober-0.1.6/android_prober/__init__.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/audio.py` & `android_prober-0.1.6/android_prober/apis/audio.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/battery.py` & `android_prober-0.1.6/android_prober/apis/battery.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/bluetooth.py` & `android_prober-0.1.6/android_prober/apis/bluetooth.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/brightness.py` & `android_prober-0.1.6/android_prober/apis/brightness.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/call.py` & `android_prober-0.1.6/android_prober/apis/call.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/camera.py` & `android_prober-0.1.6/android_prober/apis/camera.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/email.py` & `android_prober-0.1.6/android_prober/apis/email.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/filechooser.py` & `android_prober-0.1.6/android_prober/apis/filechooser.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/flash.py` & `android_prober-0.1.6/android_prober/apis/flash.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/gps.py` & `android_prober-0.1.6/android_prober/apis/gps.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/notification.py` & `android_prober-0.1.6/android_prober/apis/notification.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/runtime_permission.py` & `android_prober-0.1.6/android_prober/apis/runtime_permission.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 from inspect import getmembers, ismethod
 from android_prober.wrappers import get
 from android_prober.facades import RuntimePermission
 from android_prober import runtime_permission
 
-class Runtime:
+class RuntimePermission:
 
     def __init__(self) -> None:
         self.runtime_perm: RuntimePermission = runtime_permission
 
     @get(
         summary = "Request Location Permission",
         description = "Using this API we can request the runtime permission for location in android",
@@ -38,10 +38,10 @@
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_runpermission():
-    run_permission = Runtime()
+    run_permission = RuntimePermission()
     run_permission()
     return run_permission
```

### Comparing `android_prober-0.1.5/android_prober/apis/sensors.py` & `android_prober-0.1.6/android_prober/apis/sensors.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/service.py` & `android_prober-0.1.6/android_prober/apis/service.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/tts.py` & `android_prober-0.1.6/android_prober/apis/tts.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/apis/vibrator.py` & `android_prober-0.1.6/android_prober/apis/vibrator.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/app.py` & `android_prober-0.1.6/android_prober/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     from android_prober.apis.gps import register_gps
     from android_prober.apis.battery import register_battery
     from android_prober.apis.email import register_email
     from android_prober.apis.brightness import register_brightness
     from android_prober.apis.camera import register_camera
     from android_prober.apis.service import register_service
     from android_prober.apis.flash import register_flash
+    from android_prober.apis.runtime_permission import register_runpermission
 
 
 
     # REGISTERING THE SERVICE's
 
     register_camera()
     register_audio()
@@ -89,8 +90,9 @@
     register_notify()
     register_call()
     register_brightness()
     register_gps()
     register_battery()
     register_email()
     register_flash()
-    register_service()
+    register_service()
+    register_runpermission()
```

### Comparing `android_prober-0.1.5/android_prober/facades/__init__.py` & `android_prober-0.1.6/android_prober/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/android/bluetooth.py` & `android_prober-0.1.6/android_prober/platforms/android/bluetooth.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/android/realtime_service.py` & `android_prober-0.1.6/android_prober/platforms/android/realtime_service.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/android/runtime_permission.py` & `android_prober-0.1.6/android_prober/platforms/android/runtime_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             return True
         return True
 
 class AndroidRuntimePermission(RuntimePermission):
 
     def __init__(self) -> None:
         self.runtime_perm = AndroidPermission()
-
     
     def location_permission(self):
         status = self.runtime_perm.location_permission()
         return {"status": status, "permission": "Location Permission Requested"}
 
     def bluetooth_permission(self):
         status = self.runtime_perm.blutooth_permission()
@@ -59,9 +58,8 @@
 
     def telephony_permission(self):
         status = self.runtime_perm.telephony_permission()
         return {"status": status, "permission": "Telephony Permission Requested"}
 
 def instance():
     run_permission = AndroidRuntimePermission()
-    run_permission()
     return run_permission
```

### Comparing `android_prober-0.1.5/android_prober/platforms/android/service.py` & `android_prober-0.1.6/android_prober/platforms/android/service.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/audio.py` & `android_prober-0.1.6/android_prober/platforms/generics/audio.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/brightness.py` & `android_prober-0.1.6/android_prober/platforms/generics/brightness.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/call.py` & `android_prober-0.1.6/android_prober/platforms/generics/call.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/camera.py` & `android_prober-0.1.6/android_prober/platforms/generics/camera.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/email.py` & `android_prober-0.1.6/android_prober/platforms/generics/email.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/filechooser.py` & `android_prober-0.1.6/android_prober/platforms/generics/filechooser.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/flash.py` & `android_prober-0.1.6/android_prober/platforms/generics/flash.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/gps.py` & `android_prober-0.1.6/android_prober/platforms/generics/gps.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/notification.py` & `android_prober-0.1.6/android_prober/platforms/generics/notification.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/sensor.py` & `android_prober-0.1.6/android_prober/platforms/generics/sensor.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/tts.py` & `android_prober-0.1.6/android_prober/platforms/generics/tts.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/platforms/generics/vibrator.py` & `android_prober-0.1.6/android_prober/platforms/generics/vibrator.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/proxy_utils.py` & `android_prober-0.1.6/android_prober/proxy_utils.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/utils/common.py` & `android_prober-0.1.6/android_prober/utils/common.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober/wrappers/register_wrapper.py` & `android_prober-0.1.6/android_prober/wrappers/register_wrapper.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/android_prober.egg-info/PKG-INFO` & `android_prober-0.1.6/android_prober.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `android_prober-0.1.5/android_prober.egg-info/SOURCES.txt` & `android_prober-0.1.6/android_prober.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/examples/webview-app/main.py` & `android_prober-0.1.6/examples/webview-app/main.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.5/setup.py` & `android_prober-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from os import path
 from sys import version_info
 
 current_path = Path(__file__).parent
 full_path = path.join(current_path, "README.md")
 long_discription = ""
-version = "0.1.5"
+version = "0.1.6"
 name = "android-prober"
 description = "Library for test android api's via service"
 author = "GunaNeelamegam"
 url = "https://github.com/gunaNeelamegam"
 
 with open(full_path) as fd:
     long_discription = fd.read()
```

