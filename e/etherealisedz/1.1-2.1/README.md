# Comparing `tmp/etherealisedz-1.1.tar.gz` & `tmp/etherealisedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etherealisedz-1.1.tar", last modified: Wed May  8 14:03:29 2024, max compression
+gzip compressed data, was "etherealisedz-2.1.tar", last modified: Fri May 10 19:38:52 2024, max compression
```

## Comparing `etherealisedz-1.1.tar` & `etherealisedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:03:28.986822 etherealisedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-08 14:03:28.986822 etherealisedz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:03:28.986822 etherealisedz-1.1/etherealisedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:03:25.542758 etherealisedz-1.1/etherealisedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:03:25.718762 etherealisedz-1.1/etherealisedz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 14:03:25.542758 etherealisedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-08 14:03:26.170770 etherealisedz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:38:52.595460 etherealisedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 14:03:25.000000 etherealisedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 19:38:52.595460 etherealisedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 14:03:25.000000 etherealisedz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:38:52.595460 etherealisedz-2.1/etherealisedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:03:25.000000 etherealisedz-2.1/etherealisedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:03:25.000000 etherealisedz-2.1/etherealisedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:38:52.595460 etherealisedz-2.1/etherealisedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 19:38:52.000000 etherealisedz-2.1/etherealisedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-10 19:38:52.000000 etherealisedz-2.1/etherealisedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 19:38:52.000000 etherealisedz-2.1/etherealisedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 19:38:52.000000 etherealisedz-2.1/etherealisedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-10 19:38:52.000000 etherealisedz-2.1/etherealisedz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 19:38:52.595460 etherealisedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 19:38:52.000000 etherealisedz-2.1/setup.py
```

### Comparing `etherealisedz-1.1/setup.py` & `etherealisedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'etherealisedz',
     packages = ['etherealisedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'etherealisedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/etherealisedz',
```

