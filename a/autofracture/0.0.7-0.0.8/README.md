# Comparing `tmp/autofracture-0.0.7.tar.gz` & `tmp/autofracture-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofracture-0.0.7.tar", last modified: Fri May 10 07:23:42 2024, max compression
+gzip compressed data, was "autofracture-0.0.8.tar", last modified: Fri May 10 09:13:48 2024, max compression
```

## Comparing `autofracture-0.0.7.tar` & `autofracture-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 07:23:42.113970 autofracture-0.0.7/
--rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3400 2024-05-10 07:23:42.112971 autofracture-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2319 2024-05-10 07:12:25.000000 autofracture-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 07:23:42.098971 autofracture-0.0.7/autofracture/
--rw-rw-rw-   0        0        0       26 2024-05-10 05:49:28.000000 autofracture-0.0.7/autofracture/__init__.py
--rw-rw-rw-   0        0        0     1839 2024-05-10 05:45:37.000000 autofracture-0.0.7/autofracture/correlation.py
--rw-rw-rw-   0        0        0     3744 2024-05-10 05:45:43.000000 autofracture-0.0.7/autofracture/evaluate.py
--rw-rw-rw-   0        0        0     2075 2024-05-10 05:45:38.000000 autofracture-0.0.7/autofracture/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:23:42.111971 autofracture-0.0.7/autofracture.egg-info/
--rw-rw-rw-   0        0        0     3400 2024-05-10 07:23:42.000000 autofracture-0.0.7/autofracture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-05-10 07:23:42.000000 autofracture-0.0.7/autofracture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 07:23:42.000000 autofracture-0.0.7/autofracture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-10 07:23:42.000000 autofracture-0.0.7/autofracture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-10 07:23:42.000000 autofracture-0.0.7/autofracture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 07:23:42.113970 autofracture-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     4138 2024-05-10 07:23:12.000000 autofracture-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:13:48.233774 autofracture-0.0.8/
+-rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3585 2024-05-10 09:13:48.232774 autofracture-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2323 2024-05-10 09:08:14.000000 autofracture-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 09:13:48.219783 autofracture-0.0.8/autofracture/
+-rw-rw-rw-   0        0        0       26 2024-05-10 05:49:28.000000 autofracture-0.0.8/autofracture/__init__.py
+-rw-rw-rw-   0        0        0     1839 2024-05-10 05:45:37.000000 autofracture-0.0.8/autofracture/correlation.py
+-rw-rw-rw-   0        0        0     3744 2024-05-10 05:45:43.000000 autofracture-0.0.8/autofracture/evaluate.py
+-rw-rw-rw-   0        0        0     2075 2024-05-10 05:45:38.000000 autofracture-0.0.8/autofracture/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:13:48.231783 autofracture-0.0.8/autofracture.egg-info/
+-rw-rw-rw-   0        0        0     3585 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-10 09:13:48.000000 autofracture-0.0.8/autofracture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:13:48.233774 autofracture-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2379 2024-05-10 09:13:35.000000 autofracture-0.0.8/setup.py
```

### Comparing `autofracture-0.0.7/LICENSE` & `autofracture-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.7/PKG-INFO` & `autofracture-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.7
+Version: 0.0.8
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
-License: MIT
+License: MIT License
+Platform: all
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
@@ -65,9 +70,10 @@
 License
 -------
 
 MIT License
 
 ## Updata log
 
-* `'0.0.1'-'0.0.6`      test release
+* 
+* `'0.0.1'-'0.0.8'`      test release
 * `'0.0.1'`                 first release
```

### Comparing `autofracture-0.0.7/README.md` & `autofracture-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,9 +35,10 @@
 License
 -------
 
 MIT License
 
 ## Updata log
 
-* `'0.0.1'-'0.0.6`      test release
+* 
+* `'0.0.1'-'0.0.8'`      test release
 * `'0.0.1'`                 first release
```

### Comparing `autofracture-0.0.7/autofracture/correlation.py` & `autofracture-0.0.8/autofracture/correlation.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.7/autofracture/evaluate.py` & `autofracture-0.0.8/autofracture/evaluate.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.7/autofracture/plot.py` & `autofracture-0.0.8/autofracture/plot.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.7/autofracture.egg-info/PKG-INFO` & `autofracture-0.0.8/autofracture.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.7
+Version: 0.0.8
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
-License: MIT
+License: MIT License
+Platform: all
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
@@ -65,9 +70,10 @@
 License
 -------
 
 MIT License
 
 ## Updata log
 
-* `'0.0.1'-'0.0.6`      test release
+* 
+* `'0.0.1'-'0.0.8'`      test release
 * `'0.0.1'`                 first release
```

