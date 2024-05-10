# Comparing `tmp/autofracture-0.0.4.tar.gz` & `tmp/autofracture-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofracture-0.0.4.tar", last modified: Fri May 10 05:39:42 2024, max compression
+gzip compressed data, was "autofracture-0.0.5.tar", last modified: Fri May 10 05:54:18 2024, max compression
```

## Comparing `autofracture-0.0.4.tar` & `autofracture-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:39:42.585258 autofracture-0.0.4/
--rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3322 2024-05-10 05:39:42.584259 autofracture-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2225 2024-05-10 04:26:59.000000 autofracture-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 05:39:42.569257 autofracture-0.0.4/autofracture/
--rw-rw-rw-   0        0        0       20 2019-08-27 18:29:08.000000 autofracture-0.0.4/autofracture/__init__.py
--rw-rw-rw-   0        0        0      352 2024-05-10 05:39:12.000000 autofracture-0.0.4/autofracture/__version__.py
--rw-rw-rw-   0        0        0     7651 2024-05-10 05:21:28.000000 autofracture-0.0.4/autofracture/mzc.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:39:42.583257 autofracture-0.0.4/autofracture.egg-info/
--rw-rw-rw-   0        0        0     3322 2024-05-10 05:39:42.000000 autofracture-0.0.4/autofracture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-10 05:39:42.000000 autofracture-0.0.4/autofracture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:39:42.000000 autofracture-0.0.4/autofracture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-10 05:39:42.000000 autofracture-0.0.4/autofracture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-10 05:39:42.000000 autofracture-0.0.4/autofracture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 05:39:42.585258 autofracture-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     4104 2024-05-10 05:39:28.000000 autofracture-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:54:18.413439 autofracture-0.0.5/
+-rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3322 2024-05-10 05:54:18.412441 autofracture-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2225 2024-05-10 04:26:59.000000 autofracture-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 05:54:18.398401 autofracture-0.0.5/autofracture/
+-rw-rw-rw-   0        0        0       26 2024-05-10 05:49:28.000000 autofracture-0.0.5/autofracture/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-05-10 05:49:45.000000 autofracture-0.0.5/autofracture/__version__.py
+-rw-rw-rw-   0        0        0     1839 2024-05-10 05:45:37.000000 autofracture-0.0.5/autofracture/correlation.py
+-rw-rw-rw-   0        0        0     3744 2024-05-10 05:45:43.000000 autofracture-0.0.5/autofracture/evaluate.py
+-rw-rw-rw-   0        0        0     2075 2024-05-10 05:45:38.000000 autofracture-0.0.5/autofracture/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:54:18.412441 autofracture-0.0.5/autofracture.egg-info/
+-rw-rw-rw-   0        0        0     3322 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 05:54:18.413439 autofracture-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     4157 2024-05-10 05:54:00.000000 autofracture-0.0.5/setup.py
```

### Comparing `autofracture-0.0.4/LICENSE` & `autofracture-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.4/PKG-INFO` & `autofracture-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.4
+Version: 0.0.5
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `autofracture-0.0.4/README.md` & `autofracture-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.4/autofracture.egg-info/PKG-INFO` & `autofracture-0.0.5/autofracture.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.4
+Version: 0.0.5
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `autofracture-0.0.4/setup.py` & `autofracture-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'autofracture'
 DESCRIPTION = 'Support the intelligent fracturing process.'
 URL = 'https://github.com/MoonCapture/AutoFracture'
 EMAIL = 'mzc1226@126.com'
 AUTHOR = 'mzc'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 # What packages are required for this module to be executed? #执行这个模块需要什么包?
 REQUIRED = [
     'numpy', 'pandas', 'scikit-learn', 'matplotlib', 'seaborn', 'scipy','mzc','autogluon'
 ]
 
 # What packages are optional? #什么包是可选的?
@@ -41,15 +41,15 @@
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
-# Load the package's __version__.py module as a dictionary.
+# Load the package's __version__.py module as a dictionary. # 将包的__version__.py模块作为字典加载。
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
     with open(os.path.join(here, project_slug, '__version__.py')) as f:
         exec(f.read(), about)
 else:
     about['__version__'] = VERSION
```

