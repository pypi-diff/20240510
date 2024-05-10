# Comparing `tmp/barebonesz-1.1.tar.gz` & `tmp/barebonesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barebonesz-1.1.tar", last modified: Wed May  8 13:46:50 2024, max compression
+gzip compressed data, was "barebonesz-2.1.tar", last modified: Fri May 10 10:55:39 2024, max compression
```

## Comparing `barebonesz-1.1.tar` & `barebonesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:46:50.172236 barebonesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 13:46:50.172236 barebonesz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:46:50.172236 barebonesz-1.1/barebonesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:46:49.972233 barebonesz-1.1/barebonesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:46:49.980233 barebonesz-1.1/barebonesz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 13:46:49.972233 barebonesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 13:46:49.988233 barebonesz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:55:39.272153 barebonesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 13:46:49.000000 barebonesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 10:55:39.272153 barebonesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 13:46:49.000000 barebonesz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:55:39.268153 barebonesz-2.1/barebonesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:46:49.000000 barebonesz-2.1/barebonesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:46:49.000000 barebonesz-2.1/barebonesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:55:39.268153 barebonesz-2.1/barebonesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 10:55:39.000000 barebonesz-2.1/barebonesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 10:55:39.000000 barebonesz-2.1/barebonesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 10:55:39.000000 barebonesz-2.1/barebonesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 10:55:39.000000 barebonesz-2.1/barebonesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 10:55:39.000000 barebonesz-2.1/barebonesz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 10:55:39.272153 barebonesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 10:55:38.000000 barebonesz-2.1/setup.py
```

### Comparing `barebonesz-1.1/setup.py` & `barebonesz-2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'barebonesz',
     packages = ['barebonesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'barebonesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/barebonesz',
```

