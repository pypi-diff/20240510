# Comparing `tmp/iccore-0.0.1.tar.gz` & `tmp/iccore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iccore-0.0.1.tar", last modified: Fri May  3 10:13:42 2024, max compression
+gzip compressed data, was "iccore-0.0.2.tar", last modified: Fri May 10 11:14:11 2024, max compression
```

## Comparing `iccore-0.0.1.tar` & `iccore-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 10:13:42.963273 iccore-0.0.1/
--rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-05-03 09:50:02.000000 iccore-0.0.1/LICENSE.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)     1079 2024-05-03 10:13:42.963140 iccore-0.0.1/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)      110 2024-05-03 09:50:02.000000 iccore-0.0.1/README.md
--rw-r--r--   0 jgrogan    (503) staff       (20)     1785 2024-05-03 09:50:02.000000 iccore-0.0.1/pyproject.toml
--rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-03 10:13:42.964557 iccore-0.0.1/setup.cfg
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 10:13:42.942206 iccore-0.0.1/src/
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 10:13:42.945284 iccore-0.0.1/src/iccore/
--rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-03 09:50:02.000000 iccore-0.0.1/src/iccore/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      424 2024-05-03 10:12:40.000000 iccore-0.0.1/src/iccore/filesystem.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      313 2024-05-03 10:12:40.000000 iccore-0.0.1/src/iccore/logging_utils.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      381 2024-05-03 10:12:40.000000 iccore-0.0.1/src/iccore/process.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      197 2024-05-03 10:12:40.000000 iccore-0.0.1/src/iccore/runtime.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      126 2024-05-03 10:12:40.000000 iccore-0.0.1/src/iccore/time_utils.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 10:13:42.962292 iccore-0.0.1/src/iccore.egg-info/
--rw-r--r--   0 jgrogan    (503) staff       (20)     1079 2024-05-03 10:13:42.000000 iccore-0.0.1/src/iccore.egg-info/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)      380 2024-05-03 10:13:42.000000 iccore-0.0.1/src/iccore.egg-info/SOURCES.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-03 10:13:42.000000 iccore-0.0.1/src/iccore.egg-info/dependency_links.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)       50 2024-05-03 10:13:42.000000 iccore-0.0.1/src/iccore.egg-info/requires.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)        7 2024-05-03 10:13:42.000000 iccore-0.0.1/src/iccore.egg-info/top_level.txt
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 10:13:42.961744 iccore-0.0.1/test/
--rw-r--r--   0 jgrogan    (503) staff       (20)       44 2024-05-03 09:50:02.000000 iccore-0.0.1/test/test_iccore.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:14:11.935123 iccore-0.0.2/
+-rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-05-03 09:50:02.000000 iccore-0.0.2/LICENSE.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1090 2024-05-10 11:14:11.934968 iccore-0.0.2/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)      110 2024-05-03 09:50:02.000000 iccore-0.0.2/README.md
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1894 2024-05-10 11:12:19.000000 iccore-0.0.2/pyproject.toml
+-rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-10 11:14:11.936154 iccore-0.0.2/setup.cfg
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:14:11.868884 iccore-0.0.2/src/
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:14:11.876945 iccore-0.0.2/src/iccore/
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-03 09:50:02.000000 iccore-0.0.2/src/iccore/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      424 2024-05-03 10:12:40.000000 iccore-0.0.2/src/iccore/filesystem.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      332 2024-05-03 12:18:56.000000 iccore-0.0.2/src/iccore/logging_utils.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      381 2024-05-03 10:27:20.000000 iccore-0.0.2/src/iccore/process.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:11:07.000000 iccore-0.0.2/src/iccore/py.typed
+-rw-r--r--   0 jgrogan    (503) staff       (20)      197 2024-05-03 10:12:40.000000 iccore-0.0.2/src/iccore/runtime.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      126 2024-05-03 10:12:40.000000 iccore-0.0.2/src/iccore/time_utils.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:14:11.933982 iccore-0.0.2/src/iccore.egg-info/
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1090 2024-05-10 11:14:11.000000 iccore-0.0.2/src/iccore.egg-info/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)      400 2024-05-10 11:14:11.000000 iccore-0.0.2/src/iccore.egg-info/SOURCES.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-10 11:14:11.000000 iccore-0.0.2/src/iccore.egg-info/dependency_links.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)       50 2024-05-10 11:14:11.000000 iccore-0.0.2/src/iccore.egg-info/requires.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)        7 2024-05-10 11:14:11.000000 iccore-0.0.2/src/iccore.egg-info/top_level.txt
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:14:11.933467 iccore-0.0.2/test/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       44 2024-05-03 09:50:02.000000 iccore-0.0.2/test/test_iccore.py
```

### Comparing `iccore-0.0.1/LICENSE.txt` & `iccore-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iccore-0.0.1/PKG-INFO` & `iccore-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: iccore
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of common data structures and utilities used in other ICHEC tools
 Author-email: "James Grogan, Irish Centre for High End Computing" <james.grogan@ichec.ie>
 Project-URL: Repository, https://git.ichec.ie/performance/toolshed/iccore
 Project-URL: Homepage, https://git.ichec.ie/performance/toolshed/iccore
 Keywords: HPC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `iccore-0.0.1/pyproject.toml` & `iccore-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "iccore"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="James Grogan, Irish Centre for High End Computing", email="james.grogan@ichec.ie" },
 ]
 description = "A collection of common data structures and utilities used in other ICHEC tools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Topic :: System :: Distributed Computing"
 ]
 keywords = ["HPC"]
 
 [project.urls]
 Repository = "https://git.ichec.ie/performance/toolshed/iccore"
@@ -29,14 +29,20 @@
     "pytest",
     "pytest-cov",
     "pytest-sugar",
     "black",
     "mypy"
 ]
 
+[tool.setuptools.package-data]
+"iccore" = ["py.typed"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 testpaths = ["test",]
 log_cli = 1
 log_cli_level = "debug"
@@ -57,15 +63,15 @@
 commands =
     pytest {posargs:test}
 
 [testenv:lint]
 description = run linters
 skip_install = true
 deps =
-    black==22.12
+    black
 commands = black {posargs:src}
 
 [testenv:style]
 description = run style check
 skip_install = true
 deps =
     flake8
```

### Comparing `iccore-0.0.1/src/iccore.egg-info/PKG-INFO` & `iccore-0.0.2/src/iccore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: iccore
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of common data structures and utilities used in other ICHEC tools
 Author-email: "James Grogan, Irish Centre for High End Computing" <james.grogan@ichec.ie>
 Project-URL: Repository, https://git.ichec.ie/performance/toolshed/iccore
 Project-URL: Homepage, https://git.ichec.ie/performance/toolshed/iccore
 Keywords: HPC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

