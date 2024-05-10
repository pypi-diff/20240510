# Comparing `tmp/futteretz-1.1.tar.gz` & `tmp/futteretz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futteretz-1.1.tar", last modified: Wed May  8 16:41:20 2024, max compression
+gzip compressed data, was "futteretz-2.1.tar", last modified: Fri May 10 21:17:38 2024, max compression
```

## Comparing `futteretz-1.1.tar` & `futteretz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:41:20.697271 futteretz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 16:41:20.697271 futteretz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:41:20.697271 futteretz-1.1/futteretz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:41:20.377266 futteretz-1.1/futteretz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:41:20.385266 futteretz-1.1/futteretz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:41:20.377266 futteretz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 16:41:20.393266 futteretz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:17:38.260274 futteretz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:41:20.000000 futteretz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 21:17:38.260274 futteretz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:41:20.000000 futteretz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:17:38.260274 futteretz-2.1/futteretz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:41:20.000000 futteretz-2.1/futteretz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:41:20.000000 futteretz-2.1/futteretz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:17:38.260274 futteretz-2.1/futteretz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-10 21:17:38.000000 futteretz-2.1/futteretz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-10 21:17:38.000000 futteretz-2.1/futteretz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 21:17:38.000000 futteretz-2.1/futteretz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 21:17:38.000000 futteretz-2.1/futteretz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-10 21:17:38.000000 futteretz-2.1/futteretz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 21:17:38.260274 futteretz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-10 21:17:37.000000 futteretz-2.1/setup.py
```

### Comparing `futteretz-1.1/setup.py` & `futteretz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'futteretz',
     packages = ['futteretz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'futteretz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/futteretz',
```

