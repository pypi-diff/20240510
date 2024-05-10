# Comparing `tmp/decaspermousz-1.1.tar.gz` & `tmp/decaspermousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decaspermousz-1.1.tar", last modified: Thu May  9 05:01:19 2024, max compression
+gzip compressed data, was "decaspermousz-2.1.tar", last modified: Fri May 10 16:30:48 2024, max compression
```

## Comparing `decaspermousz-1.1.tar` & `decaspermousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:01:19.626192 decaspermousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 05:01:19.626192 decaspermousz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:01:19.626192 decaspermousz-1.1/decaspermousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:01:16.814140 decaspermousz-1.1/decaspermousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:01:17.022144 decaspermousz-1.1/decaspermousz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 05:01:16.814140 decaspermousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 05:01:17.302149 decaspermousz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:30:48.131177 decaspermousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 05:01:16.000000 decaspermousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 16:30:48.131177 decaspermousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 05:01:16.000000 decaspermousz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:30:48.047176 decaspermousz-2.1/decaspermousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:01:16.000000 decaspermousz-2.1/decaspermousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:01:17.000000 decaspermousz-2.1/decaspermousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:30:48.131177 decaspermousz-2.1/decaspermousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 16:30:45.000000 decaspermousz-2.1/decaspermousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-10 16:30:45.000000 decaspermousz-2.1/decaspermousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 16:30:45.000000 decaspermousz-2.1/decaspermousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 16:30:45.000000 decaspermousz-2.1/decaspermousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-10 16:30:45.000000 decaspermousz-2.1/decaspermousz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 16:30:48.131177 decaspermousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 16:30:39.000000 decaspermousz-2.1/setup.py
```

### Comparing `decaspermousz-1.1/setup.py` & `decaspermousz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'decaspermousz',
     packages = ['decaspermousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'decaspermousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/decaspermousz',
```

