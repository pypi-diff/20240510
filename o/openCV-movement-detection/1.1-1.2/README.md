# Comparing `tmp/openCV_movement_detection-1.1.tar.gz` & `tmp/openCV_movement_detection-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openCV_movement_detection-1.1.tar", last modified: Fri May 10 09:11:35 2024, max compression
+gzip compressed data, was "openCV_movement_detection-1.2.tar", last modified: Fri May 10 09:27:58 2024, max compression
```

## Comparing `openCV_movement_detection-1.1.tar` & `openCV_movement_detection-1.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:11:35.652999 openCV_movement_detection-1.1/
--rw-rw-rw-   0        0        0      194 2024-05-10 09:11:35.650993 openCV_movement_detection-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 09:11:35.648995 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/
--rw-rw-rw-   0        0        0      194 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:11:35.000000 openCV_movement_detection-1.1/openCV_movement_detection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:11:35.652999 openCV_movement_detection-1.1/setup.cfg
--rw-rw-rw-   0        0        0      299 2024-05-10 09:11:32.000000 openCV_movement_detection-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:58.270878 openCV_movement_detection-1.2/
+-rw-rw-rw-   0        0        0      194 2024-05-10 09:27:58.269374 openCV_movement_detection-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:58.255168 openCV_movement_detection-1.2/openCV_movement_detection/
+-rw-rw-rw-   0        0        0        0 2024-05-10 09:26:55.000000 openCV_movement_detection-1.2/openCV_movement_detection/__init__.py
+-rw-rw-rw-   0        0        0     2535 2024-05-10 09:19:53.000000 openCV_movement_detection-1.2/openCV_movement_detection/details_movement.py
+-rw-rw-rw-   0        0        0     1630 2024-05-10 09:27:53.000000 openCV_movement_detection-1.2/openCV_movement_detection/video_movement_class.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:58.267374 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/
+-rw-rw-rw-   0        0        0      194 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:27:58.270878 openCV_movement_detection-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      299 2024-05-10 09:27:53.000000 openCV_movement_detection-1.2/setup.py
```

