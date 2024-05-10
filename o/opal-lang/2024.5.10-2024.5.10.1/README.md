# Comparing `tmp/opal_lang-2024.5.10.tar.gz` & `tmp/opal_lang-2024.5.10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal_lang-2024.5.10.tar", last modified: Fri May 10 14:21:47 2024, max compression
+gzip compressed data, was "opal_lang-2024.5.10.1.tar", last modified: Fri May 10 14:38:06 2024, max compression
```

## Comparing `opal_lang-2024.5.10.tar` & `opal_lang-2024.5.10.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.309762 opal_lang-2024.5.10/
--rw-rw-rw-   0        0        0     1087 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/LICENSE
--rw-rw-rw-   0        0        0    20204 2024-05-10 14:21:47.307760 opal_lang-2024.5.10/PKG-INFO
--rw-rw-rw-   0        0        0    19652 2024-05-10 13:45:28.000000 opal_lang-2024.5.10/README.md
--rw-rw-rw-   0        0        0      769 2024-05-10 13:08:55.000000 opal_lang-2024.5.10/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 14:21:47.309762 opal_lang-2024.5.10/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.101492 opal_lang-2024.5.10/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.126500 opal_lang-2024.5.10/src/opal/
--rw-rw-rw-   0        0        0     2939 2024-05-10 13:04:32.000000 opal_lang-2024.5.10/src/opal/__init__.py
--rw-rw-rw-   0        0        0    11988 2024-05-10 13:35:05.000000 opal_lang-2024.5.10/src/opal/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.148505 opal_lang-2024.5.10/src/opal/components/
--rw-rw-rw-   0        0        0    96398 2024-05-10 14:09:56.000000 opal_lang-2024.5.10/src/opal/components/Compiler.py
--rw-rw-rw-   0        0        0    13383 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/components/Tokens.py
--rw-rw-rw-   0        0        0     3138 2024-03-03 18:36:07.000000 opal_lang-2024.5.10/src/opal/components/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.173511 opal_lang-2024.5.10/src/opal/examples/
--rw-rw-rw-   0        0        0    10096 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/examples/2048.opal
--rw-rw-rw-   0        0        0      688 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/examples/fibonacci.opal
--rw-rw-rw-   0        0        0     5598 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/examples/fireworks.opal
--rw-rw-rw-   0        0        0     4776 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/examples/rain.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.253529 opal_lang-2024.5.10/src/opal/libs/
--rw-rw-rw-   0        0        0     8863 2024-05-10 13:05:53.000000 opal_lang-2024.5.10/src/opal/libs/Array.py
--rw-rw-rw-   0        0        0     1910 2024-02-15 14:08:31.000000 opal_lang-2024.5.10/src/opal/libs/Queue.py
--rw-rw-rw-   0        0        0     1680 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/Stack.py
--rw-rw-rw-   0        0        0     7650 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/Vector.py
--rw-rw-rw-   0        0        0     1675 2024-05-09 20:32:55.000000 opal_lang-2024.5.10/src/opal/libs/_internals.py
--rw-rw-rw-   0        0        0     6951 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/char.py
--rw-rw-rw-   0        0        0     5836 2024-03-19 20:29:16.000000 opal_lang-2024.5.10/src/opal/libs/fastSort.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.267532 opal_lang-2024.5.10/src/opal/libs/graphics/
--rw-rw-rw-   0        0        0    14759 2024-05-10 13:05:28.000000 opal_lang-2024.5.10/src/opal/libs/graphics/Graphics.py
--rw-rw-rw-   0        0        0      743 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/graphics/icon.png
--rw-rw-rw-   0        0        0     2650 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/helpers.opal
--rw-rw-rw-   0        0        0     9776 2023-12-22 14:44:21.000000 opal_lang-2024.5.10/src/opal/libs/merge.opal
--rw-rw-rw-   0        0        0     5759 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/sort.opal
--rw-rw-rw-   0        0        0     2810 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/stableSort.opal
--rw-rw-rw-   0        0        0     7145 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/libs/std.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.281752 opal_lang-2024.5.10/src/opal/runner/
--rw-rw-rw-   0        0        0      772 2024-05-09 20:03:03.000000 opal_lang-2024.5.10/src/opal/runner/build.py
--rw-rw-rw-   0        0        0   270398 2023-12-15 15:23:18.000000 opal_lang-2024.5.10/src/opal/runner/icon.ico
-drwxrwxrwx   0        0        0        0 2024-05-10 14:21:47.306759 opal_lang-2024.5.10/src/opal_lang.egg-info/
--rw-rw-rw-   0        0        0    20204 2024-05-10 14:21:47.000000 opal_lang-2024.5.10/src/opal_lang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2024-05-10 14:21:47.000000 opal_lang-2024.5.10/src/opal_lang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:21:47.000000 opal_lang-2024.5.10/src/opal_lang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-10 14:21:47.000000 opal_lang-2024.5.10/src/opal_lang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-10 14:21:47.000000 opal_lang-2024.5.10/src/opal_lang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.762336 opal_lang-2024.5.10.1/
+-rw-rw-rw-   0        0        0     1087 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/LICENSE
+-rw-rw-rw-   0        0        0    20089 2024-05-10 14:38:06.760335 opal_lang-2024.5.10.1/PKG-INFO
+-rw-rw-rw-   0        0        0    19535 2024-05-10 14:37:28.000000 opal_lang-2024.5.10.1/README.md
+-rw-rw-rw-   0        0        0      771 2024-05-10 14:36:56.000000 opal_lang-2024.5.10.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:38:06.762336 opal_lang-2024.5.10.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.609152 opal_lang-2024.5.10.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.621728 opal_lang-2024.5.10.1/src/opal/
+-rw-rw-rw-   0        0        0     2939 2024-05-10 13:04:32.000000 opal_lang-2024.5.10.1/src/opal/__init__.py
+-rw-rw-rw-   0        0        0    11988 2024-05-10 13:35:05.000000 opal_lang-2024.5.10.1/src/opal/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.627034 opal_lang-2024.5.10.1/src/opal/components/
+-rw-rw-rw-   0        0        0    96398 2024-05-10 14:37:02.000000 opal_lang-2024.5.10.1/src/opal/components/Compiler.py
+-rw-rw-rw-   0        0        0    13383 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/components/Tokens.py
+-rw-rw-rw-   0        0        0     3138 2024-03-03 18:36:07.000000 opal_lang-2024.5.10.1/src/opal/components/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.665987 opal_lang-2024.5.10.1/src/opal/examples/
+-rw-rw-rw-   0        0        0    10096 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/examples/2048.opal
+-rw-rw-rw-   0        0        0      688 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/examples/fibonacci.opal
+-rw-rw-rw-   0        0        0     5598 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/examples/fireworks.opal
+-rw-rw-rw-   0        0        0     4776 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/examples/rain.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.718355 opal_lang-2024.5.10.1/src/opal/libs/
+-rw-rw-rw-   0        0        0     8863 2024-05-10 13:05:53.000000 opal_lang-2024.5.10.1/src/opal/libs/Array.py
+-rw-rw-rw-   0        0        0     1910 2024-02-15 14:08:31.000000 opal_lang-2024.5.10.1/src/opal/libs/Queue.py
+-rw-rw-rw-   0        0        0     1680 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/Stack.py
+-rw-rw-rw-   0        0        0     7650 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/Vector.py
+-rw-rw-rw-   0        0        0     1675 2024-05-09 20:32:55.000000 opal_lang-2024.5.10.1/src/opal/libs/_internals.py
+-rw-rw-rw-   0        0        0     6951 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/char.py
+-rw-rw-rw-   0        0        0     5836 2024-03-19 20:29:16.000000 opal_lang-2024.5.10.1/src/opal/libs/fastSort.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.725165 opal_lang-2024.5.10.1/src/opal/libs/graphics/
+-rw-rw-rw-   0        0        0    14759 2024-05-10 13:05:28.000000 opal_lang-2024.5.10.1/src/opal/libs/graphics/Graphics.py
+-rw-rw-rw-   0        0        0      743 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/graphics/icon.png
+-rw-rw-rw-   0        0        0     2650 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/helpers.opal
+-rw-rw-rw-   0        0        0     9776 2023-12-22 14:44:21.000000 opal_lang-2024.5.10.1/src/opal/libs/merge.opal
+-rw-rw-rw-   0        0        0     5759 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/sort.opal
+-rw-rw-rw-   0        0        0     2810 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/stableSort.opal
+-rw-rw-rw-   0        0        0     7145 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/libs/std.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.735123 opal_lang-2024.5.10.1/src/opal/runner/
+-rw-rw-rw-   0        0        0      772 2024-05-09 20:03:03.000000 opal_lang-2024.5.10.1/src/opal/runner/build.py
+-rw-rw-rw-   0        0        0   270398 2023-12-15 15:23:18.000000 opal_lang-2024.5.10.1/src/opal/runner/icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-10 14:38:06.759335 opal_lang-2024.5.10.1/src/opal_lang.egg-info/
+-rw-rw-rw-   0        0        0    20089 2024-05-10 14:38:06.000000 opal_lang-2024.5.10.1/src/opal_lang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-05-10 14:38:06.000000 opal_lang-2024.5.10.1/src/opal_lang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:38:06.000000 opal_lang-2024.5.10.1/src/opal_lang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-10 14:38:06.000000 opal_lang-2024.5.10.1/src/opal_lang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-10 14:38:06.000000 opal_lang-2024.5.10.1/src/opal_lang.egg-info/top_level.txt
```

### Comparing `opal_lang-2024.5.10/LICENSE` & `opal_lang-2024.5.10.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/PKG-INFO` & `opal_lang-2024.5.10.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-lang
-Version: 2024.5.10
+Version: 2024.5.10.1
 Summary: A programming language based on Python and Cython
 Project-URL: Homepage, https://github.com/thatsOven/opal-lang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -19,18 +19,17 @@
     
 # opal 
 opal is a transcompiled programming language based on Python and Cython. 
 
 # Installation
 To install opal on your machine, execute these commands:
 ```
-pip install opal-lang --user
+pip install opal-lang
 python -m opal build
 ```
