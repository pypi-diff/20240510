# Comparing `tmp/android_prober-0.1.4.tar.gz` & `tmp/android_prober-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android_prober-0.1.4.tar", last modified: Thu May  9 14:43:06 2024, max compression
+gzip compressed data, was "android_prober-0.1.5.tar", last modified: Fri May 10 03:47:19 2024, max compression
```

## Comparing `android_prober-0.1.4.tar` & `android_prober-0.1.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-09 14:43:01.000000 android_prober-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 14:43:06.738752 android_prober-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 14:43:01.000000 android_prober-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.726751 android_prober-0.1.4/android_prober/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.730751 android_prober-0.1.4/android_prober/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/apis/vibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.734751 android_prober-0.1.4/android_prober/facades/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/call.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/service.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/facades/vibrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.726751 android_prober-0.1.4/android_prober/platforms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.734751 android_prober-0.1.4/android_prober/platforms/android/
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/realtime_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/runtime_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/android/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober/platforms/generics/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/filechooser.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/flash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/platforms/generics/vibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/proxy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-09 14:43:01.000000 android_prober-0.1.4/android_prober/wrappers/register_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/android_prober.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 14:43:06.000000 android_prober-0.1.4/android_prober.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.726751 android_prober-0.1.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:43:06.738752 android_prober-0.1.4/examples/webview-app/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-09 14:43:01.000000 android_prober-0.1.4/examples/webview-app/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:43:06.738752 android_prober-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 14:43:01.000000 android_prober-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-10 03:47:14.000000 android_prober-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-10 03:47:19.545820 android_prober-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-10 03:47:14.000000 android_prober-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.533820 android_prober-0.1.5/android_prober/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.537820 android_prober-0.1.5/android_prober/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/apis/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.541820 android_prober-0.1.5/android_prober/facades/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/facades/vibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.533820 android_prober-0.1.5/android_prober/platforms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.541820 android_prober-0.1.5/android_prober/platforms/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/realtime_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/android/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober/platforms/generics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/platforms/generics/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/proxy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-10 03:47:14.000000 android_prober-0.1.5/android_prober/wrappers/register_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/android_prober.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 03:47:19.000000 android_prober-0.1.5/android_prober.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.533820 android_prober-0.1.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:47:19.545820 android_prober-0.1.5/examples/webview-app/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 03:47:14.000000 android_prober-0.1.5/examples/webview-app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 03:47:19.545820 android_prober-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-10 03:47:14.000000 android_prober-0.1.5/setup.py
```

### Comparing `android_prober-0.1.4/LICENSE` & `android_prober-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/PKG-INFO` & `android_prober-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `android_prober-0.1.4/README.md` & `android_prober-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/__init__.py` & `android_prober-0.1.5/android_prober/__init__.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/audio.py` & `android_prober-0.1.5/android_prober/apis/audio.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/battery.py` & `android_prober-0.1.5/android_prober/apis/battery.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/bluetooth.py` & `android_prober-0.1.5/android_prober/apis/bluetooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from android_prober import bluetooth
 from android_prober.facades import Bluetooth
 
 class Bluetooth:
 
     def __init__(self) -> None:
         self.bluetooth: Bluetooth = bluetooth
+
     @get(
         summary= "Turn on Bluetooth",
         description= "Using this Api we can able to turn on bluetooth\n Platform Support's Android",
         response_model=[(200, 'Success'), (500, 'Error')]
     )
     def enable(self) -> dict:
         return self.bluetooth.enable()
```

### Comparing `android_prober-0.1.4/android_prober/apis/brightness.py` & `android_prober-0.1.5/android_prober/apis/brightness.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/call.py` & `android_prober-0.1.5/android_prober/apis/call.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/camera.py` & `android_prober-0.1.5/android_prober/apis/camera.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/email.py` & `android_prober-0.1.5/android_prober/apis/email.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/filechooser.py` & `android_prober-0.1.5/android_prober/apis/filechooser.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/flash.py` & `android_prober-0.1.5/android_prober/apis/flash.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 from android_prober.facades import Flash
 from android_prober import flash
 from android_prober.wrappers import get
 from typing import Any
 from inspect import getmembers, ismethod
