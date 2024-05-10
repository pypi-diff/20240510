# Comparing `tmp/dignityz-1.1.tar.gz` & `tmp/dignityz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dignityz-1.1.tar", last modified: Thu May  9 03:50:12 2024, max compression
+gzip compressed data, was "dignityz-2.1.tar", last modified: Fri May 10 17:18:14 2024, max compression
```

## Comparing `dignityz-1.1.tar` & `dignityz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:50:12.763582 dignityz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 03:50:12.763582 dignityz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:50:12.763582 dignityz-1.1/dignityz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:50:09.311519 dignityz-1.1/dignityz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:50:09.467522 dignityz-1.1/dignityz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 03:50:09.311519 dignityz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 03:50:09.819528 dignityz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:18:14.227708 dignityz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 03:50:09.000000 dignityz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 17:18:14.227708 dignityz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 03:50:09.000000 dignityz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:18:14.227708 dignityz-2.1/dignityz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:50:09.000000 dignityz-2.1/dignityz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:50:09.000000 dignityz-2.1/dignityz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:18:14.227708 dignityz-2.1/dignityz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 17:18:14.000000 dignityz-2.1/dignityz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 17:18:14.000000 dignityz-2.1/dignityz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 17:18:14.000000 dignityz-2.1/dignityz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 17:18:14.000000 dignityz-2.1/dignityz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 17:18:14.000000 dignityz-2.1/dignityz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 17:18:14.227708 dignityz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 17:18:11.000000 dignityz-2.1/setup.py
```

### Comparing `dignityz-1.1/setup.py` & `dignityz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'dignityz',
     packages = ['dignityz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'dignityz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/dignityz',
```

