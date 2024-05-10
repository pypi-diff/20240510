# Comparing `tmp/betanglementz-1.1.tar.gz` & `tmp/betanglementz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanglementz-1.1.tar", last modified: Thu May  9 05:23:36 2024, max compression
+gzip compressed data, was "betanglementz-2.1.tar", last modified: Fri May 10 11:06:12 2024, max compression
```

## Comparing `betanglementz-1.1.tar` & `betanglementz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:23:36.482762 betanglementz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 05:23:36.482762 betanglementz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:23:36.482762 betanglementz-1.1/betanglementz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:23:33.482707 betanglementz-1.1/betanglementz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:23:33.686711 betanglementz-1.1/betanglementz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 05:23:33.482707 betanglementz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 05:23:33.946716 betanglementz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 11:06:12.167842 betanglementz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 05:23:33.000000 betanglementz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 11:06:12.167842 betanglementz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 05:23:33.000000 betanglementz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 11:06:12.159842 betanglementz-2.1/betanglementz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:23:33.000000 betanglementz-2.1/betanglementz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:23:33.000000 betanglementz-2.1/betanglementz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 11:06:12.167842 betanglementz-2.1/betanglementz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 11:06:11.000000 betanglementz-2.1/betanglementz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-10 11:06:11.000000 betanglementz-2.1/betanglementz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 11:06:11.000000 betanglementz-2.1/betanglementz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 11:06:11.000000 betanglementz-2.1/betanglementz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-10 11:06:11.000000 betanglementz-2.1/betanglementz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 11:06:12.167842 betanglementz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 11:06:04.000000 betanglementz-2.1/setup.py
```

### Comparing `betanglementz-1.1/setup.py` & `betanglementz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'betanglementz',
     packages = ['betanglementz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'betanglementz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/betanglementz',
```

