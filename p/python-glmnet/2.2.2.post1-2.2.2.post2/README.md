# Comparing `tmp/python_glmnet-2.2.2.post1.tar.gz` & `tmp/python_glmnet-2.2.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glmnet-2.2.2.post1.tar", last modified: Fri May 10 15:31:42 2024, max compression
+gzip compressed data, was "python_glmnet-2.2.2.post2.tar", last modified: Fri May 10 19:07:38 2024, max compression
```

## Comparing `python_glmnet-2.2.2.post1.tar` & `python_glmnet-2.2.2.post2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:31:42.351108 python_glmnet-2.2.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:31:42.347108 python_glmnet-2.2.2.post1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/LICENSES/GLMNET_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/LICENSES/SCIKIT_LEARN_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-10 15:31:42.351108 python_glmnet-2.2.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:31:42.351108 python_glmnet-2.2.2.post1/glmnet/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/_glmnet.pyf
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17642 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    23592 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:31:42.347108 python_glmnet-2.2.2.post1/glmnet/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:31:42.351108 python_glmnet-2.2.2.post1/glmnet/src/glmnet/
--rw-r--r--   0 runner    (1001) docker     (127)   561094 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/src/glmnet/glmnet5.f90
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/glmnet/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:31:42.351108 python_glmnet-2.2.2.post1/python_glmnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-10 15:31:42.000000 python_glmnet-2.2.2.post1/python_glmnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-10 15:31:42.000000 python_glmnet-2.2.2.post1/python_glmnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:31:42.000000 python_glmnet-2.2.2.post1/python_glmnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 15:31:42.000000 python_glmnet-2.2.2.post1/python_glmnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:31:42.351108 python_glmnet-2.2.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-10 15:31:35.000000 python_glmnet-2.2.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:38.696627 python_glmnet-2.2.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:38.692627 python_glmnet-2.2.2.post2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/LICENSES/GLMNET_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/LICENSES/SCIKIT_LEARN_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-10 19:07:38.692627 python_glmnet-2.2.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:38.692627 python_glmnet-2.2.2.post2/glmnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/_glmnet.pyf
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17642 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23592 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:38.688627 python_glmnet-2.2.2.post2/glmnet/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:38.692627 python_glmnet-2.2.2.post2/glmnet/src/glmnet/
+-rw-r--r--   0 runner    (1001) docker     (127)   561094 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/src/glmnet/glmnet5.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/glmnet/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:38.692627 python_glmnet-2.2.2.post2/python_glmnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-10 19:07:38.000000 python_glmnet-2.2.2.post2/python_glmnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-10 19:07:38.000000 python_glmnet-2.2.2.post2/python_glmnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:07:38.000000 python_glmnet-2.2.2.post2/python_glmnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 19:07:38.000000 python_glmnet-2.2.2.post2/python_glmnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 19:07:38.000000 python_glmnet-2.2.2.post2/python_glmnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:07:38.696627 python_glmnet-2.2.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-10 19:07:32.000000 python_glmnet-2.2.2.post2/setup.py
```

### Comparing `python_glmnet-2.2.2.post1/LICENSE` & `python_glmnet-2.2.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/LICENSES/GLMNET_LICENSE` & `python_glmnet-2.2.2.post2/LICENSES/GLMNET_LICENSE`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/LICENSES/SCIKIT_LEARN_LICENSE` & `python_glmnet-2.2.2.post2/LICENSES/SCIKIT_LEARN_LICENSE`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/PKG-INFO` & `python_glmnet-2.2.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: python-glmnet
-Version: 2.2.2.post1
+Version: 2.2.2.post2
 Summary: Python wrapper for glmnet
-Home-page: https://github.com/civisanalytics/python-glmnet
+Home-page: https://github.com/replicahq/python-glmnet
 Author: Civis Analytics Inc
-Author-email: opensource@civisanalytics.com
+Author-email: opensource@replicahq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy>=1.9.2
+Requires-Dist: scikit-learn>=0.18.0
+Requires-Dist: scipy>=0.14.1
+Requires-Dist: joblib>=0.14.1
 
 Python GLMNET
 =============
 
-|CircleCI| |Conda| |PyPI| |PyVersions|
+|CircleCI| |PyPI| |PyVersions|
 
 .. |CircleCI| image:: https://circleci.com/gh/civisanalytics/python-glmnet.svg?style=svg
     :target: https://circleci.com/gh/civisanalytics/python-glmnet
     :alt: Build status
 
-.. |Conda| image:: https://anaconda.org/conda-forge/glmnet/badges/version.svg
-   :target: https://anaconda.org/conda-forge/glmnet
-   :alt: Latest version on conda forge
-
-.. |PyPI| image:: https://img.shields.io/pypi/v/glmnet.svg
-   :target: https://pypi.org/project/glmnet/
+.. |PyPI| image:: https://img.shields.io/pypi/v/python-glmnet.svg
+   :target: https://pypi.org/project/python-glmnet/
    :alt: Latest version on PyPI
 
