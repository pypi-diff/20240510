# Comparing `tmp/autoray-0.6.8.tar.gz` & `tmp/autoray-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoray-0.6.8.tar", last modified: Mon Jan 29 17:46:12 2024, max compression
+gzip compressed data, was "autoray-0.6.9.tar", last modified: Sat Mar  9 07:46:59 2024, max compression
```

## Comparing `autoray-0.6.8.tar` & `autoray-0.6.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.269365 autoray-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-29 17:45:58.000000 autoray-0.6.8/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-29 17:45:58.000000 autoray-0.6.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.253365 autoray-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.257365 autoray-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-01-29 17:45:58.000000 autoray-0.6.8/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-29 17:45:58.000000 autoray-0.6.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-01-29 17:45:58.000000 autoray-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-29 17:45:58.000000 autoray-0.6.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-01-29 17:45:58.000000 autoray-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-29 17:45:58.000000 autoray-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-01-29 17:46:12.269365 autoray-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-01-29 17:45:58.000000 autoray-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.257365 autoray-0.6.8/autoray/
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-29 17:46:12.000000 autoray-0.6.8/autoray/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    60413 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/autoray.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.261365 autoray-0.6.8/autoray/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/experimental/complexity_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)  1265159 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/experimental/complexity_tracing_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.261365 autoray-0.6.8/autoray/lazy/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50441 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/lazy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/lazy/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-01-29 17:45:58.000000 autoray-0.6.8/autoray/lazy/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.269365 autoray-0.6.8/autoray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-01-29 17:46:12.000000 autoray-0.6.8/autoray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-29 17:46:12.000000 autoray-0.6.8/autoray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 17:46:12.000000 autoray-0.6.8/autoray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-29 17:46:12.000000 autoray-0.6.8/autoray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-29 17:46:12.000000 autoray-0.6.8/autoray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.253365 autoray-0.6.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.261365 autoray-0.6.8/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-29 17:45:58.000000 autoray-0.6.8/ci/requirements/py-base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-29 17:45:58.000000 autoray-0.6.8/ci/requirements/py-jax.yml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-29 17:45:58.000000 autoray-0.6.8/ci/requirements/py-tensorflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-29 17:45:58.000000 autoray-0.6.8/ci/requirements/py-torch.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.265365 autoray-0.6.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.265365 autoray-0.6.8/docs/_pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/_pygments/_pygments_dark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/_pygments/_pygments_light.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.265365 autoray-0.6.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    26562 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/_static/autoray-header.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/_static/autoray.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/_static/my-styles.css
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/automatic_dispatch.md
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/compilation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.265365 autoray-0.6.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    57965 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/images/autoray-readme-pic-0.png
--rw-r--r--   0 runner    (1001) docker     (127)    99582 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/images/autoray-readme-pic-1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)   782774 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/lazy_computation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-29 17:45:58.000000 autoray-0.6.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-29 17:45:58.000000 autoray-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 17:46:12.269365 autoray-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-01-29 17:45:58.000000 autoray-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:46:12.269365 autoray-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 17:45:58.000000 autoray-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-01-29 17:45:58.000000 autoray-0.6.8/tests/test_autocompile.py
--rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-01-29 17:45:58.000000 autoray-0.6.8/tests/test_autoray.py
--rw-r--r--   0 runner    (1001) docker     (127)    21396 2024-01-29 17:45:58.000000 autoray-0.6.8/tests/test_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.137127 autoray-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-09 07:46:48.000000 autoray-0.6.9/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-09 07:46:48.000000 autoray-0.6.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.121127 autoray-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.125127 autoray-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-09 07:46:48.000000 autoray-0.6.9/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-09 07:46:48.000000 autoray-0.6.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-09 07:46:48.000000 autoray-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-09 07:46:48.000000 autoray-0.6.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-03-09 07:46:48.000000 autoray-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-09 07:46:48.000000 autoray-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-03-09 07:46:59.137127 autoray-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-09 07:46:48.000000 autoray-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.125127 autoray-0.6.9/autoray/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 07:46:59.000000 autoray-0.6.9/autoray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60491 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/autoray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.129127 autoray-0.6.9/autoray/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/experimental/complexity_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1265159 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/experimental/complexity_tracing_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.129127 autoray-0.6.9/autoray/lazy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50441 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/lazy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/lazy/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-09 07:46:48.000000 autoray-0.6.9/autoray/lazy/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.137127 autoray-0.6.9/autoray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-03-09 07:46:59.000000 autoray-0.6.9/autoray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-09 07:46:59.000000 autoray-0.6.9/autoray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 07:46:59.000000 autoray-0.6.9/autoray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-09 07:46:59.000000 autoray-0.6.9/autoray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-09 07:46:59.000000 autoray-0.6.9/autoray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.121127 autoray-0.6.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.133127 autoray-0.6.9/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-09 07:46:48.000000 autoray-0.6.9/ci/requirements/py-base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-09 07:46:48.000000 autoray-0.6.9/ci/requirements/py-jax.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-09 07:46:48.000000 autoray-0.6.9/ci/requirements/py-tensorflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-09 07:46:48.000000 autoray-0.6.9/ci/requirements/py-torch.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.133127 autoray-0.6.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.133127 autoray-0.6.9/docs/_pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/_pygments/_pygments_dark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/_pygments/_pygments_light.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.133127 autoray-0.6.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    26562 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/_static/autoray-header.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/_static/autoray.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/_static/my-styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/automatic_dispatch.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/compilation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.137127 autoray-0.6.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    57965 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/images/autoray-readme-pic-0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    99582 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/images/autoray-readme-pic-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)   782774 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/lazy_computation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-09 07:46:48.000000 autoray-0.6.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-09 07:46:48.000000 autoray-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 07:46:59.137127 autoray-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-09 07:46:48.000000 autoray-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:59.137127 autoray-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:46:48.000000 autoray-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-09 07:46:48.000000 autoray-0.6.9/tests/test_autocompile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23417 2024-03-09 07:46:48.000000 autoray-0.6.9/tests/test_autoray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21396 2024-03-09 07:46:48.000000 autoray-0.6.9/tests/test_lazy.py
```

### Comparing `autoray-0.6.8/.github/workflows/pypi-release.yml` & `autoray-0.6.9/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/.github/workflows/tests.yml` & `autoray-0.6.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/.gitignore` & `autoray-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/LICENSE` & `autoray-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/PKG-INFO` & `autoray-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoray
-Version: 0.6.8
+Version: 0.6.9
 Summary: Abstract your array operations.
 Home-page: http://github.com/jcmgray/autoray
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/autoray/issues
 Project-URL: Source, https://github.com/jcmgray/autoray/
