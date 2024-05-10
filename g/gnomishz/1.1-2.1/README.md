# Comparing `tmp/gnomishz-1.1.tar.gz` & `tmp/gnomishz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnomishz-1.1.tar", last modified: Wed May  8 17:41:45 2024, max compression
+gzip compressed data, was "gnomishz-2.1.tar", last modified: Fri May 10 21:54:16 2024, max compression
```

## Comparing `gnomishz-1.1.tar` & `gnomishz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:41:45.664164 gnomishz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-08 17:41:45.664164 gnomishz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:41:45.664164 gnomishz-1.1/gnomishz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:41:45.468161 gnomishz-1.1/gnomishz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:41:45.476161 gnomishz-1.1/gnomishz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 17:41:45.468161 gnomishz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-08 17:41:45.484161 gnomishz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:54:16.672793 gnomishz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 17:41:45.000000 gnomishz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 21:54:16.672793 gnomishz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 17:41:45.000000 gnomishz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:54:16.672793 gnomishz-2.1/gnomishz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:41:45.000000 gnomishz-2.1/gnomishz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:41:45.000000 gnomishz-2.1/gnomishz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:54:16.672793 gnomishz-2.1/gnomishz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 21:54:15.000000 gnomishz-2.1/gnomishz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 21:54:15.000000 gnomishz-2.1/gnomishz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 21:54:15.000000 gnomishz-2.1/gnomishz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 21:54:15.000000 gnomishz-2.1/gnomishz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 21:54:15.000000 gnomishz-2.1/gnomishz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 21:54:16.672793 gnomishz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 21:54:10.000000 gnomishz-2.1/setup.py
```

### Comparing `gnomishz-1.1/setup.py` & `gnomishz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'gnomishz',
     packages = ['gnomishz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'gnomishz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/gnomishz',
```

