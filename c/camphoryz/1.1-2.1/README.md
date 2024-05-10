# Comparing `tmp/camphoryz-1.1.tar.gz` & `tmp/camphoryz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camphoryz-1.1.tar", last modified: Wed May  8 13:20:05 2024, max compression
+gzip compressed data, was "camphoryz-2.1.tar", last modified: Fri May 10 13:01:19 2024, max compression
```

## Comparing `camphoryz-1.1.tar` & `camphoryz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:20:05.066608 camphoryz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 13:20:05.066608 camphoryz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:20:05.066608 camphoryz-1.1/camphoryz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:20:04.862604 camphoryz-1.1/camphoryz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:20:04.870604 camphoryz-1.1/camphoryz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 13:20:04.862604 camphoryz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 13:20:04.882604 camphoryz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:01:19.371265 camphoryz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 13:20:04.000000 camphoryz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 13:01:19.371265 camphoryz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 13:20:04.000000 camphoryz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:01:19.371265 camphoryz-2.1/camphoryz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:20:04.000000 camphoryz-2.1/camphoryz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:20:04.000000 camphoryz-2.1/camphoryz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 13:01:19.371265 camphoryz-2.1/camphoryz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 13:01:19.000000 camphoryz-2.1/camphoryz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-10 13:01:19.000000 camphoryz-2.1/camphoryz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 13:01:19.000000 camphoryz-2.1/camphoryz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 13:01:19.000000 camphoryz-2.1/camphoryz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-10 13:01:19.000000 camphoryz-2.1/camphoryz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 13:01:19.371265 camphoryz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-10 13:01:18.000000 camphoryz-2.1/setup.py
```

### Comparing `camphoryz-1.1/setup.py` & `camphoryz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'camphoryz',
     packages = ['camphoryz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'camphoryz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/camphoryz',
```

