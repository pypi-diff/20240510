# Comparing `tmp/endiaperz-1.1.tar.gz` & `tmp/endiaperz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endiaperz-1.1.tar", last modified: Wed May  8 13:41:30 2024, max compression
+gzip compressed data, was "endiaperz-2.1.tar", last modified: Fri May 10 19:07:21 2024, max compression
```

## Comparing `endiaperz-1.1.tar` & `endiaperz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:41:30.198329 endiaperz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 13:41:30.198329 endiaperz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:41:30.198329 endiaperz-1.1/endiaperz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:41:30.006326 endiaperz-1.1/endiaperz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:41:30.014326 endiaperz-1.1/endiaperz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 13:41:30.006326 endiaperz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 13:41:30.026326 endiaperz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:07:21.816519 endiaperz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 13:41:30.000000 endiaperz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 19:07:21.816519 endiaperz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 13:41:30.000000 endiaperz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:07:21.812519 endiaperz-2.1/endiaperz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:41:30.000000 endiaperz-2.1/endiaperz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:41:30.000000 endiaperz-2.1/endiaperz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:07:21.812519 endiaperz-2.1/endiaperz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 19:07:21.000000 endiaperz-2.1/endiaperz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-10 19:07:21.000000 endiaperz-2.1/endiaperz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 19:07:21.000000 endiaperz-2.1/endiaperz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 19:07:21.000000 endiaperz-2.1/endiaperz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-10 19:07:21.000000 endiaperz-2.1/endiaperz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 19:07:21.816519 endiaperz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-10 19:07:21.000000 endiaperz-2.1/setup.py
```

### Comparing `endiaperz-1.1/setup.py` & `endiaperz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'endiaperz',
     packages = ['endiaperz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'endiaperz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/endiaperz',
```

