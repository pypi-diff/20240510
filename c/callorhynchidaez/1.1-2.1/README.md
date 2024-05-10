# Comparing `tmp/callorhynchidaez-1.1.tar.gz` & `tmp/callorhynchidaez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callorhynchidaez-1.1.tar", last modified: Thu May  9 11:47:05 2024, max compression
+gzip compressed data, was "callorhynchidaez-2.1.tar", last modified: Fri May 10 12:56:05 2024, max compression
```

## Comparing `callorhynchidaez-1.1.tar` & `callorhynchidaez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:47:05.382261 callorhynchidaez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1680 2024-05-09 11:47:05.382261 callorhynchidaez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:47:05.382261 callorhynchidaez-1.1/callorhynchidaez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:47:02.442207 callorhynchidaez-1.1/callorhynchidaez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:47:02.594210 callorhynchidaez-1.1/callorhynchidaez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 11:47:02.442207 callorhynchidaez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-09 11:47:02.854215 callorhynchidaez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 12:56:05.017467 callorhynchidaez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 11:47:02.000000 callorhynchidaez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-10 12:56:05.017467 callorhynchidaez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 11:47:02.000000 callorhynchidaez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 12:56:05.017467 callorhynchidaez-2.1/callorhynchidaez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:47:02.000000 callorhynchidaez-2.1/callorhynchidaez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:47:02.000000 callorhynchidaez-2.1/callorhynchidaez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 12:56:05.017467 callorhynchidaez-2.1/callorhynchidaez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-10 12:56:04.000000 callorhynchidaez-2.1/callorhynchidaez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      289 2024-05-10 12:56:04.000000 callorhynchidaez-2.1/callorhynchidaez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 12:56:04.000000 callorhynchidaez-2.1/callorhynchidaez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 12:56:04.000000 callorhynchidaez-2.1/callorhynchidaez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       17 2024-05-10 12:56:04.000000 callorhynchidaez-2.1/callorhynchidaez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 12:56:05.017467 callorhynchidaez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-10 12:55:58.000000 callorhynchidaez-2.1/setup.py
```

### Comparing `callorhynchidaez-1.1/setup.py` & `callorhynchidaez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'callorhynchidaez',
     packages = ['callorhynchidaez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'callorhynchidaez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/callorhynchidaez',
```

