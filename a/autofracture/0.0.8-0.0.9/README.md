# Comparing `tmp/autofracture-0.0.8.tar.gz` & `tmp/autofracture-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofracture-0.0.8.tar", last modified: Fri May 10 09:13:48 2024, max compression
+gzip compressed data, was "autofracture-0.0.9.tar", last modified: Fri May 10 09:35:24 2024, max compression
```

## Comparing `autofracture-0.0.8.tar` & `autofracture-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:13:48.233774 autofracture-0.0.8/
--rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3585 2024-05-10 09:13:48.232774 autofracture-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2323 2024-05-10 09:08:14.000000 autofracture-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 09:13:48.219783 autofracture-0.0.8/autofracture/
--rw-rw-rw-   0        0        0       26 2024-05-10 05:49:28.000000 autofracture-0.0.8/autofracture/__init__.py
--rw-rw-rw-   0        0        0     1839 2024-05-10 05:45:37.000000 autofracture-0.0.8/autofracture/correlation.py
--rw-rw-rw-   0        0        0     3744 2024-05-10 05:45:43.000000 autofracture-0.0.8/autofracture/evaluate.py
--rw-rw-rw-   0        0        0     2075 2024-05-10 05:45:38.000000 autofracture-0.0.8/autofracture/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-10 09:13:48.231783 autofracture-0.0.8/autofracture.egg-info/
--rw-rw-rw-   0        0        0     3585 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:13:48.233774 autofracture-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2379 2024-05-10 09:13:35.000000 autofracture-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:35:24.439564 autofracture-0.0.9/
+-rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3585 2024-05-10 09:35:24.438563 autofracture-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2323 2024-05-10 09:08:14.000000 autofracture-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 09:35:24.414563 autofracture-0.0.9/autofracture/
+-rw-rw-rw-   0        0        0       26 2024-05-10 05:49:28.000000 autofracture-0.0.9/autofracture/__init__.py
+-rw-rw-rw-   0        0        0     1839 2024-05-10 05:45:37.000000 autofracture-0.0.9/autofracture/correlation.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:35:24.437565 autofracture-0.0.9/autofracture/design/
+-rw-rw-rw-   0        0        0      115 2024-05-10 09:31:10.000000 autofracture-0.0.9/autofracture/design/__init__.py
+-rw-rw-rw-   0        0        0     5401 2024-04-25 05:41:09.000000 autofracture-0.0.9/autofracture/design/datapreprocess.py
+-rw-rw-rw-   0        0        0     3858 2024-04-25 06:53:12.000000 autofracture-0.0.9/autofracture/design/main.py
+-rw-rw-rw-   0        0        0     1797 2024-04-25 05:47:16.000000 autofracture-0.0.9/autofracture/design/opt.py
+-rw-rw-rw-   0        0        0     5214 2024-04-25 05:45:34.000000 autofracture-0.0.9/autofracture/design/production.py
+-rw-rw-rw-   0        0        0     3744 2024-05-10 05:45:43.000000 autofracture-0.0.9/autofracture/evaluate.py
+-rw-rw-rw-   0        0        0     2075 2024-05-10 05:45:38.000000 autofracture-0.0.9/autofracture/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:35:24.438563 autofracture-0.0.9/autofracture.egg-info/
+-rw-rw-rw-   0        0        0     3585 2024-05-10 09:35:24.000000 autofracture-0.0.9/autofracture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2024-05-10 09:35:24.000000 autofracture-0.0.9/autofracture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:35:24.000000 autofracture-0.0.9/autofracture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-10 09:35:24.000000 autofracture-0.0.9/autofracture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-10 09:35:24.000000 autofracture-0.0.9/autofracture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:35:24.439564 autofracture-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2379 2024-05-10 09:31:43.000000 autofracture-0.0.9/setup.py
```

### Comparing `autofracture-0.0.8/LICENSE` & `autofracture-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.8/PKG-INFO` & `autofracture-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.8
+Version: 0.0.9
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `autofracture-0.0.8/README.md` & `autofracture-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.8/autofracture/correlation.py` & `autofracture-0.0.9/autofracture/correlation.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.8/autofracture/evaluate.py` & `autofracture-0.0.9/autofracture/evaluate.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.8/autofracture/plot.py` & `autofracture-0.0.9/autofracture/plot.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.8/autofracture.egg-info/PKG-INFO` & `autofracture-0.0.9/autofracture.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.8
+Version: 0.0.9
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `autofracture-0.0.8/setup.py` & `autofracture-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   
 NAME = 'autofracture'
 DESCRIPTION = 'Support the intelligent fracturing process.'
 URL = 'https://github.com/MoonCapture/AutoFracture'
 EMAIL = 'mzc1226@126.com'
 AUTHOR = 'mzc'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed? # 执行这个模块需要什么包?
 REQUIRED = [
     'numpy', 'pandas', 'scikit-learn', 'matplotlib', 'seaborn', 'scipy','autogluon'
 ]
 # What packages are optional? # 什么包是可选的?
 EXTRAS = {
```

