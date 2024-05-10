# Comparing `tmp/opal_lang-2024.5.10.4.tar.gz` & `tmp/opal_lang-2024.5.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal_lang-2024.5.10.4.tar", last modified: Fri May 10 19:50:37 2024, max compression
+gzip compressed data, was "opal_lang-2024.5.10.5.tar", last modified: Fri May 10 21:02:20 2024, max compression
```

## Comparing `opal_lang-2024.5.10.4.tar` & `opal_lang-2024.5.10.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.925838 opal_lang-2024.5.10.4/
--rw-rw-rw-   0        0        0     1087 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/LICENSE
--rw-rw-rw-   0        0        0    20114 2024-05-10 19:50:37.923836 opal_lang-2024.5.10.4/PKG-INFO
--rw-rw-rw-   0        0        0    19535 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/README.md
--rw-rw-rw-   0        0        0      788 2024-05-10 19:50:10.000000 opal_lang-2024.5.10.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 19:50:37.925838 opal_lang-2024.5.10.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.850820 opal_lang-2024.5.10.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.857822 opal_lang-2024.5.10.4/src/opal/
--rw-rw-rw-   0        0        0     2939 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/__init__.py
--rw-rw-rw-   0        0        0    12134 2024-05-10 19:41:58.000000 opal_lang-2024.5.10.4/src/opal/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.862823 opal_lang-2024.5.10.4/src/opal/components/
--rw-rw-rw-   0        0        0    96441 2024-05-10 19:50:15.000000 opal_lang-2024.5.10.4/src/opal/components/Compiler.py
--rw-rw-rw-   0        0        0    13383 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/components/Tokens.py
--rw-rw-rw-   0        0        0     3138 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/components/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.869824 opal_lang-2024.5.10.4/src/opal/examples/
--rw-rw-rw-   0        0        0    10096 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/examples/2048.opal
--rw-rw-rw-   0        0        0      688 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/examples/fibonacci.opal
--rw-rw-rw-   0        0        0     5598 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/examples/fireworks.opal
--rw-rw-rw-   0        0        0     4776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/examples/rain.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.889828 opal_lang-2024.5.10.4/src/opal/libs/
--rw-rw-rw-   0        0        0     8863 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/Array.py
--rw-rw-rw-   0        0        0     1910 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/Queue.py
--rw-rw-rw-   0        0        0     1680 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/Stack.py
--rw-rw-rw-   0        0        0     7650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/Vector.py
--rw-rw-rw-   0        0        0     1675 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/_internals.py
--rw-rw-rw-   0        0        0     6951 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/char.py
--rw-rw-rw-   0        0        0     5836 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/fastSort.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.892829 opal_lang-2024.5.10.4/src/opal/libs/graphics/
--rw-rw-rw-   0        0        0    14759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/graphics/Graphics.py
--rw-rw-rw-   0        0        0      743 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/graphics/icon.png
--rw-rw-rw-   0        0        0     2650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/helpers.opal
--rw-rw-rw-   0        0        0     9776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/merge.opal
--rw-rw-rw-   0        0        0     5759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/sort.opal
--rw-rw-rw-   0        0        0     2810 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/stableSort.opal
--rw-rw-rw-   0        0        0     7145 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/libs/std.opal
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.896830 opal_lang-2024.5.10.4/src/opal/runner/
--rw-rw-rw-   0        0        0      772 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/runner/build.py
--rw-rw-rw-   0        0        0   270398 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.4/src/opal/runner/icon.ico
-drwxrwxrwx   0        0        0        0 2024-05-10 19:50:37.922835 opal_lang-2024.5.10.4/src/opal_lang.egg-info/
--rw-rw-rw-   0        0        0    20114 2024-05-10 19:50:37.000000 opal_lang-2024.5.10.4/src/opal_lang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2024-05-10 19:50:37.000000 opal_lang-2024.5.10.4/src/opal_lang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 19:50:37.000000 opal_lang-2024.5.10.4/src/opal_lang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-10 19:50:37.000000 opal_lang-2024.5.10.4/src/opal_lang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-10 19:50:37.000000 opal_lang-2024.5.10.4/src/opal_lang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.228132 opal_lang-2024.5.10.5/
+-rw-rw-rw-   0        0        0     1087 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/LICENSE
+-rw-rw-rw-   0        0        0    20142 2024-05-10 21:02:20.227131 opal_lang-2024.5.10.5/PKG-INFO
+-rw-rw-rw-   0        0        0    19535 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/README.md
+-rw-rw-rw-   0        0        0      808 2024-05-10 21:00:23.000000 opal_lang-2024.5.10.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 21:02:20.228132 opal_lang-2024.5.10.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.073922 opal_lang-2024.5.10.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.087556 opal_lang-2024.5.10.5/src/opal/
+-rw-rw-rw-   0        0        0     2939 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/__init__.py
+-rw-rw-rw-   0        0        0    12134 2024-05-10 19:41:58.000000 opal_lang-2024.5.10.5/src/opal/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.091559 opal_lang-2024.5.10.5/src/opal/components/
+-rw-rw-rw-   0        0        0    96441 2024-05-10 21:00:35.000000 opal_lang-2024.5.10.5/src/opal/components/Compiler.py
+-rw-rw-rw-   0        0        0    13383 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/components/Tokens.py
+-rw-rw-rw-   0        0        0     3138 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/components/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.129109 opal_lang-2024.5.10.5/src/opal/examples/
+-rw-rw-rw-   0        0        0    10096 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/examples/2048.opal
+-rw-rw-rw-   0        0        0      688 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/examples/fibonacci.opal
+-rw-rw-rw-   0        0        0     5598 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/examples/fireworks.opal
+-rw-rw-rw-   0        0        0     4776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/examples/rain.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.184121 opal_lang-2024.5.10.5/src/opal/libs/
+-rw-rw-rw-   0        0        0     8863 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/Array.py
+-rw-rw-rw-   0        0        0     1910 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/Queue.py
+-rw-rw-rw-   0        0        0     1680 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/Stack.py
+-rw-rw-rw-   0        0        0     7650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/Vector.py
+-rw-rw-rw-   0        0        0     1675 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/_internals.py
+-rw-rw-rw-   0        0        0     6951 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/char.py
+-rw-rw-rw-   0        0        0     5836 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/fastSort.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.191122 opal_lang-2024.5.10.5/src/opal/libs/graphics/
+-rw-rw-rw-   0        0        0    14759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/graphics/Graphics.py
+-rw-rw-rw-   0        0        0      743 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/graphics/icon.png
+-rw-rw-rw-   0        0        0     2650 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/helpers.opal
+-rw-rw-rw-   0        0        0     9776 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/merge.opal
+-rw-rw-rw-   0        0        0     5759 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/sort.opal
+-rw-rw-rw-   0        0        0     2810 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/stableSort.opal
+-rw-rw-rw-   0        0        0     7145 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/libs/std.opal
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.200124 opal_lang-2024.5.10.5/src/opal/runner/
+-rw-rw-rw-   0        0        0      772 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/runner/build.py
+-rw-rw-rw-   0        0        0   270398 2024-05-10 18:24:50.000000 opal_lang-2024.5.10.5/src/opal/runner/icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-10 21:02:20.225130 opal_lang-2024.5.10.5/src/opal_lang.egg-info/
+-rw-rw-rw-   0        0        0    20142 2024-05-10 21:02:20.000000 opal_lang-2024.5.10.5/src/opal_lang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-05-10 21:02:20.000000 opal_lang-2024.5.10.5/src/opal_lang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 21:02:20.000000 opal_lang-2024.5.10.5/src/opal_lang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-10 21:02:20.000000 opal_lang-2024.5.10.5/src/opal_lang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-10 21:02:20.000000 opal_lang-2024.5.10.5/src/opal_lang.egg-info/top_level.txt
```

### Comparing `opal_lang-2024.5.10.4/LICENSE` & `opal_lang-2024.5.10.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/PKG-INFO` & `opal_lang-2024.5.10.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: opal-lang
-Version: 2024.5.10.4
+Version: 2024.5.10.5
 Summary: A programming language based on Python and Cython
 Project-URL: Homepage, https://github.com/thatsOven/opal-lang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyinstaller
 Requires-Dist: colorama
 Requires-Dist: pygame
 Requires-Dist: numpy
 Requires-Dist: typeguard
 Requires-Dist: Cython
 Requires-Dist: ianthe>=2023.12.17
