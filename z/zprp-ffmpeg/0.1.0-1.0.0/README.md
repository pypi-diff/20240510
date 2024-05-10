# Comparing `tmp/zprp_ffmpeg-0.1.0.tar.gz` & `tmp/zprp_ffmpeg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zprp_ffmpeg-0.1.0.tar", last modified: Mon Apr 29 22:30:32 2024, max compression
+gzip compressed data, was "zprp_ffmpeg-1.0.0.tar", max compression
```

## Comparing `zprp_ffmpeg-0.1.0.tar` & `zprp_ffmpeg-1.0.0.tar`

### file list

```diff
@@ -1,66 +1,16 @@
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      740 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/.bumpversion.cfg
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1992 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/.cookiecutterrc
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      179 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.coveragerc
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      353 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.editorconfig
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/.github/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/.github/workflows/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     8747 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/.github/workflows/github-actions.yml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      686 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      282 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.readthedocs.yml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       83 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/AUTHORS.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1263 2024-04-29 22:13:47.000000 zprp_ffmpeg-0.1.0/CHANGELOG.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2348 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1088 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/LICENSE
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      427 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/MANIFEST.in
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     5175 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/PKG-INFO
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     4266 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/README.rst
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/ci/
--rwxr-xr-x   0 tomwez    (1000) tomwez    (1000)     2867 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/ci/bootstrap.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       72 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/ci/requirements.txt
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/ci/templates/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/ci/templates/.github/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/ci/templates/.github/workflows/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     4006 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/docs/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       28 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/authors.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       30 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/changelog.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1139 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/docs/conf.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       33 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/contributing.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      244 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/index.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       91 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/installation.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       27 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/readme.rst
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/docs/reference/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       63 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/reference/index.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      174 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/reference/zprp_ffmpeg.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       29 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/requirements.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      109 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/spelling_wordlist.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       74 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/usage.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1297 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/pyproject.toml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      843 2024-04-10 14:40:08.000000 zprp_ffmpeg-0.1.0/pytest.ini
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       38 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/setup.cfg
--rwxr-xr-x   0 tomwez    (1000) tomwez    (1000)     4096 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/setup.py
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/src/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      638 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/BaseConnector.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2598 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/FilterGraph.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)        0 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/PopenCommunicator.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1326 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/ProcessConnector.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      327 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/__init__.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      392 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/__main__.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      991 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/_api_compat.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1812 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/_zprp_ffmpeg.c
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      826 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/cli.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      153 2024-04-10 16:02:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/filters.py
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     5175 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/PKG-INFO
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1209 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/SOURCES.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)        1 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/dependency_links.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       53 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/entry_points.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)        1 2024-03-19 09:50:16.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/not-zip-safe
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       12 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/top_level.txt
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/tests/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      290 2024-04-10 14:40:08.000000 zprp_ffmpeg-0.1.0/tests/test_ProcessConnector.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      257 2024-04-10 16:11:09.000000 zprp_ffmpeg-0.1.0/tests/test_kkroening_api.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       83 2024-04-10 14:40:08.000000 zprp_ffmpeg-0.1.0/tests/test_zprp_ffmpeg.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1706 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/tox.ini
+-rw-r--r--   0        0        0       83 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1088 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4266 2024-05-10 14:32:43.968463 zprp_ffmpeg-1.0.0/README.rst
+-rw-r--r--   0        0        0     1831 2024-05-10 14:32:43.968463 zprp_ffmpeg-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      638 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/BaseConnector.py
+-rw-r--r--   0        0        0     3528 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/FilterGraph.py
+-rw-r--r--   0        0        0     1389 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/ProcessConnector.py
+-rw-r--r--   0        0        0      402 2024-05-10 14:32:43.968463 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/__init__.py
+-rw-r--r--   0        0        0      392 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/__main__.py
+-rw-r--r--   0        0        0     1023 2024-05-10 14:14:20.248797 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/_api_compat.py
+-rw-r--r--   0        0        0     1812 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/_zprp_ffmpeg.c
+-rw-r--r--   0        0        0      826 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/cli.py
+-rw-r--r--   0        0        0      153 2024-04-10 16:02:25.189086 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/filters.py
+-rw-r--r--   0        0        0     3680 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/generated_filters.py
+-rw-r--r--   0        0        0        0 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/py.typed
+-rw-r--r--   0        0        0     4966 1970-01-01 00:00:00.000000 zprp_ffmpeg-1.0.0/PKG-INFO
```

### Comparing `zprp_ffmpeg-0.1.0/LICENSE` & `zprp_ffmpeg-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-0.1.0/PKG-INFO` & `zprp_ffmpeg-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 Metadata-Version: 2.1
 Name: zprp-ffmpeg
