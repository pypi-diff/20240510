# Comparing `tmp/antibacterial-model-1.0.1.tar.gz` & `tmp/antibacterial-model-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibacterial-model-1.0.1.tar", last modified: Fri May 10 09:55:14 2024, max compression
+gzip compressed data, was "antibacterial-model-1.0.2.tar", last modified: Fri May 10 10:12:53 2024, max compression
```

## Comparing `antibacterial-model-1.0.1.tar` & `antibacterial-model-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:55:14.760492 antibacterial-model-1.0.1/
--rw-rw-rw-   0        0        0      719 2024-05-10 09:55:14.758494 antibacterial-model-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-05-10 09:37:41.000000 antibacterial-model-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 09:55:14.755504 antibacterial-model-1.0.1/antibacterial_model.egg-info/
--rw-rw-rw-   0        0        0      719 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:55:14.761497 antibacterial-model-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      980 2024-05-10 09:54:36.000000 antibacterial-model-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:12:53.882364 antibacterial-model-1.0.2/
+-rw-rw-rw-   0        0        0      719 2024-05-10 10:12:53.881355 antibacterial-model-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-05-10 09:37:41.000000 antibacterial-model-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:12:53.809410 antibacterial-model-1.0.2/antibacterial_model/
+-rw-rw-rw-   0        0        0       56 2024-05-10 10:12:36.000000 antibacterial-model-1.0.2/antibacterial_model/__init__.py
+-rw-rw-rw-   0        0        0     4043 2024-05-10 09:54:24.000000 antibacterial-model-1.0.2/antibacterial_model/model.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:12:53.879352 antibacterial-model-1.0.2/antibacterial_model.egg-info/
+-rw-rw-rw-   0        0        0      719 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:12:53.883367 antibacterial-model-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      980 2024-05-10 10:12:43.000000 antibacterial-model-1.0.2/setup.py
```

### Comparing `antibacterial-model-1.0.1/PKG-INFO` & `antibacterial-model-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.1
+Version: 1.0.2
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `antibacterial-model-1.0.1/antibacterial_model.egg-info/PKG-INFO` & `antibacterial-model-1.0.2/antibacterial_model.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.1
+Version: 1.0.2
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `antibacterial-model-1.0.1/setup.py` & `antibacterial-model-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='antibacterial-model',
-    version='1.0.1',
+    version='1.0.2',
     description='A model for predicting antibacterial activity from SMILES strings',
     author='Chonthicha Arbsuwan',
     author_email='chon7599@gmail.com',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'rdkit',
```