+
 class Flash:
     def __init__(self) -> None:
         self.status = False
         self.flash : Flash = flash
 
     @get(
         summary = "Flash Off",
         description= "Using this Api Can able to Turn off the flash on android device",
         response_model =  [(201, "Success"), (500, "Failure")]
     )
-    def flash_off(self) -> dict:
+    def off(self) -> dict:
         message = ""
         if self.status:
-            self.flash.off()
-            self.flash.release()
-            message = "Flash OFF Successfully"
-        else:
-            message = "Already Flash OFF"
-
+            return self.flash_off()
         return {
             "status": True,
             "message":message
         }
 
     @get(
         summary = "Flash on",
         description= "Using this Api Can able to Turn on the flash on android device",
         response_model =  [(201, "Success"), (500, "Failure")]
     )
-    def flash_on(self) -> dict:
+    def on(self) -> dict:
         message = ""
         if not self.status:
-            self.flash.on()
-            message = "Flash ON Successfully"
-        else:
-            message = "Flash Already On"
+            return self.flash_on()
         return {
             "status": True,
             "message": message
         }
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
```

### Comparing `android_prober-0.1.4/android_prober/apis/gps.py` & `android_prober-0.1.5/android_prober/apis/gps.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/notification.py` & `android_prober-0.1.5/android_prober/apis/notification.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/runtime_permission.py` & `android_prober-0.1.5/android_prober/apis/runtime_permission.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/sensors.py` & `android_prober-0.1.5/android_prober/apis/sensors.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/service.py` & `android_prober-0.1.5/android_prober/apis/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,23 +10,23 @@
         self.service: Service = service 
 
     @get(
     summary= "Start the BroadCast Receiver as the Service",
     description= "Using this Api We can able to Event's which are broadcasted by the android system",
     response_model=[(200, 'Success'), (500, 'Error')]
     )
-    def start_service(self) -> dict:
+    def start(self) -> dict:
         return self.service.start_service()
 
     @get(
     summary= "Stop the BroadCast Receiver as the Service",
     description= "Using this Api We can able to Event's which are broadcasted by the android system",
     response_model=[(200, 'Success'), (500, 'Error')]
     )
-    def stop_service(self) -> dict:
+    def stop(self) -> dict:
         return self.stop_service()
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
```

### Comparing `android_prober-0.1.4/android_prober/apis/tts.py` & `android_prober-0.1.5/android_prober/apis/tts.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/apis/vibrator.py` & `android_prober-0.1.5/android_prober/apis/vibrator.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/app.py` & `android_prober-0.1.5/android_prober/app.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/facades/__init__.py` & `android_prober-0.1.5/android_prober/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/android/bluetooth.py` & `android_prober-0.1.5/android_prober/platforms/android/bluetooth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from jnius import autoclass
 from typing import Union, Any
-from android_prober.utils.common import Platform
+from functools import lru_cache
 from android.broadcast import BroadcastReceiver
+from android_prober.facades import Bluetooth
 
-class BluetoothAgent:
+System = autoclass("java.lang.System")
+class AndroidBluetooth(Bluetooth):
     BluetoothAdapter = autoclass("android.bluetooth.BluetoothAdapter")
     BluetoothDevice  = autoclass("android.bluetooth.BluetoothDevice")
     SERIAL_PORT_PROFILE_UUID = "00001101-0000-1000-8000-00805F9B34FB"
 
     def __init__(self) -> None:
         self.scanned_devices = set()
         self.connected_device = None
@@ -19,40 +21,39 @@
         self.server_socket = None
 
     def on_scanning(self, context, intent):
         action = intent.getAction()
         if action == self.STARTED:
             self.scanned_devices = None
             self.scanned_devices = set()
