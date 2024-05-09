# Comparing `tmp/name_that_fucking_film-0.1.7.tar.gz` & `tmp/name_that_fucking_film-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_that_fucking_film-0.1.7.tar", max compression
+gzip compressed data, was "name_that_fucking_film-0.2.0.tar", max compression
```

## Comparing `name_that_fucking_film-0.1.7.tar` & `name_that_fucking_film-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1804 2024-05-09 19:44:12.204372 name_that_fucking_film-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.7/name_that_fucking_film/__init__.py
--rw-r--r--   0        0        0     8056 2024-05-09 21:49:28.935186 name_that_fucking_film-0.1.7/name_that_fucking_film/main.py
--rw-r--r--   0        0        0      397 2024-05-09 23:00:04.784856 name_that_fucking_film-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1804 2024-05-09 19:44:12.204372 name_that_fucking_film-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.2.0/name_that_fucking_film/__init__.py
+-rw-r--r--   0        0        0     8056 2024-05-09 21:49:28.935186 name_that_fucking_film-0.2.0/name_that_fucking_film/main.py
+-rw-r--r--   0        0        0      397 2024-05-09 23:55:02.817411 name_that_fucking_film-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 name_that_fucking_film-0.2.0/PKG-INFO
```

### Comparing `name_that_fucking_film-0.1.7/README.md` & `name_that_fucking_film-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `name_that_fucking_film-0.1.7/name_that_fucking_film/main.py` & `name_that_fucking_film-0.2.0/name_that_fucking_film/main.py`

 * *Files identical despite different names*

### Comparing `name_that_fucking_film-0.1.7/PKG-INFO` & `name_that_fucking_film-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name-that-fucking-film
-Version: 0.1.7
+Version: 0.2.0
 Summary: 
 Author: jkarenko
 Author-email: juho.karenko@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

