# Comparing `tmp/antibacterial-model-1.0.4.tar.gz` & `tmp/antibacterial-model-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibacterial-model-1.0.4.tar", last modified: Fri May 10 10:38:28 2024, max compression
+gzip compressed data, was "antibacterial-model-1.0.5.tar", last modified: Fri May 10 10:41:06 2024, max compression
```

## Comparing `antibacterial-model-1.0.4.tar` & `antibacterial-model-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 10:38:28.667888 antibacterial-model-1.0.4/
--rw-rw-rw-   0        0        0      773 2024-05-10 10:38:28.666888 antibacterial-model-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      104 2024-05-10 10:25:58.000000 antibacterial-model-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 10:38:28.570880 antibacterial-model-1.0.4/antibacterial_model/
--rw-rw-rw-   0        0        0       56 2024-05-10 10:12:36.000000 antibacterial-model-1.0.4/antibacterial_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:38:28.621904 antibacterial-model-1.0.4/antibacterial_model/data/
--rw-rw-rw-   0        0        0 16991105 2024-05-10 08:51:19.000000 antibacterial-model-1.0.4/antibacterial_model/data/anti-bact-data.csv
--rw-rw-rw-   0        0        0     4308 2024-05-10 10:38:18.000000 antibacterial-model-1.0.4/antibacterial_model/model.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:38:28.618883 antibacterial-model-1.0.4/antibacterial_model.egg-info/
--rw-rw-rw-   0        0        0      773 2024-05-10 10:38:27.000000 antibacterial-model-1.0.4/antibacterial_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-10 10:38:28.000000 antibacterial-model-1.0.4/antibacterial_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:38:27.000000 antibacterial-model-1.0.4/antibacterial_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-10 10:38:27.000000 antibacterial-model-1.0.4/antibacterial_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-10 10:38:27.000000 antibacterial-model-1.0.4/antibacterial_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 10:38:28.667888 antibacterial-model-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1075 2024-05-10 10:38:21.000000 antibacterial-model-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:41:06.143497 antibacterial-model-1.0.5/
+-rw-rw-rw-   0        0        0      773 2024-05-10 10:41:06.141478 antibacterial-model-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2024-05-10 10:25:58.000000 antibacterial-model-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:41:06.034601 antibacterial-model-1.0.5/antibacterial_model/
+-rw-rw-rw-   0        0        0       56 2024-05-10 10:12:36.000000 antibacterial-model-1.0.5/antibacterial_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:41:06.139479 antibacterial-model-1.0.5/antibacterial_model/data/
+-rw-rw-rw-   0        0        0 16991105 2024-05-10 08:51:19.000000 antibacterial-model-1.0.5/antibacterial_model/data/anti-bact-data.csv
+-rw-rw-rw-   0        0        0     7993 2024-04-08 15:16:20.000000 antibacterial-model-1.0.5/antibacterial_model/data/anti-bact-model.pkl
+-rw-rw-rw-   0        0        0     4308 2024-05-10 10:38:18.000000 antibacterial-model-1.0.5/antibacterial_model/model.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:41:06.081607 antibacterial-model-1.0.5/antibacterial_model.egg-info/
+-rw-rw-rw-   0        0        0      773 2024-05-10 10:41:05.000000 antibacterial-model-1.0.5/antibacterial_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2024-05-10 10:41:05.000000 antibacterial-model-1.0.5/antibacterial_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:41:05.000000 antibacterial-model-1.0.5/antibacterial_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-10 10:41:05.000000 antibacterial-model-1.0.5/antibacterial_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-10 10:41:05.000000 antibacterial-model-1.0.5/antibacterial_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:41:06.144478 antibacterial-model-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2024-05-10 10:40:53.000000 antibacterial-model-1.0.5/setup.py
```

### Comparing `antibacterial-model-1.0.4/PKG-INFO` & `antibacterial-model-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.4
+Version: 1.0.5
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `antibacterial-model-1.0.4/antibacterial_model/data/anti-bact-data.csv` & `antibacterial-model-1.0.5/antibacterial_model/data/anti-bact-data.csv`

 * *Files identical despite different names*

### Comparing `antibacterial-model-1.0.4/antibacterial_model/model.py` & `antibacterial-model-1.0.5/antibacterial_model/model.py`

 * *Files identical despite different names*

### Comparing `antibacterial-model-1.0.4/antibacterial_model.egg-info/PKG-INFO` & `antibacterial-model-1.0.5/antibacterial_model.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.4
+Version: 1.0.5
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `antibacterial-model-1.0.4/setup.py` & `antibacterial-model-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='antibacterial-model',
-    version='1.0.4',
+    version='1.0.5',
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
     long_description_content_type='text/markdown',
-    package_data={'antibacterial_model': ['data/anti-bact-data.csv', 'anti-bact-model.pkl']},
+    package_data={'antibacterial_model': ['data/anti-bact-data.csv', 'data/anti-bact-model.pkl']},
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

