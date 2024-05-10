# Comparing `tmp/semantra-0.1.8.tar.gz` & `tmp/semantra-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.1.8.tar", last modified: Sat Dec 16 15:55:15 2023, max compression
+gzip compressed data, was "semantra-0.1.9.tar", last modified: Tue May  7 15:37:26 2024, max compression
```

## Comparing `semantra-0.1.8.tar` & `semantra-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,20 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.971054 semantra-0.1.8/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.8/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)    11455 2023-12-16 15:55:15.970661 semantra-0.1.8/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)    10571 2023-12-16 15:52:50.000000 semantra-0.1.8/README.md
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.957539 semantra-0.1.8/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.959253 semantra-0.1.8/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.961671 semantra-0.1.8/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-07-08 13:57:37.000000 semantra-0.1.8/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-07-08 13:57:37.000000 semantra-0.1.8/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-07-08 13:57:37.000000 semantra-0.1.8/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.8/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.8/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.8/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-12-16 15:48:28.000000 semantra-0.1.8/pyproject.toml
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-12-16 15:55:15.971126 semantra-0.1.8/setup.cfg
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.957806 semantra-0.1.8/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.965267 semantra-0.1.8/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.8/src/semantra/__init__.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.967647 semantra-0.1.8/src/semantra/__pycache__/
--rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.8/src/semantra/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    11287 2023-07-08 14:51:10.000000 semantra-0.1.8/src/semantra/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     3164 2023-07-08 14:02:14.000000 semantra-0.1.8/src/semantra/__pycache__/pdf.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    20095 2023-07-08 14:51:10.000000 semantra-0.1.8/src/semantra/__pycache__/semantra.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-07-08 14:02:14.000000 semantra-0.1.8/src/semantra/__pycache__/util.cpython-39.pyc
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.968165 semantra-0.1.8/src/semantra/client_public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.968792 semantra-0.1.8/src/semantra/client_public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-07-08 13:57:37.000000 semantra-0.1.8/src/semantra/client_public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-07-08 13:57:37.000000 semantra-0.1.8/src/semantra/client_public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-07-08 13:57:37.000000 semantra-0.1.8/src/semantra/client_public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.8/src/semantra/client_public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.8/src/semantra/client_public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.8/src/semantra/client_public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)    11577 2023-07-08 14:49:47.000000 semantra-0.1.8/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-07-08 13:57:37.000000 semantra-0.1.8/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    29845 2023-12-16 15:52:50.000000 semantra-0.1.8/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-07-08 13:57:37.000000 semantra-0.1.8/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-12-16 15:55:15.970266 semantra-0.1.8/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)    11455 2023-12-16 15:55:15.000000 semantra-0.1.8/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-12-16 15:55:15.000000 semantra-0.1.8/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-12-16 15:55:15.000000 semantra-0.1.8/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-12-16 15:55:15.000000 semantra-0.1.8/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-12-16 15:55:15.000000 semantra-0.1.8/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-12-16 15:55:15.000000 semantra-0.1.8/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2024-05-07 15:37:26.816518 semantra-0.1.9/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2024-05-07 15:14:15.000000 semantra-0.1.9/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)    11614 2024-05-07 15:37:26.816090 semantra-0.1.9/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)    10704 2024-05-07 15:33:30.000000 semantra-0.1.9/README.md
+-rw-r--r--   0 freedmand   (501) staff       (20)     1036 2024-05-07 15:32:05.000000 semantra-0.1.9/pyproject.toml
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2024-05-07 15:37:26.816579 semantra-0.1.9/setup.cfg
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2024-05-07 15:37:26.812174 semantra-0.1.9/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2024-05-07 15:37:26.813754 semantra-0.1.9/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2024-05-07 15:14:15.000000 semantra-0.1.9/src/semantra/__init__.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    11577 2024-05-07 15:14:15.000000 semantra-0.1.9/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3325 2024-05-07 15:14:15.000000 semantra-0.1.9/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    29845 2024-05-07 15:14:15.000000 semantra-0.1.9/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2024-05-07 15:14:15.000000 semantra-0.1.9/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2024-05-07 15:37:26.815677 semantra-0.1.9/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)    11614 2024-05-07 15:37:26.000000 semantra-0.1.9/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)      364 2024-05-07 15:37:26.000000 semantra-0.1.9/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2024-05-07 15:37:26.000000 semantra-0.1.9/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2024-05-07 15:37:26.000000 semantra-0.1.9/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      187 2024-05-07 15:37:26.000000 semantra-0.1.9/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2024-05-07 15:37:26.000000 semantra-0.1.9/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.1.8/LICENSE` & `semantra-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.1.8/PKG-INFO` & `semantra-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.8
+Version: 0.1.9
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Requires-Dist: Pillow>=9.5.0
 Requires-Dist: pypdfium2>=4.5.0
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: tiktoken>=0.3.3
 Requires-Dist: torch>=2.0.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: transformers>=4.27.4
