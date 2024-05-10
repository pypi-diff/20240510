# Comparing `tmp/aiida_wannier90-2.1.0.tar.gz` & `tmp/aiida_wannier90-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_wannier90-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_wannier90-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_wannier90-2.1.0.tar` & `aiida_wannier90-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1301 2023-07-03 18:09:05.977599 aiida_wannier90-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2118 2023-07-03 18:09:06.101597 aiida_wannier90-2.1.0/README.md
--rw-r--r--   0        0        0     4929 2023-07-03 18:09:06.189596 aiida_wannier90-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1973 2023-07-03 18:09:06.189596 aiida_wannier90-2.1.0/src/aiida_wannier90/__init__.py
--rw-r--r--   0        0        0      200 2023-07-03 18:09:06.197595 aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/__init__.py
--rw-r--r--   0        0        0    19794 2023-07-03 18:09:06.293594 aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/postw90.py
--rw-r--r--   0        0        0    23668 2023-07-03 18:09:06.297594 aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/wannier90.py
--rw-r--r--   0        0        0      802 2023-07-03 18:09:06.389593 aiida_wannier90-2.1.0/src/aiida_wannier90/io/__init__.py
--rw-r--r--   0        0        0     1814 2023-07-03 18:09:06.393593 aiida_wannier90-2.1.0/src/aiida_wannier90/io/_group_list.py
--rw-r--r--   0        0        0    14969 2023-07-03 18:09:06.393593 aiida_wannier90-2.1.0/src/aiida_wannier90/io/_write_win.py
--rw-r--r--   0        0        0    13286 2023-07-03 18:09:06.401593 aiida_wannier90-2.1.0/src/aiida_wannier90/orbitals.py
--rw-r--r--   0        0        0      162 2023-07-03 18:09:06.401593 aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/__init__.py
--rw-r--r--   0        0        0    20688 2023-07-03 18:09:06.421592 aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/postw90.py
--rw-r--r--   0        0        0    23479 2023-07-03 18:09:06.433592 aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/wannier90.py
--rw-r--r--   0        0        0     3092 2023-07-03 18:09:06.445592 aiida_wannier90-2.1.0/src/aiida_wannier90/utils.py
--rw-r--r--   0        0        0      648 2023-07-03 18:09:06.465592 aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/__init__.py
--rw-r--r--   0        0        0    11532 2023-07-03 18:09:06.465592 aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/minimal.py
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 aiida_wannier90-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2024-04-19 09:13:11.844320 aiida_wannier90-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2125 2024-04-19 09:13:11.844320 aiida_wannier90-2.2.0/README.md
+-rw-r--r--   0        0        0     4880 2024-05-10 10:16:33.237075 aiida_wannier90-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1973 2024-05-10 10:29:22.529945 aiida_wannier90-2.2.0/src/aiida_wannier90/__init__.py
+-rw-r--r--   0        0        0      201 2024-05-10 10:16:33.237075 aiida_wannier90-2.2.0/src/aiida_wannier90/calculations/__init__.py
+-rw-r--r--   0        0        0    19791 2024-05-10 10:16:33.237075 aiida_wannier90-2.2.0/src/aiida_wannier90/calculations/postw90.py
+-rw-r--r--   0        0        0    23664 2024-04-19 09:14:10.411452 aiida_wannier90-2.2.0/src/aiida_wannier90/calculations/wannier90.py
+-rw-r--r--   0        0        0      802 2024-04-19 09:13:11.852320 aiida_wannier90-2.2.0/src/aiida_wannier90/io/__init__.py
+-rw-r--r--   0        0        0     1814 2024-04-19 09:13:11.864320 aiida_wannier90-2.2.0/src/aiida_wannier90/io/_group_list.py
+-rw-r--r--   0        0        0    15059 2024-05-10 10:16:33.237075 aiida_wannier90-2.2.0/src/aiida_wannier90/io/_write_win.py
+-rw-r--r--   0        0        0    13286 2024-04-19 09:13:11.864320 aiida_wannier90-2.2.0/src/aiida_wannier90/orbitals.py
+-rw-r--r--   0        0        0      163 2024-05-10 10:16:33.237075 aiida_wannier90-2.2.0/src/aiida_wannier90/parsers/__init__.py
+-rw-r--r--   0        0        0    20739 2024-04-19 09:14:10.411452 aiida_wannier90-2.2.0/src/aiida_wannier90/parsers/postw90.py
+-rw-r--r--   0        0        0    23530 2024-04-19 09:14:10.415452 aiida_wannier90-2.2.0/src/aiida_wannier90/parsers/wannier90.py
+-rw-r--r--   0        0        0     3092 2024-04-19 09:13:11.868320 aiida_wannier90-2.2.0/src/aiida_wannier90/utils.py
+-rw-r--r--   0        0        0      648 2024-04-19 09:13:11.868320 aiida_wannier90-2.2.0/src/aiida_wannier90/workflows/__init__.py
+-rw-r--r--   0        0        0    11532 2024-04-19 09:13:11.868320 aiida_wannier90-2.2.0/src/aiida_wannier90/workflows/minimal.py
+-rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 aiida_wannier90-2.2.0/PKG-INFO
```

### Comparing `aiida_wannier90-2.1.0/LICENSE.txt` & `aiida_wannier90-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_wannier90-2.1.0/README.md` & `aiida_wannier90-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This plugin allows to run Wannier90 calculations.
 Examples are provided to show the integration with [Quantum ESPRESSO](https://www.quantum-espresso.org) via the [aiida-quantumespresso](https://github.com/aiidateam/aiida-quantumespresso) plugin.
 
 |     | |
 |-----|----------------------------------------------------------------------------|
 |Latest release| [![PyPI version](https://badge.fury.io/py/aiida-wannier90.svg)](https://badge.fury.io/py/aiida-wannier90) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-wannier90.svg)](https://pypi.python.org/pypi/aiida-wannier90/) |
 |Getting help| [![Docs status](https://readthedocs.org/projects/aiida-wannier90/badge)](http://aiida-wannier90.readthedocs.io/) [![Google Group](https://img.shields.io/badge/-Google%20Group-lightgrey.svg)](https://groups.google.com/forum/#!forum/aiidausers)
-|Build status| [![Build Status](https://github.com/aiidateam/aiida-wannier90/actions/workflows/ci.yml/badge.svg)](https://github.com/aiidateam/aiida-wannier90/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-wannier90/branch/develop/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-wannier90) |
+|Build status| [![Build Status](https://github.com/aiidateam/aiida-wannier90/actions/workflows/ci.yml/badge.svg)](https://github.com/aiidateam/aiida-wannier90/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-wannier90/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-wannier90/tree/main) |
 |Activity| [![PyPI-downloads](https://img.shields.io/pypi/dm/aiida-wannier90.svg?style=flat)](https://pypistats.org/packages/aiida-wannier90) [![Commit Activity](https://img.shields.io/github/commit-activity/m/aiidateam/aiida-wannier90.svg)](https://github.com/aiidateam/aiida-wannier90/pulse)
 
 ## Documentation
 
 The documentation on how to use this plugin package is available on [Read the Docs](http://aiida-wannier90.readthedocs.io/).
 
 ## Acknowledgements
```

### Comparing `aiida_wannier90-2.1.0/pyproject.toml` & `aiida_wannier90-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,48 +23,46 @@
     "Development Status :: 5 - Production/Stable",
     "Framework :: AiiDA",
     "Environment :: Plugins",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Natural Language :: English",
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Science/Research"
 ]
 keywords = ["aiida", "plugin", "wannier90"]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = ["aiida-core>=2.0,<3"]
 
 [project.urls]
 Source = "https://github.com/aiidateam/aiida-wannier90"
 Documentation = "https://aiida-wannier90.readthedocs.io"
 
 [project.optional-dependencies]
 tests = [
     "pytest",
     "pytest-cov",
-    "pytest-regressions~=1.0.6",
-    "pytest-datadir~=1.3.1",
-    "pgtest~=1.3.1",
-    "codecov"
+    "pytest-regressions",
+    "pytest-datadir",
+    "pgtest",
 ]
 pre-commit = [
     "pre-commit",
-    "pylint",
+    "pylint>=3",
     "yapf>=0.28",
     "prospector>=1.3.1",
     "ruamel.yaml"
 ]
 docs = ["sphinx", "sphinx-rtd-theme", "sphinxcontrib-details-directive"]
-atomic_tools = ["ase"]
 
 [project.entry-points."aiida.calculations"]
 "wannier90.wannier90" = "aiida_wannier90.calculations:Wannier90Calculation"
 "wannier90.postw90" = "aiida_wannier90.calculations:Postw90Calculation"
 
 [project.entry-points."aiida.parsers"]
 "wannier90.wannier90" = "aiida_wannier90.parsers:Wannier90Parser"
@@ -169,20 +167,20 @@
 ]
 known_aiida = ['aiida']
 known_aiida_quantumespresso = ['aiida_quantumespresso']
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py38
+envlist = py39
 
 [testenv]
 usedevelop=True
 
-[testenv:py{38,39,310}]
+[testenv:py{39,310,311,312}]
 description = Run the test suite against a python version
 extras = testing
 commands = pytest {posargs}
 
 [testenv:pre-commit]
 description = Run the pre-commit checks
 extras = pre-commit
```

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/__init__.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,12 +26,12 @@
    *Comp. Mat. Sci.* **111**, 218-230 (2016)
    `[Journal link] <https://doi.org/10.1016/j.commatsci.2015.09.013>`_
    `[arXiv link] <https://arxiv.org/abs/1504.01163>`_
 """
 
 __authors__ = "The AiiDA team."
 __license__ = "MIT License, see LICENSE.txt file."
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 from . import calculations, io, orbitals, parsers, utils
 
 __all__ = ("io", "parsers", "orbitals", "calculations", "utils")
```

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/postw90.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/calculations/postw90.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Calculation class for the postw90.x code of Wannier90."""
+
 import fnmatch
 import os
 
 from aiida import orm
 from aiida.common import datastructures, exceptions
 from aiida.engine import CalcJob
 
@@ -74,15 +75,15 @@
         "_dos.dat",
         "_htB.dat",
         "_u.mat",
         "_u_dis.mat",
         ".vdw",
         "_band_proj.dat",
         "_band.labelinfo.dat",
-        ".node_00001.werr",
+        ".node_*.werr",
     )
 
     _DEFAULT_RETRIEVE_TEMPORARY_SUFFIXES = (
         # BoltzWann related files
         "_boltzdos.dat",
         "_elcond.dat",
         "_kappa.dat",
```

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/wannier90.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/calculations/wannier90.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         "_dos.dat",
         "_htB.dat",
         "_u.mat",
         "_u_dis.mat",
         ".vdw",
         "_band_proj.dat",
         "_band.labelinfo.dat",
-        ".node_00001.werr",
+        ".node_*.werr",
     )
 
     @classmethod
     def define(cls, spec):
         """Define the specs."""
         super().define(spec)
         spec.input(
```

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/io/__init__.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/io/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/io/_group_list.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/io/_group_list.py`

 * *Files identical despite different names*

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/io/_write_win.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/io/_write_win.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,16 +326,20 @@
     # In Wannier90 (from the user guide): Values are in
     # fractional coordinates with respect to the primitive
     # reciprocal lattice vectors.
     res = []
     for point1, point2 in path:
         coord1 = point_coords[point1]
         coord2 = point_coords[point2]
-        path_line = f"{point1} {coord1[0]} {coord1[1]} {coord1[2]} "
-        path_line += f" {point2} {coord2[0]} {coord2[1]} {coord2[2]}"
+        path_line = (
+            f"{point1} {coord1[0]:14.10f} {coord1[1]:14.10f} {coord1[2]:14.10f} "
+        )
+        path_line += (
+            f" {point2} {coord2[0]:14.10f} {coord2[1]:14.10f} {coord2[2]:14.10f}"
+        )
         res.append(path_line)
     return res
 
 
 def _format_explicit_kpoint_path(bands_kpoints: orm.KpointsData) -> ty.Tuple:
     """Prepare the lines for the Wannier90 input file related to the `explicit_kpath` and `explicit_kpath_labels`.
```

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/orbitals.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/orbitals.py`

 * *Files identical despite different names*

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/postw90.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/parsers/postw90.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,16 @@
         if error_file_name in out_folder.base.repository.list_object_names():
             self.logger.error(
                 "Errors were found please check the retrieved "
                 f"{error_file_name} file"
             )
             return self.exit_codes.ERROR_WERR_FILE_PRESENT
 
-        # Some times the error files are aiida.node_00001.werr, ...
+        # Some times the error files are aiida.node_XXXXX.werr, ...
+        # The XXXXX are 5-digit index of processor
         error_file_name = re.compile(seedname + r".+?\.werr")
         for filename in out_folder.base.repository.list_object_names():
             if error_file_name.match(filename):
                 self.logger.error(
                     f"Errors were found please check the retrieved {filename} file"
                 )
                 return self.exit_codes.ERROR_WERR_FILE_PRESENT
```

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/wannier90.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/parsers/wannier90.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,16 @@
         if error_file_name in out_folder.base.repository.list_object_names():
             self.logger.error(
                 "Errors were found please check the retrieved "
                 f"{error_file_name} file"
             )
             return self.exit_codes.ERROR_WERR_FILE_PRESENT
 
-        # Some times the error files are aiida.node_00001.werr, ...
+        # Some times the error files are aiida.node_XXXXX.werr, ...
+        # The XXXXX are 5-digit index of processor
         error_file_name = re.compile(seedname + r".+?\.werr")
         for filename in out_folder.base.repository.list_object_names():
             if error_file_name.match(filename):
                 self.logger.error(
                     f"Errors were found please check the retrieved {filename} file"
                 )
                 return self.exit_codes.ERROR_WERR_FILE_PRESENT
```

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/utils.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/__init__.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/minimal.py` & `aiida_wannier90-2.2.0/src/aiida_wannier90/workflows/minimal.py`

 * *Files identical despite different names*

### Comparing `aiida_wannier90-2.1.0/PKG-INFO` & `aiida_wannier90-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 Metadata-Version: 2.1
 Name: aiida-wannier90
-Version: 2.1.0
+Version: 2.2.0
 Summary: AiiDA Plugin for the Wannier90 code
 Keywords: aiida,plugin,wannier90
 Author: Junfeng Qiao, Dominik Gresch, Antimo Marrazzo, Daniel Marchand, Giovanni Pizzi, Norma Rivano, The AiiDA team
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Requires-Dist: aiida-core>=2.0,<3
-Requires-Dist: ase ; extra == "atomic_tools"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive ; extra == "docs"
 Requires-Dist: pre-commit ; extra == "pre-commit"
-Requires-Dist: pylint ; extra == "pre-commit"
+Requires-Dist: pylint>=3 ; extra == "pre-commit"
 Requires-Dist: yapf>=0.28 ; extra == "pre-commit"
 Requires-Dist: prospector>=1.3.1 ; extra == "pre-commit"
 Requires-Dist: ruamel.yaml ; extra == "pre-commit"
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
-Requires-Dist: pytest-regressions~=1.0.6 ; extra == "tests"
-Requires-Dist: pytest-datadir~=1.3.1 ; extra == "tests"
-Requires-Dist: pgtest~=1.3.1 ; extra == "tests"
-Requires-Dist: codecov ; extra == "tests"
+Requires-Dist: pytest-regressions ; extra == "tests"
+Requires-Dist: pytest-datadir ; extra == "tests"
+Requires-Dist: pgtest ; extra == "tests"
 Project-URL: Documentation, https://aiida-wannier90.readthedocs.io
 Project-URL: Source, https://github.com/aiidateam/aiida-wannier90
-Provides-Extra: atomic_tools
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: tests
 
 # aiida-wannier90
 
 AiiDA plugin for the [Wannier90](http://www.wannier.org) code.
 This plugin allows to run Wannier90 calculations.
 Examples are provided to show the integration with [Quantum ESPRESSO](https://www.quantum-espresso.org) via the [aiida-quantumespresso](https://github.com/aiidateam/aiida-quantumespresso) plugin.
 
 |     | |
 |-----|----------------------------------------------------------------------------|
 |Latest release| [![PyPI version](https://badge.fury.io/py/aiida-wannier90.svg)](https://badge.fury.io/py/aiida-wannier90) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-wannier90.svg)](https://pypi.python.org/pypi/aiida-wannier90/) |
 |Getting help| [![Docs status](https://readthedocs.org/projects/aiida-wannier90/badge)](http://aiida-wannier90.readthedocs.io/) [![Google Group](https://img.shields.io/badge/-Google%20Group-lightgrey.svg)](https://groups.google.com/forum/#!forum/aiidausers)
-|Build status| [![Build Status](https://github.com/aiidateam/aiida-wannier90/actions/workflows/ci.yml/badge.svg)](https://github.com/aiidateam/aiida-wannier90/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-wannier90/branch/develop/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-wannier90) |
+|Build status| [![Build Status](https://github.com/aiidateam/aiida-wannier90/actions/workflows/ci.yml/badge.svg)](https://github.com/aiidateam/aiida-wannier90/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-wannier90/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-wannier90/tree/main) |
 |Activity| [![PyPI-downloads](https://img.shields.io/pypi/dm/aiida-wannier90.svg?style=flat)](https://pypistats.org/packages/aiida-wannier90) [![Commit Activity](https://img.shields.io/github/commit-activity/m/aiidateam/aiida-wannier90.svg)](https://github.com/aiidateam/aiida-wannier90/pulse)
 
 ## Documentation
 
 The documentation on how to use this plugin package is available on [Read the Docs](http://aiida-wannier90.readthedocs.io/).
 
 ## Acknowledgements
```

