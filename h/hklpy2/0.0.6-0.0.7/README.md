# Comparing `tmp/hklpy2-0.0.6.tar.gz` & `tmp/hklpy2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hklpy2-0.0.6.tar", last modified: Wed May  8 20:10:22 2024, max compression
+gzip compressed data, was "hklpy2-0.0.7.tar", last modified: Fri May 10 00:48:07 2024, max compression
```

## Comparing `hklpy2-0.0.6.tar` & `hklpy2-0.0.7.tar`

### file list

```diff
@@ -1,63 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.442913 hklpy2-0.0.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.442913 hklpy2-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-08 20:10:14.000000 hklpy2-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 20:10:14.000000 hklpy2-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-08 20:10:22.450913 hklpy2-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-08 20:10:14.000000 hklpy2-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/source/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/source/api/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends/hkl_soleil.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends/no_op.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/lattice.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/reflection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/sample.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/z_misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/substitutions.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 20:10:14.000000 hklpy2-0.0.6/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/hklpy2/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/hkl_soleil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/no_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/tests/test_hkl_soleil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/notes.md
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-08 20:10:14.000000 hklpy2-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:10:22.450913 hklpy2-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.916697 hklpy2-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.908697 hklpy2-0.0.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 00:47:58.000000 hklpy2-0.0.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.908697 hklpy2-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-10 00:47:58.000000 hklpy2-0.0.7/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-10 00:47:58.000000 hklpy2-0.0.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-10 00:47:58.000000 hklpy2-0.0.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-10 00:47:58.000000 hklpy2-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-10 00:47:58.000000 hklpy2-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 00:47:58.000000 hklpy2-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-10 00:48:07.916697 hklpy2-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-10 00:47:58.000000 hklpy2-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.908697 hklpy2-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.908697 hklpy2-0.0.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.912697 hklpy2-0.0.7/docs/source/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.912697 hklpy2-0.0.7/docs/source/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/backends/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/backends/hkl_soleil.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/backends/no_op.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/backends/th_tth_q.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/lattice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/reflection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/sample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api/z_misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.912697 hklpy2-0.0.7/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 00:47:58.000000 hklpy2-0.0.7/docs/source/substitutions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-10 00:47:58.000000 hklpy2-0.0.7/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.912697 hklpy2-0.0.7/hklpy2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.912697 hklpy2-0.0.7/hklpy2/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/hkl_soleil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/no_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.912697 hklpy2-0.0.7/hklpy2/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/tests/test_hkl_soleil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/tests/test_th_tth_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/backends/th_tth_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.916697 hklpy2-0.0.7/hklpy2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/tests/test_demo_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/tests/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/tests/test_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-10 00:47:58.000000 hklpy2-0.0.7/hklpy2/tests/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:48:07.916697 hklpy2-0.0.7/hklpy2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-10 00:48:07.000000 hklpy2-0.0.7/hklpy2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-10 00:48:07.000000 hklpy2-0.0.7/hklpy2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:48:07.000000 hklpy2-0.0.7/hklpy2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 00:48:07.000000 hklpy2-0.0.7/hklpy2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 00:48:07.000000 hklpy2-0.0.7/hklpy2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 00:48:07.000000 hklpy2-0.0.7/hklpy2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-10 00:47:58.000000 hklpy2-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 00:48:07.916697 hklpy2-0.0.7/setup.cfg
```

### Comparing `hklpy2-0.0.6/.github/workflows/code.yml` & `hklpy2-0.0.7/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/.github/workflows/docs.yml` & `hklpy2-0.0.7/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -35,20 +35,24 @@
         if: ${{ github.event.inputs.deploy }}
         run: |
           echo "The docs will be published from this workflow run."
 
       - name: Set time zone
         run: echo "TZ=America/Chicago" >> "$GITHUB_ENV"
 
+      - name: install pandoc in the OS
+        run: sudo apt-get install pandoc
+
       - name: Sphinx build
         id: deployment
         uses: sphinx-notes/pages@v3
         with:
           documentation_path: ./docs/source
           publish: false
+          python_version: 3.12
           requirements_path: ./docs/requirements.txt
 
       - name: Diagnostic
         run: ls -lAFgh ${{ steps.deployment.outputs.artifact }}
     
       - name: Upload Docs ZIP file as artifact
         uses: actions/upload-artifact@v4
```

### Comparing `hklpy2-0.0.6/.github/workflows/pypi.yml` & `hklpy2-0.0.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/.gitignore` & `hklpy2-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/LICENSE` & `hklpy2-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/PKG-INFO` & `hklpy2-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hklpy2
-Version: 0.0.6
+Version: 0.0.7
 Summary: 2nd generation diffractometer controls for the Bluesky Framework.
 Author-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 Maintainer-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 License: Copyright (c) 2023-2024, UChicago Argonne, LLC
         
         All Rights Reserved
         
