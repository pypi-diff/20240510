# Comparing `tmp/Deep-KAN-0.0.2.tar.gz` & `tmp/Deep-KAN-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Deep-KAN-0.0.2.tar", last modified: Thu May  9 17:16:15 2024, max compression
+gzip compressed data, was "Deep-KAN-0.0.3.tar", last modified: Fri May 10 11:48:54 2024, max compression
```

## Comparing `Deep-KAN-0.0.2.tar` & `Deep-KAN-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/Deep_KAN.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3774 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:16:15.000000 Deep-KAN-0.0.2/Deep_KAN.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3774 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3423 2024-05-09 17:14:52.000000 Deep-KAN-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/deepkan/
--rw-r--r--   0 root         (0) root         (0)      108 2024-05-09 16:55:46.000000 Deep-KAN-0.0.2/deepkan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8122 2024-05-09 16:54:53.000000 Deep-KAN-0.0.2/deepkan/deepkan.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 17:16:15.286202 Deep-KAN-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      768 2024-05-09 16:56:07.000000 Deep-KAN-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 11:48:54.346552 Deep-KAN-0.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 11:48:54.346552 Deep-KAN-0.0.3/Deep_KAN.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6541 2024-05-10 11:48:54.000000 Deep-KAN-0.0.3/Deep_KAN.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-10 11:48:54.000000 Deep-KAN-0.0.3/Deep_KAN.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 11:48:54.000000 Deep-KAN-0.0.3/Deep_KAN.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-10 11:48:54.000000 Deep-KAN-0.0.3/Deep_KAN.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-10 11:48:54.000000 Deep-KAN-0.0.3/Deep_KAN.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     6541 2024-05-10 11:48:54.346552 Deep-KAN-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6246 2024-05-10 11:48:04.000000 Deep-KAN-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 11:48:54.346552 Deep-KAN-0.0.3/deepkan/
+-rw-r--r--   0 root         (0) root         (0)      205 2024-05-10 11:38:59.000000 Deep-KAN-0.0.3/deepkan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10400 2024-05-10 11:37:50.000000 Deep-KAN-0.0.3/deepkan/deepkan.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 11:48:54.346552 Deep-KAN-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      768 2024-05-10 11:48:18.000000 Deep-KAN-0.0.3/setup.py
```

### Comparing `Deep-KAN-0.0.2/setup.py` & `Deep-KAN-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Deep-KAN',
-    version='0.0.2',
+    version='0.0.3',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Implimentation of Kolmogorov–Arnold Networks(KAN)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

