# Comparing `tmp/parentlol-0.0.1.tar.gz` & `tmp/parentlol-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parentlol-0.0.1.tar", last modified: Fri May 10 02:53:43 2024, max compression
+gzip compressed data, was "parentlol-0.0.2.tar", last modified: Fri May 10 03:03:34 2024, max compression
```

## Comparing `parentlol-0.0.1.tar` & `parentlol-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 02:53:43.536983 parentlol-0.0.1/
--rw-rw-rw-   0        0        0      374 2024-05-10 02:53:43.528447 parentlol-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 02:53:43.517923 parentlol-0.0.1/ParentLOL/
--rw-rw-rw-   0        0        0     1158 2024-05-10 02:49:54.000000 parentlol-0.0.1/ParentLOL/Sprinter.py
--rw-rw-rw-   0        0        0       31 2024-05-10 02:48:55.000000 parentlol-0.0.1/ParentLOL/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 02:53:43.527444 parentlol-0.0.1/ParentLOL.egg-info/
--rw-rw-rw-   0        0        0      374 2024-05-10 02:53:43.000000 parentlol-0.0.1/ParentLOL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-10 02:53:43.000000 parentlol-0.0.1/ParentLOL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 02:53:43.000000 parentlol-0.0.1/ParentLOL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 02:53:43.000000 parentlol-0.0.1/ParentLOL.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-10 02:53:43.000000 parentlol-0.0.1/ParentLOL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 02:53:43.537984 parentlol-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      521 2024-05-10 02:52:46.000000 parentlol-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:03:34.957087 parentlol-0.0.2/
+-rw-rw-rw-   0        0        0      374 2024-05-10 03:03:34.955062 parentlol-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 03:03:34.942048 parentlol-0.0.2/ParentLOL/
+-rw-rw-rw-   0        0        0     1158 2024-05-10 03:01:41.000000 parentlol-0.0.2/ParentLOL/ParentLOL.py
+-rw-rw-rw-   0        0        0       33 2024-05-10 03:02:22.000000 parentlol-0.0.2/ParentLOL/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:03:34.953558 parentlol-0.0.2/ParentLOL.egg-info/
+-rw-rw-rw-   0        0        0      374 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:03:34.957087 parentlol-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      521 2024-05-10 03:03:09.000000 parentlol-0.0.2/setup.py
```

### Comparing `parentlol-0.0.1/ParentLOL/Sprinter.py` & `parentlol-0.0.2/ParentLOL/ParentLOL.py`

 * *Files identical despite different names*

### Comparing `parentlol-0.0.1/setup.py` & `parentlol-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ParentLOL',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[
         "colorama",
         "datetime"
     ],
     description='Printing with Ease.',
     author='parent',
```