@@ -92,13 +92,13 @@
 
 NOTE:  this project at initial development
 
 | Name | Downloads | Version | Platforms | PyPI | Coverage |
 | --- | --- | --- | --- | --- | --- |
 | [![Conda Package](https://img.shields.io/badge/package-hklpy2-green.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![PyPi](https://img.shields.io/pypi/v/hklpy2.svg)](https://pypi.python.org/pypi/hklpy2) | [![Coverage Status](https://coveralls.io/repos/github/prjemian/hklpy2/badge.svg?branch=main)](https://coveralls.io/github/prjemian/hklpy2?branch=main) |
 
-Controls for using diffractometers within the [Bluesky
+2nd generation controls for using diffractometers within the [Bluesky
 Framework](https://blueskyproject.io).
 
 ## References
 
 - hklpy2 documentation: <https://prjemian.github.io/hklpy2>
```

### Comparing `hklpy2-0.0.6/README.md` & `hklpy2-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 
 NOTE:  this project at initial development
 
 | Name | Downloads | Version | Platforms | PyPI | Coverage |
 | --- | --- | --- | --- | --- | --- |
 | [![Conda Package](https://img.shields.io/badge/package-hklpy2-green.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![PyPi](https://img.shields.io/pypi/v/hklpy2.svg)](https://pypi.python.org/pypi/hklpy2) | [![Coverage Status](https://coveralls.io/repos/github/prjemian/hklpy2/badge.svg?branch=main)](https://coveralls.io/github/prjemian/hklpy2?branch=main) |
 
-Controls for using diffractometers within the [Bluesky
+2nd generation controls for using diffractometers within the [Bluesky
 Framework](https://blueskyproject.io).
 
 ## References
 
 - hklpy2 documentation: <https://prjemian.github.io/hklpy2>
```

### Comparing `hklpy2-0.0.6/docs/Makefile` & `hklpy2-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/docs/make.bat` & `hklpy2-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/docs/source/api/backends.rst` & `hklpy2-0.0.7/docs/source/api/backends.rst`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 .. _api.backends.set:
 
 How to select a Solver
 ----------------------
 
 To select a |solver| class, call
-:func:`~hklpy2.backends.base.get_solver`. This example
+:func:`~hklpy2.misc.get_solver`. This example
 selects the |libhkl| |solver| (using its entry point name: ``"hkl_soleil"``)::
 
     >>> from hklpy2 import get_solver
     >>> Solver = get_solver("hkl_soleil")
     >>> print(f"{Solver=}")
     Solver=<class 'hklpy2.backends.hkl_soleil.HklSolver'>
```

### Comparing `hklpy2-0.0.6/docs/source/api/lattice.rst` & `hklpy2-0.0.7/docs/source/api/lattice.rst`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/docs/source/api/reflection.rst` & `hklpy2-0.0.7/docs/source/api/reflection.rst`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/docs/source/conf.py` & `hklpy2-0.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/docs/source/index.rst` & `hklpy2-0.0.7/docs/source/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -11,34 +11,36 @@
 
 .. caution:: Development in progress.
 
 .. toctree::
    :glob:
    :hidden:
 
+   guide
    api
 
-.. TODO remove from comment
-    .. icons: https://fonts.google.com/icons
+.. icons: https://fonts.google.com/icons
 
-    .. grid:: 2
+.. grid:: 2
 
-        .. grid-item-card:: :material-outlined:`summarize;3em` User Guide
-        .. grid-item-card:: :material-regular:`install_desktop;3em` Installation
-        .. grid-item-card:: :material-regular:`subscriptions;3em` API
-        .. grid-item-card:: :material-regular:`history;3em` History of changes
+    .. grid-item-card:: :material-outlined:`summarize;3em` :ref:`user_guide`
+    .. grid-item-card:: :material-regular:`subscriptions;3em` :ref:`api`
+
+.. .. grid-item-card :: :material-regular:`install_desktop;3em` Installation
+.. .. grid-item-card:: :material-regular:`history;3em` History of changes
 
 .. _about:
 
 About
 -----
 
 :home: https://prjemian.github.io/hklpy2
 :source: https://github.com/prjemian/hklpy2
 :license: :ref:`license`
 :full version: |release|
 :published: |today|
 :index: :ref:`genindex`
 :modules: :ref:`modindex`
-:1st gen: |hklpy|
+:|hklpy|: |hklpy.url|
+:|libhkl|: https://people.debian.org/~picca/hkl/hkl.html
 :acknowledgement: "This product includes software produced by UChicago Argonne,
     LLC under Contract No. DE-AC02-06CH11357 with the Department of Energy."
```

### Comparing `hklpy2-0.0.6/hklpy2/__init__.py` & `hklpy2-0.0.7/hklpy2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,17 @@
     __version__ = version(__package_name__)
     del version
 
 class Hklpy2Error(Exception):
     """Any exception from the |hklpy2| package."""
 
 
-from .backends import SOLVER_ENTRYPOINT_GROUP  # noqa: E402, F401
 from .backends import SolverBase  # noqa: E402, F401
-from .backends import get_solver  # noqa: E402, F401
-from .backends import solvers  # noqa: E402, F401
 from .lattice import SI_LATTICE_PARAMETER  # noqa: E402, F401
 from .lattice import Lattice  # noqa: E402, F401
+from .misc import SOLVER_ENTRYPOINT_GROUP  # noqa: E402, F401
+from .misc import SolverError  # noqa: E402, F401
+from .misc import get_solver  # noqa: E402, F401
+from .misc import solvers  # noqa: E402, F401
 from .reflection import Reflection  # noqa: E402, F401
 from .reflection import ReflectionsDict  # noqa: E402, F401
 from .sample import Sample  # noqa: E402, F401
```

### Comparing `hklpy2-0.0.6/hklpy2/backends/base.py` & `hklpy2-0.0.7/hklpy2/backends/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,20 @@
 """
 Backend: abstract base class
 
 .. autosummary::
 
     ~SolverBase
-    ~SOLVER_ENTRYPOINT_GROUP
-    ~get_solver
-    ~solvers
 """
 
 from abc import ABC
 from abc import abstractmethod
 
 from .. import __version__
 
-SOLVER_ENTRYPOINT_GROUP = "hklpy2.solver"
-"""Name by which |hklpy2| backend |solver| classes are grouped."""
-
-
-def get_solver(solver_name):
-    """
-    Load a Solver class from a named entry point.
-
-    ::
-
-        import hklpy2
-        Solver = hklpy2.get_solver("hkl_soleil")
-    """
-    from importlib.metadata import entry_points
-
-    entries = entry_points(group=SOLVER_ENTRYPOINT_GROUP)
-    return entries[solver_name].load()
-
-
-def solvers():
-    """
-    Dictionary of available Solver classes, mapped by entry point name.
-
-    ::
-
-        import hklpy2
-        print(hklpy2.solvers())
-    """
-    from importlib.metadata import entry_points
-
-    # fmt: off
-    entries = {
-        ep.name: ep.value
-        for ep in entry_points(group=SOLVER_ENTRYPOINT_GROUP)
-    }
-    # fmt: on
-    return entries
-
 
 class SolverBase(ABC):
     """
     Base class for all |hklpy2| |solver| classes.
 
     ::
 
@@ -80,96 +39,133 @@
     .. autosummary::
 
         ~addReflection
         ~addSample
         ~calculateOrientation
         ~forward
         ~geometries
+        ~geometry
         ~inverse
+        ~lattice
+        ~mode
         ~modes
         ~pseudo_axis_names
         ~real_axis_names
         ~refineLattice
-        ~setGeometry
-        ~setLattice
-        ~setMode
     """
 
+    __name__ = "base"
+    """Name of this Solver."""
+
     __version__ = __version__
     """Version of this Solver."""
 
     def __init__(self) -> None:
-        self.gname = None
+        self.gname = None  # TODO: refactor to use self._geometry
+        self._geometry = None
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(name={self.__name__!r})"
 
     @abstractmethod
     def addReflection(self, pseudos, reals, wavelength):
         """Add information about a reflection."""
-        pass
 
     @abstractmethod
     def addSample(self, sample):
         """Add a sample."""
-        pass
 
     @abstractmethod
     def calculateOrientation(self, r1, r2):
         """Calculate the UB (orientation) matrix from two reflections."""
-        pass
 
     @abstractmethod
     def forward(self):
         """Compute list of solutions(reals) from pseudos (hkl -> [angles])."""
-        pass
+        # based on geometry and mode
+        return [{}]
 
     @property
     @abstractmethod
     def geometries(self):
         """Ordered list of the geometry names."""
-        pass
+        return []
 
+    @property
     @abstractmethod
-    def inverse(self):
+    def geometry(self):
+        """Selected diffractometer geometry."""
+        return self._geometry
+
+    @geometry.setter
+    @abstractmethod
+    def geometry(self, value):
+        if not isinstance(value, (type(None), str)):
+            raise TypeError(f"Must supply str, received {value!r}")
+        if value not in self.geometries:
+            raise KeyError(
+                f"Geometry {value} unknown. Pick one of: {self.geometries!r}"
+            )
+        self._geometry = value
+
+    @abstractmethod
+    def inverse(self, reals: dict):
         """Compute tuple of pseudos from reals (angles -> hkl)."""
-        pass
+
+    @property
+    def lattice(self):
+        """
+        Crystal lattice parameters.  (not used by this |solver|).
+        """
+        return self._lattice
+
+    @lattice.setter
+    def lattice(self, value):
+        from .. import Lattice
+
+        if not isinstance(value, Lattice):
+            raise TypeError(f"Must supply Lattice object, received {value!r}")
+        self._lattice = value
+
+    @property
+    def mode(self):
+        """
+        Diffractometer geometry operation mode for forward().
+
+        A mode defines which axes will be modified by the
+        :meth:`forward` computation.
+        """
+        try:
+            self._mode
+        except AttributeError:
+            self._mode = None
+        return self._mode
+
+    @mode.setter
+    def mode(self, value):
+        if not isinstance(value, (type(None), str)):
+            raise TypeError(f"Must supply str, received {value!r}")
+        if value not in self.modes:
+            raise KeyError(f"Mode {value} unknown. Pick one of: {self.modes!r}")
+        self._mode = value
 
     @property
     @abstractmethod
     def modes(self):
         """List of the geometry operating modes."""
-        pass
+        return []
 
     @property
     @abstractmethod
     def pseudo_axis_names(self):
         """Ordered list of the pseudo axis names (such as h, k, l)."""
-        pass
+        return []
 
     @property
     @abstractmethod
     def real_axis_names(self):
         """Ordered list of the real axis names (such as th, tth)."""
-        pass
+        return []
 
     @abstractmethod
     def refineLattice(self, reflections):
         """Refine the lattice parameters from a list of reflections."""
-        pass
-
-    @abstractmethod
-    def setGeometry(self, gname, **kwargs):
-        """Select one of the diffractometer geometries."""
-        pass
-
-    @abstractmethod
-    def setLattice(self, lattice):
-        """Define the sample's lattice parameters."""
-        pass
-
-    @abstractmethod
-    def setMode(self, mode):
-        """
-        Define the geometry's operating mode.
-
-        A mode defines constraints on the solutions provided by the
-        :meth:`forward` computation.
-        """
-        pass
```

### Comparing `hklpy2-0.0.6/hklpy2/backends/hkl_soleil.py` & `hklpy2-0.0.7/hklpy2/backends/hkl_soleil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
 Backend: Hkl (``"hkl_soleil"``)
 
+Example::
+
+    import hklpy2
+    SolverClass = hklpy2.get_solver("hkl_soleil")
+    libhkl_solver = SolverClass()
+
 .. autosummary::
 
     ~HklSolver
 """
 
 import gi
 
 gi.require_version("Hkl", "5.0")
 
-from gi.repository import GLib  # noqa: E402, F401
+from gi.repository import GLib  # noqa: E402, F401, W0611
 from gi.repository import Hkl as libhkl  # noqa: E402
 
 from .base import SolverBase  # noqa: E402
 
 
 class HklSolver(SolverBase):
     """
@@ -26,63 +32,111 @@
     .. autosummary::
 
         ~addReflection
         ~addSample
         ~calculateOrientation
         ~forward
         ~geometries
+        ~geometry
         ~inverse
+        ~lattice
         ~modes
         ~pseudo_axis_names
         ~real_axis_names
         ~refineLattice
-        ~setGeometry
-        ~setLattice
-        ~setMode
     """
 
+    __name__ = "hkl_soleil"
     __version__ = libhkl.VERSION
 
     def __init__(self) -> None:
+        super().__init__()
         self.gname = None
 
         self.detector = libhkl.Detector.factory_new(libhkl.DetectorType(0))
         self._engine = None
         self._engines = None
-        self._factories = libhkl.factories()
+        self._factory = None
         self._geometry = None
         self.user_units = libhkl.UnitEnum.USER
 
-    def addReflection(self, pseudos, reals, wavelength):
+    def addReflection(self, pseudos, reals, wavelength):  # TODO
         """Add information about a reflection."""
-        pass  # TODO
 
-    def addSample(self, sample):
+    def addSample(self, sample):  # TODO
         """Add a sample."""
-        pass  # TODO
 
-    def calculateOrientation(self, r1, r2):
+    def calculateOrientation(self, r1, r2):  # TODO
         """Calculate the UB (orientation) matrix from two reflections."""
-        pass  # TODO
 
     def forward(self):
         """Compute list of solutions(reals) from pseudos (hkl -> [angles])."""
-        return []  # TODO
+        return [{}]
 
     @property
     def geometries(self):
-        geometries = [
-            f"{factory.name_get()}, {engine.name_get()}"
-            # f"{factory.name_get()}"
-            for factory in (self._factories or {}).values()
-            for engine in (self._engines or {}).engines_get()
-        ]
+        """
+        Ordered list of the geometry names.
+
+        .. sidebar:: compare with E4CV
+
+            TODO: confirm with the |libhkl| docs
+
+            .. seealso::
+
+                * `E4CV <https://blueskyproject.io/hklpy/geometry_tables.html#geometry-e4cv>`_
+                * `Hkl <https://people.debian.org/~picca/hkl/hkl.html>`_
+
+        For |libhkl|, each geometry may have zero or more computational
+        *engines*. Each engine has its own set of pseudos and reals.  Some of
+        the engines have additional (optional) axes.
+
+        So the geometry *names* include both the geometry and its computational
+        engine, such as `"E4CV, hkl"`.
+
+        """
+        geometries = []
+        for fname, factory in libhkl.factories().items():
+            # Underlying library raises error for the merged call:
+            #   factory.create_new_engine_list().engines_get()
+            # MUST do this in two parts here (and elsewhere).
+            engines = factory.create_new_engine_list()
+            for engine in engines.engines_get():
+                # "geometry, engine"
+                geometries.append(f"{fname}, {engine.name_get()}")
         return sorted(set(geometries))
 
-    def inverse(self):
+    @property
+    def geometry(self):
+        """
+        Diffractometer geometry and engine, such as `"E4CV, hkl"`.
+
+        To select (set) which combination of geometry and computational
+        engine, specify both such as::
+
+            solver.geometry = "E4CV, hkl"
+        """
+        return self._geometry
+
+    @geometry.setter
+    def geometry(self, value):
+        if not isinstance(value, (type(None), str)):
+            raise TypeError(f"Must supply str, received {value!r}")
+        if value not in self.geometries:
+            raise KeyError(f"Geometry {value} unknown.")
+
+        gname, engine = [s.strip() for s in value.split(",")]
+        self._factory = libhkl.factories()[gname]
+        self.gname = gname
+        self._geometry = self._factory.create_new_geometry()
+        self._engines = self._factory.create_new_engine_list()
+        self._engine = self._engines.engine_get_by_name(engine)
+        return self._geometry
+
+    def inverse(self, reals: dict):
         """Compute tuple of pseudos from reals (angles -> hkl)."""
         return tuple()  # TODO
 
     @property
     def modes(self):
         """List of the geometry operating modes."""
         return []  # TODO
@@ -99,27 +153,10 @@
         if self._geometry is not None:
             return self._geometry.axis_names_get()
 
     def refineLattice(self, reflections):
         """Refine the lattice parameters from a list of reflections."""
         pass  # TODO
 
-    def setGeometry(self, gname, engine="hkl"):
-        factory = self._factories[gname]
-        self.gname = gname
-        self._geometry = factory.create_new_geometry()
-        self._engines = factory.create_new_engine_list()
-        self._engine = self._engines.engine_get_by_name(engine)
-        return self._geometry
-
     def setLattice(self, lattice):
         """Define the sample's lattice parameters."""
         pass  # TODO
-
-    def setMode(self, mode):
-        """
-        Define the geometry's operating mode.
-
-        A mode defines constraints on the solutions provided by the
-        :meth:`forward` computation.
-        """
-        pass  # TODO
```

### Comparing `hklpy2-0.0.6/hklpy2/backends/no_op.py` & `hklpy2-0.0.7/hklpy2/backends/no_op.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 """
-Backend: no_op
+Backend: no_op (``"no_op"``)
 
 no reciprocal-space conversions
 
+Example::
+
+    import hklpy2
+    SolverClass = hklpy2.get_solver("no_op")
+    noop_solver = SolverClass()
+
 .. autosummary::
 
     ~NoOpSolver
 """
 
 from .. import __version__
 from .base import SolverBase
@@ -21,48 +27,63 @@
     .. autosummary::
 
         ~addReflection
         ~addSample
         ~calculateOrientation
         ~forward
         ~geometries
+        ~geometry
         ~inverse
+        ~lattice
+        ~mode
         ~modes
         ~pseudo_axis_names
         ~real_axis_names
         ~refineLattice
-        ~setGeometry
-        ~setLattice
-        ~setMode
     """
 
+    __name__ = "no_op"
     __version__ = __version__
 
     def __init__(self) -> None:
+        super().__init__()
         self.gname = None
         self._geometry = None
 
     def addReflection(self, pseudos, reals, wavelength):
         pass  # TODO
 
     def addSample(self, sample):
         pass  # TODO
 
     def calculateOrientation(self, r1, r2):
         return
 
     def forward(self):
-        return []
+        return [{}]
 
     @property
     def geometries(self):
         return []
 
-    def inverse(self):
-        return ["No Ops"]
+    @property
+    def geometry(self):
+        """Diffractometer geometry."""
+        return self._geometry
+
+    @geometry.setter
+    def geometry(self, value):
+        if not isinstance(value, (type(None), str)):
+            raise TypeError(f"Must supply str, received {value!r}")
+        self._geometry = value  # TODO: Why?
+        self.gname = value
+        return self.gname
+
+    def inverse(self, reals: dict):
+        return {}
 
     @property
     def modes(self):
         return []
 
     @property
     def pseudo_axis_names(self):
@@ -71,16 +92,9 @@
     @property
     def real_axis_names(self):
         return []  # no axes
 
     def refineLattice(self, reflections):
         return None
 
-    def setGeometry(self, gname, **kwargs):
-        self.gname = gname
-        return None
-
     def setLattice(self, lattice):
         pass  # TODO
-
-    def setMode(self, mode):
-        pass
```

### Comparing `hklpy2-0.0.6/hklpy2/backends/tests/test_hkl_soleil.py` & `hklpy2-0.0.7/hklpy2/backends/tests/test_hkl_soleil.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,11 @@
     assert p_axes == "h k l".split(), f"{p_axes=}"
 
 
 def test_geometries():
     solver = hkl_soleil.HklSolver()
     assert solver is not None
 
-    solver.setGeometry("E4CV")
-
     glist = solver.geometries
     assert len(glist) >= 18
-    for gname in "E4CV E4CH E6C K4CV K6C ZAXIS TwoC".split():
+    for gname in "E4CV E4CH E6C K4CV K6C ZAXIS".split():
         assert f"{gname}, hkl" in glist, f"{gname=}  {glist=}"
-    # assert glist == [], f"{glist=}"
```

### Comparing `hklpy2-0.0.6/hklpy2/lattice.py` & `hklpy2-0.0.7/hklpy2/lattice.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
         ~equal
         ~_asdict
         ~__eq__
         ~__repr__
     """
 
+    digits = 4
+
     def __init__(
         self,
         a: float,
         b: float = None,
         c: float = None,
         alpha: float = 90.0,  # degrees
         beta: float = None,  # degrees
@@ -105,9 +107,9 @@
         """
         return self.equal(self, latt)
 
     def __repr__(self):
         """
         Standard representation of lattice.
         """
-        parameters = [f"{k}={v}" for k, v in self._asdict().items()]
+        parameters = [f"{k}={round(v, self.digits)}" for k, v in self._asdict().items()]
         return "Lattice(" + ", ".join(parameters) + ")"
```

### Comparing `hklpy2-0.0.6/hklpy2/reflection.py` & `hklpy2-0.0.7/hklpy2/reflection.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,43 +39,45 @@
         self, solver, pseudos: dict, angles: dict, wavelength: float, name=None
     ) -> None:
         self.name = name or unique_name()
         self.solver = solver
         self.pseudos = pseudos
         self.angles = angles
         self.wavelength = wavelength
+        # TODO: what about optional items (azimuth, h1, h2, zones, ...)
 
     def _asdict(self):
         """Describe the reflection as a dictionary."""
         return {
             "name": repr(self.name),
+            "geometry": repr(self.solver.gname),
             "pseudos": self.pseudos,
             "angles": self.angles,
             "wavelength": self.wavelength,
-            "geometry": repr(self.solver.gname),
         }
 
     def __repr__(self):
         """
         Standard representation of reflection.
         """
         parameters = [f"{k}={v}" for k, v in self._asdict().items()]
         return "Reflection(" + ", ".join(parameters) + ")"
 
     # --------- get/set properties
 
     @property
-    def angles(self):
+    def angles(self):  # TODO: rename as reals?
         """Ordered dictionary of diffractometer's real-space axes."""
         return self._angles
 
     @angles.setter
     def angles(self, value):
         if not isinstance(value, dict):
             raise TypeError(f"Must supply dict, received angles={value!r}")
+        # TODO: validate against self.solver.real_axis_names
         self._angles = value
 
     @property
     def name(self):
         """Sample name."""
         return self._name
 
@@ -90,24 +92,25 @@
         """Ordered dictionary of diffractometer's reciprocal-space axes."""
         return self._pseudos
 
     @pseudos.setter
     def pseudos(self, value):
         if not isinstance(value, dict):
             raise TypeError(f"Must supply dict, received pseudos={value!r}")
+        # TODO: validate against self.solver.pseudo_axis_names
         self._pseudos = value
 
     @property
     def solver(self):
         """Diffractometer |solver|."""
         return self._solver
 
     @solver.setter
     def solver(self, value):
-        if not isinstance(value, SolverBase):
+        if not (isinstance(value, SolverBase) or issubclass(type(value), SolverBase)):
             raise TypeError(
                 f"Must supply SolverBase() object, received solver={value!r}"
             )
         # note: calling SolverBase() will always generate a TypeError
         # "Can't instantiate abstract class SolverBase with abstract methods" ...
         self._solver = value
 
@@ -128,29 +131,41 @@
 class ReflectionsDict(dict):
     """
     Dictionary of Reflections.
 
     .. autosummary::
 
         ~ordering
+        ~setor
         ~set_orientation_reflections
-        ~set_or
         ~swap
     """
 
     ordering = []  # TODO: use get/set property?
     """List of ordering reflection names."""
 
-    def set_orientation_reflections(self, r1: Reflection, r2: Reflection):
-        """Designate r1 & r2 as the two named reflections."""
-        self.ordering = [r1.name, r2.name]
+    def set_orientation_reflections(self, reflections: [Reflection]) -> None:
+        """Designate the order of the reflections to be used."""
+        self.ordering = [r.name for r in reflections]
 
-    set_or = set_orientation_reflections
+    setor = set_orientation_reflections
     """Common alias for :meth:`~set_orientation_reflections`."""
 
+    def add(self, reflection: Reflection, overwrite: bool = False):
+        """Add an orientation reflection."""
+        if reflection.name in self and not overwrite:
+            raise ReflectionError(
+                f"Reflection {reflection.name!r} already defined. "
+                "Set `overwrite=True` to replace it."
+            )
+        self[reflection.name] = reflection
+        if reflection.name not in self.ordering:
+            self.ordering.append(reflection.name)
+        # TODO: remove any reflections from ordering that no longer exist
+
     def swap(self):
         """Swap the two named orientation reflections."""
         if len(self.ordering) < 2:
             raise ReflectionError("Need at least two reflections to swap.")
         rname1, rname2 = self.ordering[:2]
         self.ordering[0] = rname2
         self.ordering[1] = rname1
```

### Comparing `hklpy2-0.0.6/hklpy2/sample.py` & `hklpy2-0.0.7/hklpy2/sample.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,29 +34,33 @@
         ~UB
     """
 
     def __init__(self, solver: SolverBase, lattice: Lattice, name: str = None) -> None:
         self.name = name or unique_name()
         self.solver = solver
         self.lattice = lattice
+        # TODO: reciprocal_lattice
         self.reflections = ReflectionsDict()
 
+    def __repr__(self):
+        return f"Sample(name={self.name!r}, lattice={self.lattice!r})"
+
     @property
     def U(self):
         """Return the matrix, U, crystal orientation on the diffractometer."""
         return None  # TODO
 
     @property
     def UB(self):
         """
         Return the crystal orientation matrix, UB.
 
         * :math:`UB` - orientation matrix
         * :math:`B` - crystal lattice on the diffractometer
-        * :math:`U` - rotation matrix, crystal orientation on diffractometer
+        * :math:`U` - rotation matrix, relative orientation of crystal on diffractometer
         """
         # self.solver.calculateOrientation()  # TODO
 
     def refine_lattice(self):
         """Refine the lattice parameters from 3 or more reflections."""
         if len(self.self.reflections) < 3:
             raise SampleError("Need 3 or more reflections to refine lattice.")
@@ -101,12 +105,12 @@
     @property
     def solver(self):
         """Diffractometer |solver|."""
         return self._solver
 
     @solver.setter
     def solver(self, value):
-        if not isinstance(value, SolverBase):
+        if not (isinstance(value, SolverBase) or issubclass(type(value), SolverBase)):
             raise TypeError(f"Must supply SolverBase() object, received {value!r}")
         # note: calling SolverBase() will always generate a TypeError
         # "Can't instantiate abstract class SolverBase with abstract methods" ...
         self._solver = value
```

### Comparing `hklpy2-0.0.6/hklpy2/tests/test_lattice.py` & `hklpy2-0.0.7/hklpy2/tests/test_lattice.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/hklpy2/tests/test_reflection.py` & `hklpy2-0.0.7/hklpy2/tests/test_reflection.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 def test_reflection_no_op():
     """Test with the NoOpSolver"""
     from ..backends.no_op import NoOpSolver
 
     solver = NoOpSolver()
     assert solver is not None
 
-    g = solver.setGeometry("No geometry")
-    assert g is None  # NoOpSolver always returns None for geometry
+    gname = "test geometry"
+    solver.geometry = gname
+    assert solver.gname == gname, f"{solver.gname=!r}"
 
     ref1 = Reflection(solver, {}, {}, 1.0, name="r1")
     assert ref1 is not None
     assert ref1.name == "r1"
     expected = (
-        "Reflection(name='r1', pseudos={}, angles={}, "
-        "wavelength=1.0, geometry='No geometry')"
+        f"Reflection(name='r1', geometry={gname!r}, "
+        "pseudos={}, angles={}, wavelength=1.0)"
     )
     assert str(ref1) == expected, f"{ref1}"
 
     ref2 = Reflection(solver, {}, {}, 1.01)
     assert ref2 is not None
     assert ref2.name != "r2"
     assert len(ref2.name) == len(unique_name())
@@ -39,25 +40,27 @@
 def test_reflection_hkl_soleil():
     """Test with the HklSolver"""
     from ..backends.hkl_soleil import HklSolver
 
     solver = HklSolver()
     assert solver is not None
 
-    g = solver.setGeometry("E4CV", "hkl")
-    assert g is not None
+    gname = "E4CV"
+    solver.geometry = f"{gname}, hkl"
+    assert solver.gname == gname, f"{solver.gname=!r}"
 
     reals = dict(omega=10, chi=0, phi=0, tth=20)
     pseudos = dict(h=1, k=0, l=0)
     ref1 = Reflection(solver, pseudos, reals, 1.0, name="r1")
     assert ref1.name == "r1"
     expected = (
-        "Reflection(name='r1', pseudos={'h': 1, 'k': 0, 'l': 0}, "
+        f"Reflection(name='r1', geometry={gname!r}, "
+        "pseudos={'h': 1, 'k': 0, 'l': 0}, "
         "angles={'omega': 10, 'chi': 0, 'phi': 0, 'tth': 20}, "
-        "wavelength=1.0, geometry='E4CV')"
+        "wavelength=1.0)"
     )
     assert str(ref1) == expected, f"{ref1}"
 
 
 def test_with_solver_base():
     """Special case that does not fit constructor test."""
     reason = "Can't instantiate abstract class SolverBase"
@@ -149,15 +152,15 @@
     [[does_not_raise(), None]],
 )
 def test_reflectionsdict_constructor(outcome, reason):
     with outcome as excuse:
         rdict = ReflectionsDict()
         assert rdict is not None
         assert rdict.ordering == []
-        assert rdict.set_or == rdict.set_orientation_reflections
+        assert rdict.setor == rdict.set_orientation_reflections
 
     if reason is not None:
         assert reason in str(excuse.value), f"{excuse=}"
 
 
 def test_reflectionsdict_swap():
     rdict = ReflectionsDict()
```

### Comparing `hklpy2-0.0.6/hklpy2/tests/test_sample.py` & `hklpy2-0.0.7/hklpy2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.6/hklpy2/tests/test_solver.py` & `hklpy2-0.0.7/hklpy2/tests/test_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 
 import pytest
 
-from ..backends import get_solver
+from .. import get_solver
 
 
 @pytest.mark.parametrize("solver_name", ["hkl_soleil", "no_op"])
 def test_solvers(solver_name):
     from importlib.metadata import entry_points
 
     solvers = entry_points(group="hklpy2.solver")
@@ -29,15 +29,15 @@
     assert Solver is not None
 
     solver = Solver()
     assert solver is not None
     assert isinstance(solver.__version__, str)
 
     gname = "ESRF ID01 PSIC"
-    solver.setGeometry(gname)
+    solver.geometry = f"{gname}, hkl"
     assert solver._geometry is not None
     assert solver.gname == gname
     assert solver._geometry.name_get() == gname
 
     reals = solver.real_axis_names
     assert reals == "mu eta phi nu delta".split()
```

### Comparing `hklpy2-0.0.6/hklpy2.egg-info/PKG-INFO` & `hklpy2-0.0.7/hklpy2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hklpy2
-Version: 0.0.6
+Version: 0.0.7
 Summary: 2nd generation diffractometer controls for the Bluesky Framework.
 Author-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 Maintainer-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 License: Copyright (c) 2023-2024, UChicago Argonne, LLC
         
         All Rights Reserved
         
@@ -92,13 +92,13 @@
 
 NOTE:  this project at initial development
 
 | Name | Downloads | Version | Platforms | PyPI | Coverage |
 | --- | --- | --- | --- | --- | --- |
 | [![Conda Package](https://img.shields.io/badge/package-hklpy2-green.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![PyPi](https://img.shields.io/pypi/v/hklpy2.svg)](https://pypi.python.org/pypi/hklpy2) | [![Coverage Status](https://coveralls.io/repos/github/prjemian/hklpy2/badge.svg?branch=main)](https://coveralls.io/github/prjemian/hklpy2?branch=main) |
 
-Controls for using diffractometers within the [Bluesky
+2nd generation controls for using diffractometers within the [Bluesky
 Framework](https://blueskyproject.io).
 
 ## References
 
 - hklpy2 documentation: <https://prjemian.github.io/hklpy2>
```

### Comparing `hklpy2-0.0.6/hklpy2.egg-info/SOURCES.txt` & `hklpy2-0.0.7/hklpy2.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 .github/workflows/docs.yml
 .github/workflows/pypi.yml
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/api.rst
 docs/source/conf.py
+docs/source/guide.rst
 docs/source/index.rst
 docs/source/license.rst
 docs/source/substitutions.txt
 docs/source/api/backends.rst
 docs/source/api/lattice.rst
 docs/source/api/reflection.rst
 docs/source/api/sample.rst
 docs/source/api/z_misc.rst
 docs/source/api/backends/base.rst
 docs/source/api/backends/hkl_soleil.rst
 docs/source/api/backends/no_op.rst
+docs/source/api/backends/th_tth_q.rst
+docs/source/notebooks/demo.ipynb
 hklpy2/__init__.py
 hklpy2/lattice.py
 hklpy2/misc.py
 hklpy2/notes.md
 hklpy2/reflection.py
 hklpy2/sample.py
 hklpy2.egg-info/PKG-INFO
@@ -36,14 +39,18 @@
 hklpy2.egg-info/entry_points.txt
 hklpy2.egg-info/requires.txt
 hklpy2.egg-info/top_level.txt
 hklpy2/backends/__init__.py
 hklpy2/backends/base.py
 hklpy2/backends/hkl_soleil.py
 hklpy2/backends/no_op.py
+hklpy2/backends/th_tth_q.py
 hklpy2/backends/tests/__init__.py
 hklpy2/backends/tests/test_hkl_soleil.py
+hklpy2/backends/tests/test_th_tth_q.py
 hklpy2/tests/__init__.py
+hklpy2/tests/test_backends.py
+hklpy2/tests/test_demo_notebook.py
 hklpy2/tests/test_lattice.py
 hklpy2/tests/test_reflection.py
 hklpy2/tests/test_sample.py
 hklpy2/tests/test_solver.py
```

### Comparing `hklpy2-0.0.6/pyproject.toml` & `hklpy2-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
   "ophyd",
   "pint",
 ]
 
 [project.entry-points."hklpy2.solver"]
 no_op = "hklpy2.backends.no_op:NoOpSolver"
 hkl_soleil = "hklpy2.backends.hkl_soleil:HklSolver"
+th_tth = "hklpy2.backends.th_tth_q:ThTthSolver"
 
 [project.optional-dependencies]
 hkl_soleil = [
   "pygobject",
 ]
 tests = [
   "packaging",
```