```

### Comparing `autoray-0.6.8/README.md` & `autoray-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray/__init__.py` & `autoray-0.6.9/autoray/__init__.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray/autoray.py` & `autoray-0.6.9/autoray/autoray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1990,25 +1990,27 @@
 _FUNCS["torch", "astype"] = torch_astype
 _FUNCS["torch", "to_numpy"] = torch_to_numpy
 _FUNCS["torch", "complex"] = complex_add_re_im
 _FUNCS["torch", "transpose"] = torch_transpose
 _FUNCS["torch", "count_nonzero"] = torch_count_nonzero
 _FUNCS["torch", "get_dtype_name"] = torch_get_dtype_name
 
-_FUNC_ALIASES["torch", "clip"] = "clamp"
-_FUNC_ALIASES["torch", "power"] = "pow"
 _FUNC_ALIASES["torch", "array"] = "tensor"
+_FUNC_ALIASES["torch", "clip"] = "clamp"
 _FUNC_ALIASES["torch", "concatenate"] = "cat"
+_FUNC_ALIASES["torch", "conjugate"] = "conj"
+_FUNC_ALIASES["torch", "expand_dims"] = "unsqueeze"
+_FUNC_ALIASES["torch", "linalg.expm"] = "matrix_exp"
+_FUNC_ALIASES["torch", "max"] = "amax"
+_FUNC_ALIASES["torch", "min"] = "amin"
+_FUNC_ALIASES["torch", "power"] = "pow"
 _FUNC_ALIASES["torch", "random.normal"] = "randn"
 _FUNC_ALIASES["torch", "random.uniform"] = "rand"
