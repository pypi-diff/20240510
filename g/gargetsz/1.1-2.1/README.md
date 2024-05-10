# Comparing `tmp/gargetsz-1.1.tar.gz` & `tmp/gargetsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gargetsz-1.1.tar", last modified: Thu May  9 02:33:22 2024, max compression
+gzip compressed data, was "gargetsz-2.1.tar", last modified: Fri May 10 21:33:35 2024, max compression
```

## Comparing `gargetsz-1.1.tar` & `gargetsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:33:22.703085 gargetsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 02:33:22.703085 gargetsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:33:22.703085 gargetsz-1.1/gargetsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:33:22.495082 gargetsz-1.1/gargetsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:33:22.499082 gargetsz-1.1/gargetsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 02:33:22.495082 gargetsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 02:33:22.507082 gargetsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:33:34.953830 gargetsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 02:33:22.000000 gargetsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 21:33:34.953830 gargetsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 02:33:22.000000 gargetsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:33:34.941830 gargetsz-2.1/gargetsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:33:22.000000 gargetsz-2.1/gargetsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:33:22.000000 gargetsz-2.1/gargetsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 21:33:34.953830 gargetsz-2.1/gargetsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 21:33:34.000000 gargetsz-2.1/gargetsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 21:33:34.000000 gargetsz-2.1/gargetsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 21:33:34.000000 gargetsz-2.1/gargetsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 21:33:34.000000 gargetsz-2.1/gargetsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 21:33:34.000000 gargetsz-2.1/gargetsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 21:33:34.953830 gargetsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 21:33:28.000000 gargetsz-2.1/setup.py
```

### Comparing `gargetsz-1.1/setup.py` & `gargetsz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'gargetsz',
     packages = ['gargetsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'gargetsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/gargetsz',
```

