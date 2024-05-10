# Comparing `tmp/radical_repex-1.52.0.tar.gz` & `tmp/radical_repex-1.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical_repex-1.52.0.tar", last modified: Mon Apr 15 09:55:28 2024, max compression
+gzip compressed data, was "radical_repex-1.60.0.tar", last modified: Fri May 10 15:02:12 2024, max compression
```

## Comparing `radical_repex-1.52.0.tar` & `radical_repex-1.60.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:55:28.773216 radical_repex-1.52.0/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3055 2024-04-15 09:55:23.000000 radical_repex-1.52.0/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical_repex-1.52.0/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical_repex-1.52.0/MANIFEST.in
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 09:55:28.773216 radical_repex-1.52.0/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical_repex-1.52.0/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 09:55:20.000000 radical_repex-1.52.0/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:55:28.773216 radical_repex-1.52.0/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical_repex-1.52.0/bin/radical-repex
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical_repex-1.52.0/bin/radical-repex-version
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-04-15 09:55:28.773216 radical_repex-1.52.0/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    10251 2024-04-15 09:55:20.000000 radical_repex-1.52.0/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:55:28.773216 radical_repex-1.52.0/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:55:28.773216 radical_repex-1.52.0/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:55:28.773216 radical_repex-1.52.0/src/radical/repex/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       28 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical/repex/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical/repex/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical_repex-1.52.0/src/radical/repex/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical_repex-1.52.0/src/radical/repex/algorithms.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical_repex-1.52.0/src/radical/repex/exchange.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical_repex-1.52.0/src/radical/repex/replica.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical_repex-1.52.0/src/radical/repex/utils.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:55:28.773216 radical_repex-1.52.0/src/radical.repex.egg-info/
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical.repex.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      556 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical.repex.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical.repex.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical.repex.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       39 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical.repex.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-04-15 09:55:28.000000 radical_repex-1.52.0/src/radical.repex.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 15:02:12.499640 radical_repex-1.60.0/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     3057 2024-05-10 15:02:01.000000 radical_repex-1.60.0/CHANGES.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical_repex-1.60.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical_repex-1.60.0/MANIFEST.in
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     3073 2024-05-10 15:02:12.499640 radical_repex-1.60.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical_repex-1.60.0/README.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-05-10 15:01:42.000000 radical_repex-1.60.0/VERSION
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 15:02:12.495640 radical_repex-1.60.0/bin/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical_repex-1.60.0/bin/radical-repex
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical_repex-1.60.0/bin/radical-repex-version
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       88 2024-05-10 15:01:37.000000 radical_repex-1.60.0/pyproject.toml
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-05-10 15:02:12.499640 radical_repex-1.60.0/setup.cfg
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     6941 2024-05-10 15:01:37.000000 radical_repex-1.60.0/setup.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 15:02:12.495640 radical_repex-1.60.0/src/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 15:02:12.495640 radical_repex-1.60.0/src/radical/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 15:02:12.499640 radical_repex-1.60.0/src/radical/repex/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       51 2024-05-10 15:02:12.000000 radical_repex-1.60.0/src/radical/repex/VERSION
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical_repex-1.60.0/src/radical/repex/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical_repex-1.60.0/src/radical/repex/algorithms.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical_repex-1.60.0/src/radical/repex/exchange.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical_repex-1.60.0/src/radical/repex/replica.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical_repex-1.60.0/src/radical/repex/utils.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 15:02:12.499640 radical_repex-1.60.0/src/radical.repex.egg-info/
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     3073 2024-05-10 15:02:12.000000 radical_repex-1.60.0/src/radical.repex.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      547 2024-05-10 15:02:12.000000 radical_repex-1.60.0/src/radical.repex.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-05-10 15:02:12.000000 radical_repex-1.60.0/src/radical.repex.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-05-10 15:02:12.000000 radical_repex-1.60.0/src/radical.repex.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       19 2024-05-10 15:02:12.000000 radical_repex-1.60.0/src/radical.repex.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-05-10 15:02:12.000000 radical_repex-1.60.0/src/radical.repex.egg-info/top_level.txt
```

### Comparing `radical_repex-1.52.0/LICENSE.md` & `radical_repex-1.60.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/README.md` & `radical_repex-1.60.0/README.md`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/bin/radical-repex` & `radical_repex-1.60.0/bin/radical-repex`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/src/radical/repex/__init__.py` & `radical_repex-1.60.0/src/radical/repex/__init__.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/src/radical/repex/algorithms.py` & `radical_repex-1.60.0/src/radical/repex/algorithms.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/src/radical/repex/exchange.py` & `radical_repex-1.60.0/src/radical/repex/exchange.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/src/radical/repex/replica.py` & `radical_repex-1.60.0/src/radical/repex/replica.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/src/radical/repex/utils.py` & `radical_repex-1.60.0/src/radical/repex/utils.py`

 * *Files identical despite different names*

### Comparing `radical_repex-1.52.0/src/radical.repex.egg-info/SOURCES.txt` & `radical_repex-1.60.0/src/radical.repex.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 CHANGES.md
 LICENSE.md
 MANIFEST.in
 README.md
 VERSION
+pyproject.toml
 setup.cfg
 setup.py
 bin/radical-repex
 bin/radical-repex-version
 src/radical.repex.egg-info/PKG-INFO
 src/radical.repex.egg-info/SOURCES.txt
 src/radical.repex.egg-info/dependency_links.txt
 src/radical.repex.egg-info/not-zip-safe
 src/radical.repex.egg-info/requires.txt
 src/radical.repex.egg-info/top_level.txt
-src/radical/repex/SDIST
 src/radical/repex/VERSION
 src/radical/repex/__init__.py
 src/radical/repex/algorithms.py
 src/radical/repex/exchange.py
 src/radical/repex/replica.py
 src/radical/repex/utils.py
```

