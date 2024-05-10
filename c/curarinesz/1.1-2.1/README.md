# Comparing `tmp/curarinesz-1.1.tar.gz` & `tmp/curarinesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curarinesz-1.1.tar", last modified: Thu May  9 15:34:56 2024, max compression
+gzip compressed data, was "curarinesz-2.1.tar", last modified: Fri May 10 15:43:37 2024, max compression
```

## Comparing `curarinesz-1.1.tar` & `curarinesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:34:56.198110 curarinesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 15:34:56.202110 curarinesz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:34:56.198110 curarinesz-1.1/curarinesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:34:53.638063 curarinesz-1.1/curarinesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:34:53.834067 curarinesz-1.1/curarinesz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 15:34:53.638063 curarinesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 15:34:54.138072 curarinesz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:43:37.494855 curarinesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 15:34:53.000000 curarinesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 15:43:37.494855 curarinesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 15:34:53.000000 curarinesz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:43:37.494855 curarinesz-2.1/curarinesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:34:53.000000 curarinesz-2.1/curarinesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:34:53.000000 curarinesz-2.1/curarinesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:43:37.494855 curarinesz-2.1/curarinesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 15:43:36.000000 curarinesz-2.1/curarinesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 15:43:36.000000 curarinesz-2.1/curarinesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 15:43:36.000000 curarinesz-2.1/curarinesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 15:43:36.000000 curarinesz-2.1/curarinesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 15:43:36.000000 curarinesz-2.1/curarinesz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 15:43:37.494855 curarinesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 15:43:30.000000 curarinesz-2.1/setup.py
```

### Comparing `curarinesz-1.1/setup.py` & `curarinesz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'curarinesz',
     packages = ['curarinesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'curarinesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/curarinesz',
```