-_FUNC_ALIASES["torch", "take"] = "index_select"
-_FUNC_ALIASES["torch", "linalg.expm"] = "matrix_exp"
-_FUNC_ALIASES["torch", "conjugate"] = "conj"
 _FUNC_ALIASES["torch", "split"] = "tensor_split"
-_FUNC_ALIASES["torch", "expand_dims"] = "unsqueeze"
+_FUNC_ALIASES["torch", "take"] = "index_select"
 
 _SUBMODULE_ALIASES["torch", "linalg.expm"] = "torch"
 _SUBMODULE_ALIASES["torch", "random.normal"] = "torch"
 _SUBMODULE_ALIASES["torch", "random.uniform"] = "torch"
 
 _CUSTOM_WRAPPERS["torch", "linalg.svd"] = svd_not_full_matrices_wrapper
 _CUSTOM_WRAPPERS["torch", "random.normal"] = scale_random_normal_manually
```

### Comparing `autoray-0.6.8/autoray/compiler.py` & `autoray-0.6.9/autoray/compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import functools
 
 from .autoray import (
     do,
     infer_backend,
     backend_like,
     tree_map,
-    tree_apply,
     tree_iter,
+    tree_flatten,
+    tree_unflatten,
     is_array,
 )
 from . import lazy
 
 
 class CompilePython:
     """A simple compiler that unravels all autoray calls, optionally sharing
     intermediates and folding constants, converts this to a code object using
-    ``compile``, then executes this using ``exec``. Non-array function
-    arguments are treated as static, with a new function compiled for each
-    unique hash of their values.
+    ``compile``, then executes this using ``exec``.
 
     Parameters
     ----------
     fn : callable
         Function to compile - should have signature
         ``fn(*args, **kwargs) -> array``, with ``args`` and ``kwargs`` any
         nested combination of ``tuple``, ``list`` and ``dict`` objects
@@ -35,59 +34,39 @@
         shared intermediate results can be identified.
     """
 
     def __init__(self, fn, fold_constants=True, share_intermediates=True):
         self._fn = fn
         self._fold_constants = fold_constants
         self._share_intermediates = share_intermediates
-        self._fns = {}
+        self._jit_fn = None
 
-    def _trace_fn(self, *args, **kwargs):
+    def setup(self, args, kwargs):
         """Convert the example arrays to lazy variables and trace them through
         the function.
         """
-        variables = []
-
-        def _collect_variable(x):
-            lx = lazy.array(x)
-            variables.append(lx)
-            return lx
-
-        def _run_lazy():
-            lz_args, lz_kwargs = tree_map(
-                _collect_variable, (args, kwargs), is_array
-            )
-            return self._fn(*lz_args, **lz_kwargs)
+        variables = tree_map(lazy.array, (args, kwargs))
 
         if self._share_intermediates:
             with backend_like("autoray.lazy"), lazy.shared_intermediates():
-                outs = _run_lazy()
+                outs = self._fn(*variables[0], **variables[1])
         else:
             with backend_like("autoray.lazy"):
-                outs = _run_lazy()
+                outs = self._fn(*variables[0], **variables[1])
 
         return lazy.Function(
             variables, outs, fold_constants=self._fold_constants
         )
 
     def __call__(self, *args, array_backend=None, **kwargs):
         """If necessary, build, then call the compiled function."""
