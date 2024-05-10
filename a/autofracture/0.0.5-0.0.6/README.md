# Comparing `tmp/autofracture-0.0.5.tar.gz` & `tmp/autofracture-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofracture-0.0.5.tar", last modified: Fri May 10 05:54:18 2024, max compression
+gzip compressed data, was "autofracture-0.0.6.tar", last modified: Fri May 10 07:12:54 2024, max compression
```

## Comparing `autofracture-0.0.5.tar` & `autofracture-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:54:18.413439 autofracture-0.0.5/
--rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3322 2024-05-10 05:54:18.412441 autofracture-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2225 2024-05-10 04:26:59.000000 autofracture-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 05:54:18.398401 autofracture-0.0.5/autofracture/
--rw-rw-rw-   0        0        0       26 2024-05-10 05:49:28.000000 autofracture-0.0.5/autofracture/__init__.py
--rw-rw-rw-   0        0        0      352 2024-05-10 05:49:45.000000 autofracture-0.0.5/autofracture/__version__.py
--rw-rw-rw-   0        0        0     1839 2024-05-10 05:45:37.000000 autofracture-0.0.5/autofracture/correlation.py
--rw-rw-rw-   0        0        0     3744 2024-05-10 05:45:43.000000 autofracture-0.0.5/autofracture/evaluate.py
--rw-rw-rw-   0        0        0     2075 2024-05-10 05:45:38.000000 autofracture-0.0.5/autofracture/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:54:18.412441 autofracture-0.0.5/autofracture.egg-info/
--rw-rw-rw-   0        0        0     3322 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-10 05:54:18.000000 autofracture-0.0.5/autofracture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 05:54:18.413439 autofracture-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     4157 2024-05-10 05:54:00.000000 autofracture-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:12:54.579949 autofracture-0.0.6/
+-rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 autofracture-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 autofracture-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3420 2024-05-10 07:12:54.578946 autofracture-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2319 2024-05-10 07:12:25.000000 autofracture-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 07:12:54.560425 autofracture-0.0.6/autofracture/
+-rw-rw-rw-   0        0        0       26 2024-05-10 05:49:28.000000 autofracture-0.0.6/autofracture/__init__.py
+-rw-rw-rw-   0        0        0     1839 2024-05-10 05:45:37.000000 autofracture-0.0.6/autofracture/correlation.py
+-rw-rw-rw-   0        0        0     3744 2024-05-10 05:45:43.000000 autofracture-0.0.6/autofracture/evaluate.py
+-rw-rw-rw-   0        0        0     2075 2024-05-10 05:45:38.000000 autofracture-0.0.6/autofracture/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:12:54.577946 autofracture-0.0.6/autofracture.egg-info/
+-rw-rw-rw-   0        0        0     3420 2024-05-10 07:12:54.000000 autofracture-0.0.6/autofracture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-05-10 07:12:54.000000 autofracture-0.0.6/autofracture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 07:12:54.000000 autofracture-0.0.6/autofracture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-10 07:12:54.000000 autofracture-0.0.6/autofracture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-10 07:12:54.000000 autofracture-0.0.6/autofracture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 07:12:54.579949 autofracture-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     4144 2024-05-10 07:12:29.000000 autofracture-0.0.6/setup.py
```

### Comparing `autofracture-0.0.5/LICENSE` & `autofracture-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.5/PKG-INFO` & `autofracture-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.5
+Version: 0.0.6
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -28,15 +28,14 @@
 Requires-Dist: mzc
 Requires-Dist: autogluon
 
 
 📦 AutoFracture
 ===============
 
-
 In the field of hydraulic fracturing, automatic machine learning can help in handling and analyzing large amounts of data, improving the accuracy of predicting hydraulic fracturing results, and optimizing operational parameters. Here are some aspects where automatic machine learning can play a role in the field of hydraulic fracturing:
 
 1. Data analysis and feature engineering: Automatic machine learning algorithms can assist in analyzing various data generated during the hydraulic fracturing process, such as geological, seismic, fluid mechanics data, automatically generating features, and reducing data dimensions.
 2. Predicting hydraulic fracturing outcomes: Using machine learning algorithms, it is possible to predict the outcomes of hydraulic fracturing, including parameters such as rock fracturing patterns, porosity, etc., helping engineers make more accurate decisions.
 3. Optimizing parameter configurations: Through automated machine learning algorithms, it is possible to optimize the configuration of hydraulic fracturing parameters, such as the ratio of fracturing fluid, injection speed, injection volume, etc., to achieve more efficient and cost-effective hydraulic fracturing operations.
 4. Real-time monitoring and adjustments: By combining sensors and automated machine learning algorithms, it is possible to monitor changes in parameters during the hydraulic fracturing process in real-time, and make timely adjustments to prevent unforeseen incidents, improving efficiency and safety of hydraulic fracturing.
 
