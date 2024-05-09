# Comparing `tmp/bridgecrew-3.2.89.tar.gz` & `tmp/bridgecrew-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bridgecrew-3.2.89.tar", last modified: Thu May  9 22:23:13 2024, max compression
+gzip compressed data, was "dist/bridgecrew-3.2.9.tar", last modified: Tue Feb  6 08:03:11 2024, max compression
```

## Comparing `bridgecrew-3.2.89.tar` & `bridgecrew-3.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2024-02-04 07:49:10.000000 bridgecrew-3.2.89/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bin/
--rwxr-xr-x   0 root         (0) root         (0)       93 2024-02-04 07:49:10.000000 bridgecrew-3.2.89/bin/bridgecrew
--rw-r--r--   0 root         (0) root         (0)     1368 2024-02-04 07:49:10.000000 bridgecrew-3.2.89/bin/bridgecrew.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bridgecrew/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-04 07:49:10.000000 bridgecrew-3.2.89/bridgecrew/__init__.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-02-04 07:49:10.000000 bridgecrew-3.2.89/bridgecrew/banner.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-02-04 07:49:10.000000 bridgecrew-3.2.89/bridgecrew/main.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-09 22:23:09.000000 bridgecrew-3.2.89/bridgecrew/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bridgecrew.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bridgecrew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bridgecrew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bridgecrew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bridgecrew.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/bridgecrew.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 22:23:13.000000 bridgecrew-3.2.89/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2024-02-04 07:49:10.000000 bridgecrew-3.2.89/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2024-01-22 12:14:48.000000 bridgecrew-3.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       93 2024-01-22 12:14:48.000000 bridgecrew-3.2.9/bin/bridgecrew
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-01-22 12:14:48.000000 bridgecrew-3.2.9/bin/bridgecrew.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bridgecrew/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-22 12:14:48.000000 bridgecrew-3.2.9/bridgecrew/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-01-22 12:14:48.000000 bridgecrew-3.2.9/bridgecrew/banner.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-01-22 12:14:48.000000 bridgecrew-3.2.9/bridgecrew/main.py
+-rw-r--r--   0 root         (0) root         (0)       18 2024-02-06 08:03:06.000000 bridgecrew-3.2.9/bridgecrew/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bridgecrew.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bridgecrew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bridgecrew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bridgecrew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bridgecrew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/bridgecrew.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-06 08:03:11.000000 bridgecrew-3.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-01-22 12:14:48.000000 bridgecrew-3.2.9/setup.py
```

### Comparing `bridgecrew-3.2.89/PKG-INFO` & `bridgecrew-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.89
+Version: 3.2.9
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Description: # DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
```

### Comparing `bridgecrew-3.2.89/bin/bridgecrew.cmd` & `bridgecrew-3.2.9/bin/bridgecrew.cmd`

 * *Files identical despite different names*

### Comparing `bridgecrew-3.2.89/bridgecrew.egg-info/PKG-INFO` & `bridgecrew-3.2.9/bridgecrew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.89
+Version: 3.2.9
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Description: # DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
```

### Comparing `bridgecrew-3.2.89/setup.py` & `bridgecrew-3.2.9/setup.py`

 * *Files identical despite different names*