-            print("SCANNING STARTED ")
+            System.out.println("SCANNING STARTED ")
 
         elif action == self.FOUND:
             device = intent.getParcelableExtra(self.BluetoothDevice.EXTRA_DEVICE);
             name = intent.getExtra(self.BluetoothDevice.EXTRA_NAME)
             if device:
-                print("SCANNING : ", name, device.toString())
+                System.out.println("SCANNING : " + str(name) + str(device.toString()))
                 if not name:
                     name = ""
-            self.scanned_devices.add(BluetoothAgent.BleDevice(name, device.toString()))
+            self.scanned_devices.add(AndroidBluetooth.BleDevice(name, device.toString()))
 
         elif action == self.FINISHED:
             self.ble_adapter.cancelDiscovery()
             self.boardcast_receiver.stop()
             self.boardcast_receiver = None
-            print("SCANNING STOPED")
+            System.out.println("SCANNING STOPED")
 
-    # 
-    def enable_adapter(self) -> bool:
+    def enable(self) -> bool:
         status = False
         if (self.ble_adapter and not self.ble_adapter.isEnabled()):
             self.ble_adapter.enable()
             status = self.ble_adapter.isEnabled()
         return status
 
-    def disable_adapter(self)->bool:
+    def disable(self)-> bool:
         if (self.ble_adapter and self.ble_adapter.isEnabled()):
             self.ble_adapter.disable()
         return self.ble_adapter.isEnabled()
 
     def paired_devices(self):
         if self.ble_adapter:
             bounded_devices = self.ble_adapter.getBondedDevices().toArray()
@@ -91,19 +92,19 @@
         device = self.ble_adapter.getRemoteDevice(device_info.get("address"))
         if device and device.getBondState()  != self.BluetoothDevice.BOND_NONE:
             UUID = autoclass('java.util.UUID')
             self.connected_device = device.createRfcommSocketToServiceRecord(UUID.fromString(self.SERIAL_PORT_PROFILE_UUID))
             self.connected_device.getInputStream()
             self.connected_device.getOutputStream()
             self.connected_device.connect()
-            print("CONNECTED DEVICE : ", self.connected_device.isConnected(), self.connected_device.getRemoteDevice().toString())
+            System.out.println("CONNECTED DEVICE : " + str(self.connected_device.isConnected()) + str(self.connected_device.getRemoteDevice().toString()))
 
     def disconnect(self):
         if self.connected_device:
-            print("DISCONNECTED : ", self.connected_device.isConnected())
+            System.out.println("DISCONNECTED : " + self.connected_device.isConnected())
             self.connected_device.close()
             self.is_connected = False
             self.connected_device = None
 
     def unpair(self, address: Union[str, Any]):
         if self.ble_adapter and address.strip():
             device = self.ble_adapter.getRemoteDevice(address)
@@ -111,11 +112,16 @@
                 device.removeBond();
     class BleDevice:
         def __init__(self, name ="", address= "") -> None:
             self.name = name
             self.address = address
         
         def __eq__(self, other):
-            return isinstance(other, BluetoothAgent.BleDevice) and (self.name == other.name and self.address == other.address)
+            return isinstance(other, AndroidBluetooth.BleDevice) and (self.name == other.name and self.address == other.address)
 
         def __hash__(self):
             return hash((self.name, self.address))
+
+@lru_cache
+def instance():
+    bluetooth_instance = AndroidBluetooth()
+    return bluetooth_instance
```

### Comparing `android_prober-0.1.4/android_prober/platforms/android/realtime_service.py` & `android_prober-0.1.5/android_prober/platforms/android/realtime_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 
 def get_categorys():
     return filter(lambda key: key.startswith("CATEGORY"), vars(Intent).keys())
 
 def message_loop():
     broadcast_receiver.start()
     while True:
