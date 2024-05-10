# Comparing `tmp/electz-1.1.tar.gz` & `tmp/electz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electz-1.1.tar", last modified: Wed May  8 18:02:50 2024, max compression
+gzip compressed data, was "electz-2.1.tar", last modified: Fri May 10 18:51:50 2024, max compression
```

## Comparing `electz-1.1.tar` & `electz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:02:50.663458 electz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1640 2024-05-08 18:02:50.663458 electz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:02:50.663458 electz-1.1/electz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:02:48.199413 electz-1.1/electz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:02:48.339416 electz-1.1/electz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 18:02:48.199413 electz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-08 18:02:48.499419 electz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:51:50.863287 electz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 18:02:48.000000 electz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-10 18:51:50.863287 electz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 18:02:48.000000 electz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:51:50.863287 electz-2.1/electz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:02:48.000000 electz-2.1/electz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:02:48.000000 electz-2.1/electz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 18:51:50.863287 electz-2.1/electz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-10 18:51:50.000000 electz-2.1/electz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      219 2024-05-10 18:51:50.000000 electz-2.1/electz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 18:51:50.000000 electz-2.1/electz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 18:51:50.000000 electz-2.1/electz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        7 2024-05-10 18:51:50.000000 electz-2.1/electz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 18:51:50.863287 electz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-10 18:51:50.000000 electz-2.1/setup.py
```

### Comparing `electz-1.1/setup.py` & `electz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'electz',
     packages = ['electz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'electz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/electz',
```

