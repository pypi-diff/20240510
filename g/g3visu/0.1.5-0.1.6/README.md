# Comparing `tmp/g3visu-0.1.5.tar.gz` & `tmp/g3visu-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3visu-0.1.5.tar", last modified: Fri May 10 09:29:47 2024, max compression
+gzip compressed data, was "g3visu-0.1.6.tar", last modified: Fri May 10 09:41:01 2024, max compression
```

## Comparing `g3visu-0.1.5.tar` & `g3visu-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:29:47.135039 g3visu-0.1.5/
--rw-rw-rw-   0        0        0     1091 2024-04-29 14:15:00.000000 g3visu-0.1.5/LICENCE
--rw-rw-rw-   0        0        0     1759 2024-05-10 09:29:47.135039 g3visu-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-04-30 08:21:52.000000 g3visu-0.1.5/README.md
--rw-rw-rw-   0        0        0     1520 2024-05-10 09:28:59.000000 g3visu-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 09:29:47.135039 g3visu-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 09:29:47.088794 g3visu-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 09:29:47.088794 g3visu-0.1.5/src/g3visu/
-drwxrwxrwx   0        0        0        0 2024-05-10 09:29:47.088794 g3visu-0.1.5/src/g3visu/site/
-drwxrwxrwx   0        0        0        0 2024-05-10 09:29:47.135039 g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-05-10 09:29:47.000000 g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2024-05-10 09:29:47.000000 g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:29:47.000000 g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-10 09:29:47.000000 g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      143 2024-05-10 09:29:47.000000 g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:29:47.000000 g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.220225 g3visu-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 14:15:00.000000 g3visu-0.1.6/LICENCE
+-rw-rw-rw-   0        0        0     1759 2024-05-10 09:41:01.217545 g3visu-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-30 08:21:52.000000 g3visu-0.1.6/README.md
+-rw-rw-rw-   0        0        0     1508 2024-05-10 09:39:06.000000 g3visu-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:41:01.221171 g3visu-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.093161 g3visu-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.121443 g3visu-0.1.6/src/g3visu/
+-rw-rw-rw-   0        0        0      289 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/__init__.py
+-rw-rw-rw-   0        0        0     5593 2024-04-30 12:55:51.000000 g3visu-0.1.6/src/g3visu/_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.163318 g3visu-0.1.6/src/g3visu/meta/
+-rw-rw-rw-   0        0        0       99 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/meta/__init__.py
+-rw-rw-rw-   0        0        0     3591 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/meta/_meta.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.178067 g3visu-0.1.6/src/g3visu/site/
+-rw-rw-rw-   0        0        0      120 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/site/__init__.py
+-rw-rw-rw-   0        0        0    22979 2024-05-10 08:59:38.000000 g3visu-0.1.6/src/g3visu/site/_site_svg.py
+-rw-rw-rw-   0        0        0    11402 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/site/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.198073 g3visu-0.1.6/src/g3visu/typeinfo/
+-rw-rw-rw-   0        0        0      411 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/typeinfo/__init__.py
+-rw-rw-rw-   0        0        0     1310 2024-04-30 12:56:03.000000 g3visu-0.1.6/src/g3visu/typeinfo/_list_operations.py
+-rw-rw-rw-   0        0        0    19489 2024-04-30 12:56:11.000000 g3visu-0.1.6/src/g3visu/typeinfo/_typeinfo.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/typeinfo/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.204645 g3visu-0.1.6/src/g3visu/utils/
+-rw-rw-rw-   0        0        0      308 2024-04-29 14:15:00.000000 g3visu-0.1.6/src/g3visu/utils/__init__.py
+-rw-rw-rw-   0        0        0     7709 2024-04-30 08:21:52.000000 g3visu-0.1.6/src/g3visu/utils/_download_from_sites.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:41:01.212228 g3visu-0.1.6/src/g3visu.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-05-10 09:41:01.000000 g3visu-0.1.6/src/g3visu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2024-05-10 09:41:01.000000 g3visu-0.1.6/src/g3visu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:41:01.000000 g3visu-0.1.6/src/g3visu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-10 09:41:01.000000 g3visu-0.1.6/src/g3visu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      143 2024-05-10 09:41:01.000000 g3visu-0.1.6/src/g3visu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 09:41:01.000000 g3visu-0.1.6/src/g3visu.egg-info/top_level.txt
```

### Comparing `g3visu-0.1.5/LICENCE` & `g3visu-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.5/PKG-INFO` & `g3visu-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3visu
-Version: 0.1.5
+Version: 0.1.6
 Summary: System G3 Visualization files' parsers and generators
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Visu.git
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3visu-0.1.5/pyproject.toml` & `g3visu-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3visu"
-version = "0.1.5"
+version = "0.1.6"
 description = "System G3 Visualization files' parsers and generators"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name = "Elektroline a.s." },
 ]
 classifiers = [
@@ -51,12 +51,12 @@
 package_dir = {"" = "src"}
 
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-where = ["src/g3visu/site"]
+where = ["src"]
 
 [tool.setuptools.package-data]
 g3visu = ["site.svg"]
```

### Comparing `g3visu-0.1.5/src/g3visu/site/g3visu.egg-info/PKG-INFO` & `g3visu-0.1.6/src/g3visu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3visu
-Version: 0.1.5
+Version: 0.1.6
 Summary: System G3 Visualization files' parsers and generators
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Visu.git
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