-User installation is necessary due to permission issues during the process of building the standard library.
 
 Note that you might need to install a C compiler, as Cython will be installed as a dependency.
 
 On Windows, after the building process is complete, it's possible to add the opal folder to PATH to have a global `opal` executable.
 
 # Compiler usage
 [ ] = optional
```

### Comparing `opal_lang-2024.5.10/README.md` & `opal_lang-2024.5.10.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
     
 # opal 
 opal is a transcompiled programming language based on Python and Cython. 
 
 # Installation
 To install opal on your machine, execute these commands:
 ```
-pip install opal-lang --user
+pip install opal-lang
 python -m opal build
 ```
-User installation is necessary due to permission issues during the process of building the standard library.
 
 Note that you might need to install a C compiler, as Cython will be installed as a dependency.
 
 On Windows, after the building process is complete, it's possible to add the opal folder to PATH to have a global `opal` executable.
 
 # Compiler usage
 [ ] = optional
```

### Comparing `opal_lang-2024.5.10/pyproject.toml` & `opal_lang-2024.5.10.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "*" = ["*.opal", "*.ico", "*.png"]
 
 [project]
 name = "opal-lang"
-version = "2024.5.10"
+version = "2024.5.10.1"
 description = "A programming language based on Python and Cython"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `opal_lang-2024.5.10/src/opal/__init__.py` & `opal_lang-2024.5.10.1/src/opal/__init__.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/__main__.py` & `opal_lang-2024.5.10.1/src/opal/__main__.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/components/Compiler.py` & `opal_lang-2024.5.10.1/src/opal/components/Compiler.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/components/Tokens.py` & `opal_lang-2024.5.10.1/src/opal/components/Tokens.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/components/utils.py` & `opal_lang-2024.5.10.1/src/opal/components/utils.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/examples/2048.opal` & `opal_lang-2024.5.10.1/src/opal/examples/2048.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/examples/fibonacci.opal` & `opal_lang-2024.5.10.1/src/opal/examples/fibonacci.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/examples/fireworks.opal` & `opal_lang-2024.5.10.1/src/opal/examples/fireworks.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/examples/rain.opal` & `opal_lang-2024.5.10.1/src/opal/examples/rain.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/Array.py` & `opal_lang-2024.5.10.1/src/opal/libs/Array.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/Queue.py` & `opal_lang-2024.5.10.1/src/opal/libs/Queue.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/Stack.py` & `opal_lang-2024.5.10.1/src/opal/libs/Stack.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/Vector.py` & `opal_lang-2024.5.10.1/src/opal/libs/Vector.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/_internals.py` & `opal_lang-2024.5.10.1/src/opal/libs/_internals.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/char.py` & `opal_lang-2024.5.10.1/src/opal/libs/char.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/fastSort.opal` & `opal_lang-2024.5.10.1/src/opal/libs/fastSort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/graphics/Graphics.py` & `opal_lang-2024.5.10.1/src/opal/libs/graphics/Graphics.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/graphics/icon.png` & `opal_lang-2024.5.10.1/src/opal/libs/graphics/icon.png`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/helpers.opal` & `opal_lang-2024.5.10.1/src/opal/libs/helpers.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/merge.opal` & `opal_lang-2024.5.10.1/src/opal/libs/merge.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/sort.opal` & `opal_lang-2024.5.10.1/src/opal/libs/sort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/stableSort.opal` & `opal_lang-2024.5.10.1/src/opal/libs/stableSort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/libs/std.opal` & `opal_lang-2024.5.10.1/src/opal/libs/std.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/runner/build.py` & `opal_lang-2024.5.10.1/src/opal/runner/build.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal/runner/icon.ico` & `opal_lang-2024.5.10.1/src/opal/runner/icon.ico`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10/src/opal_lang.egg-info/PKG-INFO` & `opal_lang-2024.5.10.1/src/opal_lang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-lang
-Version: 2024.5.10
+Version: 2024.5.10.1
 Summary: A programming language based on Python and Cython
 Project-URL: Homepage, https://github.com/thatsOven/opal-lang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -19,18 +19,17 @@
     
 # opal 
 opal is a transcompiled programming language based on Python and Cython. 
 
 # Installation
 To install opal on your machine, execute these commands:
 ```
-pip install opal-lang --user
+pip install opal-lang
 python -m opal build
 ```
-User installation is necessary due to permission issues during the process of building the standard library.
 
 Note that you might need to install a C compiler, as Cython will be installed as a dependency.
 
 On Windows, after the building process is complete, it's possible to add the opal folder to PATH to have a global `opal` executable.
 
 # Compiler usage
 [ ] = optional
```

### Comparing `opal_lang-2024.5.10/src/opal_lang.egg-info/SOURCES.txt` & `opal_lang-2024.5.10.1/src/opal_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

