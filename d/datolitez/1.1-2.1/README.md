# Comparing `tmp/datolitez-1.1.tar.gz` & `tmp/datolitez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datolitez-1.1.tar", last modified: Wed May  8 19:41:03 2024, max compression
+gzip compressed data, was "datolitez-2.1.tar", last modified: Fri May 10 16:09:59 2024, max compression
```

## Comparing `datolitez-1.1.tar` & `datolitez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:41:03.060083 datolitez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 19:41:03.060083 datolitez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:41:03.060083 datolitez-1.1/datolitez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:41:02.860079 datolitez-1.1/datolitez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:41:02.868079 datolitez-1.1/datolitez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 19:41:02.860079 datolitez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 19:41:02.876079 datolitez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:09:59.480111 datolitez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 19:41:02.000000 datolitez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 16:09:59.480111 datolitez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 19:41:02.000000 datolitez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:09:59.436111 datolitez-2.1/datolitez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:41:02.000000 datolitez-2.1/datolitez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:41:02.000000 datolitez-2.1/datolitez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 16:09:59.480111 datolitez-2.1/datolitez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 16:09:58.000000 datolitez-2.1/datolitez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-10 16:09:58.000000 datolitez-2.1/datolitez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 16:09:58.000000 datolitez-2.1/datolitez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 16:09:58.000000 datolitez-2.1/datolitez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-10 16:09:58.000000 datolitez-2.1/datolitez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 16:09:59.480111 datolitez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-10 16:09:50.000000 datolitez-2.1/setup.py
```

### Comparing `datolitez-1.1/setup.py` & `datolitez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'datolitez',
     packages = ['datolitez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'datolitez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/datolitez',
```

