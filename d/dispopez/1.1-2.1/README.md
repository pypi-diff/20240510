# Comparing `tmp/dispopez-1.1.tar.gz` & `tmp/dispopez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispopez-1.1.tar", last modified: Wed May  8 20:47:32 2024, max compression
+gzip compressed data, was "dispopez-2.1.tar", last modified: Fri May 10 18:05:05 2024, max compression
```

## Comparing `dispopez-1.1.tar` & `dispopez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 20:47:32.225471 dispopez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-08 20:47:32.225471 dispopez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 20:47:32.225471 dispopez-1.1/dispopez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 20:47:31.069450 dispopez-1.1/dispopez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 20:47:31.257454 dispopez-1.1/dispopez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 20:47:31.069450 dispopez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-08 20:47:31.493458 dispopez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:05:05.575356 dispopez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 20:47:31.000000 dispopez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 18:05:05.575356 dispopez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 20:47:31.000000 dispopez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:05:05.571356 dispopez-2.1/dispopez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 20:47:31.000000 dispopez-2.1/dispopez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 20:47:31.000000 dispopez-2.1/dispopez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:05:05.575356 dispopez-2.1/dispopez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 18:05:05.000000 dispopez-2.1/dispopez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 18:05:05.000000 dispopez-2.1/dispopez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 18:05:05.000000 dispopez-2.1/dispopez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 18:05:05.000000 dispopez-2.1/dispopez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 18:05:05.000000 dispopez-2.1/dispopez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 18:05:05.575356 dispopez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 18:05:05.000000 dispopez-2.1/setup.py
```

### Comparing `dispopez-1.1/setup.py` & `dispopez-2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'dispopez',
     packages = ['dispopez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'dispopez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/dispopez',
```

