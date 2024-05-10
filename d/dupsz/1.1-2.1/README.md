# Comparing `tmp/dupsz-1.1.tar.gz` & `tmp/dupsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dupsz-1.1.tar", last modified: Mon May  6 15:17:33 2024, max compression
+gzip compressed data, was "dupsz-2.1.tar", last modified: Fri May 10 18:15:13 2024, max compression
```

## Comparing `dupsz-1.1.tar` & `dupsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-06 15:17:33.207744 dupsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1636 2024-05-06 15:17:33.207744 dupsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-06 15:17:33.207744 dupsz-1.1/dupsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-06 15:17:33.003740 dupsz-1.1/dupsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-06 15:17:33.019740 dupsz-1.1/dupsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-06 15:17:33.003740 dupsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-06 15:17:33.023741 dupsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:15:13.610583 dupsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-06 15:17:33.000000 dupsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-10 18:15:13.610583 dupsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-06 15:17:33.000000 dupsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:15:13.610583 dupsz-2.1/dupsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-06 15:17:33.000000 dupsz-2.1/dupsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-06 15:17:33.000000 dupsz-2.1/dupsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:15:13.610583 dupsz-2.1/dupsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-10 18:15:13.000000 dupsz-2.1/dupsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      212 2024-05-10 18:15:13.000000 dupsz-2.1/dupsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 18:15:13.000000 dupsz-2.1/dupsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 18:15:13.000000 dupsz-2.1/dupsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        6 2024-05-10 18:15:13.000000 dupsz-2.1/dupsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 18:15:13.610583 dupsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-10 18:15:13.000000 dupsz-2.1/setup.py
```

### Comparing `dupsz-1.1/setup.py` & `dupsz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'dupsz',
     packages = ['dupsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'dupsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/dupsz',
```

