# Comparing `tmp/lazyqml-0.3.6.tar.gz` & `tmp/lazyqml-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.3.6.tar", last modified: Fri May 10 09:39:19 2024, max compression
+gzip compressed data, was "lazyqml-0.3.7.tar", last modified: Fri May 10 09:41:30 2024, max compression
```

## Comparing `lazyqml-0.3.6.tar` & `lazyqml-0.3.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.722792 lazyqml-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.714792 lazyqml-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.714792 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 09:39:09.000000 lazyqml-0.3.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 09:39:09.000000 lazyqml-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 09:39:09.000000 lazyqml-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:39:19.722792 lazyqml-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 09:39:09.000000 lazyqml-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 09:39:09.000000 lazyqml-0.3.6/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31488 2024-05-10 09:39:09.000000 lazyqml-0.3.6/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-10 09:39:09.000000 lazyqml-0.3.6/lazyqml/supervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-10 09:39:09.000000 lazyqml-0.3.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 09:39:09.000000 lazyqml-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 09:39:09.000000 lazyqml-0.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:39:09.000000 lazyqml-0.3.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:39:19.722792 lazyqml-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 09:39:09.000000 lazyqml-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 09:39:09.000000 lazyqml-0.3.6/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.371717 lazyqml-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.363717 lazyqml-0.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.367717 lazyqml-0.3.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.367717 lazyqml-0.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 09:41:19.000000 lazyqml-0.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 09:41:19.000000 lazyqml-0.3.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 09:41:19.000000 lazyqml-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 09:41:19.000000 lazyqml-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:41:30.371717 lazyqml-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 09:41:19.000000 lazyqml-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.371717 lazyqml-0.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.371717 lazyqml-0.3.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.371717 lazyqml-0.3.7/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 09:41:19.000000 lazyqml-0.3.7/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.371717 lazyqml-0.3.7/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 09:41:19.000000 lazyqml-0.3.7/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31488 2024-05-10 09:41:19.000000 lazyqml-0.3.7/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41975 2024-05-10 09:41:19.000000 lazyqml-0.3.7/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.371717 lazyqml-0.3.7/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:41:30.000000 lazyqml-0.3.7/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 09:41:30.000000 lazyqml-0.3.7/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:41:30.000000 lazyqml-0.3.7/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 09:41:30.000000 lazyqml-0.3.7/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 09:41:30.000000 lazyqml-0.3.7/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:41:30.000000 lazyqml-0.3.7/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-10 09:41:19.000000 lazyqml-0.3.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 09:41:19.000000 lazyqml-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 09:41:19.000000 lazyqml-0.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:41:19.000000 lazyqml-0.3.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:41:30.371717 lazyqml-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:41:30.371717 lazyqml-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 09:41:19.000000 lazyqml-0.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 09:41:19.000000 lazyqml-0.3.7/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.3.6/.github/workflows/docs-build.yml` & `lazyqml-0.3.7/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/.github/workflows/docs.yml` & `lazyqml-0.3.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/.github/workflows/installation.yml` & `lazyqml-0.3.7/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/.github/workflows/macos.yml` & `lazyqml-0.3.7/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/.github/workflows/pypi.yml` & `lazyqml-0.3.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/.github/workflows/ubuntu.yml` & `lazyqml-0.3.7/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/.github/workflows/windows.yml` & `lazyqml-0.3.7/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/.gitignore` & `lazyqml-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/LICENSE` & `lazyqml-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/PKG-INFO` & `lazyqml-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.6
+Version: 0.3.7
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.6/docs/contributing.md` & `lazyqml-0.3.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/docs/examples/intro.ipynb` & `lazyqml-0.3.7/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/docs/installation.md` & `lazyqml-0.3.7/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/docs/usage.md` & `lazyqml-0.3.7/docs/usage.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/lazyqml/common.py` & `lazyqml-0.3.7/lazyqml/common.py`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/lazyqml/supervised.py` & `lazyqml-0.3.7/lazyqml/supervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Main Module
 #======================================================================================
 
 """
  Import modules
 """
 
-from common import *
+from .common import *
 import warnings
 warnings.filterwarnings("ignore")
 
 """
  Classifiers
 """
 
@@ -685,21 +685,7 @@
             "Model"
         )
         if self.predictions:
             predictions_df = pd.DataFrame.from_dict(predictions)
         
         print(scores.to_markdown())
         return scores, predictions_df if self.predictions is True else scores
-
-from sklearn.datasets import load_breast_cancer, load_iris
-from sklearn.model_selection import train_test_split
-data = load_breast_cancer()
-X = data.data
-y = data.target
-
-X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.3,random_state =123)  
-#print(issubclass(optax.adam.__annotations__["return"],optax._src.base.GradientTransformation) )
-
-
-q = QuantumClassifier(nqubits=2,classifiers=["qnn"],optimizer=optax.adabelief,learningRate=0.1,verbose=True)
-
-scores, predicitons = q.fit(X_train, X_test, y_train, y_test)
```

### Comparing `lazyqml-0.3.6/lazyqml.egg-info/PKG-INFO` & `lazyqml-0.3.7/lazyqml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.6
+Version: 0.3.7
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.6/lazyqml.egg-info/SOURCES.txt` & `lazyqml-0.3.7/lazyqml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/mkdocs.yml` & `lazyqml-0.3.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/pyproject.toml` & `lazyqml-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lazyqml"
-version = "0.3.6"
+version = "0.3.7"
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
-current_version = "0.3.6"
+current_version = "0.3.7"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.3.6/requirements.txt` & `lazyqml-0.3.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/requirements_dev.txt` & `lazyqml-0.3.7/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.6/tests/test_lazyqml.py` & `lazyqml-0.3.7/tests/test_lazyqml.py`

 * *Files identical despite different names*

