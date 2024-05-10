# Comparing `tmp/elhiz-1.1.tar.gz` & `tmp/elhiz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elhiz-1.1.tar", last modified: Wed May  8 18:51:56 2024, max compression
+gzip compressed data, was "elhiz-2.1.tar", last modified: Fri May 10 18:56:54 2024, max compression
```

## Comparing `elhiz-1.1.tar` & `elhiz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:51:56.257604 elhiz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1636 2024-05-08 18:51:56.257604 elhiz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:51:56.257604 elhiz-1.1/elhiz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:51:56.073601 elhiz-1.1/elhiz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:51:56.081601 elhiz-1.1/elhiz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 18:51:56.073601 elhiz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-08 18:51:56.089601 elhiz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:56:54.852921 elhiz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 18:51:56.000000 elhiz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-10 18:56:54.852921 elhiz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 18:51:56.000000 elhiz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:56:54.852921 elhiz-2.1/elhiz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:51:56.000000 elhiz-2.1/elhiz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:51:56.000000 elhiz-2.1/elhiz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:56:54.852921 elhiz-2.1/elhiz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-10 18:56:54.000000 elhiz-2.1/elhiz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      212 2024-05-10 18:56:54.000000 elhiz-2.1/elhiz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 18:56:54.000000 elhiz-2.1/elhiz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 18:56:54.000000 elhiz-2.1/elhiz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        6 2024-05-10 18:56:54.000000 elhiz-2.1/elhiz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 18:56:54.852921 elhiz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-10 18:56:54.000000 elhiz-2.1/setup.py
```

### Comparing `elhiz-1.1/setup.py` & `elhiz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'elhiz',
     packages = ['elhiz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'elhiz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/elhiz',
```

