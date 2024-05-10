# Comparing `tmp/crinivorousz-1.1.tar.gz` & `tmp/crinivorousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crinivorousz-1.1.tar", last modified: Wed May  8 21:09:14 2024, max compression
+gzip compressed data, was "crinivorousz-2.1.tar", last modified: Fri May 10 15:27:48 2024, max compression
```

## Comparing `crinivorousz-1.1.tar` & `crinivorousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:09:14.617235 crinivorousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-08 21:09:14.617235 crinivorousz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:09:14.617235 crinivorousz-1.1/crinivorousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:09:14.441232 crinivorousz-1.1/crinivorousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:09:14.445232 crinivorousz-1.1/crinivorousz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 21:09:14.441232 crinivorousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-08 21:09:14.457232 crinivorousz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:27:48.509329 crinivorousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 21:09:14.000000 crinivorousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 15:27:48.509329 crinivorousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 21:09:14.000000 crinivorousz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:27:48.505329 crinivorousz-2.1/crinivorousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:09:14.000000 crinivorousz-2.1/crinivorousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:09:14.000000 crinivorousz-2.1/crinivorousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:27:48.509329 crinivorousz-2.1/crinivorousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 15:27:47.000000 crinivorousz-2.1/crinivorousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-10 15:27:47.000000 crinivorousz-2.1/crinivorousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 15:27:47.000000 crinivorousz-2.1/crinivorousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 15:27:47.000000 crinivorousz-2.1/crinivorousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-10 15:27:47.000000 crinivorousz-2.1/crinivorousz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 15:27:48.509329 crinivorousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 15:27:43.000000 crinivorousz-2.1/setup.py
```

### Comparing `crinivorousz-1.1/setup.py` & `crinivorousz-2.1/setup.py`

 * *Files identical despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'crinivorousz',
     packages = ['crinivorousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'crinivorousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/crinivorousz',
```

