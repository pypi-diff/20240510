# Comparing `tmp/autohemolyticz-1.1.tar.gz` & `tmp/autohemolyticz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autohemolyticz-1.1.tar", last modified: Thu May  9 02:38:52 2024, max compression
+gzip compressed data, was "autohemolyticz-2.1.tar", last modified: Fri May 10 10:34:41 2024, max compression
```

## Comparing `autohemolyticz-1.1.tar` & `autohemolyticz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:38:51.953001 autohemolyticz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-09 02:38:51.953001 autohemolyticz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:38:51.953001 autohemolyticz-1.1/autohemolyticz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:38:47.340917 autohemolyticz-1.1/autohemolyticz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:38:47.532921 autohemolyticz-1.1/autohemolyticz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 02:38:47.340917 autohemolyticz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-09 02:38:47.820926 autohemolyticz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:34:41.472944 autohemolyticz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 02:38:47.000000 autohemolyticz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-10 10:34:41.472944 autohemolyticz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 02:38:47.000000 autohemolyticz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:34:41.472944 autohemolyticz-2.1/autohemolyticz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:38:47.000000 autohemolyticz-2.1/autohemolyticz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:38:47.000000 autohemolyticz-2.1/autohemolyticz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 10:34:41.472944 autohemolyticz-2.1/autohemolyticz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-10 10:34:40.000000 autohemolyticz-2.1/autohemolyticz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-10 10:34:40.000000 autohemolyticz-2.1/autohemolyticz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 10:34:40.000000 autohemolyticz-2.1/autohemolyticz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 10:34:40.000000 autohemolyticz-2.1/autohemolyticz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-10 10:34:40.000000 autohemolyticz-2.1/autohemolyticz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 10:34:41.472944 autohemolyticz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-10 10:34:33.000000 autohemolyticz-2.1/setup.py
```

### Comparing `autohemolyticz-1.1/setup.py` & `autohemolyticz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'autohemolyticz',
     packages = ['autohemolyticz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'autohemolyticz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/autohemolyticz',
```

