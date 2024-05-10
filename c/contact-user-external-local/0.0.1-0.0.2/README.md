# Comparing `tmp/contact_user_external_local-0.0.1.tar.gz` & `tmp/contact_user_external_local-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_user_external_local-0.0.1.tar", last modified: Wed May  8 08:31:30 2024, max compression
+gzip compressed data, was "contact_user_external_local-0.0.2.tar", last modified: Thu May  9 05:59:23 2024, max compression
```

## Comparing `contact_user_external_local-0.0.1.tar` & `contact_user_external_local-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:31:30.455188 contact_user_external_local-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 08:31:30.455188 contact_user_external_local-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 08:31:04.000000 contact_user_external_local-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:31:30.451188 contact_user_external_local-0.0.1/contact_user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:31:30.455188 contact_user_external_local-0.0.1/contact_user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:31:04.000000 contact_user_external_local-0.0.1/contact_user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-08 08:31:04.000000 contact_user_external_local-0.0.1/contact_user_external_local/src/contact_user_external_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 08:31:04.000000 contact_user_external_local-0.0.1/contact_user_external_local/src/contact_user_external_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:31:30.455188 contact_user_external_local-0.0.1/contact_user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 08:31:30.000000 contact_user_external_local-0.0.1/contact_user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 08:31:30.000000 contact_user_external_local-0.0.1/contact_user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:31:30.000000 contact_user_external_local-0.0.1/contact_user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-08 08:31:30.000000 contact_user_external_local-0.0.1/contact_user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 08:31:30.000000 contact_user_external_local-0.0.1/contact_user_external_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 08:31:04.000000 contact_user_external_local-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:31:30.455188 contact_user_external_local-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-08 08:31:04.000000 contact_user_external_local-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:59:23.962563 contact_user_external_local-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 05:59:23.962563 contact_user_external_local-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 05:59:09.000000 contact_user_external_local-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:59:23.958563 contact_user_external_local-0.0.2/contact_user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:59:23.958563 contact_user_external_local-0.0.2/contact_user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:59:09.000000 contact_user_external_local-0.0.2/contact_user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-09 05:59:09.000000 contact_user_external_local-0.0.2/contact_user_external_local/src/contact_user_external_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-09 05:59:09.000000 contact_user_external_local-0.0.2/contact_user_external_local/src/contact_user_external_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:59:23.958563 contact_user_external_local-0.0.2/contact_user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 05:59:23.000000 contact_user_external_local-0.0.2/contact_user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 05:59:23.000000 contact_user_external_local-0.0.2/contact_user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:59:23.000000 contact_user_external_local-0.0.2/contact_user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 05:59:23.000000 contact_user_external_local-0.0.2/contact_user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 05:59:23.000000 contact_user_external_local-0.0.2/contact_user_external_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 05:59:09.000000 contact_user_external_local-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:59:23.962563 contact_user_external_local-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-09 05:59:09.000000 contact_user_external_local-0.0.2/setup.py
```

### Comparing `contact_user_external_local-0.0.1/contact_user_external_local/src/contact_user_external_local.py` & `contact_user_external_local-0.0.2/contact_user_external_local/src/contact_user_external_local.py`

 * *Files identical despite different names*

### Comparing `contact_user_external_local-0.0.1/contact_user_external_local/src/contact_user_external_local_constants.py` & `contact_user_external_local-0.0.2/contact_user_external_local/src/contact_user_external_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact_user_external_local-0.0.1/setup.py` & `contact_user_external_local-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
-
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.1',  # update only the minor version each time # https://pypi.org/project/contact-user-external-local/
+    version='0.0.2',  # update only the minor version each time # https://pypi.org/project/contact-user-external-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-user-external-local Python",
     long_description="PyPI Package for Circles contact-user-external-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/contact-user-external-local-python-package",
     package_dir={package_dir: f'{package_dir}/src'},
```