+        System.out.println("ANDROID PROBER");
         if stopped:
             break
         sleep(1)
     unsubscribe_telephonyservice()
     server.terminate_server()
     sleep(0.1)
     server.close()
```

### Comparing `android_prober-0.1.4/android_prober/platforms/android/runtime_permission.py` & `android_prober-0.1.5/android_prober/platforms/android/runtime_permission.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/android/service.py` & `android_prober-0.1.5/android_prober/platforms/android/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,7 +42,10 @@
         try:
             self.service.start(mActivity,'')
             status = True
         except Exception as e:
             print("EXECPTION:", e.args)
         finally :
             return status
+
+def instance():
+    return AndroidService()
```

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/audio.py` & `android_prober-0.1.5/android_prober/platforms/generics/audio.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/brightness.py` & `android_prober-0.1.5/android_prober/platforms/generics/brightness.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/call.py` & `android_prober-0.1.5/android_prober/platforms/generics/call.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/camera.py` & `android_prober-0.1.5/android_prober/platforms/generics/camera.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/email.py` & `android_prober-0.1.5/android_prober/platforms/generics/email.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/filechooser.py` & `android_prober-0.1.5/android_prober/platforms/generics/filechooser.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/flash.py` & `android_prober-0.1.5/android_prober/platforms/generics/flash.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/gps.py` & `android_prober-0.1.5/android_prober/platforms/generics/gps.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/notification.py` & `android_prober-0.1.5/android_prober/platforms/generics/notification.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/sensor.py` & `android_prober-0.1.5/android_prober/platforms/generics/sensor.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/tts.py` & `android_prober-0.1.5/android_prober/platforms/generics/tts.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/platforms/generics/vibrator.py` & `android_prober-0.1.5/android_prober/platforms/generics/vibrator.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/proxy_utils.py` & `android_prober-0.1.5/android_prober/proxy_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Structural Design Pattern Impressed from Plyer Module
 """
-import traceback
 import warnings
 from android_prober.utils.common import platform
 class Proxy:
 
     __slots__ = ['_obj', '_name', '_facade']
 
     def __init__(self, name, facade):
@@ -23,23 +22,23 @@
             name = object.__getattribute__(self, "_name")
             module = "android_prober.platforms.generics.{}".format(name)
             mod = __import__(module, fromlist= ["."])
             obj = mod.instance()
             
         except Exception as e:
             warnings.warn("".join(e.args))
-            traceback.print_exc()
             try:                
                 name = object.__getattribute__(self, '_name')
                 module = 'android_prober.platforms.{}.{}'.format(
                     platform, name)
                 mod = __import__(module, fromlist= ["."])
                 obj = mod.instance()
-            except Exception:
-                traceback.print_exc()
+
+            except Exception as e:
+                warnings.warn("".join(e.args))
                 facade = object.__getattribute__(self, '_facade')
                 obj = facade()
 
         object.__setattr__(self, '_obj', obj)
         return obj
 
     def __getattribute__(self, name):
```

### Comparing `android_prober-0.1.4/android_prober/utils/common.py` & `android_prober-0.1.5/android_prober/utils/common.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober/wrappers/register_wrapper.py` & `android_prober-0.1.5/android_prober/wrappers/register_wrapper.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/android_prober.egg-info/PKG-INFO` & `android_prober-0.1.5/android_prober.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `android_prober-0.1.4/android_prober.egg-info/SOURCES.txt` & `android_prober-0.1.5/android_prober.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/examples/webview-app/main.py` & `android_prober-0.1.5/examples/webview-app/main.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.4/setup.py` & `android_prober-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from os import path
 from sys import version_info
 
 current_path = Path(__file__).parent
 full_path = path.join(current_path, "README.md")
 long_discription = ""
-version = "0.1.4"
+version = "0.1.5"
 name = "android-prober"
 description = "Library for test android api's via service"
 author = "GunaNeelamegam"
 url = "https://github.com/gunaNeelamegam"
 
 with open(full_path) as fd:
     long_discription = fd.read()
```

