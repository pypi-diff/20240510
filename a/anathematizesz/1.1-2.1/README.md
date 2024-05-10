# Comparing `tmp/anathematizesz-1.1.tar.gz` & `tmp/anathematizesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anathematizesz-1.1.tar", last modified: Thu May  9 01:51:11 2024, max compression
+gzip compressed data, was "anathematizesz-2.1.tar", last modified: Fri May 10 09:37:25 2024, max compression
```

## Comparing `anathematizesz-1.1.tar` & `anathematizesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:51:11.292911 anathematizesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-09 01:51:11.292911 anathematizesz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:51:11.292911 anathematizesz-1.1/anathematizesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:51:04.404784 anathematizesz-1.1/anathematizesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:51:04.588788 anathematizesz-1.1/anathematizesz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 01:51:04.404784 anathematizesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-09 01:51:04.888793 anathematizesz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 09:37:25.477626 anathematizesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 01:51:04.000000 anathematizesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-10 09:37:25.477626 anathematizesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 01:51:04.000000 anathematizesz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 09:37:25.477626 anathematizesz-2.1/anathematizesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:51:04.000000 anathematizesz-2.1/anathematizesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:51:04.000000 anathematizesz-2.1/anathematizesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 09:37:25.477626 anathematizesz-2.1/anathematizesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-10 09:37:25.000000 anathematizesz-2.1/anathematizesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-10 09:37:25.000000 anathematizesz-2.1/anathematizesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 09:37:25.000000 anathematizesz-2.1/anathematizesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 09:37:25.000000 anathematizesz-2.1/anathematizesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-10 09:37:25.000000 anathematizesz-2.1/anathematizesz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 09:37:25.477626 anathematizesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-10 09:37:24.000000 anathematizesz-2.1/setup.py
```

### Comparing `anathematizesz-1.1/setup.py` & `anathematizesz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'anathematizesz',
     packages = ['anathematizesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'anathematizesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/anathematizesz',
```