+Requires-Dist: setuptools
 
 # Semantra
 
 https://user-images.githubusercontent.com/306095/233867821-601db8b0-19c6-4bae-8e93-720b324dc199.mov
 
 Semantra is a multipurpose tool for semantically searching documents. Query by meaning rather than just by matching text.
 
@@ -46,14 +47,21 @@
 
 Ensure you have [Python >= 3.9](https://www.python.org/downloads/).
 
 The easiest way to install Semantra is via `pipx`. If you do not have `pipx` installed, run:
 
 ```sh
 python3 -m pip install --user pipx
+```
+
+Or, if you have [Homebrew](https://brew.sh/) installed, you can run `brew install pipx`.
+
+Once `pipx` is installed, run:
+
+```sh
 python3 -m pipx ensurepath
 ```
 
 Open a new terminal window for the new path settings `pipx` sets to go into effect. Then run:
 
 ```sh
 pipx install semantra
```

### Comparing `semantra-0.1.8/README.md` & `semantra-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 
 Ensure you have [Python >= 3.9](https://www.python.org/downloads/).
 
 The easiest way to install Semantra is via `pipx`. If you do not have `pipx` installed, run:
 
 ```sh
 python3 -m pip install --user pipx
+```
+
+Or, if you have [Homebrew](https://brew.sh/) installed, you can run `brew install pipx`.
+
+Once `pipx` is installed, run:
+
+```sh
 python3 -m pipx ensurepath
 ```
 
 Open a new terminal window for the new path settings `pipx` sets to go into effect. Then run:
 
 ```sh
 pipx install semantra
```

### Comparing `semantra-0.1.8/pyproject.toml` & `semantra-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantra"
-version = "0.1.8"
+version = "0.1.9"
 description = "A semantic search CLI tool"
 authors = [{name = "Dylan Freedman", email = "freedmand@gmail.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -20,15 +20,16 @@
   "openai>=0.27.2",
   "Pillow>=9.5.0",
   "pypdfium2>=4.5.0",
   "python-dotenv>=1.0.0",
   "tiktoken>=0.3.3",
   "torch>=2.0.0",
   "tqdm>=4.65.0",
-  "transformers>=4.27.4"
+  "transformers>=4.27.4",
+  "setuptools"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/freedmand/semantra"
 "Repository" = "https://github.com/freedmand/semantra"
 "Bug Tracker" = "https://github.com/freedmand/semantra/issues"
```

### Comparing `semantra-0.1.8/src/semantra/models.py` & `semantra-0.1.9/src/semantra/models.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.8/src/semantra/pdf.py` & `semantra-0.1.9/src/semantra/pdf.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.8/src/semantra/semantra.py` & `semantra-0.1.9/src/semantra/semantra.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.8/src/semantra/util.py` & `semantra-0.1.9/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.8/src/semantra.egg-info/PKG-INFO` & `semantra-0.1.9/src/semantra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.8
+Version: 0.1.9
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Requires-Dist: Pillow>=9.5.0
 Requires-Dist: pypdfium2>=4.5.0
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: tiktoken>=0.3.3
 Requires-Dist: torch>=2.0.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: transformers>=4.27.4
+Requires-Dist: setuptools
 
 # Semantra
 
 https://user-images.githubusercontent.com/306095/233867821-601db8b0-19c6-4bae-8e93-720b324dc199.mov
 
 Semantra is a multipurpose tool for semantically searching documents. Query by meaning rather than just by matching text.
 
@@ -46,14 +47,21 @@
 
 Ensure you have [Python >= 3.9](https://www.python.org/downloads/).
 
 The easiest way to install Semantra is via `pipx`. If you do not have `pipx` installed, run:
 
 ```sh
 python3 -m pip install --user pipx
+```
+
+Or, if you have [Homebrew](https://brew.sh/) installed, you can run `brew install pipx`.
+
+Once `pipx` is installed, run:
+
+```sh
 python3 -m pipx ensurepath
 ```
 
 Open a new terminal window for the new path settings `pipx` sets to go into effect. Then run:
 
 ```sh
 pipx install semantra
```

