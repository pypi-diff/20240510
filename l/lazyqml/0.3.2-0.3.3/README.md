# Comparing `tmp/lazyqml-0.3.2.tar.gz` & `tmp/lazyqml-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.3.2.tar", last modified: Thu May  9 11:57:42 2024, max compression
+gzip compressed data, was "lazyqml-0.3.3.tar", last modified: Fri May 10 08:01:03 2024, max compression
```

## Comparing `lazyqml-0.3.2.tar` & `lazyqml-0.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.470495 lazyqml-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.458494 lazyqml-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.462494 lazyqml-0.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.462494 lazyqml-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 11:57:31.000000 lazyqml-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 11:57:31.000000 lazyqml-0.3.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 11:57:31.000000 lazyqml-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 11:57:31.000000 lazyqml-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-09 11:57:42.470495 lazyqml-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 11:57:31.000000 lazyqml-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.466494 lazyqml-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.466494 lazyqml-0.3.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   827658 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.466494 lazyqml-0.3.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 11:57:31.000000 lazyqml-0.3.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.466494 lazyqml-0.3.2/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 11:57:31.000000 lazyqml-0.3.2/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31458 2024-05-09 11:57:31.000000 lazyqml-0.3.2/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    41989 2024-05-09 11:57:31.000000 lazyqml-0.3.2/lazyqml/supervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.466494 lazyqml-0.3.2/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-09 11:57:42.000000 lazyqml-0.3.2/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-09 11:57:42.000000 lazyqml-0.3.2/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:57:42.000000 lazyqml-0.3.2/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 11:57:42.000000 lazyqml-0.3.2/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-09 11:57:42.000000 lazyqml-0.3.2/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 11:57:42.000000 lazyqml-0.3.2/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-09 11:57:31.000000 lazyqml-0.3.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-09 11:57:31.000000 lazyqml-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 11:57:31.000000 lazyqml-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 11:57:31.000000 lazyqml-0.3.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:57:42.470495 lazyqml-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:57:42.466494 lazyqml-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 11:57:31.000000 lazyqml-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 11:57:31.000000 lazyqml-0.3.2/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.261883 lazyqml-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.249883 lazyqml-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.253883 lazyqml-0.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.253883 lazyqml-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 08:00:52.000000 lazyqml-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 08:00:52.000000 lazyqml-0.3.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 08:00:52.000000 lazyqml-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 08:00:52.000000 lazyqml-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 08:01:03.261883 lazyqml-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 08:00:52.000000 lazyqml-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.257883 lazyqml-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.257883 lazyqml-0.3.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.257883 lazyqml-0.3.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 08:00:52.000000 lazyqml-0.3.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.257883 lazyqml-0.3.3/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 08:00:52.000000 lazyqml-0.3.3/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31488 2024-05-10 08:00:52.000000 lazyqml-0.3.3/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41946 2024-05-10 08:00:52.000000 lazyqml-0.3.3/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.257883 lazyqml-0.3.3/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 08:01:03.000000 lazyqml-0.3.3/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 08:01:03.000000 lazyqml-0.3.3/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:01:03.000000 lazyqml-0.3.3/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 08:01:03.000000 lazyqml-0.3.3/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 08:01:03.000000 lazyqml-0.3.3/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 08:01:03.000000 lazyqml-0.3.3/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-10 08:00:52.000000 lazyqml-0.3.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 08:00:52.000000 lazyqml-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 08:00:52.000000 lazyqml-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 08:00:52.000000 lazyqml-0.3.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:01:03.261883 lazyqml-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:01:03.257883 lazyqml-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 08:00:52.000000 lazyqml-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 08:00:52.000000 lazyqml-0.3.3/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.3.2/.github/workflows/docs-build.yml` & `lazyqml-0.3.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/.github/workflows/docs.yml` & `lazyqml-0.3.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/.github/workflows/installation.yml` & `lazyqml-0.3.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/.github/workflows/macos.yml` & `lazyqml-0.3.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/.github/workflows/pypi.yml` & `lazyqml-0.3.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/.github/workflows/ubuntu.yml` & `lazyqml-0.3.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/.github/workflows/windows.yml` & `lazyqml-0.3.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/.gitignore` & `lazyqml-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/LICENSE` & `lazyqml-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/PKG-INFO` & `lazyqml-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.2
+Version: 0.3.3
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.2/docs/contributing.md` & `lazyqml-0.3.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/docs/installation.md` & `lazyqml-0.3.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/docs/usage.md` & `lazyqml-0.3.3/docs/usage.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/lazyqml/common.py` & `lazyqml-0.3.3/lazyqml/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #======================================================================================
 # The common module contains common functions and classes used by the other modules.
 #======================================================================================
 
 """
  Import Packages
 """
+from tabulate import tabulate
 import math
 import logging
 import pennylane as qml
 import jax.numpy as jnp
 import optax
 from itertools import combinations
 import pennylane as qml
```

### Comparing `lazyqml-0.3.2/lazyqml/supervised.py` & `lazyqml-0.3.3/lazyqml/supervised.py`

 * *Files 4% similar despite different names*

```diff
@@ -372,14 +372,15 @@
         
         self.customMetric = customMetric
 
         if errors > 0:
             for i in errormsg:
                 logging.error(i,exc_info=False)
             exit()
+        print(tabulate([[self.learningRate,self.epochs,self.runs,self.classifiers,self.embeddings,self.ansatzs,self.features,self.nqubits,self.numLayers,self.numPredictors]], headers=['Learning Rate', 'Epochs', "# Runs","Classifiers","Embeddings","Ansatzs","Features","Qubits","Layers","Predictors"], tablefmt='orgtbl'))
 
 
     
     def fit(self, X_train, X_test, y_train, y_test):
         """
         Fit Classification algorithms to X_train and y_train, predict and score on X_test, y_test.
         If the dimensions of the training vectors are not compatible with the different models, a 
@@ -683,20 +684,7 @@
             "Model"
         )
         if self.predictions:
             predictions_df = pd.DataFrame.from_dict(predictions)
         
         print(scores.to_markdown())
         return scores, predictions_df if self.predictions is True else scores
-
-from sklearn.datasets import load_breast_cancer, load_iris
-from sklearn.model_selection import train_test_split
-
-data = load_iris()
-X = data.data
-y = data.target
-
-X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.3,random_state =123)  
-
-q = QuantumClassifier(nqubits=8,verbose=True)
-
-scores, predicitons = q.fit(X_train, X_test, y_train, y_test)
```

### Comparing `lazyqml-0.3.2/lazyqml.egg-info/PKG-INFO` & `lazyqml-0.3.3/lazyqml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.2
+Version: 0.3.3
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.2/lazyqml.egg-info/SOURCES.txt` & `lazyqml-0.3.3/lazyqml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/mkdocs.yml` & `lazyqml-0.3.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/pyproject.toml` & `lazyqml-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lazyqml"
-version = "0.3.2"
+version = "0.3.3"
 dynamic = [
     "dependencies",
 ]
 description = "LazyQML benchmarking utility to test quantum machine learning models."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -46,15 +46,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.3.2"
+current_version = "0.3.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.3.2/requirements.txt` & `lazyqml-0.3.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/requirements_dev.txt` & `lazyqml-0.3.3/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.2/tests/test_lazyqml.py` & `lazyqml-0.3.3/tests/test_lazyqml.py`

 * *Files identical despite different names*

