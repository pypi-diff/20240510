# Comparing `tmp/fivepinsz-1.1.tar.gz` & `tmp/fivepinsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fivepinsz-1.1.tar", last modified: Thu May  9 09:48:28 2024, max compression
+gzip compressed data, was "fivepinsz-2.1.tar", last modified: Fri May 10 20:51:29 2024, max compression
```

## Comparing `fivepinsz-1.1.tar` & `fivepinsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:48:28.175293 fivepinsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-09 09:48:28.175293 fivepinsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:48:28.175293 fivepinsz-1.1/fivepinsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:48:25.167238 fivepinsz-1.1/fivepinsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:48:25.327241 fivepinsz-1.1/fivepinsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 09:48:25.167238 fivepinsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-09 09:48:25.583245 fivepinsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:51:29.555522 fivepinsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 09:48:25.000000 fivepinsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 20:51:29.555522 fivepinsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 09:48:25.000000 fivepinsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:51:29.555522 fivepinsz-2.1/fivepinsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:48:25.000000 fivepinsz-2.1/fivepinsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:48:25.000000 fivepinsz-2.1/fivepinsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:51:29.555522 fivepinsz-2.1/fivepinsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 20:51:29.000000 fivepinsz-2.1/fivepinsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-10 20:51:29.000000 fivepinsz-2.1/fivepinsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 20:51:29.000000 fivepinsz-2.1/fivepinsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 20:51:29.000000 fivepinsz-2.1/fivepinsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-10 20:51:29.000000 fivepinsz-2.1/fivepinsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 20:51:29.555522 fivepinsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-10 20:51:26.000000 fivepinsz-2.1/setup.py
```

### Comparing `fivepinsz-1.1/setup.py` & `fivepinsz-2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'fivepinsz',
     packages = ['fivepinsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'fivepinsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/fivepinsz',
```

