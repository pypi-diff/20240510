# Comparing `tmp/phonecodes-1.1.0.tar.gz` & `tmp/phonecodes-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonecodes-1.1.0.tar", last modified: Fri Feb 16 21:31:12 2024, max compression
+gzip compressed data, was "phonecodes-1.1.1.tar", last modified: Thu May  9 22:00:57 2024, max compression
```

## Comparing `phonecodes-1.1.0.tar` & `phonecodes-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:31:12.735419 phonecodes-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-16 21:31:03.000000 phonecodes-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-02-16 21:31:12.735419 phonecodes-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-16 21:31:03.000000 phonecodes-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-16 21:31:03.000000 phonecodes-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 21:31:12.735419 phonecodes-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:31:12.731419 phonecodes-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:31:12.731419 phonecodes-1.1.0/src/phonecodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 21:31:03.000000 phonecodes-1.1.0/src/phonecodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-02-16 21:31:03.000000 phonecodes-1.1.0/src/phonecodes/phonecode_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-02-16 21:31:03.000000 phonecodes-1.1.0/src/phonecodes/phonecodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-02-16 21:31:03.000000 phonecodes-1.1.0/src/phonecodes/pronlex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:31:12.735419 phonecodes-1.1.0/src/phonecodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-02-16 21:31:12.000000 phonecodes-1.1.0/src/phonecodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-16 21:31:12.000000 phonecodes-1.1.0/src/phonecodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 21:31:12.000000 phonecodes-1.1.0/src/phonecodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 21:31:12.000000 phonecodes-1.1.0/src/phonecodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-16 21:31:12.000000 phonecodes-1.1.0/src/phonecodes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:31:12.735419 phonecodes-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-02-16 21:31:03.000000 phonecodes-1.1.0/test/test_phonecodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-02-16 21:31:03.000000 phonecodes-1.1.0/test/test_pronlex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:00:57.959832 phonecodes-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-09 22:00:47.000000 phonecodes-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-09 22:00:57.959832 phonecodes-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-09 22:00:47.000000 phonecodes-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-09 22:00:47.000000 phonecodes-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:00:57.959832 phonecodes-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:00:57.955832 phonecodes-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:00:57.959832 phonecodes-1.1.1/src/phonecodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:00:47.000000 phonecodes-1.1.1/src/phonecodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-05-09 22:00:47.000000 phonecodes-1.1.1/src/phonecodes/phonecode_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-09 22:00:47.000000 phonecodes-1.1.1/src/phonecodes/phonecodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-09 22:00:47.000000 phonecodes-1.1.1/src/phonecodes/pronlex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:00:57.959832 phonecodes-1.1.1/src/phonecodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-09 22:00:57.000000 phonecodes-1.1.1/src/phonecodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 22:00:57.000000 phonecodes-1.1.1/src/phonecodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:00:57.000000 phonecodes-1.1.1/src/phonecodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 22:00:57.000000 phonecodes-1.1.1/src/phonecodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 22:00:57.000000 phonecodes-1.1.1/src/phonecodes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:00:57.959832 phonecodes-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-09 22:00:47.000000 phonecodes-1.1.1/test/test_phonecodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-09 22:00:47.000000 phonecodes-1.1.1/test/test_pronlex.py
```

### Comparing `phonecodes-1.1.0/LICENSE.txt` & `phonecodes-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phonecodes-1.1.0/PKG-INFO` & `phonecodes-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonecodes
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for loading dictionaries with various phonecodes (IPA, Callhome, X-SAMPA, ARPABET, DISC=CELEX, Buckeye), for converting among those phonecodes, and for searching those dictionaries for word sequences matching a target.
 License: MIT License
         
         Copyright (c) 2024, Virginia Partridge
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,15 +27,15 @@
 Project-URL: Homepage, https://github.com/ginic/phonecodes
 Project-URL: Repository, https://github.com/ginic/phonecodes.git
 Project-URL: Issues, https://github.com/ginic/phonecodes/issues
 Project-URL: Changelog, https://github.com/ginic/phonecodes/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
```

### Comparing `phonecodes-1.1.0/README.md` & `phonecodes-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `phonecodes-1.1.0/pyproject.toml` & `phonecodes-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phonecodes"
-version = "1.1.0"
+version = "1.1.1"
 description = "Tools for loading dictionaries with various phonecodes (IPA, Callhome, X-SAMPA, ARPABET, DISC=CELEX, Buckeye), for converting among those phonecodes, and for searching those dictionaries for word sequences matching a target."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
@@ -24,15 +24,15 @@
 # Extra dependencies only needed for running tests go here
 test = [
     "pytest",
 ]
 
 # Dependencies that are useful only to developers, like an autoformatter and support for visualizations in jupyter notebooks go here
 dev = [
-    "ruff"
+    "ruff",
 ]
 
 [project.urls]
 Homepage = "https://github.com/ginic/phonecodes"
 Repository = "https://github.com/ginic/phonecodes.git"
 Issues = "https://github.com/ginic/phonecodes/issues"
 Changelog = "https://github.com/ginic/phonecodes/blob/master/CHANGELOG.md"
```

### Comparing `phonecodes-1.1.0/src/phonecodes/phonecode_tables.py` & `phonecodes-1.1.1/src/phonecodes/phonecode_tables.py`

 * *Files identical despite different names*

### Comparing `phonecodes-1.1.0/src/phonecodes/phonecodes.py` & `phonecodes-1.1.1/src/phonecodes/phonecodes.py`

 * *Files identical despite different names*

### Comparing `phonecodes-1.1.0/src/phonecodes/pronlex.py` & `phonecodes-1.1.1/src/phonecodes/pronlex.py`

 * *Files identical despite different names*

### Comparing `phonecodes-1.1.0/src/phonecodes.egg-info/PKG-INFO` & `phonecodes-1.1.1/src/phonecodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonecodes
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for loading dictionaries with various phonecodes (IPA, Callhome, X-SAMPA, ARPABET, DISC=CELEX, Buckeye), for converting among those phonecodes, and for searching those dictionaries for word sequences matching a target.
 License: MIT License
         
         Copyright (c) 2024, Virginia Partridge
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,15 +27,15 @@
 Project-URL: Homepage, https://github.com/ginic/phonecodes
 Project-URL: Repository, https://github.com/ginic/phonecodes.git
 Project-URL: Issues, https://github.com/ginic/phonecodes/issues
 Project-URL: Changelog, https://github.com/ginic/phonecodes/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
```

### Comparing `phonecodes-1.1.0/test/test_phonecodes.py` & `phonecodes-1.1.1/test/test_phonecodes.py`

 * *Files identical despite different names*

### Comparing `phonecodes-1.1.0/test/test_pronlex.py` & `phonecodes-1.1.1/test/test_pronlex.py`

 * *Files identical despite different names*