```

### Comparing `opal_lang-2024.5.10.4/README.md` & `opal_lang-2024.5.10.5/README.md`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/pyproject.toml` & `opal_lang-2024.5.10.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "*" = ["*.opal", "*.ico", "*.png"]
 
 [project]
 name = "opal-lang"
-version = "2024.5.10.4"
+version = "2024.5.10.5"
 description = "A programming language based on Python and Cython"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "pyinstaller",
     "colorama",
     "pygame",
     "numpy",
     "typeguard",
     "Cython",
     "ianthe>=2023.12.17"
 ]
```

### Comparing `opal_lang-2024.5.10.4/src/opal/__init__.py` & `opal_lang-2024.5.10.5/src/opal/__init__.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/__main__.py` & `opal_lang-2024.5.10.5/src/opal/__main__.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/components/Compiler.py` & `opal_lang-2024.5.10.5/src/opal/components/Compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from importlib import import_module
 from traceback import format_exception
 import os
 
 from opal.components.utils  import *
 from opal.components.Tokens import *
 
-VERSION = (2024, 5, 10, 4)
+VERSION = (2024, 5, 10, 5)
 SET_OPS = ("+=", "-=", "**=", "//=", "*=", "/=", "%=", "&=", "|=", "^=", ">>=", "<<=", "@=", "=")
 CYTHON_TYPES = (
     "short", "int", "long", "long long", "float", "bint",
     "double", "long double", "list", "object", "str", 
     "tuple", "dict", "range", "bytes", "bytearray", "complex"
 )
 CYTHON_FN_TYPES = CYTHON_TYPES + ("void", "bool")