-        # separate variable arrays from constant kwargs
-        arrays = []
-        constants = []
-        tree_apply(
-            lambda x: (arrays if is_array(x) else constants).append(x),
-            (args, kwargs),
-        )
-        key = hash(tuple(constants))
-        try:
-            return self._fns[key](arrays)
-        except KeyError:
-            fn = self._fns[key] = self._trace_fn(*args, **kwargs)
-            return fn(arrays)
+        if self._jit_fn is None:
+            self._jit_fn = self.setup(args, kwargs)
+
+        return self._jit_fn(args, kwargs)
 
 
 class CompileJax:
     """ """
 
     def __init__(self, fn, enable_x64=None, platform_name=None, **kwargs):
         self._fn = fn
@@ -96,30 +75,30 @@
         self._jit_fn = None
         self._jit_kwargs = kwargs
 
     def setup(self):
         import jax
 
         if self._enable_x64 is not None:
-            from jax.config import config
+            import jax
 
-            config.update("jax_enable_x64", self._enable_x64)
+            jax.config.update("jax_enable_x64", self._enable_x64)
 
         if self._platform_name is not None:
-            from jax.config import config
+            import jax
 
-            config.update("jax_platform_name", self._platform_name)
+            jax.config.update("jax_platform_name", self._platform_name)
 
         self._jit_fn = jax.jit(self._fn, **self._jit_kwargs)
         self._fn = None
 
     def __call__(self, *args, array_backend=None, **kwargs):
         if self._jit_fn is None:
             self.setup()
-        out = self._jit_fn(*args, *kwargs)
+        out = self._jit_fn(*args, **kwargs)
         if array_backend != "jax":
             out = do("asarray", out, like=array_backend)
         return out
 
 
 class CompileTensorFlow:
     """ """
@@ -155,27 +134,35 @@
 
         if not hasattr(fn, "__name__") and isinstance(fn, functools.partial):
             # torch jit.trace requires fn.__name__ and others
             functools.update_wrapper(fn, fn.func)
 
         self._fn = fn
         self._jit_fn = None
+        kwargs.setdefault("check_trace", False)
         self._jit_kwargs = kwargs
 
-    def setup(self, args):
-        self._jit_fn = self.torch.jit.trace(self._fn, args, **self._jit_kwargs)
-        self._fn = None
+    def setup(self, *args, **kwargs):
+        flat_tensors, ref_tree = tree_flatten((args, kwargs), get_ref=True)
+
+        def flat_fn(flat_tensors):
+            args, kwargs = tree_unflatten(flat_tensors, ref_tree)
+            return self._fn(*args, **kwargs)
+
+        self._jit_fn = self.torch.jit.trace(
+            flat_fn, [flat_tensors], **self._jit_kwargs
+        )
 
     def __call__(self, *args, array_backend=None, **kwargs):
         if array_backend != "torch":
             # torch doesn't handle numpy arrays itself
             args = tree_map(self.torch.as_tensor, args, is_array)
         if self._jit_fn is None:
-            self.setup(args)
-        out = self._jit_fn(*args, **kwargs)
+            self.setup(*args, **kwargs)
+        out = self._jit_fn(tree_flatten((args, kwargs)))
         if array_backend != "torch":
             out = do("asarray", out, like=array_backend)
         return out
 
 
 _backend_lookup = {}
```

### Comparing `autoray-0.6.8/autoray/experimental/complexity_tracing.py` & `autoray-0.6.9/autoray/experimental/complexity_tracing.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray/experimental/complexity_tracing_example.ipynb` & `autoray-0.6.9/autoray/experimental/complexity_tracing_example.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray/lazy/__init__.py` & `autoray-0.6.9/autoray/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray/lazy/core.py` & `autoray-0.6.9/autoray/lazy/core.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray/lazy/draw.py` & `autoray-0.6.9/autoray/lazy/draw.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray/lazy/linalg.py` & `autoray-0.6.9/autoray/lazy/linalg.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/autoray.egg-info/PKG-INFO` & `autoray-0.6.9/autoray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoray
-Version: 0.6.8
+Version: 0.6.9
 Summary: Abstract your array operations.
 Home-page: http://github.com/jcmgray/autoray
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/autoray/issues
 Project-URL: Source, https://github.com/jcmgray/autoray/
