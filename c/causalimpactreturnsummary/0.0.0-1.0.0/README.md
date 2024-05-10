# Comparing `tmp/causalimpactreturnsummary-0.0.0.tar.gz` & `tmp/causalimpactreturnsummary-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalimpactreturnsummary-0.0.0.tar", last modified: Fri May 10 10:29:58 2024, max compression
+gzip compressed data, was "causalimpactreturnsummary-1.0.0.tar", last modified: Fri May 10 11:04:13 2024, max compression
```

## Comparing `causalimpactreturnsummary-0.0.0.tar` & `causalimpactreturnsummary-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 10:29:58.791549 causalimpactreturnsummary-0.0.0/
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     3786 2024-05-10 10:29:58.791470 causalimpactreturnsummary-0.0.0/PKG-INFO
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     2613 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/README.md
--rw-r--r--   0 danielwilkinson   (501) staff       (20)      450 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/pyproject.toml
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     1615 2024-05-10 10:29:58.791931 causalimpactreturnsummary-0.0.0/setup.cfg
--rw-r--r--   0 danielwilkinson   (501) staff       (20)      709 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/setup.py
-drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 10:29:58.787093 causalimpactreturnsummary-0.0.0/src/
-drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 10:29:58.790942 causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     3786 2024-05-10 10:29:58.000000 causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/PKG-INFO
--rw-r--r--   0 danielwilkinson   (501) staff       (20)      586 2024-05-10 10:29:58.000000 causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/SOURCES.txt
--rw-r--r--   0 danielwilkinson   (501) staff       (20)        1 2024-05-10 10:29:58.000000 causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/dependency_links.txt
--rw-r--r--   0 danielwilkinson   (501) staff       (20)        1 2024-05-10 10:29:58.000000 causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/not-zip-safe
--rw-r--r--   0 danielwilkinson   (501) staff       (20)      136 2024-05-10 10:29:58.000000 causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/requires.txt
--rw-r--r--   0 danielwilkinson   (501) staff       (20)       13 2024-05-10 10:29:58.000000 causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/top_level.txt
-drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 10:29:58.789894 causalimpactreturnsummary-0.0.0/src/causalimpact/
--rw-r--r--   0 danielwilkinson   (501) staff       (20)      863 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/src/causalimpact/__init__.py
--rw-r--r--   0 danielwilkinson   (501) staff       (20)    37209 2024-05-10 10:05:30.000000 causalimpactreturnsummary-0.0.0/src/causalimpact/analysis.py
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     4748 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/src/causalimpact/inferences.py
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     1936 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/src/causalimpact/misc.py
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     7780 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/src/causalimpact/model.py
-drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 10:29:58.790639 causalimpactreturnsummary-0.0.0/tests/
--rw-r--r--   0 danielwilkinson   (501) staff       (20)    35197 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/tests/test_analysis.py
--rw-r--r--   0 danielwilkinson   (501) staff       (20)    10559 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/tests/test_inferences.py
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     2539 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/tests/test_misc.py
--rw-r--r--   0 danielwilkinson   (501) staff       (20)     2727 2024-05-10 10:03:54.000000 causalimpactreturnsummary-0.0.0/tests/test_model.py
+drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 11:04:13.451789 causalimpactreturnsummary-1.0.0/
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     3786 2024-05-10 11:04:13.451699 causalimpactreturnsummary-1.0.0/PKG-INFO
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     2613 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/README.md
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)      450 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/pyproject.toml
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     1615 2024-05-10 11:04:13.452292 causalimpactreturnsummary-1.0.0/setup.cfg
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)      729 2024-05-10 11:04:01.000000 causalimpactreturnsummary-1.0.0/setup.py
+drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 11:04:13.444337 causalimpactreturnsummary-1.0.0/src/
+drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 11:04:13.448909 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)      863 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/__init__.py
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)    37209 2024-05-10 10:34:20.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/analysis.py
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     4748 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/inferences.py
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     1936 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/misc.py
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     7780 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/model.py
+drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 11:04:13.451139 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     3786 2024-05-10 11:04:13.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/PKG-INFO
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     1172 2024-05-10 11:04:13.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/SOURCES.txt
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)        1 2024-05-10 11:04:13.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/dependency_links.txt
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)        1 2024-05-10 10:34:43.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/not-zip-safe
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)      136 2024-05-10 11:04:13.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/requires.txt
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)       26 2024-05-10 11:04:13.000000 causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/top_level.txt
+drwxr-xr-x   0 danielwilkinson   (501) staff       (20)        0 2024-05-10 11:04:13.450908 causalimpactreturnsummary-1.0.0/tests/
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)    35197 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/tests/test_analysis.py
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)    10559 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/tests/test_inferences.py
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     2539 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/tests/test_misc.py
+-rw-r--r--   0 danielwilkinson   (501) staff       (20)     2727 2024-05-10 10:03:54.000000 causalimpactreturnsummary-1.0.0/tests/test_model.py
```

### Comparing `causalimpactreturnsummary-0.0.0/PKG-INFO` & `causalimpactreturnsummary-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: causalImpactReturnSummary
-Version: 0.0.0
+Name: causalimpactreturnsummary
+Version: 1.0.0
 Summary: Python Package for causal inference using Bayesian structural time-series models with data returned..
 Home-page: https://github.com/jamalsenouci/causalimpact/
 Author: Dan Wilkinson
 Author-email: danwdigital@gmail.com
 License: MIT
 Project-URL: Documentation, https://nbviewer.org/github/jamalsenouci/causalimpact/blob/master/GettingStarted.ipynb
 Project-URL: Source, https://github.com/jamalsenouci/causalimpact/
