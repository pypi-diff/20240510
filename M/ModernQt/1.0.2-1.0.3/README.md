# Comparing `tmp/modernqt-1.0.2.tar.gz` & `tmp/modernqt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernqt-1.0.2.tar", last modified: Fri May 10 11:44:27 2024, max compression
+gzip compressed data, was "modernqt-1.0.3.tar", last modified: Fri May 10 12:02:01 2024, max compression
```

## Comparing `modernqt-1.0.2.tar` & `modernqt-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:44:27.741494 modernqt-1.0.2/
--rw-r--r--   0 step      (1000) step      (1000)     1067 2024-05-02 17:11:53.000000 modernqt-1.0.2/LICENSE
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:44:27.741494 modernqt-1.0.2/ModernQt/
--rw-r--r--   0 step      (1000) step      (1000)       31 2024-05-09 08:20:56.000000 modernqt-1.0.2/ModernQt/__init__.py
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:44:27.741494 modernqt-1.0.2/ModernQt/widgets/
--rw-r--r--   0 step      (1000) step      (1000)      238 2024-05-09 06:11:10.000000 modernqt-1.0.2/ModernQt/widgets/__init__.py
-drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 11:44:27.741494 modernqt-1.0.2/ModernQt.egg-info/
--rw-r--r--   0 step      (1000) step      (1000)     1443 2024-05-10 11:44:27.000000 modernqt-1.0.2/ModernQt.egg-info/PKG-INFO
--rw-r--r--   0 step      (1000) step      (1000)      260 2024-05-10 11:44:27.000000 modernqt-1.0.2/ModernQt.egg-info/SOURCES.txt
--rw-r--r--   0 step      (1000) step      (1000)        1 2024-05-10 11:44:27.000000 modernqt-1.0.2/ModernQt.egg-info/dependency_links.txt
--rw-r--r--   0 step      (1000) step      (1000)       30 2024-05-10 11:44:27.000000 modernqt-1.0.2/ModernQt.egg-info/requires.txt
--rw-r--r--   0 step      (1000) step      (1000)        9 2024-05-10 11:44:27.000000 modernqt-1.0.2/ModernQt.egg-info/top_level.txt
--rw-r--r--   0 step      (1000) step      (1000)     1443 2024-05-10 11:44:27.741494 modernqt-1.0.2/PKG-INFO
--rw-r--r--   0 step      (1000) step      (1000)      917 2024-05-10 11:43:54.000000 modernqt-1.0.2/README.md
--rw-r--r--   0 step      (1000) step      (1000)      353 2024-05-10 11:44:21.000000 modernqt-1.0.2/pyproject.toml
--rw-r--r--   0 step      (1000) step      (1000)       38 2024-05-10 11:44:27.741494 modernqt-1.0.2/setup.cfg
--rw-r--r--   0 step      (1000) step      (1000)     1045 2024-05-10 11:44:14.000000 modernqt-1.0.2/setup.py
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 12:02:01.921219 modernqt-1.0.3/
+-rw-r--r--   0 step      (1000) step      (1000)     1067 2024-05-02 17:11:53.000000 modernqt-1.0.3/LICENSE
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 12:02:01.921219 modernqt-1.0.3/ModernQt/
+-rw-r--r--   0 step      (1000) step      (1000)       31 2024-05-09 08:20:56.000000 modernqt-1.0.3/ModernQt/__init__.py
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 12:02:01.921219 modernqt-1.0.3/ModernQt/widgets/
+-rw-r--r--   0 step      (1000) step      (1000)      238 2024-05-09 06:11:10.000000 modernqt-1.0.3/ModernQt/widgets/__init__.py
+drwxr-xr-x   0 step      (1000) step      (1000)        0 2024-05-10 12:02:01.921219 modernqt-1.0.3/ModernQt.egg-info/
+-rw-r--r--   0 step      (1000) step      (1000)     1442 2024-05-10 12:02:01.000000 modernqt-1.0.3/ModernQt.egg-info/PKG-INFO
+-rw-r--r--   0 step      (1000) step      (1000)      260 2024-05-10 12:02:01.000000 modernqt-1.0.3/ModernQt.egg-info/SOURCES.txt
+-rw-r--r--   0 step      (1000) step      (1000)        1 2024-05-10 12:02:01.000000 modernqt-1.0.3/ModernQt.egg-info/dependency_links.txt
+-rw-r--r--   0 step      (1000) step      (1000)       30 2024-05-10 12:02:01.000000 modernqt-1.0.3/ModernQt.egg-info/requires.txt
+-rw-r--r--   0 step      (1000) step      (1000)        9 2024-05-10 12:02:01.000000 modernqt-1.0.3/ModernQt.egg-info/top_level.txt
+-rw-r--r--   0 step      (1000) step      (1000)     1442 2024-05-10 12:02:01.921219 modernqt-1.0.3/PKG-INFO
+-rw-r--r--   0 step      (1000) step      (1000)      917 2024-05-10 11:43:54.000000 modernqt-1.0.3/README.md
+-rw-r--r--   0 step      (1000) step      (1000)      353 2024-05-10 11:45:58.000000 modernqt-1.0.3/pyproject.toml
+-rw-r--r--   0 step      (1000) step      (1000)       38 2024-05-10 12:02:01.921219 modernqt-1.0.3/setup.cfg
+-rw-r--r--   0 step      (1000) step      (1000)     1044 2024-05-10 12:01:53.000000 modernqt-1.0.3/setup.py
```

### Comparing `modernqt-1.0.2/LICENSE` & `modernqt-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modernqt-1.0.2/ModernQt.egg-info/PKG-INFO` & `modernqt-1.0.3/ModernQt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ModernQt
-Version: 1.0.2
+Version: 1.0.3
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt 
 Home-page: https://github.com/chebupelka8/ModernQt
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyside6>=6.7.0
 Requires-Dist: pillow>=10.3.0
 
 <p align="center">
     <img src="Logo.png">
```

### Comparing `modernqt-1.0.2/PKG-INFO` & `modernqt-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ModernQt
-Version: 1.0.2
+Version: 1.0.3
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt 
 Home-page: https://github.com/chebupelka8/ModernQt
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyside6>=6.7.0
 Requires-Dist: pillow>=10.3.0
 
 <p align="center">
     <img src="Logo.png">
```

### Comparing `modernqt-1.0.2/README.md` & `modernqt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `modernqt-1.0.2/setup.py` & `modernqt-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         data = file.read()
     
     return data
     
 
 setup(
     name='ModernQt',
-    version='1.0.2',
+    version='1.0.3',
     author='chebupelka8',
     author_email='stpzamyatin@gmail.com',
     description=DESCRIPTION,
     long_description=load_readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/chebupelka8/ModernQt',
     packages=find_packages(),
     install_requires=["pyside6>=6.7.0", "pillow>=10.3.0"],
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
-    python_requires='>=3.11'
+    python_requires='>=3.7'
 )
```

