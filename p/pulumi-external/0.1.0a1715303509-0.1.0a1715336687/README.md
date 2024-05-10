# Comparing `tmp/pulumi_external-0.1.0a1715303509.tar.gz` & `tmp/pulumi_external-0.1.0a1715336687.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_external-0.1.0a1715303509.tar", last modified: Fri May 10 01:26:17 2024, max compression
+gzip compressed data, was "pulumi_external-0.1.0a1715336687.tar", last modified: Fri May 10 10:27:31 2024, max compression
```

## Comparing `pulumi_external-0.1.0a1715303509.tar` & `pulumi_external-0.1.0a1715336687.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:26:17.680551 pulumi_external-0.1.0a1715303509/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-10 01:26:17.680551 pulumi_external-0.1.0a1715303509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:26:17.680551 pulumi_external-0.1.0a1715303509/pulumi_external/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/pulumi_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/pulumi_external/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/pulumi_external/get_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/pulumi_external/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/pulumi_external/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/pulumi_external/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:26:17.680551 pulumi_external-0.1.0a1715303509/pulumi_external.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-10 01:26:17.000000 pulumi_external-0.1.0a1715303509/pulumi_external.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-10 01:26:17.000000 pulumi_external-0.1.0a1715303509/pulumi_external.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:26:17.000000 pulumi_external-0.1.0a1715303509/pulumi_external.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:26:17.000000 pulumi_external-0.1.0a1715303509/pulumi_external.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 01:26:17.000000 pulumi_external-0.1.0a1715303509/pulumi_external.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 01:26:10.000000 pulumi_external-0.1.0a1715303509/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:26:17.680551 pulumi_external-0.1.0a1715303509/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.716563 pulumi_external-0.1.0a1715336687/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-10 10:27:31.712563 pulumi_external-0.1.0a1715336687/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.712563 pulumi_external-0.1.0a1715336687/pulumi_external/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/pulumi_external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/pulumi_external/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/pulumi_external/get_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/pulumi_external/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/pulumi_external/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/pulumi_external/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.712563 pulumi_external-0.1.0a1715336687/pulumi_external.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-10 10:27:31.000000 pulumi_external-0.1.0a1715336687/pulumi_external.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-10 10:27:31.000000 pulumi_external-0.1.0a1715336687/pulumi_external.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:27:31.000000 pulumi_external-0.1.0a1715336687/pulumi_external.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 10:27:31.000000 pulumi_external-0.1.0a1715336687/pulumi_external.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 10:27:31.000000 pulumi_external-0.1.0a1715336687/pulumi_external.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 10:27:24.000000 pulumi_external-0.1.0a1715336687/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:27:31.716563 pulumi_external-0.1.0a1715336687/setup.cfg
```

### Comparing `pulumi_external-0.1.0a1715303509/PKG-INFO` & `pulumi_external-0.1.0a1715336687/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_external
-Version: 0.1.0a1715303509
+Version: 0.1.0a1715336687
 Summary: A Pulumi package for creating and managing External cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-external
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_external-0.1.0a1715303509/README.md` & `pulumi_external-0.1.0a1715336687/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1715303509/pulumi_external/__init__.py` & `pulumi_external-0.1.0a1715336687/pulumi_external/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1715303509/pulumi_external/_utilities.py` & `pulumi_external-0.1.0a1715336687/pulumi_external/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1715303509/pulumi_external/get_external.py` & `pulumi_external-0.1.0a1715336687/pulumi_external/get_external.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1715303509/pulumi_external/provider.py` & `pulumi_external-0.1.0a1715336687/pulumi_external/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1715303509/pulumi_external.egg-info/PKG-INFO` & `pulumi_external-0.1.0a1715336687/pulumi_external.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_external
-Version: 0.1.0a1715303509
+Version: 0.1.0a1715336687
 Summary: A Pulumi package for creating and managing External cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-external
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_external-0.1.0a1715303509/pyproject.toml` & `pulumi_external-0.1.0a1715336687/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_external"
   description = "A Pulumi package for creating and managing External cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1715303509"
+  version = "0.1.0a1715336687"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-external"
 
 [build-system]
```

