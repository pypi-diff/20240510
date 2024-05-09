# Comparing `tmp/name_that_fucking_film-0.1.5.tar.gz` & `tmp/name_that_fucking_film-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_that_fucking_film-0.1.5.tar", max compression
+gzip compressed data, was "name_that_fucking_film-0.1.6.tar", max compression
```

## Comparing `name_that_fucking_film-0.1.5.tar` & `name_that_fucking_film-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1830 2024-05-09 19:42:12.954240 name_that_fucking_film-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.5/name_that_fucking_film/__init__.py
--rw-r--r--   0        0        0     6833 2024-05-09 19:34:21.600252 name_that_fucking_film-0.1.5/name_that_fucking_film/main.py
--rw-r--r--   0        0        0      397 2024-05-09 19:42:28.191658 name_that_fucking_film-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1804 2024-05-09 19:44:12.204372 name_that_fucking_film-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.6/name_that_fucking_film/__init__.py
+-rw-r--r--   0        0        0     6833 2024-05-09 19:34:21.600252 name_that_fucking_film-0.1.6/name_that_fucking_film/main.py
+-rw-r--r--   0        0        0      397 2024-05-09 19:44:16.794377 name_that_fucking_film-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.6/PKG-INFO
```

### Comparing `name_that_fucking_film-0.1.5/README.md` & `name_that_fucking_film-0.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Clone the repository
 git clone https://github.com/jkarenko/name-that-fucking-film.git
 cd name-that-fucking-film
 
 # Install dependencies using Poetry
 poetry install
 
-# Enter the virtual environment
+# run
 poetry run python name_that_fucking_film/main.py {path_to_dir_containing_resources}
 ```
 
 Or using PIP
 ```bash
 # Install from PyPI
 pip install name-that-fucking-film
```

### Comparing `name_that_fucking_film-0.1.5/name_that_fucking_film/main.py` & `name_that_fucking_film-0.1.6/name_that_fucking_film/main.py`

 * *Files identical despite different names*

### Comparing `name_that_fucking_film-0.1.5/PKG-INFO` & `name_that_fucking_film-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name-that-fucking-film
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: jkarenko
 Author-email: juho.karenko@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -35,15 +35,15 @@
 # Clone the repository
 git clone https://github.com/jkarenko/name-that-fucking-film.git
 cd name-that-fucking-film
 
 # Install dependencies using Poetry
 poetry install
 
-# Enter the virtual environment
+# run
 poetry run python name_that_fucking_film/main.py {path_to_dir_containing_resources}
 ```
 
 Or using PIP
 ```bash
 # Install from PyPI
 pip install name-that-fucking-film
```

