# Comparing `tmp/dsplus-0.4.9.tar.gz` & `tmp/dsplus-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.4.9.tar", last modified: Tue May  7 13:08:16 2024, max compression
+gzip compressed data, was "dsplus-0.5.1.tar", last modified: Fri May 10 00:16:47 2024, max compression
```

## Comparing `dsplus-0.4.9.tar` & `dsplus-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:08:16.493100 dsplus-0.4.9/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.9/LICENSE
--rw-rw-rw-   0        0        0      690 2024-05-07 13:08:16.489566 dsplus-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:08:16.470854 dsplus-0.4.9/dsplus/
--rw-rw-rw-   0        0        0      171 2024-05-07 13:08:01.000000 dsplus-0.4.9/dsplus/__init__.py
--rw-rw-rw-   0        0        0    25485 2024-05-07 12:38:31.000000 dsplus-0.4.9/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    43727 2024-05-07 13:06:53.000000 dsplus-0.4.9/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    57143 2024-05-06 23:46:36.000000 dsplus-0.4.9/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    59122 2024-05-06 04:39:55.000000 dsplus-0.4.9/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:08:16.483968 dsplus-0.4.9/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-05-07 13:08:16.000000 dsplus-0.4.9/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-07 13:08:16.000000 dsplus-0.4.9/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:08:16.000000 dsplus-0.4.9/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 13:08:16.000000 dsplus-0.4.9/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:08:16.493100 dsplus-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:08:16.485270 dsplus-0.4.9/tests/
--rw-rw-rw-   0        0        0    13083 2024-05-07 12:46:09.000000 dsplus-0.4.9/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.527594 dsplus-0.5.1/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      895 2024-05-10 00:16:47.522133 dsplus-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-10 00:15:58.000000 dsplus-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.479007 dsplus-0.5.1/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-05-10 00:14:12.000000 dsplus-0.5.1/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    25485 2024-05-07 12:38:31.000000 dsplus-0.5.1/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    43727 2024-05-07 13:06:53.000000 dsplus-0.5.1/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    57143 2024-05-08 02:06:30.000000 dsplus-0.5.1/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    59122 2024-05-06 04:39:55.000000 dsplus-0.5.1/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.506667 dsplus-0.5.1/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      895 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 00:16:47.529039 dsplus-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      982 2024-05-10 00:11:27.000000 dsplus-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.511347 dsplus-0.5.1/tests/
+-rw-rw-rw-   0        0        0    13083 2024-05-07 12:46:09.000000 dsplus-0.5.1/tests/Test_pandas.py
```

### Comparing `dsplus-0.4.9/LICENSE` & `dsplus-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.9/PKG-INFO` & `dsplus-0.5.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.9
+Version: 0.5.1
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Helper functions and classes for data science tasks
+This package contains helper functions and classes for various data science tasks.
+
+This package is still in the beta stage. Please expect frequent updates to fix bugs and add functionalities. A full documentation will be added soon.
 
 # Installation
 
 ```bash
 pip install dsplus
 ```
```

### Comparing `dsplus-0.4.9/dsplus/pb_functions_general.py` & `dsplus-0.5.1/dsplus/pb_functions_general.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.9/dsplus/pb_functions_pandas.py` & `dsplus-0.5.1/dsplus/pb_functions_pandas.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.9/dsplus/pb_functions_plotly.py` & `dsplus-0.5.1/dsplus/pb_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.9/dsplus/pb_functions_spatial.py` & `dsplus-0.5.1/dsplus/pb_functions_spatial.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.9/dsplus.egg-info/PKG-INFO` & `dsplus-0.5.1/dsplus.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.9
+Version: 0.5.1
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Helper functions and classes for data science tasks
+This package contains helper functions and classes for various data science tasks.
+
+This package is still in the beta stage. Please expect frequent updates to fix bugs and add functionalities. A full documentation will be added soon.
 
 # Installation
 
 ```bash
 pip install dsplus
 ```
```

### Comparing `dsplus-0.4.9/tests/Test_pandas.py` & `dsplus-0.5.1/tests/Test_pandas.py`

 * *Files identical despite different names*