-.. |PyVersions| image:: https://img.shields.io/pypi/pyversions/glmnet.svg
-   :target: https://pypi.org/project/glmnet/
+.. |PyVersions| image:: https://img.shields.io/pypi/pyversions/python-glmnet.svg
+   :target: https://pypi.org/project/python-glmnet/
    :alt: Supported python versions for python-glmnet
 
-Fork of `python-glmnet <https://github.com/civisanalytics/python-glmnet>`_ with support for more recent
+Fork of `python-glmnet <https://github.com/replicahq/python-glmnet>`_ with support for more recent
 Python versions.
 
 This is a Python wrapper for the fortran library used in the R package
 `glmnet <http://web.stanford.edu/~hastie/glmnet/glmnet_alpha.html>`__.
 While the library includes linear, logistic, Cox, Poisson, and
 multiple-response Gaussian, only linear and logistic are implemented in
 this package.
@@ -45,15 +45,15 @@
 
 Installation
 ------------
 
 requirements
 ~~~~~~~~~~~~
 
-``python-glmnet`` requires Python version >= 3.6, ``scikit-learn``, ``numpy``,
+``python-glmnet`` requires Python version >= 3.9, ``scikit-learn``, ``numpy``,
 and ``scipy``. Installation from source or via ``pip`` requires a Fortran compiler.
 
 conda
 ~~~~~
 
 .. code:: bash
 
@@ -61,15 +61,15 @@
 
 
 pip
 ~~~
 
 .. code:: bash
 
-    pip install glmnet
+    pip install python-glmnet
 
 
 source
 ~~~~~~
 
 ``glmnet`` depends on numpy, scikit-learn and scipy.
 A working Fortran compiler is also required to build the package.
```

### Comparing `python_glmnet-2.2.2.post1/README.rst` & `python_glmnet-2.2.2.post2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Python GLMNET
 =============
 
-|CircleCI| |Conda| |PyPI| |PyVersions|
+|CircleCI| |PyPI| |PyVersions|
 
 .. |CircleCI| image:: https://circleci.com/gh/civisanalytics/python-glmnet.svg?style=svg
     :target: https://circleci.com/gh/civisanalytics/python-glmnet
     :alt: Build status
 
-.. |Conda| image:: https://anaconda.org/conda-forge/glmnet/badges/version.svg
-   :target: https://anaconda.org/conda-forge/glmnet
-   :alt: Latest version on conda forge
-
-.. |PyPI| image:: https://img.shields.io/pypi/v/glmnet.svg
-   :target: https://pypi.org/project/glmnet/
+.. |PyPI| image:: https://img.shields.io/pypi/v/python-glmnet.svg
+   :target: https://pypi.org/project/python-glmnet/
    :alt: Latest version on PyPI
 
-.. |PyVersions| image:: https://img.shields.io/pypi/pyversions/glmnet.svg
-   :target: https://pypi.org/project/glmnet/
+.. |PyVersions| image:: https://img.shields.io/pypi/pyversions/python-glmnet.svg
+   :target: https://pypi.org/project/python-glmnet/
    :alt: Supported python versions for python-glmnet
 
-Fork of `python-glmnet <https://github.com/civisanalytics/python-glmnet>`_ with support for more recent
+Fork of `python-glmnet <https://github.com/replicahq/python-glmnet>`_ with support for more recent
 Python versions.
 
 This is a Python wrapper for the fortran library used in the R package
 `glmnet <http://web.stanford.edu/~hastie/glmnet/glmnet_alpha.html>`__.
 While the library includes linear, logistic, Cox, Poisson, and
 multiple-response Gaussian, only linear and logistic are implemented in
 this package.
@@ -34,15 +30,15 @@
 
 Installation
 ------------
 
 requirements
 ~~~~~~~~~~~~
 
-``python-glmnet`` requires Python version >= 3.6, ``scikit-learn``, ``numpy``,
+``python-glmnet`` requires Python version >= 3.9, ``scikit-learn``, ``numpy``,
 and ``scipy``. Installation from source or via ``pip`` requires a Fortran compiler.
 
 conda
 ~~~~~
 
 .. code:: bash
 
@@ -50,15 +46,15 @@
 
 
 pip
 ~~~
 
 .. code:: bash
 
-    pip install glmnet
+    pip install python-glmnet
 
 
 source
 ~~~~~~
 
 ``glmnet`` depends on numpy, scikit-learn and scipy.
 A working Fortran compiler is also required to build the package.
```

### Comparing `python_glmnet-2.2.2.post1/glmnet/_glmnet.pyf` & `python_glmnet-2.2.2.post2/glmnet/_glmnet.pyf`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/glmnet/doc.py` & `python_glmnet-2.2.2.post2/glmnet/doc.py`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/glmnet/errors.py` & `python_glmnet-2.2.2.post2/glmnet/errors.py`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/glmnet/linear.py` & `python_glmnet-2.2.2.post2/glmnet/linear.py`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/glmnet/logistic.py` & `python_glmnet-2.2.2.post2/glmnet/logistic.py`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/glmnet/scorer.py` & `python_glmnet-2.2.2.post2/glmnet/scorer.py`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/glmnet/src/glmnet/glmnet5.f90` & `python_glmnet-2.2.2.post2/glmnet/src/glmnet/glmnet5.f90`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/glmnet/util.py` & `python_glmnet-2.2.2.post2/glmnet/util.py`

 * *Files identical despite different names*

