# Comparing `tmp/openCV_movement_detection-1.0.tar.gz` & `tmp/openCV_movement_detection-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openCV_movement_detection-1.0.tar", last modified: Fri May 10 08:16:10 2024, max compression
+gzip compressed data, was "openCV_movement_detection-1.1.tar", last modified: Fri May 10 09:11:35 2024, max compression
```

## Comparing `openCV_movement_detection-1.0.tar` & `openCV_movement_detection-1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.476048 openCV_movement_detection-1.0/
--rw-rw-rw-   0        0        0      176 2024-05-10 08:16:10.474510 openCV_movement_detection-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.472961 openCV_movement_detection-1.0/openCV_movement_detection.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-10 08:16:10.000000 openCV_movement_detection-1.0/openCV_movement_detection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-10 08:16:10.000000 openCV_movement_detection-1.0/openCV_movement_detection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:16:10.000000 openCV_movement_detection-1.0/openCV_movement_detection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 08:16:10.000000 openCV_movement_detection-1.0/openCV_movement_detection.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:16:10.000000 openCV_movement_detection-1.0/openCV_movement_detection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:16:10.476560 openCV_movement_detection-1.0/setup.cfg
--rw-rw-rw-   0        0        0      281 2024-05-10 08:14:10.000000 openCV_movement_detection-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:11:35.652999 openCV_movement_detection-1.1/
+-rw-rw-rw-   0        0        0      194 2024-05-10 09:11:35.650993 openCV_movement_detection-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 09:11:35.648995 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/
+-rw-rw-rw-   0        0        0      194 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:11:35.652999 openCV_movement_detection-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      299 2024-05-10 09:11:32.000000 openCV_movement_detection-1.1/setup.py
```

