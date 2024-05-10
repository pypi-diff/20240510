# Comparing `tmp/samtool-0.0.1.tar.gz` & `tmp/samtool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samtool-0.0.1.tar", last modified: Fri May 10 14:45:12 2024, max compression
+gzip compressed data, was "samtool-0.0.2.tar", last modified: Fri May 10 14:57:15 2024, max compression
```

## Comparing `samtool-0.0.1.tar` & `samtool-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:45:12.974144 samtool-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 14:45:09.000000 samtool-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-10 14:45:12.974144 samtool-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-10 14:45:09.000000 samtool-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:45:12.970143 samtool-0.0.1/samtool/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-10 14:45:09.000000 samtool-0.0.1/samtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-10 14:45:09.000000 samtool-0.0.1/samtool/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-10 14:45:09.000000 samtool-0.0.1/samtool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:45:12.974144 samtool-0.0.1/samtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-10 14:45:12.000000 samtool-0.0.1/samtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-10 14:45:12.000000 samtool-0.0.1/samtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:45:12.000000 samtool-0.0.1/samtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-10 14:45:12.000000 samtool-0.0.1/samtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 14:45:12.000000 samtool-0.0.1/samtool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:45:12.974144 samtool-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-10 14:45:09.000000 samtool-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:57:15.848438 samtool-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 14:57:10.000000 samtool-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-10 14:57:15.848438 samtool-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-10 14:57:10.000000 samtool-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:57:15.844437 samtool-0.0.2/samtool/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-10 14:57:10.000000 samtool-0.0.2/samtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-10 14:57:10.000000 samtool-0.0.2/samtool/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-10 14:57:10.000000 samtool-0.0.2/samtool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:57:15.848438 samtool-0.0.2/samtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-10 14:57:15.000000 samtool-0.0.2/samtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-10 14:57:15.000000 samtool-0.0.2/samtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:57:15.000000 samtool-0.0.2/samtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-10 14:57:15.000000 samtool-0.0.2/samtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 14:57:15.000000 samtool-0.0.2/samtool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:57:15.848438 samtool-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-10 14:57:10.000000 samtool-0.0.2/setup.py
```

### Comparing `samtool-0.0.1/LICENSE` & `samtool-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `samtool-0.0.1/PKG-INFO` & `samtool-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samtool
-Version: 0.0.1
+Version: 0.0.2
 Summary: SamTool is a Python library designed for easy integration of the SAM (Segment Anything with Masking) model into computer vision projects. SAM is a state-of-the-art model for segmenting objects in images with high accuracy.
 Home-page: https://github.com/manbehindthemadness/samtool
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `samtool-0.0.1/README.md` & `samtool-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `samtool-0.0.1/samtool/main.py` & `samtool-0.0.2/samtool/main.py`

 * *Files identical despite different names*

### Comparing `samtool-0.0.1/samtool/utils.py` & `samtool-0.0.2/samtool/utils.py`

 * *Files identical despite different names*

### Comparing `samtool-0.0.1/samtool.egg-info/PKG-INFO` & `samtool-0.0.2/samtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samtool
-Version: 0.0.1
+Version: 0.0.2
 Summary: SamTool is a Python library designed for easy integration of the SAM (Segment Anything with Masking) model into computer vision projects. SAM is a state-of-the-art model for segmenting objects in images with high accuracy.
 Home-page: https://github.com/manbehindthemadness/samtool
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `samtool-0.0.1/setup.py` & `samtool-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 try:
     from install_preserve import preserve
 except ImportError:
     import pip  # noqa
     pip.main(['install', 'install-preserve'])
-    pip.main(['install', './segment-anything'])
+    pip.main(['install', 'git+https://github.com/facebookresearch/segment-anything.git'])
     from install_preserve import preserve  # noqa
 
 install_requires = [
     'pyyaml',
     'tqdm',
     'numpy',
     'matplotlib',
@@ -30,15 +30,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='samtool',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

