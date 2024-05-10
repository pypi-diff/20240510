# Comparing `tmp/antibacterial-model-1.0.0.tar.gz` & `tmp/antibacterial-model-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibacterial-model-1.0.0.tar", last modified: Fri May 10 09:39:04 2024, max compression
+gzip compressed data, was "antibacterial-model-1.0.1.tar", last modified: Fri May 10 09:55:14 2024, max compression
```

## Comparing `antibacterial-model-1.0.0.tar` & `antibacterial-model-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:39:04.437631 antibacterial-model-1.0.0/
--rw-rw-rw-   0        0        0      719 2024-05-10 09:39:04.436655 antibacterial-model-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-05-10 09:37:41.000000 antibacterial-model-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 09:39:04.434625 antibacterial-model-1.0.0/antibacterial_model.egg-info/
--rw-rw-rw-   0        0        0      719 2024-05-10 09:39:03.000000 antibacterial-model-1.0.0/antibacterial_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-10 09:39:04.000000 antibacterial-model-1.0.0/antibacterial_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:39:03.000000 antibacterial-model-1.0.0/antibacterial_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-10 09:39:03.000000 antibacterial-model-1.0.0/antibacterial_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:39:03.000000 antibacterial-model-1.0.0/antibacterial_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:39:04.438626 antibacterial-model-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2024-05-10 09:38:49.000000 antibacterial-model-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:55:14.760492 antibacterial-model-1.0.1/
+-rw-rw-rw-   0        0        0      719 2024-05-10 09:55:14.758494 antibacterial-model-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-05-10 09:37:41.000000 antibacterial-model-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 09:55:14.755504 antibacterial-model-1.0.1/antibacterial_model.egg-info/
+-rw-rw-rw-   0        0        0      719 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:55:14.000000 antibacterial-model-1.0.1/antibacterial_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:55:14.761497 antibacterial-model-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      980 2024-05-10 09:54:36.000000 antibacterial-model-1.0.1/setup.py
```

### Comparing `antibacterial-model-1.0.0/PKG-INFO` & `antibacterial-model-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.0
+Version: 1.0.1
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `antibacterial-model-1.0.0/antibacterial_model.egg-info/PKG-INFO` & `antibacterial-model-1.0.1/antibacterial_model.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.0
+Version: 1.0.1
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `antibacterial-model-1.0.0/setup.py` & `antibacterial-model-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='antibacterial-model',
-    version='1.0.0',
+    version='1.0.1',
     description='A model for predicting antibacterial activity from SMILES strings',
     author='Chonthicha Arbsuwan',
     author_email='chon7599@gmail.com',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'rdkit',
         'scikit-learn',
         'joblib',
         'pandas',
     ],
     long_description=open('README.md').read(),
-        long_description_content_type='text/markdown',
+    long_description_content_type='text/markdown',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

