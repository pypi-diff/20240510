# Comparing `tmp/evaluatedz-1.1.tar.gz` & `tmp/evaluatedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaluatedz-1.1.tar", last modified: Thu May  9 19:37:03 2024, max compression
+gzip compressed data, was "evaluatedz-2.1.tar", last modified: Fri May 10 19:49:00 2024, max compression
```

## Comparing `evaluatedz-1.1.tar` & `evaluatedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:37:03.662004 evaluatedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 19:37:03.662004 evaluatedz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:37:03.662004 evaluatedz-1.1/evaluatedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:37:00.461945 evaluatedz-1.1/evaluatedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:37:00.709949 evaluatedz-1.1/evaluatedz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 19:37:00.461945 evaluatedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 19:37:01.097957 evaluatedz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:49:00.522692 evaluatedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 19:37:00.000000 evaluatedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 19:49:00.522692 evaluatedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 19:37:00.000000 evaluatedz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:49:00.518692 evaluatedz-2.1/evaluatedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:37:00.000000 evaluatedz-2.1/evaluatedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:37:00.000000 evaluatedz-2.1/evaluatedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 19:49:00.518692 evaluatedz-2.1/evaluatedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 19:49:00.000000 evaluatedz-2.1/evaluatedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 19:49:00.000000 evaluatedz-2.1/evaluatedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 19:49:00.000000 evaluatedz-2.1/evaluatedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 19:49:00.000000 evaluatedz-2.1/evaluatedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 19:49:00.000000 evaluatedz-2.1/evaluatedz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 19:49:00.522692 evaluatedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 19:48:59.000000 evaluatedz-2.1/setup.py
```

### Comparing `evaluatedz-1.1/setup.py` & `evaluatedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'evaluatedz',
     packages = ['evaluatedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'evaluatedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/evaluatedz',
```

