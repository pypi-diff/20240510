# Comparing `tmp/ejecteez-1.1.tar.gz` & `tmp/ejecteez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejecteez-1.1.tar", last modified: Mon May  6 15:10:35 2024, max compression
+gzip compressed data, was "ejecteez-2.1.tar", last modified: Fri May 10 18:41:07 2024, max compression
```

## Comparing `ejecteez-1.1.tar` & `ejecteez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-06 15:10:35.856081 ejecteez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-06 15:10:35.856081 ejecteez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-06 15:10:35.856081 ejecteez-1.1/ejecteez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-06 15:10:35.684078 ejecteez-1.1/ejecteez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-06 15:10:35.692078 ejecteez-1.1/ejecteez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-06 15:10:35.684078 ejecteez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-06 15:10:35.692078 ejecteez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:41:07.555382 ejecteez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-06 15:10:35.000000 ejecteez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 18:41:07.555382 ejecteez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-06 15:10:35.000000 ejecteez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:41:07.551382 ejecteez-2.1/ejecteez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-06 15:10:35.000000 ejecteez-2.1/ejecteez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-06 15:10:35.000000 ejecteez-2.1/ejecteez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:41:07.555382 ejecteez-2.1/ejecteez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 18:41:07.000000 ejecteez-2.1/ejecteez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 18:41:07.000000 ejecteez-2.1/ejecteez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 18:41:07.000000 ejecteez-2.1/ejecteez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 18:41:07.000000 ejecteez-2.1/ejecteez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 18:41:07.000000 ejecteez-2.1/ejecteez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 18:41:07.555382 ejecteez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 18:41:06.000000 ejecteez-2.1/setup.py
```

### Comparing `ejecteez-1.1/setup.py` & `ejecteez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'ejecteez',
     packages = ['ejecteez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'ejecteez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/ejecteez',
```

