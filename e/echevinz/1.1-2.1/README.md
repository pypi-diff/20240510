# Comparing `tmp/echevinz-1.1.tar.gz` & `tmp/echevinz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echevinz-1.1.tar", last modified: Wed May  8 20:08:13 2024, max compression
+gzip compressed data, was "echevinz-2.1.tar", last modified: Fri May 10 18:25:25 2024, max compression
```

## Comparing `echevinz-1.1.tar` & `echevinz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 20:08:13.770394 echevinz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-08 20:08:13.770394 echevinz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 20:08:13.770394 echevinz-1.1/echevinz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 20:08:13.066381 echevinz-1.1/echevinz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 20:08:13.130382 echevinz-1.1/echevinz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 20:08:13.066381 echevinz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-08 20:08:13.258385 echevinz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:25:25.081957 echevinz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 20:08:13.000000 echevinz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 18:25:25.081957 echevinz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 20:08:13.000000 echevinz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:25:25.081957 echevinz-2.1/echevinz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 20:08:13.000000 echevinz-2.1/echevinz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 20:08:13.000000 echevinz-2.1/echevinz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:25:25.081957 echevinz-2.1/echevinz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 18:25:24.000000 echevinz-2.1/echevinz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 18:25:24.000000 echevinz-2.1/echevinz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 18:25:24.000000 echevinz-2.1/echevinz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 18:25:24.000000 echevinz-2.1/echevinz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 18:25:24.000000 echevinz-2.1/echevinz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 18:25:25.081957 echevinz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 18:25:23.000000 echevinz-2.1/setup.py
```

### Comparing `echevinz-1.1/setup.py` & `echevinz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'echevinz',
     packages = ['echevinz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'echevinz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/echevinz',
```