```

### Comparing `autoray-0.6.8/autoray.egg-info/SOURCES.txt` & `autoray-0.6.9/autoray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/Makefile` & `autoray-0.6.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/_pygments/_pygments_dark.py` & `autoray-0.6.9/docs/_pygments/_pygments_dark.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/_pygments/_pygments_light.py` & `autoray-0.6.9/docs/_pygments/_pygments_light.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/_static/autoray-header.png` & `autoray-0.6.9/docs/_static/autoray-header.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/_static/autoray.ico` & `autoray-0.6.9/docs/_static/autoray.ico`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/_static/my-styles.css` & `autoray-0.6.9/docs/_static/my-styles.css`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/automatic_dispatch.md` & `autoray-0.6.9/docs/automatic_dispatch.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/compilation.ipynb` & `autoray-0.6.9/docs/compilation.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/conf.py` & `autoray-0.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/development.md` & `autoray-0.6.9/docs/development.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/images/autoray-readme-pic-0.png` & `autoray-0.6.9/docs/images/autoray-readme-pic-0.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/images/autoray-readme-pic-1.png` & `autoray-0.6.9/docs/images/autoray-readme-pic-1.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/index.md` & `autoray-0.6.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/installation.md` & `autoray-0.6.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/lazy_computation.ipynb` & `autoray-0.6.9/docs/lazy_computation.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/docs/make.bat` & `autoray-0.6.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/pyproject.toml` & `autoray-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/setup.py` & `autoray-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.8/tests/test_autocompile.py` & `autoray-0.6.9/tests/test_autocompile.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,30 +82,8 @@
         return a + c, b - c
 
     a = gen_rand((2, 3), "numpy")
     b = gen_rand((4, 5), "numpy")
     x, y = foo(a, b, 1)
 
     assert_allclose(x, a - b.sum() + 1)
-    assert_allclose(y, b - (a - b.sum()).sum() - 1)
-
-
-def test_static_kwargs_change():
-    @autojit
-    def foo(a, b, c):
-        if c == "sum":
-            return a + b
-        elif c == "sub":
-            return a - b
-
-    assert (
-        foo(
-            do("array", 100, like="numpy"), do("array", 1, like="numpy"), "sum"
-        )
-        == 101
-    )
-    assert (
-        foo(
-            do("array", 100, like="numpy"), do("array", 1, like="numpy"), "sub"
-        )
-        == 99
-    )
+    assert_allclose(y, b - (a - b.sum()).sum() - 1)
```

### Comparing `autoray-0.6.8/tests/test_autoray.py` & `autoray-0.6.9/tests/test_autoray.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 BACKENDS = [pytest.param("numpy")]
 for lib in ["cupy", "dask", "tensorflow", "torch", "mars", "jax", "sparse"]:
     if importlib.util.find_spec(lib):
         BACKENDS.append(pytest.param(lib))
 
         if lib == "jax":
             import os
-            from jax.config import config
+            import jax
 
-            config.update("jax_enable_x64", True)
-            config.update("jax_platform_name", "cpu")
+            jax.config.update("jax_enable_x64", True)
+            jax.config.update("jax_platform_name", "cpu")
             os.environ["XLA_PYTHON_CLIENT_ALLOCATOR"] = "platform"
     else:
         BACKENDS.append(
             pytest.param(
                 lib, marks=pytest.mark.skipif(True, reason=f"No {lib}.")
             )
         )
```

### Comparing `autoray-0.6.8/tests/test_lazy.py` & `autoray-0.6.9/tests/test_lazy.py`

 * *Files identical despite different names*

