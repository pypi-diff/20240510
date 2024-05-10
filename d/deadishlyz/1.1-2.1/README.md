# Comparing `tmp/deadishlyz-1.1.tar.gz` & `tmp/deadishlyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadishlyz-1.1.tar", last modified: Thu May  9 06:07:53 2024, max compression
+gzip compressed data, was "deadishlyz-2.1.tar", last modified: Fri May 10 16:15:21 2024, max compression
```

## Comparing `deadishlyz-1.1.tar` & `deadishlyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:07:53.871604 deadishlyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 06:07:53.871604 deadishlyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:07:53.871604 deadishlyz-1.1/deadishlyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:07:50.763547 deadishlyz-1.1/deadishlyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:07:50.959551 deadishlyz-1.1/deadishlyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 06:07:50.763547 deadishlyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 06:07:51.267557 deadishlyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:15:20.994055 deadishlyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 06:07:50.000000 deadishlyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 16:15:20.994055 deadishlyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 06:07:50.000000 deadishlyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:15:20.986055 deadishlyz-2.1/deadishlyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:07:50.000000 deadishlyz-2.1/deadishlyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:07:50.000000 deadishlyz-2.1/deadishlyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:15:20.994055 deadishlyz-2.1/deadishlyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 16:15:20.000000 deadishlyz-2.1/deadishlyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 16:15:20.000000 deadishlyz-2.1/deadishlyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 16:15:20.000000 deadishlyz-2.1/deadishlyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 16:15:20.000000 deadishlyz-2.1/deadishlyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 16:15:20.000000 deadishlyz-2.1/deadishlyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 16:15:20.994055 deadishlyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 16:15:13.000000 deadishlyz-2.1/setup.py
```

### Comparing `deadishlyz-1.1/setup.py` & `deadishlyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'deadishlyz',
     packages = ['deadishlyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'deadishlyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/deadishlyz',
```

