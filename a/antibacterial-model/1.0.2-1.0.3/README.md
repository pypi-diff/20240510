# Comparing `tmp/antibacterial-model-1.0.2.tar.gz` & `tmp/antibacterial-model-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibacterial-model-1.0.2.tar", last modified: Fri May 10 10:12:53 2024, max compression
+gzip compressed data, was "antibacterial-model-1.0.3.tar", last modified: Fri May 10 10:27:33 2024, max compression
```

## Comparing `antibacterial-model-1.0.2.tar` & `antibacterial-model-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 10:12:53.882364 antibacterial-model-1.0.2/
--rw-rw-rw-   0        0        0      719 2024-05-10 10:12:53.881355 antibacterial-model-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       50 2024-05-10 09:37:41.000000 antibacterial-model-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 10:12:53.809410 antibacterial-model-1.0.2/antibacterial_model/
--rw-rw-rw-   0        0        0       56 2024-05-10 10:12:36.000000 antibacterial-model-1.0.2/antibacterial_model/__init__.py
--rw-rw-rw-   0        0        0     4043 2024-05-10 09:54:24.000000 antibacterial-model-1.0.2/antibacterial_model/model.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:12:53.879352 antibacterial-model-1.0.2/antibacterial_model.egg-info/
--rw-rw-rw-   0        0        0      719 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-10 10:12:53.000000 antibacterial-model-1.0.2/antibacterial_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 10:12:53.883367 antibacterial-model-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      980 2024-05-10 10:12:43.000000 antibacterial-model-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:33.259131 antibacterial-model-1.0.3/
+-rw-rw-rw-   0        0        0      773 2024-05-10 10:27:33.258134 antibacterial-model-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2024-05-10 10:25:58.000000 antibacterial-model-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:33.164125 antibacterial-model-1.0.3/antibacterial_model/
+-rw-rw-rw-   0        0        0       56 2024-05-10 10:12:36.000000 antibacterial-model-1.0.3/antibacterial_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:33.204134 antibacterial-model-1.0.3/antibacterial_model/data/
+-rw-rw-rw-   0        0        0 16991105 2024-05-10 08:51:19.000000 antibacterial-model-1.0.3/antibacterial_model/data/anti-bact-data.csv
+-rw-rw-rw-   0        0        0     4266 2024-05-10 10:24:11.000000 antibacterial-model-1.0.3/antibacterial_model/model.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:33.202141 antibacterial-model-1.0.3/antibacterial_model.egg-info/
+-rw-rw-rw-   0        0        0      773 2024-05-10 10:27:32.000000 antibacterial-model-1.0.3/antibacterial_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-10 10:27:32.000000 antibacterial-model-1.0.3/antibacterial_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:27:32.000000 antibacterial-model-1.0.3/antibacterial_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-10 10:27:32.000000 antibacterial-model-1.0.3/antibacterial_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-10 10:27:32.000000 antibacterial-model-1.0.3/antibacterial_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:27:33.260135 antibacterial-model-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2024-05-10 10:27:16.000000 antibacterial-model-1.0.3/setup.py
```

### Comparing `antibacterial-model-1.0.2/PKG-INFO` & `antibacterial-model-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.2
+Version: 1.0.3
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Anti Bacterial prediction
 ---
-This project is 
+#### A model for predicting antibacterial activity from SMILES strings
```

### Comparing `antibacterial-model-1.0.2/antibacterial_model/model.py` & `antibacterial-model-1.0.3/antibacterial_model/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import numpy as np
 from rdkit import Chem
 from rdkit.Chem import Descriptors, EState, rdMolDescriptors, Fragments, GraphDescriptors
 from sklearn.preprocessing import StandardScaler
 import joblib
 import datetime
 import pandas as pd
+import os
 
 FEATURES_SELECTED = ['EState_VSA10', 'VSA_EState6', 'BCUT2D_LOGPHI', 'fr_lactam',
        'BCUT2D_CHGLO', 'EState_VSA2', 'BalabanJ', 'BCUT2D_MRHI',
        'NumHeteroatoms', 'MaxEStateIndex', 'EState_VSA5', 'Chi3v',
        'VSA_EState4', 'MaxAbsPartialCharge', 'TPSA', 'MinEStateIndex',
        'MinPartialCharge', 'VSA_EState8', 'Chi4v', 'BCUT2D_MWHI']
 
 class AntibacterialModel:
     def __init__(self):
         # Model
-        self.model = joblib.load('anti-bact-model.pkl')
+        self.currentPath = os.path.dirname(os.path.abspath(__file__) , 'data')
+        modelPath = os.path.join(self.currentPath, 'anti-bact-model.pkl')
+        
+        self.model = joblib.load(modelPath)
         self.model.set_params(random_state=42)
         self.model.feature_names = FEATURES_SELECTED
         
         self.scaler = StandardScaler()
         self.scaler.feature_names = FEATURES_SELECTED
         self._preload_data()
     # Predict from text files which contain SMILES strings
@@ -42,15 +46,16 @@
             output_file_path = f'predictions_{timestamp}.txt'
         
         with open(output_file_path, 'w') as file:
             for smiles, pred in zip(input_smiles_list, result):
                 file.write(f'{smiles} - Prediction : {pred}\n')
 
     def _preload_data(self):
-        data = pd.read_csv("anti-bact-data.csv")
+        csvPath = os.path.join(self.currentPath, 'anti-bact-data.csv')
+        data = pd.read_csv(csvPath)
         self.scaler.fit(data[self.scaler.feature_names].values)
         
     def scale_data(self, data):
         scaled_data = self.scaler.transform(data)
         return scaled_data
     
     def map_to_label(self, predictions):
```

### Comparing `antibacterial-model-1.0.2/antibacterial_model.egg-info/PKG-INFO` & `antibacterial-model-1.0.3/antibacterial_model.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antibacterial-model
-Version: 1.0.2
+Version: 1.0.3
 Summary: A model for predicting antibacterial activity from SMILES strings
 Author: Chonthicha Arbsuwan
 Author-email: chon7599@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Anti Bacterial prediction
 ---
-This project is 
+#### A model for predicting antibacterial activity from SMILES strings
```

### Comparing `antibacterial-model-1.0.2/setup.py` & `antibacterial-model-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='antibacterial-model',
-    version='1.0.2',
+    version='1.0.3',
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
+    package_data={'antibacterial_model': ['data/anti-bact-data.csv', 'anti-bact-model.pkl']},
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

