# Comparing `tmp/glitch-python-hcl2-0.2.0.tar.gz` & `tmp/glitch-python-hcl2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glitch-python-hcl2-0.2.0.tar", last modified: Fri May 10 11:32:28 2024, max compression
+gzip compressed data, was "glitch-python-hcl2-0.2.1.tar", last modified: Fri May 10 11:47:11 2024, max compression
```

## Comparing `glitch-python-hcl2-0.2.0.tar` & `glitch-python-hcl2-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4902 2024-05-09 16:10:12.000000 glitch-python-hcl2-0.2.0/CHANGELOG.md
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1063 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/LICENSE
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      141 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/MANIFEST.in
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4215 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/PKG-INFO
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3311 2024-05-09 16:11:03.000000 glitch-python-hcl2-0.2.0/README.md
-drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/
--rw-r--r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4215 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/PKG-INFO
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      370 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/SOURCES.txt
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)        1 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/dependency_links.txt
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       17 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/requires.txt
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       10 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/top_level.txt
-drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/hcl2/
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      176 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/__init__.py
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3905 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/__main__.py
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1173 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/api.py
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3450 2024-05-09 16:10:12.000000 glitch-python-hcl2-0.2.0/hcl2/hcl2.lark
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      378 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/parser.py
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/py.typed
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)    14911 2024-05-10 10:39:04.000000 glitch-python-hcl2-0.2.0/hcl2/transformer.py
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       38 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/setup.cfg
--rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1701 2024-05-10 11:32:15.000000 glitch-python-hcl2-0.2.0/setup.py
+drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:47:11.790426 glitch-python-hcl2-0.2.1/
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4902 2024-05-09 16:10:12.000000 glitch-python-hcl2-0.2.1/CHANGELOG.md
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1063 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.1/LICENSE
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      141 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.1/MANIFEST.in
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4215 2024-05-10 11:47:11.790426 glitch-python-hcl2-0.2.1/PKG-INFO
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3311 2024-05-09 16:11:03.000000 glitch-python-hcl2-0.2.1/README.md
+drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:47:11.790426 glitch-python-hcl2-0.2.1/glitch_python_hcl2.egg-info/
+-rw-r--r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4215 2024-05-10 11:47:11.000000 glitch-python-hcl2-0.2.1/glitch_python_hcl2.egg-info/PKG-INFO
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      370 2024-05-10 11:47:11.000000 glitch-python-hcl2-0.2.1/glitch_python_hcl2.egg-info/SOURCES.txt
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)        1 2024-05-10 11:47:11.000000 glitch-python-hcl2-0.2.1/glitch_python_hcl2.egg-info/dependency_links.txt
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       17 2024-05-10 11:47:11.000000 glitch-python-hcl2-0.2.1/glitch_python_hcl2.egg-info/requires.txt
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       10 2024-05-10 11:47:11.000000 glitch-python-hcl2-0.2.1/glitch_python_hcl2.egg-info/top_level.txt
+drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:47:11.790426 glitch-python-hcl2-0.2.1/hcl2/
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      176 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.1/hcl2/__init__.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3905 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.1/hcl2/__main__.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1173 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.1/hcl2/api.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3450 2024-05-09 16:10:12.000000 glitch-python-hcl2-0.2.1/hcl2/hcl2.lark
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      378 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.1/hcl2/parser.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.1/hcl2/py.typed
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)    14911 2024-05-10 10:39:04.000000 glitch-python-hcl2-0.2.1/hcl2/transformer.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       38 2024-05-10 11:47:11.790426 glitch-python-hcl2-0.2.1/setup.cfg
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1743 2024-05-10 11:46:58.000000 glitch-python-hcl2-0.2.1/setup.py
```

### Comparing `glitch-python-hcl2-0.2.0/CHANGELOG.md` & `glitch-python-hcl2-0.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.2.0/LICENSE` & `glitch-python-hcl2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.2.0/PKG-INFO` & `glitch-python-hcl2-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glitch-python-hcl2
-Version: 0.2.0
+Version: 0.2.1
 Summary: A parser for HCL2
 Home-page: https://github.com/joaotgoncalves/python-hcl2
 Author: João Gonçalves
 Author-email: joao.marques.goncalves@tecnico.ulisboa.pt
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `glitch-python-hcl2-0.2.0/README.md` & `glitch-python-hcl2-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/PKG-INFO` & `glitch-python-hcl2-0.2.1/glitch_python_hcl2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glitch-python-hcl2
-Version: 0.2.0
+Version: 0.2.1
 Summary: A parser for HCL2
 Home-page: https://github.com/joaotgoncalves/python-hcl2
 Author: João Gonçalves
 Author-email: joao.marques.goncalves@tecnico.ulisboa.pt
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `glitch-python-hcl2-0.2.0/hcl2/__main__.py` & `glitch-python-hcl2-0.2.1/hcl2/__main__.py`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.2.0/hcl2/api.py` & `glitch-python-hcl2-0.2.1/hcl2/api.py`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.2.0/hcl2/hcl2.lark` & `glitch-python-hcl2-0.2.1/hcl2/hcl2.lark`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.2.0/hcl2/transformer.py` & `glitch-python-hcl2-0.2.1/hcl2/transformer.py`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.2.0/setup.py` & `glitch-python-hcl2-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import os.path
 from setuptools import setup, find_packages
 
 
+this_directory = os.path.abspath(os.path.dirname(__file__))
+
+
 def get_long_description():
     """Reads the long description from the README"""
-    this_directory = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as file:
         return file.read()
 
 
 def get_requirements():
     """Reads the installation requirements from requirements.txt"""
-    with open("requirements.txt", encoding="utf8") as reqfile:
+    with open(
+        os.path.join(this_directory, "requirements.txt"), encoding="utf8"
+    ) as reqfile:
         return [
             line
             for line in reqfile.read().split("\n")
             if not line.startswith(("#", "-"))
         ]
 
 
 setup(
     name="glitch-python-hcl2",
-    version="0.2.0",
+    version="0.2.1",
     author="João Gonçalves",
     author_email="joao.marques.goncalves@tecnico.ulisboa.pt",
     url="https://github.com/joaotgoncalves/python-hcl2",
     license="MIT",
     classifiers=[
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Intended Audience :: Developers",
```

