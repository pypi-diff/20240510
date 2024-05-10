# Comparing `tmp/dishonorsz-1.1.tar.gz` & `tmp/dishonorsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dishonorsz-1.1.tar", last modified: Wed May  8 13:57:42 2024, max compression
+gzip compressed data, was "dishonorsz-2.1.tar", last modified: Fri May 10 17:49:33 2024, max compression
```

## Comparing `dishonorsz-1.1.tar` & `dishonorsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:57:42.296362 dishonorsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 13:57:42.296362 dishonorsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:57:42.296362 dishonorsz-1.1/dishonorsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:57:37.292268 dishonorsz-1.1/dishonorsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:57:37.440271 dishonorsz-1.1/dishonorsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 13:57:37.292268 dishonorsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 13:57:37.756277 dishonorsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:49:33.926242 dishonorsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 13:57:37.000000 dishonorsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 17:49:33.926242 dishonorsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 13:57:37.000000 dishonorsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:49:33.918242 dishonorsz-2.1/dishonorsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:57:37.000000 dishonorsz-2.1/dishonorsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:57:37.000000 dishonorsz-2.1/dishonorsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:49:33.926242 dishonorsz-2.1/dishonorsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 17:49:33.000000 dishonorsz-2.1/dishonorsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 17:49:33.000000 dishonorsz-2.1/dishonorsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 17:49:33.000000 dishonorsz-2.1/dishonorsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 17:49:33.000000 dishonorsz-2.1/dishonorsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 17:49:33.000000 dishonorsz-2.1/dishonorsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 17:49:33.926242 dishonorsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 17:49:33.000000 dishonorsz-2.1/setup.py
```

### Comparing `dishonorsz-1.1/setup.py` & `dishonorsz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'dishonorsz',
     packages = ['dishonorsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'dishonorsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/dishonorsz',
```

