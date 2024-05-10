# Comparing `tmp/autofracture-0.0.1.tar.gz` & `tmp/autofracture-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofracture-0.0.1.tar", last modified: Fri May 10 03:27:41 2024, max compression
+gzip compressed data, was "autofracture-0.0.2.tar", last modified: Fri May 10 04:29:54 2024, max compression
```

## Comparing `autofracture-0.0.1.tar` & `autofracture-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:27:41.065858 autofracture-0.0.1/
--rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3415 2024-05-10 03:27:41.064857 autofracture-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2019-08-27 18:29:08.000000 autofracture-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 03:27:41.053854 autofracture-0.0.1/autofracture/
--rw-rw-rw-   0        0        0       20 2019-08-27 18:29:08.000000 autofracture-0.0.1/autofracture/__init__.py
--rw-rw-rw-   0        0        0      352 2024-05-10 03:19:27.000000 autofracture-0.0.1/autofracture/__version__.py
--rw-rw-rw-   0        0        0     7651 2024-05-10 03:19:44.000000 autofracture-0.0.1/autofracture/mzc.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:27:41.063862 autofracture-0.0.1/autofracture.egg-info/
--rw-rw-rw-   0        0        0     3415 2024-05-10 03:27:40.000000 autofracture-0.0.1/autofracture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-10 03:27:41.000000 autofracture-0.0.1/autofracture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:27:40.000000 autofracture-0.0.1/autofracture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-10 03:27:40.000000 autofracture-0.0.1/autofracture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-10 03:27:40.000000 autofracture-0.0.1/autofracture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 03:27:41.065858 autofracture-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4086 2024-05-10 03:22:28.000000 autofracture-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:29:54.516839 autofracture-0.0.2/
+-rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3296 2024-05-10 04:29:54.515840 autofracture-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2225 2024-05-10 04:26:59.000000 autofracture-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 04:29:54.507837 autofracture-0.0.2/autofracture/
+-rw-rw-rw-   0        0        0       20 2019-08-27 18:29:08.000000 autofracture-0.0.2/autofracture/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-05-10 03:19:27.000000 autofracture-0.0.2/autofracture/__version__.py
+-rw-rw-rw-   0        0        0     7651 2024-05-10 03:19:44.000000 autofracture-0.0.2/autofracture/mzc.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:29:54.514841 autofracture-0.0.2/autofracture.egg-info/
+-rw-rw-rw-   0        0        0     3296 2024-05-10 04:29:54.000000 autofracture-0.0.2/autofracture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-10 04:29:54.000000 autofracture-0.0.2/autofracture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 04:29:54.000000 autofracture-0.0.2/autofracture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-10 04:29:54.000000 autofracture-0.0.2/autofracture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-10 04:29:54.000000 autofracture-0.0.2/autofracture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 04:29:54.516839 autofracture-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4092 2024-05-10 04:29:26.000000 autofracture-0.0.2/setup.py
```

### Comparing `autofracture-0.0.1/LICENSE` & `autofracture-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.1/autofracture/mzc.py` & `autofracture-0.0.2/autofracture/mzc.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.1/setup.py` & `autofracture-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # Package meta-data.
 NAME = 'autofracture'
 DESCRIPTION = 'Support the intelligent fracturing process.'
 URL = 'https://github.com/MoonCapture/AutoFracture'
 EMAIL = 'mzc1226@126.com'
 AUTHOR = 'mzc'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed? #执行这个模块需要什么包?
 REQUIRED = [
-    'numpy', 'pandas', 'scikit-learn', 'matplotlib', 'seaborn', 'scipy'
+    'numpy', 'pandas', 'scikit-learn', 'matplotlib', 'seaborn', 'scipy','mzc'
 ]
 
 # What packages are optional? #什么包是可选的?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

