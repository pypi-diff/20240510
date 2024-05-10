# Comparing `tmp/qtpyinheritance-0.0.2.tar.gz` & `tmp/qtpyinheritance-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qtpyinheritance-0.0.2.tar", last modified: Fri Jun  3 18:52:12 2022, max compression
+gzip compressed data, was "qtpyinheritance-0.0.3.tar", last modified: Fri May 10 20:03:21 2024, max compression
```

## Comparing `qtpyinheritance-0.0.2.tar` & `qtpyinheritance-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,46 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1482 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/LICENSE
--rw-r--r--   0 klauer   (1318172782) 1704612529      323 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529      857 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      378 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/README.rst
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/docs/
--rw-r--r--   0 klauer   (1318172782) 1704612529      625 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/docs/Makefile
--rw-r--r--   0 klauer   (1318172782) 1704612529      796 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/docs/make.bat
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/docs/source/
--rw-r--r--   0 klauer   (1318172782) 1704612529     5417 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/docs/source/conf.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      604 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/docs/source/index.rst
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance/
--rw-r--r--   0 klauer   (1318172782) 1704612529      177 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/qtpyinheritance/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8308 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/qtpyinheritance/properties.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1612 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/qtpyinheritance/signals.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance/tests/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/qtpyinheritance/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/qtpyinheritance/tests/conftest.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1712 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/qtpyinheritance/tests/test_properties.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1491 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/qtpyinheritance/tests/test_signals.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529      857 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      604 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        5 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       16 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/qtpyinheritance.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        5 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      189 2022-06-03 18:52:12.000000 qtpyinheritance-0.0.2/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     1492 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    68611 2022-06-03 18:48:15.000000 qtpyinheritance-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.783260 qtpyinheritance-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.779260 qtpyinheritance-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.779260 qtpyinheritance-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-10 20:03:21.783260 qtpyinheritance-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.779260 qtpyinheritance-0.0.3/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.779260 qtpyinheritance-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.779260 qtpyinheritance-0.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.779260 qtpyinheritance-0.0.3/qtpyinheritance/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 20:03:21.000000 qtpyinheritance-0.0.3/qtpyinheritance/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.783260 qtpyinheritance-0.0.3/qtpyinheritance/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/qtpyinheritance/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:03:21.783260 qtpyinheritance-0.0.3/qtpyinheritance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-10 20:03:21.000000 qtpyinheritance-0.0.3/qtpyinheritance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 20:03:21.000000 qtpyinheritance-0.0.3/qtpyinheritance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:03:21.000000 qtpyinheritance-0.0.3/qtpyinheritance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-10 20:03:21.000000 qtpyinheritance-0.0.3/qtpyinheritance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 20:03:21.000000 qtpyinheritance-0.0.3/qtpyinheritance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-10 20:03:11.000000 qtpyinheritance-0.0.3/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:03:21.783260 qtpyinheritance-0.0.3/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qtpyinheritance-0.0.2/LICENSE` & `qtpyinheritance-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qtpyinheritance-0.0.2/docs/Makefile` & `qtpyinheritance-0.0.3/docs/Makefile`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `qtpyinheritance-0.0.2/docs/make.bat` & `qtpyinheritance-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qtpyinheritance-0.0.2/docs/source/conf.py` & `qtpyinheritance-0.0.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
+
 import sphinx_rtd_theme
 
 module_path = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                            '../../')
 sys.path.insert(0, module_path)
 
 # -- Project information -----------------------------------------------------
 
 project = 'qtpyinheritance'
 author = 'Ken Lauer'
 
 from datetime import datetime
+
 year = datetime.now().year
 copyright = str(year) + ', Ken Lauer'
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
 release = ''
```

### Comparing `qtpyinheritance-0.0.2/docs/source/index.rst` & `qtpyinheritance-0.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `qtpyinheritance-0.0.2/qtpyinheritance/properties.py` & `qtpyinheritance-0.0.3/qtpyinheritance/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 from qtpy import QtCore
 
-
 logger = logging.getLogger(__name__)
 
 SKIP_TYPENAMES = {'Shadow', 'Shape'}
 
 
 def get_qt_properties(cls):
     'Yields all QMetaProperty instances from a given class'
@@ -165,18 +164,18 @@
             # Some types such as SizeConstraint are not supported in PyQt5
             logger.debug('Unable to create %s', prop_cls.__name__, exc_info=ex)
 
     return passthrough_properties
 
 
 def forward_property(
-        attr_name, cls, prop_name, *,
-        designable=None, scriptable=None, stored=None, user=None,
-        rw_class=PassthroughProperty, ro_class=ReadonlyPassthroughProperty
-        ):
+    attr_name, cls, prop_name, *,
+    designable=None, scriptable=None, stored=None, user=None,
+    rw_class=PassthroughProperty, ro_class=ReadonlyPassthroughProperty
+):
     '''
     Forward one property from a QObject attribute in a class given its name
 
     For use in class definitions. As the usage is somewhat nonstandard, be sure
     to look at the example below.
 
     Parameters
```

### Comparing `qtpyinheritance-0.0.2/qtpyinheritance/signals.py` & `qtpyinheritance-0.0.3/qtpyinheritance/signals.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import inspect
 import functools
+import inspect
 
 from qtpy import QtCore
 
 
 def should_inherit(obj, *, signals=True, slots=True):
     '''
     Check a single object to see if it should be inherited
```

### Comparing `qtpyinheritance-0.0.2/qtpyinheritance/tests/test_properties.py` & `qtpyinheritance-0.0.3/qtpyinheritance/tests/test_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from qtpy import QtWidgets
 
 import qtpyinheritance.properties
-from qtpyinheritance.properties import forward_property, forward_properties
+from qtpyinheritance.properties import forward_properties, forward_property
 
 
 def test_forward_properties(qtbot):
     class MyClass(QtWidgets.QFrame):
         def __init__(self, parent=None):
             super().__init__(parent=parent)
             self.label = QtWidgets.QLabel()
```

### Comparing `qtpyinheritance-0.0.2/qtpyinheritance/tests/test_signals.py` & `qtpyinheritance-0.0.3/qtpyinheritance/tests/test_signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import collections
 
 import qtpy
 from qtpy import QtCore
 
 import qtpyinheritance.signals
 
-
 print(qtpy.QT_VERSION, qtpy.API_NAME)
 
 
 class BaseA(QtCore.QObject):
     signal_a = QtCore.Signal(str)
 
     @QtCore.Slot(str)
```

