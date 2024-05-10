# Comparing `tmp/cochleogram-0.9.0.tar.gz` & `tmp/cochleogram-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.9.0.tar", last modified: Tue May  7 22:05:34 2024, max compression
+gzip compressed data, was "cochleogram-0.9.1.tar", last modified: Fri May 10 21:15:11 2024, max compression
```

## Comparing `cochleogram-0.9.0.tar` & `cochleogram-0.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.726924 cochleogram-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.718924 cochleogram-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.718924 cochleogram-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-07 22:05:30.000000 cochleogram-0.9.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-07 22:05:30.000000 cochleogram-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-07 22:05:34.726924 cochleogram-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 22:05:30.000000 cochleogram-0.9.0/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.722924 cochleogram-0.9.0/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.726924 cochleogram-0.9.0/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/main-icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (127)    25893 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.726924 cochleogram-0.9.0/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-07 22:05:30.000000 cochleogram-0.9.0/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-07 22:05:30.000000 cochleogram-0.9.0/license
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 22:05:30.000000 cochleogram-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-05-07 22:05:30.000000 cochleogram-0.9.0/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:05:34.726924 cochleogram-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:11.252504 cochleogram-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:11.244504 cochleogram-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:11.248504 cochleogram-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-10 21:15:07.000000 cochleogram-0.9.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-10 21:15:07.000000 cochleogram-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-10 21:15:11.252504 cochleogram-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-10 21:15:07.000000 cochleogram-0.9.1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:11.248504 cochleogram-0.9.1/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:11.252504 cochleogram-0.9.1/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/main-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25893 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-05-10 21:15:07.000000 cochleogram-0.9.1/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 21:15:11.000000 cochleogram-0.9.1/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:15:11.252504 cochleogram-0.9.1/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-10 21:15:11.000000 cochleogram-0.9.1/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-10 21:15:11.000000 cochleogram-0.9.1/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:15:11.000000 cochleogram-0.9.1/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-10 21:15:11.000000 cochleogram-0.9.1/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-10 21:15:11.000000 cochleogram-0.9.1/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 21:15:11.000000 cochleogram-0.9.1/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 21:15:07.000000 cochleogram-0.9.1/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-10 21:15:07.000000 cochleogram-0.9.1/license
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-10 21:15:07.000000 cochleogram-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-05-10 21:15:07.000000 cochleogram-0.9.1/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:15:11.252504 cochleogram-0.9.1/setup.cfg
```

### Comparing `cochleogram-0.9.0/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.9.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/.gitignore` & `cochleogram-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/PKG-INFO` & `cochleogram-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.9.0
+Version: 0.9.1
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: atom
 Requires-Dist: enaml[qt6-pyside]
+Requires-Dist: pyside6<6.7.0
 Requires-Dist: matplotlib
 Requires-Dist: ndimage-enaml>=0.0.8
 Requires-Dist: numpy
 Requires-Dist: raster_geometry
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: scikit-image
```

### Comparing `cochleogram-0.9.0/cochleogram/config.py` & `cochleogram-0.9.1/cochleogram/config.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/gui.enaml` & `cochleogram-0.9.1/cochleogram/gui.enaml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/icons/cells.png` & `cochleogram-0.9.1/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/icons/exclude.png` & `cochleogram-0.9.1/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/icons/main-icon.ico` & `cochleogram-0.9.1/cochleogram/icons/main-icon.ico`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/icons/main-icon.png` & `cochleogram-0.9.1/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/icons/make_icons.py` & `cochleogram-0.9.1/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/icons/spiral.png` & `cochleogram-0.9.1/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/icons/tile.png` & `cochleogram-0.9.1/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/instructions.html` & `cochleogram-0.9.1/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/main.py` & `cochleogram-0.9.1/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/model.py` & `cochleogram-0.9.1/cochleogram/model.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/plot.py` & `cochleogram-0.9.1/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/presenter.py` & `cochleogram-0.9.1/cochleogram/presenter.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/readers.py` & `cochleogram-0.9.1/cochleogram/readers.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram/util.py` & `cochleogram-0.9.1/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.9.1/cochleogram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.9.0
+Version: 0.9.1
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: atom
 Requires-Dist: enaml[qt6-pyside]
+Requires-Dist: pyside6<6.7.0
 Requires-Dist: matplotlib
 Requires-Dist: ndimage-enaml>=0.0.8
 Requires-Dist: numpy
 Requires-Dist: raster_geometry
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: scikit-image
```

### Comparing `cochleogram-0.9.0/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.9.1/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/license` & `cochleogram-0.9.1/license`

 * *Files identical despite different names*

### Comparing `cochleogram-0.9.0/pyproject.toml` & `cochleogram-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ]
 maintainers = [
     {name = "Brad Buran", email="buran@ohsu.edu"},
 ]
 dependencies = [
     "atom",
     "enaml[qt6-pyside]",
+	"pyside6 < 6.7.0", # bug in 6.7.0
     "matplotlib",
 	"ndimage-enaml >= 0.0.8",
     "numpy",
     "raster_geometry",
     "pandas",
     "scipy",
     "scikit-image",
```

### Comparing `cochleogram-0.9.0/readme.rst` & `cochleogram-0.9.1/readme.rst`

 * *Files identical despite different names*

