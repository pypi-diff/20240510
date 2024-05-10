# Comparing `tmp/pathway-0.dev0.tar.gz` & `tmp/pathway-0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathway-0.dev0.tar", last modified: Tue Jan 10 14:43:00 2023, max compression
+gzip compressed data, was "pathway-0.post1.tar", last modified: Thu Mar 23 13:31:57 2023, max compression
```

## Comparing `pathway-0.dev0.tar` & `pathway-0.post1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 embe     (2029317394) embe     (2029317394)        0 2023-01-10 14:43:00.456303 pathway-0.dev0/
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)     1255 2023-01-10 14:43:00.455705 pathway-0.dev0/PKG-INFO
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)      935 2023-01-10 14:04:59.000000 pathway-0.dev0/README.md
-drwxr-xr-x   0 embe     (2029317394) embe     (2029317394)        0 2023-01-10 14:43:00.450540 pathway-0.dev0/pathway/
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)       72 2023-01-10 14:04:59.000000 pathway-0.dev0/pathway/__init__.py
-drwxr-xr-x   0 embe     (2029317394) embe     (2029317394)        0 2023-01-10 14:43:00.454668 pathway-0.dev0/pathway.egg-info/
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)     1255 2023-01-10 14:43:00.000000 pathway-0.dev0/pathway.egg-info/PKG-INFO
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)      168 2023-01-10 14:43:00.000000 pathway-0.dev0/pathway.egg-info/SOURCES.txt
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)        1 2023-01-10 14:43:00.000000 pathway-0.dev0/pathway.egg-info/dependency_links.txt
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)        8 2023-01-10 14:43:00.000000 pathway-0.dev0/pathway.egg-info/top_level.txt
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)      401 2023-01-10 14:42:42.000000 pathway-0.dev0/pyproject.toml
--rw-r--r--   0 embe     (2029317394) embe     (2029317394)       38 2023-01-10 14:43:00.456486 pathway-0.dev0/setup.cfg
+drwxr-xr-x   0 embe     (2029317394) embe     (2029317394)        0 2023-03-23 13:31:57.569268 pathway-0.post1/
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)     1323 2023-03-23 13:31:57.568686 pathway-0.post1/PKG-INFO
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)      935 2023-03-06 14:38:26.000000 pathway-0.post1/README.md
+drwxr-xr-x   0 embe     (2029317394) embe     (2029317394)        0 2023-03-23 13:31:57.562602 pathway-0.post1/pathway/
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)     1649 2023-03-23 13:30:44.000000 pathway-0.post1/pathway/__init__.py
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)      440 2023-03-23 13:30:44.000000 pathway-0.post1/pathway/_stub_finder.py
+drwxr-xr-x   0 embe     (2029317394) embe     (2029317394)        0 2023-03-23 13:31:57.567590 pathway-0.post1/pathway.egg-info/
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)     1323 2023-03-23 13:31:57.000000 pathway-0.post1/pathway.egg-info/PKG-INFO
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)      192 2023-03-23 13:31:57.000000 pathway-0.post1/pathway.egg-info/SOURCES.txt
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)        1 2023-03-23 13:31:57.000000 pathway-0.post1/pathway.egg-info/dependency_links.txt
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)        8 2023-03-23 13:31:57.000000 pathway-0.post1/pathway.egg-info/top_level.txt
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)      457 2023-03-23 13:30:44.000000 pathway-0.post1/pyproject.toml
+-rw-r--r--   0 embe     (2029317394) embe     (2029317394)       38 2023-03-23 13:31:57.569450 pathway-0.post1/setup.cfg
```

### Comparing `pathway-0.dev0/PKG-INFO` & `pathway-0.post1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pathway
-Version: 0.dev0
+Version: 0.post1
 Summary: Pathway is a data processing framework which takes care of streaming data updates for you.
 Project-URL: Homepage, https://pathway.com/
 Project-URL: Documentation, https://pathway.com/developers/
+Project-URL: Troubleshooting, https://pathway.com/troubleshooting/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Welcome to [Pathway](https://pathway.com)!
 
 **Pathway is a data processing framework which takes care of streaming data updates for you.**
```

### Comparing `pathway-0.dev0/README.md` & `pathway-0.post1/README.md`

 * *Files identical despite different names*

### Comparing `pathway-0.dev0/pathway.egg-info/PKG-INFO` & `pathway-0.post1/pathway.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pathway
-Version: 0.dev0
+Version: 0.post1
 Summary: Pathway is a data processing framework which takes care of streaming data updates for you.
 Project-URL: Homepage, https://pathway.com/
 Project-URL: Documentation, https://pathway.com/developers/
+Project-URL: Troubleshooting, https://pathway.com/troubleshooting/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Welcome to [Pathway](https://pathway.com)!
 
 **Pathway is a data processing framework which takes care of streaming data updates for you.**
```

