# Comparing `tmp/fluez-1.1.tar.gz` & `tmp/fluez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluez-1.1.tar", last modified: Thu May  9 19:53:43 2024, max compression
+gzip compressed data, was "fluez-2.1.tar", last modified: Fri May 10 20:56:41 2024, max compression
```

## Comparing `fluez-1.1.tar` & `fluez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:53:43.584482 fluez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1636 2024-05-09 19:53:43.584482 fluez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:53:43.584482 fluez-1.1/fluez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:53:40.464424 fluez-1.1/fluez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:53:40.648428 fluez-1.1/fluez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 19:53:40.464424 fluez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-09 19:53:40.936433 fluez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:56:41.821270 fluez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 19:53:40.000000 fluez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-10 20:56:41.821270 fluez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 19:53:40.000000 fluez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:56:41.821270 fluez-2.1/fluez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:53:40.000000 fluez-2.1/fluez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:53:40.000000 fluez-2.1/fluez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:56:41.821270 fluez-2.1/fluez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-10 20:56:40.000000 fluez-2.1/fluez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      212 2024-05-10 20:56:40.000000 fluez-2.1/fluez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 20:56:40.000000 fluez-2.1/fluez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 20:56:40.000000 fluez-2.1/fluez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        6 2024-05-10 20:56:40.000000 fluez-2.1/fluez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 20:56:41.825271 fluez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-10 20:56:35.000000 fluez-2.1/setup.py
```

### Comparing `fluez-1.1/setup.py` & `fluez-2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'fluez',
     packages = ['fluez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'fluez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/fluez',
```

