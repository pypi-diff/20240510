# Comparing `tmp/albifyz-1.1.tar.gz` & `tmp/albifyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albifyz-1.1.tar", last modified: Wed May  8 13:30:47 2024, max compression
+gzip compressed data, was "albifyz-2.1.tar", last modified: Fri May 10 08:50:34 2024, max compression
```

## Comparing `albifyz-1.1.tar` & `albifyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:30:47.438464 albifyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-08 13:30:47.438464 albifyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:30:47.438464 albifyz-1.1/albifyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:30:45.258424 albifyz-1.1/albifyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:30:45.418427 albifyz-1.1/albifyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 13:30:45.258424 albifyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-08 13:30:45.654431 albifyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:50:34.213774 albifyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 13:30:45.000000 albifyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-10 08:50:34.213774 albifyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 13:30:45.000000 albifyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:50:34.209774 albifyz-2.1/albifyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:30:45.000000 albifyz-2.1/albifyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:30:45.000000 albifyz-2.1/albifyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 08:50:34.213774 albifyz-2.1/albifyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-10 08:50:34.000000 albifyz-2.1/albifyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-10 08:50:34.000000 albifyz-2.1/albifyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 08:50:34.000000 albifyz-2.1/albifyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 08:50:34.000000 albifyz-2.1/albifyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-10 08:50:34.000000 albifyz-2.1/albifyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 08:50:34.213774 albifyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-10 08:50:33.000000 albifyz-2.1/setup.py
```

### Comparing `albifyz-1.1/setup.py` & `albifyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'albifyz',
     packages = ['albifyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'albifyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/albifyz',
```

