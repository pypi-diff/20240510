# Comparing `tmp/utils_woodsx-0.0.1.tar.gz` & `tmp/utils_woodsx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_woodsx-0.0.1.tar", last modified: Fri Jan  5 05:38:17 2024, max compression
+gzip compressed data, was "utils_woodsx-0.0.2.tar", last modified: Fri May 10 10:10:48 2024, max compression
```

## Comparing `utils_woodsx-0.0.1.tar` & `utils_woodsx-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-01-05 05:38:17.632690 utils_woodsx-0.0.1/
--rw-r--r--   0 woods      (501) staff       (20)     1065 2024-01-05 03:10:35.000000 utils_woodsx-0.0.1/LICENSE
--rw-r--r--   0 woods      (501) staff       (20)      411 2024-01-05 05:38:17.631959 utils_woodsx-0.0.1/PKG-INFO
--rw-r--r--   0 woods      (501) staff       (20)       49 2024-01-05 03:06:56.000000 utils_woodsx-0.0.1/README.md
--rw-r--r--   0 woods      (501) staff       (20)      435 2024-01-05 03:06:27.000000 utils_woodsx-0.0.1/pyproject.toml
--rw-r--r--   0 woods      (501) staff       (20)       38 2024-01-05 05:38:17.632820 utils_woodsx-0.0.1/setup.cfg
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-01-05 05:38:17.624766 utils_woodsx-0.0.1/src/
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-01-05 05:38:17.627598 utils_woodsx-0.0.1/src/utils_woodsx/
--rw-r--r--   0 woods      (501) staff       (20)        0 2024-01-05 02:25:38.000000 utils_woodsx-0.0.1/src/utils_woodsx/__init__.py
--rw-r--r--   0 woods      (501) staff       (20)       53 2024-01-05 02:28:11.000000 utils_woodsx-0.0.1/src/utils_woodsx/example.py
-drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-01-05 05:38:17.631259 utils_woodsx-0.0.1/src/utils_woodsx.egg-info/
--rw-r--r--   0 woods      (501) staff       (20)      411 2024-01-05 05:38:17.000000 utils_woodsx-0.0.1/src/utils_woodsx.egg-info/PKG-INFO
--rw-r--r--   0 woods      (501) staff       (20)      249 2024-01-05 05:38:17.000000 utils_woodsx-0.0.1/src/utils_woodsx.egg-info/SOURCES.txt
--rw-r--r--   0 woods      (501) staff       (20)        1 2024-01-05 05:38:17.000000 utils_woodsx-0.0.1/src/utils_woodsx.egg-info/dependency_links.txt
--rw-r--r--   0 woods      (501) staff       (20)       13 2024-01-05 05:38:17.000000 utils_woodsx-0.0.1/src/utils_woodsx.egg-info/top_level.txt
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-10 10:10:48.449295 utils_woodsx-0.0.2/
+-rw-r--r--   0 woods      (501) staff       (20)     1065 2024-05-10 09:11:30.000000 utils_woodsx-0.0.2/LICENSE
+-rw-r--r--   0 woods      (501) staff       (20)      411 2024-05-10 10:10:48.449111 utils_woodsx-0.0.2/PKG-INFO
+-rw-r--r--   0 woods      (501) staff       (20)       49 2024-05-10 09:11:30.000000 utils_woodsx-0.0.2/README.md
+-rw-r--r--   0 woods      (501) staff       (20)      435 2024-05-10 10:10:41.000000 utils_woodsx-0.0.2/pyproject.toml
+-rw-r--r--   0 woods      (501) staff       (20)       38 2024-05-10 10:10:48.449329 utils_woodsx-0.0.2/setup.cfg
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-10 10:10:48.447920 utils_woodsx-0.0.2/src/
+-rw-r--r--   0 woods      (501) staff       (20)       76 2024-05-10 10:06:28.000000 utils_woodsx-0.0.2/src/text.py
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-10 10:10:48.448369 utils_woodsx-0.0.2/src/utils_woodsx/
+-rw-r--r--   0 woods      (501) staff       (20)        0 2024-05-10 09:11:02.000000 utils_woodsx-0.0.2/src/utils_woodsx/__init__.py
+-rw-r--r--   0 woods      (501) staff       (20)       53 2024-05-10 10:06:37.000000 utils_woodsx-0.0.2/src/utils_woodsx/example.py
+-rw-r--r--   0 woods      (501) staff       (20)     1323 2024-05-10 09:51:36.000000 utils_woodsx-0.0.2/src/utils_woodsx/excel.py
+-rw-r--r--   0 woods      (501) staff       (20)      867 2024-05-10 09:34:51.000000 utils_woodsx-0.0.2/src/utils_woodsx/html.py
+drwxr-xr-x   0 woods      (501) staff       (20)        0 2024-05-10 10:10:48.448962 utils_woodsx-0.0.2/src/utils_woodsx.egg-info/
+-rw-r--r--   0 woods      (501) staff       (20)      411 2024-05-10 10:10:48.000000 utils_woodsx-0.0.2/src/utils_woodsx.egg-info/PKG-INFO
+-rw-r--r--   0 woods      (501) staff       (20)      312 2024-05-10 10:10:48.000000 utils_woodsx-0.0.2/src/utils_woodsx.egg-info/SOURCES.txt
+-rw-r--r--   0 woods      (501) staff       (20)        1 2024-05-10 10:10:48.000000 utils_woodsx-0.0.2/src/utils_woodsx.egg-info/dependency_links.txt
+-rw-r--r--   0 woods      (501) staff       (20)       18 2024-05-10 10:10:48.000000 utils_woodsx-0.0.2/src/utils_woodsx.egg-info/top_level.txt
```

### Comparing `utils_woodsx-0.0.1/LICENSE` & `utils_woodsx-0.0.2/LICENSE`

 * *Files identical despite different names*

