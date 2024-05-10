# Comparing `tmp/conclavistz-1.1.tar.gz` & `tmp/conclavistz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conclavistz-1.1.tar", last modified: Wed May  8 14:20:21 2024, max compression
+gzip compressed data, was "conclavistz-2.1.tar", last modified: Fri May 10 14:51:44 2024, max compression
```

## Comparing `conclavistz-1.1.tar` & `conclavistz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:20:21.233592 conclavistz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-08 14:20:21.233592 conclavistz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:20:21.233592 conclavistz-1.1/conclavistz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:20:20.985588 conclavistz-1.1/conclavistz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:20:20.993588 conclavistz-1.1/conclavistz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 14:20:20.985588 conclavistz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-08 14:20:21.005588 conclavistz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:51:44.265440 conclavistz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 14:20:20.000000 conclavistz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-10 14:51:44.265440 conclavistz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 14:20:20.000000 conclavistz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:51:44.265440 conclavistz-2.1/conclavistz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:20:20.000000 conclavistz-2.1/conclavistz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:20:20.000000 conclavistz-2.1/conclavistz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 14:51:44.265440 conclavistz-2.1/conclavistz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-10 14:51:44.000000 conclavistz-2.1/conclavistz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-10 14:51:44.000000 conclavistz-2.1/conclavistz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 14:51:44.000000 conclavistz-2.1/conclavistz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 14:51:44.000000 conclavistz-2.1/conclavistz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-10 14:51:44.000000 conclavistz-2.1/conclavistz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 14:51:44.265440 conclavistz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-10 14:51:43.000000 conclavistz-2.1/setup.py
```

### Comparing `conclavistz-1.1/setup.py` & `conclavistz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'conclavistz',
     packages = ['conclavistz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'conclavistz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/conclavistz',
```