@@ -64,7 +63,12 @@
 - [The Hitchhiker's Guide to Packaging]
 - [Cookiecutter template for a Python package]
 
 License
 -------
 
 MIT License
+
+## Updata log
+
+* `'0.0.1'-'0.0.6`      test release
+* `'0.0.1'`                 first release
```

### Comparing `autofracture-0.0.5/README.md` & `autofracture-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 📦 AutoFracture
 ===============
 
-
 In the field of hydraulic fracturing, automatic machine learning can help in handling and analyzing large amounts of data, improving the accuracy of predicting hydraulic fracturing results, and optimizing operational parameters. Here are some aspects where automatic machine learning can play a role in the field of hydraulic fracturing:
 
 1. Data analysis and feature engineering: Automatic machine learning algorithms can assist in analyzing various data generated during the hydraulic fracturing process, such as geological, seismic, fluid mechanics data, automatically generating features, and reducing data dimensions.
 2. Predicting hydraulic fracturing outcomes: Using machine learning algorithms, it is possible to predict the outcomes of hydraulic fracturing, including parameters such as rock fracturing patterns, porosity, etc., helping engineers make more accurate decisions.
 3. Optimizing parameter configurations: Through automated machine learning algorithms, it is possible to optimize the configuration of hydraulic fracturing parameters, such as the ratio of fracturing fluid, injection speed, injection volume, etc., to achieve more efficient and cost-effective hydraulic fracturing operations.
 4. Real-time monitoring and adjustments: By combining sensors and automated machine learning algorithms, it is possible to monitor changes in parameters during the hydraulic fracturing process in real-time, and make timely adjustments to prevent unforeseen incidents, improving efficiency and safety of hydraulic fracturing.
 
@@ -33,7 +32,12 @@
 - [The Hitchhiker's Guide to Packaging]
 - [Cookiecutter template for a Python package]
 
 License
 -------
 
 MIT License
+
+## Updata log
+
+* `'0.0.1'-'0.0.6`      test release
+* `'0.0.1'`                 first release
```

### Comparing `autofracture-0.0.5/autofracture/correlation.py` & `autofracture-0.0.6/autofracture/correlation.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.5/autofracture/evaluate.py` & `autofracture-0.0.6/autofracture/evaluate.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.5/autofracture/plot.py` & `autofracture-0.0.6/autofracture/plot.py`

 * *Files identical despite different names*

### Comparing `autofracture-0.0.5/autofracture.egg-info/PKG-INFO` & `autofracture-0.0.6/autofracture.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofracture
-Version: 0.0.5
+Version: 0.0.6
 Summary: Support the intelligent fracturing process.
 Home-page: https://github.com/MoonCapture/AutoFracture
 Author: mzc
 Author-email: mzc1226@126.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -28,15 +28,14 @@
 Requires-Dist: mzc
 Requires-Dist: autogluon
 
 
 📦 AutoFracture
 ===============
 
-
 In the field of hydraulic fracturing, automatic machine learning can help in handling and analyzing large amounts of data, improving the accuracy of predicting hydraulic fracturing results, and optimizing operational parameters. Here are some aspects where automatic machine learning can play a role in the field of hydraulic fracturing:
 
 1. Data analysis and feature engineering: Automatic machine learning algorithms can assist in analyzing various data generated during the hydraulic fracturing process, such as geological, seismic, fluid mechanics data, automatically generating features, and reducing data dimensions.
 2. Predicting hydraulic fracturing outcomes: Using machine learning algorithms, it is possible to predict the outcomes of hydraulic fracturing, including parameters such as rock fracturing patterns, porosity, etc., helping engineers make more accurate decisions.
 3. Optimizing parameter configurations: Through automated machine learning algorithms, it is possible to optimize the configuration of hydraulic fracturing parameters, such as the ratio of fracturing fluid, injection speed, injection volume, etc., to achieve more efficient and cost-effective hydraulic fracturing operations.
 4. Real-time monitoring and adjustments: By combining sensors and automated machine learning algorithms, it is possible to monitor changes in parameters during the hydraulic fracturing process in real-time, and make timely adjustments to prevent unforeseen incidents, improving efficiency and safety of hydraulic fracturing.
 
@@ -64,7 +63,12 @@
 - [The Hitchhiker's Guide to Packaging]
 - [Cookiecutter template for a Python package]
 
 License
 -------
 
 MIT License
+
+## Updata log
+
+* `'0.0.1'-'0.0.6`      test release
+* `'0.0.1'`                 first release
```

### Comparing `autofracture-0.0.5/setup.py` & `autofracture-0.0.6/setup.py`

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
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 # What packages are required for this module to be executed? #执行这个模块需要什么包?
 REQUIRED = [
     'numpy', 'pandas', 'scikit-learn', 'matplotlib', 'seaborn', 'scipy','mzc','autogluon'
 ]
 
 # What packages are optional? #什么包是可选的?
@@ -91,15 +91,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

