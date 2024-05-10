# Comparing `tmp/bw-processing-0.9.tar.gz` & `tmp/bw_processing-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw-processing-0.9.tar", last modified: Mon Sep 18 20:06:16 2023, max compression
+gzip compressed data, was "bw_processing-0.9.1.tar", last modified: Fri May 10 20:45:23 2024, max compression
```

## Comparing `bw-processing-0.9.tar` & `bw_processing-0.9.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.710407 bw-processing-0.9/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-08-23 19:48:32.000000 bw-processing-0.9/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       96 2023-08-23 19:48:32.000000 bw-processing-0.9/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)    16363 2023-09-18 20:06:16.710328 bw-processing-0.9/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)    14848 2023-08-23 19:48:32.000000 bw-processing-0.9/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.706220 bw-processing-0.9/bw_processing/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1395 2023-09-18 20:05:52.000000 bw-processing-0.9/bw_processing/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5839 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/array_creation.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1340 2023-09-15 05:31:11.000000 bw-processing-0.9/bw_processing/constants.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    44381 2023-09-15 05:31:11.000000 bw-processing-0.9/bw_processing/datapackage.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1395 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/errors.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.709547 bw-processing-0.9/bw_processing/examples/
--rw-r--r--   0 chrismutel   (501) staff       (20)       73 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/examples/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      602 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/examples/interfaces.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3575 2023-09-15 05:31:11.000000 bw-processing-0.9/bw_processing/examples/parquet_files.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      772 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/examples/simple.zip
--rw-r--r--   0 chrismutel   (501) staff       (20)     1632 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/filesystem.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5612 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/indexing.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4733 2023-09-18 19:57:07.000000 bw-processing-0.9/bw_processing/io_helpers.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5054 2023-09-15 05:31:11.000000 bw-processing-0.9/bw_processing/io_parquet_helpers.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8415 2023-09-15 05:31:11.000000 bw-processing-0.9/bw_processing/io_pyarrow_helpers.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6291 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/merging.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      484 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/proxies.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3819 2023-01-03 15:12:55.000000 bw-processing-0.9/bw_processing/unique_fields.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2948 2023-08-24 20:20:38.000000 bw-processing-0.9/bw_processing/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.709443 bw-processing-0.9/bw_processing.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)    16363 2023-09-18 20:06:16.000000 bw-processing-0.9/bw_processing.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1098 2023-09-18 20:06:16.000000 bw-processing-0.9/bw_processing.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-09-18 20:06:16.000000 bw-processing-0.9/bw_processing.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-23 19:55:37.000000 bw-processing-0.9/bw_processing.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      121 2023-09-18 20:06:16.000000 bw-processing-0.9/bw_processing.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       34 2023-09-18 20:06:16.000000 bw-processing-0.9/bw_processing.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.707977 bw-processing-0.9/dev/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6528 2023-09-11 13:15:06.000000 bw-processing-0.9/dev/calculation_package.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4240 2023-09-11 13:15:06.000000 bw-processing-0.9/dev/loading.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     9654 2023-09-11 13:15:06.000000 bw-processing-0.9/dev/processed_package.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      741 2023-09-11 13:15:06.000000 bw-processing-0.9/dev/resources.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1195 2023-09-11 13:15:06.000000 bw-processing-0.9/dev/speed_tests.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.708151 bw-processing-0.9/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1151 2023-08-23 19:48:32.000000 bw-processing-0.9/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-08-23 19:48:32.000000 bw-processing-0.9/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1673 2023-09-18 20:06:16.710731 bw-processing-0.9/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.709669 bw-processing-0.9/tests/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.708438 bw-processing-0.9/tests/fixtures/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1065 2023-09-15 05:31:11.000000 bw-processing-0.9/tests/fixtures/basic_arrays.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-09-18 20:06:16.708689 bw-processing-0.9/tests/helpers/
--rw-r--r--   0 chrismutel   (501) staff       (20)      112 2023-09-15 05:31:11.000000 bw-processing-0.9/tests/helpers/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      843 2023-09-15 05:31:11.000000 bw-processing-0.9/tests/helpers/basic_array_helpers.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6824 2023-08-24 20:21:32.000000 bw-processing-0.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-10 20:45:19.000000 bw_processing-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 20:45:19.000000 bw_processing-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-10 20:45:23.027037 bw_processing-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-05-10 20:45:19.000000 bw_processing-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/bw_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/array_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44619 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/bw_processing/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/parquet_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/simple.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/io_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/io_parquet_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/io_pyarrow_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/unique_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/bw_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:45:22.000000 bw_processing-0.9.1/bw_processing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/calculation_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/processed_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/speed_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-10 20:45:19.000000 bw_processing-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 20:45:19.000000 bw_processing-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-10 20:45:23.027037 bw_processing-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/fixtures/basic_arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/helpers/basic_array_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/test_utils.py
```

### Comparing `bw-processing-0.9/LICENSE` & `bw_processing-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/PKG-INFO` & `bw_processing-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-processing
-Version: 0.9
+Version: 0.9.1
 Summary: Tools to create structured arrays in a common format
 Home-page: https://github.com/brightway-lca/bw_processing
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -42,26 +42,26 @@
 # bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
 [![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/bw-processing)][pypi status]
