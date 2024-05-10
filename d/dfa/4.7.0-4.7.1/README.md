# Comparing `tmp/dfa-4.7.0.tar.gz` & `tmp/dfa-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfa-4.7.0.tar", max compression
+gzip compressed data, was "dfa-4.7.1.tar", max compression
```

## Comparing `dfa-4.7.0.tar` & `dfa-4.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1082 2024-04-06 21:02:22.520870 dfa-4.7.0/LICENSE
--rw-r--r--   0        0        0     7737 2024-04-06 21:02:22.520870 dfa-4.7.0/README.md
--rw-r--r--   0        0        0      230 2024-04-06 21:02:22.521870 dfa-4.7.0/dfa/__init__.py
--rw-r--r--   0        0        0    11108 2024-05-03 04:23:29.638050 dfa-4.7.0/dfa/dfa.py
--rw-r--r--   0        0        0      649 2024-04-06 21:02:22.521870 dfa-4.7.0/dfa/draw.py
--rw-r--r--   0        0        0     6752 2024-05-08 03:32:12.192184 dfa-4.7.0/dfa/utils.py
--rw-r--r--   0        0        0      670 2024-05-08 03:32:47.472021 dfa-4.7.0/pyproject.toml
--rw-r--r--   0        0        0     8629 1970-01-01 00:00:00.000000 dfa-4.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-06 21:02:22.520870 dfa-4.7.1/LICENSE
+-rw-r--r--   0        0        0     7737 2024-04-06 21:02:22.520870 dfa-4.7.1/README.md
+-rw-r--r--   0        0        0      230 2024-04-06 21:02:22.521870 dfa-4.7.1/dfa/__init__.py
+-rw-r--r--   0        0        0    11108 2024-05-10 02:14:45.273924 dfa-4.7.1/dfa/dfa.py
+-rw-r--r--   0        0        0      649 2024-04-06 21:02:22.521870 dfa-4.7.1/dfa/draw.py
+-rw-r--r--   0        0        0     6752 2024-05-08 03:32:12.192184 dfa-4.7.1/dfa/utils.py
+-rw-r--r--   0        0        0      670 2024-05-10 02:17:22.208334 dfa-4.7.1/pyproject.toml
+-rw-r--r--   0        0        0     8629 1970-01-01 00:00:00.000000 dfa-4.7.1/PKG-INFO
```

### Comparing `dfa-4.7.0/LICENSE` & `dfa-4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dfa-4.7.0/README.md` & `dfa-4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dfa-4.7.0/dfa/dfa.py` & `dfa-4.7.1/dfa/dfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         access_string = []
         while stack:
             (curr, suffix), depth = stack.pop()
             if curr in visited:
                 continue
             visited.add(curr)
 
-            del access_string[depth:]     # Remove previous path suffix.
+            del access_string[depth-1:]   # Remove previous path suffix.
             access_string.extend(suffix)  # Add new path suffix.
 
             yield (curr, access_string)
 
             successors = ((self._transition(curr, a), (a,)) for a in inputs)
             stack.extend((state, depth + 1) for state in successors)
```

### Comparing `dfa-4.7.0/dfa/draw.py` & `dfa-4.7.1/dfa/draw.py`

 * *Files identical despite different names*

### Comparing `dfa-4.7.0/dfa/utils.py` & `dfa-4.7.1/dfa/utils.py`

 * *Files identical despite different names*

### Comparing `dfa-4.7.0/pyproject.toml` & `dfa-4.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dfa"
 readme="README.md"
-version = "4.7.0"
+version = "4.7.1"
 description = "Python library for modeling DFAs, Moore Machines, and Transition Systems."
 authors = ["Marcell Vazquez-Chanlatte <marcell.vc@eecs.berkeley.edu>"]
 repository = "https://github.com/mvcisback/dfa"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dfa-4.7.0/PKG-INFO` & `dfa-4.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfa
-Version: 4.7.0
+Version: 4.7.1
 Summary: Python library for modeling DFAs, Moore Machines, and Transition Systems.
 Home-page: https://github.com/mvcisback/dfa
 License: MIT
 Author: Marcell Vazquez-Chanlatte
 Author-email: marcell.vc@eecs.berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

