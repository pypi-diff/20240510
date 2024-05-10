# Comparing `tmp/frangulicz-1.1.tar.gz` & `tmp/frangulicz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frangulicz-1.1.tar", last modified: Thu May  9 01:07:34 2024, max compression
+gzip compressed data, was "frangulicz-2.1.tar", last modified: Fri May 10 21:07:12 2024, max compression
```

## Comparing `frangulicz-1.1.tar` & `frangulicz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:07:34.380594 frangulicz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 01:07:34.380594 frangulicz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:07:34.380594 frangulicz-1.1/frangulicz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:07:30.956531 frangulicz-1.1/frangulicz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:07:31.192535 frangulicz-1.1/frangulicz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 01:07:30.956531 frangulicz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 01:07:31.472540 frangulicz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:07:12.184831 frangulicz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 01:07:30.000000 frangulicz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 21:07:12.184831 frangulicz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 01:07:30.000000 frangulicz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:07:12.180831 frangulicz-2.1/frangulicz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:07:30.000000 frangulicz-2.1/frangulicz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:07:31.000000 frangulicz-2.1/frangulicz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:07:12.184831 frangulicz-2.1/frangulicz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 21:07:12.000000 frangulicz-2.1/frangulicz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 21:07:12.000000 frangulicz-2.1/frangulicz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 21:07:12.000000 frangulicz-2.1/frangulicz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 21:07:12.000000 frangulicz-2.1/frangulicz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 21:07:12.000000 frangulicz-2.1/frangulicz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 21:07:12.184831 frangulicz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 21:07:11.000000 frangulicz-2.1/setup.py
```

### Comparing `frangulicz-1.1/setup.py` & `frangulicz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'frangulicz',
     packages = ['frangulicz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'frangulicz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/frangulicz',
```

