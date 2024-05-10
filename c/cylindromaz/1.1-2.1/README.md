# Comparing `tmp/cylindromaz-1.1.tar.gz` & `tmp/cylindromaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylindromaz-1.1.tar", last modified: Thu May  9 04:55:40 2024, max compression
+gzip compressed data, was "cylindromaz-2.1.tar", last modified: Fri May 10 15:59:25 2024, max compression
```

## Comparing `cylindromaz-1.1.tar` & `cylindromaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:55:40.311958 cylindromaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 04:55:40.311958 cylindromaz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:55:40.311958 cylindromaz-1.1/cylindromaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:55:34.683855 cylindromaz-1.1/cylindromaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:55:34.887859 cylindromaz-1.1/cylindromaz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 04:55:34.679855 cylindromaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 04:55:35.287866 cylindromaz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:59:25.880372 cylindromaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 04:55:34.000000 cylindromaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-10 15:59:25.880372 cylindromaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 04:55:34.000000 cylindromaz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:59:25.876372 cylindromaz-2.1/cylindromaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:55:34.000000 cylindromaz-2.1/cylindromaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:55:34.000000 cylindromaz-2.1/cylindromaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 15:59:25.880372 cylindromaz-2.1/cylindromaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-10 15:59:25.000000 cylindromaz-2.1/cylindromaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-10 15:59:25.000000 cylindromaz-2.1/cylindromaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 15:59:25.000000 cylindromaz-2.1/cylindromaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 15:59:25.000000 cylindromaz-2.1/cylindromaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-10 15:59:25.000000 cylindromaz-2.1/cylindromaz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 15:59:25.880372 cylindromaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-10 15:59:25.000000 cylindromaz-2.1/setup.py
```

### Comparing `cylindromaz-1.1/setup.py` & `cylindromaz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'cylindromaz',
     packages = ['cylindromaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'cylindromaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/cylindromaz',
```

