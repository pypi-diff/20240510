# Comparing `tmp/cuttlesz-1.1.tar.gz` & `tmp/cuttlesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuttlesz-1.1.tar", last modified: Thu May  9 07:31:13 2024, max compression
+gzip compressed data, was "cuttlesz-2.1.tar", last modified: Fri May 10 15:54:08 2024, max compression
```

## Comparing `cuttlesz-1.1.tar` & `cuttlesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:31:12.979587 cuttlesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 07:31:12.979587 cuttlesz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:31:12.979587 cuttlesz-1.1/cuttlesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:31:09.555524 cuttlesz-1.1/cuttlesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:31:09.751528 cuttlesz-1.1/cuttlesz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 07:31:09.555524 cuttlesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 07:31:10.191536 cuttlesz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:54:08.406493 cuttlesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 07:31:09.000000 cuttlesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 15:54:08.406493 cuttlesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 07:31:09.000000 cuttlesz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:54:08.362492 cuttlesz-2.1/cuttlesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:31:09.000000 cuttlesz-2.1/cuttlesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:31:09.000000 cuttlesz-2.1/cuttlesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:54:08.406493 cuttlesz-2.1/cuttlesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 15:54:06.000000 cuttlesz-2.1/cuttlesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 15:54:06.000000 cuttlesz-2.1/cuttlesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 15:54:06.000000 cuttlesz-2.1/cuttlesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 15:54:06.000000 cuttlesz-2.1/cuttlesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 15:54:06.000000 cuttlesz-2.1/cuttlesz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 15:54:08.406493 cuttlesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 15:54:01.000000 cuttlesz-2.1/setup.py
```

### Comparing `cuttlesz-1.1/setup.py` & `cuttlesz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'cuttlesz',
     packages = ['cuttlesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'cuttlesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/cuttlesz',
```

