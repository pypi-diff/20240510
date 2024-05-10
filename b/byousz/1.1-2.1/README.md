# Comparing `tmp/byousz-1.1.tar.gz` & `tmp/byousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byousz-1.1.tar", last modified: Wed May  8 23:56:40 2024, max compression
+gzip compressed data, was "byousz-2.1.tar", last modified: Fri May 10 12:29:45 2024, max compression
```

## Comparing `byousz-1.1.tar` & `byousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:56:40.061987 byousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1640 2024-05-08 23:56:40.061987 byousz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:56:40.061987 byousz-1.1/byousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:56:39.857983 byousz-1.1/byousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:56:39.865983 byousz-1.1/byousz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 23:56:39.857983 byousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-08 23:56:39.873983 byousz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 12:29:45.904331 byousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 23:56:39.000000 byousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-10 12:29:45.904331 byousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 23:56:39.000000 byousz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 12:29:45.904331 byousz-2.1/byousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:56:39.000000 byousz-2.1/byousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:56:39.000000 byousz-2.1/byousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 12:29:45.904331 byousz-2.1/byousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-10 12:29:45.000000 byousz-2.1/byousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      219 2024-05-10 12:29:45.000000 byousz-2.1/byousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 12:29:45.000000 byousz-2.1/byousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 12:29:45.000000 byousz-2.1/byousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        7 2024-05-10 12:29:45.000000 byousz-2.1/byousz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 12:29:45.904331 byousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-10 12:29:39.000000 byousz-2.1/setup.py
```

### Comparing `byousz-1.1/setup.py` & `byousz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'byousz',
     packages = ['byousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'byousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/byousz',
```

