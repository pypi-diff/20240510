# Comparing `tmp/pulumi_http-0.1.0a1715303697.tar.gz` & `tmp/pulumi_http-0.1.0a1715337278.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_http-0.1.0a1715303697.tar", last modified: Fri May 10 01:26:00 2024, max compression
+gzip compressed data, was "pulumi_http-0.1.0a1715337278.tar", last modified: Fri May 10 10:38:03 2024, max compression
```

## Comparing `pulumi_http-0.1.0a1715303697.tar` & `pulumi_http-0.1.0a1715337278.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:26:00.583678 pulumi_http-0.1.0a1715303697/
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-10 01:26:00.583678 pulumi_http-0.1.0a1715303697/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:26:00.579678 pulumi_http-0.1.0a1715303697/pulumi_http/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/get_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pulumi_http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:26:00.583678 pulumi_http-0.1.0a1715303697/pulumi_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-10 01:26:00.000000 pulumi_http-0.1.0a1715303697/pulumi_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-10 01:26:00.000000 pulumi_http-0.1.0a1715303697/pulumi_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:26:00.000000 pulumi_http-0.1.0a1715303697/pulumi_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:26:00.000000 pulumi_http-0.1.0a1715303697/pulumi_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 01:26:00.000000 pulumi_http-0.1.0a1715303697/pulumi_http.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 01:25:52.000000 pulumi_http-0.1.0a1715303697/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:26:00.583678 pulumi_http-0.1.0a1715303697/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:03.005715 pulumi_http-0.1.0a1715337278/
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-10 10:38:03.005715 pulumi_http-0.1.0a1715337278/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:03.005715 pulumi_http-0.1.0a1715337278/pulumi_http/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/get_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pulumi_http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:03.005715 pulumi_http-0.1.0a1715337278/pulumi_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-10 10:38:02.000000 pulumi_http-0.1.0a1715337278/pulumi_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-10 10:38:03.000000 pulumi_http-0.1.0a1715337278/pulumi_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:38:02.000000 pulumi_http-0.1.0a1715337278/pulumi_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 10:38:02.000000 pulumi_http-0.1.0a1715337278/pulumi_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 10:38:02.000000 pulumi_http-0.1.0a1715337278/pulumi_http.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 10:37:56.000000 pulumi_http-0.1.0a1715337278/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:38:03.005715 pulumi_http-0.1.0a1715337278/setup.cfg
```

### Comparing `pulumi_http-0.1.0a1715303697/PKG-INFO` & `pulumi_http-0.1.0a1715337278/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_http
-Version: 0.1.0a1715303697
+Version: 0.1.0a1715337278
 Summary: A Pulumi package for creating and managing HTTP cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-http
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_http-0.1.0a1715303697/README.md` & `pulumi_http-0.1.0a1715337278/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.1.0a1715303697/pulumi_http/__init__.py` & `pulumi_http-0.1.0a1715337278/pulumi_http/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.1.0a1715303697/pulumi_http/_inputs.py` & `pulumi_http-0.1.0a1715337278/pulumi_http/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.1.0a1715303697/pulumi_http/_utilities.py` & `pulumi_http-0.1.0a1715337278/pulumi_http/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.1.0a1715303697/pulumi_http/get_http.py` & `pulumi_http-0.1.0a1715337278/pulumi_http/get_http.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.1.0a1715303697/pulumi_http/outputs.py` & `pulumi_http-0.1.0a1715337278/pulumi_http/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.1.0a1715303697/pulumi_http/provider.py` & `pulumi_http-0.1.0a1715337278/pulumi_http/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_http-0.1.0a1715303697/pulumi_http.egg-info/PKG-INFO` & `pulumi_http-0.1.0a1715337278/pulumi_http.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_http
-Version: 0.1.0a1715303697
+Version: 0.1.0a1715337278
 Summary: A Pulumi package for creating and managing HTTP cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-http
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_http-0.1.0a1715303697/pyproject.toml` & `pulumi_http-0.1.0a1715337278/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_http"
   description = "A Pulumi package for creating and managing HTTP cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1715303697"
+  version = "0.1.0a1715337278"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-http"
 
 [build-system]
```

