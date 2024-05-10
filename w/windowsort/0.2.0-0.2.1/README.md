# Comparing `tmp/windowsort-0.2.0.tar.gz` & `tmp/windowsort-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windowsort-0.2.0.tar", last modified: Wed Oct 18 20:03:56 2023, max compression
+gzip compressed data, was "windowsort-0.2.1.tar", last modified: Fri May 10 15:53:41 2024, max compression
```

## Comparing `windowsort-0.2.0.tar` & `windowsort-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-18 20:03:56.536052 windowsort-0.2.0/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      165 2023-10-18 20:03:56.536052 windowsort-0.2.0/PKG-INFO
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       12 2023-10-17 18:52:17.000000 windowsort-0.2.0/README.md
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       38 2023-10-18 20:03:56.536052 windowsort-0.2.0/setup.cfg
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      507 2023-10-18 20:01:47.000000 windowsort-0.2.0/setup.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-18 20:03:56.532052 windowsort-0.2.0/src/
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-18 20:03:56.536052 windowsort-0.2.0/src/windowsort/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 windowsort-0.2.0/src/windowsort/__init__.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      526 2023-10-18 16:42:48.000000 windowsort-0.2.0/src/windowsort/colors.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    12016 2023-10-18 19:48:36.000000 windowsort-0.2.0/src/windowsort/datahandler.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    11718 2023-10-18 17:08:33.000000 windowsort-0.2.0/src/windowsort/drift.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    11379 2023-10-18 19:49:42.000000 windowsort-0.2.0/src/windowsort/gui.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     8197 2023-09-29 20:43:03.000000 windowsort-0.2.0/src/windowsort/snapshot.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     7002 2023-10-18 18:05:05.000000 windowsort-0.2.0/src/windowsort/spikes.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      600 2023-09-29 20:43:03.000000 windowsort-0.2.0/src/windowsort/threshold.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    12298 2023-10-18 16:59:04.000000 windowsort-0.2.0/src/windowsort/timeamplitudewindow.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    15771 2023-10-18 18:40:03.000000 windowsort-0.2.0/src/windowsort/units.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     7466 2023-10-18 18:43:47.000000 windowsort-0.2.0/src/windowsort/voltage.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-18 20:03:56.536052 windowsort-0.2.0/src/windowsort.egg-info/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      165 2023-10-18 20:03:56.000000 windowsort-0.2.0/src/windowsort.egg-info/PKG-INFO
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      544 2023-10-18 20:03:56.000000 windowsort-0.2.0/src/windowsort.egg-info/SOURCES.txt
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        1 2023-10-18 20:03:56.000000 windowsort-0.2.0/src/windowsort.egg-info/dependency_links.txt
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       51 2023-10-18 20:03:56.000000 windowsort-0.2.0/src/windowsort.egg-info/entry_points.txt
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      136 2023-10-18 20:03:56.000000 windowsort-0.2.0/src/windowsort.egg-info/requires.txt
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       11 2023-10-18 20:03:56.000000 windowsort-0.2.0/src/windowsort.egg-info/top_level.txt
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-10 15:53:41.296290 windowsort-0.2.1/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      165 2024-05-10 15:53:41.296290 windowsort-0.2.1/PKG-INFO
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       56 2023-10-18 20:11:48.000000 windowsort-0.2.1/README.md
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       38 2024-05-10 15:53:41.296290 windowsort-0.2.1/setup.cfg
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      507 2024-05-10 15:29:46.000000 windowsort-0.2.1/setup.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-10 15:53:41.292291 windowsort-0.2.1/src/
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-10 15:53:41.296290 windowsort-0.2.1/src/windowsort/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 windowsort-0.2.1/src/windowsort/__init__.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      526 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/colors.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    12016 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/datahandler.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    11718 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/drift.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    11379 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/gui.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     8197 2023-09-29 20:43:03.000000 windowsort-0.2.1/src/windowsort/snapshot.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     7002 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/spikes.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      600 2023-09-29 20:43:03.000000 windowsort-0.2.1/src/windowsort/threshold.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    12298 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/timeamplitudewindow.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    15771 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/units.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     7466 2023-10-18 20:10:04.000000 windowsort-0.2.1/src/windowsort/voltage.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-10 15:53:41.296290 windowsort-0.2.1/src/windowsort.egg-info/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      165 2024-05-10 15:53:41.000000 windowsort-0.2.1/src/windowsort.egg-info/PKG-INFO
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      544 2024-05-10 15:53:41.000000 windowsort-0.2.1/src/windowsort.egg-info/SOURCES.txt
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        1 2024-05-10 15:53:41.000000 windowsort-0.2.1/src/windowsort.egg-info/dependency_links.txt
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       51 2024-05-10 15:53:41.000000 windowsort-0.2.1/src/windowsort.egg-info/entry_points.txt
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      144 2024-05-10 15:53:41.000000 windowsort-0.2.1/src/windowsort.egg-info/requires.txt
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       11 2024-05-10 15:53:41.000000 windowsort-0.2.1/src/windowsort.egg-info/top_level.txt
```

### Comparing `windowsort-0.2.0/src/windowsort/colors.py` & `windowsort-0.2.1/src/windowsort/colors.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/datahandler.py` & `windowsort-0.2.1/src/windowsort/datahandler.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/drift.py` & `windowsort-0.2.1/src/windowsort/drift.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/gui.py` & `windowsort-0.2.1/src/windowsort/gui.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/snapshot.py` & `windowsort-0.2.1/src/windowsort/snapshot.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/spikes.py` & `windowsort-0.2.1/src/windowsort/spikes.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/threshold.py` & `windowsort-0.2.1/src/windowsort/threshold.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/timeamplitudewindow.py` & `windowsort-0.2.1/src/windowsort/timeamplitudewindow.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/units.py` & `windowsort-0.2.1/src/windowsort/units.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort/voltage.py` & `windowsort-0.2.1/src/windowsort/voltage.py`

 * *Files identical despite different names*

### Comparing `windowsort-0.2.0/src/windowsort.egg-info/SOURCES.txt` & `windowsort-0.2.1/src/windowsort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

