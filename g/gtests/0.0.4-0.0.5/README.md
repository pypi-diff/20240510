# Comparing `tmp/gtests-0.0.4.tar.gz` & `tmp/gtests-0.0.5.tar.gz`

## Comparing `gtests-0.0.4.tar` & `gtests-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtests-0.0.4/setup.cfg
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 gtests-0.0.4/setup.py
--rw-r--r--   0        0        0    33344 2020-02-02 00:00:00.000000 gtests-0.0.4/src/gtests/MST.so
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtests-0.0.4/src/gtests/__init__.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 gtests-0.0.4/src/gtests/graphutilities.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 gtests-0.0.4/src/gtests/gtests.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 gtests-0.0.4/LICENSE
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 gtests-0.0.4/README.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 gtests-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 gtests-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 gtests-0.0.5/setup.cfg
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 gtests-0.0.5/setup.py
+-rw-r--r--   0        0        0    33344 2020-02-02 00:00:00.000000 gtests-0.0.5/src/gtests/MST.so
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtests-0.0.5/src/gtests/__init__.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 gtests-0.0.5/src/gtests/graphutilities.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 gtests-0.0.5/src/gtests/gtests.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 gtests-0.0.5/LICENSE
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 gtests-0.0.5/README.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 gtests-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 gtests-0.0.5/PKG-INFO
```

### Comparing `gtests-0.0.4/setup.py` & `gtests-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'gtestsPackage',         # How you named your package folder (MyLib)
   packages = ['gtests'],   # Chose the same as "name"
-  version = '0.0.4',      # Start with a small number and increase it with every change you make
+  version = '0.0.5',      # Start with a small number and increase it with every change you make
   license='GPL-3.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Graph-Based Two Sample Test',   # Give a short description about your library
   author = 'Alexander Wold',                   # Type in your name
   author_email = 'alexwold@iastate.edu',      # Type in your E-Mail
   url = 'https://github.com/atwold/gtests.git',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/atwold/gtests/archive/refs/tags/0.0.4.tar.gz',    # I explain this later on
   keywords = ['TWO-SAMPLE', 'GRAPH-BASED', 'GRAPH', 'TWO SAMPLE', 'GRAPH BASED', 'TEST', 'NONPARAMETRIC'],   # Keywords that define your package best
```

### Comparing `gtests-0.0.4/src/gtests/MST.so` & `gtests-0.0.5/src/gtests/MST.so`

 * *Files identical despite different names*

### Comparing `gtests-0.0.4/src/gtests/graphutilities.py` & `gtests-0.0.5/src/gtests/graphutilities.py`

 * *Files identical despite different names*

### Comparing `gtests-0.0.4/src/gtests/gtests.py` & `gtests-0.0.5/src/gtests/gtests.py`

 * *Files identical despite different names*

### Comparing `gtests-0.0.4/LICENSE` & `gtests-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gtests-0.0.4/PKG-INFO` & `gtests-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtests
-Version: 0.0.4
+Version: 0.0.5
 Summary: Graph-Based Two Sample Test
 Author-email: Alexander Wold <alexwold@iastate.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
```

