# Comparing `tmp/neuralneuron-15.6.tar.gz` & `tmp/neuralneuron-16.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralneuron-15.6.tar", last modified: Thu May  9 19:03:12 2024, max compression
+gzip compressed data, was "neuralneuron-16.5.tar", last modified: Fri May 10 16:34:43 2024, max compression
```

## Comparing `neuralneuron-15.6.tar` & `neuralneuron-16.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 19:03:12.355292 neuralneuron-15.6/
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-09 19:03:12.355292 neuralneuron-15.6/PKG-INFO
-drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 19:03:12.354292 neuralneuron-15.6/neuralneuron/
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1727 2024-05-09 18:50:37.000000 neuralneuron-15.6/neuralneuron/A1.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      767 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/A2.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1315 2024-05-09 18:33:16.000000 neuralneuron-15.6/neuralneuron/A3.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1126 2024-05-09 18:33:37.000000 neuralneuron-15.6/neuralneuron/A4.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1199 2024-05-09 19:02:31.000000 neuralneuron-15.6/neuralneuron/A5.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     2129 2024-05-09 18:14:14.000000 neuralneuron-15.6/neuralneuron/A8.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     3215 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/B1.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1123 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/B4.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     4468 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/C2.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1532 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/C4.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/__init__.py
-drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 19:03:12.354292 neuralneuron-15.6/neuralneuron.egg-info/
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/PKG-INFO
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      367 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        1 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       13 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/top_level.txt
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       38 2024-05-09 19:03:12.355292 neuralneuron-15.6/setup.cfg
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      300 2024-05-09 19:02:15.000000 neuralneuron-15.6/setup.py
+drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-10 16:34:43.947871 neuralneuron-16.5/
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-10 16:34:43.947871 neuralneuron-16.5/PKG-INFO
+drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-10 16:34:43.946871 neuralneuron-16.5/neuralneuron/
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1727 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/A1.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      767 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/A2.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1315 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/A3.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1126 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/A4.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1199 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/A5.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     2129 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/A8.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     3215 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/B1.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1123 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/B4.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     4468 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/C2.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1532 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/C4.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        0 2024-05-10 16:16:25.000000 neuralneuron-16.5/neuralneuron/__init__.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     2979 2024-05-10 16:33:13.000000 neuralneuron-16.5/neuralneuron/practical1.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     2143 2024-05-10 16:31:59.000000 neuralneuron-16.5/neuralneuron/practical2.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     3147 2024-05-10 16:32:36.000000 neuralneuron-16.5/neuralneuron/practical4.py
+drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-10 16:34:43.946871 neuralneuron-16.5/neuralneuron.egg-info/
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-10 16:34:43.000000 neuralneuron-16.5/neuralneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      448 2024-05-10 16:34:43.000000 neuralneuron-16.5/neuralneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        1 2024-05-10 16:34:43.000000 neuralneuron-16.5/neuralneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       13 2024-05-10 16:34:43.000000 neuralneuron-16.5/neuralneuron.egg-info/top_level.txt
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       38 2024-05-10 16:34:43.947871 neuralneuron-16.5/setup.cfg
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      289 2024-05-10 16:34:36.000000 neuralneuron-16.5/setup.py
```

### Comparing `neuralneuron-15.6/neuralneuron/A1.py` & `neuralneuron-16.5/neuralneuron/A1.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/A2.py` & `neuralneuron-16.5/neuralneuron/A2.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/A3.py` & `neuralneuron-16.5/neuralneuron/A3.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/A4.py` & `neuralneuron-16.5/neuralneuron/A4.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/A5.py` & `neuralneuron-16.5/neuralneuron/A5.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/A8.py` & `neuralneuron-16.5/neuralneuron/A8.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/B1.py` & `neuralneuron-16.5/neuralneuron/B1.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/B4.py` & `neuralneuron-16.5/neuralneuron/B4.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/C2.py` & `neuralneuron-16.5/neuralneuron/C2.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-15.6/neuralneuron/C4.py` & `neuralneuron-16.5/neuralneuron/C4.py`

 * *Files identical despite different names*

