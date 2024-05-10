# Comparing `tmp/armhoopz-1.1.tar.gz` & `tmp/armhoopz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armhoopz-1.1.tar", last modified: Thu May  9 01:34:24 2024, max compression
+gzip compressed data, was "armhoopz-2.1.tar", last modified: Fri May 10 10:13:49 2024, max compression
```

## Comparing `armhoopz-1.1.tar` & `armhoopz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:34:24.474327 armhoopz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 01:34:24.474327 armhoopz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:34:24.474327 armhoopz-1.1/armhoopz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:34:21.458271 armhoopz-1.1/armhoopz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:34:21.654275 armhoopz-1.1/armhoopz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 01:34:21.458271 armhoopz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 01:34:21.858279 armhoopz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:13:49.553890 armhoopz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 01:34:21.000000 armhoopz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 10:13:49.553890 armhoopz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 01:34:21.000000 armhoopz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:13:49.553890 armhoopz-2.1/armhoopz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:34:21.000000 armhoopz-2.1/armhoopz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:34:21.000000 armhoopz-2.1/armhoopz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:13:49.553890 armhoopz-2.1/armhoopz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 10:13:48.000000 armhoopz-2.1/armhoopz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 10:13:48.000000 armhoopz-2.1/armhoopz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 10:13:48.000000 armhoopz-2.1/armhoopz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 10:13:48.000000 armhoopz-2.1/armhoopz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 10:13:48.000000 armhoopz-2.1/armhoopz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 10:13:49.553890 armhoopz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 10:13:42.000000 armhoopz-2.1/setup.py
```

### Comparing `armhoopz-1.1/setup.py` & `armhoopz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'armhoopz',
     packages = ['armhoopz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'armhoopz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/armhoopz',
```

