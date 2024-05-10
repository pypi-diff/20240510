# Comparing `tmp/lazyqml-0.3.5.tar.gz` & `tmp/lazyqml-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.3.5.tar", last modified: Fri May 10 09:25:07 2024, max compression
+gzip compressed data, was "lazyqml-0.3.6.tar", last modified: Fri May 10 09:39:19 2024, max compression
```

## Comparing `lazyqml-0.3.5.tar` & `lazyqml-0.3.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.771769 lazyqml-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.763769 lazyqml-0.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.767769 lazyqml-0.3.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.767769 lazyqml-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 09:24:57.000000 lazyqml-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 09:24:57.000000 lazyqml-0.3.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 09:24:57.000000 lazyqml-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 09:24:57.000000 lazyqml-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:25:07.771769 lazyqml-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 09:24:57.000000 lazyqml-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.767769 lazyqml-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.767769 lazyqml-0.3.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.767769 lazyqml-0.3.5/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 09:24:57.000000 lazyqml-0.3.5/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.771769 lazyqml-0.3.5/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 09:24:57.000000 lazyqml-0.3.5/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31488 2024-05-10 09:24:57.000000 lazyqml-0.3.5/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    41975 2024-05-10 09:24:57.000000 lazyqml-0.3.5/lazyqml/supervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.771769 lazyqml-0.3.5/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:25:07.000000 lazyqml-0.3.5/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 09:25:07.000000 lazyqml-0.3.5/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:25:07.000000 lazyqml-0.3.5/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 09:25:07.000000 lazyqml-0.3.5/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 09:25:07.000000 lazyqml-0.3.5/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:25:07.000000 lazyqml-0.3.5/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-10 09:24:57.000000 lazyqml-0.3.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 09:24:57.000000 lazyqml-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 09:24:57.000000 lazyqml-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:24:57.000000 lazyqml-0.3.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:25:07.771769 lazyqml-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:25:07.771769 lazyqml-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 09:24:57.000000 lazyqml-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 09:24:57.000000 lazyqml-0.3.5/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.722792 lazyqml-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.714792 lazyqml-0.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.714792 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 09:39:09.000000 lazyqml-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 09:39:09.000000 lazyqml-0.3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 09:39:09.000000 lazyqml-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 09:39:09.000000 lazyqml-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:39:19.722792 lazyqml-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 09:39:09.000000 lazyqml-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 09:39:09.000000 lazyqml-0.3.6/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 09:39:09.000000 lazyqml-0.3.6/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31488 2024-05-10 09:39:09.000000 lazyqml-0.3.6/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-10 09:39:09.000000 lazyqml-0.3.6/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:39:19.000000 lazyqml-0.3.6/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-10 09:39:09.000000 lazyqml-0.3.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-10 09:39:09.000000 lazyqml-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 09:39:09.000000 lazyqml-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 09:39:09.000000 lazyqml-0.3.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:39:19.722792 lazyqml-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:19.718792 lazyqml-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 09:39:09.000000 lazyqml-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 09:39:09.000000 lazyqml-0.3.6/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.3.5/.github/workflows/docs-build.yml` & `lazyqml-0.3.6/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/.github/workflows/docs.yml` & `lazyqml-0.3.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/.github/workflows/installation.yml` & `lazyqml-0.3.6/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/.github/workflows/macos.yml` & `lazyqml-0.3.6/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/.github/workflows/pypi.yml` & `lazyqml-0.3.6/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/.github/workflows/ubuntu.yml` & `lazyqml-0.3.6/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/.github/workflows/windows.yml` & `lazyqml-0.3.6/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/.gitignore` & `lazyqml-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/LICENSE` & `lazyqml-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/PKG-INFO` & `lazyqml-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.5
+Version: 0.3.6
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.5/docs/contributing.md` & `lazyqml-0.3.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/docs/examples/intro.ipynb` & `lazyqml-0.3.6/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/docs/installation.md` & `lazyqml-0.3.6/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/docs/usage.md` & `lazyqml-0.3.6/docs/usage.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/lazyqml/common.py` & `lazyqml-0.3.6/lazyqml/common.py`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/lazyqml/supervised.py` & `lazyqml-0.3.6/lazyqml/supervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Main Module
 #======================================================================================
 
 """
  Import modules
 """
 
-from .common import *
+from common import *
 import warnings
 warnings.filterwarnings("ignore")
 
 """
  Classifiers
 """
 
@@ -325,52 +325,52 @@
 
         self.maxSamples = maxSamples
 
         if isinstance(verbose,bool):
             self.verbose = verbose
             self.verboseprint = print if verbose else lambda *a, **k: None
         else:
-            logging.info("Verbose is not an instance of bool, False will be assumed.")
+            logging.warn("Verbose is not an instance of bool, False will be assumed.")
             self.verboseprint = lambda *a, **k: None
 
         if optimizer is None:
-            logging.info("No optimizer has been passed adam will be used by default.")
+            logging.warn("No optimizer has been passed adam will be used by default.")
             self.optimizer = optax.adam(learning_rate=self.learningRate)
         else:
             if issubclass(optimizer.__annotations__["return"],optax._src.base.GradientTransformation):
-                logging.info("Optimizer is an optax optimizer; setting its learning rate.")
+                logging.warn("Optimizer is an optax optimizer; setting its learning rate.")
                 self.optimizer = optax.inject_hyperparams(optimizer)(learning_rate=self.learningRate)
             else:
                 
-                logging.info("Optimizer is not from optax library; using the default optimizer.")
+                logging.warn("Optimizer is not from optax library; using the default optimizer.")
                 self.optimizer = optax.adam(learning_rate=self.learningRate)
         
         if customImputerNum is not None:
             module = inspect.getmodule(customImputerNum)
             # Check if the module belongs to sklearn.impute
             if module.__name__.startswith('sklearn.impute'):
-                logging.info("The object belongs to the sklearn.impute module. Custom Numeric Imputer will be used.")
+                logging.warn("The object belongs to the sklearn.impute module. Custom Numeric Imputer will be used.")
                 self.numeric_transformer = Pipeline(
                 steps=[("imputer",customImputerNum), ("scaler", StandardScaler())])
             else:
-                logging.info("The object does not belong to the sklearn.impute module. Default Custom Numeric Imputer will be used.")
+                logging.warn("The object does not belong to the sklearn.impute module. Default Custom Numeric Imputer will be used.")
         else:
             self.numeric_transformer = Pipeline(
             steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())])
 
 
         if customImputerCat is not None:
             module = inspect.getmodule(customImputerNum)
             # Check if the module belongs to sklearn.impute
             if module.__name__.startswith('sklearn.impute'):
-                logging.info("The object belongs to the sklearn.impute module. Custom Numeric Categorical will be used.")
+                logging.warn("The object belongs to the sklearn.impute module. Custom Numeric Categorical will be used.")
                 self.categorical_transformer = Pipeline(
                 steps=[("imputer",customImputerCat), ("scaler", StandardScaler())])
             else:
-                logging.info("The object does not belong to the sklearn.impute module. Default Custom Categorical Imputer will be used.")
+                logging.warn("The object does not belong to the sklearn.impute module. Default Custom Categorical Imputer will be used.")
         else:    
             self.categorical_transformer = Pipeline(
             steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())])
         
         self.customMetric = customMetric
 
         if errors > 0:
@@ -685,7 +685,21 @@
             "Model"
         )
         if self.predictions:
             predictions_df = pd.DataFrame.from_dict(predictions)
         
         print(scores.to_markdown())
         return scores, predictions_df if self.predictions is True else scores
+
+from sklearn.datasets import load_breast_cancer, load_iris
+from sklearn.model_selection import train_test_split
+data = load_breast_cancer()
+X = data.data
+y = data.target
+
+X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.3,random_state =123)  
+#print(issubclass(optax.adam.__annotations__["return"],optax._src.base.GradientTransformation) )
+
+
+q = QuantumClassifier(nqubits=2,classifiers=["qnn"],optimizer=optax.adabelief,learningRate=0.1,verbose=True)
+
+scores, predicitons = q.fit(X_train, X_test, y_train, y_test)
```

### Comparing `lazyqml-0.3.5/lazyqml.egg-info/PKG-INFO` & `lazyqml-0.3.6/lazyqml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.5
+Version: 0.3.6
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.5/lazyqml.egg-info/SOURCES.txt` & `lazyqml-0.3.6/lazyqml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/mkdocs.yml` & `lazyqml-0.3.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/pyproject.toml` & `lazyqml-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lazyqml"
-version = "0.3.5"
+version = "0.3.6"
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
-current_version = "0.3.5"
+current_version = "0.3.6"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.3.5/requirements.txt` & `lazyqml-0.3.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/requirements_dev.txt` & `lazyqml-0.3.6/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.5/tests/test_lazyqml.py` & `lazyqml-0.3.6/tests/test_lazyqml.py`

 * *Files identical despite different names*