```

### Comparing `causalimpactreturnsummary-0.0.0/README.md` & `causalimpactreturnsummary-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/setup.cfg` & `causalimpactreturnsummary-1.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-name = causalImpactReturnSummary
+name = causalimpactreturnsummary
 description = Python Package for causal inference using Bayesian structural time-series models with data returned..
 author = Dan Wilkinson
 author_email = danwdigital@gmail.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
@@ -68,15 +68,15 @@
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 
 [pyscaffold]
-version = 4.2.1
+version = 0.0.1
 package = causalimpact
 extensions = 
 	no_skeleton
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `causalimpactreturnsummary-0.0.0/setup.py` & `causalimpactreturnsummary-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Learn more under: https://pyscaffold.org/
 """
 
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
-        setup(use_scm_version={"version_scheme": "no-guess-dev"})
+        setup(use_scm_version={"version_scheme": "no-guess-dev"}, version='1.0.0',), 
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
         )
```

### Comparing `causalimpactreturnsummary-0.0.0/src/causalImpactReturnSummary.egg-info/PKG-INFO` & `causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: causalImpactReturnSummary
-Version: 0.0.0
+Name: causalimpactreturnsummary
+Version: 1.0.0
 Summary: Python Package for causal inference using Bayesian structural time-series models with data returned..
 Home-page: https://github.com/jamalsenouci/causalimpact/
 Author: Dan Wilkinson
 Author-email: danwdigital@gmail.com
 License: MIT
 Project-URL: Documentation, https://nbviewer.org/github/jamalsenouci/causalimpact/blob/master/GettingStarted.ipynb
 Project-URL: Source, https://github.com/jamalsenouci/causalimpact/
```

### Comparing `causalimpactreturnsummary-0.0.0/src/causalimpact/__init__.py` & `causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/__init__.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/src/causalimpact/analysis.py` & `causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/analysis.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/src/causalimpact/inferences.py` & `causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/inferences.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/src/causalimpact/misc.py` & `causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/misc.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/src/causalimpact/model.py` & `causalimpactreturnsummary-1.0.0/src/causalImpactReturnSummary/model.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/tests/test_analysis.py` & `causalimpactreturnsummary-1.0.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/tests/test_inferences.py` & `causalimpactreturnsummary-1.0.0/tests/test_inferences.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/tests/test_misc.py` & `causalimpactreturnsummary-1.0.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `causalimpactreturnsummary-0.0.0/tests/test_model.py` & `causalimpactreturnsummary-1.0.0/tests/test_model.py`

 * *Files identical despite different names*

