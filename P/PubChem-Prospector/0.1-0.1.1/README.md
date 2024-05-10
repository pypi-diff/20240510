# Comparing `tmp/PubChem_Prospector-0.1.tar.gz` & `tmp/PubChem_Prospector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PubChem_Prospector-0.1.tar", last modified: Fri May 10 02:05:43 2024, max compression
+gzip compressed data, was "PubChem_Prospector-0.1.1.tar", last modified: Fri May 10 03:33:45 2024, max compression
```

## Comparing `PubChem_Prospector-0.1.tar` & `PubChem_Prospector-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 02:05:43.336476 PubChem_Prospector-0.1/
--rw-rw-rw-   0        0        0    35823 2024-05-10 00:27:39.000000 PubChem_Prospector-0.1/LICENSE
--rw-rw-rw-   0        0        0      554 2024-05-10 02:05:43.336476 PubChem_Prospector-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 02:05:43.314175 PubChem_Prospector-0.1/PubChem_Prospector/
--rw-rw-rw-   0        0        0        0 2024-05-09 22:24:29.000000 PubChem_Prospector-0.1/PubChem_Prospector/__init__.py
--rw-rw-rw-   0        0        0     6996 2024-05-09 22:48:45.000000 PubChem_Prospector-0.1/PubChem_Prospector/prospector.py
-drwxrwxrwx   0        0        0        0 2024-05-10 02:05:43.334481 PubChem_Prospector-0.1/PubChem_Prospector.egg-info/
--rw-rw-rw-   0        0        0      554 2024-05-10 02:05:43.000000 PubChem_Prospector-0.1/PubChem_Prospector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-05-10 02:05:43.000000 PubChem_Prospector-0.1/PubChem_Prospector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 02:05:43.000000 PubChem_Prospector-0.1/PubChem_Prospector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 02:05:43.000000 PubChem_Prospector-0.1/PubChem_Prospector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-10 02:05:43.000000 PubChem_Prospector-0.1/PubChem_Prospector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8642 2024-05-10 00:42:32.000000 PubChem_Prospector-0.1/README.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 02:05:43.336476 PubChem_Prospector-0.1/setup.cfg
--rw-rw-rw-   0        0        0      717 2024-05-10 02:02:02.000000 PubChem_Prospector-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:33:45.945913 PubChem_Prospector-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-10 00:27:39.000000 PubChem_Prospector-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      556 2024-05-10 03:33:45.944915 PubChem_Prospector-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 03:33:45.928706 PubChem_Prospector-0.1.1/PubChem_Prospector/
+-rw-rw-rw-   0        0        0        0 2024-05-09 22:24:29.000000 PubChem_Prospector-0.1.1/PubChem_Prospector/__init__.py
+-rw-rw-rw-   0        0        0     6996 2024-05-09 22:48:45.000000 PubChem_Prospector-0.1.1/PubChem_Prospector/prospector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:33:45.943951 PubChem_Prospector-0.1.1/PubChem_Prospector.egg-info/
+-rw-rw-rw-   0        0        0      556 2024-05-10 03:33:45.000000 PubChem_Prospector-0.1.1/PubChem_Prospector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-05-10 03:33:45.000000 PubChem_Prospector-0.1.1/PubChem_Prospector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:33:45.000000 PubChem_Prospector-0.1.1/PubChem_Prospector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 03:33:45.000000 PubChem_Prospector-0.1.1/PubChem_Prospector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-10 03:33:45.000000 PubChem_Prospector-0.1.1/PubChem_Prospector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8642 2024-05-10 00:42:32.000000 PubChem_Prospector-0.1.1/README.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:33:45.945913 PubChem_Prospector-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-05-10 03:10:00.000000 PubChem_Prospector-0.1.1/setup.py
```

### Comparing `PubChem_Prospector-0.1/LICENSE` & `PubChem_Prospector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PubChem_Prospector-0.1/PKG-INFO` & `PubChem_Prospector-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PubChem_Prospector
-Version: 0.1
+Version: 0.1.1
 Summary: functions for bulk scraping pubchem annotations
 Home-page: https://github.com/demontrees/PubChem_Prospector
 Author: demontrees
 Author-email: demontrees96@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `PubChem_Prospector-0.1/PubChem_Prospector/prospector.py` & `PubChem_Prospector-0.1.1/PubChem_Prospector/prospector.py`

 * *Files identical despite different names*

### Comparing `PubChem_Prospector-0.1/PubChem_Prospector.egg-info/PKG-INFO` & `PubChem_Prospector-0.1.1/PubChem_Prospector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PubChem-Prospector
-Version: 0.1
+Version: 0.1.1
 Summary: functions for bulk scraping pubchem annotations
 Home-page: https://github.com/demontrees/PubChem_Prospector
 Author: demontrees
 Author-email: demontrees96@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `PubChem_Prospector-0.1/README.txt` & `PubChem_Prospector-0.1.1/README.txt`

 * *Files identical despite different names*

### Comparing `PubChem_Prospector-0.1/setup.py` & `PubChem_Prospector-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="PubChem_Prospector",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     description="functions for bulk scraping pubchem annotations",
     author="demontrees",
     author_email="demontrees96@gmail.com",
     url="https://github.com/demontrees/PubChem_Prospector",
     install_requires=[
         'urllib3>=1.26.16'
```

