# Comparing `tmp/focusployer-1.0.tar.gz` & `tmp/focusployer-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "focusployer-1.0.tar", last modified: Fri May 10 15:35:10 2024, max compression
+gzip compressed data, was "focusployer-1.1.tar", last modified: Fri May 10 15:40:04 2024, max compression
```

## Comparing `focusployer-1.0.tar` & `focusployer-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-10 15:35:10.178519 focusployer-1.0/
--rw-r--r--   0 evsi       (501) staff       (20)      111 2024-05-10 15:35:10.178315 focusployer-1.0/PKG-INFO
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-10 15:35:10.177466 focusployer-1.0/focusployer/
--rw-r--r--   0 evsi       (501) staff       (20)      130 2024-05-10 12:12:21.000000 focusployer-1.0/focusployer/__init__.py
--rw-r--r--   0 evsi       (501) staff       (20)     3539 2024-05-10 12:02:28.000000 focusployer-1.0/focusployer/deployer.py
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-10 15:35:10.178086 focusployer-1.0/focusployer.egg-info/
--rw-r--r--   0 evsi       (501) staff       (20)      111 2024-05-10 15:35:10.000000 focusployer-1.0/focusployer.egg-info/PKG-INFO
--rw-r--r--   0 evsi       (501) staff       (20)      230 2024-05-10 15:35:10.000000 focusployer-1.0/focusployer.egg-info/SOURCES.txt
--rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-10 15:35:10.000000 focusployer-1.0/focusployer.egg-info/dependency_links.txt
--rw-r--r--   0 evsi       (501) staff       (20)       16 2024-05-10 15:35:10.000000 focusployer-1.0/focusployer.egg-info/requires.txt
--rw-r--r--   0 evsi       (501) staff       (20)       12 2024-05-10 15:35:10.000000 focusployer-1.0/focusployer.egg-info/top_level.txt
--rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-10 15:35:10.178563 focusployer-1.0/setup.cfg
--rw-r--r--   0 evsi       (501) staff       (20)      196 2024-05-10 15:34:57.000000 focusployer-1.0/setup.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-10 15:40:04.554712 focusployer-1.1/
+-rw-r--r--   0 evsi       (501) staff       (20)     1815 2024-05-10 15:40:04.554405 focusployer-1.1/PKG-INFO
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-10 15:40:04.553527 focusployer-1.1/focusployer/
+-rw-rw-r--   0 evsi       (501) staff       (20)      130 2024-05-10 15:28:29.000000 focusployer-1.1/focusployer/__init__.py
+-rw-rw-r--   0 evsi       (501) staff       (20)     3539 2024-05-10 15:28:29.000000 focusployer-1.1/focusployer/deployer.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-10 15:40:04.554162 focusployer-1.1/focusployer.egg-info/
+-rw-r--r--   0 evsi       (501) staff       (20)     1815 2024-05-10 15:40:04.000000 focusployer-1.1/focusployer.egg-info/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)      230 2024-05-10 15:40:04.000000 focusployer-1.1/focusployer.egg-info/SOURCES.txt
+-rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-10 15:40:04.000000 focusployer-1.1/focusployer.egg-info/dependency_links.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       16 2024-05-10 15:40:04.000000 focusployer-1.1/focusployer.egg-info/requires.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       12 2024-05-10 15:40:04.000000 focusployer-1.1/focusployer.egg-info/top_level.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-10 15:40:04.554759 focusployer-1.1/setup.cfg
+-rw-r--r--   0 evsi       (501) staff       (20)      295 2024-05-10 15:39:24.000000 focusployer-1.1/setup.py
```

### Comparing `focusployer-1.0/focusployer/deployer.py` & `focusployer-1.1/focusployer/deployer.py`

 * *Files identical despite different names*

