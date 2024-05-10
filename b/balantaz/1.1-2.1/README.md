# Comparing `tmp/balantaz-1.1.tar.gz` & `tmp/balantaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balantaz-1.1.tar", last modified: Wed May  8 14:41:07 2024, max compression
+gzip compressed data, was "balantaz-2.1.tar", last modified: Fri May 10 10:45:22 2024, max compression
```

## Comparing `balantaz-1.1.tar` & `balantaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:41:07.908265 balantaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-08 14:41:07.908265 balantaz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:41:07.908265 balantaz-1.1/balantaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:41:07.700261 balantaz-1.1/balantaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:41:07.708261 balantaz-1.1/balantaz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 14:41:07.700261 balantaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-08 14:41:07.712261 balantaz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:45:22.236750 balantaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 14:41:07.000000 balantaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 10:45:22.236750 balantaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 14:41:07.000000 balantaz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:45:22.156749 balantaz-2.1/balantaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:41:07.000000 balantaz-2.1/balantaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:41:07.000000 balantaz-2.1/balantaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:45:22.236750 balantaz-2.1/balantaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 10:45:20.000000 balantaz-2.1/balantaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 10:45:20.000000 balantaz-2.1/balantaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 10:45:20.000000 balantaz-2.1/balantaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 10:45:20.000000 balantaz-2.1/balantaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 10:45:20.000000 balantaz-2.1/balantaz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 10:45:22.236750 balantaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 10:45:08.000000 balantaz-2.1/setup.py
```

### Comparing `balantaz-1.1/setup.py` & `balantaz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'balantaz',
     packages = ['balantaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'balantaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/balantaz',
```

