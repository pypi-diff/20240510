# Comparing `tmp/pysurvmc-0.1.tar.gz` & `tmp/pysurvmc-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurvmc-0.1.tar", last modified: Mon May  6 21:37:30 2024, max compression
+gzip compressed data, was "pysurvmc-0.2.tar", last modified: Fri May 10 09:55:26 2024, max compression
```

## Comparing `pysurvmc-0.1.tar` & `pysurvmc-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:37:30.486405 pysurvmc-0.1/
--rw-rw-rw-   0        0        0      677 2024-05-06 21:37:30.486405 pysurvmc-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 21:37:30.485405 pysurvmc-0.1/PySurvMC.egg-info/
--rw-rw-rw-   0        0        0      677 2024-05-06 21:37:30.000000 pysurvmc-0.1/PySurvMC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-05-06 21:37:30.000000 pysurvmc-0.1/PySurvMC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:37:30.000000 pysurvmc-0.1/PySurvMC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2024-05-06 21:37:30.000000 pysurvmc-0.1/PySurvMC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:37:30.000000 pysurvmc-0.1/PySurvMC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 21:37:30.486405 pysurvmc-0.1/setup.cfg
--rw-rw-rw-   0        0        0      799 2024-05-06 21:37:11.000000 pysurvmc-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:55:26.891985 pysurvmc-0.2/
+-rw-rw-rw-   0        0        0     2974 2024-05-10 09:55:26.891985 pysurvmc-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 09:55:26.890980 pysurvmc-0.2/PySurvMC.egg-info/
+-rw-rw-rw-   0        0        0     2974 2024-05-10 09:55:26.000000 pysurvmc-0.2/PySurvMC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-05-10 09:55:26.000000 pysurvmc-0.2/PySurvMC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:55:26.000000 pysurvmc-0.2/PySurvMC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2024-05-10 09:55:26.000000 pysurvmc-0.2/PySurvMC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:55:26.000000 pysurvmc-0.2/PySurvMC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:55:26.891985 pysurvmc-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-05-10 09:53:57.000000 pysurvmc-0.2/setup.py
```

### Comparing `pysurvmc-0.1/setup.py` & `pysurvmc-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from setuptools import setup, find_packages
 
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+
+long_description = (this_directory / "Readme.md").read_text()
+
 setup(
     name='PySurvMC',
-    version='0.1',
+    version='0.2',
     author='yueht17',
     author_email="yueht17@foxmail.com",
-    description='A Python package for Survival Analysis with Monte Carlo Simulation',
+    # description='A Python package for Survival Analysis with Monte Carlo Simulation',
+
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+
     packages=find_packages(),
     install_requires=[
         "pymc>=5.14.0",
         "arviz>=0.13.0",
         "cachetools>=4.2.1",
         "cloudpickle",
         "numpy>=1.15.0",
```

