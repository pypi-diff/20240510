# Comparing `tmp/derepressionz-1.1.tar.gz` & `tmp/derepressionz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "derepressionz-1.1.tar", last modified: Thu May  9 07:25:26 2024, max compression
+gzip compressed data, was "derepressionz-2.1.tar", last modified: Fri May 10 17:02:32 2024, max compression
```

## Comparing `derepressionz-1.1.tar` & `derepressionz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:25:26.945232 derepressionz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 07:25:26.945232 derepressionz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:25:26.945232 derepressionz-1.1/derepressionz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:25:23.961177 derepressionz-1.1/derepressionz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:25:24.229182 derepressionz-1.1/derepressionz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 07:25:23.961177 derepressionz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 07:25:24.549188 derepressionz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:02:32.126371 derepressionz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 07:25:23.000000 derepressionz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 17:02:32.126371 derepressionz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 07:25:23.000000 derepressionz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:02:32.126371 derepressionz-2.1/derepressionz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:25:23.000000 derepressionz-2.1/derepressionz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:25:24.000000 derepressionz-2.1/derepressionz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:02:32.126371 derepressionz-2.1/derepressionz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 17:02:31.000000 derepressionz-2.1/derepressionz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-10 17:02:31.000000 derepressionz-2.1/derepressionz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 17:02:31.000000 derepressionz-2.1/derepressionz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 17:02:31.000000 derepressionz-2.1/derepressionz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-10 17:02:31.000000 derepressionz-2.1/derepressionz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 17:02:32.126371 derepressionz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 17:02:25.000000 derepressionz-2.1/setup.py
```

### Comparing `derepressionz-1.1/setup.py` & `derepressionz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'derepressionz',
     packages = ['derepressionz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'derepressionz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/derepressionz',
```

