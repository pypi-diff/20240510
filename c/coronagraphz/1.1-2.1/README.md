# Comparing `tmp/coronagraphz-1.1.tar.gz` & `tmp/coronagraphz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coronagraphz-1.1.tar", last modified: Thu May  9 02:17:49 2024, max compression
+gzip compressed data, was "coronagraphz-2.1.tar", last modified: Fri May 10 15:12:19 2024, max compression
```

## Comparing `coronagraphz-1.1.tar` & `coronagraphz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:17:49.618414 coronagraphz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 02:17:49.618414 coronagraphz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:17:49.618414 coronagraphz-1.1/coronagraphz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:17:49.434410 coronagraphz-1.1/coronagraphz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:17:49.446411 coronagraphz-1.1/coronagraphz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 02:17:49.434410 coronagraphz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 02:17:49.450410 coronagraphz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:12:19.436180 coronagraphz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 02:17:49.000000 coronagraphz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 15:12:19.436180 coronagraphz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 02:17:49.000000 coronagraphz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:12:19.436180 coronagraphz-2.1/coronagraphz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:17:49.000000 coronagraphz-2.1/coronagraphz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:17:49.000000 coronagraphz-2.1/coronagraphz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:12:19.436180 coronagraphz-2.1/coronagraphz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 15:12:18.000000 coronagraphz-2.1/coronagraphz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-10 15:12:18.000000 coronagraphz-2.1/coronagraphz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 15:12:18.000000 coronagraphz-2.1/coronagraphz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 15:12:18.000000 coronagraphz-2.1/coronagraphz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-10 15:12:18.000000 coronagraphz-2.1/coronagraphz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 15:12:19.436180 coronagraphz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 15:12:14.000000 coronagraphz-2.1/setup.py
```

### Comparing `coronagraphz-1.1/setup.py` & `coronagraphz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'coronagraphz',
     packages = ['coronagraphz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'coronagraphz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/coronagraphz',
```

