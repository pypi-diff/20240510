# Comparing `tmp/neuralneuron-14.6.tar.gz` & `tmp/neuralneuron-15.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralneuron-14.6.tar", last modified: Thu May  9 18:54:51 2024, max compression
+gzip compressed data, was "neuralneuron-15.6.tar", last modified: Thu May  9 19:03:12 2024, max compression
```

## Comparing `neuralneuron-14.6.tar` & `neuralneuron-15.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 18:54:51.020149 neuralneuron-14.6/
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-09 18:54:51.020149 neuralneuron-14.6/PKG-INFO
-drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 18:54:51.019149 neuralneuron-14.6/neuralneuron/
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1727 2024-05-09 18:50:37.000000 neuralneuron-14.6/neuralneuron/A1.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      767 2024-05-09 18:00:54.000000 neuralneuron-14.6/neuralneuron/A2.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1315 2024-05-09 18:33:16.000000 neuralneuron-14.6/neuralneuron/A3.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1126 2024-05-09 18:33:37.000000 neuralneuron-14.6/neuralneuron/A4.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      797 2024-05-09 18:00:54.000000 neuralneuron-14.6/neuralneuron/A5.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     2129 2024-05-09 18:14:14.000000 neuralneuron-14.6/neuralneuron/A8.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     3215 2024-05-09 18:00:54.000000 neuralneuron-14.6/neuralneuron/B1.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1123 2024-05-09 18:00:54.000000 neuralneuron-14.6/neuralneuron/B4.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     4468 2024-05-09 18:00:54.000000 neuralneuron-14.6/neuralneuron/C2.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1532 2024-05-09 18:00:54.000000 neuralneuron-14.6/neuralneuron/C4.py
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 18:00:54.000000 neuralneuron-14.6/neuralneuron/__init__.py
-drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 18:54:51.020149 neuralneuron-14.6/neuralneuron.egg-info/
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-09 18:54:50.000000 neuralneuron-14.6/neuralneuron.egg-info/PKG-INFO
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      367 2024-05-09 18:54:50.000000 neuralneuron-14.6/neuralneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        1 2024-05-09 18:54:50.000000 neuralneuron-14.6/neuralneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       13 2024-05-09 18:54:50.000000 neuralneuron-14.6/neuralneuron.egg-info/top_level.txt
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       38 2024-05-09 18:54:51.020149 neuralneuron-14.6/setup.cfg
--rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      300 2024-05-09 18:54:35.000000 neuralneuron-14.6/setup.py
+drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 19:03:12.355292 neuralneuron-15.6/
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-09 19:03:12.355292 neuralneuron-15.6/PKG-INFO
+drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 19:03:12.354292 neuralneuron-15.6/neuralneuron/
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1727 2024-05-09 18:50:37.000000 neuralneuron-15.6/neuralneuron/A1.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      767 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/A2.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1315 2024-05-09 18:33:16.000000 neuralneuron-15.6/neuralneuron/A3.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1126 2024-05-09 18:33:37.000000 neuralneuron-15.6/neuralneuron/A4.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1199 2024-05-09 19:02:31.000000 neuralneuron-15.6/neuralneuron/A5.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     2129 2024-05-09 18:14:14.000000 neuralneuron-15.6/neuralneuron/A8.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     3215 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/B1.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1123 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/B4.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     4468 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/C2.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)     1532 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/C4.py
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 18:00:54.000000 neuralneuron-15.6/neuralneuron/__init__.py
+drwxrwxr-x   0 noobtain  (1000) noobtain  (1000)        0 2024-05-09 19:03:12.354292 neuralneuron-15.6/neuralneuron.egg-info/
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      193 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      367 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)        1 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       13 2024-05-09 19:03:12.000000 neuralneuron-15.6/neuralneuron.egg-info/top_level.txt
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)       38 2024-05-09 19:03:12.355292 neuralneuron-15.6/setup.cfg
+-rw-rw-r--   0 noobtain  (1000) noobtain  (1000)      300 2024-05-09 19:02:15.000000 neuralneuron-15.6/setup.py
```

### Comparing `neuralneuron-14.6/neuralneuron/A1.py` & `neuralneuron-15.6/neuralneuron/A1.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/A2.py` & `neuralneuron-15.6/neuralneuron/A2.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/A3.py` & `neuralneuron-15.6/neuralneuron/A3.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/A4.py` & `neuralneuron-15.6/neuralneuron/A4.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/A8.py` & `neuralneuron-15.6/neuralneuron/A8.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/B1.py` & `neuralneuron-15.6/neuralneuron/B1.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/B4.py` & `neuralneuron-15.6/neuralneuron/B4.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/C2.py` & `neuralneuron-15.6/neuralneuron/C2.py`

 * *Files identical despite different names*

### Comparing `neuralneuron-14.6/neuralneuron/C4.py` & `neuralneuron-15.6/neuralneuron/C4.py`

 * *Files identical despite different names*

