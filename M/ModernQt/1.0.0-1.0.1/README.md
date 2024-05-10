# Comparing `tmp/modernqt-1.0.0.tar.gz` & `tmp/modernqt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernqt-1.0.0.tar", last modified: Fri May 10 11:30:33 2024, max compression
+gzip compressed data, was "modernqt-1.0.1.tar", last modified: Fri May 10 11:41:22 2024, max compression
```

## Comparing `modernqt-1.0.0.tar` & `modernqt-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:30:33.749864 modernqt-1.0.0/
--rw-r--r--   0 step      (1000) step      (1000)     1067 2024-05-02 17:11:53.000000 modernqt-1.0.0/LICENSE
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:30:33.749864 modernqt-1.0.0/ModernQt/
--rw-r--r--   0 step      (1000) step      (1000)       31 2024-05-09 08:20:56.000000 modernqt-1.0.0/ModernQt/__init__.py
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:30:33.749864 modernqt-1.0.0/ModernQt/widgets/
--rw-r--r--   0 step      (1000) step      (1000)      238 2024-05-09 06:11:10.000000 modernqt-1.0.0/ModernQt/widgets/__init__.py
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:30:33.749864 modernqt-1.0.0/ModernQt.egg-info/
--rw-r--r--   0 step      (1000) step      (1000)     1462 2024-05-10 11:30:33.000000 modernqt-1.0.0/ModernQt.egg-info/PKG-INFO
--rw-r--r--   0 step      (1000) step      (1000)      260 2024-05-10 11:30:33.000000 modernqt-1.0.0/ModernQt.egg-info/SOURCES.txt
--rw-r--r--   0 step      (1000) step      (1000)        1 2024-05-10 11:30:33.000000 modernqt-1.0.0/ModernQt.egg-info/dependency_links.txt
--rw-r--r--   0 step      (1000) step      (1000)       30 2024-05-10 11:30:33.000000 modernqt-1.0.0/ModernQt.egg-info/requires.txt
--rw-r--r--   0 step      (1000) step      (1000)        9 2024-05-10 11:30:33.000000 modernqt-1.0.0/ModernQt.egg-info/top_level.txt
--rw-r--r--   0 step      (1000) step      (1000)     1462 2024-05-10 11:30:33.749864 modernqt-1.0.0/PKG-INFO
--rw-r--r--   0 step      (1000) step      (1000)      936 2024-05-05 15:43:55.000000 modernqt-1.0.0/README.md
--rw-r--r--   0 step      (1000) step      (1000)      353 2024-05-10 11:17:30.000000 modernqt-1.0.0/pyproject.toml
--rw-r--r--   0 step      (1000) step      (1000)       38 2024-05-10 11:30:33.749864 modernqt-1.0.0/setup.cfg
--rw-r--r--   0 step      (1000) step      (1000)     1045 2024-05-10 11:30:03.000000 modernqt-1.0.0/setup.py
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:41:22.250044 modernqt-1.0.1/
+-rw-r--r--   0 step      (1000) step      (1000)     1067 2024-05-02 17:11:53.000000 modernqt-1.0.1/LICENSE
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:41:22.246711 modernqt-1.0.1/ModernQt/
+-rw-r--r--   0 step      (1000) step      (1000)       31 2024-05-09 08:20:56.000000 modernqt-1.0.1/ModernQt/__init__.py
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:41:22.246711 modernqt-1.0.1/ModernQt/widgets/
+-rw-r--r--   0 step      (1000) step      (1000)      238 2024-05-09 06:11:10.000000 modernqt-1.0.1/ModernQt/widgets/__init__.py
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:41:22.250044 modernqt-1.0.1/ModernQt.egg-info/
+-rw-r--r--   0 step      (1000) step      (1000)     1433 2024-05-10 11:41:22.000000 modernqt-1.0.1/ModernQt.egg-info/PKG-INFO
+-rw-r--r--   0 step      (1000) step      (1000)      260 2024-05-10 11:41:22.000000 modernqt-1.0.1/ModernQt.egg-info/SOURCES.txt
+-rw-r--r--   0 step      (1000) step      (1000)        1 2024-05-10 11:41:22.000000 modernqt-1.0.1/ModernQt.egg-info/dependency_links.txt
+-rw-r--r--   0 step      (1000) step      (1000)       30 2024-05-10 11:41:22.000000 modernqt-1.0.1/ModernQt.egg-info/requires.txt
+-rw-r--r--   0 step      (1000) step      (1000)        9 2024-05-10 11:41:22.000000 modernqt-1.0.1/ModernQt.egg-info/top_level.txt
+-rw-r--r--   0 step      (1000) step      (1000)     1433 2024-05-10 11:41:22.250044 modernqt-1.0.1/PKG-INFO
+-rw-r--r--   0 step      (1000) step      (1000)      907 2024-05-10 11:37:18.000000 modernqt-1.0.1/README.md
+-rw-r--r--   0 step      (1000) step      (1000)      353 2024-05-10 11:40:33.000000 modernqt-1.0.1/pyproject.toml
+-rw-r--r--   0 step      (1000) step      (1000)       38 2024-05-10 11:41:22.250044 modernqt-1.0.1/setup.cfg
+-rw-r--r--   0 step      (1000) step      (1000)     1045 2024-05-10 11:40:24.000000 modernqt-1.0.1/setup.py
```

### Comparing `modernqt-1.0.0/LICENSE` & `modernqt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modernqt-1.0.0/ModernQt.egg-info/PKG-INFO` & `modernqt-1.0.1/ModernQt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModernQt
-Version: 1.0.0
+Version: 1.0.1
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt 
 Home-page: https://github.com/chebupelka8/ModernQt
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 </p>
 
 <b>ModernQt</b>: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 
 <h3>How to use</h3>
 
 ```sh
-git clone https://github.com/chebupelka8/ModernQt
+pip install ModernQt
 ```
 
 ```python
 from ModernQt.widgets import PushButton
 ...
 ```
```

### Comparing `modernqt-1.0.0/PKG-INFO` & `modernqt-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModernQt
-Version: 1.0.0
+Version: 1.0.1
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt 
 Home-page: https://github.com/chebupelka8/ModernQt
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 </p>
 
 <b>ModernQt</b>: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 
 <h3>How to use</h3>
 
 ```sh
-git clone https://github.com/chebupelka8/ModernQt
+pip install ModernQt
 ```
 
 ```python
 from ModernQt.widgets import PushButton
 ...
 ```
```

### Comparing `modernqt-1.0.0/README.md` & `modernqt-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 </p>
 
 <b>ModernQt</b>: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 
 <h3>How to use</h3>
 
 ```sh
-git clone https://github.com/chebupelka8/ModernQt
+pip install ModernQt
 ```
 
 ```python
 from ModernQt.widgets import PushButton
 ...
 ```
```

### Comparing `modernqt-1.0.0/setup.py` & `modernqt-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         data = file.read()
     
     return data
     
 
 setup(
     name='ModernQt',
-    version='1.0.0',
+    version='1.0.1',
     author='chebupelka8',
     author_email='stpzamyatin@gmail.com',
     description=DESCRIPTION,
     long_description=load_readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/chebupelka8/ModernQt',
     packages=find_packages(),
```

