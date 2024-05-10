# Comparing `tmp/adlike-0.0.3.tar.gz` & `tmp/adlike-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adlike-0.0.3.tar", last modified: Wed May  8 13:43:38 2024, max compression
+gzip compressed data, was "adlike-0.0.4.tar", last modified: Fri May 10 15:11:23 2024, max compression
```

## Comparing `adlike-0.0.3.tar` & `adlike-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:43:38.873320 adlike-0.0.3/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)     1123 2024-05-08 13:43:38.872464 adlike-0.0.3/PKG-INFO
--rw-r--r--   0 reeteshmukul   (501) staff       (20)      605 2024-05-08 13:42:38.000000 adlike-0.0.3/README.md
--rw-r--r--   0 reeteshmukul   (501) staff       (20)      609 2024-05-08 13:43:30.000000 adlike-0.0.3/pyproject.toml
--rw-r--r--   0 reeteshmukul   (501) staff       (20)       38 2024-05-08 13:43:38.873431 adlike-0.0.3/setup.cfg
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:43:38.867948 adlike-0.0.3/src/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)        0 2024-04-17 12:03:13.000000 adlike-0.0.3/src/__init__.py
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:43:38.869071 adlike-0.0.3/src/adlike/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)       21 2024-04-17 12:03:08.000000 adlike-0.0.3/src/adlike/__init__.py
--rw-r--r--   0 reeteshmukul   (501) staff       (20)     4583 2024-04-25 09:07:37.000000 adlike-0.0.3/src/adlike/adlike.py
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:43:38.871715 adlike-0.0.3/src/adlike.egg-info/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)     1123 2024-05-08 13:43:38.000000 adlike-0.0.3/src/adlike.egg-info/PKG-INFO
--rw-r--r--   0 reeteshmukul   (501) staff       (20)      220 2024-05-08 13:43:38.000000 adlike-0.0.3/src/adlike.egg-info/SOURCES.txt
--rw-r--r--   0 reeteshmukul   (501) staff       (20)        1 2024-05-08 13:43:38.000000 adlike-0.0.3/src/adlike.egg-info/dependency_links.txt
--rw-r--r--   0 reeteshmukul   (501) staff       (20)       16 2024-05-08 13:43:38.000000 adlike-0.0.3/src/adlike.egg-info/top_level.txt
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-10 15:11:23.181929 adlike-0.0.4/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)     1123 2024-05-10 15:11:23.181508 adlike-0.0.4/PKG-INFO
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)      605 2024-05-08 13:42:38.000000 adlike-0.0.4/README.md
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)      610 2024-05-10 15:10:56.000000 adlike-0.0.4/pyproject.toml
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)       38 2024-05-10 15:11:23.182020 adlike-0.0.4/setup.cfg
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-10 15:11:23.176987 adlike-0.0.4/src/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)        0 2024-04-17 12:03:13.000000 adlike-0.0.4/src/__init__.py
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-10 15:11:23.178535 adlike-0.0.4/src/adlike/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)       21 2024-04-17 12:03:08.000000 adlike-0.0.4/src/adlike/__init__.py
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)     4583 2024-04-25 09:07:37.000000 adlike-0.0.4/src/adlike/adlike.py
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-10 15:11:23.181088 adlike-0.0.4/src/adlike.egg-info/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)     1123 2024-05-10 15:11:23.000000 adlike-0.0.4/src/adlike.egg-info/PKG-INFO
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)      220 2024-05-10 15:11:23.000000 adlike-0.0.4/src/adlike.egg-info/SOURCES.txt
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)        1 2024-05-10 15:11:23.000000 adlike-0.0.4/src/adlike.egg-info/dependency_links.txt
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)       16 2024-05-10 15:11:23.000000 adlike-0.0.4/src/adlike.egg-info/top_level.txt
```

### Comparing `adlike-0.0.3/PKG-INFO` & `adlike-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlike
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package to determine if an Image is an Advertisement
 Author-email: Chitra Vyanjan <chitra.vyanjan@gmail.com>
 Project-URL: Homepage, https://github.com/chitravyanjan/adlike
 Project-URL: Issues, https://github.com/chitravyanjan/adlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `adlike-0.0.3/README.md` & `adlike-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `adlike-0.0.3/pyproject.toml` & `adlike-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adlike"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Chitra Vyanjan", email="chitra.vyanjan@gmail.com" },
 ]
 description = "A python package to determine if an Image is an Advertisement"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/chitravyanjan/adlike"
-Issues = "https://github.com/chitravyanjan/adlike/issues"
+Issues = "https://github.com/chitravyanjan/adlike/issues"
```

### Comparing `adlike-0.0.3/src/adlike/adlike.py` & `adlike-0.0.4/src/adlike/adlike.py`

 * *Files identical despite different names*

### Comparing `adlike-0.0.3/src/adlike.egg-info/PKG-INFO` & `adlike-0.0.4/src/adlike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlike
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package to determine if an Image is an Advertisement
 Author-email: Chitra Vyanjan <chitra.vyanjan@gmail.com>
 Project-URL: Homepage, https://github.com/chitravyanjan/adlike
 Project-URL: Issues, https://github.com/chitravyanjan/adlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

