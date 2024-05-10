# Comparing `tmp/elaborationz-1.1.tar.gz` & `tmp/elaborationz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elaborationz-1.1.tar", last modified: Wed May  8 21:57:16 2024, max compression
+gzip compressed data, was "elaborationz-2.1.tar", last modified: Fri May 10 18:46:35 2024, max compression
```

## Comparing `elaborationz-1.1.tar` & `elaborationz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:57:16.714254 elaborationz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-08 21:57:16.718255 elaborationz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:57:16.714254 elaborationz-1.1/elaborationz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:57:16.542251 elaborationz-1.1/elaborationz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:57:16.554252 elaborationz-1.1/elaborationz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 21:57:16.542251 elaborationz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-08 21:57:16.558252 elaborationz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:46:35.333433 elaborationz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 21:57:16.000000 elaborationz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 18:46:35.333433 elaborationz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 21:57:16.000000 elaborationz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:46:35.261432 elaborationz-2.1/elaborationz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:57:16.000000 elaborationz-2.1/elaborationz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:57:16.000000 elaborationz-2.1/elaborationz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:46:35.333433 elaborationz-2.1/elaborationz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 18:46:33.000000 elaborationz-2.1/elaborationz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-10 18:46:33.000000 elaborationz-2.1/elaborationz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 18:46:33.000000 elaborationz-2.1/elaborationz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 18:46:33.000000 elaborationz-2.1/elaborationz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-10 18:46:33.000000 elaborationz-2.1/elaborationz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 18:46:35.333433 elaborationz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 18:46:19.000000 elaborationz-2.1/setup.py
```

### Comparing `elaborationz-1.1/setup.py` & `elaborationz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'elaborationz',
     packages = ['elaborationz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'elaborationz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/elaborationz',
```