```

### Comparing `opal_lang-2024.5.10.4/src/opal/components/Tokens.py` & `opal_lang-2024.5.10.5/src/opal/components/Tokens.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/components/utils.py` & `opal_lang-2024.5.10.5/src/opal/components/utils.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/examples/2048.opal` & `opal_lang-2024.5.10.5/src/opal/examples/2048.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/examples/fibonacci.opal` & `opal_lang-2024.5.10.5/src/opal/examples/fibonacci.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/examples/fireworks.opal` & `opal_lang-2024.5.10.5/src/opal/examples/fireworks.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/examples/rain.opal` & `opal_lang-2024.5.10.5/src/opal/examples/rain.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/Array.py` & `opal_lang-2024.5.10.5/src/opal/libs/Array.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/Queue.py` & `opal_lang-2024.5.10.5/src/opal/libs/Queue.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/Stack.py` & `opal_lang-2024.5.10.5/src/opal/libs/Stack.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/Vector.py` & `opal_lang-2024.5.10.5/src/opal/libs/Vector.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/_internals.py` & `opal_lang-2024.5.10.5/src/opal/libs/_internals.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/char.py` & `opal_lang-2024.5.10.5/src/opal/libs/char.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/fastSort.opal` & `opal_lang-2024.5.10.5/src/opal/libs/fastSort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/graphics/Graphics.py` & `opal_lang-2024.5.10.5/src/opal/libs/graphics/Graphics.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/graphics/icon.png` & `opal_lang-2024.5.10.5/src/opal/libs/graphics/icon.png`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/helpers.opal` & `opal_lang-2024.5.10.5/src/opal/libs/helpers.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/merge.opal` & `opal_lang-2024.5.10.5/src/opal/libs/merge.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/sort.opal` & `opal_lang-2024.5.10.5/src/opal/libs/sort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/stableSort.opal` & `opal_lang-2024.5.10.5/src/opal/libs/stableSort.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/libs/std.opal` & `opal_lang-2024.5.10.5/src/opal/libs/std.opal`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/runner/build.py` & `opal_lang-2024.5.10.5/src/opal/runner/build.py`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal/runner/icon.ico` & `opal_lang-2024.5.10.5/src/opal/runner/icon.ico`

 * *Files identical despite different names*

### Comparing `opal_lang-2024.5.10.4/src/opal_lang.egg-info/PKG-INFO` & `opal_lang-2024.5.10.5/src/opal_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: opal-lang
-Version: 2024.5.10.4
+Version: 2024.5.10.5
 Summary: A programming language based on Python and Cython
 Project-URL: Homepage, https://github.com/thatsOven/opal-lang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyinstaller
 Requires-Dist: colorama
 Requires-Dist: pygame
 Requires-Dist: numpy
 Requires-Dist: typeguard
 Requires-Dist: Cython
 Requires-Dist: ianthe>=2023.12.17
```

### Comparing `opal_lang-2024.5.10.4/src/opal_lang.egg-info/SOURCES.txt` & `opal_lang-2024.5.10.5/src/opal_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

