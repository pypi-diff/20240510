# Comparing `tmp/optimaladj-0.0.4.tar.gz` & `tmp/optimaladj-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimaladj-0.0.4.tar", last modified: Thu Dec  1 10:26:46 2022, max compression
+gzip compressed data, was "optimaladj-0.0.5.tar", last modified: Fri May 10 07:28:44 2024, max compression
```

## Comparing `optimaladj-0.0.4.tar` & `optimaladj-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2022-12-01 10:26:46.466076 optimaladj-0.0.4/
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)     1093 2021-12-29 12:40:13.000000 optimaladj-0.0.4/LICENSE
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)     3732 2022-12-01 10:26:46.465474 optimaladj-0.0.4/PKG-INFO
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)     3202 2022-01-08 10:28:19.000000 optimaladj-0.0.4/README.md
-drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2022-12-01 10:26:46.455183 optimaladj-0.0.4/optimaladj/
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)    14155 2022-11-28 21:00:15.000000 optimaladj-0.0.4/optimaladj/CausalGraph.py
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)        0 2021-12-29 12:40:13.000000 optimaladj-0.0.4/optimaladj/__init__.py
-drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2022-12-01 10:26:46.460560 optimaladj-0.0.4/optimaladj.egg-info/
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)     3732 2022-12-01 10:26:46.000000 optimaladj-0.0.4/optimaladj.egg-info/PKG-INFO
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)      273 2022-12-01 10:26:46.000000 optimaladj-0.0.4/optimaladj.egg-info/SOURCES.txt
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)        1 2022-12-01 10:26:46.000000 optimaladj-0.0.4/optimaladj.egg-info/dependency_links.txt
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)       17 2022-12-01 10:26:46.000000 optimaladj-0.0.4/optimaladj.egg-info/top_level.txt
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)       38 2022-12-01 10:26:46.466279 optimaladj-0.0.4/setup.cfg
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)      727 2022-11-28 21:01:24.000000 optimaladj-0.0.4/setup.py
-drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2022-12-01 10:26:46.463567 optimaladj-0.0.4/tests/
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)        0 2021-12-29 12:40:13.000000 optimaladj-0.0.4/tests/__init__.py
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)    10561 2022-11-29 19:01:33.000000 optimaladj-0.0.4/tests/examples.py
--rw-r--r--   0 ezequielsmucler   (502) staff       (20)     2755 2022-11-29 19:01:07.000000 optimaladj-0.0.4/tests/test_CausalGraph.py
+drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2024-05-10 07:28:44.456435 optimaladj-0.0.5/
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)     1093 2021-12-29 12:40:13.000000 optimaladj-0.0.5/LICENSE
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)     3732 2024-05-10 07:28:44.456036 optimaladj-0.0.5/PKG-INFO
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)     3202 2022-01-08 10:28:19.000000 optimaladj-0.0.5/README.md
+drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2024-05-10 07:28:44.446941 optimaladj-0.0.5/optimaladj/
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)    14165 2024-05-10 07:18:58.000000 optimaladj-0.0.5/optimaladj/CausalGraph.py
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)        0 2021-12-29 12:40:13.000000 optimaladj-0.0.5/optimaladj/__init__.py
+drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2024-05-10 07:28:44.450882 optimaladj-0.0.5/optimaladj.egg-info/
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)     3732 2024-05-10 07:28:44.000000 optimaladj-0.0.5/optimaladj.egg-info/PKG-INFO
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)      273 2024-05-10 07:28:44.000000 optimaladj-0.0.5/optimaladj.egg-info/SOURCES.txt
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)        1 2024-05-10 07:28:44.000000 optimaladj-0.0.5/optimaladj.egg-info/dependency_links.txt
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)       17 2024-05-10 07:28:44.000000 optimaladj-0.0.5/optimaladj.egg-info/top_level.txt
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)       38 2024-05-10 07:28:44.456699 optimaladj-0.0.5/setup.cfg
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)      727 2024-05-10 07:22:59.000000 optimaladj-0.0.5/setup.py
+drwxr-xr-x   0 ezequielsmucler   (502) staff       (20)        0 2024-05-10 07:28:44.455176 optimaladj-0.0.5/tests/
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)        0 2021-12-29 12:40:13.000000 optimaladj-0.0.5/tests/__init__.py
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)    10561 2024-05-10 07:18:58.000000 optimaladj-0.0.5/tests/examples.py
+-rw-r--r--   0 ezequielsmucler   (502) staff       (20)     2755 2024-05-10 07:18:58.000000 optimaladj-0.0.5/tests/test_CausalGraph.py
```

### Comparing `optimaladj-0.0.4/LICENSE` & `optimaladj-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optimaladj-0.0.4/PKG-INFO` & `optimaladj-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimaladj
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to compute optimal adjustment sets in causal graphs
 Home-page: https://github.com/facusapienza21/optimaladj
 Author: Facundo Sapienza, Ezequiel Smucler
 Author-email: ezequiels.90@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `optimaladj-0.0.4/README.md` & `optimaladj-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `optimaladj-0.0.4/optimaladj/CausalGraph.py` & `optimaladj-0.0.5/optimaladj/CausalGraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         Returns
         ----------
         optimal: set
         """
         H1 = self.build_H1(treatment, outcome, L, N)
         if treatment in H1.neighbors(outcome):
             raise NoAdjException(EXCEPTION_NO_ADJ)
-        elif N == self.nodes() or set(N).issubset(
+        elif set(N) == set(self.nodes()) or set(N).issubset(
             self.ancestors_all(L + [treatment, outcome])
         ):
             optimal = nx.node_boundary(H1, set([outcome]))
             return optimal
         else:
             raise ConditionException(EXCEPTION_COND)
```

### Comparing `optimaladj-0.0.4/optimaladj.egg-info/PKG-INFO` & `optimaladj-0.0.5/optimaladj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimaladj
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to compute optimal adjustment sets in causal graphs
 Home-page: https://github.com/facusapienza21/optimaladj
 Author: Facundo Sapienza, Ezequiel Smucler
 Author-email: ezequiels.90@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `optimaladj-0.0.4/setup.py` & `optimaladj-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="optimaladj",
-    version="0.0.4",
+    version="0.0.5",
     author="Facundo Sapienza, Ezequiel Smucler",
     author_email="ezequiels.90@gmail.com",
     description="A package to compute optimal adjustment sets in causal graphs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facusapienza21/optimaladj",
     packages=setuptools.find_packages(),
```

### Comparing `optimaladj-0.0.4/tests/examples.py` & `optimaladj-0.0.5/tests/examples.py`

 * *Files identical despite different names*

### Comparing `optimaladj-0.0.4/tests/test_CausalGraph.py` & `optimaladj-0.0.5/tests/test_CausalGraph.py`

 * *Files identical despite different names*

