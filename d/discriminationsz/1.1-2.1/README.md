# Comparing `tmp/discriminationsz-1.1.tar.gz` & `tmp/discriminationsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discriminationsz-1.1.tar", last modified: Thu May  9 05:18:06 2024, max compression
+gzip compressed data, was "discriminationsz-2.1.tar", last modified: Fri May 10 17:39:14 2024, max compression
```

## Comparing `discriminationsz-1.1.tar` & `discriminationsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:18:06.284693 discriminationsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1680 2024-05-09 05:18:06.284693 discriminationsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:18:06.284693 discriminationsz-1.1/discriminationsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:18:03.472641 discriminationsz-1.1/discriminationsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:18:03.608644 discriminationsz-1.1/discriminationsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 05:18:03.472641 discriminationsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-09 05:18:03.860648 discriminationsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:39:14.550953 discriminationsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 05:18:03.000000 discriminationsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-10 17:39:14.550953 discriminationsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 05:18:03.000000 discriminationsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:39:14.518952 discriminationsz-2.1/discriminationsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:18:03.000000 discriminationsz-2.1/discriminationsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:18:03.000000 discriminationsz-2.1/discriminationsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 17:39:14.550953 discriminationsz-2.1/discriminationsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-10 17:39:13.000000 discriminationsz-2.1/discriminationsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      289 2024-05-10 17:39:13.000000 discriminationsz-2.1/discriminationsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 17:39:13.000000 discriminationsz-2.1/discriminationsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 17:39:13.000000 discriminationsz-2.1/discriminationsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       17 2024-05-10 17:39:13.000000 discriminationsz-2.1/discriminationsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 17:39:14.554953 discriminationsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-10 17:39:06.000000 discriminationsz-2.1/setup.py
```

### Comparing `discriminationsz-1.1/setup.py` & `discriminationsz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'discriminationsz',
     packages = ['discriminationsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'discriminationsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/discriminationsz',
```

