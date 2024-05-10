# Comparing `tmp/cephalalgiaz-1.1.tar.gz` & `tmp/cephalalgiaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cephalalgiaz-1.1.tar", last modified: Wed May  8 17:47:00 2024, max compression
+gzip compressed data, was "cephalalgiaz-2.1.tar", last modified: Fri May 10 13:49:04 2024, max compression
```

## Comparing `cephalalgiaz-1.1.tar` & `cephalalgiaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:47:00.629962 cephalalgiaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-08 17:47:00.629962 cephalalgiaz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:47:00.629962 cephalalgiaz-1.1/cephalalgiaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:47:00.437958 cephalalgiaz-1.1/cephalalgiaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:47:00.445958 cephalalgiaz-1.1/cephalalgiaz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 17:47:00.437958 cephalalgiaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-08 17:47:00.457959 cephalalgiaz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:49:04.800264 cephalalgiaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 17:47:00.000000 cephalalgiaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 13:49:04.800264 cephalalgiaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 17:47:00.000000 cephalalgiaz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:49:04.796264 cephalalgiaz-2.1/cephalalgiaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:47:00.000000 cephalalgiaz-2.1/cephalalgiaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:47:00.000000 cephalalgiaz-2.1/cephalalgiaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:49:04.800264 cephalalgiaz-2.1/cephalalgiaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 13:49:04.000000 cephalalgiaz-2.1/cephalalgiaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-10 13:49:04.000000 cephalalgiaz-2.1/cephalalgiaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 13:49:04.000000 cephalalgiaz-2.1/cephalalgiaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 13:49:04.000000 cephalalgiaz-2.1/cephalalgiaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-10 13:49:04.000000 cephalalgiaz-2.1/cephalalgiaz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 13:49:04.800264 cephalalgiaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 13:49:04.000000 cephalalgiaz-2.1/setup.py
```

### Comparing `cephalalgiaz-1.1/setup.py` & `cephalalgiaz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'cephalalgiaz',
     packages = ['cephalalgiaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'cephalalgiaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/cephalalgiaz',
```

