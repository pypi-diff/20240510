# Comparing `tmp/phones_local-0.0.21.tar.gz` & `tmp/phones_local-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.21.tar", last modified: Fri May 10 10:01:37 2024, max compression
+gzip compressed data, was "phones_local-0.0.22.tar", last modified: Fri May 10 11:07:18 2024, max compression
```

## Comparing `phones_local-0.0.21.tar` & `phones_local-0.0.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:01:37.221043 phones_local-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 10:01:37.221043 phones_local-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 10:01:05.000000 phones_local-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:01:37.217043 phones_local-0.0.21/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:01:37.221043 phones_local-0.0.21/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:01:05.000000 phones_local-0.0.21/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-10 10:01:05.000000 phones_local-0.0.21/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-10 10:01:05.000000 phones_local-0.0.21/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:01:37.221043 phones_local-0.0.21/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 10:01:37.000000 phones_local-0.0.21/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-10 10:01:37.000000 phones_local-0.0.21/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:01:37.000000 phones_local-0.0.21/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 10:01:37.000000 phones_local-0.0.21/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 10:01:37.000000 phones_local-0.0.21/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 10:01:05.000000 phones_local-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:01:37.221043 phones_local-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 10:01:05.000000 phones_local-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:18.638459 phones_local-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 11:07:18.638459 phones_local-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 11:06:54.000000 phones_local-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:18.634459 phones_local-0.0.22/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:18.638459 phones_local-0.0.22/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:06:54.000000 phones_local-0.0.22/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-10 11:06:54.000000 phones_local-0.0.22/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-10 11:06:54.000000 phones_local-0.0.22/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:18.638459 phones_local-0.0.22/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 11:07:18.000000 phones_local-0.0.22/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-10 11:07:18.000000 phones_local-0.0.22/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:07:18.000000 phones_local-0.0.22/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 11:07:18.000000 phones_local-0.0.22/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 11:07:18.000000 phones_local-0.0.22/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 11:06:54.000000 phones_local-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:07:18.638459 phones_local-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 11:06:54.000000 phones_local-0.0.22/setup.py
```

### Comparing `phones_local-0.0.21/PKG-INFO` & `phones_local-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.21
+Version: 0.0.22
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.21/README.md` & `phones_local-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.21/phones_local/src/phone_local_constans.py` & `phones_local-0.0.22/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.21/phones_local/src/phones_local.py` & `phones_local-0.0.22/phones_local/src/phones_local.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.21/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.22/phones_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.21
+Version: 0.0.22
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.21/pyproject.toml` & `phones_local-0.0.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.21/setup.py` & `phones_local-0.0.22/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.21',  # https://pypi.org/project/phones-local/
+    version='0.0.22',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

