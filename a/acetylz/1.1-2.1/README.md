# Comparing `tmp/acetylz-1.1.tar.gz` & `tmp/acetylz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetylz-1.1.tar", last modified: Wed May  8 22:50:48 2024, max compression
+gzip compressed data, was "acetylz-2.1.tar", last modified: Fri May 10 08:24:46 2024, max compression
```

## Comparing `acetylz-1.1.tar` & `acetylz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:50:48.545277 acetylz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-08 22:50:48.545277 acetylz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:50:48.545277 acetylz-1.1/acetylz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:50:45.473220 acetylz-1.1/acetylz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:50:45.625223 acetylz-1.1/acetylz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 22:50:45.469220 acetylz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-08 22:50:45.853227 acetylz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:24:46.897311 acetylz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 22:50:45.000000 acetylz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-10 08:24:46.897311 acetylz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 22:50:45.000000 acetylz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:24:46.897311 acetylz-2.1/acetylz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:50:45.000000 acetylz-2.1/acetylz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:50:45.000000 acetylz-2.1/acetylz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:24:46.897311 acetylz-2.1/acetylz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-10 08:24:46.000000 acetylz-2.1/acetylz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-10 08:24:46.000000 acetylz-2.1/acetylz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 08:24:46.000000 acetylz-2.1/acetylz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 08:24:46.000000 acetylz-2.1/acetylz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-10 08:24:46.000000 acetylz-2.1/acetylz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 08:24:46.897311 acetylz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-10 08:24:42.000000 acetylz-2.1/setup.py
```

### Comparing `acetylz-1.1/setup.py` & `acetylz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'acetylz',
     packages = ['acetylz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'acetylz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/acetylz',
```

