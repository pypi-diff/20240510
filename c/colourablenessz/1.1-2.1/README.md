# Comparing `tmp/colourablenessz-1.1.tar.gz` & `tmp/colourablenessz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colourablenessz-1.1.tar", last modified: Thu May  9 09:58:55 2024, max compression
+gzip compressed data, was "colourablenessz-2.1.tar", last modified: Fri May 10 14:30:57 2024, max compression
```

## Comparing `colourablenessz-1.1.tar` & `colourablenessz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:58:55.658851 colourablenessz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-09 09:58:55.658851 colourablenessz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:58:55.658851 colourablenessz-1.1/colourablenessz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:58:55.462848 colourablenessz-1.1/colourablenessz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:58:55.470848 colourablenessz-1.1/colourablenessz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 09:58:55.458848 colourablenessz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-09 09:58:55.478848 colourablenessz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:30:57.170462 colourablenessz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 09:58:55.000000 colourablenessz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-10 14:30:57.170462 colourablenessz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 09:58:55.000000 colourablenessz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:30:57.170462 colourablenessz-2.1/colourablenessz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:58:55.000000 colourablenessz-2.1/colourablenessz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:58:55.000000 colourablenessz-2.1/colourablenessz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:30:57.170462 colourablenessz-2.1/colourablenessz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-10 14:30:56.000000 colourablenessz-2.1/colourablenessz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-10 14:30:56.000000 colourablenessz-2.1/colourablenessz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 14:30:56.000000 colourablenessz-2.1/colourablenessz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 14:30:56.000000 colourablenessz-2.1/colourablenessz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-10 14:30:56.000000 colourablenessz-2.1/colourablenessz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 14:30:57.170462 colourablenessz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-10 14:30:51.000000 colourablenessz-2.1/setup.py
```

### Comparing `colourablenessz-1.1/setup.py` & `colourablenessz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'colourablenessz',
     packages = ['colourablenessz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'colourablenessz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/colourablenessz',
```

