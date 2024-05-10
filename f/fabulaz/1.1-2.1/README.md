# Comparing `tmp/fabulaz-1.1.tar.gz` & `tmp/fabulaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabulaz-1.1.tar", last modified: Thu May  9 13:50:39 2024, max compression
+gzip compressed data, was "fabulaz-2.1.tar", last modified: Fri May 10 20:15:03 2024, max compression
```

## Comparing `fabulaz-1.1.tar` & `fabulaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 13:50:39.871215 fabulaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-09 13:50:39.871215 fabulaz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 13:50:39.871215 fabulaz-1.1/fabulaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 13:50:36.263152 fabulaz-1.1/fabulaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 13:50:36.471155 fabulaz-1.1/fabulaz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 13:50:36.263152 fabulaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-09 13:50:36.863162 fabulaz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:15:03.879306 fabulaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 13:50:36.000000 fabulaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-10 20:15:03.879306 fabulaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 13:50:36.000000 fabulaz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:15:03.879306 fabulaz-2.1/fabulaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 13:50:36.000000 fabulaz-2.1/fabulaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 13:50:36.000000 fabulaz-2.1/fabulaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 20:15:03.879306 fabulaz-2.1/fabulaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-10 20:15:03.000000 fabulaz-2.1/fabulaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-10 20:15:03.000000 fabulaz-2.1/fabulaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 20:15:03.000000 fabulaz-2.1/fabulaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 20:15:03.000000 fabulaz-2.1/fabulaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-10 20:15:03.000000 fabulaz-2.1/fabulaz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 20:15:03.879306 fabulaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-10 20:15:03.000000 fabulaz-2.1/setup.py
```

### Comparing `fabulaz-1.1/setup.py` & `fabulaz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'fabulaz',
     packages = ['fabulaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'fabulaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/fabulaz',
```