-[![License](https://img.shields.io/pypi/l/bw-processing)][license]
+[![License](https://img.shields.io/pypi/l/bw_processing)][license]
 
 [![Read the documentation at https://bw-processing.readthedocs.io/](https://img.shields.io/readthedocs/bw-processing/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/brightway-lca/bw-processing/actions/workflows/python-test.yml/badge.svg)][tests]
+[![Testing](https://github.com/brightway-lca/bw_processing/actions/workflows/python-test.yml/badge.svg)][tests]
 [![Codecov](https://codecov.io/gh/brightway-lca/bw-processing/branch/main/graph/badge.svg)][codecov]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi status]: https://pypi.org/project/bw-processing/
 [read the docs]: https://bw-processing.readthedocs.io/
-[tests]: https://github.com/brightway-lca/bw-processing/actions?workflow=Tests
+[tests]: https://github.com/brightway-lca/bw_processing/actions/workflows/python-test.yml
 [codecov]: https://app.codecov.io/gh/brightway-lca/bw-processing
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Table of Contents
 
 - [Background](#background)
```

### Comparing `bw-processing-0.9/README.md` & `bw_processing-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
 [![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/bw-processing)][pypi status]
-[![License](https://img.shields.io/pypi/l/bw-processing)][license]
+[![License](https://img.shields.io/pypi/l/bw_processing)][license]
 
 [![Read the documentation at https://bw-processing.readthedocs.io/](https://img.shields.io/readthedocs/bw-processing/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/brightway-lca/bw-processing/actions/workflows/python-test.yml/badge.svg)][tests]
+[![Testing](https://github.com/brightway-lca/bw_processing/actions/workflows/python-test.yml/badge.svg)][tests]
 [![Codecov](https://codecov.io/gh/brightway-lca/bw-processing/branch/main/graph/badge.svg)][codecov]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi status]: https://pypi.org/project/bw-processing/
 [read the docs]: https://bw-processing.readthedocs.io/
-[tests]: https://github.com/brightway-lca/bw-processing/actions?workflow=Tests
+[tests]: https://github.com/brightway-lca/bw_processing/actions/workflows/python-test.yml
 [codecov]: https://app.codecov.io/gh/brightway-lca/bw-processing
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Table of Contents
 
 - [Background](#background)
```

### Comparing `bw-processing-0.9/bw_processing/__init__.py` & `bw_processing-0.9.1/bw_processing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "reset_index",
     "safe_filename",
     "simple_graph",
     "UNCERTAINTY_DTYPE",
     "UndefinedInterface",
 )
 
-__version__ = "0.9"
+__version__ = "0.9.1"
 
 
 from .array_creation import create_array, create_structured_array
 from .constants import (
     DEFAULT_LICENSES,
     INDICES_DTYPE,
     UNCERTAINTY_DTYPE,
```

### Comparing `bw-processing-0.9/bw_processing/array_creation.py` & `bw_processing-0.9.1/bw_processing/array_creation.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/constants.py` & `bw_processing-0.9.1/bw_processing/constants.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/datapackage.py` & `bw_processing-0.9.1/bw_processing/datapackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         self.metadata = {
             "profile": "data-package",
             "name": name,
             "id": id_ or uuid.uuid4().hex,
             "licenses": (metadata or {}).get("licenses", DEFAULT_LICENSES),
             "resources": [],
-            "created": datetime.datetime.utcnow().isoformat("T") + "Z",
+            "created": datetime.datetime.now(datetime.UTC).isoformat("T") + "Z",
             "combinatorial": combinatorial,
             "sequential": sequential,
             "seed": seed,
             "sum_intra_duplicates": sum_intra_duplicates,
             "sum_inter_duplicates": sum_inter_duplicates,
             "matrix_serialize_format_type": matrix_serialize_format_type.value,
         }
@@ -1049,25 +1049,24 @@
     All arguments are optional; if a `PyFilesystem2 <https://docs.pyfilesystem.org/en/latest/>`__ filesystem is not provided, a `MemoryFS <https://docs.pyfilesystem.org/en/latest/reference/memoryfs.html>`__ will be used.
 
     All metadata elements should follow the `datapackage specification <https://frictionlessdata.io/specs/data-package/>`__.
 
     Licenses are specified as a list in ``metadata``. The default license is the `Open Data Commons Public Domain Dedication and License v1.0 <http://opendatacommons.org/licenses/pddl/>`__.
 
     Args:
-
-        * fs: A `Filesystem`, optional. A new `MemoryFS` is used if not provided.
-        * name: `str`, optional. A new uuid is used if not provided.
-        * id_. `str`, optional. A new uuid is used if not provided.
-        * metadata. `dict`, optional. Metadata dictionary following datapackage specification; see above.
-        * combinatorial. `bool`, default `False.: Policy on how to sample columns across multiple data arrays; see readme.
-        * sequential. `bool`, default `False.: Policy on how to sample columns in data arrays; see readme.
-        * seed. `int`, optional. Seed to use in random number generator.
-        * sum_intra_duplicates. `bool`, default `True`. Should duplicate elements in a single data resource be summed together, or should the last value replace previous values.
-        * sum_inter_duplicates. `bool`, default `False`. Should duplicate elements in across data resources be summed together, or should the last value replace previous values. Order of data resources is given by the order they are added to the data package.
-        * matrix_serialize_format_type. `MatrixSerializeFormat`, default `MatrixSerializeFormat.NUMPY`. Matrix serialization format type.
+        * fs: A ``Filesystem``, optional. A new ``MemoryFS`` is used if not provided.
+        * name: ``str``, optional. A new uuid is used if not provided.
+        * `id_`: ``str``, optional. A new uuid is used if not provided.
+        * metadata: ``dict``, optional. Metadata dictionary following datapackage specification; see above.
+        * combinatorial: ``bool``, default ``False`` .: Policy on how to sample columns across multiple data arrays; see readme.
+        * sequential: ``bool``, default ``False`` .: Policy on how to sample columns in data arrays; see readme.
+        * seed: ``int``, optional. Seed to use in random number generator.
+        * sum_intra_duplicates: ``bool``, default ``True``. Should duplicate elements in a single data resource be summed together, or should the last value replace previous values.
+        * sum_inter_duplicates: ``bool``, default ``False``. Should duplicate elements in across data resources be summed together, or should the last value replace previous values. Order of data resources is given by the order they are added to the data package.
+        * matrix_serialize_format_type: ``MatrixSerializeFormat``, default ``MatrixSerializeFormat.NUMPY``. Matrix serialization format type.
 
     Returns:
 
         A `Datapackage` instance.
 
     """
     obj = Datapackage()
@@ -1095,47 +1094,54 @@
 
     Can load proxies to data instead of the data itself, which can be useful when interacting with large arrays or large packages where only a subset of the data will be accessed.
 
     Proxies use something similar to `functools.partial` to create a callable class instead of returning the raw data (see https://github.com/brightway-lca/bw_processing/issues/9 for why we can't just use `partial`). datapackage access methods (i.e. `.get_resource`) will automatically resolve proxies when needed.
 
     Args:
 
-        * fs_or_obj. A `Filesystem` or an instance of `DatapackageBase`.
-        * mmap_mode. `str`, optional. Define memory mapping mode to use when loading Numpy arrays.
-        * proxy. bool, default `False`. Load proxies instead of complete Numpy arrays; see above.
+        * fs_or_obj: A `Filesystem` or an instance of `DatapackageBase`.
+        * mmap_mode: `str`, optional. Define memory mapping mode to use when loading Numpy arrays.
+        * proxy: bool, default `False`. Load proxies instead of complete Numpy arrays; see above.
 
     Returns:
 
         A `Datapackage` instance.
 
     """
     if isinstance(fs_or_obj, DatapackageBase):
         obj = fs_or_obj
     else:
         obj = Datapackage()
         obj._load(fs=fs_or_obj, mmap_mode=mmap_mode, proxy=proxy)
     return obj
 
 
-def simple_graph(data: dict, fs: Optional[FS] = None, **metadata):
+def simple_graph(data: dict, fs: Optional[FS] = None, **metadata)->Datapackage:
     """Easy creation of simple datapackages with only persistent vectors.
 
-    ``data`` is a dictionary with the form:
+    Args:
+        * data: is a dictionary.
+            The data dictionary has the form::
 
-    ..code-block:: python
+                {
+                    matrix_name: [ 
+                    (row_id, col_id, value, flip) 
+                    ]
+                }
 
-        matrix_name (str): [
-            (row id (int), col id (int), value (float), flip (bool, default False))
-        ]
 
-    ``fs`` is a filesystem.
+            Where `row_id` and `col_id are an `int` s, value is a `float` and flip is a `bool`  (False by default).
 
-    ``metadata`` are passed as kwargs to ``create_datapackage()``.
+        * fs: is a filesystem.
+        * metadata: are passed as kwargs to ``create_datapackage()``.
 
-    Returns the datapackage."""
+    Returns:
+        the datapackage.
+
+    """
     dp = create_datapackage(fs=fs, **metadata)
     for key, value in data.items():
         indices_array = np.array([row[:2] for row in value], dtype=INDICES_DTYPE)
         data_array = np.array([row[2] for row in value])
         flip_array = np.array(
             [row[3] if len(row) > 3 else False for row in value], dtype=bool
         )
```

### Comparing `bw-processing-0.9/bw_processing/errors.py` & `bw_processing-0.9.1/bw_processing/errors.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/examples/interfaces.py` & `bw_processing-0.9.1/bw_processing/examples/interfaces.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/examples/parquet_files.py` & `bw_processing-0.9.1/bw_processing/examples/parquet_files.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/examples/simple.zip` & `bw_processing-0.9.1/bw_processing/examples/simple.zip`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/filesystem.py` & `bw_processing-0.9.1/bw_processing/filesystem.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/indexing.py` & `bw_processing-0.9.1/bw_processing/indexing.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/io_helpers.py` & `bw_processing-0.9.1/bw_processing/io_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from fs.base import FS
 from fs.osfs import OSFS
 from fs.zipfs import ZipFS
 
 from .constants import MatrixSerializeFormat
 from .errors import InvalidMimetype
 from .proxies import Proxy
+
 try:
     from .io_parquet_helpers import load_ndarray_from_parquet, save_arr_to_parquet
+
     PARQUET = True
 except ImportError:
     load_ndarray_from_parquet = None
     save_arr_to_parquet = None
     PARQUET = False
```

### Comparing `bw-processing-0.9/bw_processing/io_parquet_helpers.py` & `bw_processing-0.9.1/bw_processing/io_parquet_helpers.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/io_pyarrow_helpers.py` & `bw_processing-0.9.1/bw_processing/io_pyarrow_helpers.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing/merging.py` & `bw_processing-0.9.1/bw_processing/merging.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
         resource["nrows"] = len(data)
     return resource
 
 
 def add_resource_suffix(metadata: dict, suffix: str) -> dict:
     """Update the ``name``, ``path``, and ``group`` values to include ``suffix``. The suffix comes after the basename but after the data type suffix (e.g. indices, data).
 
-    Given the suffix _foo" and the metadata:
+    Given the suffix ``_foo`` and the metadata::
 
         {
             "name": "sa-data-vector-from-dict.indices",
             "path": "sa-data-vector-from-dict.indices.npy",
             "group": "sa-data-vector-from-dict",
         }
 
-    Returns:
+    It will return::
 
         {
             "name": "sa-data-vector-from-dict_foo.indices",
             "path": "sa-data-vector-from-dict_foo.indices.npy",
             "group": "sa-data-vector-from-dict_foo",
         }
```

### Comparing `bw-processing-0.9/bw_processing/unique_fields.py` & `bw_processing-0.9.1/bw_processing/unique_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def greedy_set_cover(data, exclude=None, raise_error=True):
     """Find unique set of attributes that uniquely identifies each element in ``data``.
 
     Feature selection is a well known problem, and is analogous to the `set cover problem <https://en.wikipedia.org/wiki/Set_cover_problem>`__, for which there is a `well known heuristic <https://en.wikipedia.org/wiki/Set_cover_problem#Greedy_algorithm>`__.
 
-    Example:
+    Example::
 
         data = [
             {'a': 1, 'b': 2, 'c': 3},
             {'a': 2, 'b': 2, 'c': 3},
             {'a': 1, 'b': 2, 'c': 4},
         ]
         greedy_set_cover(data)
@@ -69,15 +69,15 @@
 
 
 def as_unique_attributes(data, exclude=None, include=None, raise_error=False):
     """Format ``data`` as unique set of attributes and values for use in ``create_processed_datapackage``.
 
     Each element in ``data`` must have the attribute ``id``, and it must be unique. However, the field "id" is not used in selecting the unique set of attributes.
 
-    If no set of attributes is found that uniquely identifies all features is found, all fields are used. To have this case raise an error, pass ``raise_error=True``.
+    If no set of attributes is found that uniquely identifies all features is found, all fields are used. To have this case raise an error, pass ``raise_error=True``.::
 
         data = [
             {},
         ]
 
     Args:
         data (iterable): List of dictionaries with the same fields.
@@ -85,14 +85,15 @@
         include (iterable): Fields to include when returning, even if not unique
 
     Returns:
         (list of field names as strings, dictionary of data ids to values for given field names)
 
     Raises:
         InconsistentFields: Not all features provides all fields.
+
     """
     include = set(include or [])
     fields = greedy_set_cover(data, exclude=exclude, raise_error=raise_error)
 
     if len({tuple(sorted(obj.keys())) for obj in data}) > 1:
         raise InconsistentFields
```

### Comparing `bw-processing-0.9/bw_processing/utils.py` & `bw_processing-0.9.1/bw_processing/utils.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/bw_processing.egg-info/PKG-INFO` & `bw_processing-0.9.1/bw_processing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-processing
-Version: 0.9
+Version: 0.9.1
 Summary: Tools to create structured arrays in a common format
 Home-page: https://github.com/brightway-lca/bw_processing
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -42,26 +42,26 @@
 # bw-processing
 
 Library for storing numeric data for use in matrix-based calculations. Designed for use with the [Brightway life cycle assessment framework](https://brightway.dev/).
 
 [![PyPI](https://img.shields.io/pypi/v/bw-processing.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw-processing.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/bw-processing)][pypi status]
-[![License](https://img.shields.io/pypi/l/bw-processing)][license]
+[![License](https://img.shields.io/pypi/l/bw_processing)][license]
 
 [![Read the documentation at https://bw-processing.readthedocs.io/](https://img.shields.io/readthedocs/bw-processing/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/brightway-lca/bw-processing/actions/workflows/python-test.yml/badge.svg)][tests]
+[![Testing](https://github.com/brightway-lca/bw_processing/actions/workflows/python-test.yml/badge.svg)][tests]
 [![Codecov](https://codecov.io/gh/brightway-lca/bw-processing/branch/main/graph/badge.svg)][codecov]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi status]: https://pypi.org/project/bw-processing/
 [read the docs]: https://bw-processing.readthedocs.io/
-[tests]: https://github.com/brightway-lca/bw-processing/actions?workflow=Tests
+[tests]: https://github.com/brightway-lca/bw_processing/actions/workflows/python-test.yml
 [codecov]: https://app.codecov.io/gh/brightway-lca/bw-processing
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Table of Contents
 
 - [Background](#background)
```

### Comparing `bw-processing-0.9/bw_processing.egg-info/SOURCES.txt` & `bw_processing-0.9.1/bw_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/dev/calculation_package.py` & `bw_processing-0.9.1/dev/calculation_package.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/dev/loading.py` & `bw_processing-0.9.1/dev/loading.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/dev/processed_package.py` & `bw_processing-0.9.1/dev/processed_package.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/dev/resources.py` & `bw_processing-0.9.1/dev/resources.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/dev/speed_tests.py` & `bw_processing-0.9.1/dev/speed_tests.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/setup.cfg` & `bw_processing-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/tests/fixtures/basic_arrays.py` & `bw_processing-0.9.1/tests/fixtures/basic_arrays.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/tests/helpers/basic_array_helpers.py` & `bw_processing-0.9.1/tests/helpers/basic_array_helpers.py`

 * *Files identical despite different names*

### Comparing `bw-processing-0.9/tests/test_utils.py` & `bw_processing-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

