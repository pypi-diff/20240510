# Comparing `tmp/cidaridaez-1.1.tar.gz` & `tmp/cidaridaez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cidaridaez-1.1.tar", last modified: Thu May  9 08:21:28 2024, max compression
+gzip compressed data, was "cidaridaez-2.1.tar", last modified: Fri May 10 14:20:40 2024, max compression
```

## Comparing `cidaridaez-1.1.tar` & `cidaridaez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:21:28.027119 cidaridaez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 08:21:28.027119 cidaridaez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:21:28.027119 cidaridaez-1.1/cidaridaez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:21:27.847116 cidaridaez-1.1/cidaridaez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:21:27.863116 cidaridaez-1.1/cidaridaez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 08:21:27.847116 cidaridaez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 08:21:27.871116 cidaridaez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:20:40.611091 cidaridaez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 08:21:27.000000 cidaridaez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 14:20:40.611091 cidaridaez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 08:21:27.000000 cidaridaez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:20:40.607091 cidaridaez-2.1/cidaridaez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:21:27.000000 cidaridaez-2.1/cidaridaez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:21:27.000000 cidaridaez-2.1/cidaridaez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:20:40.611091 cidaridaez-2.1/cidaridaez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 14:20:40.000000 cidaridaez-2.1/cidaridaez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 14:20:40.000000 cidaridaez-2.1/cidaridaez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 14:20:40.000000 cidaridaez-2.1/cidaridaez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 14:20:40.000000 cidaridaez-2.1/cidaridaez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 14:20:40.000000 cidaridaez-2.1/cidaridaez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 14:20:40.611091 cidaridaez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 14:20:39.000000 cidaridaez-2.1/setup.py
```

### Comparing `cidaridaez-1.1/setup.py` & `cidaridaez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'cidaridaez',
     packages = ['cidaridaez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'cidaridaez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/cidaridaez',
```

