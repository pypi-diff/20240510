# Comparing `tmp/pennylane-sphinx-theme-0.5.5.tar.gz` & `tmp/pennylane-sphinx-theme-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane-sphinx-theme-0.5.5.tar", last modified: Fri Feb 23 18:46:01 2024, max compression
+gzip compressed data, was "pennylane-sphinx-theme-0.5.6.tar", last modified: Fri May 10 19:05:06 2024, max compression
```

## Comparing `pennylane-sphinx-theme-0.5.5.tar` & `pennylane-sphinx-theme-0.5.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:46:01.012136 pennylane-sphinx-theme-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-23 18:45:44.000000 pennylane-sphinx-theme-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-02-23 18:46:01.012136 pennylane-sphinx-theme-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-02-23 18:45:44.000000 pennylane-sphinx-theme-0.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:46:01.012136 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-23 18:45:44.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-23 18:45:44.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-02-23 18:45:44.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-02-23 18:45:44.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/navbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:46:01.012136 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-02-23 18:46:00.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-23 18:46:00.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 18:46:00.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-23 18:46:00.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-23 18:46:00.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-23 18:46:00.000000 pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 18:46:01.012136 pennylane-sphinx-theme-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-23 18:45:44.000000 pennylane-sphinx-theme-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:05:06.156062 pennylane-sphinx-theme-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 19:04:46.000000 pennylane-sphinx-theme-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-10 19:05:06.156062 pennylane-sphinx-theme-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-10 19:04:46.000000 pennylane-sphinx-theme-0.5.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:05:06.152061 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-10 19:04:46.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-10 19:04:46.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-10 19:04:46.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-10 19:04:46.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/navbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:05:06.156062 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-10 19:05:06.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 19:05:06.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:05:06.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-10 19:05:06.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 19:05:06.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 19:05:06.000000 pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:05:06.156062 pennylane-sphinx-theme-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-10 19:04:46.000000 pennylane-sphinx-theme-0.5.6/setup.py
```

### Comparing `pennylane-sphinx-theme-0.5.5/LICENSE` & `pennylane-sphinx-theme-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane-sphinx-theme-0.5.5/PKG-INFO` & `pennylane-sphinx-theme-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-sphinx-theme
-Version: 0.5.5
+Version: 0.5.6
 Summary: Sphinx theme for PennyLane open-source Python packages
 Home-page: https://github.com/XanaduAI/pennylane-sphinx-theme
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: PennyLane Sphinx Theme
         ######################
```

### Comparing `pennylane-sphinx-theme-0.5.5/README.rst` & `pennylane-sphinx-theme-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/__init__.py` & `pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module registers the PennyLane Sphinx Theme. For more information, see
 https://www.sphinx-doc.org/en/master/development/theming.html
 """
+
 from pathlib import Path
 
 from xanadu_sphinx_theme import templates_dir
 
 from ._version import __version__
 from .footer import FOOTER
 from .navbar import NAVBAR_LEFT, NAVBAR_RIGHT
```

### Comparing `pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/footer.py` & `pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/footer.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             "links": [
                 {
                     "name": "Learn",
                     "href": "https://pennylane.ai/qml/",
                 },
                 {
                     "name": "Codebook",
-                    "href": "https://codebook.xanadu.ai/",
+                    "href": "https://pennylane.ai/codebook/",
                 },
                 {
                     "name": "Education",
                     "href": "https://pennylane.ai/education/",
                 },
                 {
                     "name": "Videos",
```

### Comparing `pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme/navbar.py` & `pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme/navbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         "dropdown": [
             {
                 "name": "Demos",
                 "href": "https://pennylane.ai/qml/demonstrations/",
             },
             {
                 "name": "Codebook",
-                "href": "https://codebook.xanadu.ai/",
+                "href": "https://pennylane.ai/codebook/",
                 "external": True,
             },
             {
                 "name": "Challenges",
                 "href": "https://pennylane.ai/challenges/",
             },
             {
```

### Comparing `pennylane-sphinx-theme-0.5.5/pennylane_sphinx_theme.egg-info/PKG-INFO` & `pennylane-sphinx-theme-0.5.6/pennylane_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-sphinx-theme
-Version: 0.5.5
+Version: 0.5.6
 Summary: Sphinx theme for PennyLane open-source Python packages
 Home-page: https://github.com/XanaduAI/pennylane-sphinx-theme
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: PennyLane Sphinx Theme
         ######################
```

### Comparing `pennylane-sphinx-theme-0.5.5/setup.py` & `pennylane-sphinx-theme-0.5.6/setup.py`

 * *Files identical despite different names*

