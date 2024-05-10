# Comparing `tmp/openCV_movement_detection-1.2.tar.gz` & `tmp/openCV_movement_detection-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openCV_movement_detection-1.2.tar", last modified: Fri May 10 09:27:58 2024, max compression
+gzip compressed data, was "openCV_movement_detection-1.3.tar", last modified: Fri May 10 09:39:21 2024, max compression
```

## Comparing `openCV_movement_detection-1.2.tar` & `openCV_movement_detection-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:27:58.270878 openCV_movement_detection-1.2/
--rw-rw-rw-   0        0        0      194 2024-05-10 09:27:58.269374 openCV_movement_detection-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 09:27:58.255168 openCV_movement_detection-1.2/openCV_movement_detection/
--rw-rw-rw-   0        0        0        0 2024-05-10 09:26:55.000000 openCV_movement_detection-1.2/openCV_movement_detection/__init__.py
--rw-rw-rw-   0        0        0     2535 2024-05-10 09:19:53.000000 openCV_movement_detection-1.2/openCV_movement_detection/details_movement.py
--rw-rw-rw-   0        0        0     1630 2024-05-10 09:27:53.000000 openCV_movement_detection-1.2/openCV_movement_detection/video_movement_class.py
-drwxrwxrwx   0        0        0        0 2024-05-10 09:27:58.267374 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/
--rw-rw-rw-   0        0        0      194 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-10 09:27:58.000000 openCV_movement_detection-1.2/openCV_movement_detection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:27:58.270878 openCV_movement_detection-1.2/setup.cfg
--rw-rw-rw-   0        0        0      299 2024-05-10 09:27:53.000000 openCV_movement_detection-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:39:21.234591 openCV_movement_detection-1.3/
+-rw-rw-rw-   0        0        0      194 2024-05-10 09:39:21.232590 openCV_movement_detection-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 09:39:21.220563 openCV_movement_detection-1.3/openCV_movement_detection/
+-rw-rw-rw-   0        0        0        0 2024-05-10 09:26:55.000000 openCV_movement_detection-1.3/openCV_movement_detection/__init__.py
+-rw-rw-rw-   0        0        0     2535 2024-05-10 09:19:53.000000 openCV_movement_detection-1.3/openCV_movement_detection/details_movement.py
+-rw-rw-rw-   0        0        0     1656 2024-05-10 09:39:17.000000 openCV_movement_detection-1.3/openCV_movement_detection/video_movement_class.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:39:21.231590 openCV_movement_detection-1.3/openCV_movement_detection.egg-info/
+-rw-rw-rw-   0        0        0      194 2024-05-10 09:39:21.000000 openCV_movement_detection-1.3/openCV_movement_detection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-10 09:39:21.000000 openCV_movement_detection-1.3/openCV_movement_detection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:39:21.000000 openCV_movement_detection-1.3/openCV_movement_detection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 09:39:21.000000 openCV_movement_detection-1.3/openCV_movement_detection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-10 09:39:21.000000 openCV_movement_detection-1.3/openCV_movement_detection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:39:21.234591 openCV_movement_detection-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      299 2024-05-10 09:39:17.000000 openCV_movement_detection-1.3/setup.py
```

### Comparing `openCV_movement_detection-1.2/openCV_movement_detection/details_movement.py` & `openCV_movement_detection-1.3/openCV_movement_detection/details_movement.py`

 * *Files identical despite different names*

### Comparing `openCV_movement_detection-1.2/openCV_movement_detection/video_movement_class.py` & `openCV_movement_detection-1.3/openCV_movement_detection/video_movement_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import cv2
-from details_movement import change_frame, get_mask, contour_movement, text_movement, \
+from openCV_movement_detection.details_movement import change_frame, get_mask, contour_movement, text_movement, \
     make_video_no_roi, make_video_roi
 
 
 class VideoMovementClass:
 
     def detect_movement(self, path, rois, no_rois, min_contour_area=10, circularity_threshold=0.5, blur=1, brightness=1):
         cap = cv2.VideoCapture(path)
```

