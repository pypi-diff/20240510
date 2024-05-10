# Comparing `tmp/internet_domain_local-0.0.8.tar.gz` & `tmp/internet_domain_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internet_domain_local-0.0.8.tar", last modified: Sat Apr 20 17:03:15 2024, max compression
+gzip compressed data, was "internet_domain_local-0.0.9.tar", last modified: Thu May  9 06:17:30 2024, max compression
```

## Comparing `internet_domain_local-0.0.8.tar` & `internet_domain_local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:03:15.969749 internet_domain_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-20 17:03:15.969749 internet_domain_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 17:02:51.000000 internet_domain_local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:03:15.969749 internet_domain_local-0.0.8/internet_domain_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:03:15.969749 internet_domain_local-0.0.8/internet_domain_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 17:02:51.000000 internet_domain_local-0.0.8/internet_domain_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-04-20 17:02:51.000000 internet_domain_local-0.0.8/internet_domain_local/src/internet_domain_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-20 17:02:51.000000 internet_domain_local-0.0.8/internet_domain_local/src/internet_domain_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:03:15.969749 internet_domain_local-0.0.8/internet_domain_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-20 17:03:15.000000 internet_domain_local-0.0.8/internet_domain_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-20 17:03:15.000000 internet_domain_local-0.0.8/internet_domain_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:03:15.000000 internet_domain_local-0.0.8/internet_domain_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-20 17:03:15.000000 internet_domain_local-0.0.8/internet_domain_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 17:03:15.000000 internet_domain_local-0.0.8/internet_domain_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-20 17:02:51.000000 internet_domain_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:03:15.969749 internet_domain_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-20 17:02:51.000000 internet_domain_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:17:30.874215 internet_domain_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 06:17:30.874215 internet_domain_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 06:17:09.000000 internet_domain_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:17:30.874215 internet_domain_local-0.0.9/internet_domain_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:17:30.874215 internet_domain_local-0.0.9/internet_domain_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:17:09.000000 internet_domain_local-0.0.9/internet_domain_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-09 06:17:09.000000 internet_domain_local-0.0.9/internet_domain_local/src/internet_domain_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-09 06:17:09.000000 internet_domain_local-0.0.9/internet_domain_local/src/internet_domain_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:17:30.874215 internet_domain_local-0.0.9/internet_domain_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 06:17:30.000000 internet_domain_local-0.0.9/internet_domain_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-09 06:17:30.000000 internet_domain_local-0.0.9/internet_domain_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:17:30.000000 internet_domain_local-0.0.9/internet_domain_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-09 06:17:30.000000 internet_domain_local-0.0.9/internet_domain_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 06:17:30.000000 internet_domain_local-0.0.9/internet_domain_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-09 06:17:09.000000 internet_domain_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:17:30.874215 internet_domain_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-09 06:17:09.000000 internet_domain_local-0.0.9/setup.py
```

### Comparing `internet_domain_local-0.0.8/internet_domain_local/src/internet_domain_local.py` & `internet_domain_local-0.0.9/internet_domain_local/src/internet_domain_local.py`

 * *Files identical despite different names*

### Comparing `internet_domain_local-0.0.8/internet_domain_local/src/internet_domain_local_constants.py` & `internet_domain_local-0.0.9/internet_domain_local/src/internet_domain_local_constants.py`

 * *Files identical despite different names*

### Comparing `internet_domain_local-0.0.8/setup.py` & `internet_domain_local-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "internet-domain-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles internet-domain-local Python",
     long_description="PyPI Package for Circles internet-domain-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/internet-domain-local-python-package",
     packages=[package_dir],
@@ -22,11 +22,9 @@
     ],
     # TODO: Update which packages to include with this package
     install_requires=[
         'PyMySQL>=1.0.2',
         'pytest>=7.4.0',
         'mysql-connector>=2.2.9',
         'logzio-python-handler>= 4.1.0',
-        'user-context-remote>=0.0.17',
-        'python-sdk-local>=0.0.27'
     ],
 )
```