-Version: 0.1.0
-Summary: Implementation of the successor to the ffmpeg-python library
-Home-page: https://github.com/Madghostek/zprp-ffmpeg
-Author: 
-Author-email: 
+Version: 1.0.0
+Summary: ffmpeg filter graph bindings for python
 License: MIT
-Project-URL: Documentation, https://zprp-ffmpeg.readthedocs.io/
-Project-URL: Changelog, https://zprp-ffmpeg.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/Madghostek/zprp-ffmpeg/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
+Author: Your Name
+Author-email: you@example.com
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-License-File: LICENSE
-License-File: AUTHORS.rst
+Requires-Dist: pycparser (>=2.22,<3.0)
+Requires-Dist: pytest (>=8.1.1,<9.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
+Description-Content-Type: text/x-rst
 
 ===============
 Design proposal
 ===============
 Biblioteka ma za zadanie zastąpić i rozszerzyć istniejącą bibliotekę (https://github.com/kkroening/ffmpeg-python)
 
 Minimalną funkcjonalność, którą chcemy zaimplementować, to ta oferowana przez powyższą bibliotekę, czyli korzystanie z grafów filtrów poprzez prosty interfejs. Poza tym, zależy nam na lepszej integracji z IDE (opisy filtrów w docstringach, typy argumentów), żeby ograniczyć potrzebę krążenia po dokumentacji FFmpeg.
@@ -75,16 +63,61 @@
 Dokumentacja będzie pisana regularnie wraz z kodem jako docstringi
 
 
 ========
 Overview
 ========
 
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+
+    * - docs
+      - |docs|
+    * - tests
+      - |github-actions| |codecov|
+    * - package
+      - |version| |wheel| |supported-versions| |supported-implementations| |commits-since|
+.. |docs| image:: https://readthedocs.org/projects/zprp-ffmpeg/badge/?style=flat
+    :target: https://readthedocs.org/projects/zprp-ffmpeg/
+    :alt: Documentation Status
+
+.. |github-actions| image:: https://github.com/ffmpeg-zprp/zprp-ffmpeg/actions/workflows/github-actions.yml/badge.svg
+    :alt: GitHub Actions Build Status
+    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/actions
+
+.. |codecov| image:: https://codecov.io/gh/ffmpeg-zprp/zprp-ffmpeg/branch/main/graphs/badge.svg?branch=main
+    :alt: Coverage Status
+    :target: https://app.codecov.io/gh/ffmpeg-zprp/zprp-ffmpeg
+
+.. |version| image:: https://img.shields.io/pypi/v/zprp-ffmpeg.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/zprp-ffmpeg
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/zprp-ffmpeg.svg
+    :alt: PyPI Wheel
+    :target: https://pypi.org/project/zprp-ffmpeg
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/zprp-ffmpeg.svg
+    :alt: Supported versions
+    :target: https://pypi.org/project/zprp-ffmpeg
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/zprp-ffmpeg.svg
+    :alt: Supported implementations
+    :target: https://pypi.org/project/zprp-ffmpeg
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v1.0.0.svg
+    :alt: Commits since latest release
+    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v1.0.0...main
 
 
+
+.. end-badges
+
 Implementation of the successor to the ffmpeg-python library
 
 * Free software: MIT license
 
 Installation
 ============
 
@@ -124,28 +157,7 @@
             tox
 
     - - Other
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
-### Changelog
-
-All notable changes to this project will be documented in this file. Dates are displayed in UTC.
-
-#### [v0.1.0](https://github.com/Madghostek/zprp-ffmpeg/compare/v0.0.0...v0.1.0)
-
-> 29 April 2024
-
-- Mypy [`#2`](https://github.com/Madghostek/zprp-ffmpeg/pull/2)
-- Ffmpeg connector and initial stream class logic [`#1`](https://github.com/Madghostek/zprp-ffmpeg/pull/1)
-- feature: add very basic graph structure and crucial api parts [`cb6c4fd`](https://github.com/Madghostek/zprp-ffmpeg/commit/cb6c4fd2473b66f968131dfd806e82902395f78b)
-- feature: crucial base classes for the package [`e133438`](https://github.com/Madghostek/zprp-ffmpeg/commit/e133438f08fbf248f28e7d67b4c40640ed9f3717)
-- fix: remove not needed class, fix mypy type errors [`91aa8cf`](https://github.com/Madghostek/zprp-ffmpeg/commit/91aa8cf23ad051d4126083c57f6749bd49d4d517)
-
-#### v0.0.0
-
-> 26 March 2024
-
-- Change authors [`2892f0f`](https://github.com/Madghostek/zprp-ffmpeg/commit/2892f0fac9b13743e06969e8e8a46ee8792541dd)
-- Restore design proposal [`09e47f5`](https://github.com/Madghostek/zprp-ffmpeg/commit/09e47f5279fc933980b10e220292e400f2635b4e)
-- Try to revert merge. [`6c4fda6`](https://github.com/Madghostek/zprp-ffmpeg/commit/6c4fda6d834687cc2a3e4e9cca4df722df1356aa)
```

### Comparing `zprp_ffmpeg-0.1.0/README.rst` & `zprp_ffmpeg-1.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/zprp-ffmpeg
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/zprp-ffmpeg.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/zprp-ffmpeg
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v0.1.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v1.0.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v0.1.0...main
+    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v1.0.0...main
 
 
 
 .. end-badges
 
 Implementation of the successor to the ffmpeg-python library
```

### Comparing `zprp_ffmpeg-0.1.0/pyproject.toml` & `zprp_ffmpeg-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,47 @@
+[tool.poetry]
+name = "zprp-ffmpeg"
+version = "1.0.0"
+description = "ffmpeg filter graph bindings for python"
+authors = ["Your Name <you@example.com>"]
+license = "MIT"
+readme = "README.rst"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+pytest = "^8.1.1"
+pycparser = "^2.22"
+tqdm = "^4.66.4"
+
+[tool.poetry.group.typecheck.dependencies]
+types-tqdm = "^4.66.0.20240417"
+mypy = "^1.10.0"
+
+
 [build-system]
-requires = [
-    "setuptools>=30.3.0",
-]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 extend-exclude = ["static", "ci/templates"]
 line-length = 140
 src = ["src", "tests"]
 target-version = "py38"
 
+
 [tool.ruff.lint.per-file-ignores]
 "ci/*" = ["S"]
 
 [tool.ruff.lint]
 ignore = [
     "RUF001", # ruff-specific rules ambiguous-unicode-character-string
     "S101", # flake8-bandit assert
     "S308", # flake8-bandit suspicious-mark-safe-usage
     "E501", # pycodestyle line-too-long
+    "E741", # "I,O,l" variable names (generated ffmpeg filters have that...)
 ]
 select = [
     "B", # flake8-bugbear
     "C4", # flake8-comprehensions
     "DTZ", # flake8-datetimez
     "E", # pycodestyle errors
     "EXE", # flake8-executable
@@ -50,8 +70,9 @@
 force-single-line = true
 
 [tool.black]
 line-length = 140
 target-version = ["py38"]
 
 [tool.mypy]
-disable_error_code = ["import-not-found"] # temporarytem
+implicit_reexport = true
+exclude = ["src/filters_autogen/FFmpeg/*","src/filters_autogen/pycparser/*"]
```

### Comparing `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/BaseConnector.py` & `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/BaseConnector.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     """
     Abstract class for talking with ffmpeg.
 
     A connector always needs a `run` method to execute something user wants.
     """
 
     # this is basically a named constructor
-    @abstractmethod
     @classmethod
+    @abstractmethod
     def run(cls, graph: Stream) -> "BaseConnector":
         """Executes given fliter graph
         :param graph: filter graph describing user operations.
 
         :return: a handle to read output from ffmpeg, for example stdout from process."""
 
     @abstractmethod
```

### Comparing `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/ProcessConnector.py` & `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/ProcessConnector.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import subprocess
 
 from .BaseConnector import BaseConnector
 from .FilterGraph import Stream
 
 
 class ProcessConnector(BaseConnector):
-
     # @TODO: this isn't ideal because attacker can sideload malicious executable...
     # Maybe warn user to set this in config for safety?
     ffmpeg_executable_path = "ffmpeg"
 
     def __init__(self, ffmpeg_process) -> None:
         self.ffmpeg_process: subprocess.Popen = ffmpeg_process
         super().__init__()
@@ -19,24 +18,27 @@
     def compile(graph: Stream) -> str:
         """
         Builds a command for ffmpeg from FilterGraph
 
         :param graph: the graph to compile
         :return: a string to pass as an argument to ffmpeg
         """
-        # @TODO: implement this once FilterGraph is done
-        return "-i input.mp4 -vf hflip -y output.mpt"
+
+        command = [node.get_command() for node in graph._nodes]
+
+        return " ".join(command)
 
     @classmethod
-    def run(cls, graph: Stream) -> "BaseConnector":
+    def run(cls, graph: Stream, extra_options: str = "") -> "BaseConnector":
         """
         Builds a command from FilterGraph, starts ffmpeg process, and passes the command.
 
         :return: subprocess.Popen instance
         """
 
-        command = ProcessConnector.compile(graph)
+        command = ProcessConnector.compile(graph) + extra_options
+        print("Command:", command)
         ffmpeg_process = subprocess.Popen([ProcessConnector.ffmpeg_executable_path, *shlex.split(command)])  # noqa: S603
         return cls(ffmpeg_process)
 
     def communicate(self):
         return self.ffmpeg_process.communicate()
```

### Comparing `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/_api_compat.py` & `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/_api_compat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """compatibility layer to match the kkroening library.
-   @TODO: better docstrings"""
+@TODO: better docstrings"""
 
 from typing import Tuple
 
 from zprp_ffmpeg.BaseConnector import BaseConnector
 
 from .FilterGraph import SinkFilter
 from .FilterGraph import SourceFilter
@@ -20,16 +20,16 @@
 def output(stream: Stream, filename: str):
     sink = SinkFilter(filename)
     stream.append(sink)
     return stream
 
 
 # this api always uses process
-def run(stream: Stream) -> Tuple[str, str]:
+def run(stream: Stream, extra_options: str) -> Tuple[str, str]:
     """Returns (stdout,stderr) tuple"""
-    return ProcessConnector.run(stream).communicate()
+    return ProcessConnector.run(stream, extra_options).communicate()
 
 
 # this api always uses process
 def run_async(stream: Stream) -> BaseConnector:
     """Returns handle to a process. Can raise an exception if script tries to terminate before ffmpeg is done."""
     return ProcessConnector.run(stream)
```

### Comparing `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/_zprp_ffmpeg.c` & `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/_zprp_ffmpeg.c`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/cli.py` & `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/cli.py`

 * *Files identical despite different names*

