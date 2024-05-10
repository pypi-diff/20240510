# Comparing `tmp/aerogenesisz-1.1.tar.gz` & `tmp/aerogenesisz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerogenesisz-1.1.tar", last modified: Wed May  8 16:57:12 2024, max compression
+gzip compressed data, was "aerogenesisz-2.1.tar", last modified: Fri May 10 08:35:00 2024, max compression
```

## Comparing `aerogenesisz-1.1.tar` & `aerogenesisz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:57:12.366984 aerogenesisz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-08 16:57:12.366984 aerogenesisz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:57:12.366984 aerogenesisz-1.1/aerogenesisz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:57:11.702971 aerogenesisz-1.1/aerogenesisz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:57:11.810973 aerogenesisz-1.1/aerogenesisz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:57:11.702971 aerogenesisz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-08 16:57:11.990977 aerogenesisz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:35:00.080606 aerogenesisz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:57:11.000000 aerogenesisz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 08:35:00.080606 aerogenesisz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:57:11.000000 aerogenesisz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:35:00.076606 aerogenesisz-2.1/aerogenesisz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:57:11.000000 aerogenesisz-2.1/aerogenesisz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:57:11.000000 aerogenesisz-2.1/aerogenesisz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:35:00.080606 aerogenesisz-2.1/aerogenesisz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 08:34:59.000000 aerogenesisz-2.1/aerogenesisz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-10 08:34:59.000000 aerogenesisz-2.1/aerogenesisz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 08:34:59.000000 aerogenesisz-2.1/aerogenesisz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 08:34:59.000000 aerogenesisz-2.1/aerogenesisz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-10 08:34:59.000000 aerogenesisz-2.1/aerogenesisz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 08:35:00.080606 aerogenesisz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 08:34:57.000000 aerogenesisz-2.1/setup.py
```

### Comparing `aerogenesisz-1.1/setup.py` & `aerogenesisz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'aerogenesisz',
     packages = ['aerogenesisz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'aerogenesisz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/aerogenesisz',
```

