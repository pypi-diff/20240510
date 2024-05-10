# Comparing `tmp/pulumi_null-0.1.0a1715061333.tar.gz` & `tmp/pulumi_null-0.1.0a1715234767.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_null-0.1.0a1715061333.tar", last modified: Tue May  7 06:04:35 2024, max compression
+gzip compressed data, was "pulumi_null-0.1.0a1715234767.tar", last modified: Thu May  9 06:14:16 2024, max compression
```

## Comparing `pulumi_null-0.1.0a1715061333.tar` & `pulumi_null-0.1.0a1715234767.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:04:35.128530 pulumi_null-0.1.0a1715061333/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-07 06:04:35.128530 pulumi_null-0.1.0a1715061333/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:04:35.124530 pulumi_null-0.1.0a1715061333/pulumi_null/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pulumi_null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pulumi_null/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pulumi_null/get_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pulumi_null/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pulumi_null/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pulumi_null/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pulumi_null/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:04:35.128530 pulumi_null-0.1.0a1715061333/pulumi_null.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-07 06:04:35.000000 pulumi_null-0.1.0a1715061333/pulumi_null.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 06:04:35.000000 pulumi_null-0.1.0a1715061333/pulumi_null.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 06:04:35.000000 pulumi_null-0.1.0a1715061333/pulumi_null.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 06:04:35.000000 pulumi_null-0.1.0a1715061333/pulumi_null.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 06:04:35.000000 pulumi_null-0.1.0a1715061333/pulumi_null.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-07 06:04:26.000000 pulumi_null-0.1.0a1715061333/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 06:04:35.128530 pulumi_null-0.1.0a1715061333/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:14:16.232259 pulumi_null-0.1.0a1715234767/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-09 06:14:16.232259 pulumi_null-0.1.0a1715234767/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:14:16.232259 pulumi_null-0.1.0a1715234767/pulumi_null/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pulumi_null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pulumi_null/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pulumi_null/get_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pulumi_null/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pulumi_null/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pulumi_null/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pulumi_null/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:14:16.232259 pulumi_null-0.1.0a1715234767/pulumi_null.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-09 06:14:16.000000 pulumi_null-0.1.0a1715234767/pulumi_null.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 06:14:16.000000 pulumi_null-0.1.0a1715234767/pulumi_null.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:14:16.000000 pulumi_null-0.1.0a1715234767/pulumi_null.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:14:16.000000 pulumi_null-0.1.0a1715234767/pulumi_null.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 06:14:16.000000 pulumi_null-0.1.0a1715234767/pulumi_null.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-09 06:14:08.000000 pulumi_null-0.1.0a1715234767/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:14:16.232259 pulumi_null-0.1.0a1715234767/setup.cfg
```

### Comparing `pulumi_null-0.1.0a1715061333/PKG-INFO` & `pulumi_null-0.1.0a1715234767/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_null
-Version: 0.1.0a1715061333
+Version: 0.1.0a1715234767
 Summary: A Pulumi package for creating and managing Null cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_null-0.1.0a1715061333/README.md` & `pulumi_null-0.1.0a1715234767/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.1.0a1715061333/pulumi_null/__init__.py` & `pulumi_null-0.1.0a1715234767/pulumi_null/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.1.0a1715061333/pulumi_null/_utilities.py` & `pulumi_null-0.1.0a1715234767/pulumi_null/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.1.0a1715061333/pulumi_null/get_data_source.py` & `pulumi_null-0.1.0a1715234767/pulumi_null/get_data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.1.0a1715061333/pulumi_null/provider.py` & `pulumi_null-0.1.0a1715234767/pulumi_null/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.1.0a1715061333/pulumi_null/resource.py` & `pulumi_null-0.1.0a1715234767/pulumi_null/resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.1.0a1715061333/pulumi_null.egg-info/PKG-INFO` & `pulumi_null-0.1.0a1715234767/pulumi_null.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_null
-Version: 0.1.0a1715061333
+Version: 0.1.0a1715234767
 Summary: A Pulumi package for creating and managing Null cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_null-0.1.0a1715061333/pyproject.toml` & `pulumi_null-0.1.0a1715234767/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_null"
   description = "A Pulumi package for creating and managing Null cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1715061333"
+  version = "0.1.0a1715234767"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-null"
 
 [build-system]
```