### Comparing `python_glmnet-2.2.2.post1/python_glmnet.egg-info/PKG-INFO` & `python_glmnet-2.2.2.post2/python_glmnet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: python-glmnet
-Version: 2.2.2.post1
+Version: 2.2.2.post2
 Summary: Python wrapper for glmnet
-Home-page: https://github.com/civisanalytics/python-glmnet
+Home-page: https://github.com/replicahq/python-glmnet
 Author: Civis Analytics Inc
-Author-email: opensource@civisanalytics.com
+Author-email: opensource@replicahq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy>=1.9.2
+Requires-Dist: scikit-learn>=0.18.0
+Requires-Dist: scipy>=0.14.1
+Requires-Dist: joblib>=0.14.1
 
 Python GLMNET
 =============
 
-|CircleCI| |Conda| |PyPI| |PyVersions|
+|CircleCI| |PyPI| |PyVersions|
 
 .. |CircleCI| image:: https://circleci.com/gh/civisanalytics/python-glmnet.svg?style=svg
     :target: https://circleci.com/gh/civisanalytics/python-glmnet
     :alt: Build status
 
-.. |Conda| image:: https://anaconda.org/conda-forge/glmnet/badges/version.svg
-   :target: https://anaconda.org/conda-forge/glmnet
-   :alt: Latest version on conda forge
-
-.. |PyPI| image:: https://img.shields.io/pypi/v/glmnet.svg
-   :target: https://pypi.org/project/glmnet/
+.. |PyPI| image:: https://img.shields.io/pypi/v/python-glmnet.svg
+   :target: https://pypi.org/project/python-glmnet/
    :alt: Latest version on PyPI
 
-.. |PyVersions| image:: https://img.shields.io/pypi/pyversions/glmnet.svg
-   :target: https://pypi.org/project/glmnet/
+.. |PyVersions| image:: https://img.shields.io/pypi/pyversions/python-glmnet.svg
+   :target: https://pypi.org/project/python-glmnet/
    :alt: Supported python versions for python-glmnet
 
-Fork of `python-glmnet <https://github.com/civisanalytics/python-glmnet>`_ with support for more recent
+Fork of `python-glmnet <https://github.com/replicahq/python-glmnet>`_ with support for more recent
 Python versions.
 
 This is a Python wrapper for the fortran library used in the R package
 `glmnet <http://web.stanford.edu/~hastie/glmnet/glmnet_alpha.html>`__.
 While the library includes linear, logistic, Cox, Poisson, and
 multiple-response Gaussian, only linear and logistic are implemented in
 this package.
@@ -45,15 +45,15 @@
 
 Installation
 ------------
 
 requirements
 ~~~~~~~~~~~~
 
-``python-glmnet`` requires Python version >= 3.6, ``scikit-learn``, ``numpy``,
+``python-glmnet`` requires Python version >= 3.9, ``scikit-learn``, ``numpy``,
 and ``scipy``. Installation from source or via ``pip`` requires a Fortran compiler.
 
 conda
 ~~~~~
 
 .. code:: bash
 
@@ -61,15 +61,15 @@
 
 
 pip
 ~~~
 
 .. code:: bash
 
-    pip install glmnet
+    pip install python-glmnet
 
 
 source
 ~~~~~~
 
 ``glmnet`` depends on numpy, scikit-learn and scipy.
 A working Fortran compiler is also required to build the package.
```

### Comparing `python_glmnet-2.2.2.post1/setup.py` & `python_glmnet-2.2.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from numpy.distutils.core import Extension, setup
 except ImportError:
     sys.exit("install requires: 'numpy'."
              " use pip or easy_install."
              " \n  $ pip install numpy")
 
 
-_VERSION = "2.2.2.post1"
+_VERSION = "2.2.2.post2"
 
 f_compile_args = ['-ffixed-form', '-fdefault-real-8']
 
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as _in:
         return _in.read()
@@ -64,16 +64,16 @@
 if __name__ == "__main__":
     setup(name="glmnet",
           version=_VERSION,
           description="Python wrapper for glmnet",
           long_description=read('README.rst'),
           long_description_content_type="text/x-rst",
           author="Civis Analytics Inc",
-          author_email="opensource@civisanalytics.com",
-          url="https://github.com/civisanalytics/python-glmnet",
+          author_email="opensource@replicahq.com",
+          url="https://github.com/replicahq/python-glmnet",
           install_requires=[
               "numpy>=1.9.2",
               "scikit-learn>=0.18.0",
               "scipy>=0.14.1",
               "joblib>=0.14.1",
           ],
           python_requires=">=3.9",
```

