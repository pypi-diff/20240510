# Comparing `tmp/demephitizez-1.1.tar.gz` & `tmp/demephitizez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demephitizez-1.1.tar", last modified: Wed May  8 16:46:35 2024, max compression
+gzip compressed data, was "demephitizez-2.1.tar", last modified: Fri May 10 16:41:20 2024, max compression
```

## Comparing `demephitizez-1.1.tar` & `demephitizez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:46:35.207129 demephitizez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-08 16:46:35.207129 demephitizez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:46:35.207129 demephitizez-1.1/demephitizez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:46:34.999126 demephitizez-1.1/demephitizez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:46:35.007126 demephitizez-1.1/demephitizez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:46:34.999126 demephitizez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-08 16:46:35.019126 demephitizez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:41:20.270872 demephitizez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:46:34.000000 demephitizez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 16:41:20.270872 demephitizez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:46:34.000000 demephitizez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:41:20.266872 demephitizez-2.1/demephitizez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:46:34.000000 demephitizez-2.1/demephitizez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:46:35.000000 demephitizez-2.1/demephitizez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:41:20.270872 demephitizez-2.1/demephitizez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 16:41:20.000000 demephitizez-2.1/demephitizez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-10 16:41:20.000000 demephitizez-2.1/demephitizez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 16:41:20.000000 demephitizez-2.1/demephitizez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 16:41:20.000000 demephitizez-2.1/demephitizez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-10 16:41:20.000000 demephitizez-2.1/demephitizez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 16:41:20.270872 demephitizez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 16:41:19.000000 demephitizez-2.1/setup.py
```

### Comparing `demephitizez-1.1/setup.py` & `demephitizez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'demephitizez',
     packages = ['demephitizez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'demephitizez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/demephitizez',
```

