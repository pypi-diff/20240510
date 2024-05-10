# Comparing `tmp/chevroletz-1.1.tar.gz` & `tmp/chevroletz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chevroletz-1.1.tar", last modified: Wed May  8 15:30:05 2024, max compression
+gzip compressed data, was "chevroletz-2.1.tar", last modified: Fri May 10 13:59:38 2024, max compression
```

## Comparing `chevroletz-1.1.tar` & `chevroletz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:30:05.210216 chevroletz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 15:30:05.210216 chevroletz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:30:05.210216 chevroletz-1.1/chevroletz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:30:04.958212 chevroletz-1.1/chevroletz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:30:04.966212 chevroletz-1.1/chevroletz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 15:30:04.958212 chevroletz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 15:30:04.970212 chevroletz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:59:38.439852 chevroletz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 15:30:04.000000 chevroletz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 13:59:38.439852 chevroletz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 15:30:04.000000 chevroletz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:59:38.439852 chevroletz-2.1/chevroletz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:30:04.000000 chevroletz-2.1/chevroletz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:30:04.000000 chevroletz-2.1/chevroletz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:59:38.439852 chevroletz-2.1/chevroletz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 13:59:37.000000 chevroletz-2.1/chevroletz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 13:59:37.000000 chevroletz-2.1/chevroletz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 13:59:37.000000 chevroletz-2.1/chevroletz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 13:59:37.000000 chevroletz-2.1/chevroletz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 13:59:37.000000 chevroletz-2.1/chevroletz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 13:59:38.443852 chevroletz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 13:59:32.000000 chevroletz-2.1/setup.py
```

### Comparing `chevroletz-1.1/setup.py` & `chevroletz-2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'chevroletz',
     packages = ['chevroletz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'chevroletz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/chevroletz',
```

