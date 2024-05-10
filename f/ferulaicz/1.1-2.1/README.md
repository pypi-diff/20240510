# Comparing `tmp/ferulaicz-1.1.tar.gz` & `tmp/ferulaicz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferulaicz-1.1.tar", last modified: Thu May  9 09:09:38 2024, max compression
+gzip compressed data, was "ferulaicz-2.1.tar", last modified: Fri May 10 20:36:12 2024, max compression
```

## Comparing `ferulaicz-1.1.tar` & `ferulaicz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:09:38.008350 ferulaicz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-09 09:09:38.008350 ferulaicz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:09:38.008350 ferulaicz-1.1/ferulaicz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:09:37.836347 ferulaicz-1.1/ferulaicz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:09:37.844347 ferulaicz-1.1/ferulaicz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 09:09:37.836347 ferulaicz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-09 09:09:37.848347 ferulaicz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:36:12.074633 ferulaicz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 09:09:37.000000 ferulaicz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 20:36:12.074633 ferulaicz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 09:09:37.000000 ferulaicz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:36:12.074633 ferulaicz-2.1/ferulaicz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:09:37.000000 ferulaicz-2.1/ferulaicz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:09:37.000000 ferulaicz-2.1/ferulaicz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:36:12.074633 ferulaicz-2.1/ferulaicz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 20:36:11.000000 ferulaicz-2.1/ferulaicz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-10 20:36:11.000000 ferulaicz-2.1/ferulaicz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 20:36:11.000000 ferulaicz-2.1/ferulaicz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 20:36:11.000000 ferulaicz-2.1/ferulaicz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-10 20:36:11.000000 ferulaicz-2.1/ferulaicz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 20:36:12.074633 ferulaicz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-10 20:36:05.000000 ferulaicz-2.1/setup.py
```

### Comparing `ferulaicz-1.1/setup.py` & `ferulaicz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'ferulaicz',
     packages = ['ferulaicz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'ferulaicz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/ferulaicz',
```

