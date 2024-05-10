# Comparing `tmp/android_prober-0.1.3.tar.gz` & `tmp/android_prober-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android_prober-0.1.3.tar", last modified: Thu May  9 13:58:20 2024, max compression
+gzip compressed data, was "android_prober-0.1.4.tar", last modified: Thu May  9 14:43:06 2024, max compression
```

## Comparing `android_prober-0.1.3.tar` & `android_prober-0.1.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-09 13:58:11.000000 android_prober-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 13:58:20.599536 android_prober-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 13:58:11.000000 android_prober-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.587536 android_prober-0.1.3/android_prober/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.591536 android_prober-0.1.3/android_prober/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/vibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.595536 android_prober-0.1.3/android_prober/facades/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/call.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/service.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/vibrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.587536 android_prober-0.1.3/android_prober/platforms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.595536 android_prober-0.1.3/android_prober/platforms/android/
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/realtime_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober/platforms/generics/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/vibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/proxy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/wrappers/register_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.587536 android_prober-0.1.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/examples/webview-app/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-09 13:58:11.000000 android_prober-0.1.3/examples/webview-app/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:58:20.599536 android_prober-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 13:58:11.000000 android_prober-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-09 14:43:01.000000 android_prober-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 14:43:06.738752 android_prober-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 14:43:01.000000 android_prober-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.726751 android_prober-0.1.4/android_prober/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.730751 android_prober-0.1.4/android_prober/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.734751 android_prober-0.1.4/android_prober/facades/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/vibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.726751 android_prober-0.1.4/android_prober/platforms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.734751 android_prober-0.1.4/android_prober/platforms/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/realtime_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober/platforms/generics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/proxy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/wrappers/register_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.726751 android_prober-0.1.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/examples/webview-app/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-09 14:43:01.000000 android_prober-0.1.4/examples/webview-app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:43:06.738752 android_prober-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 14:43:01.000000 android_prober-0.1.4/setup.py
```

### Comparing `android_prober-0.1.3/LICENSE` & `android_prober-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/PKG-INFO` & `android_prober-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `android_prober-0.1.3/README.md` & `android_prober-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/__init__.py` & `android_prober-0.1.4/android_prober/__init__.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/audio.py` & `android_prober-0.1.4/android_prober/apis/audio.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/battery.py` & `android_prober-0.1.4/android_prober/apis/battery.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/bluetooth.py` & `android_prober-0.1.4/android_prober/apis/bluetooth.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/brightness.py` & `android_prober-0.1.4/android_prober/apis/brightness.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/call.py` & `android_prober-0.1.4/android_prober/apis/call.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/camera.py` & `android_prober-0.1.4/android_prober/apis/camera.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/email.py` & `android_prober-0.1.4/android_prober/apis/email.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/filechooser.py` & `android_prober-0.1.4/android_prober/apis/filechooser.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/flash.py` & `android_prober-0.1.4/android_prober/apis/flash.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/gps.py` & `android_prober-0.1.4/android_prober/apis/gps.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/notification.py` & `android_prober-0.1.4/android_prober/apis/notification.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/runtime_permission.py` & `android_prober-0.1.4/android_prober/apis/runtime_permission.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/sensors.py` & `android_prober-0.1.4/android_prober/apis/sensors.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/service.py` & `android_prober-0.1.4/android_prober/apis/service.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/tts.py` & `android_prober-0.1.4/android_prober/apis/tts.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/apis/vibrator.py` & `android_prober-0.1.4/android_prober/apis/vibrator.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/app.py` & `android_prober-0.1.4/android_prober/app.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/facades/__init__.py` & `android_prober-0.1.4/android_prober/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/android/bluetooth.py` & `android_prober-0.1.4/android_prober/platforms/android/bluetooth.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/android/realtime_service.py` & `android_prober-0.1.4/android_prober/platforms/android/realtime_service.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/android/runtime_permission.py` & `android_prober-0.1.4/android_prober/platforms/android/runtime_permission.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/android/service.py` & `android_prober-0.1.4/android_prober/platforms/android/service.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/audio.py` & `android_prober-0.1.4/android_prober/platforms/generics/audio.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/brightness.py` & `android_prober-0.1.4/android_prober/platforms/generics/brightness.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/call.py` & `android_prober-0.1.4/android_prober/platforms/generics/call.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/camera.py` & `android_prober-0.1.4/android_prober/platforms/generics/camera.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/email.py` & `android_prober-0.1.4/android_prober/platforms/generics/email.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/filechooser.py` & `android_prober-0.1.4/android_prober/platforms/generics/filechooser.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/flash.py` & `android_prober-0.1.4/android_prober/platforms/generics/flash.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/gps.py` & `android_prober-0.1.4/android_prober/platforms/generics/gps.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/notification.py` & `android_prober-0.1.4/android_prober/platforms/generics/notification.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/sensor.py` & `android_prober-0.1.4/android_prober/platforms/generics/sensor.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/tts.py` & `android_prober-0.1.4/android_prober/platforms/generics/tts.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/platforms/generics/vibrator.py` & `android_prober-0.1.4/android_prober/platforms/generics/vibrator.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/proxy_utils.py` & `android_prober-0.1.4/android_prober/proxy_utils.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/utils/common.py` & `android_prober-0.1.4/android_prober/utils/common.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober/wrappers/register_wrapper.py` & `android_prober-0.1.4/android_prober/wrappers/register_wrapper.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/android_prober.egg-info/PKG-INFO` & `android_prober-0.1.4/android_prober.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `android_prober-0.1.3/android_prober.egg-info/SOURCES.txt` & `android_prober-0.1.4/android_prober.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/examples/webview-app/main.py` & `android_prober-0.1.4/examples/webview-app/main.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.3/setup.py` & `android_prober-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from os import path
 from sys import version_info
 
 current_path = Path(__file__).parent
 full_path = path.join(current_path, "README.md")
 long_discription = ""
-version = "0.1.3"
+version = "0.1.4"
 name = "android-prober"
 description = "Library for test android api's via service"
 author = "GunaNeelamegam"
 url = "https://github.com/gunaNeelamegam"
 
 with open(full_path) as fd:
     long_discription = fd.read()
```

