# Comparing `tmp/gastrogastrotomyz-1.1.tar.gz` & `tmp/gastrogastrotomyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gastrogastrotomyz-1.1.tar", last modified: Thu May  9 05:06:59 2024, max compression
+gzip compressed data, was "gastrogastrotomyz-2.1.tar", last modified: Fri May 10 21:38:45 2024, max compression
```

## Comparing `gastrogastrotomyz-1.1.tar` & `gastrogastrotomyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:06:59.488437 gastrogastrotomyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 05:06:59.488437 gastrogastrotomyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:06:59.488437 gastrogastrotomyz-1.1/gastrogastrotomyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:06:55.804370 gastrogastrotomyz-1.1/gastrogastrotomyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:06:55.980373 gastrogastrotomyz-1.1/gastrogastrotomyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 05:06:55.804370 gastrogastrotomyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 05:06:56.292379 gastrogastrotomyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:38:45.367542 gastrogastrotomyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 05:06:55.000000 gastrogastrotomyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-10 21:38:45.367542 gastrogastrotomyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 05:06:55.000000 gastrogastrotomyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:38:45.367542 gastrogastrotomyz-2.1/gastrogastrotomyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:06:55.000000 gastrogastrotomyz-2.1/gastrogastrotomyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:06:55.000000 gastrogastrotomyz-2.1/gastrogastrotomyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:38:45.367542 gastrogastrotomyz-2.1/gastrogastrotomyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-10 21:38:45.000000 gastrogastrotomyz-2.1/gastrogastrotomyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-10 21:38:45.000000 gastrogastrotomyz-2.1/gastrogastrotomyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 21:38:45.000000 gastrogastrotomyz-2.1/gastrogastrotomyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 21:38:45.000000 gastrogastrotomyz-2.1/gastrogastrotomyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-10 21:38:45.000000 gastrogastrotomyz-2.1/gastrogastrotomyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 21:38:45.371542 gastrogastrotomyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-10 21:38:44.000000 gastrogastrotomyz-2.1/setup.py
```

### Comparing `gastrogastrotomyz-1.1/setup.py` & `gastrogastrotomyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'gastrogastrotomyz',
     packages = ['gastrogastrotomyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'gastrogastrotomyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/gastrogastrotomyz',
```

